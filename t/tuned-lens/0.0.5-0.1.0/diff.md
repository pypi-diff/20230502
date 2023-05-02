# Comparing `tmp/tuned-lens-0.0.5.tar.gz` & `tmp/tuned-lens-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuned-lens-0.0.5.tar", last modified: Wed Apr 19 16:10:28 2023, max compression
+gzip compressed data, was "tuned-lens-0.1.0.tar", last modified: Tue May  2 01:29:34 2023, max compression
```

## Comparing `tuned-lens-0.0.5.tar` & `tuned-lens-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:27.999213 tuned-lens-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_load_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_subspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/ablation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/model_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/_model_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/downstream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/lenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/plotting/plot_lens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/residual_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/argparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/cbe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/downstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/eval_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/train_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/tuned_lens/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/logit_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/residual_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/scripts/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_load_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_model_surgery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_unembed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tuned_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/ablation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/model_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/unembed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/prediction_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/token_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/trajectory_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/eval_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/train_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/logit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tuned_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/top_level.txt
```

### Comparing `tuned-lens-0.0.5/LICENSE` & `tuned-lens-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.5/PKG-INFO` & `tuned-lens-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `tuned-lens-0.0.5/README.md` & `tuned-lens-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.5/pyproject.toml` & `tuned-lens-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,59 +12,59 @@
 dependencies = [
     "accelerate",
     "datasets",
     "plotly>=5.13.1",
     "scikit-learn",
     "zstandard",
     "torch>=1.13.0",
-    "transformers",
+    "transformers>=4.28.1",
     "huggingface_hub>=0.12.1",
+    "simple-parsing>=0.1.1",
+    "wandb>=0.15.0",
 ]
-version = "0.0.5"
+version = "0.1.0"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "bump2version",
     "pytest-skip-slow",
     "pytest",
 ]
 docs = [
     "furo",
     "myst-parser",
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-rtd-theme",
+    "nbsphinx",
 ]
 test = [
     "pytest-skip-slow",
     "pytest-cov",
+    "nbmake",
     "pytest",
     "mock",
 ]
 notebooks = [
     "ipywidgets",
 ]
 
 [project.scripts]
-tuned-lens = "tuned_lens.__main__:run"
+tuned-lens = "tuned_lens.__main__:main"
 
 [tool.setuptools.packages.find]
 namespaces = false
 
-[tool.pytest.ini_options]
-addini = "slow : mark tests as slow these will be skipped by default"
-
 [tool.ruff]
-# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F", "D"]
+select = ["E", "F", "D", "I"]
 ignore = []
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
+fixable = ["A", "B", "C", "D", "E", "F", "I"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
@@ -103,10 +103,8 @@
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "docs/**.py" = ["D"]
 "tests/**.py" = ["D"]
-"tuned_lens/stats/**.py" = ["D"]
 "tuned_lens/causal/**.py" = ["D"]
-"tuned_lens/nn/probe_dict.py" = ["D"]
```

### Comparing `tuned-lens-0.0.5/tests/test_subspaces.py` & `tuned-lens-0.1.0/tests/test_subspaces.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from tuned_lens.causal import remove_subspace
 import pytest
 import torch as th
 
+from tuned_lens.causal import remove_subspace
+
 
 @pytest.mark.parametrize("d", list(range(1, 1000, 100)))
 def test_remove_subspace(d: int):
     a = th.randn(10, d, dtype=th.float64)
 
     for k in range(1, d, 10):
         b = th.randn(d, k, dtype=th.float64)
```

### Comparing `tuned-lens-0.0.5/tuned_lens/causal/ablation.py` & `tuned-lens-0.1.0/tuned_lens/causal/ablation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Provides tools for ablating layers of a transformer model."""
-from ..model_surgery import get_transformer_layers
-from .utils import derange
 from contextlib import contextmanager
 from typing import Literal
+
 import torch as th
 
+from ..model_surgery import get_transformer_layers
+from .utils import derange
+
 
 @contextmanager
 def ablate_layer(
     model: th.nn.Module,
     layer_index: int,
     method: Literal["resample", "mean", "zero"],
     *,
```

### Comparing `tuned-lens-0.0.5/tuned_lens/causal/subspaces.py` & `tuned-lens-0.1.0/tuned_lens/causal/subspaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""Provides tools for extracting causal bases from models and ablating subspaces"""
-from ..model_surgery import get_transformer_layers
-from ..nn import Decoder, TunedLens
-from ..utils import maybe_all_reduce
-from .utils import derange
+"""Provides tools for extracting causal bases from models and ablating subspaces."""
 from contextlib import contextmanager
-from tqdm.auto import trange
-from typing import Iterable, Literal, NamedTuple, Optional, Union, Sequence
+from typing import Iterable, Literal, NamedTuple, Optional, Sequence
+
 import torch as th
 import torch.distributed as dist
 import torch.nn.functional as F
+from tqdm.auto import trange
+
+from ..model_surgery import get_transformer_layers
+from ..nn import Lens
+from ..utils import maybe_all_reduce
+from .utils import derange
 
 
 @contextmanager
 def ablate_subspace(
     model: th.nn.Module,
     A: th.Tensor,
     layer_index: int,
@@ -22,14 +24,16 @@
     """Context manager that ablates a subspace of activations.
 
     Args:
         model: A hugging face transformer model.
         A: Either a 2D matrix whose column space is to be removed, or a 1D vector whose
             span is to be removed.
         layer_index: The index of the layer to ablate.
+        mode: Which method to use for removing information along the subspace.
+            Defaults to `"zero"`.
         orthonormal: if True, `A` is assumed to be orthonormal.
     """
     _, layers = get_transformer_layers(model)
 
     def wrapper(_, __, outputs):
         h, *extras = outputs
         h_ = remove_subspace(h, A, mode, orthonormal)
@@ -57,33 +61,33 @@
     """
 
     energies: th.Tensor
     vectors: th.Tensor
 
 
 def extract_causal_bases(
-    model: Union[Decoder, TunedLens],
+    lens: Lens,
     hiddens: Sequence[th.Tensor],
     k: int,
     *,
     labels: Optional[th.Tensor] = None,
     max_iter: int = 100,
     mode: Literal["mean", "resample", "zero"] = "mean",
-    no_translator: bool = False,
 ) -> Iterable[CausalBasis]:
     """Extract causal bases for probes at each layer of a model.
 
     Args:
-        model: A model to compute causal bases for. This can be a `Decoder` or a
-            `TunedLens` instance.
+        lens: A lens to compute causal bases for.
         hiddens: A sequence of hidden states from the model.
         k: The number of basis vectors to compute for each layer.
         max_iter: The maximum number of iterations to run L-BFGS for each vector.
+        mode: Which method to use for removing information along the subspace.
+            Defaults to `"zero"`.
     """
-    model.requires_grad_(False)
+    lens.requires_grad_(False)
 
     device = hiddens[0].device
     dtype = hiddens[0].dtype
     d = hiddens[0].shape[-1]
 
     hiddens = [h.detach() for h in hiddens]
     num_layers = len(hiddens) - 1
@@ -95,29 +99,19 @@
     eye = th.eye(d, device=device, dtype=dtype)
 
     show_pbar = not dist.is_initialized() or dist.get_rank() == 0
     pbar = trange(num_layers * k) if show_pbar else None
 
     # Outer loop iterates over layers
     for i in range(num_layers):
-        U = model.unembedding.weight.data.T
+        U = lens.unembed.unembedding.weight.data.T
 
-        if isinstance(model, Decoder):
-            log_p = model(hiddens[i]).log_softmax(-1)
-
-        elif isinstance(model, TunedLens):
-            logits = (
-                model(hiddens[i], i)
-                if not no_translator
-                else model.to_logits(hiddens[i])
-            )
-            log_p = logits.log_softmax(-1)
-            U = (eye + model[i].weight.data.T) @ U
-        else:
-            raise NotImplementedError()
+        logits = lens(hiddens[i], i)
+        log_p = logits.log_softmax(-1)
+        U = lens.transform_hidden(U, i)  # TODO not sure if we need transposes here
 
         # Compute the baseline loss up front so that we can subtract it
         # from the post-ablation losses to get the loss increment
         if labels is not None:
             base_loss = F.cross_entropy(
                 log_p[:, :-1].flatten(0, -2), labels[:, 1:].flatten()
             )
@@ -166,20 +160,15 @@
                 nonlocal energy_delta, nfev, last_energy
                 nfev += 1
 
                 opt.zero_grad(set_to_none=False)
                 v_ = project(v)
                 h_ = remove_subspace(hiddens[i], v_, mode=mode, orthonormal=True)
 
-                if isinstance(model, Decoder):
-                    logits = model(h_)
-                elif isinstance(model, TunedLens):
-                    logits = model(h_, i)
-                else:
-                    raise TypeError(f"Unknown lens type {type(model)}")
+                logits = lens(h_, i)
 
                 if labels is not None:
                     loss = -F.cross_entropy(
                         logits[:, :-1].flatten(0, 1), labels[:, 1:].flatten()
                     )
                 else:
                     log_q = logits.log_softmax(-1)
```

### Comparing `tuned-lens-0.0.5/tuned_lens/causal/utils.py` & `tuned-lens-0.1.0/tuned_lens/causal/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
+
 import torch as th
 
 
 def derange(batch: th.Tensor, generator: Optional[th.Generator] = None) -> th.Tensor:
     """Shuffle a tensor along axis 0, making sure there are no fixed points."""
-
     # Things get more complicated if there are multiple ranks. We perform the
     # derangement *hierarchically*, first generating a shared permutation of the ranks
     indices = sample_derangement(
         batch.shape[0], device=batch.device, generator=generator
     )
     return batch[indices]
```

### Comparing `tuned-lens-0.0.5/tuned_lens/load_artifacts.py` & `tuned-lens-0.1.0/tuned_lens/load_artifacts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Load lens artifacts from the hub or locally storage."""
-from typing import Optional, Tuple
-from pathlib import Path
 import os
+from pathlib import Path
+from typing import Optional
 
 from huggingface_hub import hf_hub_download
 
 
 def load_lens_artifacts(
     resource_id: str,
     repo_id: Optional[str] = None,
     repo_type: Optional[str] = None,
     revision: Optional[str] = None,
     config_file: str = "config.json",
     ckpt_file: str = "params.pt",
     subfolder: str = "lens",
-) -> Tuple[Path, Path]:
+    cache_dir: Optional[str] = None,
+) -> tuple[Path, Path]:
     """First checks for lens resource locally then tries to download it from the hub.
 
     Args:
         resource_id: The id of the lens resource.
         repo_id: The repository to download the lens from. Defaults to
             'AlignmentResearch/tuned-lens'. However, this default can be overridden by
             setting the TUNED_LENS_REPO_ID environment variable.
         repo_type: The type of repository to download the lens from. Defaults to
             'space'. However, this default can be overridden by setting the
             TUNED_LENS_REPO_TYPE environment variable.
         config_file: The name of the config file in the folder contain the lens.
         ckpt_file: The name of the checkpoint file in the folder contain the lens.
         revision: The revision of the lens to download.
         subfolder: The subfolder of the repository to download the lens from.
+        cache_dir: The directory to cache the lens in.
 
     Returns:
         * The path to the config.json file
         * The path to the params.pt file
 
     Raises:
         ValueError: if the lens resource could not be found.
@@ -57,21 +59,23 @@
     subfolder = "/".join((subfolder, resource_id))
     params_path = hf_hub_download(
         filename=ckpt_file,
         repo_id=repo_id,
         repo_type=repo_type,
         revision=revision,
         subfolder=subfolder,
+        cache_dir=cache_dir,
     )
 
     config_path = hf_hub_download(
         filename=config_file,
         repo_id=repo_id,
         repo_type=repo_type,
         revision=revision,
         subfolder=subfolder,
+        cache_dir=cache_dir,
     )
 
     if config_path is not None and params_path is not None:
         return Path(config_path), Path(params_path)
 
     raise ValueError("Could not find lens resource locally or on the hf hub.")
```

### Comparing `tuned-lens-0.0.5/tuned_lens/stats/logit_stats.py` & `tuned-lens-0.1.0/tuned_lens/stats/logit_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from torch.distributions import Dirichlet
+"""Online MLE for the Dirichlet distribution from which logits are sampled."""
 from typing import Optional
-from ..utils import maybe_all_reduce
+
 import torch as th
+from torch.distributions import Dirichlet
+
+from ..utils import maybe_all_reduce
 
 
 class LogitStats:
     """Online MLE for the Dirichlet distribution from which logits are sampled.
 
     Shape and device are lazily inferred from the first stream that is passed to
     `update()`. Only a running mean of the log-likelihoods for each class is stored,
@@ -14,25 +17,27 @@
     """
 
     n: int
     marginal_probs: Optional[th.Tensor]
     sufficient_stats: Optional[th.Tensor]
 
     def __init__(self):
+        """Create a LogitStats object."""
         self.n = 0
         self.marginal_probs = None
         self.sufficient_stats = None
 
     def all_reduce_(self):
         """All-reduce the stats across all processes."""
         if self.sufficient_stats is not None:
             maybe_all_reduce(self.sufficient_stats)
 
     @th.no_grad()
     def update(self, logits: th.Tensor, assume_normalized: bool = False):
+        """Update the sufficient statistics with a new batch of logits."""
         K = logits.shape[-1]
         logits = logits.reshape(-1, K).float()
         if not assume_normalized:
             logits = logits.log_softmax(dim=-1)
 
         N = logits.shape[0]
         if self.marginal_probs is None:
```

### Comparing `tuned-lens-0.0.5/tuned_lens/utils.py` & `tuned-lens-0.1.0/tuned_lens/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Utilities for distributed training and handling nested collections of tensors."""
 
+import hashlib
 from itertools import islice
-from typing import cast, Any, Callable, Iterable, Sequence, Type, TypeVar, Union
+from typing import Any, Callable, Iterable, Sequence, Type, TypeVar, Union, cast
+
+import numpy as np
 import torch as th
 import torch.distributed as dist
-
+from numpy.typing import NDArray
 
 T = TypeVar("T")
 
 
 def assert_type(typ: Type[T], obj: Any) -> T:
     """Assert that an object is of a given type at runtime and return it."""
     if not isinstance(obj, typ):
@@ -228,7 +231,17 @@
     sums.reverse()
     return sums
 
 
 def send_to_device(tree: TreeType, device: th.device) -> TreeType:
     """Recursively send all tensors in a pytree to a device."""
     return pytree_map(lambda t: t.to(device), tree)
+
+
+def tensor_hash(tensor: NDArray) -> str:
+    """Fast hash of a matrix that is robust to dtype and small perturbations.
+
+    Note this relies on the ordering of the elements in the matrix, so it is
+    if the matrix is in any way sorted this will not work well. In addition,
+    this hash is intended for large tensors 64 + elements.
+    """
+    return hashlib.sha256(str.encode(np.array_str(tensor, precision=1))).hexdigest()
```

### Comparing `tuned-lens-0.0.5/tuned_lens.egg-info/PKG-INFO` & `tuned-lens-0.1.0/tuned_lens.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `tuned-lens-0.0.5/tuned_lens.egg-info/SOURCES.txt` & `tuned-lens-0.1.0/tuned_lens.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 tests/__init__.py
-tests/test_decoder.py
+tests/conftest.py
+tests/test_data.py
 tests/test_distance.py
-tests/test_feature_extraction.py
 tests/test_lenses.py
 tests/test_load_artifact.py
-tests/test_plotting.py
+tests/test_model_surgery.py
 tests/test_stats.py
 tests/test_subspaces.py
+tests/test_unembed.py
+tests/test_utils.py
+tests/scripts/__init__.py
+tests/scripts/test_integration.py
 tuned_lens/__init__.py
 tuned_lens/__main__.py
 tuned_lens/data.py
 tuned_lens/load_artifacts.py
 tuned_lens/model_surgery.py
-tuned_lens/residual_stream.py
 tuned_lens/utils.py
 tuned_lens.egg-info/PKG-INFO
 tuned_lens.egg-info/SOURCES.txt
 tuned_lens.egg-info/dependency_links.txt
 tuned_lens.egg-info/entry_points.txt
 tuned_lens.egg-info/requires.txt
 tuned_lens.egg-info/top_level.txt
 tuned_lens/causal/__init__.py
 tuned_lens/causal/ablation.py
 tuned_lens/causal/subspaces.py
 tuned_lens/causal/utils.py
 tuned_lens/nn/__init__.py
-tuned_lens/nn/_model_specific.py
-tuned_lens/nn/decoder.py
-tuned_lens/nn/downstream_wrapper.py
 tuned_lens/nn/lenses.py
+tuned_lens/nn/unembed.py
 tuned_lens/plotting/__init__.py
-tuned_lens/plotting/plot_lens.py
+tuned_lens/plotting/prediction_trajectory.py
+tuned_lens/plotting/token_formatter.py
+tuned_lens/plotting/trajectory_plotting.py
 tuned_lens/scripts/__init__.py
-tuned_lens/scripts/argparsers.py
-tuned_lens/scripts/cbe.py
-tuned_lens/scripts/downstream.py
 tuned_lens/scripts/eval_loop.py
-tuned_lens/scripts/lens.py
+tuned_lens/scripts/ingredients.py
 tuned_lens/scripts/train_loop.py
 tuned_lens/stats/__init__.py
-tuned_lens/stats/anomaly.py
-tuned_lens/stats/dimensionality.py
 tuned_lens/stats/distance.py
-tuned_lens/stats/logit_stats.py
-tuned_lens/stats/rank.py
-tuned_lens/stats/residual_stats.py
+tuned_lens/stats/logit_stats.py
```

