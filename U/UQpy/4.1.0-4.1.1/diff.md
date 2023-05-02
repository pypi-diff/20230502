# Comparing `tmp/UQpy-4.1.0.tar.gz` & `tmp/UQpy-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UQpy-4.1.0.tar", last modified: Fri Apr 28 22:56:36 2023, max compression
+gzip compressed data, was "UQpy-4.1.1.tar", last modified: Tue May  2 21:20:53 2023, max compression
```

## Comparing `UQpy-4.1.0.tar` & `UQpy-4.1.1.tar`

### file list

```diff
@@ -1,330 +1,329 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.952403 UQpy-4.1.0/
--rw-r--r--   0 runner     (501) staff       (20)     1075 2023-04-28 22:03:53.000000 UQpy-4.1.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-28 22:56:36.952019 UQpy-4.1.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     5526 2023-04-28 22:03:53.000000 UQpy-4.1.0/README.rst
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-28 22:56:36.952514 UQpy-4.1.0/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     1046 2023-04-28 22:03:54.000000 UQpy-4.1.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.753139 UQpy-4.1.0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.770341 UQpy-4.1.0/src/UQpy/
--rw-r--r--   0 runner     (501) staff       (20)     1583 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.773424 UQpy-4.1.0/src/UQpy/dimension_reduction/
--rw-r--r--   0 runner     (501) staff       (20)      200 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.774475 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/
--rw-r--r--   0 runner     (501) staff       (20)    14135 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py
--rw-r--r--   0 runner     (501) staff       (20)       80 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.775867 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/
--rw-r--r--   0 runner     (501) staff       (20)     3926 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py
--rw-r--r--   0 runner     (501) staff       (20)    12719 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py
--rw-r--r--   0 runner     (501) staff       (20)      268 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.776931 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/
--rw-r--r--   0 runner     (501) staff       (20)     3465 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.777995 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/GrassmannProjection.py
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.779024 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/
--rw-r--r--   0 runner     (501) staff       (20)     6969 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py
--rw-r--r--   0 runner     (501) staff       (20)       72 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.780313 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/
--rw-r--r--   0 runner     (501) staff       (20)     1206 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/DirectPOD.py
--rw-r--r--   0 runner     (501) staff       (20)     1302 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/SnapshotPOD.py
--rw-r--r--   0 runner     (501) staff       (20)      179 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.781191 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     6163 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/POD.py
--rw-r--r--   0 runner     (501) staff       (20)       56 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.781611 UQpy-4.1.0/src/UQpy/distributions/
--rw-r--r--   0 runner     (501) staff       (20)      209 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.785452 UQpy-4.1.0/src/UQpy/distributions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2414 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Copula.py
--rw-r--r--   0 runner     (501) staff       (20)     4131 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution.py
--rw-r--r--   0 runner     (501) staff       (20)     1326 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution1D.py
--rw-r--r--   0 runner     (501) staff       (20)     1094 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionContinuous1D.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py
--rw-r--r--   0 runner     (501) staff       (20)      680 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionND.py
--rw-r--r--   0 runner     (501) staff       (20)      488 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.834528 UQpy-4.1.0/src/UQpy/distributions/collection/
--rw-r--r--   0 runner     (501) staff       (20)      822 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Beta.py
--rw-r--r--   0 runner     (501) staff       (20)      701 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Binomial.py
--rw-r--r--   0 runner     (501) staff       (20)      566 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Cauchy.py
--rw-r--r--   0 runner     (501) staff       (20)      740 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/ChiSquare.py
--rw-r--r--   0 runner     (501) staff       (20)      570 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Exponential.py
--rw-r--r--   0 runner     (501) staff       (20)      683 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Gamma.py
--rw-r--r--   0 runner     (501) staff       (20)      701 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/GeneralizedExtreme.py
--rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/InverseGaussian.py
--rw-r--r--   0 runner     (501) staff       (20)     6418 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/JointCopula.py
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/JointIndependent.py
--rw-r--r--   0 runner     (501) staff       (20)      568 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Laplace.py
--rw-r--r--   0 runner     (501) staff       (20)      562 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Levy.py
--rw-r--r--   0 runner     (501) staff       (20)      570 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Logistic.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Lognormal.py
--rw-r--r--   0 runner     (501) staff       (20)      568 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Maxwell.py
--rw-r--r--   0 runner     (501) staff       (20)     1980 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Multinomial.py
--rw-r--r--   0 runner     (501) staff       (20)     2618 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/MultivariateNormal.py
--rw-r--r--   0 runner     (501) staff       (20)      562 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Normal.py
--rw-r--r--   0 runner     (501) staff       (20)      684 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Pareto.py
--rw-r--r--   0 runner     (501) staff       (20)      529 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Poisson.py
--rw-r--r--   0 runner     (501) staff       (20)      569 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Rayleigh.py
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/TruncatedNormal.py
--rw-r--r--   0 runner     (501) staff       (20)      550 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Uniform.py
--rw-r--r--   0 runner     (501) staff       (20)     1469 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.836303 UQpy-4.1.0/src/UQpy/distributions/copulas/
--rw-r--r--   0 runner     (501) staff       (20)     1527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Clayton.py
--rw-r--r--   0 runner     (501) staff       (20)     1583 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Frank.py
--rw-r--r--   0 runner     (501) staff       (20)     2939 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Gumbel.py
--rw-r--r--   0 runner     (501) staff       (20)      159 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.838656 UQpy-4.1.0/src/UQpy/inference/
--rw-r--r--   0 runner     (501) staff       (20)     7270 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/BayesModelSelection.py
--rw-r--r--   0 runner     (501) staff       (20)     5220 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/BayesParameterEstimation.py
--rw-r--r--   0 runner     (501) staff       (20)     7269 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/InformationModelSelection.py
--rw-r--r--   0 runner     (501) staff       (20)     8194 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/MLE.py
--rw-r--r--   0 runner     (501) staff       (20)      593 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.839702 UQpy-4.1.0/src/UQpy/inference/evidence_methods/
--rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/HarmonicMean.py
--rw-r--r--   0 runner     (501) staff       (20)      126 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.840687 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      908 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.842585 UQpy-4.1.0/src/UQpy/inference/inference_models/
--rw-r--r--   0 runner     (501) staff       (20)     4003 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/ComputationalModel.py
--rw-r--r--   0 runner     (501) staff       (20)     2903 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/DistributionModel.py
--rw-r--r--   0 runner     (501) staff       (20)     1301 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/LogLikelihoodModel.py
--rw-r--r--   0 runner     (501) staff       (20)      302 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.843544 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/InferenceModel.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.845336 UQpy-4.1.0/src/UQpy/inference/information_criteria/
--rw-r--r--   0 runner     (501) staff       (20)      883 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/AIC.py
--rw-r--r--   0 runner     (501) staff       (20)     1004 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/AICc.py
--rw-r--r--   0 runner     (501) staff       (20)      959 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/BIC.py
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.846272 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      649 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py
--rw-r--r--   0 runner     (501) staff       (20)      100 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.847234 UQpy-4.1.0/src/UQpy/reliability/
--rw-r--r--   0 runner     (501) staff       (20)    13794 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/SubsetSimulation.py
--rw-r--r--   0 runner     (501) staff       (20)      136 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.849007 UQpy-4.1.0/src/UQpy/reliability/taylor_series/
--rw-r--r--   0 runner     (501) staff       (20)    16597 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/FORM.py
--rw-r--r--   0 runner     (501) staff       (20)     6843 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/SORM.py
--rw-r--r--   0 runner     (501) staff       (20)      185 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.850250 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     6400 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py
--rw-r--r--   0 runner     (501) staff       (20)       68 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.851329 UQpy-4.1.0/src/UQpy/run_model/
--rwxr-xr-x   0 runner     (501) staff       (20)    11467 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/RunModel.py
--rw-r--r--   0 runner     (501) staff       (20)       91 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.855294 UQpy-4.1.0/src/UQpy/run_model/model_execution/
--rw-r--r--   0 runner     (501) staff       (20)     2410 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ClusterExecution.py
--rw-r--r--   0 runner     (501) staff       (20)     2632 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ParallelExecution.py
--rw-r--r--   0 runner     (501) staff       (20)     6848 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/PythonModel.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/SerialExecution.py
--rw-r--r--   0 runner     (501) staff       (20)    23079 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ThirdPartyModel.py
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.859203 UQpy-4.1.0/src/UQpy/sampling/
--rw-r--r--   0 runner     (501) staff       (20)    11872 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/AdaptiveKriging.py
--rw-r--r--   0 runner     (501) staff       (20)     8359 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/ImportanceSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     9204 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/MonteCarloSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     3835 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/SimplexSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     5079 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/ThetaCriterionPCE.py
--rw-r--r--   0 runner     (501) staff       (20)      492 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.862714 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py
--rw-r--r--   0 runner     (501) staff       (20)     1330 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py
--rw-r--r--   0 runner     (501) staff       (20)     1535 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py
--rw-r--r--   0 runner     (501) staff       (20)     1062 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py
--rw-r--r--   0 runner     (501) staff       (20)     1627 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.863683 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      717 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.867054 UQpy-4.1.0/src/UQpy/sampling/mcmc/
--rw-r--r--   0 runner     (501) staff       (20)    14747 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/DRAM.py
--rw-r--r--   0 runner     (501) staff       (20)    13883 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/DREAM.py
--rw-r--r--   0 runner     (501) staff       (20)     7890 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/MetropolisHastings.py
--rw-r--r--   0 runner     (501) staff       (20)    12556 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py
--rw-r--r--   0 runner     (501) staff       (20)     8369 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/Stretch.py
--rw-r--r--   0 runner     (501) staff       (20)      385 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.868092 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)    18931 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/MCMC.py
--rw-r--r--   0 runner     (501) staff       (20)       51 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.869758 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/
--rw-r--r--   0 runner     (501) staff       (20)    13557 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py
--rw-r--r--   0 runner     (501) staff       (20)    17860 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py
--rw-r--r--   0 runner     (501) staff       (20)      243 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.870728 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     5548 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.872757 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/
--rw-r--r--   0 runner     (501) staff       (20)     5475 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     4839 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     8527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)      530 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.873772 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/StratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)       94 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.876087 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py
--rw-r--r--   0 runner     (501) staff       (20)     2125 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py
--rw-r--r--   0 runner     (501) staff       (20)     1587 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py
--rw-r--r--   0 runner     (501) staff       (20)      933 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py
--rw-r--r--   0 runner     (501) staff       (20)      588 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.877093 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1069 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py
--rw-r--r--   0 runner     (501) staff       (20)       93 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.878530 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/
--rw-r--r--   0 runner     (501) staff       (20)     5703 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.879754 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2517 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py
--rw-r--r--   0 runner     (501) staff       (20)       80 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.882694 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/
--rw-r--r--   0 runner     (501) staff       (20)     4785 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py
--rw-r--r--   0 runner     (501) staff       (20)    12238 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/SamplingCriterion.py
--rw-r--r--   0 runner     (501) staff       (20)    19271 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py
--rw-r--r--   0 runner     (501) staff       (20)      407 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.884951 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     3383 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py
--rw-r--r--   0 runner     (501) staff       (20)       77 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.893751 UQpy-4.1.0/src/UQpy/sensitivity/
--rw-r--r--   0 runner     (501) staff       (20)    15373 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/ChatterjeeSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    10943 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/CramerVonMisesSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    14008 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    12705 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/MorrisSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)     5812 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/PceSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)     9026 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/PostProcess.py
--rw-r--r--   0 runner     (501) staff       (20)    33267 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/SobolSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)      637 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.895153 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2577 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/PickFreeze.py
--rw-r--r--   0 runner     (501) staff       (20)     9919 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/Sensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)      105 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.899557 UQpy-4.1.0/src/UQpy/stochastic_process/
--rw-r--r--   0 runner     (501) staff       (20)    12136 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/BispectralRepresentation.py
--rw-r--r--   0 runner     (501) staff       (20)     7111 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/InverseTranslation.py
--rw-r--r--   0 runner     (501) staff       (20)     5317 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py
--rw-r--r--   0 runner     (501) staff       (20)     6802 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py
--rw-r--r--   0 runner     (501) staff       (20)     9744 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/SpectralRepresentation.py
--rw-r--r--   0 runner     (501) staff       (20)     7111 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/Translation.py
--rw-r--r--   0 runner     (501) staff       (20)      523 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.902293 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/
--rw-r--r--   0 runner     (501) staff       (20)      378 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1159 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py
--rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py
--rw-r--r--   0 runner     (501) staff       (20)     1087 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.902799 UQpy-4.1.0/src/UQpy/surrogates/
--rw-r--r--   0 runner     (501) staff       (20)      290 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.903841 UQpy-4.1.0/src/UQpy/surrogates/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      212 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/baseclass/Surrogate.py
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.904917 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/
--rwxr-xr-x   0 runner     (501) staff       (20)    16575 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      277 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.905867 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/
--rw-r--r--   0 runner     (501) staff       (20)     2363 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py
--rw-r--r--   0 runner     (501) staff       (20)      150 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.906871 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      708 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py
--rw-r--r--   0 runner     (501) staff       (20)       94 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.908379 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/
--rw-r--r--   0 runner     (501) staff       (20)     1279 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/Matern.py
--rw-r--r--   0 runner     (501) staff       (20)      612 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/RBF.py
--rw-r--r--   0 runner     (501) staff       (20)      193 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.909291 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2135 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py
--rw-r--r--   0 runner     (501) staff       (20)       77 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.911178 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/
--rw-r--r--   0 runner     (501) staff       (20)      305 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/ConstantRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/LinearRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     1323 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.912133 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      385 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/Regression.py
--rw-r--r--   0 runner     (501) staff       (20)       95 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.913029 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/
--rw-r--r--   0 runner     (501) staff       (20)    12979 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py
--rw-r--r--   0 runner     (501) staff       (20)      584 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.916252 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/
--rw-r--r--   0 runner     (501) staff       (20)     2608 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py
--rw-r--r--   0 runner     (501) staff       (20)     1528 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py
--rw-r--r--   0 runner     (501) staff       (20)     1868 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py
--rw-r--r--   0 runner     (501) staff       (20)     1252 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     1599 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.917831 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     5969 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     6186 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py
--rw-r--r--   0 runner     (501) staff       (20)      190 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.920244 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/
--rw-r--r--   0 runner     (501) staff       (20)     3015 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     5634 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      951 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     2687 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      378 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.921302 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      229 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/Regression.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.922113 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/
--rw-r--r--   0 runner     (501) staff       (20)    17080 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py
--rw-r--r--   0 runner     (501) staff       (20)       23 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.923937 UQpy-4.1.0/src/UQpy/transformations/
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Correlate.py
--rw-r--r--   0 runner     (501) staff       (20)     1027 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Decorrelate.py
--rw-r--r--   0 runner     (501) staff       (20)    20420 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Nataf.py
--rw-r--r--   0 runner     (501) staff       (20)       95 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.929320 UQpy-4.1.0/src/UQpy/utilities/
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/Constants.py
--rw-r--r--   0 runner     (501) staff       (20)      429 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/DistanceMetric.py
--rw-r--r--   0 runner     (501) staff       (20)     1324 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/FminCobyla.py
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/GrassmannPoint.py
--rw-r--r--   0 runner     (501) staff       (20)     1920 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/MinimizeOptimizer.py
--rw-r--r--   0 runner     (501) staff       (20)      772 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/NoPublicConstructor.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/UQpyLoggingFormatter.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11339 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/Utilities.py
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/ValidationTypes.py
--rw-r--r--   0 runner     (501) staff       (20)      399 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.930918 UQpy-4.1.0/src/UQpy/utilities/distances/
--rw-r--r--   0 runner     (501) staff       (20)      170 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.934037 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1244 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/Distance.py
--rw-r--r--   0 runner     (501) staff       (20)     1270 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     2053 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      237 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.940410 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/
--rw-r--r--   0 runner     (501) staff       (20)      642 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      618 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      620 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      634 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      626 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      612 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      590 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py
--rw-r--r--   0 runner     (501) staff       (20)      767 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.946910 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/
--rw-r--r--   0 runner     (501) staff       (20)      954 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      979 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      991 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1085 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1128 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1068 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      764 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.948775 UQpy-4.1.0/src/UQpy/utilities/kernels/
--rw-r--r--   0 runner     (501) staff       (20)      772 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/BinetCauchyKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     2939 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/GaussianKernel.py
--rw-r--r--   0 runner     (501) staff       (20)      785 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/ProjectionKernel.py
--rw-r--r--   0 runner     (501) staff       (20)      254 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.951368 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     2090 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/Kernel.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.772963 UQpy-4.1.0/src/UQpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    14004 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       57 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.824408 UQpy-4.1.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1075 2023-05-02 20:20:58.000000 UQpy-4.1.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-05-02 21:20:53.823999 UQpy-4.1.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5526 2023-05-02 20:20:58.000000 UQpy-4.1.1/README.rst
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-05-02 21:20:53.824550 UQpy-4.1.1/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     1046 2023-05-02 20:20:58.000000 UQpy-4.1.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.423331 UQpy-4.1.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.443079 UQpy-4.1.1/src/UQpy/
+-rw-r--r--   0 runner     (501) staff       (20)     1583 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.446081 UQpy-4.1.1/src/UQpy/dimension_reduction/
+-rw-r--r--   0 runner     (501) staff       (20)      200 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.447146 UQpy-4.1.1/src/UQpy/dimension_reduction/diffusion_maps/
+-rw-r--r--   0 runner     (501) staff       (20)    14145 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py
+-rw-r--r--   0 runner     (501) staff       (20)       80 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/diffusion_maps/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.448606 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/
+-rw-r--r--   0 runner     (501) staff       (20)     3926 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py
+-rw-r--r--   0 runner     (501) staff       (20)    12719 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py
+-rw-r--r--   0 runner     (501) staff       (20)      268 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.449673 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/
+-rw-r--r--   0 runner     (501) staff       (20)     3465 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py
+-rw-r--r--   0 runner     (501) staff       (20)      176 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.450728 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      171 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/GrassmannProjection.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.451750 UQpy-4.1.1/src/UQpy/dimension_reduction/hosvd/
+-rw-r--r--   0 runner     (501) staff       (20)     6969 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py
+-rw-r--r--   0 runner     (501) staff       (20)       72 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/hosvd/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.453250 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/DirectPOD.py
+-rw-r--r--   0 runner     (501) staff       (20)     1302 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/SnapshotPOD.py
+-rw-r--r--   0 runner     (501) staff       (20)      179 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.454184 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     6163 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/baseclass/POD.py
+-rw-r--r--   0 runner     (501) staff       (20)       56 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/dimension_reduction/pod/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.454629 UQpy-4.1.1/src/UQpy/distributions/
+-rw-r--r--   0 runner     (501) staff       (20)      209 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.458323 UQpy-4.1.1/src/UQpy/distributions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2414 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/Copula.py
+-rw-r--r--   0 runner     (501) staff       (20)     4131 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/Distribution.py
+-rw-r--r--   0 runner     (501) staff       (20)     1326 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/Distribution1D.py
+-rw-r--r--   0 runner     (501) staff       (20)     1094 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionContinuous1D.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py
+-rw-r--r--   0 runner     (501) staff       (20)      680 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionND.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.470546 UQpy-4.1.1/src/UQpy/distributions/collection/
+-rw-r--r--   0 runner     (501) staff       (20)      822 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Beta.py
+-rw-r--r--   0 runner     (501) staff       (20)      701 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Binomial.py
+-rw-r--r--   0 runner     (501) staff       (20)      566 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Cauchy.py
+-rw-r--r--   0 runner     (501) staff       (20)      740 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/ChiSquare.py
+-rw-r--r--   0 runner     (501) staff       (20)      570 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Exponential.py
+-rw-r--r--   0 runner     (501) staff       (20)      683 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Gamma.py
+-rw-r--r--   0 runner     (501) staff       (20)      701 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/GeneralizedExtreme.py
+-rw-r--r--   0 runner     (501) staff       (20)      710 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/InverseGaussian.py
+-rw-r--r--   0 runner     (501) staff       (20)     6418 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/JointCopula.py
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/JointIndependent.py
+-rw-r--r--   0 runner     (501) staff       (20)      568 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Laplace.py
+-rw-r--r--   0 runner     (501) staff       (20)      562 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Levy.py
+-rw-r--r--   0 runner     (501) staff       (20)      570 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Logistic.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Lognormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      568 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Maxwell.py
+-rw-r--r--   0 runner     (501) staff       (20)     1980 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Multinomial.py
+-rw-r--r--   0 runner     (501) staff       (20)     2618 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/MultivariateNormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      562 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Normal.py
+-rw-r--r--   0 runner     (501) staff       (20)      684 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Pareto.py
+-rw-r--r--   0 runner     (501) staff       (20)      529 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Poisson.py
+-rw-r--r--   0 runner     (501) staff       (20)      569 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Rayleigh.py
+-rw-r--r--   0 runner     (501) staff       (20)      826 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/TruncatedNormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      550 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/Uniform.py
+-rw-r--r--   0 runner     (501) staff       (20)     1469 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/collection/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.472765 UQpy-4.1.1/src/UQpy/distributions/copulas/
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/copulas/Clayton.py
+-rw-r--r--   0 runner     (501) staff       (20)     1583 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/copulas/Frank.py
+-rw-r--r--   0 runner     (501) staff       (20)     2939 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/copulas/Gumbel.py
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/distributions/copulas/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.475559 UQpy-4.1.1/src/UQpy/inference/
+-rw-r--r--   0 runner     (501) staff       (20)     7270 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/BayesModelSelection.py
+-rw-r--r--   0 runner     (501) staff       (20)     5220 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/BayesParameterEstimation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7269 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/InformationModelSelection.py
+-rw-r--r--   0 runner     (501) staff       (20)     8194 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/MLE.py
+-rw-r--r--   0 runner     (501) staff       (20)      593 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.476823 UQpy-4.1.1/src/UQpy/inference/evidence_methods/
+-rw-r--r--   0 runner     (501) staff       (20)      527 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/evidence_methods/HarmonicMean.py
+-rw-r--r--   0 runner     (501) staff       (20)      126 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/evidence_methods/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.478075 UQpy-4.1.1/src/UQpy/inference/evidence_methods/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      908 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/evidence_methods/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.481306 UQpy-4.1.1/src/UQpy/inference/inference_models/
+-rw-r--r--   0 runner     (501) staff       (20)     4003 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/ComputationalModel.py
+-rw-r--r--   0 runner     (501) staff       (20)     2903 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/DistributionModel.py
+-rw-r--r--   0 runner     (501) staff       (20)     1301 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/LogLikelihoodModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      302 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.483575 UQpy-4.1.1/src/UQpy/inference/inference_models/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/baseclass/InferenceModel.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/inference_models/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.487316 UQpy-4.1.1/src/UQpy/inference/information_criteria/
+-rw-r--r--   0 runner     (501) staff       (20)      883 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/AIC.py
+-rw-r--r--   0 runner     (501) staff       (20)     1004 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/AICc.py
+-rw-r--r--   0 runner     (501) staff       (20)      959 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/BIC.py
+-rw-r--r--   0 runner     (501) staff       (20)      230 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.489670 UQpy-4.1.1/src/UQpy/inference/information_criteria/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      649 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py
+-rw-r--r--   0 runner     (501) staff       (20)      100 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/inference/information_criteria/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.490984 UQpy-4.1.1/src/UQpy/reliability/
+-rw-r--r--   0 runner     (501) staff       (20)    13794 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/SubsetSimulation.py
+-rw-r--r--   0 runner     (501) staff       (20)      136 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.492658 UQpy-4.1.1/src/UQpy/reliability/taylor_series/
+-rw-r--r--   0 runner     (501) staff       (20)    16597 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/taylor_series/FORM.py
+-rw-r--r--   0 runner     (501) staff       (20)     6843 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/taylor_series/SORM.py
+-rw-r--r--   0 runner     (501) staff       (20)      185 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/taylor_series/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.493712 UQpy-4.1.1/src/UQpy/reliability/taylor_series/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     6400 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py
+-rw-r--r--   0 runner     (501) staff       (20)       68 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/reliability/taylor_series/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.495150 UQpy-4.1.1/src/UQpy/run_model/
+-rwxr-xr-x   0 runner     (501) staff       (20)    11467 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/RunModel.py
+-rw-r--r--   0 runner     (501) staff       (20)       91 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.501546 UQpy-4.1.1/src/UQpy/run_model/model_execution/
+-rw-r--r--   0 runner     (501) staff       (20)     2410 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/ClusterExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)     2632 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/ParallelExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)     6848 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/PythonModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/SerialExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)    23079 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/ThirdPartyModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      244 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/run_model/model_execution/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.506626 UQpy-4.1.1/src/UQpy/sampling/
+-rw-r--r--   0 runner     (501) staff       (20)    11872 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/AdaptiveKriging.py
+-rw-r--r--   0 runner     (501) staff       (20)     8359 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/ImportanceSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     9204 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/MonteCarloSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     3835 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/SimplexSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     5079 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/ThetaCriterionPCE.py
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.511325 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py
+-rw-r--r--   0 runner     (501) staff       (20)     1330 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py
+-rw-r--r--   0 runner     (501) staff       (20)     1535 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py
+-rw-r--r--   0 runner     (501) staff       (20)     1062 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)     1627 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.512646 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      717 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.517163 UQpy-4.1.1/src/UQpy/sampling/mcmc/
+-rw-r--r--   0 runner     (501) staff       (20)    14747 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/DRAM.py
+-rw-r--r--   0 runner     (501) staff       (20)    13883 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/DREAM.py
+-rw-r--r--   0 runner     (501) staff       (20)     7890 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/MetropolisHastings.py
+-rw-r--r--   0 runner     (501) staff       (20)    12556 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py
+-rw-r--r--   0 runner     (501) staff       (20)     8369 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/Stretch.py
+-rw-r--r--   0 runner     (501) staff       (20)      385 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.518775 UQpy-4.1.1/src/UQpy/sampling/mcmc/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)    18931 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/baseclass/MCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)       51 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.521118 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/
+-rw-r--r--   0 runner     (501) staff       (20)    13557 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)    17860 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)      243 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.522805 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     5544 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.525722 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/
+-rw-r--r--   0 runner     (501) staff       (20)     5475 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     4839 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     8527 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)      530 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.526990 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/baseclass/StratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)       94 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.530984 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py
+-rw-r--r--   0 runner     (501) staff       (20)     2125 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py
+-rw-r--r--   0 runner     (501) staff       (20)     1587 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py
+-rw-r--r--   0 runner     (501) staff       (20)      933 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py
+-rw-r--r--   0 runner     (501) staff       (20)      588 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.532529 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py
+-rw-r--r--   0 runner     (501) staff       (20)       93 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.533959 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/
+-rw-r--r--   0 runner     (501) staff       (20)     5703 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.535018 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2517 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py
+-rw-r--r--   0 runner     (501) staff       (20)       80 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.537687 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/
+-rw-r--r--   0 runner     (501) staff       (20)     4785 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)    12238 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/SamplingCriterion.py
+-rw-r--r--   0 runner     (501) staff       (20)    19271 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)      407 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.538933 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     3383 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py
+-rw-r--r--   0 runner     (501) staff       (20)       77 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.544032 UQpy-4.1.1/src/UQpy/sensitivity/
+-rw-r--r--   0 runner     (501) staff       (20)    15373 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/ChatterjeeSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    10943 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/CramerVonMisesSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    14008 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    12705 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/MorrisSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)     5812 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/PceSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)     9026 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/PostProcess.py
+-rw-r--r--   0 runner     (501) staff       (20)    33267 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/SobolSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)      637 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.546063 UQpy-4.1.1/src/UQpy/sensitivity/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2577 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/baseclass/PickFreeze.py
+-rw-r--r--   0 runner     (501) staff       (20)     9919 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/baseclass/Sensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)      105 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/sensitivity/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.552801 UQpy-4.1.1/src/UQpy/stochastic_process/
+-rw-r--r--   0 runner     (501) staff       (20)    12136 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/BispectralRepresentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7111 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/InverseTranslation.py
+-rw-r--r--   0 runner     (501) staff       (20)     5317 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py
+-rw-r--r--   0 runner     (501) staff       (20)     6802 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py
+-rw-r--r--   0 runner     (501) staff       (20)     9744 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/SpectralRepresentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7111 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/Translation.py
+-rw-r--r--   0 runner     (501) staff       (20)      523 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.557971 UQpy-4.1.1/src/UQpy/stochastic_process/supportive/
+-rw-r--r--   0 runner     (501) staff       (20)      378 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/supportive/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.558989 UQpy-4.1.1/src/UQpy/surrogates/
+-rw-r--r--   0 runner     (501) staff       (20)      290 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.560759 UQpy-4.1.1/src/UQpy/surrogates/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      212 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/baseclass/Surrogate.py
+-rw-r--r--   0 runner     (501) staff       (20)       58 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.563569 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/
+-rwxr-xr-x   0 runner     (501) staff       (20)    17234 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.565069 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/
+-rw-r--r--   0 runner     (501) staff       (20)     2363 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py
+-rw-r--r--   0 runner     (501) staff       (20)      150 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.568197 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      708 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)       94 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.572264 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/
+-rw-r--r--   0 runner     (501) staff       (20)      305 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/ConstantRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/LinearRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     1323 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.691177 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      385 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/Regression.py
+-rw-r--r--   0 runner     (501) staff       (20)       95 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.703638 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/
+-rw-r--r--   0 runner     (501) staff       (20)    12979 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.713181 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/
+-rw-r--r--   0 runner     (501) staff       (20)     2608 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py
+-rw-r--r--   0 runner     (501) staff       (20)     1528 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py
+-rw-r--r--   0 runner     (501) staff       (20)     1868 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.715479 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     5969 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     6186 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py
+-rw-r--r--   0 runner     (501) staff       (20)      190 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.719154 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/
+-rw-r--r--   0 runner     (501) staff       (20)     3015 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     5634 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      951 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     2687 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      378 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.720703 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      229 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/Regression.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.721793 UQpy-4.1.1/src/UQpy/surrogates/stochastic_reduced_order_models/
+-rw-r--r--   0 runner     (501) staff       (20)    17080 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py
+-rw-r--r--   0 runner     (501) staff       (20)       23 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/surrogates/stochastic_reduced_order_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.725023 UQpy-4.1.1/src/UQpy/transformations/
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/transformations/Correlate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1027 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/transformations/Decorrelate.py
+-rw-r--r--   0 runner     (501) staff       (20)    20420 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/transformations/Nataf.py
+-rw-r--r--   0 runner     (501) staff       (20)       95 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/transformations/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.739336 UQpy-4.1.1/src/UQpy/utilities/
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/Constants.py
+-rw-r--r--   0 runner     (501) staff       (20)      429 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/DistanceMetric.py
+-rw-r--r--   0 runner     (501) staff       (20)     1324 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/FminCobyla.py
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/GrassmannPoint.py
+-rw-r--r--   0 runner     (501) staff       (20)     1920 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/MinimizeOptimizer.py
+-rw-r--r--   0 runner     (501) staff       (20)      772 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/NoPublicConstructor.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/UQpyLoggingFormatter.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11339 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/Utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)      826 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/ValidationTypes.py
+-rw-r--r--   0 runner     (501) staff       (20)      399 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.739941 UQpy-4.1.1/src/UQpy/utilities/distances/
+-rw-r--r--   0 runner     (501) staff       (20)      170 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.742585 UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     1244 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/Distance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1270 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     2053 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      237 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.747776 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/
+-rw-r--r--   0 runner     (501) staff       (20)      642 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      618 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      620 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      634 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      626 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      612 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      590 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py
+-rw-r--r--   0 runner     (501) staff       (20)      767 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.752646 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/
+-rw-r--r--   0 runner     (501) staff       (20)      954 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      979 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      991 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1128 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      932 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      764 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.753605 UQpy-4.1.1/src/UQpy/utilities/kernels/
+-rw-r--r--   0 runner     (501) staff       (20)     3094 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/GaussianKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      319 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.756059 UQpy-4.1.1/src/UQpy/utilities/kernels/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      216 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)     1204 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/baseclass/Kernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.757457 UQpy-4.1.1/src/UQpy/utilities/kernels/euclidean_kernels/
+-rw-r--r--   0 runner     (501) staff       (20)     1500 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/euclidean_kernels/Matern.py
+-rw-r--r--   0 runner     (501) staff       (20)      790 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/euclidean_kernels/RBF.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/euclidean_kernels/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.770359 UQpy-4.1.1/src/UQpy/utilities/kernels/grassmannian_kernels/
+-rw-r--r--   0 runner     (501) staff       (20)      585 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/grassmannian_kernels/BinetCauchyKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      781 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/grassmannian_kernels/ProjectionKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      182 2023-05-02 20:20:58.000000 UQpy-4.1.1/src/UQpy/utilities/kernels/grassmannian_kernels/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-02 21:20:53.445601 UQpy-4.1.1/src/UQpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-05-02 21:20:53.000000 UQpy-4.1.1/src/UQpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    13974 2023-05-02 21:20:53.000000 UQpy-4.1.1/src/UQpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-02 21:20:53.000000 UQpy-4.1.1/src/UQpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       57 2023-05-02 21:20:53.000000 UQpy-4.1.1/src/UQpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2023-05-02 21:20:53.000000 UQpy-4.1.1/src/UQpy.egg-info/top_level.txt
```

### Comparing `UQpy-4.1.0/LICENSE` & `UQpy-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/PKG-INFO` & `UQpy-4.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQpy
-Version: 4.1.0
+Version: 4.1.1
 Summary: UQpy is a general purpose toolbox for Uncertainty Quantification
 Home-page: https://github.com/SURGroup/UQpy
 Author: Michael D. Shields, Dimitris G. Giovanis, Audrey Olivier, Aakash Bangalore-Satish, Mohit Chauhan, Lohit Vandanapu, Ketson R.M. dos Santos
 Author-email: UQpy.info@gmail.com
 License: MIT
 Platform: OSX
 Platform: Windows
```

### Comparing `UQpy-4.1.0/README.rst` & `UQpy-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/setup.py` & `UQpy-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/__init__.py` & `UQpy-4.1.1/src/UQpy/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from UQpy.utilities import GaussianKernel, GrassmannPoint
 from UQpy.utilities.Utilities import *
 from UQpy.utilities.Utilities import _nn_coord
 from beartype import beartype
 from typing import Annotated, Union
 from beartype.vale import Is
 from UQpy.utilities.ValidationTypes import Numpy2DFloatArray, NumpyFloatArray
-from UQpy.utilities.kernels.baseclass import Kernel
+from UQpy.utilities.kernels.baseclass.Kernel import Kernel
 
 
 class DiffusionMaps:
     AlphaType = Annotated[Union[float, int], Is[lambda number: 0 <= number <= 1]]
     IntegerLargerThanUnityType = Annotated[int, Is[lambda number: number >= 1]]
 
     @beartype
@@ -64,15 +64,15 @@
         self.parsimonious_indices = None
         """Indices of the most important eigenvectors. This attribute will only be populated if the 
         :py:meth:`parsimonious`  method is invoked."""
 
         if kernel_matrix is not None:
             self.kernel_matrix = kernel_matrix
         elif data is not None and kernel is not None:
-            kernel.calculate_kernel_matrix(points=data)
+            kernel.calculate_kernel_matrix(x=data, s=data)
             self.kernel_matrix = kernel.kernel_matrix
         else:
             raise ValueError("Either `kernel_matrix` or both `data` and `kernel` must be provided")
 
         self.alpha = alpha
         self.eigenvectors_number = n_eigenvectors
         self.is_sparse = is_sparse
```

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/DirectPOD.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/pod/DirectPOD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/SnapshotPOD.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/pod/SnapshotPOD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/POD.py` & `UQpy-4.1.1/src/UQpy/dimension_reduction/pod/baseclass/POD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/Copula.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/Copula.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/Distribution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution1D.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/Distribution1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionContinuous1D.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionContinuous1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionND.py` & `UQpy-4.1.1/src/UQpy/distributions/baseclass/DistributionND.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Beta.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Beta.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Binomial.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Binomial.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Cauchy.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Cauchy.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/ChiSquare.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/ChiSquare.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Exponential.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Exponential.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Gamma.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Gamma.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/GeneralizedExtreme.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/GeneralizedExtreme.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/InverseGaussian.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/InverseGaussian.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/JointCopula.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/JointCopula.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/JointIndependent.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/JointIndependent.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Laplace.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Laplace.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Levy.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Levy.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Logistic.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Logistic.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Lognormal.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Lognormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Maxwell.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Maxwell.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Multinomial.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Multinomial.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/MultivariateNormal.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/MultivariateNormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Normal.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Normal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Pareto.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Pareto.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Poisson.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Poisson.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Rayleigh.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Rayleigh.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/TruncatedNormal.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/TruncatedNormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/Uniform.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/Uniform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/collection/__init__.py` & `UQpy-4.1.1/src/UQpy/distributions/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/copulas/Clayton.py` & `UQpy-4.1.1/src/UQpy/distributions/copulas/Clayton.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/copulas/Frank.py` & `UQpy-4.1.1/src/UQpy/distributions/copulas/Frank.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/distributions/copulas/Gumbel.py` & `UQpy-4.1.1/src/UQpy/distributions/copulas/Gumbel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/BayesModelSelection.py` & `UQpy-4.1.1/src/UQpy/inference/BayesModelSelection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/BayesParameterEstimation.py` & `UQpy-4.1.1/src/UQpy/inference/BayesParameterEstimation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/InformationModelSelection.py` & `UQpy-4.1.1/src/UQpy/inference/InformationModelSelection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/MLE.py` & `UQpy-4.1.1/src/UQpy/inference/MLE.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/__init__.py` & `UQpy-4.1.1/src/UQpy/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/evidence_methods/HarmonicMean.py` & `UQpy-4.1.1/src/UQpy/inference/evidence_methods/HarmonicMean.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py` & `UQpy-4.1.1/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/inference_models/ComputationalModel.py` & `UQpy-4.1.1/src/UQpy/inference/inference_models/ComputationalModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/inference_models/DistributionModel.py` & `UQpy-4.1.1/src/UQpy/inference/inference_models/DistributionModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/inference_models/LogLikelihoodModel.py` & `UQpy-4.1.1/src/UQpy/inference/inference_models/LogLikelihoodModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/InferenceModel.py` & `UQpy-4.1.1/src/UQpy/inference/inference_models/baseclass/InferenceModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/information_criteria/AIC.py` & `UQpy-4.1.1/src/UQpy/inference/information_criteria/AIC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/information_criteria/AICc.py` & `UQpy-4.1.1/src/UQpy/inference/information_criteria/AICc.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/information_criteria/BIC.py` & `UQpy-4.1.1/src/UQpy/inference/information_criteria/BIC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py` & `UQpy-4.1.1/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/reliability/SubsetSimulation.py` & `UQpy-4.1.1/src/UQpy/reliability/SubsetSimulation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/reliability/taylor_series/FORM.py` & `UQpy-4.1.1/src/UQpy/reliability/taylor_series/FORM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/reliability/taylor_series/SORM.py` & `UQpy-4.1.1/src/UQpy/reliability/taylor_series/SORM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py` & `UQpy-4.1.1/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/RunModel.py` & `UQpy-4.1.1/src/UQpy/run_model/RunModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/model_execution/ClusterExecution.py` & `UQpy-4.1.1/src/UQpy/run_model/model_execution/ClusterExecution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/model_execution/ParallelExecution.py` & `UQpy-4.1.1/src/UQpy/run_model/model_execution/ParallelExecution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/model_execution/PythonModel.py` & `UQpy-4.1.1/src/UQpy/run_model/model_execution/PythonModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/model_execution/SerialExecution.py` & `UQpy-4.1.1/src/UQpy/run_model/model_execution/SerialExecution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/run_model/model_execution/ThirdPartyModel.py` & `UQpy-4.1.1/src/UQpy/run_model/model_execution/ThirdPartyModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/AdaptiveKriging.py` & `UQpy-4.1.1/src/UQpy/sampling/AdaptiveKriging.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/ImportanceSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/ImportanceSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/MonteCarloSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/MonteCarloSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/SimplexSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/SimplexSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/ThetaCriterionPCE.py` & `UQpy-4.1.1/src/UQpy/sampling/ThetaCriterionPCE.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py` & `UQpy-4.1.1/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/DRAM.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/DRAM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/DREAM.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/DREAM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/MetropolisHastings.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/MetropolisHastings.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/Stretch.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/Stretch.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/MCMC.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/baseclass/MCMC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py` & `UQpy-4.1.1/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         """
         Parent class to parallel and sequential tempering MCMC algorithms.
 
         :param pdf_intermediate: callable that computes the intermediate factor. It should take at
          least two inputs :code:`x` (ndarray, point(s) at which to evaluate the function), and :code:`temper_param` (float,
          tempering parameter). Eit  her `pdf_intermediate` or `log_pdf_intermediate` must be provided
          (`log_pdf_intermediate` is preferred). Within the code, the `log_pdf_intermediate` is evaluated as:
-             :code:`log_pdf_intermediate(x, temper_param, *args_pdf_intermediate)`
+         :code:`log_pdf_intermediate(x, temper_param, *args_pdf_intermediate)`
          where `args_pdf_intermediate` are additional positional arguments that are provided to the class via its
          `args_pdf_intermediate` input
         :param log_pdf_intermediate: see `pdf_intermediate`
         :param args_pdf_intermediate: see `pdf_intermediate`
         :param distribution_reference: reference pdf :math:`p_0` as a :class:`.Distribution` object
         :param save_log_pdf: see same input in :class:`MCMC`
         """
```

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/__init__.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py` & `UQpy-4.1.1/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/ChatterjeeSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/ChatterjeeSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/CramerVonMisesSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/CramerVonMisesSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/MorrisSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/MorrisSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/PceSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/PceSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/PostProcess.py` & `UQpy-4.1.1/src/UQpy/sensitivity/PostProcess.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/SobolSensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/SobolSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/__init__.py` & `UQpy-4.1.1/src/UQpy/sensitivity/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/baseclass/PickFreeze.py` & `UQpy-4.1.1/src/UQpy/sensitivity/baseclass/PickFreeze.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/sensitivity/baseclass/Sensitivity.py` & `UQpy-4.1.1/src/UQpy/sensitivity/baseclass/Sensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/BispectralRepresentation.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/BispectralRepresentation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/InverseTranslation.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/InverseTranslation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/SpectralRepresentation.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/SpectralRepresentation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/Translation.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/Translation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/__init__.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py` & `UQpy-4.1.1/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 import numpy as np
 from scipy.linalg import cholesky, cho_solve
 
 from beartype import beartype
 
-
 from UQpy.utilities.Utilities import process_random_state
 from UQpy.surrogates.baseclass.Surrogate import Surrogate
 from UQpy.utilities.ValidationTypes import RandomStateType
-from UQpy.surrogates.gaussian_process.kernels.baseclass.Kernel import Kernel
+from UQpy.utilities.kernels.baseclass.Kernel import Kernel
 from UQpy.surrogates.gaussian_process.constraints.baseclass.Constraints import ConstraintsGPR
-from UQpy.surrogates.gaussian_process.regression_models.baseclass.Regression import Regression
 
 
 class GaussianProcessRegression(Surrogate):
     @beartype
     def __init__(
             self,
             kernel: Kernel,
@@ -200,22 +198,26 @@
                     minimizer[i__, :] = p_.x
                     fun_value[i__, 0] = p_.fun
 
             if min(fun_value) == np.inf:
                 raise NotImplementedError("Maximum likelihood estimator failed: Choose different starting point or "
                                           "increase nopt")
             t = np.argmin(fun_value)
-            self.hyperparameters = 10**minimizer[t, :]
+            self.hyperparameters = 10 ** minimizer[t, :]
 
         # Updated Correlation matrix corresponding to MLE estimates of hyperparameters
         if self.noise:
-            self.K = self.kernel.c(x=s_, s=s_, params=self.hyperparameters[:-1]) + \
-                     np.eye(nsamples)*(self.hyperparameters[-1])**2
+            self.kernel.kernel_parameter = self.hyperparameters[:-2]
+            sigma = self.hyperparameters[-2]
+            self.K = sigma ** 2 * self.kernel.calculate_kernel_matrix(x=s_, s=s_) + \
+                     np.eye(nsamples) * (self.hyperparameters[-1]) ** 2
         else:
-            self.K = self.kernel.c(x=s_, s=s_, params=self.hyperparameters)
+            self.kernel.kernel_parameter = self.hyperparameters[:-1]
+            sigma = self.hyperparameters[-1]
+            self.K = sigma ** 2 * self.kernel.calculate_kernel_matrix(x=s_, s=s_)
 
         self.cc = cholesky(self.K + 1e-10 * np.eye(nsamples), lower=True)
         self.alpha_ = cho_solve((self.cc, True), y_)
 
         if self.regression_model is not None:
             # Compute the regression coefficient (solving this linear equation: F * beta = Y)
             # Eq: 3.8, DACE
@@ -260,49 +262,56 @@
         kernelparameters = hyperparameters
         if self.noise:
             kernelparameters = hyperparameters[:-1]
             noise_std = hyperparameters[-1]
 
         if hyperparameters is not None:
             # This is used for MLE constraints, if constraints call 'predict' method.
-            K = self.kernel.c(x=s_, s=s_, params=kernelparameters) + \
+            self.kernel.kernel_parameter = kernelparameters[:-1]
+            sigma = kernelparameters[-1]
+            K = sigma ** 2 * self.kernel.calculate_kernel_matrix(x=s_, s=s_) + \
                 np.eye(self.samples.shape[0]) * (noise_std ** 2)
             cc = np.linalg.cholesky(K + 1e-10 * np.eye(self.samples.shape[0]))
             mu = 0
             if self.regression_model is not None:
                 f_dash = np.linalg.solve(cc, self.F)
                 y_dash = np.linalg.solve(cc, y_)
                 q_, g_ = np.linalg.qr(f_dash)  # Eq: 3.11, DACE
                 # Check if F is a full rank matrix
                 if np.linalg.matrix_rank(g_) != min(np.size(self.F, 0), np.size(self.F, 1)):
                     raise NotImplementedError("Chosen regression functions are not sufficiently linearly independent")
                 # Design parameters (beta: regression coefficient)
                 beta = np.linalg.solve(g_, np.matmul(np.transpose(q_), y_dash))
                 mu = np.einsum("ij,jk->ik", self.F, beta)
-            alpha_ = cho_solve((cc, True), y_-mu)
+            alpha_ = cho_solve((cc, True), y_ - mu)
         else:
             cc, alpha_ = self.cc, self.alpha_
 
         mu1 = 0
         if self.regression_model is not None:
             fx = self.regression_model.r(x_)
             if self.beta is None:
                 mu1 = np.einsum("ij,jk->ik", fx, beta)
             else:
                 mu1 = np.einsum("ij,jk->ik", fx, self.beta)
 
-        k = self.kernel.c(x=x_, s=s_, params=kernelparameters)
+        self.kernel.kernel_parameter = kernelparameters[:-1]
+        sigma = kernelparameters[-1]
+
+        k = sigma**2*self.kernel.calculate_kernel_matrix(x=x_, s=s_)
         y = mu1 + k @ alpha_
         if self.normalize:
             y = self.value_mean + y * self.value_std
         if x_.shape[1] == 1:
             y = y.flatten()
 
         if return_std:
-            k1 = self.kernel.c(x=x_, s=x_, params=kernelparameters)
+            self.kernel.kernel_parameter = kernelparameters[:-1]
+            sigma = kernelparameters[-1]
+            k1 = sigma**2*self.kernel.calculate_kernel_matrix(x=x_, s=x_)
             var = (k1 - k @ cho_solve((cc, True), k.T)).diagonal()
             mse = np.sqrt(var)
             if self.normalize:
                 mse = self.value_std * mse
             if x_.shape[1] == 1:
                 mse = mse.flatten()
             return y, mse
@@ -322,28 +331,32 @@
         :param fx_: Basis function evaluated at training points
         :return:
         """
         # Return the log-likelihood function and it's gradient. Gradient is calculated using Central Difference
         m = s.shape[0]
 
         if ind_noise:
-            k__ = k_.c(x=s, s=s, params=10 ** p0[:-1]) + np.eye(m) * (10 ** p0[-1]) ** 2
+            k_.kernel_parameter = 10 ** p0[:-2]
+            sigma = 10 ** p0[-2]
+            k__ = sigma ** 2 * k_.calculate_kernel_matrix(x=s, s=s) + np.eye(m) * (10 ** p0[-1]) ** 2
         else:
-            k__ = k_.c(x=s, s=s, params=10 ** p0)
+            k_.kernel_parameter = 10 ** p0[:-1]
+            sigma = 10 ** p0[-1]
+            k__ = sigma ** 2 * k_.calculate_kernel_matrix(x=s, s=s)
         cc = cholesky(k__ + 1e-10 * np.eye(m), lower=True)
 
         mu = 0
         if fx_ is not None:
             f_dash = np.linalg.solve(cc, fx_)
             y_dash = np.linalg.solve(cc, y)
             q_, g_ = np.linalg.qr(f_dash)  # Eq: 3.11, DACE
             # Check if F is a full rank matrix
             if np.linalg.matrix_rank(g_) != min(np.size(fx_, 0), np.size(fx_, 1)):
                 raise NotImplementedError("Chosen regression functions are not sufficiently linearly independent")
             # Design parameters (beta: regression coefficient)
             beta = np.linalg.solve(g_, np.matmul(np.transpose(q_), y_dash))
             mu = np.einsum("ij,jk->ik", fx_, beta)
 
-        term1 = (y-mu).T @ (cho_solve((cc, True), y-mu))
+        term1 = (y - mu).T @ (cho_solve((cc, True), y - mu))
         term2 = 2 * np.sum(np.log(np.abs(np.diag(cc))))
 
         return 0.5 * (term1 + term2 + m * np.log(2 * np.pi))[0, 0]
```

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py` & `UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py` & `UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/__init__.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py` & `UQpy-4.1.1/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py` & `UQpy-4.1.1/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/transformations/Correlate.py` & `UQpy-4.1.1/src/UQpy/transformations/Correlate.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/transformations/Decorrelate.py` & `UQpy-4.1.1/src/UQpy/transformations/Decorrelate.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/transformations/Nataf.py` & `UQpy-4.1.1/src/UQpy/transformations/Nataf.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/FminCobyla.py` & `UQpy-4.1.1/src/UQpy/utilities/FminCobyla.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/GrassmannPoint.py` & `UQpy-4.1.1/src/UQpy/utilities/GrassmannPoint.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/MinimizeOptimizer.py` & `UQpy-4.1.1/src/UQpy/utilities/MinimizeOptimizer.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/NoPublicConstructor.py` & `UQpy-4.1.1/src/UQpy/utilities/NoPublicConstructor.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/UQpyLoggingFormatter.py` & `UQpy-4.1.1/src/UQpy/utilities/UQpyLoggingFormatter.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/Utilities.py` & `UQpy-4.1.1/src/UQpy/utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/ValidationTypes.py` & `UQpy-4.1.1/src/UQpy/utilities/ValidationTypes.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/Distance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/Distance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/__init__.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/euclidean_distances/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/__init__.py` & `UQpy-4.1.1/src/UQpy/utilities/distances/grassmannian_distances/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.1.0/src/UQpy/utilities/kernels/BinetCauchyKernel.py` & `UQpy-4.1.1/src/UQpy/utilities/kernels/grassmannian_kernels/BinetCauchyKernel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,22 @@
+from typing import Tuple
+
 import numpy as np
 
-from UQpy.utilities.GrassmannPoint import GrassmannPoint
 from UQpy.utilities.kernels import GrassmannianKernel
 
 
 class BinetCauchyKernel(GrassmannianKernel):
     """
     A class to calculate the Binet-Cauchy kernel.
 
     """
-    def apply_method(self, points):
-        points.evaluate_matrix(self, self.calculate_kernel_matrix)
-
-    def kernel_entry(self, xi: GrassmannPoint, xj: GrassmannPoint) -> float:
+    def element_wise_operation(self, xi_j: Tuple) -> float:
         """
-        Compute the Binet-Cauchy kernel entry for two points on the Grassmann manifold.
-
-        :param xi: Orthonormal matrix representing the first point.
-        :param xj: Orthonormal matrix representing the second point.
+        Compute the Projection kernel entry for a tuple of points on the Grassmann manifold.
 
+        :param xi_j: Tuple of orthonormal matrices representing the grassmann points.
         """
-        r = np.dot(xi.data.T, xj.data)
+        xi, xj = xi_j
+        r = np.dot(xi.T, xj)
         det = np.linalg.det(r)
         return det * det
```

### Comparing `UQpy-4.1.0/src/UQpy/utilities/kernels/GaussianKernel.py` & `UQpy-4.1.1/src/UQpy/utilities/kernels/GaussianKernel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+import itertools
+from typing import Tuple
+
 import numpy as np
 import scipy
-import scipy.spatial.distance as sd
+from scipy.spatial.distance import cdist
 
 from UQpy.utilities.ValidationTypes import RandomStateType, Numpy2DFloatArray
 from UQpy.utilities.kernels import EuclideanKernel
 from scipy.spatial.distance import pdist
+import scipy.spatial.distance as sd
 
 
 class GaussianKernel(EuclideanKernel):
     """
     A class to calculate the Gaussian kernel defined as:
 
     .. math::
         k(x_j, x_i) = \exp[-(x_j - xj)^2/4\epsilon]
 
     """
-    def __init__(self, epsilon: float = 1.0):
+    def __init__(self, kernel_parameter: float = 1.0):
         """
         :param epsilon: Scale parameter of the Gaussian kernel
         """
-        super().__init__()
-        self.epsilon = epsilon
+        super().__init__(kernel_parameter=kernel_parameter)
 
-    def kernel_entry(self, xi: Numpy2DFloatArray, xj: Numpy2DFloatArray):
-        """
-        Given two points, this method computes the Gaussian kernel value between those two points
+    def calculate_kernel_matrix(self, x, s):
+        product = [self.element_wise_operation(point_pair)
+                   for point_pair in list(itertools.product(x, s))]
+        self.kernel_matrix = np.array(product).reshape(len(x), len(s))
+        return self.kernel_matrix
+
+    def element_wise_operation(self, xi_j: Tuple) -> float:
+        xi, xj = xi_j
 
-        :param xi: First point.
-        :param xj: Second point.
-        :return: Float representing the kernel entry.
-        """
         if len(xi.shape) == 1:
             d = pdist(np.array([xi, xj]), "sqeuclidean")
         else:
-            d = np.linalg.norm(xi-xj, 'fro') ** 2
-        return np.exp(-d / (2*self.epsilon**2))
+            d = np.linalg.norm(xi - xj, 'fro') ** 2
+        return np.exp(-d / (2 * self.kernel_parameter ** 2))
 
     def optimize_parameters(self, data: np.ndarray, tolerance: float,
                             n_nearest_neighbors: int,
                             n_cutoff_samples: int,
                             random_state: RandomStateType = None):
         """
```

### Comparing `UQpy-4.1.0/src/UQpy.egg-info/PKG-INFO` & `UQpy-4.1.1/src/UQpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQpy
-Version: 4.1.0
+Version: 4.1.1
 Summary: UQpy is a general purpose toolbox for Uncertainty Quantification
 Home-page: https://github.com/SURGroup/UQpy
 Author: Michael D. Shields, Dimitris G. Giovanis, Audrey Olivier, Aakash Bangalore-Satish, Mohit Chauhan, Lohit Vandanapu, Ketson R.M. dos Santos
 Author-email: UQpy.info@gmail.com
 License: MIT
 Platform: OSX
 Platform: Windows
```

### Comparing `UQpy-4.1.0/src/UQpy.egg-info/SOURCES.txt` & `UQpy-4.1.1/src/UQpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -175,19 +175,14 @@
 src/UQpy/surrogates/baseclass/__init__.py
 src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py
 src/UQpy/surrogates/gaussian_process/__init__.py
 src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py
 src/UQpy/surrogates/gaussian_process/constraints/__init__.py
 src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py
 src/UQpy/surrogates/gaussian_process/constraints/baseclass/__init__.py
-src/UQpy/surrogates/gaussian_process/kernels/Matern.py
-src/UQpy/surrogates/gaussian_process/kernels/RBF.py
-src/UQpy/surrogates/gaussian_process/kernels/__init__.py
-src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py
-src/UQpy/surrogates/gaussian_process/kernels/baseclass/__init__.py
 src/UQpy/surrogates/gaussian_process/regression_models/ConstantRegression.py
 src/UQpy/surrogates/gaussian_process/regression_models/LinearRegression.py
 src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py
 src/UQpy/surrogates/gaussian_process/regression_models/__init__.py
 src/UQpy/surrogates/gaussian_process/regression_models/baseclass/Regression.py
 src/UQpy/surrogates/gaussian_process/regression_models/baseclass/__init__.py
 src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py
@@ -244,15 +239,19 @@
 src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py
 src/UQpy/utilities/distances/grassmannian_distances/__init__.py
-src/UQpy/utilities/kernels/BinetCauchyKernel.py
 src/UQpy/utilities/kernels/GaussianKernel.py
-src/UQpy/utilities/kernels/ProjectionKernel.py
 src/UQpy/utilities/kernels/__init__.py
 src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py
 src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py
 src/UQpy/utilities/kernels/baseclass/Kernel.py
-src/UQpy/utilities/kernels/baseclass/__init__.py
+src/UQpy/utilities/kernels/baseclass/__init__.py
+src/UQpy/utilities/kernels/euclidean_kernels/Matern.py
+src/UQpy/utilities/kernels/euclidean_kernels/RBF.py
+src/UQpy/utilities/kernels/euclidean_kernels/__init__.py
+src/UQpy/utilities/kernels/grassmannian_kernels/BinetCauchyKernel.py
+src/UQpy/utilities/kernels/grassmannian_kernels/ProjectionKernel.py
+src/UQpy/utilities/kernels/grassmannian_kernels/__init__.py
```

