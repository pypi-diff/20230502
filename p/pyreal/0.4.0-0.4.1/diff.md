# Comparing `tmp/pyreal-0.4.0.tar.gz` & `tmp/pyreal-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreal-0.4.0.tar", max compression
+gzip compressed data, was "pyreal-0.4.1.tar", max compression
```

## Comparing `pyreal-0.4.0.tar` & `pyreal-0.4.1.tar`

### file list

```diff
@@ -1,138 +1,144 @@
--rw-r--r--   0        0        0      165 2023-04-10 15:12:35.216516 pyreal-0.4.0/AUTHORS.rst
--rw-r--r--   0        0        0        9 2023-04-10 15:12:35.216516 pyreal-0.4.0/HISTORY.md
--rw-r--r--   0        0        0     1075 2023-04-10 15:12:35.216516 pyreal-0.4.0/LICENSE
--rw-r--r--   0        0        0     4238 2023-04-10 15:12:35.216516 pyreal-0.4.0/README.md
--rw-r--r--   0        0        0     1856 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      240 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/__init__.py
--rw-r--r--   0        0        0     3042 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/explainer_challenge.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/__init__.py
--rw-r--r--   0        0        0      436 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
--rw-r--r--   0        0        0      430 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/__init__.py
--rw-r--r--   0        0        0      439 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
--rw-r--r--   0        0        0      436 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
--rw-r--r--   0        0        0     1623 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/dataset.py
--rw-r--r--   0        0        0      610 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/download_datasets_script.py
--rw-r--r--   0        0        0     5213 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/main.py
--rw-r--r--   0        0        0    15073 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
--rw-r--r--   0        0        0     1652 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/adult_logistic_regression.pkl
--rw-r--r--   0        0        0     3108 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
--rw-r--r--   0        0        0     1244 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
--rw-r--r--   0        0        0      941 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
--rw-r--r--   0        0        0      881 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/breast-w_logistic_regression.pkl
--rw-r--r--   0        0        0     1116 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/cmc_logistic_regression.pkl
--rw-r--r--   0        0        0    62681 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
--rw-r--r--   0        0        0     1180 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
--rw-r--r--   0        0        0     1300 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/credit-g_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/diabetes_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/electricity_logistic_regression.pkl
--rw-r--r--   0        0        0     4528 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
--rw-r--r--   0        0        0     3423 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
--rw-r--r--   0        0        0      948 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/ilpd_logistic_regression.pkl
--rw-r--r--   0        0        0   129793 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/isolet_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/jm1_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kc1_logistic_regression.pkl
--rw-r--r--   0        0        0      977 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kc2_logistic_regression.pkl
--rw-r--r--   0        0        0     1396 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
--rw-r--r--   0        0        0     4636 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/letter_logistic_regression.pkl
--rw-r--r--   0        0        0     4865 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/madelon_logistic_regression.pkl
--rw-r--r--   0        0        0    18351 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
--rw-r--r--   0        0        0     7151 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
--rw-r--r--   0        0        0     1551 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
--rw-r--r--   0        0        0     4831 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
--rw-r--r--   0        0        0    63793 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
--rw-r--r--   0        0        0     1807 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/nomao_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/optdigits_logistic_regression.pkl
--rw-r--r--   0        0        0     1439 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc1_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc3_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc4_logistic_regression.pkl
--rw-r--r--   0        0        0     2351 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pendigits_logistic_regression.pkl
--rw-r--r--   0        0        0      900 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/phoneme_logistic_regression.pkl
--rw-r--r--   0        0        0     1191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
--rw-r--r--   0        0        0     2703 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/satimage_logistic_regression.pkl
--rw-r--r--   0        0        0    21553 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/semeion_logistic_regression.pkl
--rw-r--r--   0        0        0     1228 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/sick_logistic_regression.pkl
--rw-r--r--   0        0        0     1319 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/spambase_logistic_regression.pkl
--rw-r--r--   0        0        0     7738 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/splice_logistic_regression.pkl
--rw-r--r--   0        0        0     1025 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
--rw-r--r--   0        0        0     1444 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/vehicle_logistic_regression.pkl
--rw-r--r--   0        0        0     3384 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/vowel_logistic_regression.pkl
--rw-r--r--   0        0        0     1695 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/wdbc_logistic_regression.pkl
--rw-r--r--   0        0        0      145 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models.py
--rw-r--r--   0        0        0    10056 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10104 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
--rw-r--r--   0        0        0    10111 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
--rw-r--r--   0        0        0    10072 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0    10069 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10073 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0     1186 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/task.py
--rw-r--r--   0        0        0     1879 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/__init__.py
--rw-r--r--   0        0        0    18048 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/base.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/__init__.py
--rw-r--r--   0        0        0     3018 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/base.py
--rw-r--r--   0        0        0     6168 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/decision_tree_explainer.py
--rw-r--r--   0        0        0     3071 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/surrogate_decision_tree.py
--rw-r--r--   0        0        0     7766 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/generic_explainer.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/__init__.py
--rw-r--r--   0        0        0     3982 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/base.py
--rw-r--r--   0        0        0     5985 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/global_feature_importance.py
--rw-r--r--   0        0        0     1866 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/permutation_feature_importance.py
--rw-r--r--   0        0        0     3505 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/shap_feature_importance.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/__init__.py
--rw-r--r--   0        0        0     4671 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/base.py
--rw-r--r--   0        0        0     6452 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/local_feature_contribution.py
--rw-r--r--   0        0        0     4057 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/shap_feature_contribution.py
--rw-r--r--   0        0        0     2955 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/simple_counterfactual_contribution.py
--rw-r--r--   0        0        0      372 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/__init__.py
--rw-r--r--   0        0        0     4376 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/base.py
--rw-r--r--   0        0        0     5102 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
--rw-r--r--   0        0        0     5489 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/realapp/__init__.py
--rw-r--r--   0        0        0    17709 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/realapp/realapp.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/__init__.py
--rw-r--r--   0        0        0     8996 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/ames_housing.py
--rw-r--r--   0        0        0     1769 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/california_housing.py
--rw-r--r--   0        0        0   460673 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data.csv
--rw-r--r--   0        0        0    13637 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data_description.txt
--rw-r--r--   0        0        0     3431 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
--rw-r--r--   0        0        0    14681 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
--rw-r--r--   0        0        0  1217129 2023-04-10 15:12:35.236516 pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/california.csv
--rw-r--r--   0        0        0    68558 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_student/data.csv
--rw-r--r--   0        0        0     1514 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_student/students.csv
--rw-r--r--   0        0        0    60300 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_titanic/data.csv
--rw-r--r--   0        0        0     4569 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/student_performance.py
--rw-r--r--   0        0        0     3233 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/titanic.py
--rw-r--r--   0        0        0     1756 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/__init__.py
--rw-r--r--   0        0        0    16940 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/base.py
--rw-r--r--   0        0        0     5376 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/feature_select.py
--rw-r--r--   0        0        0     2719 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/impute.py
--rw-r--r--   0        0        0    15375 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/one_hot_encode.py
--rw-r--r--   0        0        0     2164 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/pad.py
--rw-r--r--   0        0        0     6565 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/sax.py
--rw-r--r--   0        0        0    16093 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/time_series_formatter.py
--rw-r--r--   0        0        0     1337 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/wrappers.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/__init__.py
--rw-r--r--   0        0        0     4137 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/base.py
--rw-r--r--   0        0        0      987 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/decision_tree.py
--rw-r--r--   0        0        0     5184 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/feature_based.py
--rw-r--r--   0        0        0      646 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/time_series_saliency.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/__init__.py
--rw-r--r--   0        0        0     7810 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/_plot_tree.py
--rw-r--r--   0        0        0     1968 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/dataloader.py
--rw-r--r--   0        0        0     1821 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/model_utils.py
--rw-r--r--   0        0        0      520 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/__init__.py
--rw-r--r--   0        0        0    14256 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/feature_based_vis.py
--rw-r--r--   0        0        0     2576 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/time_series_vis.py
--rw-r--r--   0        0        0     2687 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/tree_vis.py
--rw-r--r--   0        0        0      870 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/visualize_config.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 pyreal-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-05-02 15:02:52.904501 pyreal-0.4.1/AUTHORS.rst
+-rw-r--r--   0        0        0        9 2023-05-02 15:02:52.904501 pyreal-0.4.1/HISTORY.md
+-rw-r--r--   0        0        0     1075 2023-05-02 15:02:52.904501 pyreal-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4244 2023-05-02 15:02:52.904501 pyreal-0.4.1/README.md
+-rw-r--r--   0        0        0     1856 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/__init__.py
+-rw-r--r--   0        0        0     3042 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/explainer_challenge.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/gfi/__init__.py
+-rw-r--r--   0        0        0      436 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
+-rw-r--r--   0        0        0      430 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/lfc/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
+-rw-r--r--   0        0        0      436 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
+-rw-r--r--   0        0        0     1623 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/dataset.py
+-rw-r--r--   0        0        0      610 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/download_datasets_script.py
+-rw-r--r--   0        0        0     5213 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/main.py
+-rw-r--r--   0        0        0    15073 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
+-rw-r--r--   0        0        0     1652 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/adult_logistic_regression.pkl
+-rw-r--r--   0        0        0     3108 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
+-rw-r--r--   0        0        0     1244 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
+-rw-r--r--   0        0        0      941 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
+-rw-r--r--   0        0        0      881 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/breast-w_logistic_regression.pkl
+-rw-r--r--   0        0        0     1116 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/cmc_logistic_regression.pkl
+-rw-r--r--   0        0        0    62681 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
+-rw-r--r--   0        0        0     1180 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
+-rw-r--r--   0        0        0     1300 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/credit-g_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/diabetes_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/electricity_logistic_regression.pkl
+-rw-r--r--   0        0        0     4528 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
+-rw-r--r--   0        0        0     3423 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
+-rw-r--r--   0        0        0      948 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/ilpd_logistic_regression.pkl
+-rw-r--r--   0        0        0   129793 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/isolet_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/jm1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/kc1_logistic_regression.pkl
+-rw-r--r--   0        0        0      977 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/kc2_logistic_regression.pkl
+-rw-r--r--   0        0        0     1396 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
+-rw-r--r--   0        0        0     4636 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/letter_logistic_regression.pkl
+-rw-r--r--   0        0        0     4865 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/madelon_logistic_regression.pkl
+-rw-r--r--   0        0        0    18351 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
+-rw-r--r--   0        0        0     7151 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
+-rw-r--r--   0        0        0     1551 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
+-rw-r--r--   0        0        0     4831 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
+-rw-r--r--   0        0        0    63793 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
+-rw-r--r--   0        0        0     1807 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/nomao_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/optdigits_logistic_regression.pkl
+-rw-r--r--   0        0        0     1439 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/pc1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/pc3_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/pc4_logistic_regression.pkl
+-rw-r--r--   0        0        0     2351 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/pendigits_logistic_regression.pkl
+-rw-r--r--   0        0        0      900 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/phoneme_logistic_regression.pkl
+-rw-r--r--   0        0        0     1191 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
+-rw-r--r--   0        0        0     2703 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/satimage_logistic_regression.pkl
+-rw-r--r--   0        0        0    21553 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/semeion_logistic_regression.pkl
+-rw-r--r--   0        0        0     1228 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/sick_logistic_regression.pkl
+-rw-r--r--   0        0        0     1319 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/spambase_logistic_regression.pkl
+-rw-r--r--   0        0        0     7738 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/splice_logistic_regression.pkl
+-rw-r--r--   0        0        0     1025 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
+-rw-r--r--   0        0        0     1444 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/vehicle_logistic_regression.pkl
+-rw-r--r--   0        0        0     3384 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/vowel_logistic_regression.pkl
+-rw-r--r--   0        0        0     1695 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/models/wdbc_logistic_regression.pkl
+-rw-r--r--   0        0        0      145 2023-05-02 15:02:52.908501 pyreal-0.4.1/pyreal/benchmark/models.py
+-rw-r--r--   0        0        0    10056 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10104 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
+-rw-r--r--   0        0        0    10111 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
+-rw-r--r--   0        0        0    10072 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10069 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10073 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0     1186 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/benchmark/task.py
+-rw-r--r--   0        0        0     2136 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/__init__.py
+-rw-r--r--   0        0        0    20625 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/base.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/dte/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/dte/base.py
+-rw-r--r--   0        0        0     3019 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/dte/decision_tree_explainer.py
+-rw-r--r--   0        0        0     3448 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/dte/surrogate_decision_tree.py
+-rw-r--r--   0        0        0     4883 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/generic_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/gfi/__init__.py
+-rw-r--r--   0        0        0     4301 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/gfi/base.py
+-rw-r--r--   0        0        0     2984 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/gfi/global_feature_importance.py
+-rw-r--r--   0        0        0     2237 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/gfi/permutation_feature_importance.py
+-rw-r--r--   0        0        0     3729 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/gfi/shap_feature_importance.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/lfc/__init__.py
+-rw-r--r--   0        0        0     4990 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/lfc/base.py
+-rw-r--r--   0        0        0     3135 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/lfc/local_feature_contribution.py
+-rw-r--r--   0        0        0     4425 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/lfc/shap_feature_contribution.py
+-rw-r--r--   0        0        0     3354 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/lfc/simple_counterfactual_contribution.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/pdp/__init__.py
+-rw-r--r--   0        0        0     3625 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/pdp/base.py
+-rw-r--r--   0        0        0     2796 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/pdp/partial_dependence.py
+-rw-r--r--   0        0        0     1929 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/pdp/partial_dependence_explainer.py
+-rw-r--r--   0        0        0      372 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/time_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/time_series/saliency/__init__.py
+-rw-r--r--   0        0        0     4689 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/time_series/saliency/base.py
+-rw-r--r--   0        0        0     5623 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
+-rw-r--r--   0        0        0     5916 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/realapp/__init__.py
+-rw-r--r--   0        0        0    20614 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/realapp/realapp.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/sample_applications/__init__.py
+-rw-r--r--   0        0        0     8997 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/sample_applications/ames_housing.py
+-rw-r--r--   0        0        0     1769 2023-05-02 15:02:52.912501 pyreal-0.4.1/pyreal/sample_applications/california_housing.py
+-rw-r--r--   0        0        0   460673 2023-05-02 15:02:52.916501 pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/data.csv
+-rw-r--r--   0        0        0    13637 2023-05-02 15:02:52.916501 pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/data_description.txt
+-rw-r--r--   0        0        0     3431 2023-05-02 15:02:52.916501 pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
+-rw-r--r--   0        0        0    14681 2023-05-02 15:02:52.916501 pyreal-0.4.1/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
+-rw-r--r--   0        0        0  1217129 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/data_cal_housing/california.csv
+-rw-r--r--   0        0        0    68558 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/data_student/data.csv
+-rw-r--r--   0        0        0     1514 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/data_student/students.csv
+-rw-r--r--   0        0        0    60300 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/data_titanic/data.csv
+-rw-r--r--   0        0        0     4570 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/student_performance.py
+-rw-r--r--   0        0        0     3183 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/sample_applications/titanic.py
+-rw-r--r--   0        0        0     1837 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/__init__.py
+-rw-r--r--   0        0        0    16940 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/base.py
+-rw-r--r--   0        0        0     5376 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/feature_select.py
+-rw-r--r--   0        0        0     2726 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/impute.py
+-rw-r--r--   0        0        0    15382 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/one_hot_encode.py
+-rw-r--r--   0        0        0     2171 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/pad.py
+-rw-r--r--   0        0        0     6565 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/sax.py
+-rw-r--r--   0        0        0    16182 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/time_series_formatter.py
+-rw-r--r--   0        0        0      469 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/type_cast.py
+-rw-r--r--   0        0        0     1344 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/transformers/wrappers.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/__init__.py
+-rw-r--r--   0        0        0     4137 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/base.py
+-rw-r--r--   0        0        0      987 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/decision_tree.py
+-rw-r--r--   0        0        0     5184 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/feature_based.py
+-rw-r--r--   0        0        0     3084 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/feature_value_based.py
+-rw-r--r--   0        0        0      646 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/types/explanations/time_series_saliency.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/utils/__init__.py
+-rw-r--r--   0        0        0     7810 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/utils/_plot_tree.py
+-rw-r--r--   0        0        0     1968 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/utils/dataloader.py
+-rw-r--r--   0        0        0     1821 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/utils/model_utils.py
+-rw-r--r--   0        0        0      520 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/visualize/__init__.py
+-rw-r--r--   0        0        0    14256 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/visualize/feature_based_vis.py
+-rw-r--r--   0        0        0     2576 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/visualize/time_series_vis.py
+-rw-r--r--   0        0        0     2687 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/visualize/tree_vis.py
+-rw-r--r--   0        0        0      870 2023-05-02 15:02:52.924502 pyreal-0.4.1/pyreal/visualize/visualize_config.py
+-rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 pyreal-0.4.1/PKG-INFO
```

### Comparing `pyreal-0.4.0/LICENSE` & `pyreal-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/README.md` & `pyreal-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,14 @@
 ![Quickstart](docs/images/titanic.png)
 
 We can see here that the input passenger's predicted chance of survival was greatly reduced
 because of their sex (male) and ticket class (3rd class).
 
 ### Terminology
 Pyreal introduces specific terms and naming schemes to refer to different feature spaces and
-transformations. The [Terminology User Guide](https://sibyl-ml.dev/pyreal/user_guides/transformer_workflow.html#terminology) provides an introduction to these terms.
+transformations. The [Terminology User Guide](https://dtail.gitbook.io/pyreal/developing-applications/developer-terminology-guide) provides an introduction to these terms.
 
 # What's next?
 
 For more details about **Pyreal** and all its possibilities
 and features, please check the [documentation site](
 https://dtail.gitbook.io/pyreal/).
```

### Comparing `pyreal-0.4.0/pyproject.toml` & `pyreal-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 maintainers = [
   "MIT Data To AI Lab <dailabmit@gmail.com>",
 ]
 
 description = "Library for evaluating and deploying human readable machine learning explanations."
 name = "pyreal"
-version = "0.4.0"
+version = "0.4.1"
 
 license = ""
 
 readme = "README.md"
 
 documentation = "https://sibyl-dev.github.io/pyreal"
 homepage = "https://sibyl-ml.dev/"
```

### Comparing `pyreal-0.4.0/pyreal/benchmark/challenges/explainer_challenge.py` & `pyreal-0.4.1/pyreal/benchmark/challenges/explainer_challenge.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/dataset.py` & `pyreal-0.4.1/pyreal/benchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/download_datasets_script.py` & `pyreal-0.4.1/pyreal/benchmark/download_datasets_script.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/main.py` & `pyreal-0.4.1/pyreal/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/adult_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/adult_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/balance-scale_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/balance-scale_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/breast-w_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/breast-w_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/cmc_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/cmc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/cnae-9_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/cnae-9_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/credit-approval_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/credit-approval_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/credit-g_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/credit-g_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/diabetes_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/diabetes_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/electricity_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/electricity_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/ilpd_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/ilpd_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/isolet_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/isolet_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/jm1_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/jm1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/kc1_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/kc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/kc2_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/kc2_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/letter_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/letter_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/madelon_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/madelon_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/mnist_784_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/mnist_784_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/nomao_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/nomao_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/optdigits_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/optdigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/pc1_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/pc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/pc3_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/pc3_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/pc4_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/pc4_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/pendigits_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/pendigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/phoneme_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/phoneme_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/satimage_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/satimage_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/semeion_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/semeion_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/sick_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/sick_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/spambase_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/spambase_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/splice_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/splice_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/vehicle_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/vehicle_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/vowel_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/vowel_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/models/wdbc_logistic_regression.pkl` & `pyreal-0.4.1/pyreal/benchmark/models/wdbc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge` & `pyreal-0.4.1/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/benchmark/task.py` & `pyreal-0.4.1/pyreal/benchmark/task.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/explainers/__init__.py` & `pyreal-0.4.1/pyreal/explainers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 from pyreal.explainers.base import ExplainerBase
 from pyreal.explainers.gfi.base import GlobalFeatureImportanceBase
 from pyreal.explainers.gfi.shap_feature_importance import ShapFeatureImportance
 from pyreal.explainers.gfi.permutation_feature_importance import PermutationFeatureImportance
-from pyreal.explainers.gfi.global_feature_importance import GlobalFeatureImportance, gfi
+from pyreal.explainers.gfi.global_feature_importance import GlobalFeatureImportance
 
 from pyreal.explainers.lfc.base import LocalFeatureContributionsBase
 from pyreal.explainers.lfc.shap_feature_contribution import ShapFeatureContribution
 from pyreal.explainers.lfc.simple_counterfactual_contribution import (
     SimpleCounterfactualContribution,
 )
-from pyreal.explainers.lfc.local_feature_contribution import LocalFeatureContribution, lfc
+from pyreal.explainers.lfc.local_feature_contribution import LocalFeatureContribution
 
 from pyreal.explainers.dte.base import DecisionTreeExplainerBase
 from pyreal.explainers.dte.surrogate_decision_tree import SurrogateDecisionTree
-from pyreal.explainers.dte.decision_tree_explainer import DecisionTreeExplainer, dte
+from pyreal.explainers.dte.decision_tree_explainer import DecisionTreeExplainer
+
+from pyreal.explainers.pdp.base import PartialDependenceExplainerBase
+from pyreal.explainers.pdp.partial_dependence import PartialDependence
+from pyreal.explainers.pdp.partial_dependence_explainer import PartialDependenceExplainer
 
 from pyreal.explainers.time_series.saliency.base import SaliencyBase
 from pyreal.explainers.time_series.saliency.univariate_occlusion_saliency import (
     UnivariateOcclusionSaliency,
 )
 from pyreal.explainers.time_series.saliency.univariate_lime_saliency import (
     UnivariateLimeSaliency,
 )
 
-from pyreal.explainers.generic_explainer import Explainer, explain
+from pyreal.explainers.generic_explainer import Explainer
 
 
 __all__ = [
     "ExplainerBase",
     "LocalFeatureContributionsBase",
     "ShapFeatureContribution",
     "SimpleCounterfactualContribution",
     "LocalFeatureContribution",
-    "lfc",
     "GlobalFeatureImportanceBase",
     "ShapFeatureImportance",
     "GlobalFeatureImportance",
-    "gfi",
     "PermutationFeatureImportance",
     "DecisionTreeExplainerBase",
     "DecisionTreeExplainer",
     "SurrogateDecisionTree",
-    "dte",
+    "PartialDependenceExplainerBase",
+    "PartialDependence",
+    "PartialDependenceExplainer",
     "SaliencyBase",
     "UnivariateOcclusionSaliency",
     "UnivariateLimeSaliency",
     "Explainer",
-    "explain",
 ]
```

### Comparing `pyreal-0.4.0/pyreal/explainers/base.py` & `pyreal-0.4.1/pyreal/explainers/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     Args:
         model (string filepath or model object):
            Filepath to the pickled model to explain, or model object with .predict() function
            model.predict() should return a single value prediction for each input
            Classification models should return the index or class. If the latter, the `classes`
            parameter should be provided.
         x_train_orig (DataFrame of shape (n_instances, x_orig_feature_count)):
-           The training set for the explainer
-        y_orig (DataFrame of shape (n_instances,)):
+           The training set for the explainer. If none, must be provided separately when fitting
+        y_train (DataFrame of shape (n_instances,)):
            The y values for the dataset
         feature_descriptions (dict):
            Interpretable descriptions of each feature
         classes (array):
             List of class names returned by the model, in the order that the internal model
             considers them if applicable.
             Can be automatically extracted if model is an sklearn classifier
@@ -107,21 +107,23 @@
            If False, self.fit() must be manually called before produce() is called
         training_size (Integer):
             If given this value, sample a training set with size of this value
             from x_train_orig and use it to train the explainer instead of the
             entire x_train_orig.
         return_original_explanation (Boolean):
             If True, return the explanation originally generated without any transformations
+        fit_transformers (Boolean):
+            If True, fit transformers on x_train_orig. Requires x_train_orig not be None
     """
 
     def __init__(
         self,
         model,
-        x_train_orig,
-        y_orig=None,
+        x_train_orig=None,
+        y_train=None,
         feature_descriptions=None,
         classes=None,
         class_descriptions=None,
         transformers=None,
         fit_on_init=False,
         training_size=None,
         return_original_explanation=False,
@@ -132,23 +134,24 @@
         else:
             predict_method = getattr(model, "predict", None)
             if not callable(predict_method):
                 raise TypeError("Given model that does not have a .predict function")
             self.model = model
 
         self.x_train_orig = x_train_orig
-        self.y_orig = y_orig
+        self.y_train = y_train
 
-        if not isinstance(x_train_orig, pd.DataFrame) or (
-            y_orig is not None
-            and not (isinstance(y_orig, pd.DataFrame) or isinstance(y_orig, pd.Series))
+        if x_train_orig is not None and not isinstance(x_train_orig, pd.DataFrame):
+            raise TypeError("x_train_orig must be of type DataFrame")
+        if y_train is not None and not (
+            isinstance(y_train, pd.DataFrame) or isinstance(y_train, pd.Series)
         ):
-            raise TypeError("x_orig and y_orig must be of type DataFrame")
+            raise TypeError("y_train must be of type DataFrame or Series")
 
-        self.x_orig_feature_count = x_train_orig.shape[1]
+        # self.x_orig_feature_count = x_train_orig.shape[1]
 
         self.transformers = _check_transformers(transformers)
 
         self.feature_descriptions = feature_descriptions
 
         self.classes = classes
         if (
@@ -160,51 +163,46 @@
             and is_classifier(model)
             and hasattr(model, "classes_")
         ):
             self.classes = model.classes_
 
         self.class_descriptions = class_descriptions
         self.return_original_explanation = return_original_explanation
-        self.training_size = training_size
-        if training_size is None:
-            self.training_size = self.x_train_orig.shape[0]
 
-        # this argument stores the indices of the rows of data we want to use
-        data_sample_indices = self.x_train_orig.index
+        self.x_train_orig_subset = self.x_train_orig
+        self.y_train_subset = self.y_train
 
-        if self.training_size is None:
-            log.info(
-                "Info: training_size not provided. Defaulting to train with full "
-                "dataset, running time might be slow."
+        self.training_size = training_size
+        if x_train_orig is not None and training_size is not None:
+            self.x_train_orig_subset, self.y_train_subset = self._select_training_set(
+                x_train_orig, y_train
             )
-        elif self.training_size < len(self.x_train_orig.index):
-            if self.classes is not None and self.training_size < len(self.classes):
-                raise ValueError("training_size must be larger than the number of classes")
-            else:
-                data_sample_indices = pd.Index(
-                    np.random.choice(self.x_train_orig.index, self.training_size, replace=False)
-                )
-
-        # use _x_train_orig for fitting explainer
-        self._x_train_orig = self.x_train_orig.loc[data_sample_indices]
-        if y_orig is not None:
-            self._y_orig = self.y_orig.loc[data_sample_indices]
 
         if fit_transformers:
+            if x_train_orig is None:
+                raise ValueError("Cannot fit transformers unless x_train_orig is provided")
             a_transformers = _get_transformers(self.transformers, algorithm=True)
             i_transformers = _get_transformers(self.transformers, interpret=True)
             fit_transformers_func(a_transformers, self.x_train_orig)
             fit_transformers_func(i_transformers, self.x_train_orig)
 
         if fit_on_init:
+            if x_train_orig is None:
+                raise
             self.fit()
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
-        Fit this explainer object. Abstract method
+        Fit this explainer object.
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
         return self
 
     @abstractmethod
     def produce(self, x_orig):
         """
         Return the explanation, in the desired form.
@@ -422,33 +420,38 @@
 
         Returns:
             DataFrame of shape (n_instances, x_interpret_feature_count)
                 Transformed, interpretable data
         """
         return self.convert_columns_to_interpretable(self.transform_to_x_interpret(x_orig))
 
-    def evaluate_model(self, scorer):
+    def evaluate_model(self, scorer, x_orig=None, y=None):
         """
         Evaluate the model using a chosen scorer algorithm.
 
         Args:
             scorer (string):
                 Type of scorer to use. See sklearn's scoring parameter options here:
                 https://scikit-learn.org/stable/modules/model_evaluation.html#scoring-parameter
+            x_orig (DataFrame of shape (n_instances, n_features)):
+                Dataset to score on. Required if x_train_orig was not provided at initialization.
+                If None, use self.x_train_orig
+            y (DataFrame of shape (n_instances, n_features)):
+                Dataset to score on. Required if y_train was not provided at initialization
+
 
         Returns:
             float
                 A score for the model
-
         """
-        if self.y_orig is None:
-            raise ValueError("Explainer must have a y_orig parameter to score model")
+        x_orig, y = self._get_training_data(x_orig, y)
+
         scorer = get_scorer(scorer)
-        x = self.transform_to_x_model(self._x_train_orig)
-        score = scorer(self.model, x, self._y_orig)
+        x_model = self.transform_to_x_model(x_orig)
+        score = scorer(self.model, x_model, y)
         return score
 
     @abstractmethod
     def evaluate_variation(self, with_fit=False, explanations=None, n_iterations=20, n_rows=10):
         """
         Evaluate the variation of the explanations generated by this Explainer.
         A variation of 0 means this explainer is expected to generate the exact same explanation
@@ -468,7 +471,59 @@
             n_rows (int):
                 Number of rows of dataset to generate explanations on
 
         Returns:
             float
                 The variation of this Explainer's explanations
         """
+
+    def _get_x_train_orig(self, x_train_orig):
+        """
+        Helper function to get the appropriate x_orig or raise errors if something goes wrong
+        Args:
+            x_train_orig (DataFrame or None):
+                Provided DataFrame
+        Returns:
+            The dataframe to use (x_orig or self.x_train_orig)
+
+        Raises:
+            ValueError if no valid dataframe
+        """
+        if x_train_orig is not None:
+            return self._select_training_set(x_train_orig)[0]
+        if self.x_train_orig_subset is not None:
+            return self.x_train_orig_subset
+        else:
+            raise ValueError("Must provide x_train_orig at initialization or fitting time!")
+
+    def _get_training_data(self, x_train_orig, y_train):
+        if x_train_orig is None and self.x_train_orig is None:
+            raise ValueError("Must provide x_train_orig at initialization or fitting time")
+        if y_train is None and self.y_train is None:
+            raise ValueError("Must provide y_train at initialization or fitting time")
+        if x_train_orig is not None and y_train is None:
+            raise ValueError("Must provide y_train if providing x_train_orig")
+
+        if x_train_orig is None:
+            return self.x_train_orig_subset, self.y_train_subset
+        else:
+            return self._select_training_set(x_train_orig, y_train)
+
+    def _select_training_set(self, x_train, y_train=None):
+        if self.training_size is None:
+            return x_train, y_train
+        if self.training_size < len(x_train.index):
+            if self.classes is not None and self.training_size < len(self.classes):
+                raise ValueError("training_size must be larger than the number of classes")
+            else:
+                data_sample_indices = pd.Index(
+                    np.random.choice(x_train.index, self.training_size, replace=False)
+                )
+
+            # use x_train_orig_subset for fitting explainer
+            x_train_subset = x_train.loc[data_sample_indices]
+            if y_train is not None:
+                y_train_subset = y_train.loc[data_sample_indices]
+                return x_train_subset, y_train_subset
+            return x_train_subset, None
+        else:
+            return x_train, y_train
```

### Comparing `pyreal-0.4.0/pyreal/explainers/dte/base.py` & `pyreal-0.4.1/pyreal/explainers/dte/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,22 +17,28 @@
            The training set for the explainer
         interpretable_features (Boolean):
             If True, return explanations using the interpretable feature descriptions instead of
             default names
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, interpretable_features=True, **kwargs):
+    def __init__(self, model, x_train_orig=None, interpretable_features=True, **kwargs):
         self.interpretable_features = interpretable_features
         super(DecisionTreeExplainerBase, self).__init__(model, x_train_orig, **kwargs)
 
     @abstractmethod
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit this explainer object
+
+        Args:
+             x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
 
     @abstractmethod
     def produce(self, x_orig=None):
         """
         Produce the decision tree explanation
 
@@ -48,15 +54,15 @@
         """
         Returns the (interpreted) features of the dataset.
 
         Returns:
             The features of the dataset. Interpret the features if
             `interpretable_features` is set to true.
         """
-        x_algorithm = self.transform_to_x_algorithm(self._x_train_orig)
+        x_algorithm = self.transform_to_x_algorithm(self.x_train_orig_subset)
 
         if self.interpretable_features:
             features = self.convert_columns_to_interpretable(x_algorithm).columns
         else:
             features = x_algorithm.columns
 
         return features
```

### Comparing `pyreal-0.4.0/pyreal/explainers/dte/surrogate_decision_tree.py` & `pyreal-0.4.1/pyreal/explainers/dte/surrogate_decision_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,38 +21,47 @@
         is_classifier (bool):
             Set this True for a classification model, False for a regression model.
         max_depth (int):
             The max_depth of the tree.
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, is_classifier=True, max_depth=None, **kwargs):
+    def __init__(self, model, x_train_orig=None, is_classifier=True, max_depth=None, **kwargs):
         self.explainer = None
         self.explainer_input_size = None
         self.is_classifer = is_classifier
         self.max_depth = max_depth
         super(SurrogateDecisionTree, self).__init__(model, x_train_orig, **kwargs)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the decision tree.
         TODO: Perhaps use sklearn's GridSearchCV to find the "best" tree.
+
+        Args:
+             x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
-        a_dataset = self.transform_to_x_algorithm(self._x_train_orig)
-        m_dataset = self.transform_to_x_model(self._x_train_orig)
+        x_train_orig = self._get_x_train_orig(x_train_orig)
+
+        a_dataset = self.transform_to_x_algorithm(x_train_orig)
+        m_dataset = self.transform_to_x_model(x_train_orig)
+
         self.explainer_input_size = a_dataset.shape[1]
         if self.is_classifer:
             self.explainer = tree.DecisionTreeClassifier(max_depth=self.max_depth)
             self.explainer.fit(a_dataset, self.model.predict(m_dataset))
         else:
             self.explainer = tree.DecisionTreeRegressor(max_depth=self.max_depth)
             self.explainer.fit(a_dataset, self.model.predict(m_dataset))
         return self
 
-    def produce(self):
+    def produce(self, x_orig=None):
         """
         Produce the explanation as a decision tree model.
 
         Returns:
             An explanation class in the form of a decision tree model
         """
```

### Comparing `pyreal-0.4.0/pyreal/explainers/gfi/base.py` & `pyreal-0.4.1/pyreal/explainers/gfi/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,29 @@
            The training set for the explainer
         interpretable_features (Boolean):
             If True, return explanations using the interpretable feature descriptions instead of
             default names
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, interpretable_features=True, **kwargs):
+    def __init__(self, model, x_train_orig=None, interpretable_features=True, **kwargs):
         self.interpretable_features = interpretable_features
         self.importance = None
         super(GlobalFeatureImportanceBase, self).__init__(model, x_train_orig, **kwargs)
 
     @abstractmethod
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit this explainer object
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
 
     def produce(self, x_orig=None):
         """
         Produce the global feature importance explanation
 
         Args:
@@ -95,10 +101,10 @@
         """
         if explanations is None:
             explanations = []
             for i in range(n_iterations - 1):
                 if with_fit:
                     self.fit()
                 explanations.append(
-                    self.produce(self._x_train_orig.iloc[0:n_rows]).get().to_numpy()
+                    self.produce(self.x_train_orig_subset.iloc[0:n_rows]).get().to_numpy()
                 )
         return np.max(np.var(explanations, axis=0))
```

### Comparing `pyreal-0.4.0/pyreal/explainers/gfi/permutation_feature_importance.py` & `pyreal-0.4.1/pyreal/explainers/gfi/permutation_feature_importance.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,36 +17,46 @@
         model (string filepath or model object):
            Filepath to the pickled model to explain, or model object with .predict() function
         x_train_orig (DataFrame of size (n_instances, n_features)):
             Training set in original form.
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, **kwargs):
+    def __init__(self, model, x_train_orig=None, **kwargs):
         self.explainer = None
         self.explainer_input_size = None
+        self.importance_from_fit = None
+
         super(PermutationFeatureImportance, self).__init__(model, x_train_orig, **kwargs)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the feature importance explainer.
         No-op as permutation_importance does not require fitting
+
+        Args:
+            y_train:
+            x_train_orig:
         """
+        x_train_orig, y_train = self._get_training_data(x_train_orig, y_train)
+
+        x = self.transform_to_x_model(x_train_orig)
+        columns = x.columns
+        x = np.asanyarray(x)
+        importance_result = permutation_importance(self.model, x, y_train, n_repeats=100)
+        importances = importance_result.importances_mean
+        self.importance_from_fit = pd.DataFrame(importances.reshape(1, -1), columns=columns)
+
         return self
 
     def get_importance(self):
         """
         Calculate the explanation of each feature using the permutation feature importance
         algorithm.
 
         Returns:
             DataFrame of shape (n_features, ):
                  The global importance of each feature
         """
-        x = self.transform_to_x_model(self._x_train_orig)
-        columns = x.columns
-        x = np.asanyarray(x)
-        importance_result = permutation_importance(self.model, x, self._y_orig, n_repeats=100)
-        importances = importance_result.importances_mean
-        return FeatureImportanceExplanation(
-            pd.DataFrame(importances.reshape(1, -1), columns=columns)
-        )
+        if self.importance_from_fit is None:
+            raise RuntimeError("Must fit explainer before calling produce!")
+        return FeatureImportanceExplanation(self.importance_from_fit)
```

### Comparing `pyreal-0.4.0/pyreal/explainers/gfi/shap_feature_importance.py` & `pyreal-0.4.1/pyreal/explainers/gfi/shap_feature_importance.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,67 +19,76 @@
         x_train_orig (DataFrame of size (n_instances, n_features)):
             Training set in original form.
         shap_type (string, one of ["kernel", "linear"]):
             Type of shap algorithm to use. If None, SHAP will pick one.
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, shap_type=None, **kwargs):
+    def __init__(self, model, x_train_orig=None, shap_type=None, **kwargs):
         supported_types = ["kernel", "linear"]
         if shap_type is not None and shap_type not in supported_types:
             raise ValueError(
                 "Shap type not supported, given %s, expected one of %s or None"
                 % (shap_type, str(supported_types))
             )
         else:
             self.shap_type = shap_type
 
         self.explainer = None
         self.explainer_input_size = None
+        self.importance_from_fit = None
+
         super(ShapFeatureImportance, self).__init__(model, x_train_orig, **kwargs)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the feature importance explainer
+
+        Args:
+            y_train:
+            x_train_orig:
         """
-        dataset = self.transform_to_x_model(self._x_train_orig)
-        self.explainer_input_size = dataset.shape[1]
+        x_train_orig = self._get_x_train_orig(x_train_orig)
+
+        x_model = self.transform_to_x_model(x_train_orig)
+        self.explainer_input_size = x_model.shape[1]
         if self.shap_type == "kernel":
-            self.explainer = KernelExplainer(self.model.predict, dataset)
+            self.explainer = KernelExplainer(self.model.predict, x_model)
         # Note: we manually check for linear model here because of SHAP bug
         elif self.shap_type == "linear":
-            self.explainer = LinearExplainer(self.model, dataset)
+            self.explainer = LinearExplainer(self.model, x_model)
         else:
-            self.explainer = ShapExplainer(self.model, dataset)  # SHAP will pick an algorithm
-        return self
-
-    def get_importance(self):
-        """
-        Calculate the explanation of each feature using SHAP.
+            self.explainer = ShapExplainer(self.model, x_model)  # SHAP will pick an algorithm
 
-        Returns:
-            DataFrame of shape (n_features, ):
-                 The global importance of each feature
-        """
-        if self.explainer is None:
-            raise AttributeError("Instance has no explainer. Must call fit() before produce()")
-        x_model = self.transform_to_x_model(self._x_train_orig)
         x_model_np = np.asanyarray(x_model)
         if isinstance(self.explainer, TreeExplainer):
             shap_values = np.array(self.explainer.shap_values(x_model_np, check_additivity=False))
         else:
             shap_values = np.array(self.explainer.shap_values(x_model_np))
 
         if shap_values.ndim < 2:
             raise RuntimeError("Something went wrong with SHAP - expected at least 2 dimensions")
         if shap_values.ndim > 2:
-            predictions = self.model_predict(self._x_train_orig)
+            predictions = self.model_predict(x_train_orig)
 
             if self.classes is not None:
                 predictions = [np.where(self.classes == i)[0][0] for i in predictions]
-
+            print(shap_values.shape)
+            print(predictions)
             shap_values = shap_values[predictions, np.arange(shap_values.shape[1]), :]
 
         importances = np.mean(np.absolute(shap_values), axis=0).reshape(1, -1)
-        return AdditiveFeatureImportanceExplanation(
-            pd.DataFrame(importances, columns=x_model.columns)
-        )
+        self.importance_from_fit = pd.DataFrame(importances, columns=x_model.columns)
+
+        return self
+
+    def get_importance(self):
+        """
+        Calculate the explanation of each feature using SHAP.
+
+        Returns:
+            DataFrame of shape (n_features, ):
+                 The global importance of each feature
+        """
+        if self.importance_from_fit is None:
+            raise RuntimeError("Must fit explainer before calling produce!")
+        return AdditiveFeatureImportanceExplanation(self.importance_from_fit)
```

### Comparing `pyreal-0.4.0/pyreal/explainers/lfc/base.py` & `pyreal-0.4.1/pyreal/explainers/lfc/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,28 @@
            The training set for the explainer
         interpretable_features (Boolean):
             If True, return explanations using the interpretable feature descriptions instead of
             default names
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, interpretable_features=True, **kwargs):
+    def __init__(self, model, x_train_orig=None, interpretable_features=True, **kwargs):
         self.interpretable_features = interpretable_features
         super(LocalFeatureContributionsBase, self).__init__(model, x_train_orig, **kwargs)
 
     @abstractmethod
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit this explainer object
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
 
     def produce(self, x_orig):
         """
         Produce the local feature contribution explanation
 
         Args:
@@ -108,11 +114,11 @@
         """
         if explanations is None:
             explanations = []
             for i in range(n_iterations - 1):
                 if with_fit:
                     self.fit()
                 explanations.append(
-                    self.produce(self._x_train_orig.iloc[0:n_rows]).get().to_numpy()
+                    self.produce(self.x_train_orig_subset.iloc[0:n_rows]).get().to_numpy()
                 )
 
         return np.max(np.var(explanations, axis=0))
```

### Comparing `pyreal-0.4.0/pyreal/explainers/lfc/shap_feature_contribution.py` & `pyreal-0.4.1/pyreal/explainers/lfc/shap_feature_contribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,33 +21,41 @@
         x_train_orig (DataFrame of size (n_instances, n_features)):
             Training set in original form.
         shap_type (string, one of ["kernel", "linear"]):
             Type of shap algorithm to use. If None, SHAP will pick one.
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, shap_type=None, **kwargs):
+    def __init__(self, model, x_train_orig=None, shap_type=None, **kwargs):
         supported_types = ["kernel", "linear"]
         if shap_type is not None and shap_type not in supported_types:
             raise ValueError(
                 "Shap type not supported, given %s, expected one of %s or None"
                 % (shap_type, str(supported_types))
             )
         else:
             self.shap_type = shap_type
 
         self.explainer = None
         self.explainer_input_size = None
         super(ShapFeatureContribution, self).__init__(model, x_train_orig, **kwargs)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the contribution explainer
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
-        dataset = self.transform_to_x_algorithm(self._x_train_orig)
+        x_train_orig = self._get_x_train_orig(x_train_orig)
+
+        dataset = self.transform_to_x_algorithm(x_train_orig)
         self.explainer_input_size = dataset.shape[1]
         if self.shap_type == "kernel":
             self.explainer = KernelExplainer(self.model.predict, dataset)
         # Note: we manually check for linear model here because of SHAP bug
         elif self.shap_type == "linear":
             self.explainer = LinearExplainer(self.model, dataset)
         else:
```

### Comparing `pyreal-0.4.0/pyreal/explainers/lfc/simple_counterfactual_contribution.py` & `pyreal-0.4.1/pyreal/explainers/lfc/simple_counterfactual_contribution.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     """
     SimpleCounterfactualContribution object.
 
     A SimpleCounterfactualContribution object gets feature contribution explanations by changing
     each feature to a set of other possible feature values through a random selection from the
     column, and then averaging the change in model prediction.
 
+    Note that this explainer will save the full dataset when fitting.
+
     Does not support classification models
 
     Expects categorical features rather than one-hot-encodings. Otherwise, can take any state.
 
     Args:
         model (string filepath or model object):
            Filepath to the pickled regression model to explain, or model object with .predict()
@@ -24,30 +26,38 @@
         x_train_orig (DataFrame of size (n_instances, n_features)):
             Training set in original form.
         n_iterations (int):
             Number of samples to replace each feature with.
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, n_iterations=30, **kwargs):
+    def __init__(self, model, x_train_orig=None, n_iterations=30, **kwargs):
         self.explainer_input_size = None
         self.n_iterations = n_iterations
         super(SimpleCounterfactualContribution, self).__init__(model, x_train_orig, **kwargs)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the contribution explainer
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
-        dataset = self.transform_to_x_algorithm(self._x_train_orig)
-        self.explainer_input_size = dataset.shape[1]
+        x_train_orig = self._get_x_train_orig(x_train_orig)
+
+        self.x_algo = self.transform_to_x_algorithm(x_train_orig)
+        self.explainer_input_size = self.x_algo.shape[1]
         return self
 
     def get_contributions(self, x_orig):
         """
-        Calculate the explanation of each feature in x using SHAP.
+        Calculate the explanation of each feature in x using the sample counterfactural algorithm.
 
         Args:
             x_orig (DataFrame of shape (n_instances, n_features)):
                The input to be explained
         Returns:
             DataFrame of shape (n_instances, n_features):
                  The contribution of each feature
@@ -55,19 +65,18 @@
         x = self.transform_to_x_algorithm(x_orig)
         if x.shape[1] != self.explainer_input_size:
             raise ValueError(
                 "Received input of wrong size.Expected ({},), received {}".format(
                     self.explainer_input_size, x.shape
                 )
             )
-        x_train_explain = self.transform_to_x_algorithm(self._x_train_orig)
         pred_orig = self.model_predict_on_algorithm(x)
         contributions = pd.DataFrame(np.zeros_like(x), columns=x.columns)
         for col in x:
             total_abs_change = 0
             for i in range(self.n_iterations):
                 x_copy = x.copy()
-                x_copy[col] = x_train_explain[col].sample().iloc[0]
+                x_copy[col] = self.x_algo[col].sample().iloc[0]
                 pred_new = self.model_predict_on_algorithm(x_copy)
                 total_abs_change += abs(pred_new - pred_orig)
             contributions[col] = total_abs_change / self.n_iterations
         return FeatureContributionExplanation(contributions)
```

### Comparing `pyreal-0.4.0/pyreal/explainers/time_series/saliency/base.py` & `pyreal-0.4.1/pyreal/explainers/time_series/saliency/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,28 @@
            .predict() should return probabilities of classes for classification,
             or numeric outputs for regression
         x_train_orig (dataframe of shape (n_instances, length of series)):
            The training set for the explainer
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig, interpretable_features=True, **kwargs):
+    def __init__(self, model, x_train_orig=None, interpretable_features=True, **kwargs):
         self.interpretable_features = interpretable_features
         super(SaliencyBase, self).__init__(model, x_train_orig, **kwargs)
 
     @abstractmethod
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
         """
         Fit this explainer object
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
         """
 
     def produce(self, x_orig):
         """
         Produce a saliency explanation for a univariate time series
 
         Args:
```

### Comparing `pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py` & `pyreal-0.4.1/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,44 +21,63 @@
     Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge
     Discovery and Data Mining. http://arxiv.org/abs/1602.04938)
 
     Can only take a single row input to .produce()
     """
 
     def __init__(
-        self, model, x_train_orig, y_orig, regression=False, suppress_prob_warnings=False, **kwargs
+        self,
+        model,
+        x_train_orig=None,
+        y_train=None,
+        regression=False,
+        suppress_prob_warnings=False,
+        **kwargs
     ):
         """
         Args:
             model (string filepath or model object):
                 Filepath to the pickled model to explain, or model object with .predict() function
             x_train_orig (DataFrame of size (n_instances, n_features)):
                 Training set in original form.
-            y_orig (DataFrame of shape (n_instances,)):
+            y_train (DataFrame of shape (n_instances,)):
                 The y values for the dataset
             regression (Boolean):
                 If true, model is a regression model.
                 If false, must provide a num_classes or classes parameter
             suppress_prob_warnings (Boolean):
                 LIME warns when class predictions do not sum to 1, because it suggests the model
                 is not predicting probabilites. In some cases, such as multilabel prediction,
                 this warning may be incorrect. In this case, set this parameter to True.
             **kwargs: see base Explainer args
         """
         self.suppress_prob_warnings = suppress_prob_warnings
         self.explainer = None
         self.regression = regression
-        super(UnivariateLimeSaliency, self).__init__(model, x_train_orig, y_orig=y_orig, **kwargs)
+        super(UnivariateLimeSaliency, self).__init__(
+            model, x_train_orig, y_train=y_train, **kwargs
+        )
 
-    def fit(self):
-        x_train_algo = self.transform_to_x_algorithm(self.x_train_orig)
+    def fit(self, x_train_orig=None, y_train=None):
+        """
+        Fit this explainer object
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
+        """
+        x_train_orig, y_train = self._get_training_data(x_train_orig, y_train)
+
+        x_train_algo = self.transform_to_x_algorithm(x_train_orig)
         num_timesteps = x_train_algo.shape[1]
 
         x_train_algo_np = np.copy(x_train_algo)[: self.training_size, :]
-        y_train_np = np.copy(self.y_orig)[: self.training_size]
+        y_train_np = np.copy(y_train)[: self.training_size]
 
         if self.regression:
             mode = "regression"
         else:
             mode = "classification"
 
         self.explainer = lime_tabular.RecurrentTabularExplainer(
```

### Comparing `pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py` & `pyreal-0.4.1/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,22 @@
     value by iteratively occluding windows of data, and calculating the resulting change in model
     prediction.
 
     Can only take a single row input to .produce()
     """
 
     def __init__(
-        self, model, x_train_orig, regression=False, width=5, k="avg", num_classes=None, **kwargs
+        self,
+        model,
+        x_train_orig=None,
+        regression=False,
+        width=5,
+        k="avg",
+        num_classes=None,
+        **kwargs
     ):
         """
         Generates a feature importance explanation of time-series type data by iteratively
         occluding windows of data and computing the change in model prediction
 
         Args:
             model (string filepath or model object):
@@ -55,15 +62,24 @@
         if self.num_classes is None and self.classes is None:
             raise ValueError(
                 "Must provide classes or num_classes parameter when regression is False"
             )
         elif self.num_classes is None:
             self.num_classes = len(self.classes)
 
-    def fit(self):
+    def fit(self, x_train_orig=None, y_train=None):
+        """
+        Fit this explainer object
+
+        Args:
+            x_train_orig (DataFrame of shape (n_instances, n_features):
+                Training set to fit on, required if not provided on initialization
+            y_train:
+                Targets of training set, required if not provided on initialization
+        """
         return self
 
     def get_contributions(self, x_orig):
         """
         Calculate the explanation of each feature in x using occlusion.
         Args:
             x_orig (DataFrame of shape (1, n_features)):
```

### Comparing `pyreal-0.4.0/pyreal/realapp/realapp.py` & `pyreal-0.4.1/pyreal/realapp/realapp.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     """
     Maintains all information about a Pyreal application to generate explanations
     """
 
     def __init__(
         self,
         models,
-        X_train_orig,
-        y_orig=None,
+        X_train_orig=None,
+        y_train=None,
         transformers=None,
         feature_descriptions=None,
         active_model_id=None,
         classes=None,
         class_descriptions=None,
         fit_transformers=False,
         id_column=None,
@@ -92,16 +92,16 @@
         """
         Initialize a RealApp object
 
         Args:
             models (model object, list of models, or dict of model_id:model):
                 Model(s) for this application
             X_train_orig (DataFrame of shape (n_instances,n_features):
-                Training data for models
-            y_orig (DataFrame of shape (n_instances,)):
+                Training data for models. If None, must be provided when preparing explainers.
+            y_train (DataFrame of shape (n_instances,)):
                 The y values for the dataset
             transformers (Transformer object or list of Transformer objects):
                 Transformers for this application
             feature_descriptions (dictionary of feature_name:feature_description):
                 Mapping of default feature names to readable names
             active_model_id (string or int):
                 ID of model to store as active model, if None, this is set to the first model
@@ -132,32 +132,42 @@
                 raise ValueError("active_model_id not in models")
             self.active_model_id = active_model_id
         else:
             self.active_model_id = next(iter(self.models))
 
         self.id_column = id_column
 
-        if self.id_column is not None and self.id_column in X_train_orig:
+        if (
+            X_train_orig is not None
+            and self.id_column is not None
+            and self.id_column in X_train_orig
+        ):
             self.X_train_orig = X_train_orig.drop(columns=self.id_column)
         else:
             self.X_train_orig = X_train_orig
-        self.y_orig = y_orig
+        self.y_train = y_train
 
         self.classes = classes
         self.class_descriptions = class_descriptions
 
         if isinstance(transformers, list):
             self.transformers = transformers
         else:  # assume single transformer given
             self.transformers = [transformers]
         self.transformers = transformers
         self.feature_descriptions = feature_descriptions
 
-        self.fit_transformers = fit_transformers
-        self.transformers_fitted = False
+        if fit_transformers:
+            # Hacky way of fitting transformers, may want to clean up later
+            Explainer(
+                self.models[next(iter(self.models))],
+                X_train_orig,
+                transformers=self.transformers,
+                fit_transformers=True,
+            )
 
         # Base explainer used for general transformations and model predictions
         # Also validates data, model, and transformers
         self.base_explainers = {
             model_id: self._make_base_explainer(self.models[model_id]) for model_id in self.models
         }
 
@@ -171,28 +181,18 @@
         Args:
             model (model object):
                 The model to be explained by this explainer
         Returns:
             Explainer
                 The explainer
         """
-        fit_transformers = False
-
-        if self.fit_transformers and not self.transformers_fitted:
-            self.transformers_fitted = True
-            fit_transformers = True
-            print("fitting transformers")
-
         return Explainer(
             model,
-            self.X_train_orig,
-            y_orig=self.y_orig,
             transformers=self.transformers,
             feature_descriptions=self.feature_descriptions,
-            fit_transformers=fit_transformers,
         )
 
     def _explainer_exists(self, explanation_type, algorithm):
         """
         Check if the requested explainer exists
 
         Args:
@@ -244,14 +244,16 @@
 
     def _produce_explanation_helper(
         self,
         explanation_type_code,
         algorithm,
         prepare_explainer_func,
         format_output_func,
+        x_train_orig=None,
+        y_train=None,
         x_orig=None,
         model_id=None,
         force_refit=False,
         **kwargs
     ):
         """
         Produce an explanation from a specified Explainer
@@ -261,14 +263,18 @@
                 Code for explanation_type
             algorithm (string):
                 Name of algorithm
             prepare_explainer_func (function):
                 Function that initializes and fits the appropriate explainer
             format_output_func (function):
                 Function that formats Explanation objects into the appropriate output format
+            x_train_orig (DataFrame of shape (n_instances, n_features)):
+                Training data, if not provided at initialization.
+            y_train (DataFrame or Series):
+                Training targets, if not provided at initialization
             x_orig (DataFrame):
                 Data to explain, required for local explanations
             model_id (string or int):
                 ID of model to explain
             force_refit (Boolean):
                 If True, initialize and fit a new explainer even if the appropriate explainer
                 already exists
@@ -281,15 +287,21 @@
         """
         if model_id is None:
             model_id = self.active_model_id
 
         if self._explainer_exists(explanation_type_code, algorithm) and not force_refit:
             explainer = self._get_explainer(explanation_type_code, algorithm)
         else:
-            explainer = prepare_explainer_func(model_id=model_id, algorithm=algorithm, **kwargs)
+            explainer = prepare_explainer_func(
+                model_id=model_id,
+                algorithm=algorithm,
+                x_train_orig=x_train_orig,
+                y_train=y_train,
+                **kwargs
+            )
 
         if x_orig is not None:
             ids = None
 
             if self.id_column is not None and self.id_column in x_orig:
                 ids = x_orig[self.id_column]
                 x_orig = x_orig.drop(columns=self.id_column)
@@ -373,66 +385,83 @@
             return preds
         preds_dict = {}
         for i, row_id in enumerate(ids):
             preds_dict[row_id] = preds[i]
         return preds_dict
 
     def prepare_feature_contributions(
-        self, model_id=None, algorithm=None, shap_type=None, training_size=None
+        self,
+        model_id=None,
+        x_train_orig=None,
+        y_train=None,
+        algorithm=None,
+        shap_type=None,
+        training_size=None,
     ):
         """
         Initialize and fit a local feature contribution explainer
 
         Args:
             model_id (int or string):
                 Model id to explain
+            x_train_orig (DataFrame of shape (n_instances, n_features)):
+                Training data, if not provided at initialization.
+            y_train (DataFrame or Series):
+                Training targets, if not provided at initialization
             algorithm (string):
                 LFC algorithm to use
             shap_type (string):
                 If algorithm is "shap", type of shap to use
 
         Returns:
             A fit LocalFeatureContribution explainer
         """
         if algorithm is None:
             algorithm = "shap"
 
+        if model_id is None:
+            model_id = self.active_model_id
+
         explainer = LocalFeatureContribution(
             self.models[model_id],
-            self.X_train_orig,
-            y_orig=self.y_orig,
             transformers=self.transformers,
             feature_descriptions=self.feature_descriptions,
             e_algorithm=algorithm,
             shap_type=shap_type,
             classes=self.classes,
             class_descriptions=self.class_descriptions,
-            fit_on_init=True,
             training_size=training_size,
         )
+        explainer.fit(self._get_x_train_orig(x_train_orig), self._get_y_train(y_train))
         self._add_explainer("lfc", algorithm, explainer)
         return explainer
 
     def produce_feature_contributions(
         self,
         x_orig,
         model_id=None,
+        x_train_orig=None,
+        y_train=None,
         algorithm=None,
         shap_type=None,
         force_refit=False,
         training_size=None,
     ):
         """
         Produce a feature contribution explanation
 
         Args:
             x_orig (DataFrame):
                 Input to explain
             model_id (string or int):
                 ID of model to explain
+            x_train_orig (DataFrame):
+                Data to fit on, if not provided during initialization
+            y_train (DataFrame or Series):
+                Training targets to fit on, if not provided during initialization
             algorithm (string):
                 Name of algorithm
             shap_type (string):
                 If algorithm="shap", type of SHAP explainer to use
             force_refit (Boolean):
                 If True, initialize and fit a new explainer even if the appropriate explainer
                 already exists
@@ -445,70 +474,89 @@
             algorithm = "shap"
 
         return self._produce_explanation_helper(
             "lfc",
             algorithm,
             self.prepare_feature_contributions,
             format_feature_contribution_output,
+            x_train_orig=x_train_orig,
+            y_train=y_train,
             x_orig=x_orig,
             model_id=model_id,
             force_refit=force_refit,
             shap_type=shap_type,
             training_size=training_size,
         )
 
     def prepare_feature_importance(
-        self, model_id=None, algorithm=None, shap_type=None, training_size=None
+        self,
+        model_id=None,
+        x_train_orig=None,
+        y_train=None,
+        algorithm=None,
+        shap_type=None,
+        training_size=None,
     ):
         """
         Initialize and fit a global feature importance explainer
 
         Args:
             model_id (int or string):
                 Model id to explain
+            x_train_orig (DataFrame of shape (n_instances, n_features)):
+                Training data, if not provided at initialization.
+            y_train (DataFrame or Series):
+                Training targets, if not provided at initialization
             algorithm (string):
                 GFI algorithm to use
             shap_type (string):
                 If algorithm is "shap", type of shap to use
 
         Returns:
             A fit GlobalFeatureImportance explainer
         """
         if algorithm is None:
             algorithm = "shap"
 
+        if model_id is None:
+            model_id = self.active_model_id
+
         explainer = GlobalFeatureImportance(
             self.models[model_id],
-            self.X_train_orig,
-            y_orig=self.y_orig,
             transformers=self.transformers,
             feature_descriptions=self.feature_descriptions,
             e_algorithm=algorithm,
             classes=self.classes,
             class_descriptions=self.class_descriptions,
             shap_type=shap_type,
-            fit_on_init=True,
             training_size=training_size,
         )
+        explainer.fit(self._get_x_train_orig(x_train_orig), self._get_y_train(y_train))
         self._add_explainer("gfi", algorithm, explainer)
         return explainer
 
     def produce_feature_importance(
         self,
         model_id=None,
+        x_train_orig=None,
+        y_train=None,
         algorithm=None,
         shap_type=None,
         force_refit=False,
     ):
         """
         Produce a GlobalFeatureImportance explainer
 
         Args:
             model_id (string or int):
                 ID of model to explain
+            x_train_orig (DataFrame):
+                Data to fit on, if not provided during initialization
+            y_train (DataFrame or Series):
+                Training targets to fit on, if not provided during initialization
             algorithm (string):
                 Name of algorithm
             shap_type (string):
                 If algorithm="shap", type of SHAP explainer to use
             force_refit (Boolean):
                 If True, initialize and fit a new explainer even if the appropriate explainer
                 already exists
@@ -521,10 +569,40 @@
 
         return self._produce_explanation_helper(
             "gfi",
             algorithm,
             self.prepare_feature_importance,
             format_feature_importance_output,
             model_id=model_id,
+            x_train_orig=x_train_orig,
+            y_train=y_train,
             force_refit=force_refit,
             shap_type=shap_type,
         )
+
+    def _get_x_train_orig(self, x_train_orig):
+        """
+        Helper function to get the appropriate x_orig or raise errors if something goes wrong
+        Args:
+            x_train_orig (DataFrame or None):
+                Provided DataFrame
+        Returns:
+            The dataframe to use (x_orig or self.x_train_orig), may be None if neither is given
+        """
+        if x_train_orig is not None:
+            return x_train_orig
+        else:
+            return self.X_train_orig
+
+    def _get_y_train(self, y_train):
+        """
+        Helper function to get the appropriate y or raise errors if something goes wrong
+        Args:
+            y (DataFrame or None):
+                Provided DataFrame
+        Returns:
+            The dataframe to use (y or self.y_train), may be None if neither is given
+        """
+        if y_train is not None:
+            return y_train
+        else:
+            return self.y_train
```

### Comparing `pyreal-0.4.0/pyreal/sample_applications/ames_housing.py` & `pyreal-0.4.1/pyreal/sample_applications/ames_housing.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,12 +167,12 @@
     model = load_model()
     transformers = load_transformers()
     feature_descriptions = load_feature_descriptions()
 
     return RealApp(
         model,
         x_train_orig,
-        y_orig=y,
+        y_train=y,
         transformers=transformers,
         feature_descriptions=feature_descriptions,
         id_column="Id",
     )
```

### Comparing `pyreal-0.4.0/pyreal/sample_applications/california_housing.py` & `pyreal-0.4.1/pyreal/sample_applications/california_housing.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data_description.txt` & `pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/data_description.txt`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/california.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_cal_housing/california.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_student/data.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_student/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_student/students.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_student/students.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/data_titanic/data.csv` & `pyreal-0.4.1/pyreal/sample_applications/data_titanic/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/sample_applications/student_performance.py` & `pyreal-0.4.1/pyreal/sample_applications/student_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,12 +131,12 @@
     model = load_model()
     transformers = load_transformers()
     feature_descriptions = load_feature_descriptions()
 
     return RealApp(
         model,
         x_train_orig,
-        y_orig=y,
+        y_train=y,
         transformers=transformers,
         feature_descriptions=feature_descriptions,
         id_column="name",
     )
```

### Comparing `pyreal-0.4.0/pyreal/sample_applications/titanic.py` & `pyreal-0.4.1/pyreal/sample_applications/titanic.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 def load_model():
     if os.path.exists(MODEL_FILE):
         return pickle.load(open(os.path.join(DATA_DIR, "model.pkl"), "rb"))
     else:
         transformers = load_transformers()
         x_orig, y = load_data(include_targets=True)
         x_model = run_transformers(transformers, x_orig)
-        # model = LogisticRegression(max_iter=500)
         model = LGBMClassifier()
         model.fit(x_model, y)
 
         if not os.path.isdir(DATA_DIR):
             os.mkdir(DATA_DIR)
         with open(MODEL_FILE, "wb") as f:
             pickle.dump(model, f)
@@ -99,11 +98,11 @@
     model = load_model()
     transformers = load_transformers()
     feature_descriptions = load_feature_descriptions()
 
     return RealApp(
         model,
         x_train_orig,
-        y_orig=y,
+        y_train=y,
         transformers=transformers,
         feature_descriptions=feature_descriptions,
     )
```

### Comparing `pyreal-0.4.0/pyreal/transformers/__init__.py` & `pyreal-0.4.1/pyreal/transformers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     Numpy2dToNestedFrame,
     Numpy3dToMultiIndexFrame,
     Numpy3dToNestedFrame,
     Pandas2dToMultiIndexFrame,
 )
 from pyreal.transformers.wrappers import DataFrameWrapper
 from pyreal.transformers.pad import TimeSeriesPadder
+from pyreal.transformers.type_cast import BoolToIntCaster
 
 __all__ = [
     "Transformer",
     "fit_transformers",
     "run_transformers",
     "DimensionAdder",
     "BreakingTransformError",
@@ -53,8 +54,9 @@
     "NestedFrameToNumpy3d",
     "Numpy2dToMultiIndexFrame",
     "Numpy2dToNestedFrame",
     "Numpy3dToMultiIndexFrame",
     "Numpy3dToNestedFrame",
     "Pandas2dToMultiIndexFrame",
     "TimeSeriesPadder",
+    "BoolToIntCaster",
 ]
```

### Comparing `pyreal-0.4.0/pyreal/transformers/base.py` & `pyreal-0.4.1/pyreal/transformers/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/transformers/feature_select.py` & `pyreal-0.4.1/pyreal/transformers/feature_select.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/transformers/impute.py` & `pyreal-0.4.1/pyreal/transformers/impute.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         )
 
         self.means = x[self.numeric_cols].mean(axis=0)
         self.modes = x[self.categorical_cols].mode(axis=0)
         if self.modes.shape[0] > 0:
             self.modes = self.modes.iloc[0, :]
 
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Imputes `x`. Numeric columns get imputed with the column mean. Categorical columns get
         imputed with the column mode.
         Args:
             x (DataFrame of shape (n_instances, n_features)):
```

### Comparing `pyreal-0.4.0/pyreal/transformers/one_hot_encode.py` & `pyreal-0.4.1/pyreal/transformers/one_hot_encode.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         Returns:
             None
         """
 
         if self.columns is None:
             self.columns = x.columns
         self.ohe.fit(x[self.columns])
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         One-hot encode `x`.
         Args:
             x (DataFrame of shape (n_instances, n_features)):
                 The dataset to transform
```

### Comparing `pyreal-0.4.0/pyreal/transformers/pad.py` & `pyreal-0.4.1/pyreal/transformers/pad.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
         """
         if self.length is None:
             if isinstance(x, pd.DataFrame):
                 self.length = x.shape[1]
             else:
                 self.length = len(max(x, key=lambda x_: len(x_)))
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Reorders and selects the features in x. If no length has been set
         and the transformer has not been fit, pad to the longest subsequence length
 
         Args:
```

### Comparing `pyreal-0.4.0/pyreal/transformers/sax.py` & `pyreal-0.4.1/pyreal/transformers/sax.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/transformers/time_series_formatter.py` & `pyreal-0.4.1/pyreal/transformers/time_series_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         else:
             if isinstance(self.var_name, str):
                 self.mi = pd.MultiIndex.from_product([[self.var_name], self.timestamps])
             elif isinstance(self.var_name, (list, pd.Index)):
                 self.mi = pd.MultiIndex.from_product([self.var_name, self.timestamps])
             else:
                 raise TypeError(f"var_name must be a String, received type: {type(self.var_name)}")
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Converts input data into a DataFrame with MultiIndex columns
 
         Args:
             x (ndarray of shape (n_instances, n_timepoints)):
@@ -191,15 +191,15 @@
         # create indices for MultiIndex DataFrame
         if self.var_name is None:
             self.mi = pd.MultiIndex.from_product([["var_0"], columns])
         else:
             if not isinstance(self.var_name, str):
                 raise TypeError(f"var_name must be a String, received type: {type(self.var_name)}")
             self.mi = pd.MultiIndex.from_product([[self.var_name], columns])
-        super().fit()
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Converts input data into a DataFrame with MultiIndex columns
 
         Args:
             x (DataFrame of shape (n_instances, n_timepoints)):
@@ -255,15 +255,15 @@
             if len(self.timestamps) != n_timepoints:
                 raise TypeError(
                     f"Input data has {n_timepoints} timepoints, but only "
                     f"{len(self.timestamps)} steps are supplied in timestamps."
                 )
 
         self.mi = pd.MultiIndex.from_product([self.var_names, self.timestamps])
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Converts input data into a DataFrame with MultiIndex column
 
         Args:
             x (ndarray with shape (n_instances, n_columns, n_timepoints)):
@@ -326,15 +326,15 @@
         # use the values of an instance of a single variable as inference
         sample_series = x.iloc[0][0]
 
         self.var_names = x.columns
         self.timestamps = sample_series.index
 
         self.mi = pd.MultiIndex.from_product([self.var_names, self.timestamps])
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Converts input data into a DataFrame with MultiIndex columns
 
         Args:
             x (pandas DataFrame):
@@ -441,14 +441,15 @@
         Check if the input data is a NumPy 2D array
 
         Args:
             x (ndarray of shape (n_instances, n_timepoints)):
                 Input ndarray
         """
         fit_transformers(self._transformers, x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Convert input NumPy 2D array into sktime nested DataFrame.
         """
         return run_transformers(self._transformers, x)
 
@@ -479,14 +480,15 @@
         Check if the input data is a NumPy 3D array
 
         Args:
             x (ndarray of shape (n_instances, n_timepoints)):
                 Input ndarray
         """
         fit_transformers(self._transformers, x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Convert input NumPy 3D array into sktime nested DataFrame.
         """
         return run_transformers(self._transformers, x)
```

### Comparing `pyreal-0.4.0/pyreal/transformers/wrappers.py` & `pyreal-0.4.1/pyreal/transformers/wrappers.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             **params:
                 Additional transformer parameters
 
         Returns:
             None
         """
         self.wrapped_transformer.fit(x)
-        super().fit(x)
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Transform `x` using the wrapped transformer
         Args:
             x (DataFrame of shape (n_instances, n_features)):
                 The dataset to transform
```

### Comparing `pyreal-0.4.0/pyreal/types/explanations/base.py` & `pyreal-0.4.1/pyreal/types/explanations/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/types/explanations/decision_tree.py` & `pyreal-0.4.1/pyreal/types/explanations/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/types/explanations/feature_based.py` & `pyreal-0.4.1/pyreal/types/explanations/feature_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/types/explanations/time_series_saliency.py` & `pyreal-0.4.1/pyreal/types/explanations/time_series_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/utils/_plot_tree.py` & `pyreal-0.4.1/pyreal/utils/_plot_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/utils/dataloader.py` & `pyreal-0.4.1/pyreal/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/utils/model_utils.py` & `pyreal-0.4.1/pyreal/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/visualize/__init__.py` & `pyreal-0.4.1/pyreal/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/visualize/feature_based_vis.py` & `pyreal-0.4.1/pyreal/visualize/feature_based_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/visualize/time_series_vis.py` & `pyreal-0.4.1/pyreal/visualize/time_series_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/visualize/tree_vis.py` & `pyreal-0.4.1/pyreal/visualize/tree_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/pyreal/visualize/visualize_config.py` & `pyreal-0.4.1/pyreal/visualize/visualize_config.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.0/PKG-INFO` & `pyreal-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreal
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for evaluating and deploying human readable machine learning explanations.
 Home-page: https://sibyl-ml.dev/
 Keywords: pyreal,Pyreal
 Author: Alexandra Zytek
 Author-email: zyteka@mit.edu
 Maintainer: MIT Data To AI Lab
 Maintainer-email: dailabmit@gmail.com
@@ -133,15 +133,15 @@
 ![Quickstart](docs/images/titanic.png)
 
 We can see here that the input passenger's predicted chance of survival was greatly reduced
 because of their sex (male) and ticket class (3rd class).
 
 ### Terminology
 Pyreal introduces specific terms and naming schemes to refer to different feature spaces and
-transformations. The [Terminology User Guide](https://sibyl-ml.dev/pyreal/user_guides/transformer_workflow.html#terminology) provides an introduction to these terms.
+transformations. The [Terminology User Guide](https://dtail.gitbook.io/pyreal/developing-applications/developer-terminology-guide) provides an introduction to these terms.
 
 # What's next?
 
 For more details about **Pyreal** and all its possibilities
 and features, please check the [documentation site](
 https://dtail.gitbook.io/pyreal/).
```

