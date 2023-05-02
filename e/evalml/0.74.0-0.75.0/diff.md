# Comparing `tmp/evalml-0.74.0.tar.gz` & `tmp/evalml-0.75.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-cri8awbd/evalml-0.74.0.tar", last modified: Wed Apr 19 16:24:47 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-zhlwywqf/evalml-0.75.0.tar", last modified: Tue May  2 17:20:46 2023, max compression
```

## Comparing `evalml-0.74.0.tar` & `evalml-0.75.0.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/
--rw-r--r--   0 root         (0) root         (0)     1513 2023-04-19 16:24:34.000000 evalml-0.74.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8233 2023-04-19 16:24:47.000000 evalml-0.74.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-19 16:24:34.000000 evalml-0.74.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/automl/
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/automl/automl_algorithm/
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/automl_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11921 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/automl_algorithm/automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    29145 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/automl_algorithm/default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    21384 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/automl_algorithm/iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    79676 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/automl_search.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/automl/engine/
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/engine/cf_engine.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/engine/dask_engine.py
--rw-r--r--   0 root         (0) root         (0)    15405 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/engine/engine_base.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/engine/sequential_engine.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/progress.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/automl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/data_checks/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_action.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_action_code.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     3156 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_message.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_message_code.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_check_message_type.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/data_checks.py
--rw-r--r--   0 root         (0) root         (0)    25088 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/default_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    20762 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)    11843 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    17159 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7242 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8124 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/data_checks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/demos/
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/churn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/demos/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     1103 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/diabetes.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/fraud.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/weather.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/demos/wine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/exceptions/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/exceptions/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/model_family/
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_family/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_family/model_family.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_family/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/model_understanding/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/_partial_dependence_utils.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/force_plots.py
--rw-r--r--   0 root         (0) root         (0)    15125 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/metrics.py
--rw-r--r--   0 root         (0) root         (0)    27420 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/partial_dependence_functions.py
--rw-r--r--   0 root         (0) root         (0)    13556 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/permutation_importance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
--rw-r--r--   0 root         (0) root         (0)    36936 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15630 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/prediction_explanations/explainers.py
--rw-r--r--   0 root         (0) root         (0)    22293 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/model_understanding/visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/objectives/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/fraud_cost.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/multiclass_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/objective_base.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/sensitivity_low_alert.py
--rw-r--r--   0 root         (0) root         (0)    33865 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/standard_metrics.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/time_series_regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     6835 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/objectives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/binary_classification_pipeline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     7845 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    40232 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/component_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10149 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/component_base.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/component_base_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/ensemble/
--rw-r--r--   0 root         (0) root         (0)      349 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/estimators/
--rw-r--r--   0 root         (0) root         (0)      964 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/
--rw-r--r--   0 root         (0) root         (0)     1445 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8797 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4811 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8530 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13466 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7329 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5128 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/
--rw-r--r--   0 root         (0) root         (0)     1478 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6235 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/column_selectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
--rw-r--r--   0 root         (0) root         (0)    13779 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12206 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/
--rw-r--r--   0 root         (0) root         (0)      599 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8253 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/imputer.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    11389 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)    17526 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/samplers/
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
--rw-r--r--   0 root         (0) root         (0)     7283 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/samplers/oversampler.py
--rw-r--r--   0 root         (0) root         (0)     8265 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/samplers/undersampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/pipelines/components/transformers/scalers/
--rw-r--r--   0 root         (0) root         (0)      141 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/scalers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)    18498 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/components/utils.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/multiclass_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    33022 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/pipeline_meta.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    17176 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/time_series_classification_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    15153 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/time_series_pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    12880 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/time_series_regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    53306 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/no_split.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     5599 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/time_series_split.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/data_splitters/training_validation_split.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/preprocessing/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/problem_types/
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/problem_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/problem_types/problem_types.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/problem_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/automl_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/dask_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
--rw-r--r--   0 root         (0) root         (0)    17604 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
--rw-r--r--   0 root         (0) root         (0)    14529 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
--rw-r--r--   0 root         (0) root         (0)   179543 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38707 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38820 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_classification.py
--rw-r--r--   0 root         (0) root         (0)    15745 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
--rw-r--r--   0 root         (0) root         (0)     8716 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_regression.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
--rw-r--r--   0 root         (0) root         (0)    12934 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_automl_utils.py
--rw-r--r--   0 root         (0) root         (0)    32956 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_engine_base.py
--rw-r--r--   0 root         (0) root         (0)    36749 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_search_iterative.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/automl_tests/test_time_series_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/component_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27084 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    11644 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_column_selector_transformers.py
--rw-r--r--   0 root         (0) root         (0)    64838 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_components.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_en_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_en_regressor.py
--rw-r--r--   0 root         (0) root         (0)    15118 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_estimators.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_feature_selectors.py
--rw-r--r--   0 root         (0) root         (0)    14950 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_featuretools.py
--rw-r--r--   0 root         (0) root         (0)     9627 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
--rw-r--r--   0 root         (0) root         (0)    25736 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_imputer.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_knn_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     8017 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_label_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_lda.py
--rw-r--r--   0 root         (0) root         (0)    13414 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_lgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     9754 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_lgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8111 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_lsa.py
--rw-r--r--   0 root         (0) root         (0)    20457 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     9988 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_nullable_types_replacer.py
--rw-r--r--   0 root         (0) root         (0)    26816 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_one_hot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    25966 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)    19941 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_oversampler.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_pca.py
--rw-r--r--   0 root         (0) root         (0)    12025 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)    23430 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)    18269 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)    10542 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_target_encoder.py
--rw-r--r--   0 root         (0) root         (0)     9398 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    30311 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    24722 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_time_series_imputer.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     6246 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_undersampler.py
--rw-r--r--   0 root         (0) root         (0)     9766 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/component_tests/test_xgboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)    80070 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     9729 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data/tips.csv
--rw-r--r--   0 root         (0) root         (0)    61194 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data/titanic.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/data_checks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24199 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_action.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_message.py
--rw-r--r--   0 root         (0) root         (0)    29212 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)    12185 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    30182 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    26417 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)    18212 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/data_checks_tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/demo_tests/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/dependency_update_check/
--rw-r--r--   0 root         (0) root         (0)      636 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/dependency_update_check/minimum_requirements.txt
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10709 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
--rw-r--r--   0 root         (0) root         (0)     5184 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/integration_tests/test_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/integration_tests/test_time_series_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/model_family_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_family_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_family_tests/test_model_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
--rw-r--r--   0 root         (0) root         (0)    67430 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
--rw-r--r--   0 root         (0) root         (0)    19357 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)    14744 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)    26774 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    98520 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
--rw-r--r--   0 root         (0) root         (0)    29313 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/model_understanding_tests/test_visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/objective_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_fraud_detection.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_objectives.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_sla.py
--rw-r--r--   0 root         (0) root         (0)    27155 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/objective_tests/test_standard_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
--rw-r--r--   0 root         (0) root         (0)    94308 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_component_graph.py
--rw-r--r--   0 root         (0) root         (0)     8969 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_graphs.py
--rw-r--r--   0 root         (0) root         (0)    49985 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
--rw-r--r--   0 root         (0) root         (0)   101164 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    68369 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/test_no_split.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/test_split_data.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/problem_type_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/problem_type_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/problem_type_tests/test_problem_types.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/test_all_test_dirs_included.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/tuner_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/tuner_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/tuner_tests/test_random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     9170 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/tuner_tests/test_skopt_tuner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    30486 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     4685 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/test_nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)    12628 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tests/utils_tests/test_woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/tuners/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/skopt_tuner.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/tuner.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/tuners/tuner_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml/utils/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/base_meta.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    26270 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/update_checker.py
--rw-r--r--   0 root         (0) root         (0)     6346 2023-04-19 16:24:34.000000 evalml-0.74.0/evalml/utils/woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8233 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20684 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1229 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-19 16:24:47.000000 evalml-0.74.0/evalml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5012 2023-04-19 16:24:34.000000 evalml-0.74.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 16:24:47.000000 evalml-0.74.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-05-02 17:20:32.000000 evalml-0.75.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-02 17:20:46.000000 evalml-0.75.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-05-02 17:20:32.000000 evalml-0.75.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/automl_algorithm/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    29145 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    21384 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    79617 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_search.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/engine/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)    15405 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/engine_base.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/sequential_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/progress.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/data_checks/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action_code.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message_code.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    25088 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/default_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    20762 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    17159 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8124 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/demos/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/churn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/demos/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/diabetes.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/fraud.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/weather.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/wine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/exceptions/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_family/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/model_family.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_understanding/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/_partial_dependence_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    15125 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    27420 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/partial_dependence_functions.py
+-rw-r--r--   0 root         (0) root         (0)    13556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/permutation_importance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
+-rw-r--r--   0 root         (0) root         (0)    36936 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15630 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/explainers.py
+-rw-r--r--   0 root         (0) root         (0)    22293 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/objectives/
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/fraud_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/multiclass_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/objective_base.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/sensitivity_low_alert.py
+-rw-r--r--   0 root         (0) root         (0)    33865 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/standard_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/time_series_regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     6835 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/binary_classification_pipeline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    40232 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/component_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/component_base.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/component_base_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8797 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8530 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13466 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/column_selectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    13779 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12206 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/imputer.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    15805 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/undersampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    18498 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/multiclass_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    33022 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/pipeline_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_classification_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    15747 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    53306 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/no_split.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/time_series_split.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/training_validation_split.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/problem_types/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/problem_types.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/automl_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/dask_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
+-rw-r--r--   0 root         (0) root         (0)    17604 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)    14529 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)   179549 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38707 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38820 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification.py
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    32956 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_engine_base.py
+-rw-r--r--   0 root         (0) root         (0)    36749 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_search_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_time_series_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/component_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27084 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    11644 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_column_selector_transformers.py
+-rw-r--r--   0 root         (0) root         (0)    64838 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_components.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_en_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_en_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    15118 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_estimators.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_feature_selectors.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
+-rw-r--r--   0 root         (0) root         (0)    25736 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_knn_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     8017 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lda.py
+-rw-r--r--   0 root         (0) root         (0)    13414 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9754 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lsa.py
+-rw-r--r--   0 root         (0) root         (0)    20457 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_nullable_types_replacer.py
+-rw-r--r--   0 root         (0) root         (0)    26816 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_one_hot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    25966 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_pca.py
+-rw-r--r--   0 root         (0) root         (0)    12025 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    23430 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_target_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    30311 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    24722 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_undersampler.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_xgboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    80070 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     9729 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/tips.csv
+-rw-r--r--   0 root         (0) root         (0)    61194 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/titanic.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/data_checks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24199 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    12185 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    30182 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    26417 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/demo_tests/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/dependency_update_check/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/minimum_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_time_series_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_family_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_family_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_family_tests/test_model_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)    67430 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)    26774 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    98520 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/objective_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_fraud_detection.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_objectives.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_sla.py
+-rw-r--r--   0 root         (0) root         (0)    27155 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_standard_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_component_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_graphs.py
+-rw-r--r--   0 root         (0) root         (0)    49985 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
+-rw-r--r--   0 root         (0) root         (0)   101164 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    70356 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_no_split.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_split_data.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/problem_type_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/problem_type_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/problem_type_tests/test_problem_types.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/test_all_test_dirs_included.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/tuner_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     9170 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_skopt_tuner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30486 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tuners/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/skopt_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/tuner.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/tuner_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/utils/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/base_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26270 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/update_checker.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20684 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-05-02 17:20:32.000000 evalml-0.75.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 17:20:46.000000 evalml-0.75.0/setup.cfg
```

### Comparing `evalml-0.74.0/LICENSE` & `evalml-0.75.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/PKG-INFO` & `evalml-0.75.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.74.0
+Version: 0.75.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.74.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.75.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.74.0/README.md` & `evalml-0.75.0/README.md`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/__init__.py` & `evalml-0.75.0/evalml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", FutureWarning)
     warnings.simplefilter("ignore", DeprecationWarning)
     import skopt
 warnings.filterwarnings("ignore", category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-__version__ = "0.74.0"
+__version__ = "0.75.0"
```

### Comparing `evalml-0.74.0/evalml/automl/automl_algorithm/automl_algorithm.py` & `evalml-0.75.0/evalml/automl/automl_algorithm/automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/automl_algorithm/default_algorithm.py` & `evalml-0.75.0/evalml/automl/automl_algorithm/default_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/automl_algorithm/iterative_algorithm.py` & `evalml-0.75.0/evalml/automl/automl_algorithm/iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/automl_search.py` & `evalml-0.75.0/evalml/automl/automl_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 from evalml.utils import convert_to_seconds, infer_feature_types
 from evalml.utils.gen_utils import contains_all_ts_parameters
 from evalml.utils.logger import (
     get_logger,
     log_batch_times,
     log_subtitle,
     log_title,
-    time_elapsed,
 )
 
 
 def build_engine_from_str(engine_str):
     """Function that converts a convenience string for an parallel engine type and returns an instance of that engine.
 
     Args:
@@ -1122,16 +1121,16 @@
                         )
                         pipeline_id = self._post_evaluation_callback(
                             pipeline,
                             data,
                             cached_data,
                             job_log,
                         )
-                        pipeline_times[pipeline.name] = time_elapsed(
-                            start_pipeline_time,
+                        pipeline_times[pipeline.name] = (
+                            time.time() - start_pipeline_time
                         )
                         new_pipeline_ids.append(pipeline_id)
                         computations[current_computation_index] = (computation, True)
                         computations_left_to_process -= 1
                     current_computation_index = (current_computation_index + 1) % max(
                         len(computations),
                         1,
@@ -1159,20 +1158,19 @@
                 error_msgs = set(
                     [str(pl_fold["Exception"]) for pl_fold in self.errors.values()],
                 )
                 raise AutoMLSearchException(
                     f"All pipelines in the current AutoML batch produced a score of np.nan on the primary objective {self.objective}. Exception(s) raised: {error_msgs}. Check the 'errors' attribute of the AutoMLSearch object for a full breakdown of errors and tracebacks.",
                 )
             if len(pipeline_times) > 0:
-                pipeline_times["Total time of batch"] = time_elapsed(start_batch_time)
+                pipeline_times["Total time of batch"] = time.time() - start_batch_time
                 batch_times[self._get_batch_number()] = pipeline_times
 
         self.search_duration = time.time() - self.progress.start_time
-        elapsed_time = time_elapsed(self.progress.start_time)
-        desc = f"\nSearch finished after {elapsed_time}"
+        desc = f"\nSearch finished after {self.search_duration:.2f} seconds"
         desc = desc.ljust(self._MAX_NAME_LEN)
         self.logger.info(desc)
 
         if self.timing is True:
             log_batch_times(self.logger, batch_times)
 
         self._find_best_pipeline()
```

### Comparing `evalml-0.74.0/evalml/automl/callbacks.py` & `evalml-0.75.0/evalml/automl/callbacks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/engine/cf_engine.py` & `evalml-0.75.0/evalml/automl/engine/cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/engine/dask_engine.py` & `evalml-0.75.0/evalml/automl/engine/dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/engine/engine_base.py` & `evalml-0.75.0/evalml/automl/engine/engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/engine/sequential_engine.py` & `evalml-0.75.0/evalml/automl/engine/sequential_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/pipeline_search_plots.py` & `evalml-0.75.0/evalml/automl/pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/progress.py` & `evalml-0.75.0/evalml/automl/progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/automl/utils.py` & `evalml-0.75.0/evalml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/__init__.py` & `evalml-0.75.0/evalml/data_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/class_imbalance_data_check.py` & `evalml-0.75.0/evalml/data_checks/class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check.py` & `evalml-0.75.0/evalml/data_checks/data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check_action.py` & `evalml-0.75.0/evalml/data_checks/data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check_action_code.py` & `evalml-0.75.0/evalml/data_checks/data_check_action_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check_action_option.py` & `evalml-0.75.0/evalml/data_checks/data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check_message.py` & `evalml-0.75.0/evalml/data_checks/data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_check_message_code.py` & `evalml-0.75.0/evalml/data_checks/data_check_message_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/data_checks.py` & `evalml-0.75.0/evalml/data_checks/data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/datetime_format_data_check.py` & `evalml-0.75.0/evalml/data_checks/datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/default_data_checks.py` & `evalml-0.75.0/evalml/data_checks/default_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/id_columns_data_check.py` & `evalml-0.75.0/evalml/data_checks/id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/invalid_target_data_check.py` & `evalml-0.75.0/evalml/data_checks/invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/multicollinearity_data_check.py` & `evalml-0.75.0/evalml/data_checks/multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/no_variance_data_check.py` & `evalml-0.75.0/evalml/data_checks/no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/null_data_check.py` & `evalml-0.75.0/evalml/data_checks/null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/outliers_data_check.py` & `evalml-0.75.0/evalml/data_checks/outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/sparsity_data_check.py` & `evalml-0.75.0/evalml/data_checks/sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/target_distribution_data_check.py` & `evalml-0.75.0/evalml/data_checks/target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/target_leakage_data_check.py` & `evalml-0.75.0/evalml/data_checks/target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/ts_parameters_data_check.py` & `evalml-0.75.0/evalml/data_checks/ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/ts_splitting_data_check.py` & `evalml-0.75.0/evalml/data_checks/ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/uniqueness_data_check.py` & `evalml-0.75.0/evalml/data_checks/uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/data_checks/utils.py` & `evalml-0.75.0/evalml/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/breast_cancer.py` & `evalml-0.75.0/evalml/demos/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/churn.py` & `evalml-0.75.0/evalml/demos/churn.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/data/churn.csv` & `evalml-0.75.0/evalml/demos/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/data/daily-min-temperatures.csv` & `evalml-0.75.0/evalml/demos/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/data/fraud_transactions.csv.gz` & `evalml-0.75.0/evalml/demos/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/diabetes.py` & `evalml-0.75.0/evalml/demos/diabetes.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/fraud.py` & `evalml-0.75.0/evalml/demos/fraud.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/weather.py` & `evalml-0.75.0/evalml/demos/weather.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/demos/wine.py` & `evalml-0.75.0/evalml/demos/wine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/exceptions/__init__.py` & `evalml-0.75.0/evalml/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/exceptions/exceptions.py` & `evalml-0.75.0/evalml/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_family/model_family.py` & `evalml-0.75.0/evalml/model_family/model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_family/utils.py` & `evalml-0.75.0/evalml/model_family/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/__init__.py` & `evalml-0.75.0/evalml/model_understanding/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py` & `evalml-0.75.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/_partial_dependence_utils.py` & `evalml-0.75.0/evalml/model_understanding/_partial_dependence_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/decision_boundary.py` & `evalml-0.75.0/evalml/model_understanding/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/feature_explanations.py` & `evalml-0.75.0/evalml/model_understanding/feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/force_plots.py` & `evalml-0.75.0/evalml/model_understanding/force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/metrics.py` & `evalml-0.75.0/evalml/model_understanding/metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/partial_dependence_functions.py` & `evalml-0.75.0/evalml/model_understanding/partial_dependence_functions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/permutation_importance.py` & `evalml-0.75.0/evalml/model_understanding/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/prediction_explanations/_algorithms.py` & `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py` & `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/prediction_explanations/_user_interface.py` & `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/prediction_explanations/explainers.py` & `evalml-0.75.0/evalml/model_understanding/prediction_explanations/explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/model_understanding/visualizations.py` & `evalml-0.75.0/evalml/model_understanding/visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/__init__.py` & `evalml-0.75.0/evalml/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/binary_classification_objective.py` & `evalml-0.75.0/evalml/objectives/binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/cost_benefit_matrix.py` & `evalml-0.75.0/evalml/objectives/cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/fraud_cost.py` & `evalml-0.75.0/evalml/objectives/fraud_cost.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/lead_scoring.py` & `evalml-0.75.0/evalml/objectives/lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/objective_base.py` & `evalml-0.75.0/evalml/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/sensitivity_low_alert.py` & `evalml-0.75.0/evalml/objectives/sensitivity_low_alert.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/standard_metrics.py` & `evalml-0.75.0/evalml/objectives/standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/objectives/utils.py` & `evalml-0.75.0/evalml/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/__init__.py` & `evalml-0.75.0/evalml/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/binary_classification_pipeline.py` & `evalml-0.75.0/evalml/pipelines/binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/binary_classification_pipeline_mixin.py` & `evalml-0.75.0/evalml/pipelines/binary_classification_pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/classification_pipeline.py` & `evalml-0.75.0/evalml/pipelines/classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/component_graph.py` & `evalml-0.75.0/evalml/pipelines/component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/component_base.py` & `evalml-0.75.0/evalml/pipelines/components/component_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/component_base_meta.py` & `evalml-0.75.0/evalml/pipelines/components/component_base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py` & `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/estimator.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/et_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py` & `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/column_selectors.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/column_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/encoders/label_encoder.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/encoders/target_encoder.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/target_imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/__init__.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/lsa.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/samplers/base_sampler.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/samplers/oversampler.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/samplers/undersampler.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/transformers/transformer.py` & `evalml-0.75.0/evalml/pipelines/components/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/components/utils.py` & `evalml-0.75.0/evalml/pipelines/components/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/multiclass_classification_pipeline.py` & `evalml-0.75.0/evalml/pipelines/multiclass_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/pipeline_base.py` & `evalml-0.75.0/evalml/pipelines/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/pipeline_meta.py` & `evalml-0.75.0/evalml/pipelines/pipeline_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/regression_pipeline.py` & `evalml-0.75.0/evalml/pipelines/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/time_series_classification_pipelines.py` & `evalml-0.75.0/evalml/pipelines/time_series_classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/time_series_pipeline_base.py` & `evalml-0.75.0/evalml/pipelines/time_series_pipeline_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,14 +247,15 @@
         """
         if self.estimator is None:
             raise ValueError(
                 "Cannot call predict_in_sample() on a component graph because the final component is not an Estimator.",
             )
         X, y = self._drop_time_index(X, y)
         X_train, y_train = self._drop_time_index(X_train, y_train)
+        X, y = self._ensure_correct_indices(X, y, X_train)
         target = infer_feature_types(y)
         features = self.transform_all_but_final(
             X,
             target,
             X_train,
             y_train,
             calculating_residuals=calculating_residuals,
@@ -262,14 +263,26 @@
         predictions = self._estimator_predict(features)
         if len(predictions) == len(y):
             predictions.index = y.index
         predictions = self.inverse_transform(predictions)
         predictions = predictions.rename(self.input_target_name)
         return infer_feature_types(predictions)
 
+    def _ensure_correct_indices(self, X, y, X_train):
+        """Ensures that X and y holdout's indices are the correct integer or time units w.r.t the training data.
+
+        For predict in sample where the holdout is known to follow the training data.
+        """
+        if X_train.index.is_numeric():
+            starting_index = X_train.index[-1] + 1 + self.gap
+            correct_index = range(starting_index, starting_index + len(y))
+            X.index = correct_index
+            y.index = correct_index
+        return X, y
+
     def _create_empty_series(self, y_train, size):
         return ww.init_series(
             pd.Series([y_train.iloc[0]] * size),
             logical_type=y_train.ww.logical_type,
         )
 
     def predict(self, X, objective=None, X_train=None, y_train=None):
```

### Comparing `evalml-0.74.0/evalml/pipelines/time_series_regression_pipeline.py` & `evalml-0.75.0/evalml/pipelines/time_series_regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/pipelines/utils.py` & `evalml-0.75.0/evalml/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/preprocessing/data_splitters/no_split.py` & `evalml-0.75.0/evalml/preprocessing/data_splitters/no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/preprocessing/data_splitters/sk_splitters.py` & `evalml-0.75.0/evalml/preprocessing/data_splitters/sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/preprocessing/data_splitters/time_series_split.py` & `evalml-0.75.0/evalml/preprocessing/data_splitters/time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/preprocessing/data_splitters/training_validation_split.py` & `evalml-0.75.0/evalml/preprocessing/data_splitters/training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/preprocessing/utils.py` & `evalml-0.75.0/evalml/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/problem_types/problem_types.py` & `evalml-0.75.0/evalml/problem_types/problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/problem_types/utils.py` & `evalml-0.75.0/evalml/problem_types/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/dask_test_utils.py` & `evalml-0.75.0/evalml/tests/automl_tests/dask_test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py` & `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py` & `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py` & `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,17 +252,17 @@
         batch_times = automl.search()
 
     out = caplog.text
     assert isinstance(batch_times, dict)
     assert isinstance(list(batch_times.keys())[0], int)
     assert isinstance(batch_times[1], dict)
     assert isinstance(list(batch_times[1].keys())[0], str)
-    assert isinstance(batch_times[1]["Total time of batch"], str)
-    assert isinstance(batch_times[2]["Total time of batch"], str)
-    assert isinstance(batch_times[3]["Total time of batch"], str)
+    assert isinstance(batch_times[1]["Total time of batch"], float)
+    assert isinstance(batch_times[2]["Total time of batch"], float)
+    assert isinstance(batch_times[3]["Total time of batch"], float)
 
     assert len(batch_times) == 3
     assert len(batch_times[1]) == 2
     assert len(batch_times[2]) == 2
     assert len(batch_times[3]) == 8
 
     assert "Batch Time Stats" in out
```

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_algorithm.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_classification.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_regression.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_automl_utils.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_automl_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_default_algorithm.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_default_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_engine_base.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_iterative_algorithm.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_pipeline_search_plots.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_progress.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_search.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_search_iterative.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_search_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/automl_tests/test_time_series_split.py` & `evalml-0.75.0/evalml/tests/automl_tests/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py` & `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py` & `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py` & `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_arima_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_baseline_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_baseline_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_catboost_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_catboost_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_column_selector_transformers.py` & `evalml-0.75.0/evalml/tests/component_tests/test_column_selector_transformers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_components.py` & `evalml-0.75.0/evalml/tests/component_tests/test_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_datetime_featurizer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_decision_tree_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_decision_tree_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_drop_rows_transformer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_en_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_en_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_en_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_en_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_estimators.py` & `evalml-0.75.0/evalml/tests/component_tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_et_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_et_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_feature_selectors.py` & `evalml-0.75.0/evalml/tests/component_tests/test_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_featuretools.py` & `evalml-0.75.0/evalml/tests/component_tests/test_featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py` & `evalml-0.75.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_knn_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_knn_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_label_encoder.py` & `evalml-0.75.0/evalml/tests/component_tests/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_lda.py` & `evalml-0.75.0/evalml/tests/component_tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_lgbm_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_lgbm_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_log_transformer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_lsa.py` & `evalml-0.75.0/evalml/tests/component_tests/test_lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_natural_language_featurizer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_nullable_types_replacer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_nullable_types_replacer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_one_hot_encoder.py` & `evalml-0.75.0/evalml/tests/component_tests/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_ordinal_encoder.py` & `evalml-0.75.0/evalml/tests/component_tests/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_oversampler.py` & `evalml-0.75.0/evalml/tests/component_tests/test_oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_pca.py` & `evalml-0.75.0/evalml/tests/component_tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_per_column_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_prophet_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_simple_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_standard_scaler.py` & `evalml-0.75.0/evalml/tests/component_tests/test_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_svm_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_svm_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_target_encoder.py` & `evalml-0.75.0/evalml/tests/component_tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_target_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_time_series_featurizer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_time_series_imputer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_time_series_regularizer.py` & `evalml-0.75.0/evalml/tests/component_tests/test_time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_undersampler.py` & `evalml-0.75.0/evalml/tests/component_tests/test_undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_utils.py` & `evalml-0.75.0/evalml/tests/component_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_xgboost_classifier.py` & `evalml-0.75.0/evalml/tests/component_tests/test_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/component_tests/test_xgboost_regressor.py` & `evalml-0.75.0/evalml/tests/component_tests/test_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/conftest.py` & `evalml-0.75.0/evalml/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data/churn.csv` & `evalml-0.75.0/evalml/tests/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data/daily-min-temperatures.csv` & `evalml-0.75.0/evalml/tests/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data/fraud_transactions.csv.gz` & `evalml-0.75.0/evalml/tests/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data/tips.csv` & `evalml-0.75.0/evalml/tests/data/tips.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data/titanic.csv` & `evalml-0.75.0/evalml/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_action.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_action_option.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_data_check_message.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_data_checks.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_null_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_outliers_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/data_checks_tests/test_utils.py` & `evalml-0.75.0/evalml/tests/data_checks_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/demo_tests/test_datasets.py` & `evalml-0.75.0/evalml/tests/demo_tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt` & `evalml-0.75.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-black==23.3.0
+IPython==8.10.0
+PyYAML==5.4
+black[jupyter]==22.3.0
 catboost==1.1.1
-category-encoders==2.5.1.post0
-click==8.1.3
-cloudpickle==2.2.1
-colorama==0.4.6
-dask==2023.4.0
-featuretools==1.25.0
-graphviz==0.20.1
-holidays==0.20
-imbalanced-learn==0.10.1
-ipywidgets==8.0.4
-kaleido==0.2.1
-lightgbm==3.3.5
+category-encoders==2.2.2
+click==8.0.0
+cloudpickle==1.5.0
+colorama==0.4.4
+coverage[toml]==6.4
+dask==2022.2.0
+distributed==2022.2.0
+featuretools[dask]==1.16.0
+graphviz==0.13
+holidays==0.13
+imbalanced-learn==0.9.1
+ipywidgets==7.5
+kaleido==0.1.0
+lightgbm==2.3.1
 lime==0.2.0.1
-matplotlib==3.7.1
-matplotlib-inline==0.1.6
-networkx==3.1
-nlp-primitives==2.11.0
-numpy==1.23.5
-packaging==23.1
-pandas==1.5.3
-plotly==5.14.1
-pmdarima==2.0.3
-pyzmq==25.0.2
+matplotlib==3.3.3
+nbval==0.9.3
+networkx==2.6
+nlp-primitives==2.9.0
+numpy==1.21.0
+packaging==23.0
+pandas==1.5.0
+plotly==5.0.0
+pmdarima==1.8.5
+pytest-cov==2.10.1
+pytest-timeout==1.4.2
+pytest-xdist==2.1.0
+pytest==7.1.2
+pyzmq==20.0.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
-scipy==1.9.1
-seaborn==0.12.2
-shap==0.41.0
+scipy==1.5.0
+seaborn==0.11.1
+shap==0.40.0
 sktime==0.17.0
-statsmodels==0.13.5
-texttable==1.6.7
+statsmodels==0.12.2
+texttable==1.6.2
 tomli==2.0.1
-vowpalwabbit==9.8.0
-woodwork==0.23.0
-xgboost==1.7.5
+vowpalwabbit==8.11.0
+woodwork[dask]==0.22.0
+xgboost==1.7.0
```

### Comparing `evalml-0.74.0/evalml/tests/dependency_update_check/minimum_requirements.txt` & `evalml-0.75.0/evalml/tests/dependency_update_check/minimum_requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 black[jupyter]==22.3.0
 catboost==1.1.1
 category-encoders==2.2.2
 click==8.0.0
 cloudpickle==1.5.0
 colorama==0.4.4
 dask==2022.2.0
-featuretools==1.16.0
+distributed==2022.2.0
+featuretools[dask]==1.16.0
 graphviz==0.13
 holidays==0.13
 imbalanced-learn==0.9.1
 ipywidgets==7.5
 kaleido==0.1.0
 lightgbm==2.3.1
 lime==0.2.0.1
@@ -28,9 +29,9 @@
 seaborn==0.11.1
 shap==0.40.0
 sktime==0.17.0
 statsmodels==0.12.2
 texttable==1.6.2
 tomli==2.0.1
 vowpalwabbit==8.11.0
-woodwork==0.22.0
+woodwork[dask]==0.22.0
 xgboost==1.7.0
```

### Comparing `evalml-0.74.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py` & `evalml-0.75.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/integration_tests/test_nullable_types.py` & `evalml-0.75.0/evalml/tests/integration_tests/test_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/integration_tests/test_time_series_integration.py` & `evalml-0.75.0/evalml/tests/integration_tests/test_time_series_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_family_tests/test_model_family.py` & `evalml-0.75.0/evalml/tests/model_family_tests/test_model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_decision_boundary.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_feature_explanations.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_metrics.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_partial_dependence.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_permutation_importance.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/model_understanding_tests/test_visualizations.py` & `evalml-0.75.0/evalml/tests/model_understanding_tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_binary_classification_objective.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_fraud_detection.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_fraud_detection.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_lead_scoring.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_objectives.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_sla.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/objective_tests/test_standard_metrics.py` & `evalml-0.75.0/evalml/tests/objective_tests/test_standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_component_graph.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_graphs.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_pipeline_utils.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_pipelines.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py` & `evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,14 +664,77 @@
 
     assert len(preds) == 1
     assert (preds.index == target.iloc[20 + 1 : 20 + 1 + 1].index).all()
     assert len(preds_in_sample) == len(target.iloc[20:])
     assert (preds_in_sample.index == target.iloc[20:].index).all()
 
 
+def test_predict_in_sample_index_error(ts_data):
+    X_train, X_holdout, y_train = ts_data(
+        problem_type="time series regression",
+        train_target_index_dt=False,
+        train_features_index_dt=False,
+        no_features=True,
+    )
+    y_holdout = y_train[-len(X_holdout) :]
+    problem_configuration = {
+        "max_delay": 2,
+        "gap": 0,
+        "forecast_horizon": 5,
+        "time_index": "date",
+    }
+
+    pipeline = TimeSeriesRegressionPipeline(
+        component_graph={
+            "Imputer": ["Imputer", "X", "y"],
+            "Time Series Featurizer": ["Time Series Featurizer", "Imputer.x", "y"],
+            "STL Decomposer": ["STL Decomposer", "Time Series Featurizer.x", "y"],
+            "DateTime Featurizer": [
+                "DateTime Featurizer",
+                "Time Series Featurizer.x",
+                "STL Decomposer.y",
+            ],
+            "Drop NaN Rows Transformer": [
+                "Drop NaN Rows Transformer",
+                "DateTime Featurizer.x",
+                "STL Decomposer.y",
+            ],
+            "Extra Trees Regressor": [
+                "Extra Trees Regressor",
+                "Drop NaN Rows Transformer.x",
+                "Drop NaN Rows Transformer.y",
+            ],
+        },
+        parameters={
+            "pipeline": problem_configuration,
+            "Time Series Featurizer": problem_configuration,
+        },
+    )
+    pipeline.fit(X_train, y_train)
+
+    preds_in_sample = pipeline.predict_in_sample(
+        X_holdout,
+        y_holdout,
+        X_train=X_train,
+        y_train=y_train,
+    )
+
+    y_reset_holdout = y_holdout.reset_index(drop=True)
+    X_reset_holdout = X_holdout.reset_index(drop=True)
+    X_reset_holdout.ww.init(schema=X_holdout.ww.schema)
+    preds_in_sample_reset = pipeline.predict_in_sample(
+        X_reset_holdout,
+        y_reset_holdout,
+        X_train=X_train,
+        y_train=y_train,
+    )
+
+    assert_series_equal(preds_in_sample, preds_in_sample_reset)
+
+
 @pytest.mark.parametrize("only_use_y", [False])
 @pytest.mark.parametrize("include_delayed_features", [True, False])
 @pytest.mark.parametrize(
     "forecast_horizon,gap,max_delay,time_index",
     [
         (1, 0, 1, None),
         (3, 1, 1, None),
```

### Comparing `evalml-0.74.0/evalml/tests/preprocessing_tests/test_no_split.py` & `evalml-0.75.0/evalml/tests/preprocessing_tests/test_no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/preprocessing_tests/test_sk_splitters.py` & `evalml-0.75.0/evalml/tests/preprocessing_tests/test_sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/preprocessing_tests/test_split_data.py` & `evalml-0.75.0/evalml/tests/preprocessing_tests/test_split_data.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/preprocessing_tests/test_training_validation_split.py` & `evalml-0.75.0/evalml/tests/preprocessing_tests/test_training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/problem_type_tests/test_problem_types.py` & `evalml-0.75.0/evalml/tests/problem_type_tests/test_problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/test_all_test_dirs_included.py` & `evalml-0.75.0/evalml/tests/test_all_test_dirs_included.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/tuner_tests/test_grid_search_tuner.py` & `evalml-0.75.0/evalml/tests/tuner_tests/test_grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/tuner_tests/test_random_search_tuner.py` & `evalml-0.75.0/evalml/tests/tuner_tests/test_random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/tuner_tests/test_skopt_tuner.py` & `evalml-0.75.0/evalml/tests/tuner_tests/test_skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/utils_tests/test_cli_utils.py` & `evalml-0.75.0/evalml/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/utils_tests/test_gen_utils.py` & `evalml-0.75.0/evalml/tests/utils_tests/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/utils_tests/test_logger.py` & `evalml-0.75.0/evalml/tests/utils_tests/test_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,24 +71,21 @@
     logger.critical("Test critical")
     assert "Test critical" in caplog.text
     assert "CRITICAL" in caplog.text
 
 
 def test_logger_batch_times(caplog, logger_env_cleanup):
     logger = get_logger(TEST_LOGGER_NAME)
-    batch_times = {"1": {"test": "00:01", "tset": "10:00"}, "2": {"pipe": "00:02"}}
+    batch_times = {"1": {"test": 1.2345, "tset": 9.8}, "2": {"pipe": 2}}
     log_batch_times(logger, batch_times)
     assert "Batch 1 time stats" in caplog.text
-    assert "test:" in caplog.text
-    assert "00:01" in caplog.text
-    assert "tset" in caplog.text
-    assert "10:00" in caplog.text
+    assert "test: 1.23 seconds" in caplog.text
+    assert "tset: 9.80 seconds" in caplog.text
     assert "Batch 2 time stats" in caplog.text
-    assert "pipe" in caplog.text
-    assert "00:02" in caplog.text
+    assert "pipe: 2.00 seconds" in caplog.text
 
 
 @pytest.mark.parametrize(
     "time_passed,answer",
     [(101199, "28:06:39"), (3660, "1:01:00"), (65, "01:05"), (7, "00:07")],
 )
 @patch("time.time")
```

### Comparing `evalml-0.74.0/evalml/tests/utils_tests/test_nullable_type_utils.py` & `evalml-0.75.0/evalml/tests/utils_tests/test_nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tests/utils_tests/test_woodwork_utils.py` & `evalml-0.75.0/evalml/tests/utils_tests/test_woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tuners/grid_search_tuner.py` & `evalml-0.75.0/evalml/tuners/grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tuners/random_search_tuner.py` & `evalml-0.75.0/evalml/tuners/random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tuners/skopt_tuner.py` & `evalml-0.75.0/evalml/tuners/skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/tuners/tuner.py` & `evalml-0.75.0/evalml/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/__init__.py` & `evalml-0.75.0/evalml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/base_meta.py` & `evalml-0.75.0/evalml/utils/base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/cli_utils.py` & `evalml-0.75.0/evalml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/gen_utils.py` & `evalml-0.75.0/evalml/utils/gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/logger.py` & `evalml-0.75.0/evalml/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,10 +66,13 @@
     """
     log_title(logger, "Batch Time Stats")
     for batch_number in batch_times:
         subtitle = "Batch " + str(batch_number) + " time stats:"
         log_subtitle(logger, subtitle)
         for pipeline_name in batch_times[batch_number]:
             logger.info(
-                "\n" + pipeline_name + ": " + batch_times[batch_number][pipeline_name],
+                "\n"
+                + pipeline_name
+                + ": "
+                + f"{batch_times[batch_number][pipeline_name]:.2f} seconds",
             )
         logger.info("")
```

### Comparing `evalml-0.74.0/evalml/utils/nullable_type_utils.py` & `evalml-0.75.0/evalml/utils/nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml/utils/woodwork_utils.py` & `evalml-0.75.0/evalml/utils/woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml.egg-info/PKG-INFO` & `evalml-0.75.0/evalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.74.0
+Version: 0.75.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.74.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.75.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.74.0/evalml.egg-info/SOURCES.txt` & `evalml-0.75.0/evalml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.74.0/evalml.egg-info/requires.txt` & `evalml-0.75.0/evalml.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 pyzmq>=20.0.0
 colorama>=0.4.4
 cloudpickle>=1.5.0
 click>=8.0.0
 shap>=0.40.0
 statsmodels>=0.12.2
 texttable>=1.6.2
-woodwork>=0.22.0
+woodwork[dask]>=0.22.0
 dask!=2022.10.1,>=2022.2.0
-featuretools>=1.16.0
+distributed!=2022.10.1,>=2022.2.0
+featuretools[dask]>=1.16.0
 nlp-primitives>=2.9.0
 networkx>=2.6
 plotly>=5.0.0
 kaleido>=0.1.0
 ipywidgets<8.0.5,>=7.5
 xgboost>=1.7.0
 catboost>=1.1.1
@@ -63,13 +64,13 @@
 
 [test]
 pytest==7.1.2
 pytest-xdist==2.1.0
 pytest-timeout==1.4.2
 pytest-cov==2.10.1
 nbval==0.9.3
-IPython>=8.10.0
+IPython<8.12.1,>=8.10.0
 PyYAML==5.4
 coverage[toml]>=6.4
 
 [updater]
 alteryx-open-src-update-checker>=2.1.0
```

### Comparing `evalml-0.74.0/pyproject.toml` & `evalml-0.75.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
     "pyzmq >= 20.0.0",
     "colorama >= 0.4.4",
     "cloudpickle >= 1.5.0",
     "click >= 8.0.0",
     "shap >= 0.40.0",
     "statsmodels >= 0.12.2",
     "texttable >= 1.6.2",
-    "woodwork >= 0.22.0",
+    "woodwork[dask] >= 0.22.0",
     "dask >= 2022.2.0, != 2022.10.1",
-    "featuretools >= 1.16.0",
+    "distributed >= 2022.2.0, != 2022.10.1",
+    "featuretools[dask] >= 1.16.0",
     "nlp-primitives >= 2.9.0",
     "networkx >= 2.6",
     "plotly >= 5.0.0",
     "kaleido >= 0.1.0",
     "ipywidgets >= 7.5, < 8.0.5",
     "xgboost >= 1.7.0",
     "catboost >= 1.1.1",
@@ -78,15 +79,15 @@
 [project.optional-dependencies]
 test = [
     "pytest == 7.1.2",
     "pytest-xdist == 2.1.0",
     "pytest-timeout == 1.4.2",
     "pytest-cov == 2.10.1",
     "nbval == 0.9.3",
-    "IPython >= 8.10.0",
+    "IPython >= 8.10.0, <8.12.1",
     "PyYAML == 5.4",
     "coverage[toml] >= 6.4",
 ]
 dev = [
     "ruff == 0.0.228",
     "darglint == 1.8.0",
     "pre-commit >= 2.20.0",
```

