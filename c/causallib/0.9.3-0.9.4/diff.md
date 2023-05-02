# Comparing `tmp/causallib-0.9.3.tar.gz` & `tmp/causallib-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causallib-0.9.3.tar", last modified: Sun Apr 23 20:38:39 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "causallib-0.9.4.tar", last modified: Tue May  2 14:18:35 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `causallib-0.9.3.tar` & `causallib-0.9.4.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     7906 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4800 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/analysis/
--rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.3/causallib/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/
--rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/adversarial_balancing.py
--rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/classifier_selection.py
--rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/__init__.py
--rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/faissknn.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/hemm/
--rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/gen_synthetic_data.py
--rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm.py
--rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_api.py
--rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_metrics.py
--rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_outcome_models.py
--rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_utilities.py
--rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/load_ihdp_data.py
--rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/README.md
--rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.3/causallib/contrib/README.md
--rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/
--rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
--rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/contrib/tests/
--rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/contrib/tests/test_adversarial_balancing.py
--rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/tests/test_hemm.py
--rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/tests/test_shared_sparsity_selection.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/datasets/data/
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/
--rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/x.csv
--rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
--rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
--rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
--rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
--rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
--rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
--rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
--rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
--rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
--rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/data/nhefs/
--rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS.csv
--rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS_codebook.csv
--rw-rw-rw-   0        0        0     9765 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/datasets/data_loader.py
--rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/README.md
--rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/estimation/
--rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/estimation/base_estimator.py
--rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.3/causallib/estimation/base_weight.py
--rw-rw-rw-   0        0        0    26053 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/estimation/doubly_robust.py
--rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/ipw.py
--rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.3/causallib/estimation/marginal_outcome.py
--rw-rw-rw-   0        0        0    38742 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/estimation/matching.py
--rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/overlap_weights.py
--rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/estimation/README.md
--rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.3/causallib/estimation/rlearner.py
--rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/estimation/standardization.py
--rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/tmle.py
--rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/xlearner.py
--rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.3/causallib/estimation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/evaluation/
--rw-rw-rw-   0        0        0     9384 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/evaluator.py
--rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/evaluation/plots/
--rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/curve_data_makers.py
--rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/data_extractors.py
--rw-rw-rw-   0        0        0    14523 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/plots/mixins.py
--rw-rw-rw-   0        0        0    39399 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/plots/plots.py
--rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/__init__.py
--rw-rw-rw-   0        0        0     9034 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/predictions.py
--rw-rw-rw-   0        0        0     8848 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/predictor.py
--rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/README.md
--rw-rw-rw-   0        0        0     7143 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/results.py
--rw-rw-rw-   0        0        0     6566 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/scoring.py
--rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/metrics/
--rw-rw-rw-   0        0        0     3334 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/outcome_metrics.py
--rw-rw-rw-   0        0        0     6426 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/propensity_metrics.py
--rw-rw-rw-   0        0        0     5043 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/scorers.py
--rw-rw-rw-   0        0        0     5076 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/weight_metrics.py
--rw-rw-rw-   0        0        0      370 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/model_selection/
--rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/model_selection/search.py
--rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/model_selection/split.py
--rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/model_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/preprocessing/
--rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/preprocessing/confounder_selection.py
--rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/preprocessing/filters.py
--rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/preprocessing/README.md
--rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.3/causallib/preprocessing/transformers.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/simulation/
--rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/simulation/CausalSimulator3.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/survival/
--rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/base_survival.py
--rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/marginal_survival.py
--rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/regression_curve_fitter.py
--rw-rw-rw-   0        0        0     8700 2023-04-23 19:51:30.000000 causallib-0.9.3/causallib/survival/standardized_survival.py
--rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/survival_utils.py
--rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/univariate_curve_fitter.py
--rw-rw-rw-   0        0        0     3188 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/survival/weighted_standardized_survival.py
--rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/survival/weighted_survival.py
--rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/tests/
--rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.3/causallib/tests/survival_matching.py
--rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/tests/test_base_weight.py
--rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/tests/test_causal_simulator3.py
--rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_confounder_selection.py
--rw-rw-rw-   0        0        0     3769 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/tests/test_datasets.py
--rw-rw-rw-   0        0        0    25686 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_doublyrobust.py
--rw-rw-rw-   0        0        0     5694 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_evaluation.py
--rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_ipw.py
--rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/tests/test_marginal_outcome.py
--rw-rw-rw-   0        0        0    28672 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_matching.py
--rw-rw-rw-   0        0        0    13540 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_metrics.py
--rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_overlap_weights.py
--rw-rw-rw-   0        0        0    10277 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_plots.py
--rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_rlearner.py
--rw-rw-rw-   0        0        0     7796 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_scorers.py
--rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/tests/test_search.py
--rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_split.py
--rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_standardization.py
--rw-rw-rw-   0        0        0    30021 2023-04-23 19:58:37.000000 causallib-0.9.3/causallib/tests/test_survival.py
--rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_tmle.py
--rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/tests/test_transformers.py
--rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/tests/test_utils.py
--rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_xlearner.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/utils/
--rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/utils/crossfit.py
--rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/utils/general_tools.py
--rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/utils/stat_utils.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/utils/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-23 20:01:11.000000 causallib-0.9.3/causallib/__init__.py
--rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     7906 2023-04-23 20:38:07.000000 causallib-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     6787 2023-03-29 12:38:12.000000 causallib-0.9.3/README.md
--rwxrwxrwx   0        0        0      179 2023-03-29 12:20:56.000000 causallib-0.9.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 20:38:07.000000 causallib-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     2792 2023-03-29 12:38:12.000000 causallib-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     7906 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4800 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/analysis/
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.4/causallib/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/
+-rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/adversarial_balancing.py
+-rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/classifier_selection.py
+-rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/__init__.py
+-rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/faissknn.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/hemm/
+-rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/gen_synthetic_data.py
+-rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm.py
+-rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_api.py
+-rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_metrics.py
+-rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_outcome_models.py
+-rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_utilities.py
+-rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/load_ihdp_data.py
+-rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/README.md
+-rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.4/causallib/contrib/README.md
+-rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/
+-rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/tests/
+-rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/contrib/tests/test_adversarial_balancing.py
+-rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/tests/test_hemm.py
+-rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/tests/test_shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/
+-rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/x.csv
+-rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
+-rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
+-rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
+-rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
+-rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
+-rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
+-rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
+-rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
+-rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
+-rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/nhefs/
+-rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS.csv
+-rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS_codebook.csv
+-rw-rw-rw-   0        0        0     9138 2023-05-02 12:28:47.000000 causallib-0.9.4/causallib/datasets/data_loader.py
+-rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/README.md
+-rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/estimation/
+-rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/estimation/base_estimator.py
+-rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.4/causallib/estimation/base_weight.py
+-rw-rw-rw-   0        0        0    26241 2023-05-02 13:20:05.000000 causallib-0.9.4/causallib/estimation/doubly_robust.py
+-rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/ipw.py
+-rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.4/causallib/estimation/marginal_outcome.py
+-rw-rw-rw-   0        0        0    38742 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/estimation/matching.py
+-rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/overlap_weights.py
+-rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/estimation/README.md
+-rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.4/causallib/estimation/rlearner.py
+-rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/estimation/standardization.py
+-rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/tmle.py
+-rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/xlearner.py
+-rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.4/causallib/estimation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/evaluation/
+-rw-rw-rw-   0        0        0     9384 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/evaluator.py
+-rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/evaluation/plots/
+-rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/curve_data_makers.py
+-rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/data_extractors.py
+-rw-rw-rw-   0        0        0    14523 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/plots/mixins.py
+-rw-rw-rw-   0        0        0    39399 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/plots/plots.py
+-rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/__init__.py
+-rw-rw-rw-   0        0        0     9034 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/predictions.py
+-rw-rw-rw-   0        0        0     8848 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/predictor.py
+-rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/README.md
+-rw-rw-rw-   0        0        0     7143 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/results.py
+-rw-rw-rw-   0        0        0     6566 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/scoring.py
+-rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/metrics/
+-rw-rw-rw-   0        0        0     3334 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/outcome_metrics.py
+-rw-rw-rw-   0        0        0     6426 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/propensity_metrics.py
+-rw-rw-rw-   0        0        0     5043 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/scorers.py
+-rw-rw-rw-   0        0        0     5076 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/weight_metrics.py
+-rw-rw-rw-   0        0        0      370 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/model_selection/
+-rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/model_selection/search.py
+-rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/model_selection/split.py
+-rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/model_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/preprocessing/
+-rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/preprocessing/confounder_selection.py
+-rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/preprocessing/filters.py
+-rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/preprocessing/README.md
+-rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.4/causallib/preprocessing/transformers.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/simulation/
+-rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/simulation/CausalSimulator3.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/survival/
+-rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/base_survival.py
+-rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/marginal_survival.py
+-rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/regression_curve_fitter.py
+-rw-rw-rw-   0        0        0     8700 2023-04-23 19:51:30.000000 causallib-0.9.4/causallib/survival/standardized_survival.py
+-rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/survival_utils.py
+-rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/univariate_curve_fitter.py
+-rw-rw-rw-   0        0        0     5013 2023-05-02 13:20:05.000000 causallib-0.9.4/causallib/survival/weighted_standardized_survival.py
+-rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/survival/weighted_survival.py
+-rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/tests/
+-rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.4/causallib/tests/survival_matching.py
+-rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/tests/test_base_weight.py
+-rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/tests/test_causal_simulator3.py
+-rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_confounder_selection.py
+-rw-rw-rw-   0        0        0     7395 2023-05-02 12:28:47.000000 causallib-0.9.4/causallib/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    26809 2023-05-02 13:13:41.000000 causallib-0.9.4/causallib/tests/test_doublyrobust.py
+-rw-rw-rw-   0        0        0     5694 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_evaluation.py
+-rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_ipw.py
+-rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/tests/test_marginal_outcome.py
+-rw-rw-rw-   0        0        0    28672 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_matching.py
+-rw-rw-rw-   0        0        0    13540 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_overlap_weights.py
+-rw-rw-rw-   0        0        0    10277 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_plots.py
+-rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_rlearner.py
+-rw-rw-rw-   0        0        0     7796 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_scorers.py
+-rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/tests/test_search.py
+-rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_split.py
+-rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_standardization.py
+-rw-rw-rw-   0        0        0    32521 2023-05-02 13:49:18.000000 causallib-0.9.4/causallib/tests/test_survival.py
+-rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_tmle.py
+-rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/tests/test_transformers.py
+-rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/tests/test_utils.py
+-rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_xlearner.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/utils/
+-rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/utils/crossfit.py
+-rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/utils/general_tools.py
+-rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/utils/stat_utils.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/utils/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-02 13:50:06.000000 causallib-0.9.4/causallib/__init__.py
+-rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     7906 2023-05-02 13:51:57.000000 causallib-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6787 2023-03-29 12:38:12.000000 causallib-0.9.4/README.md
+-rwxrwxrwx   0        0        0      176 2023-05-02 13:57:24.000000 causallib-0.9.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:51:57.000000 causallib-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     2792 2023-03-29 12:38:12.000000 causallib-0.9.4/setup.py
```

### Comparing `causallib-0.9.3/causallib.egg-info/PKG-INFO` & `causallib-0.9.4/causallib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.3/causallib.egg-info/SOURCES.txt` & `causallib-0.9.4/causallib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/adversarial_balancing/adversarial_balancing.py` & `causallib-0.9.4/causallib/contrib/adversarial_balancing/adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/adversarial_balancing/classifier_selection.py` & `causallib-0.9.4/causallib/contrib/adversarial_balancing/classifier_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/faissknn.py` & `causallib-0.9.4/causallib/contrib/faissknn.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/gen_synthetic_data.py` & `causallib-0.9.4/causallib/contrib/hemm/gen_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/hemm.py` & `causallib-0.9.4/causallib/contrib/hemm/hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/hemm_api.py` & `causallib-0.9.4/causallib/contrib/hemm/hemm_api.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/hemm_metrics.py` & `causallib-0.9.4/causallib/contrib/hemm/hemm_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/hemm_outcome_models.py` & `causallib-0.9.4/causallib/contrib/hemm/hemm_outcome_models.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/hemm_utilities.py` & `causallib-0.9.4/causallib/contrib/hemm/hemm_utilities.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/load_ihdp_data.py` & `causallib-0.9.4/causallib/contrib/hemm/load_ihdp_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/hemm/README.md` & `causallib-0.9.4/causallib/contrib/hemm/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/README.md` & `causallib-0.9.4/causallib/contrib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py` & `causallib-0.9.4/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/tests/test_adversarial_balancing.py` & `causallib-0.9.4/causallib/contrib/tests/test_adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/tests/test_hemm.py` & `causallib-0.9.4/causallib/contrib/tests/test_hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/contrib/tests/test_shared_sparsity_selection.py` & `causallib-0.9.4/causallib/contrib/tests/test_shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/x.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/x.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_1.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_1.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_10.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_10.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_2.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_2.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_3.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_3.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_4.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_4.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_5.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_5.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_6.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_6.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_7.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_7.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_8.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_8.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_9.csv` & `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_9.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS.csv` & `causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS_codebook.csv` & `causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS_codebook.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/datasets/data_loader.py` & `causallib-0.9.4/causallib/datasets/data_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,44 +121,24 @@
 
     Returns:
         X (pd.DataFrame): Baseline covariate matrix of size (num_subjects, num_features).
         a (pd.Series): Treatment assignment of size (num_subjects,). Quit smoking vs. non-quit.
         t (pd.Series): Followup duration, size (num_subjects,).
         y (pd.Series): Observed outcome (1) or right censoring event (0), size (num_subjects,).
     """
+    nhefs_all = load_nhefs(raw=True)[0]
+    t = (nhefs_all["yrdth"] - 83) * 12 + nhefs_all["modth"]
+    t = t.fillna(120)
+    y = nhefs_all["death"]
+
+    nhefs = load_nhefs(augment=augment, onehot=onehot, restrict=False)
+    a = nhefs.a
+    X = nhefs.X
 
-    nhefs_all = load_nhefs(raw=True, augment=augment, onehot=onehot)[0]
-
-    nhefs_all['longevity'] = (nhefs_all.yrdth - 83) * 12 + nhefs_all.modth - 1
-    nhefs_all['longevity'].fillna(120, inplace=True)
-
-    # Pre-process data
-    a = nhefs_all['qsmk']
-    t = nhefs_all['longevity']
-    y = nhefs_all['death']
-    X = nhefs_all[[
-        "sex", "race", "age",
-        "active", "education", "exercise",
-        "smokeintensity", "smokeyrs",
-        "wt71"
-    ]]
-
-    # Add square terms and dummy variables
-    squares = {}
-    for col in ['age', 'wt71', 'smokeintensity', 'smokeyrs']:
-        squares[f'{col}^2'] = X[col] * X[col]
-    X = X.assign(**squares)
-    X = pd.get_dummies(
-        X, columns=["active", "education", "exercise"], drop_first=True
-    )
-
-    # Make timeline 1-index (to comply with some lifelines fitters that require strictly positive time steps)
-    t = t + 1
-
-    data = Bunch(X=X, a=a, t=t, y=y)
+    data = Bunch(X=X, a=a, t=t, y=y, descriptors=nhefs.descriptors)
     return data
 
 
 def load_acic16(instance=1, raw=False):
     """ Loads single dataset from the 2016 Atlantic Causal Inference Conference data challenge.
 
     The dataset is based on real covariates but synthetically simulates the treatment assignment
```

### Comparing `causallib-0.9.3/causallib/datasets/README.md` & `causallib-0.9.4/causallib/datasets/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/base_estimator.py` & `causallib-0.9.4/causallib/estimation/base_estimator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/base_weight.py` & `causallib-0.9.4/causallib/estimation/base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/doubly_robust.py` & `causallib-0.9.4/causallib/estimation/doubly_robust.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,26 @@
         self.weight_covariates = weight_covariates
 
     @abc.abstractmethod
     def fit(self, X, a, y, refit_weight_model=True, **kwargs):
         raise NotImplementedError
 
     def _extract_outcome_model_data(self, X):
-        outcome_covariates = self.outcome_covariates or X.columns
+        if self.outcome_covariates is None:
+            outcome_covariates = X.columns
+        else:
+            outcome_covariates = self.outcome_covariates
         X_outcome = X[outcome_covariates]
         return X_outcome
 
     def _extract_weight_model_data(self, X):
-        weight_covariates = self.weight_covariates or X.columns
+        if self.weight_covariates is None:
+            weight_covariates = X.columns
+        else:
+            weight_covariates = self.weight_covariates
         X_weight = X[weight_covariates]
         return X_weight
 
     def _prepare_data(self, X, a):
         """
         Extract the relevant parts for outcome model and weight model for the entire data matrix
```

### Comparing `causallib-0.9.3/causallib/estimation/ipw.py` & `causallib-0.9.4/causallib/estimation/ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/marginal_outcome.py` & `causallib-0.9.4/causallib/estimation/marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/matching.py` & `causallib-0.9.4/causallib/estimation/matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/overlap_weights.py` & `causallib-0.9.4/causallib/estimation/overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/README.md` & `causallib-0.9.4/causallib/estimation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/rlearner.py` & `causallib-0.9.4/causallib/estimation/rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/standardization.py` & `causallib-0.9.4/causallib/estimation/standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/tmle.py` & `causallib-0.9.4/causallib/estimation/tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/estimation/xlearner.py` & `causallib-0.9.4/causallib/estimation/xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/evaluator.py` & `causallib-0.9.4/causallib/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/metrics.py` & `causallib-0.9.4/causallib/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/plots/curve_data_makers.py` & `causallib-0.9.4/causallib/evaluation/plots/curve_data_makers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/plots/data_extractors.py` & `causallib-0.9.4/causallib/evaluation/plots/data_extractors.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/plots/mixins.py` & `causallib-0.9.4/causallib/evaluation/plots/mixins.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/plots/plots.py` & `causallib-0.9.4/causallib/evaluation/plots/plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/predictions.py` & `causallib-0.9.4/causallib/evaluation/predictions.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/predictor.py` & `causallib-0.9.4/causallib/evaluation/predictor.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/README.md` & `causallib-0.9.4/causallib/evaluation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/results.py` & `causallib-0.9.4/causallib/evaluation/results.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/evaluation/scoring.py` & `causallib-0.9.4/causallib/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/metrics/outcome_metrics.py` & `causallib-0.9.4/causallib/metrics/outcome_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/metrics/propensity_metrics.py` & `causallib-0.9.4/causallib/metrics/propensity_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/metrics/scorers.py` & `causallib-0.9.4/causallib/metrics/scorers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/metrics/weight_metrics.py` & `causallib-0.9.4/causallib/metrics/weight_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/model_selection/search.py` & `causallib-0.9.4/causallib/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/model_selection/split.py` & `causallib-0.9.4/causallib/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/preprocessing/confounder_selection.py` & `causallib-0.9.4/causallib/preprocessing/confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/preprocessing/filters.py` & `causallib-0.9.4/causallib/preprocessing/filters.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/preprocessing/README.md` & `causallib-0.9.4/causallib/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/preprocessing/transformers.py` & `causallib-0.9.4/causallib/preprocessing/transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/README.md` & `causallib-0.9.4/causallib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/simulation/CausalSimulator3.py` & `causallib-0.9.4/causallib/simulation/CausalSimulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/base_survival.py` & `causallib-0.9.4/causallib/survival/base_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/marginal_survival.py` & `causallib-0.9.4/causallib/survival/marginal_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/regression_curve_fitter.py` & `causallib-0.9.4/causallib/survival/regression_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/standardized_survival.py` & `causallib-0.9.4/causallib/survival/standardized_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/survival_utils.py` & `causallib-0.9.4/causallib/survival/survival_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/univariate_curve_fitter.py` & `causallib-0.9.4/causallib/survival/univariate_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/weighted_survival.py` & `causallib-0.9.4/causallib/survival/weighted_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/survival/__init__.py` & `causallib-0.9.4/causallib/survival/__init__.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/survival_matching.py` & `causallib-0.9.4/causallib/tests/survival_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_base_weight.py` & `causallib-0.9.4/causallib/tests/test_base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_causal_simulator3.py` & `causallib-0.9.4/causallib/tests/test_causal_simulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_confounder_selection.py` & `causallib-0.9.4/causallib/tests/test_confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_doublyrobust.py` & `causallib-0.9.4/causallib/tests/test_doublyrobust.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,29 @@
         estimator = estimator.__class__(estimator.outcome_model, estimator.weight_model,
                                         outcome_covariates=[0, 1, 2, 3], weight_covariates=[3, 4])
         estimator.fit(data["X"], data["a"], data["y"])
         self.assertEqual(estimator.outcome_model.learner.coef_.size,
                          len(estimator.outcome_covariates) + n_added_outcome_model_features)
         self.assertEqual(estimator.weight_model.learner.coef_.size, len(estimator.weight_covariates))
 
+    def ensure_fit_with_no_outcome_covariates(self, estimator, n_added_outcome_model_features):
+        data = self.create_uninformative_ox_dataset()
+        # Reinitialize estimator:
+        estimator = estimator.__class__(estimator.outcome_model, estimator.weight_model,
+                                        outcome_covariates=[], weight_covariates=None)
+        estimator.fit(data["X"], data["a"], data["y"])
+        self.assertEqual(
+            estimator.outcome_model.learner.coef_.size,
+            n_added_outcome_model_features
+        )
+        self.assertEqual(
+            estimator.weight_model.learner.coef_.size,
+            data["X"].shape[1]
+        )
+
     def ensure_weight_refitting_refits(self, estimator):
         data = self.create_uninformative_ox_dataset()
         with self.subTest("Test first fit of weight_model did fit the model"):
             estimator.fit(data["X"], data["a"], data["y"])
             self.assertEqual(estimator.weight_model.learner.coef_.size, data["X"].shape[1])
         with self.subTest("Test no-refitting does not refit"):
             estimator.weight_model.learner.coef_ = np.zeros_like(estimator.weight_model.learner.coef_)
@@ -239,14 +254,17 @@
 
     def test_is_fitted(self):
         self.ensure_is_fitted(self.estimator)
 
     def test_data_is_separated_between_models(self):
         self.ensure_data_is_separated_between_models(self.estimator, 1)  # 1 treatment assignment feature
 
+    def test_fit_with_no_outcome_covariates(self):
+        self.ensure_fit_with_no_outcome_covariates(self.estimator, 1)
+
     def test_weight_refitting_refits(self):
         self.ensure_weight_refitting_refits(self.estimator)
 
     def test_model_combinations_work(self):
         self.ensure_model_combinations_work(AIPW)
 
     def test_pipeline_learner(self):
@@ -339,14 +357,18 @@
 
     def test_is_fitted(self):
         self.ensure_is_fitted(self.estimator)
 
     def test_data_is_separated_between_models(self):
         self.ensure_data_is_separated_between_models(self.estimator, 1)  # 1 treatment assignment feature
 
+    def test_fit_with_no_outcome_covariates(self):
+        # Basically an Marginal Structural Model (MSM)
+        self.ensure_fit_with_no_outcome_covariates(self.estimator, 1)
+
     def test_weight_refitting_refits(self):
         self.ensure_weight_refitting_refits(self.estimator)
 
     def test_model_combinations_work(self):
         self.ensure_model_combinations_work(WeightedStandardization)
 
     def test_pipeline_learner(self):
@@ -449,14 +471,17 @@
 
     def test_is_fitted(self):
         self.ensure_is_fitted(self.estimator)
 
     def test_data_is_separated_between_models(self):
         self.ensure_data_is_separated_between_models(self.estimator, 1 + 1)  # 1 ip-feature + 1 treatment assignment
 
+    def test_fit_with_no_outcome_covariates(self):
+        self.ensure_fit_with_no_outcome_covariates(self.estimator, 1 + 1)
+
     def test_weight_refitting_refits(self):
         self.ensure_weight_refitting_refits(self.estimator)
 
     def test_model_combinations_work(self):
         self.ensure_model_combinations_work(PropensityFeatureStandardization)
 
     def test_pipeline_learner(self):
```

### Comparing `causallib-0.9.3/causallib/tests/test_evaluation.py` & `causallib-0.9.4/causallib/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_ipw.py` & `causallib-0.9.4/causallib/tests/test_ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_marginal_outcome.py` & `causallib-0.9.4/causallib/tests/test_marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_matching.py` & `causallib-0.9.4/causallib/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_metrics.py` & `causallib-0.9.4/causallib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_overlap_weights.py` & `causallib-0.9.4/causallib/tests/test_overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_plots.py` & `causallib-0.9.4/causallib/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_rlearner.py` & `causallib-0.9.4/causallib/tests/test_rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_scorers.py` & `causallib-0.9.4/causallib/tests/test_scorers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_search.py` & `causallib-0.9.4/causallib/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_split.py` & `causallib-0.9.4/causallib/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_standardization.py` & `causallib-0.9.4/causallib/tests/test_standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_survival.py` & `causallib-0.9.4/causallib/tests/test_survival.py`

 * *Files 8% similar despite different names*

```diff
@@ -542,14 +542,56 @@
                   'survival_model': LogisticRegression(max_iter=4000, C=5),
                   'stratify': False}
         adjusted_diff = fit_synthetic_data(model_cls=model, params=params, test_data=test_data)
 
         self.assertAlmostEqual(adjusted_diff, TEST_DATA_DRUG_EFFECTS_A_ORACLE_DIFF,
                                delta=TEST_DATA_DRUG_EFFECTS_DELTA)
 
+    def test_different_covariates_per_model(self):
+        data = TEST_DATA_TTE_DRUG_EFFECTS['A']
+        X = data[['x_0', 'x_1']]
+        a, t, y = data['a'], data['t'], data['y']
+
+        model = WeightedStandardizedSurvival(
+            weight_model=IPW(LogisticRegression(max_iter=2000)),
+            survival_model=LogisticRegression(max_iter=4000),
+            stratify=False,
+            weight_covariates=["x_0"],
+            outcome_covariates=None,
+        )
+        model.fit(X, a, t, y)
+
+        # Weight model is fitted only on `x_0`:
+        self.assertEqual(model.weight_model.learner.coef_.size, 1)
+        # Outcome model is fitted on all `x_0, x_1` and treatment and time:
+        self.assertEqual(model.survival_model.learner.coef_.size, 2 + 1 + 1)
+
+        po = model.estimate_population_outcome(X, a, t)
+
+    def test_fit_with_no_outcome_covariates(self):
+        data = TEST_DATA_TTE_DRUG_EFFECTS['A']
+        X = data[['x_0', 'x_1']]
+        a, t, y = data['a'], data['t'], data['y']
+
+        model = WeightedStandardizedSurvival(
+            weight_model=IPW(LogisticRegression(max_iter=2000)),
+            survival_model=LogisticRegression(max_iter=4000),
+            stratify=False,
+            weight_covariates=None,
+            outcome_covariates=[],
+        )
+        model.fit(X, a, t, y)
+
+        # Weight model is fitted on both `x_0, x_1`:
+        self.assertEqual(model.weight_model.learner.coef_.size, 2)
+        # Outcome model is fitted only on a treatment indicator and time:
+        self.assertEqual(model.survival_model.learner.coef_.size, 1 + 1)
+
+        po = model.estimate_population_outcome(X, a, t)
+
 
 @unittest.skipUnless(LIFELINES_FOUND, 'lifelines not found')
 class TestLifelines(unittest.TestCase):
     """
     Test integration with 'lifelines' Python package.
     """
     def setUp(self) -> None:
@@ -647,14 +689,35 @@
         with self.subTest("Unstratified Cox Regression"):
             model = StandardizedSurvival(
                 lifelines.CoxPHFitter(penalizer=10),
                 stratify=False,
             )
             ensure_individual_estimation(model, data)
 
+    def test_fit_with_no_outcome_covariates(self):
+        data = TEST_DATA_TTE_DRUG_EFFECTS['A']
+        X = data[['x_0', 'x_1']]
+        a, t, y = data['a'], data['t'], data['y']
+
+        model = WeightedStandardizedSurvival(
+            weight_model=IPW(LogisticRegression(max_iter=2000)),
+            survival_model=lifelines.CoxPHFitter(),
+            stratify=False,
+            weight_covariates=None,
+            outcome_covariates=[],
+        )
+        model.fit(X, a, t, y)
+
+        # Weight model is fitted on both `x_0, x_1`:
+        self.assertEqual(model.weight_model.learner.coef_.size, 2)
+        # Outcome model is fitted only on a treatment indicator:
+        self.assertEqual(model.survival_model.params_.size, 1)
+
+        po = model.estimate_population_outcome(X, a, t)
+
 
 class TestFeatureTransform(unittest.TestCase):
     """
     Test scikit-learn Pipeline/transform as a base learner for standardized survival curves.
     """
     def setUp(self) -> None:
         test_data = TEST_DATA_TTE_DRUG_EFFECTS['A']
```

### Comparing `causallib-0.9.3/causallib/tests/test_tmle.py` & `causallib-0.9.4/causallib/tests/test_tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_transformers.py` & `causallib-0.9.4/causallib/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_utils.py` & `causallib-0.9.4/causallib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/tests/test_xlearner.py` & `causallib-0.9.4/causallib/tests/test_xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/utils/crossfit.py` & `causallib-0.9.4/causallib/utils/crossfit.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/utils/general_tools.py` & `causallib-0.9.4/causallib/utils/general_tools.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/causallib/utils/stat_utils.py` & `causallib-0.9.4/causallib/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/LICENSE` & `causallib-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/PKG-INFO` & `causallib-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.3/README.md` & `causallib-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.3/setup.py` & `causallib-0.9.4/setup.py`

 * *Files identical despite different names*

