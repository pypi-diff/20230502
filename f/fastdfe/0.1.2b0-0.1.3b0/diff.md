# Comparing `tmp/fastdfe-0.1.2b0.tar.gz` & `tmp/fastdfe-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.2b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.3b0.tar", max compression
```

## Comparing `fastdfe-0.1.2b0.tar` & `fastdfe-0.1.3b0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      316 2023-04-24 05:28:36.304713 fastdfe-0.1.2b0/README.md
--rw-r--r--   0        0        0     2649 2023-04-28 15:00:53.726538 fastdfe-0.1.2b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    15675 2023-04-28 15:54:32.817541 fastdfe-0.1.2b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    40231 2023-04-28 16:01:50.252285 fastdfe-0.1.2b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4749 2023-04-25 17:46:33.252414 fastdfe-0.1.2b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0     9520 2023-04-28 15:00:53.695766 fastdfe-0.1.2b0/fastdfe/config.py
--rw-r--r--   0        0        0    14889 2023-04-26 07:24:19.626163 fastdfe-0.1.2b0/fastdfe/discretization.py
--rw-r--r--   0        0        0     3937 2023-04-25 17:46:33.230441 fastdfe-0.1.2b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     1381 2023-04-25 17:46:33.199691 fastdfe-0.1.2b0/fastdfe/mle.py
--rw-r--r--   0        0        0    23671 2023-04-28 15:00:53.721080 fastdfe-0.1.2b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    21128 2023-04-28 15:13:39.927333 fastdfe-0.1.2b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    10986 2023-04-28 15:06:24.181963 fastdfe-0.1.2b0/fastdfe/parser.py
--rw-r--r--   0        0        0    17094 2023-04-28 15:54:32.832520 fastdfe-0.1.2b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0    35860 2023-04-28 16:01:50.239910 fastdfe-0.1.2b0/fastdfe/shared_inference.py
--rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.2b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0    31116 2023-04-28 16:01:50.255162 fastdfe-0.1.2b0/fastdfe/visualization.py
--rw-r--r--   0        0        0      642 2023-04-28 16:09:12.911964 fastdfe-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 fastdfe-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0      322 2023-05-02 08:38:16.143704 fastdfe-0.1.3b0/README.md
+-rw-r--r--   0        0        0     2590 2023-04-29 07:23:15.706767 fastdfe-0.1.3b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    17303 2023-05-02 08:38:16.179841 fastdfe-0.1.3b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    42920 2023-05-02 08:43:30.818811 fastdfe-0.1.3b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4762 2023-04-29 08:09:34.806177 fastdfe-0.1.3b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0     9585 2023-04-29 08:09:34.816833 fastdfe-0.1.3b0/fastdfe/config.py
+-rw-r--r--   0        0        0    15043 2023-04-29 08:10:05.020182 fastdfe-0.1.3b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0     3902 2023-04-29 08:09:34.792156 fastdfe-0.1.3b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     1541 2023-04-29 08:10:05.029271 fastdfe-0.1.3b0/fastdfe/mle.py
+-rw-r--r--   0        0        0    33480 2023-05-02 08:38:16.181798 fastdfe-0.1.3b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    21091 2023-05-02 08:38:16.182403 fastdfe-0.1.3b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    11316 2023-04-29 08:12:55.242293 fastdfe-0.1.3b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    12467 2023-05-02 08:38:16.183198 fastdfe-0.1.3b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5254 2023-04-29 07:57:26.449161 fastdfe-0.1.3b0/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0    36485 2023-05-02 08:49:18.285827 fastdfe-0.1.3b0/fastdfe/shared_inference.py
+-rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.3b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    30684 2023-05-02 08:38:16.185031 fastdfe-0.1.3b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0      642 2023-05-02 08:50:43.544962 fastdfe-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 fastdfe-0.1.3b0/PKG-INFO
```

### Comparing `fastdfe-0.1.2b0/fastdfe/__init__.py` & `fastdfe-0.1.3b0/fastdfe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 from .parametrization import Parametrization, GammaExpParametrization, DiscreteParametrization, \
     GammaDiscreteParametrization, DisplacedGammaParametrization
 from .config import Config
 from .abstract_inference import Inference
 from .base_inference import BaseInference, InferenceResults
 from .shared_inference import SharedInference, SharedParams
 from .optimization import Covariate
-from .polydfe import PolyDFE, PolyDFEResult
 from .visualization import Visualization
 from .spectrum import Spectrum, Spectra
 from .parser import Parser, BaseTransitionStratification, BaseContextStratification, DegeneracyStratification, \
     TransitionTransversionStratification, ReferenceBaseStratification
 
 __all__ = [
     'Parametrization',
@@ -71,15 +70,14 @@
     'DisplacedGammaParametrization',
     'Config',
     'Inference',
     'BaseInference',
     'SharedInference',
     'SharedParams',
     'Covariate',
-    'PolyDFE',
     'Visualization',
     'Spectrum',
     'Spectra',
     'Parser',
     'BaseTransitionStratification',
     'BaseContextStratification',
     'DegeneracyStratification',
```

### Comparing `fastdfe-0.1.2b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.3b0/fastdfe/abstract_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Abstract inference class and static utilities.
+"""
+
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-12"
 
 from abc import ABC, abstractmethod
 from typing import List, Optional, Literal
 from typing_extensions import Self
@@ -13,14 +17,17 @@
 
 from .bootstrap import Bootstrap
 from .parametrization import Parametrization, from_string
 from .visualization import Visualization
 
 
 class Inference:
+    """
+    Static utility methods for inference objects.
+    """
 
     @staticmethod
     def plot_discretized(
             inferences: List['AbstractInference'],
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
@@ -82,15 +89,15 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFEs',
             labels: list | np.ndarray = None,
-            scale: Literal['lin', 'log'] = 'lin',
+            scale: Literal['lin', 'log', 'symlog'] = 'lin',
             scale_density: bool = False,
             ax: plt.Axes = None,
             **kwargs
 
     ) -> plt.Axes:
         """
         Visualize several DFEs given by the list of inference objects.
@@ -135,49 +142,89 @@
             bins=intervals,
             **locals()
         )
 
     @staticmethod
     def plot_inferred_parameters(
             inferences: List['AbstractInference'],
+            labels: list | np.ndarray,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
-            labels: list | np.ndarray = None,
-            scale: Literal['lin', 'log'] = 'log',
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
             legend: bool = True,
             ax: plt.Axes = None,
             **kwargs
 
     ) -> plt.Axes:
         """
         Visualize several discretized DFEs given by the list of inference objects.
         Note that the DFE parametrization needs to be the same for all inference objects.
 
+        :param inferences: List of inference objects.
+        :param labels: Unique labels for the DFEs.
         :param scale: y-scale of the plot.
         :param legend: Whether to show a legend.
-        :param inferences: List of inference objects.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
-        :param labels: Labels for the DFEs.
         :param ax: Axes of the plot.
         :param kwargs: Additional arguments for the plot.
         :return: Axes of the plot.
+        :raises ValueError: If no inference objects are given.
         """
+        if len(inferences) == 0:
+            raise ValueError('No inference objects given.')
+
+        # get sorted list of parameter names
+        param_names = sorted(inferences[0].get_bootstrap_param_names())
+
+        if labels is None:
+            labels = list()
+
+        errors = {}
+        values = {}
+        for label, inf in zip(labels, inferences):
+
+            values[label] = list(inf.get_bootstrap_params()[k] for k in param_names)
+
+            # whether to compute errors
+            if confidence_intervals and inf.bootstraps is not None:
+
+                # use mean of bootstraps instead of original values
+                if bootstrap_type == 'percentile':
+                    values[label] = inf.bootstraps[param_names].mean().to_list()
+
+                # compute errors
+                errors[label], _ = Bootstrap.get_errors(
+                    values=values[label],
+                    bs=inf.bootstraps[param_names].to_numpy(),
+                    bootstrap_type=bootstrap_type,
+                    ci_level=ci_level
+                )
+            else:
+                errors[label] = None
+
         return Visualization.plot_inferred_parameters(
-            params=[inf.get_bootstrap_params() for inf in inferences],
-            bootstraps=[inf.bootstraps for inf in inferences],
-            **locals()
+            values=values,
+            errors=errors,
+            param_names=param_names,
+            file=file,
+            show=show,
+            title=title,
+            labels=labels,
+            scale=scale,
+            legend=len(labels) > 1,
+            ax=ax
         )
 
     @staticmethod
     def get_discretized(
             bootstraps: pd.DataFrame,
             params: dict,
             model: Parametrization,
@@ -231,15 +278,15 @@
             params: dict,
             bootstraps: pd.DataFrame,
             model: Parametrization | str,
             ci_level: float = 0.05,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
 
-    ) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray):
+    ) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray):
         """
         Compute errors and confidence interval for a discretized DFE.
 
         :param params: Parameters of the model
         :param bootstraps: Bootstrapped samples
         :param model: DFE parametrization
         :param ci_level: Confidence interval level
@@ -430,7 +477,14 @@
         Load object from file.
 
         :param classes: Classes to be used for unserialization
         :param file: File to load from
         """
         with open(file, 'r') as fh:
             return cls.from_json(fh.read(), classes)
+
+    @abstractmethod
+    def get_bootstrap_param_names(self) -> List[str]:
+        """
+        Get the names of the parameters to be included in the bootstraps.
+        """
+        pass
```

### Comparing `fastdfe-0.1.2b0/fastdfe/base_inference.py` & `fastdfe-0.1.3b0/fastdfe/base_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+Base inference class.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import copy
 import functools
 import itertools
 import json
 import logging
 import time
 from typing import List, Optional, Dict, Literal, cast
 
+import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from numpy.linalg import norm
 from scipy.optimize._optimize import OptimizeResult
 from scipy.stats import chi2
 from typing_extensions import Self
 
 from . import parametrization, optimization
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .discretization import Discretization
 from .json_handlers import CustomEncoder
-from .optimization import Optimization, flatten_dict, pack_params, expand_fixed
+from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, scale_values
 from .parametrization import Parametrization, from_string
 from .spectrum import Spectrum, Spectra
 from .spectrum import standard_kingman
 from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class BaseInference(AbstractInference):
     """
-    Base inference class for inferring the SFS given one
-    neutral and one selected SFS.
-    Note that Inference is by default seeded.
+    Base inference class for inferring the SFS given one neutral and one selected SFS.
+    Note that BaseInference is by default seeded.
 
     .. warning::
         TODO add confidence intervals for inferred SFS.
+        TODO take average of likelihood after bootstrapping?
     """
 
     #: Default parameters not connected to the DFE parametrization
     default_x0 = dict(
         eps=0.0
     )
 
     #: Default parameter bounds not connected to the DFE parametrization
     default_bounds = dict(
         eps=(0, 0.15)
     )
 
     #: Scales for the parameters not connected to the DFE parametrization
-    scales = dict(
+    default_scales = dict(
         eps='lin'
     )
 
     #: Default options for the MLE
     default_opts_mle = dict(
         # ftol=1e-20,
         # gtol=1e-20
@@ -188,21 +189,24 @@
         # expand 'all' type
         #: Fixed parameters
         self.fixed_params: Dict[str, Dict[str, float]] = expand_fixed(fixed_params, ['all'])
 
         # check that the fixed parameters are valid
         self.check_fixed_params_exist()
 
+        #: scale for all parameters
+        self.scales = self.model.scales | self.default_scales
+
         if optimization is None:
             # create optimization instance
             # merge with default values of inference and model
             #: Optimization instance
             self.optimization: Optimization = Optimization(
                 bounds=self.model.bounds | self.default_bounds | bounds,
-                scales=self.model.scales | self.scales,
+                scales=self.scales,
                 opts_mle=self.default_opts_mle | opts_mle,
                 loss_type=loss_type,
                 param_names=self.param_names,
                 parallelize=self.parallelize,
                 fixed_params=fixed_params,
                 seed=seed
             )
@@ -303,22 +307,24 @@
             return func(self, *args, **kwargs)
 
         return wrapper
 
     def run(
             self,
             do_bootstrap: bool = None,
-            pbar: bool = None
+            pbar: bool = None,
+            **kwargs
 
     ) -> Spectrum:
         """
         Perform the DFE inference.
 
         :param pbar: Whether to show a progress bar.
         :param do_bootstrap: Whether to perform bootstrapping.
+        :param kwargs: Keyword arguments.
         :return: Modelled SFS.
         """
         # check if locked
         self.raise_if_locked()
 
         # starting time of inference
         start_time = time.time()
@@ -338,14 +344,15 @@
         # parallelized so that the pre-computation does not have to be
         # performed in each thread.
         _ = self.discretization.dfe_to_sfs
 
         # perform numerical minimization
         result, params_mle = self.optimization.run(
             x0=self.x0,
+            scales=self.scales,
             get_counts=self.get_counts(),
             n_runs=self.n_runs,
             pbar=pbar
         )
 
         # normalize parameters
         params_mle['all'] = self.model.normalize(params_mle['all'])
@@ -382,17 +389,25 @@
         Get loss function.
         Note that the order of the parameters has to be the same as in
         params_mle. The types also need to be specified here. For a
         BaseInference objects, the mean we need to pass dict(all=...).
 
         :return: The likelihood.
         """
+        x0_cached = self.optimization.x0
         self.optimization.x0 = params
 
-        return -self.optimization.get_loss_function(self.get_counts())(pack_params(flatten_dict(params)))
+        # prepare parameters
+        params = pack_params(self.optimization.scale_values(flatten_dict(params)))
+
+        lk = -self.optimization.get_loss_function(self.get_counts())(params)
+
+        self.optimization.x0 = x0_cached
+
+        return lk
 
     def assign_result(self, result: OptimizeResult, params_mle: dict):
         """
         Assign optimization result and MLE parameters.
 
         :param params_mle: MLE parameters.
         :param result: Optimization result.
@@ -441,20 +456,25 @@
 
         :param kwargs: Dictionary of properties to update.
         """
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
-    def bootstrap(self, n_samples: int = None, parallelize: bool = None) -> pd.DataFrame:
+    def bootstrap(
+            self, n_samples: int = None,
+            parallelize: bool = None,
+            update_likelihood: bool = True
+    ) -> pd.DataFrame:
         """
         Perform the parametric bootstrap.
 
         :param n_samples: Number of bootstrap samples.
         :param parallelize: Whether to parallelize the bootstrap.
+        :param update_likelihood: Whether to update the likelihood to be the mean of the bootstrap samples.
         :return: Dataframe with bootstrap results.
         """
         # check if locked
         self.raise_if_locked()
 
         # perform inference first if not done yet
         self.run_if_required()
@@ -504,14 +524,18 @@
 
         # add estimates for alpha to the bootstraps
         self.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
+        # determine average likelihood of successful runs
+        if update_likelihood:
+            self.likelihood = np.mean([-res.fun for res in result[:, 0] if res.success] + [self.likelihood])
+
         return self.bootstraps
 
     def add_alpha_to_bootstraps(self):
         """
         Add estimates for alpha to the bootstraps.
         """
         logger.debug('Computing estimates for alpha.')
@@ -549,14 +573,15 @@
         # resample spectra
         sfs_sel = self.resample_sfs(self.sfs_sel)
         sfs_neut = self.resample_sfs(self.sfs_neut)
 
         # perform numerical minimization
         result, params_mle = self.optimization.run(
             x0=dict(all=self.params_mle),
+            scales=self.get_scales_linear(),
             n_runs=1,
             debug_iterations=False,
             print_info=False,
             get_counts=dict(all=lambda params: self.model_sfs(
                 params,
                 sfs_neut=sfs_neut,
                 sfs_sel=sfs_sel
@@ -564,14 +589,22 @@
         )
 
         # normalize MLE estimates
         params_mle['all'] = self.model.normalize(params_mle['all'])
 
         return result, params_mle
 
+    def get_scales_linear(self) -> Dict[str, Literal['lin']]:
+        """
+        Get linear scales for all parameters. We do this for the bootstraps as x0 should be close to MLE.
+
+        :return: Dictionary of scales.
+        """
+        return cast(Dict[str, Literal['lin']], dict((p, 'lin') for p in self.scales.keys()))
+
     def model_sfs(self, params: dict, sfs_neut: Spectrum, sfs_sel: Spectrum) -> (np.ndarray, np.ndarray):
         """
         Model the selected SFS from the given parameters.
 
         :param sfs_sel: Observed spectrum of selected sites.
         :param sfs_neut: Observed spectrum of neutral sites.
         :param params: Dictionary of parameters.
@@ -632,15 +665,15 @@
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = None,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             scale_density: bool = False,
-            scale: Literal['lin', 'log'] = 'lin',
+            scale: Literal['lin', 'log', 'symlog'] = 'lin',
             title: str = 'DFE',
             ax: plt.Axes = None
 
     ) -> plt.Axes:
         """
         Plot continuous DFE.
         The special constants np.inf and -np.inf are also valid interval bounds.
@@ -815,43 +848,68 @@
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
         self.plot_sfs_comparison(show=show)
         self.plot_continuous(show=show)
         self.plot_interval_density(show=show)
         self.plot_likelihoods(show=show)
 
+    def get_errors_discretized_dfe(
+            self,
+            ci_level: float = 0.05,
+            intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
+    ) -> np.ndarray:
+        """
+        Get the discretized DFE errors.
+
+        :param ci_level: Confidence interval level.
+        :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
+        :param bootstrap_type: Type of bootstrap to use.
+        :return: Arrays of errors, confidence intervals, bootstraps, means and values
+        """
+        return Inference.get_errors_discretized_dfe(
+            params=self.params_mle,
+            bootstraps=self.bootstraps,
+            model=self.model,
+            ci_level=ci_level,
+            intervals=intervals,
+            bootstrap_type=bootstrap_type
+        )
+
     @run_if_required_wrapper
     def plot_inferred_parameters(
             self,
-            file: str = None,
             confidence_intervals: bool = True,
-            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
+            file: str = None,
             show: bool = True,
-            title: str = 'inferred parameters',
-            scale: Literal['lin', 'log'] = 'log',
+            title: str = 'parameter estimates',
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
+            legend: bool = True,
             ax: plt.Axes = None,
             **kwargs
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
+        :param legend: Whether to show the legend.
         :param confidence_intervals: Whether to show confidence intervals.
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for the confidence intervals.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
         :return: Axes object
         """
-        return Visualization.plot_inferred_parameters(
-            params=[self.get_bootstrap_params()],
-            bootstraps=[self.bootstraps],
+        return Inference.plot_inferred_parameters(
+            inferences=[self],
+            labels=['all'],
             file=file,
             show=show,
             title=title,
             ci_level=ci_level,
             confidence_intervals=confidence_intervals,
             bootstrap_type=bootstrap_type,
             scale=scale,
@@ -860,15 +918,15 @@
 
     @run_if_required_wrapper
     def plot_likelihoods(
             self,
             file: str = None,
             show: bool = True,
             title: str = 'likelihoods',
-            scale: Literal['lin', 'log'] = 'lin',
+            scale: Literal['lin', 'log', 'symlog'] = 'lin',
             ax: plt.Axes = None,
             **kwargs
     ) -> plt.Axes:
         """
         Visualize the likelihoods of the optimization runs.
 
         :param scale: y-scale of the plot.
@@ -1065,14 +1123,22 @@
         """
         Get the parameters to be included in the bootstraps.
 
         :return: Parameters to be included in the bootstraps.
         """
         return self.params_mle | dict(alpha=self.alpha)
 
+    def get_bootstrap_param_names(self) -> List[str]:
+        """
+        Get the parameters to be included in the bootstraps.
+
+        :return: Parameters to be included in the bootstraps.
+        """
+        return list(self.get_bootstrap_params().keys())
+
     def get_optimized_param_names(self) -> List[str]:
         """
         Get the parameters names for the parameters that are optimized.
 
         :return: List of parameter names.
         """
         return list(set(flatten_dict(self.get_x0())) - set(flatten_dict(self.fixed_params)))
@@ -1164,14 +1230,23 @@
 
         :param params: Fixed parameters.
         """
         self.fixed_params = expand_fixed(params, ['all'])
 
         self.optimization.set_fixed_params(self.fixed_params)
 
+    def to_json(self) -> str:
+        """
+        Serialize object.
+
+        :return: JSON string
+        """
+        # using make_ref=True resulted in weird behaviour when unserializing.
+        return jsonpickle.encode(self, indent=4, warn=True, make_refs=False)
+
 
 class InferenceResults:
     def __init__(self, inference: BaseInference):
         """
         Inference results.
 
         :param inference: Inference object.
```

### Comparing `fastdfe-0.1.2b0/fastdfe/bootstrap.py` & `fastdfe-0.1.3b0/fastdfe/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+Bootstrap utilities.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
@@ -13,14 +13,18 @@
 from scipy.stats import norm as normal
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class Bootstrap:
+    """
+    Bootstrap utilities.
+    """
+
     @staticmethod
     def get_bounds_from_quantile(data: list | np.ndarray, a1: float, a2: float, n: int) -> (float, float):
         """
         Get confidence interval bounds.
 
         :param data: Sorted data
         :param a1: Lower quantile
```

### Comparing `fastdfe-0.1.2b0/fastdfe/config.py` & `fastdfe-0.1.3b0/fastdfe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+Configuration class.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import json
@@ -12,22 +12,24 @@
 
 import yaml
 
 from .json_handlers import CustomEncoder
 from .optimization import Covariate
 from .optimization import SharedParams, merge_dicts
 from .parametrization import Parametrization, from_string, to_string
-from .polydfe import parse_init_file, models, create_sfs_config, create_init_file
+from .polydfe_utils import create_sfs_config, parse_init_file, create_init_file, models
 from .spectrum import Spectra, parse_polydfe_sfs_config
 
 logger = logging.getLogger('fastdfe')
 
+
 class Config:
     """
-    Configuration class to be used for Inference and polyDFE.
+    Configuration class to be used for :class:``~fastdfe.base_inference.BaseInference`` and
+    :class:``fastdfe.shared_inference.SharedInference``.
     """
 
     def __init__(
             self,
             polydfe_spectra_config: str = None,
             polydfe_init_file: str = None,
             polydfe_init_file_id: int = 1,
```

### Comparing `fastdfe-0.1.2b0/fastdfe/discretization.py` & `fastdfe-0.1.3b0/fastdfe/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+Discretization of DFE to SFS transformation.
+"""
+
+__author__ = "Janek Sendrowski"
+__contact__ = "sendrowski.janek@gmail.com"
+__date__ = "2023-02-26"
+
 import logging
 from functools import cached_property, wraps
 from typing import Literal
 
 import mpmath as mp
 import numpy as np
 from scipy.integrate import quad
```

### Comparing `fastdfe-0.1.2b0/fastdfe/json_handlers.py` & `fastdfe-0.1.3b0/fastdfe/json_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+JSON handlers.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import json
```

### Comparing `fastdfe-0.1.2b0/fastdfe/mle.py` & `fastdfe-0.1.3b0/fastdfe/mle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,25 @@
+"""
+MLE utilities.
+"""
+
+__author__ = "Janek Sendrowski"
+__contact__ = "sendrowski.janek@gmail.com"
+__date__ = "2023-02-26"
+
 import numpy as np
 from typing import Union
 from scipy.special import factorial
 
 
 class MLE:
+    """
+    MLE utilities.
+    """
+
     @staticmethod
     def log_poisson(mu, k):
         """
         Compute log(Poisson(mu, k)).
 
         :param mu: Mean of Poisson distribution
         :param k: Number of events
```

### Comparing `fastdfe-0.1.2b0/fastdfe/optimization.py` & `fastdfe-0.1.3b0/fastdfe/optimization.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+Optimization module.
+"""
+
+__author__ = "Janek Sendrowski"
+__contact__ = "sendrowski.janek@gmail.com"
+__date__ = "2023-02-26"
+
 import copy
 import logging
 from dataclasses import dataclass
 from typing import Callable, List, Dict, Literal, Tuple, Optional
 
 import multiprocess as mp
 import numpy as np
@@ -91,29 +99,29 @@
 
         # assign value to the final subkey
         subdict[subkeys[-1]] = value if not isinstance(value, dict) else unflatten_dict(value, separator)
 
     return res
 
 
-def unpack_params(x: np.ndarray, original: Dict[str, dict]) -> Dict[str, dict]:
+def unpack_params(x: np.ndarray, original: Dict[str, dict | tuple | float]) -> Dict[str, dict | tuple | float]:
     """
     Unpack params from numpy array. This is the inverse of pack_params and is used
     as scipy.optimize.minimize only accepts numpy arrays as parameters.
 
     :param x: Numpy array
     :param original: Original dictionary
     :return: Unpacked dictionary
     """
     keys = flatten_dict(original).keys()
 
     return unflatten_dict(dict(zip(keys, x)))
 
 
-def pack_params(params: Dict[str, dict]) -> np.ndarray:
+def pack_params(params: Dict[str, dict | tuple | float]) -> np.ndarray:
     """
     Pack params into numpy array. This is used as scipy.optimize.minimize only accepts
     numpy arrays as parameters. This is the inverse of unpack_params.
 
     :param params: Dictionary to pack
     :return: numpy array
     """
@@ -325,14 +333,239 @@
     # evaluate counts for each type
     for key in get_counts.keys():
         counts[key] = get_counts[key](unpacked[key])
 
     return counts
 
 
+def to_symlog(x: float, linthresh: float = 1e-5) -> float:
+    """
+    Convert a value to the symlog scale.
+
+    :param x: The input value on the original scale.
+    :param linthresh: The positive value that determines the range within which the
+                      symlog scale is linear. Must be greater than 0.
+    :return: The value on the symlog scale.
+    """
+    sign = np.sign(x)
+    abs_x = np.abs(x)
+    log_x = np.log10(abs_x + linthresh) - np.log10(linthresh)
+
+    return sign * (abs_x / linthresh if abs_x <= linthresh else log_x)
+
+
+def from_symlog(y: float, linthresh: float = 1e-5) -> float:
+    """
+    Convert a value from the symlog scale back to the original scale.
+
+    :param y: The input value on the symlog scale.
+    :param linthresh: The positive value that determines the range within which the
+                      symlog scale is linear. Must be greater than 0.
+    :return: The value on the original scale.
+    """
+    sign = np.sign(y)
+    abs_y = np.abs(y)
+    exp_y = np.power(10, abs_y + np.log10(linthresh)) - linthresh
+
+    return sign * (abs_y * linthresh if abs_y <= 1 else exp_y)
+
+
+def scale_bound(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']):
+    """
+    Convert a bound to the specified scale. For symlog scale we assume the symmetric bounds,
+    so that the upper bound denotes the boundaries and the lower bound the linear threshold.
+
+    :param bounds: The bound to convert
+    :param scale: The scale to convert to
+    :return: The converted bound
+    :raises ValueError: if the scale is unknown
+    """
+    if scale == 'lin':
+        return bounds
+
+    if scale == 'log':
+        if bounds[1] < 0:
+            return -np.log10(-bounds[0]), -np.log10(-bounds[1])
+
+        if bounds[0] > 0:
+            return np.log10(bounds[0]), np.log10(bounds[1])
+
+        raise ValueError('Bounds must not span zero for log scale.')
+
+    if scale == 'symlog':
+
+        if bounds[0] <= 0 or bounds[1] <= 0:
+            raise ValueError('Both bounds must be positive for symlog scale.')
+
+        return to_symlog(-bounds[1], linthresh=bounds[0]), to_symlog(bounds[1], linthresh=bounds[0])
+
+    raise ValueError(f'Unknown scale {scale}.')
+
+
+def unscale_bound(
+        scaled_bounds: Tuple[float, float],
+        scale: Literal['lin', 'log', 'symlog'],
+        linthresh: float = 1e-5
+) -> Tuple[float, float]:
+    """
+    Convert a bound from the specified scale back to the original scale. For symlog scale,
+    we assume symmetric bounds, so that the upper bound denotes the boundaries and
+    the lower bound the linear threshold, i.e. ``bounds = (-bounds[1], bounds[1])`` and ``linthresh = bounds[0]``.
+    Note that we cannot reliably recover negative bounds that were log scaled.
+
+    :param linthresh:
+    :param scaled_bounds: The bound to convert
+    :param scale: The scale to convert from
+    :return: The converted bound
+    :raises ValueError: if the scale is unknown
+    """
+    if scale == 'lin':
+        return scaled_bounds
+
+    if scale == 'log':
+        return np.power(10, scaled_bounds[0]), np.power(10, scaled_bounds[1])
+
+    if scale == 'symlog':
+        upper_bound = from_symlog(scaled_bounds[1], linthresh=linthresh)
+
+        return linthresh, upper_bound
+
+    raise ValueError(f'Unknown scale {scale}.')
+
+
+def scale_bounds(
+        bounds: Dict[str, Tuple[float, float]],
+        scales: Dict[str, Literal['lin', 'log', 'symlog']]
+) -> Dict[str, Tuple[float, float]]:
+    """
+    Convert bounds to the specified scale. For symlog scale we assume the symmetric bounds,
+    so that the upper bound denotes the boundaries and the lower bound the linear threshold.
+
+    :param bounds: Flattened dictionary of bounds to convert index by type and parameter
+    :param scales: Dictionary of scales indexed by parameter
+    :return: The converted bounds
+    :raises ValueError: if the scale is unknown
+    """
+    scaled_bounds = {}
+
+    for key, value in bounds.items():
+        scaled_bounds[key] = scale_bound(value, scale=scales[get_basename(key)])
+
+    return scaled_bounds
+
+
+def scale_value(value: float, bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> float:
+    """
+    Convert a value to the specified scale. For symlog scale, the untransformed bounds are needed,
+    so that the upper bound denotes the boundaries and the lower bound the linear threshold.
+
+    :param value: The value to convert.
+    :param bounds: The untransformed bounds for the symlog scale.
+    :param scale: The scale to convert to.
+    :return: The converted value.
+    :raises ValueError: if the scale is unknown.
+    """
+    if scale == 'lin':
+        return value
+
+    if scale == 'log':
+
+        if value < 0:
+            return -np.log10(-value)
+
+        return np.log10(value)
+
+    if scale == 'symlog':
+        return to_symlog(value, linthresh=bounds[0])
+
+    raise ValueError(f'Unknown scale {scale}.')
+
+
+def unscale_value(scaled_value: float, bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> float:
+    """
+    Convert a value from the specified scale back to the original scale. For symlog scale,
+    the untransformed bounds are needed, so that the upper bound denotes the boundaries
+    and the lower bound the linear threshold.
+
+    :param scaled_value: The value to convert.
+    :param bounds: The untransformed bounds for the symlog scale.
+    :param scale: The scale to convert from.
+    :return: The converted value.
+    :raises ValueError: if the scale is unknown.
+    """
+    if scale == 'lin':
+        return scaled_value
+
+    if scale == 'log':
+
+        if bounds[1] < 0:
+            return -np.power(10, -scaled_value)
+
+        return np.power(10, scaled_value)
+
+    if scale == 'symlog':
+        return from_symlog(scaled_value, linthresh=bounds[0])
+
+    raise ValueError(f'Unknown scale {scale}.')
+
+
+def scale_values(
+        params: Dict[str, Dict[str, float]],
+        bounds: Dict[str, Tuple[float, float]],
+        scales: Dict[str, Literal['lin', 'log', 'symlog']]
+) -> Dict[str, Dict[str, float]]:
+    """
+    Scale values according to the given scales.
+
+    :param params: Nested dictionary of parameters indexed by type and parameter
+    :param scales: Dictionary of scales indexed by parameter name
+    :param bounds: Dictionary of bounds indexed by parameter name
+    :return: Nested dictionary of scaled parameters indexed by type and parameter
+    """
+    scaled = {}
+
+    for key, value in flatten_dict(params).items():
+        # scale value
+        scaled[key] = scale_value(value, bounds[get_basename(key)], scales[get_basename(key)])
+
+    return unflatten_dict(scaled)
+
+
+def unscale_values(
+        params: Dict[str, Dict[str, float]],
+        bounds: Dict[str, Tuple[float, float]],
+        scales: Dict[str, Literal['lin', 'log', 'symlog']]
+) -> Dict[str, Dict[str, float]]:
+    """
+    Unscale values according to the given scales.
+
+    :param params: Nested dictionary of parameters indexed by type and parameter
+    :param scales: Dictionary of scales indexed by parameter name
+    :param bounds: Dictionary of scales indexed by parameter name
+    :return: Nested dictionary of unscaled parameters indexed by type and parameter
+    """
+    unscaled = {}
+
+    for key, value in flatten_dict(params).items():
+        # unscale value
+        unscaled[key] = unscale_value(value, bounds[get_basename(key)], scales[get_basename(key)])
+
+    return unflatten_dict(unscaled)
+
+
+def get_basename(name: str) -> str:
+    """
+    Get the basename of parameter string, i.e. type.param -> param.
+
+    :param name: The string to get the basename from.
+    :return: The basename.
+    """
+    return name.split('.')[-1]
+
+
 @dataclass
 class SharedParams:
     """
     Class specifying the sharing of params among types.
     'all' means all available types or params.
     """
     #: The params to share
@@ -345,36 +578,33 @@
 @dataclass
 class Covariate:
     """
     Class defining a covariate which induces a relationship
     with one or many parameters. The relationship is defined
     by a callback function which modifies the parameters. The
     default callback introduces a linear relationship.
-
-    .. warning::
-        TODO let covariate vary on log scale?
     """
 
     #: The parameter to modify
     param: str
 
     #: The values of the covariate for each type
     values: Dict[str, float]
 
     #: The callback function to modify the parameters
     callback: Optional[Callable] = None
 
     #: The bounds of the covariate parameter to be estimated
-    bounds: tuple = (-10, 10)
+    bounds: tuple = (1e-4, 1e4)
 
     #: The initial value of the covariate
     x0: float = 0
 
-    # the scale of the bounds
-    bounds_scale: Literal['lin', 'log'] = 'lin'
+    #: The scale of the bounds. See :func:`scale_value` for details.
+    bounds_scale: Literal['lin', 'log', 'symlog'] = 'symlog'
 
     def __post_init__(self):
         """
         Cast bounds to tuple and check if an inverse_callback is provided
         when a custom callback is specified.
         """
         self.bounds = tuple(self.bounds)
@@ -417,30 +647,31 @@
     """
     Class for optimizing the DFE.
     """
 
     def __init__(
             self,
             bounds: Dict[str, tuple],
-            scales: dict,
             param_names: List[str],
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             parallelize: bool = True,
             fixed_params: Dict[str, Dict[str, float]] = {},
+            scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             seed: int = None
     ):
         """
         Create object.
 
         :param parallelize: Whether to parallelize the optimization
         :param bounds: Dictionary of bounds
         :param opts_mle: Dictionary of options for the optimizer
         :param loss_type: Type of loss function to use
         :param fixed_params: Dictionary of fixed parameters
+        :param scales: Dictionary of scales
         :param param_names: List of parameter names
         """
         self.bounds = bounds
         self.scales = scales
 
         self.opts_mle = opts_mle
         self.loss_type = loss_type
@@ -467,33 +698,38 @@
         # get a random generator instance
         self.rng = np.random.default_rng(seed=seed)
 
     def run(
             self,
             get_counts: Dict[str, Callable],
             x0: Dict[str, Dict[str, float]] = {},
+            scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             n_runs: int = 1,
             debug_iterations: bool = True,
             print_info: bool = True,
             pbar: bool = None
     ) -> (OptimizeResult, dict):
         """
         Perform the optimization procedure.
 
+        :param scales: Scales of the parameters
         :param pbar: Whether to show a progress bar
         :param print_info: Whether to inform the user about the bounds
         :param n_runs: Number of optimization runs
         :param x0: Dictionary of initial values
         :param get_counts: Dictionary of functions to evaluate counts for each type
         :param debug_iterations: Whether to print debug messages for each iteration
         :return: The optimization result and the likelihoods
         """
         # number of optimization runs
         self.n_runs = n_runs
 
+        # store the scales of the parameters
+        self.scales = scales
+
         # filter out unneeded values
         # this also holds the fixed parameters
         self.x0 = filter_dict(x0, self.param_names)
 
         # flatten initial values
         flattened = flatten_dict(self.x0)
 
@@ -512,31 +748,31 @@
 
         # correct initial values to be within bounds
         self.x0 = unflatten_dict(correct_values(flattened, self.bounds, warn=True))
 
         # determine parameter bounds
         bounds = self.get_bounds(flatten_dict(self.x0))
 
-        def optimize(x0: Dict[str, dict]) -> OptimizeResult:
+        def optimize(x0: Dict[str, Dict[str, float]]) -> OptimizeResult:
             """
             Perform numerical minimization.
 
             :param x0: Initial values
             :return: Optimization result
             """
             logger.debug(f"Initial parameters: {x0}.")
 
             return minimize(
                 fun=self.get_loss_function(
                     get_counts=get_counts,
                     print_debug=debug_iterations
                 ),
-                x0=pack_params(x0),
+                x0=pack_params(self.scale_values(x0)),
                 method="L-BFGS-B",
-                bounds=pack_params(bounds),
+                bounds=pack_params(scale_bounds(bounds, self.scales)),
                 options=self.opts_mle
             )
 
         # initial parameters for the samples
         initial_params = [self.x0] + [self.sample_x0(self.x0) for _ in range(self.n_runs - 1)]
 
         # parallelize MLE for different initializations
@@ -547,23 +783,35 @@
 
         # get result with the lowest likelihood
         result = results[np.argmax(self.likelihoods)]
 
         # unpack MLE params array into a dictionary
         params_mle = unpack_params(result.x, self.x0)
 
+        # unscale parameters
+        params_mle = unscale_values(params_mle, self.bounds, self.scales)
+
         # check if the MLE reached one of the bounds
         if print_info:
             self.check_bounds(flatten_dict(params_mle))
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         return result, params_mle
 
+    def scale_values(self, x0: Dict[str, Dict[str, float]]) -> Dict[str, Dict[str, float]]:
+        """
+        Scale the values of the parameters.
+
+        :param x0: Dictionary of initial values
+        :return: Dictionary of scaled initial values
+        """
+        return scale_values(x0, self.bounds, self.scales)
+
     def get_loss_function(
             self,
             get_counts: Dict[str, Callable],
             print_debug: bool = True
     ) -> Callable:
         """
         Get the loss function.
@@ -576,17 +824,20 @@
         def loss(x: np.ndarray) -> float:
             """
             The loss function.
 
             :param x: Parameters
             :return: The loss
             """
-            # unpack parameters into dictionary use the keys of self.x0
+            # unpack parameters into dictionary using the keys of self.x0
             params = unpack_params(x, self.x0)
 
+            # unscale parameters
+            params = unscale_values(params, self.bounds, self.scales)
+
             # Model SFS from parameters.
             # Here the order of types does not matter.
             # We only collect the counts for types that are
             # given in get_counts. This makes it possible to
             # avoid specifying type 'all' which is of no use
             # in joint inference.
             counts_dict = evaluate_counts(get_counts, params)
@@ -637,56 +888,83 @@
                 sample[key] = self.sample_x0(value)
             else:
                 sample[key] = self.sample_value(self.bounds[key], self.scales[key])
 
         return sample
 
     @staticmethod
-    def sample_value(bounds: Tuple[float, float], scale: Literal['lin', 'log']) -> float:
+    def sample_value(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> float:
         """
         Sample a value between given bounds using the given scaling.
         This function works for positive, negative, and mixed bounds.
+        Note that when ``scale == 'symlog'``, ``bounds[0]`` defines the linear threshold and
+        the actual bounds are ``(-bounds[1], bounds[1])``.
 
         :param bounds: Tuple of lower and upper bounds
         :param scale: Scaling of the parameter.
         :return: Sampled value
         """
 
         def flip(bounds: Tuple[float, float]) -> Tuple[float, float]:
+            """
+            Flip the bounds.
+
+            :param bounds:
+            :return: flipped bounds
+            """
             return -bounds[1], -bounds[0]
 
+        def symlog_rvs(lower: float, upper: float) -> float:
+            """
+            Sample from a symmetric log-uniform distribution.
+
+            :param lower: lower bound which is the linear threshold
+            :param upper: upper bound so that the actual bounds are (-upper, upper)
+            :return: sampled value
+            """
+            val = loguniform.rvs(lower, upper)
+
+            # flip sign with 50% probability
+            return val if uniform.rvs() < 0.5 else -val
+
+        # dictionary of scaling functions
         scaling_functions = {
             'lin': uniform.rvs,
-            'log': loguniform.rvs
+            'log': loguniform.rvs,
+            'symlog': symlog_rvs
         }
 
         # raise an error if the scale is not valid
         if scale not in scaling_functions:
             raise ValueError(f"Scale must be one of: {', '.join(scaling_functions.keys())}")
 
         # raise an error if bounds span 0 and scale is 'log'
         if bounds[0] < 0 < bounds[1] and scale == 'log':
-            raise ValueError('Log scale not possible for bounds that span 0.')
+            raise ValueError(f"Log scale not possible for bounds that span 0.")
+
+        # raise an error if bounds are negative and scale is 'symlog'
+        if bounds[0] < 0 and scale == 'symlog':
+            raise ValueError(f"Symlog scale not possible for negative bounds.")
 
         # flip bounds if they are negative
         flipped = bounds[0] < 0
         if flipped:
             bounds = flip(bounds)
 
         # sample a value using the appropriate scaling function
         sample = scaling_functions[scale](bounds[0], bounds[1] - bounds[0])
 
         # return the sampled value, flipping back if necessary
         return -sample if flipped else sample
 
-    def get_bounds(self, x0: dict) -> dict:
+    def get_bounds(self, x0: Dict[str, float]) -> Dict[str, Tuple[float, float]]:
         """
         Get a nested dictionary of bounds the same structure as the given initial values.
 
-        :param x0: Initial values
+        :param x0: Flattened dictionary of initial values
         :return: A dictionary of initial values
         """
         bounds = {}
 
         for key, value in x0.items():
 
             # check if the parameter is fixed
```

### Comparing `fastdfe-0.1.2b0/fastdfe/parametrization.py` & `fastdfe-0.1.3b0/fastdfe/parametrization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+DFE parametrizations.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import logging
@@ -62,15 +62,15 @@
     #: Scales over which to optimize the parameters, either 'log' or 'lin'
     scales = {}
 
     def __init__(self):
         """
         Initialize parametrization.
         """
-        # determine argument names
+        #: argument names
         self.param_names: List = list(self.x0.keys())
 
     @staticmethod
     def accepts_scalars(func: Callable) -> Callable[[np.ndarray | float], np.ndarray | float]:
         """
         Make func accept scalar values.
```

### Comparing `fastdfe-0.1.2b0/fastdfe/parser.py` & `fastdfe-0.1.3b0/fastdfe/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,42 @@
+"""
+Parser module.
+"""
+
+__author__ = "Janek Sendrowski"
+__contact__ = "sendrowski.janek@gmail.com"
+__date__ = "2023-03-26"
+
 import gzip
 import itertools
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Callable, Literal, Optional
+from typing import List, Callable, Literal, Optional, TextIO
 
 import numpy as np
 from cyvcf2 import VCF, Variant
 from pyfaidx import Fasta
 from tqdm import tqdm
 
 from .spectrum import Spectra
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
+#: the DNA bases
+bases = ["A", "C", "G", "T"]
+
 
 class NoTypeException(BaseException):
     """
     Exception thrown when no type can be determined.
     """
     pass
 
 
-# the DNA bases
-bases = ["A", "C", "G", "T"]
-
-
 class Stratification(ABC):
     """
     Abstract class for Stratifying the SFS by determining
     a site's type based on its properties.
     """
 
     @abstractmethod
@@ -257,21 +264,29 @@
 
         # get a random generator instance
         self.rng = np.random.default_rng(seed=seed)
 
         self.sfs = self.create_sfs_dictionary()
 
     @staticmethod
-    def open_file(file: str):
+    def open_file(file: str) -> TextIO:
+        """
+        Open a file, either gzipped or not.
+        :param file:
+        :return: stream
+        """
         if file.endswith('.gz'):
             return gzip.open(file, "rt")
 
         return open(file, 'r')
 
     def count_lines_vcf(self):
+        """
+        Count the number of sites in the VCF file.
+        """
         from . import disable_pbar
 
         i = 0
 
         logger.info('Counting number of sites.')
 
         with self.open_file(self.vcf_file) as f:
```

### Comparing `fastdfe-0.1.2b0/fastdfe/polydfe.py` & `fastdfe-0.1.3b0/fastdfe/polydfe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,211 +1,46 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+polyDFE wrapper utilities.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import copy
 import json
 import logging
-import os
 import subprocess
 import tempfile
 import time
-from typing import Callable, List, Optional, TextIO, Literal
+from typing import Callable, List, Optional, Literal
 
 import numpy as np
 import pandas as pd
 import rpy2.robjects as ro
 from matplotlib import pyplot as plt
 from rpy2.robjects.packages import importr
 from rpy2.robjects.vectors import ListVector
 from typing_extensions import Self
 
-from . import config
-from .abstract_inference import AbstractInference
+from .abstract_inference import AbstractInference, Inference
+from .config import Config
 from .parametrization import from_string, Parametrization, DiscreteParametrization
-from .spectrum import Spectrum
-from .visualization import Visualization
+from .polydfe_utils import create_sfs_config, models
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
-# model mapping
-models = dict(
-    DisplacedGammaParametrization='A',
-    GammaDiscreteParametrization='B',
-    GammaExpParametrization='C',
-    DiscreteParametrization='D'
-)
 
-
-def create_sfs_config(
-        file: str,
-        sfs_neut: Spectrum,
-        sfs_sel: Spectrum
-):
-    """
-    Create a sfs config file for polyDFE.
-
-    :param sfs_sel: Selected sfs
-    :param sfs_neut: Neutral sfs
-    :param file: Path to config file
-    """
-
-    def write_line(f: TextIO, sfs: Spectrum, sep: str = '\t'):
-        """
-        Concatenate given array and write to stream.
-
-        :param sfs: SFS
-        :param f: File stream
-        :param sep: separator
-        """
-        # SFS and number of mutational target sites
-        # we ignore divergence data here
-        data = list(sfs.polymorphic) + [sfs.n_sites]
-
-        f.write(sep.join(map(str, data)) + os.linesep)
-
-    # number of spectra per time
-    m_neut = 1
-    m_sel = 1
-    with open(file, 'w') as fh:
-        fh.write(' '.join(map(str, [m_neut, m_sel, sfs_sel.n])) + os.linesep)
-
-        write_line(fh, sfs_neut)
-        write_line(fh, sfs_sel)
-
-
-def parse_init_file(
-        dfe_params: list,
-        file: str,
-        id: int = 1,
-        ignore: list = ['eps_deprecated', 'r']
-) -> (dict, dict):
-    """
-    Parse polyDFE init file.
-    This will define the initial parameters and
-    which ones will be held fixed during the optimization.
-    We do not support fixing some of the polyDFE's parameters
-    like theta and the nuisance parameters. Some other parameters
-    are not supported altogether.
-
-    :param dfe_params: List of dfe parameters
-    :param file: Path to init file
-    :param id: Init id
-    :param ignore: List of parameters to ignore
-    :return Dictionary of fixed parameters and dictionary of initial values
-    """
-    logger.info('Parsing init file.')
-
-    # columns except for nuisance parameters
-    columns = PolyDFE.columns + list(dfe_params)
-
-    # load init file into dataframe
-    df = pd.read_csv(file, delimiter=r"\s+", comment='#', header=None, index_col=0)
-
-    # check if id is present
-    if id not in df.index:
-        raise Exception(f'Id {id} not found in init file. Possible ids: {str(df.index.to_list())}.')
-
-    # extract row with specified id
-    data = df.loc[id]
-
-    # Retrieve parameters and their modes.
-    # Note that the parameter order is important
-    # when recreating the init file.
-    params, params_mode = {}, {}
-    for i, col in enumerate(columns):
-        params[col] = data[2 * i + 2]
-        params_mode[col] = int(data[2 * i + 1])
-
-    # assign nuisance parameters
-    params['r'] = list(data[2 * len(columns) + 1:])
-    params_mode['r'] = int(data[2 * len(columns) + 1])
-
-    # determine fixed parameters and initial conditions
-    fixed_params = {}
-    x0 = {}
-    for param in params_mode.keys():
-        if param not in ignore:
-            # here we don't distinguish between shared and independent parameters
-            if params_mode[param] == PolyDFE.ParamMode.fixed:
-                fixed_params[param] = params[param]
-
-            x0[param] = params[param]
-
-    # issue notice
-    logger.info(f"Found initial params: {x0} and fixed params: {fixed_params} when parsing init file.")
-
-    return fixed_params, x0
-
-
-def create_init_file(
-        file: str,
-        fixed_params: List,
-        x0: dict,
-        dfe_params: List,
-        n: int,
-        id: int = 1
-):
+class PolyDFEResult:
     """
-    Create an init file for polyDFE.
-
-    :param id: Init id
-    :param n: SFS sample size
-    :param dfe_params: List of dfe parameters
-    :param x0: Dictionary of initial values
-    :param fixed_params: List of fixed parameters
-    :param file: File path to write init file to
+    Class for parsing polyDFE output.
     """
-    columns = PolyDFE.columns + list(dfe_params) + ['r']
-
-    # copy dict to avoid modification
-    x0 = x0.copy()
-
-    if 'r' in x0:
-        # assign existing nuisance parameters
-        x0['r'] = ' '.join([str(r) for r in x0['r']])
-    else:
-        # make up initial nuisance parameters
-        x0['r'] = ' '.join(['1'] * (n - 1))
-
-    # create list of initial parameters
-    params = []
-    for col in columns:
-        if col in x0:
-            params += [x0[col]]
-        else:
-            params += [0]
-
-    # create list of parameter modes
-    params_mode = []
-    for col in columns:
-        if col in fixed_params:
-            params_mode += [PolyDFE.ParamMode.fixed]
-        else:
-            params_mode += [PolyDFE.ParamMode.independent]
-
-    # concatenate parameters and their modes
-    params_with_mode = [str(a) + ' ' + str(b) for a, b in zip(list(params_mode), params)]
-
-    # prepend an id value and join
-    line = '\t'.join([str(id)] + params_with_mode)
-
-    # write line to file
-    with open(file, 'w') as fh:
-        fh.write(line)
-
-
-class PolyDFEResult:
     # default postprocessing source
-    default_postprocessing_source = 'resources/polydfe/postprocessing/script.R'
+    default_postprocessing_source = '../resources/polydfe/postprocessing/script.R'
 
     # mapping of polyDFE params to new name
     param_mapping = dict(
         eps_an='eps'
     )
 
     def __init__(
@@ -309,35 +144,20 @@
         with open(file, 'w') as fh:
             fh.write(self.to_json())
 
 
 class PolyDFE(AbstractInference):
     """
     polyDFE wrapper.
+
+    Note that this class has dependencies outside of pip.
     Currently only model C is fully implemented.
     """
 
-    # leading column names in init file
-    columns = [
-        'eps',
-        'eps_deprecated',
-        'lambda',
-        'theta_bar',
-        'a'
-    ]
-
-    class ParamMode:
-        """
-        Parameter modes in polyDFE input files.
-        """
-        independent = 0
-        fixed = 1
-        shared = 2
-
-    def __init__(self, config: 'config.Config'):
+    def __init__(self, config: Config):
         """
         Create polyDFE wrapper.
 
         :param config: Config object
         """
         super().__init__()
 
@@ -362,29 +182,27 @@
 
         :param model: polyDFE model name
         :return: Native model name
         """
         return {v: k for k, v in models.items()}[model]
 
     @classmethod
-    def from_config(cls, config: 'Config') -> Self:
+    def from_config(cls, config: Config) -> Self:
         """
         Load from config object.
 
         :param config: Config object
         """
         return cls(config)
 
     @classmethod
     def from_config_file(cls, file: str) -> Self:
         """
         Load from config object.
         """
-        from fastdfe import Config
-
         return cls.from_config(Config.from_file(file))
 
     def run(
             self,
             output_file: str,
             bin: str = 'polydfe',
             wd: str = None,
@@ -448,15 +266,15 @@
             output_file=output_file,
             additional_data=dict(execution_time=self.execution_time),
             postprocessing_source=postprocessing_source
         )
 
         return self.summary
 
-    def create_bootstrap(self) -> 'config.Config':
+    def create_bootstrap(self) -> Config:
         """
         Create a bootstrap sample using polyDFE's resampling.
 
         :return: Config object
         """
         if self.summary is None:
             raise Exception('PolyDFE needs to be run before creating bootstrap samples.')
@@ -505,36 +323,48 @@
         Plot everything.
         """
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
 
     def plot_inferred_parameters(
             self,
+            confidence_intervals: bool = True,
+            ci_level: float = 0.05,
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
-            scale: Literal['lin', 'log'] = 'log',
-            ax: plt.Axes = None
+            title: str = 'parameter estimates',
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
+            legend: bool = True,
+            ax: plt.Axes = None,
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: Scale of the y-axis
+        :param legend: Show legend
+        :param ax: Axes object
+        :param title: Title of the plot
+        :param show: Show the plot
         :param file: File to save the plot to
         :param show: Show the plot
         :param ax: Axes object
         :return: Axes object
         """
-        param_names = self.get_bootstrap_param_names()
-
-        return Visualization.plot_inferred_parameters(
-            params=[self.get_bootstrap_params()],
-            bootstraps=[self.bootstraps[param_names]] if self.bootstraps is not None else [None],
-            scale=scale,
+        return Inference.plot_inferred_parameters(
+            inferences=[self],
+            labels=['all'],
+            confidence_intervals=confidence_intervals,
+            ci_level=ci_level,
+            bootstrap_type=bootstrap_type,
             file=file,
             show=show,
+            title=title,
+            legend=legend,
+            scale=scale,
             ax=ax
         )
 
     def get_bootstrap_param_names(self) -> List[str]:
         """
         Parameter names for parameters included in bootstraps.
```

### Comparing `fastdfe-0.1.2b0/fastdfe/shared_inference.py` & `fastdfe-0.1.3b0/fastdfe/shared_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Shared inference module.
+"""
+
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import copy
 import functools
 import logging
@@ -153,21 +157,24 @@
 
         # check that the fixed parameters are valid
         self.check_fixed_params_exist()
 
         # check if the fixed parameters are compatible with the shared parameters
         self.check_no_shared_params_fixed()
 
+        # scales for all parameters
+        self.scales = self.model.scales | self.default_scales | scales_cov
+
         # create optimization instance for joint inference
         # take initial values and bounds from marginal inferences
         # and from this inference for type 'all'
         #: Joint optimization instance
         self.optimization: Optimization = Optimization(
             bounds=self.model.bounds | self.default_bounds | bounds | bounds_cov,
-            scales=self.model.scales | self.scales | scales_cov,
+            scales=self.scales,
             opts_mle=self.optimization.opts_mle,
             loss_type=self.optimization.loss_type,
             param_names=self.model.param_names + ['eps'] + args_cov,
             parallelize=self.parallelize,
             fixed_params=self.fixed_params,
             seed=self.seed
         )
@@ -293,21 +300,23 @@
 
             # add to shared parameters
             self.shared_params.append(SharedParams(params=cov_but_not_shared, types=self.types))
 
     def run(
             self,
             do_bootstrap: bool = None,
-            pbar: bool = True
+            pbar: bool = True,
+            **kwargs
     ) -> Spectrum:
         """
         Run inference.
 
         :param do_bootstrap: Whether to perform bootstrapping.
         :param pbar: Whether to show progress bar.
+        :param kwargs: Additional keyword arguments passed to
         :return: Modelled SFS.
         """
 
         # run marginal optimization
         self.run_marginal()
 
         # run joint optimization
@@ -390,14 +399,15 @@
 
         # starting time of joint inference
         start_time = time.time()
 
         # Perform joint optimization.
         self.result, self.params_mle = self.optimization.run(
             x0=self.get_x0(),
+            scales=self.scales,
             n_runs=self.n_runs,
             get_counts=self.get_counts()
         )
 
         # normalize parameters for each type
         for t in self.types:
             self.params_mle[t] = self.model.normalize(self.params_mle[t])
@@ -502,20 +512,26 @@
                 covariate=params[k],
                 type=type,
                 params=params
             )
 
         return params
 
-    def bootstrap(self, n_samples: int = None, parallelize: bool = None) -> Optional[pd.DataFrame]:
+    def bootstrap(
+            self,
+            n_samples: int = None,
+            parallelize: bool = None,
+            update_likelihood: bool = True
+    ) -> Optional[pd.DataFrame]:
         """
         Perform the parametric bootstrap both for the marginal and joint inferences.
 
         :param n_samples: Number of bootstrap samples
         :param parallelize: Whether to parallelize computations
+        :param update_likelihood: Whether to update the likelihood
         :return: DataFrame with bootstrap samples
         """
         # perform inference first if not done yet
         self.run_if_required()
 
         # update properties
         self.update_properties(
@@ -577,14 +593,18 @@
 
             # add estimates for alpha to the bootstraps
             inf.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
+        # determine average likelihood of successful runs
+        if update_likelihood:
+            self.likelihood = np.mean([-res.fun for res in result[:, 0] if res.success] + [self.likelihood])
+
         return self.bootstraps
 
     def run_joint_bootstrap_sample(self, seed: int = None) -> (OptimizeResult, dict):
         """
         Resample the observed selected SFS and rerun the optimization procedure.
         We take the MLE params as initial params here.
 
@@ -594,14 +614,15 @@
             self.rng = np.random.default_rng(seed=seed)
 
         # perform joint optimization
         # Note that it's important we bind t into the lambda function
         # at the time of creation.
         result, params_mle = self.optimization.run(
             x0=self.params_mle_shared,
+            scales=self.get_scales_linear(),
             n_runs=1,
             debug_iterations=False,
             print_info=False,
             get_counts=dict((t, lambda params, t=t: inf.model_sfs(
                 correct_values(self.add_covariates(params, t), self.optimization.bounds),
                 sfs_neut=self.resample_sfs(self.marginal_inferences[t].sfs_neut),
                 sfs_sel=self.resample_sfs(self.marginal_inferences[t].sfs_sel)
@@ -829,15 +850,15 @@
             intervals: np.ndarray = None,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'DFE comparison',
             labels: List[str] = None,
             scale_density: bool = False,
-            scale: Literal['lin', 'log'] = 'lin',
+            scale: Literal['lin', 'log', 'symlog'] = 'lin',
             ax: plt.Axes = None
     ) -> plt.Axes:
         """
         Plot discretized DFE. The special constants ``np.inf`` and ``-np.inf`` are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
@@ -927,16 +948,15 @@
     def to_json(self) -> str:
         """
         Serialize object. Note that the deserialized inference objects no
         longer share the same optimization instance among other things.
 
         :return: JSON string
         """
-        # using make_ref=True resulted in weird behaviour
-        # when unserializing.
+        # using make_ref=True resulted in weird behaviour when unserializing.
         return jsonpickle.encode(self, indent=4, warn=True, make_refs=False)
 
     @functools.cached_property
     def alpha(self) -> Optional[float]:
         """
         The is no single alpha for the joint inference. Please refer
         to the ``self.joint_inferences[t].alpha``.
```

### Comparing `fastdfe-0.1.2b0/fastdfe/spectrum.py` & `fastdfe-0.1.3b0/fastdfe/spectrum.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.2b0/fastdfe/visualization.py` & `fastdfe-0.1.3b0/fastdfe/visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """
-Infer the DFE from the SFS using discretized DFE.
+Visualization module.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import functools
 import logging
 from typing import Callable, List, Literal, Dict
 
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 import seaborn as sns
 from matplotlib import colors
 from matplotlib.colors import LogNorm
 from matplotlib.container import BarContainer
 from matplotlib.ticker import MaxNLocator
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from . import Parametrization
-from .bootstrap import Bootstrap
 from .spectrum import Spectrum
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class Visualization:
@@ -314,15 +312,14 @@
         ticks = ax.get_xticks()
         ticks_new = ["{:.0e}".format(s[int(l)]) if 0 <= int(l) < n_bins else None for l in ticks]
 
         ax.set_xticks(ticks)
         ax.set_xticklabels(ticks_new)
 
     @staticmethod
-    @clear_show_save
     def plot_sfs_comparison(
             ax: plt.Axes,
             spectra: List[Spectrum] | np.ndarray,
             labels: List[str] = [],
             file: str = None,
             show: bool = True,
             title: str = 'SFS comparison',
@@ -344,85 +341,62 @@
         """
         # plot modelled vs observed non-neutral SFS
         ax = Visualization.plot_spectra(
             spectra=spectra,
             labels=labels,
             use_subplots=use_subplots,
             show_monomorphic=show_monomorphic,
+            title=title,
             ax=ax
         )
 
-        # set title
-        ax.set_title(title)
-
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_inferred_parameters(
-            params: List[dict],
-            bootstraps: List[pd.DataFrame],
             ax: plt.Axes,
+            values: Dict[str, np.ndarray],
+            labels: list | np.ndarray,
+            param_names: list | np.ndarray,
+            errors: Dict[str, np.ndarray | None],
             file: str = None,
             show: bool = True,
-            confidence_intervals: bool = True,
-            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
-            ci_level: float = 0.05,
             title: str = 'parameter estimates',
-            scale: Literal['lin', 'log'] = 'log',
-            labels: List[str] = None,
-            **kwargs
+            legend: bool = True,
+            scale: Literal['lin', 'log', 'symlog'] = 'log'
     ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
-        using a bar plot.
+        using a bar plot. Note that there problems with parameters that span 0.
 
-        :param labels: Labels for the parameters
+        :param labels: Unique labels for the DFEs
+        :param param_names: Labels for the parameters
         :param scale: Whether to use a linear or log scale
         :param title: Title of the plot
-        :param ci_level: Confidence level
-        :param bootstrap_type: Type of bootstrap to use
-        :param confidence_intervals: Whether to show confidence intervals
-        :param params: List of parameter dictionaries in the same order as the labels
-        :param bootstraps: List of dataframes containing bootstrapped parameter values in the same order as the labels
+        :param legend: Whether to show the legend
+        :param errors: Dictionary of errors with the parameter in the same order as ``labels``
+        :param values: Dictionary of parameter values with the parameter in the same order as ``labels``
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param ax: Axes to plot on
         :return: Axes
         """
-        n_types = len(params)
+        n_types = len(values)
 
         width_total = 0.9
         width = width_total / n_types
 
-        # get keys of first element which we use to order the rest
-        keys = sorted(list(params[0].keys()))
-        n_values = len(keys)
+        # number of parameters
+        n_params = len(param_names)
 
         # iterate over types
-        for i, param, bs in zip(range(n_types), params, bootstraps):
+        for i, vals, errs in zip(range(n_types), values.values(), errors.values()):
 
-            values = list(param[k] for k in keys)
-
-            # determine confidence interval if bootstraps were given
-            if confidence_intervals and bs is not None:
-                errors, _ = Bootstrap.get_errors(
-                    values=np.abs(values),
-                    bs=np.abs(bs[keys].to_numpy()),
-                    bootstrap_type=bootstrap_type,
-                    ci_level=ci_level
-                )
-            else:
-                errors = None
-
-            # whether to use the mean of all bootstraps instead of the original values
-            use_means = confidence_intervals and bs is not None and bootstrap_type == 'percentile'
-
-            x = np.arange(n_values) + i * width
-            y = np.abs(bs[keys].mean().to_list() if use_means else values)
+            x = np.arange(n_params) + i * width
 
             def name_to_label(key: str) -> str:
                 """
                 Add parameter name to label.
 
                 :param key: Parameter name
                 :return: Label
@@ -432,46 +406,55 @@
                     alpha='α',
                     eps='ε'
                 )
 
                 # map to new name
                 label = label_mapping[key] if key in label_mapping else key
 
+                # get index of parameter
+                k = np.where(np.array(param_names) == key)[0][0]
+
                 # check parameter value and add minus sign if negative
-                if param[key] >= 0:
+                if vals[k] >= 0:
                     return '$' + label + '$'
 
                 return '$-' + key + '$'
 
             # append a minus sign to negative parameters values
-            xlabels = np.array([name_to_label(key) for key in keys])
+            xlabels = np.array([name_to_label(key) for key in param_names])
 
+            # flip errors for negative parameters
+            if errs is not None:
+                errs = np.array([err if vals[i] >= 0 else err[::-1] for i, err in enumerate(errs.T)]).T
+
+            # Plot bars.
+            # Note that we plot the absolute value of the parameter
             bars = ax.bar(
                 x=x,
-                height=y,
-                yerr=errors,
+                height=np.abs(vals),
+                yerr=errs,
                 error_kw=dict(
                     capsize=width * 7
                 ),
-                label=labels[i] if labels is not None else None,
+                label=labels[i],
                 width=width,
                 linewidth=0,
                 hatch=Visualization.get_hatch(i, labels),
                 color=Visualization.get_color(labels[i], labels) if labels is not None else None
             )
 
             Visualization.darken_edge_colors(bars)
 
             # customize x-ticks
-            x = np.arange(n_values)
+            x = np.arange(n_params)
             ax.set_xticks([i + (width_total - width) / 2 for i in x], x)
             ax.set_xticklabels(xlabels)
 
         # show legend if specified
-        if labels is not None:
+        if legend:
             plt.legend(prop=dict(size=8), loc='upper right')
 
         # set title
         ax.set_title(title)
 
         # change to log-scale if specified
         if scale == 'log':
@@ -535,32 +518,38 @@
     def plot_spectra(
             spectra: List[Spectrum],
             ax: plt.Axes,
             labels: List[str] = [],
             log_scale: bool = False,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
+            title: str = None,
             n_ticks=10,
             file: str = None,
             show: bool = True
     ) -> plt.Axes:
         """
         Plot the given 1D spectra.
 
         :param show_monomorphic: Whether to show monomorphic site counts
         :param n_ticks: Number of x-ticks to use
         :param ax: Axes to plot on
         :param use_subplots: Whether to use subplots
+        :param title: Title of plot
         :param spectra: List of spectra to plot
         :param labels: List of labels for each spectrum
         :param log_scale: Whether to use logarithmic y-scale
         :param file: File to save plot to
         :param show: Whether to show the plot
         :return: Axes
         """
+        if ax is None:
+            plt.clf()
+            _, ax = plt.subplots()
+
         if use_subplots:
             n_plots = len(spectra)
             n_rows = int(np.ceil(np.sqrt(n_plots)))
             n_cols = int(np.ceil(np.sqrt(n_plots)))
             fig = plt.figure(figsize=(6.4 * n_cols ** (1 / 3), 4.8 * n_rows ** (1 / 3)))
             axes = fig.subplots(ncols=n_cols, nrows=n_rows, squeeze=False).flatten()
 
@@ -623,15 +612,19 @@
 
         if log_scale:
             ax.set_yscale('log')
 
         if len(labels) == 1:
             ax.set_title(labels[0])
         elif len(labels) > 1:
-            plt.legend(prop=dict(size=8))
+
+            # set title
+            ax.set_title(title)
+
+            ax.legend(prop=dict(size=8))
 
         # show and save plot
         Visualization.show_and_save(file, show)
 
         return ax
 
     @staticmethod
@@ -724,15 +717,15 @@
     @staticmethod
     @clear_show_save
     def plot_likelihoods(
             likelihoods: list | np.ndarray,
             file: str, show: bool,
             title: str,
             ax: plt.Axes,
-            scale: Literal['lin', 'log'] = 'lin'
+            scale: Literal['lin', 'log', 'symlog'] = 'lin'
     ) -> plt.Axes:
         """
         A scatter plot of the likelihoods specified.
 
         :param scale: Scale of y-axis
         :param likelihoods: Likelihoods to plot
         :param file: File to save plot to
@@ -882,15 +875,15 @@
     @staticmethod
     @clear_show_save
     def plot_covariates(
             covariates: Dict[str, 'Covariate'],
             params_marginal: Dict[str, Dict[str, float]],
             params_joint: Dict[str, Dict[str, float]],
             axs: List[plt.Axes],
-            scale: Literal['lin', 'log'] = 'log',
+            scale: Literal['lin', 'log', 'symlog'] = 'log',
             file: str = None,
             show: bool = True,
             **kwargs
     ) -> List[plt.Axes]:
         """
         Plot covariates.
 
@@ -943,15 +936,15 @@
                 x=x + width,
                 height=y2,
                 width=width,
                 label='joint'
             )
 
             # proper representation of parameter
-            param_repr = f'${cov.param}' if params_marginal[types[0]][cov.param] >= 0 else f'$-{cov.param}'
+            param_repr = f'${cov.param}$' if params_marginal[types[0]][cov.param] >= 0 else f'$-{cov.param}$'
 
             # set title
             ax.set_title(f"param={param_repr}, {p}={params_joint[types[0]][p]}")
 
             # adjust ticks
             ax.set_xticks(np.arange(len(types)) + width / 2)
             ax.set_xticklabels(types)
```

### Comparing `fastdfe-0.1.2b0/pyproject.toml` & `fastdfe-0.1.3b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "0.1.2-beta"
+version = "0.1.3-beta"
 description = "Fast, flexible, and hierarchical inference of the distribution of fitness effects"
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `fastdfe-0.1.2b0/PKG-INFO` & `fastdfe-0.1.3b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: Fast, flexible, and hierarchical inference of the distribution of fitness effects
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,8 +23,8 @@
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 fastDFE is a new package designed for inferring the distribution of fitness effects (DFE) from site-frequency spectra (SFS). As it is currently in its beta phase, we are continuously working to improve and refine its features.
 
-<!--- Please see the [documentation](docs/_build/html/index.html) for more details. --->
+Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

