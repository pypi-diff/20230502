# Comparing `tmp/whacc-1.3.8.tar.gz` & `tmp/whacc-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whacc-1.3.8.tar", last modified: Thu Jan 12 22:51:44 2023, max compression
+gzip compressed data, was "dist/whacc-1.3.9.tar", last modified: Fri Jan 13 19:25:54 2023, max compression
```

## Comparing `whacc-1.3.8.tar` & `whacc-1.3.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.148955 whacc-1.3.8/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-05-10 20:03:18.000000 whacc-1.3.8/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      289 2022-11-05 19:49:52.000000 whacc-1.3.8/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)     2344 2023-01-12 22:51:44.148501 whacc-1.3.8/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1575 2023-01-12 22:48:12.000000 whacc-1.3.8/README.md
--rw-r--r--   0 phil       (501) staff       (20)      274 2022-05-10 20:03:18.000000 whacc-1.3.8/full_requirements.txt
--rw-r--r--   0 phil       (501) staff       (20)      801 2022-05-10 20:03:18.000000 whacc-1.3.8/lfs-files.txt
--rw-r--r--   0 phil       (501) staff       (20)      420 2022-11-16 22:36:32.000000 whacc-1.3.8/requirements.txt
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-01-12 22:51:44.149102 whacc-1.3.8/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     2582 2023-01-12 22:51:16.000000 whacc-1.3.8/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.823905 whacc-1.3.8/whacc/
--rw-r--r--   0 phil       (501) staff       (20)    14340 2023-01-06 21:33:26.000000 whacc-1.3.8/whacc/.DS_Store
--rw-r--r--   0 phil       (501) staff       (20)    12288 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/.gitattributes.swp
--rw-r--r--   0 phil       (501) staff       (20)      341 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.830464 whacc-1.3.8/whacc/__pycache__/
--rw-r--r--   0 phil       (501) staff       (20)      365 2022-05-10 21:02:15.000000 whacc-1.3.8/whacc/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    16027 2022-10-25 23:40:12.000000 whacc-1.3.8/whacc/__pycache__/analysis.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    18536 2022-11-09 19:12:35.000000 whacc-1.3.8/whacc/__pycache__/feature_maker.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    50852 2022-07-14 16:43:58.000000 whacc-1.3.8/whacc/__pycache__/image_tools.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    11135 2022-11-04 05:27:07.000000 whacc-1.3.8/whacc/__pycache__/model_maker.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    20173 2022-11-01 19:56:48.000000 whacc-1.3.8/whacc/__pycache__/pole_tracker.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)     7125 2022-12-21 18:51:26.000000 whacc-1.3.8/whacc/__pycache__/retrain_LGBM.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)     7485 2022-05-10 21:02:15.000000 whacc-1.3.8/whacc/__pycache__/subset_h5_generator.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)     6713 2022-11-04 21:23:44.000000 whacc-1.3.8/whacc/__pycache__/touch_curation_GUI.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)     9716 2022-05-10 21:04:08.000000 whacc-1.3.8/whacc/__pycache__/transfer_learning.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    77723 2022-12-16 21:44:24.000000 whacc-1.3.8/whacc/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    25062 2022-10-25 23:35:45.000000 whacc-1.3.8/whacc/analysis.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.865596 whacc-1.3.8/whacc/examples/
--rw-r--r--   0 phil       (501) staff       (20)     2931 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/0.5 before batch processing.py
--rw-r--r--   0 phil       (501) staff       (20)     2519 2022-10-31 23:50:36.000000 whacc-1.3.8/whacc/examples/1_make_h5_example.py
--rw-r--r--   0 phil       (501) staff       (20)     1202 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/2_predict_touches_example.py
--rw-r--r--   0 phil       (501) staff       (20)     3137 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/3_make_subset_H5_example.py
--rw-r--r--   0 phil       (501) staff       (20)     5182 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/4_augment_H5_example.py
--rw-r--r--   0 phil       (501) staff       (20)     1931 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/5_split_data_for_retrain_example.py
--rw-r--r--   0 phil       (501) staff       (20)     3133 2022-05-10 21:10:53.000000 whacc-1.3.8/whacc/examples/6_retrain_example.py
--rw-r--r--   0 phil       (501) staff       (20)      343 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/7.5_convert_h5_to_features.py
--rw-r--r--   0 phil       (501) staff       (20)     6702 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/7_select_TL_trials.py
--rw-r--r--   0 phil       (501) staff       (20)     8541 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/8_make_feature_data.py
--rw-r--r--   0 phil       (501) staff       (20)      900 2023-01-06 21:35:15.000000 whacc-1.3.8/whacc/examples/9_re_train_GBM_EXAMPLE.py
--rw-r--r--   0 phil       (501) staff       (20)    80894 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/CNN_+lightGBM_V5_Testing_GPU_RAM_limits_V2.py
--rw-r--r--   0 phil       (501) staff       (20)    31926 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/SCRATCH5.py
--rw-r--r--   0 phil       (501) staff       (20)     9462 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/TL_10_20_30.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2021-04-02 17:08:45.000000 whacc-1.3.8/whacc/examples/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      608 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/add_pole_times.py
--rw-r--r--   0 phil       (501) staff       (20)     6516 2022-10-27 22:57:01.000000 whacc-1.3.8/whacc/examples/best_T1V1t2_model.py
--rw-r--r--   0 phil       (501) staff       (20)     2024 2022-07-20 20:27:10.000000 whacc-1.3.8/whacc/examples/colors.py
--rw-r--r--   0 phil       (501) staff       (20)    22067 2022-12-16 18:22:47.000000 whacc-1.3.8/whacc/examples/compare_models_for_feature_selection.py
--rw-r--r--   0 phil       (501) staff       (20)    47144 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/convert_h5_to_feature_h5.py
--rw-r--r--   0 phil       (501) staff       (20)     2135 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/copy_temp.py
--rw-r--r--   0 phil       (501) staff       (20)    15933 2022-07-27 22:42:00.000000 whacc-1.3.8/whacc/examples/define_in_range.py
--rw-r--r--   0 phil       (501) staff       (20)     7938 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/diff_h5_creator.py
--rw-r--r--   0 phil       (501) staff       (20)     1765 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/error_analysis_example.py
--rw-r--r--   0 phil       (501) staff       (20)    11718 2022-07-18 16:29:23.000000 whacc-1.3.8/whacc/examples/final_CNN_performance_with_final_mathcing_datasets.py
--rw-r--r--   0 phil       (501) staff       (20)     2081 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/full_pipeline.py
--rw-r--r--   0 phil       (501) staff       (20)     4738 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/full_pipeline_no_transfer_learning.py
--rw-r--r--   0 phil       (501) staff       (20)    64731 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/gists.py
--rw-r--r--   0 phil       (501) staff       (20)      351 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/gui_example.py
--rw-r--r--   0 phil       (501) staff       (20)     1039 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/h5_tester.py
--rw-r--r--   0 phil       (501) staff       (20)    21539 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/heat_map_plotter.py
--rw-r--r--   0 phil       (501) staff       (20)    19294 2022-07-12 20:31:05.000000 whacc-1.3.8/whacc/examples/heat_mapper_boost_mods.py
--rw-r--r--   0 phil       (501) staff       (20)    21698 2022-10-12 23:12:01.000000 whacc-1.3.8/whacc/examples/heatmap_maker.py
--rw-r--r--   0 phil       (501) staff       (20)     8594 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/load_all_predictions_from_all_100_final_models_for_cloud.py
--rw-r--r--   0 phil       (501) staff       (20)    51448 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/lstm_transfer_learning_lstm_using_subsets_v3.py
--rw-r--r--   0 phil       (501) staff       (20)      848 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/make_master_training_H5_example.py
--rw-r--r--   0 phil       (501) staff       (20)    27736 2022-11-14 18:35:39.000000 whacc-1.3.8/whacc/examples/make_new_data_and train.py
--rw-r--r--   0 phil       (501) staff       (20)    35432 2022-07-29 17:01:48.000000 whacc-1.3.8/whacc/examples/pack_samsons_data.py
--rw-r--r--   0 phil       (501) staff       (20)     2034 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/re_pole_down.py
--rw-r--r--   0 phil       (501) staff       (20)    52560 2022-12-21 17:10:15.000000 whacc-1.3.8/whacc/examples/redo_all_data.py
--rw-r--r--   0 phil       (501) staff       (20)    21737 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/run_all_model.py
--rw-r--r--   0 phil       (501) staff       (20)    13587 2022-07-26 17:45:35.000000 whacc-1.3.8/whacc/examples/scratch4.py
--rw-r--r--   0 phil       (501) staff       (20)   177391 2022-08-04 05:25:56.000000 whacc-1.3.8/whacc/examples/scratch8.py
--rw-r--r--   0 phil       (501) staff       (20)   127311 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/scratch_3.py
--rw-r--r--   0 phil       (501) staff       (20)    12424 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/subset_to_altered_for_training.py
--rw-r--r--   0 phil       (501) staff       (20)     4500 2022-10-27 20:23:28.000000 whacc-1.3.8/whacc/examples/temp_TVt1_and_TVt2_model_directories.py
--rw-r--r--   0 phil       (501) staff       (20)    13881 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/test_training_with_worst_trials.py
--rw-r--r--   0 phil       (501) staff       (20)    28149 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/testing_LSTM_model_defnitions.py
--rw-r--r--   0 phil       (501) staff       (20)    16560 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/testing_batch_predicting.py
--rw-r--r--   0 phil       (501) staff       (20)     5833 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/examples/var_rename_scratch.py
--rw-r--r--   0 phil       (501) staff       (20)    37211 2022-11-08 21:58:45.000000 whacc-1.3.8/whacc/feature_maker.py
--rw-r--r--   0 phil       (501) staff       (20)    31109 2022-05-10 21:52:37.000000 whacc-1.3.8/whacc/feature_maker_temp.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.878266 whacc-1.3.8/whacc/figures/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-23 02:21:16.000000 whacc-1.3.8/whacc/figures/CNN_plots.py
--rw-r--r--   0 phil       (501) staff       (20)     3806 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/FIG_2_border_touches_explained.py
--rw-r--r--   0 phil       (501) staff       (20)     7974 2022-10-25 17:14:30.000000 whacc-1.3.8/whacc/figures/FIG_2_pie_graph_percentages.py
--rw-r--r--   0 phil       (501) staff       (20)     4607 2022-10-28 20:21:01.000000 whacc-1.3.8/whacc/figures/FIG_2_pie_graph_percentages_V2.py
--rw-r--r--   0 phil       (501) staff       (20)     4060 2022-08-03 20:27:24.000000 whacc-1.3.8/whacc/figures/PSTH neuron compare.py
--rw-r--r--   0 phil       (501) staff       (20)    14690 2022-10-17 17:21:34.000000 whacc-1.3.8/whacc/figures/PSTH_V1.py
--rw-r--r--   0 phil       (501) staff       (20)    17331 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/SHAP_histograms.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.8/whacc/figures/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.879949 whacc-1.3.8/whacc/figures/__pycache__/
--rw-r--r--   0 phil       (501) staff       (20)      159 2022-05-13 18:55:43.000000 whacc-1.3.8/whacc/figures/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)     1886 2022-11-16 19:00:17.000000 whacc-1.3.8/whacc/figures/__pycache__/pretty_plots.cpython-38.pyc
--rw-r--r--   0 phil       (501) staff       (20)    22218 2022-11-18 04:31:35.000000 whacc-1.3.8/whacc/figures/all agree analysis fig V2.py
--rw-r--r--   0 phil       (501) staff       (20)     6503 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/all agree analysis.py
--rw-r--r--   0 phil       (501) staff       (20)    16803 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/error_analysis_explained_critical_errors.py
--rw-r--r--   0 phil       (501) staff       (20)     1873 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/error_type_analysis.py
--rw-r--r--   0 phil       (501) staff       (20)     3601 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/features_with_video.py
--rw-r--r--   0 phil       (501) staff       (20)    10434 2022-10-27 20:30:32.000000 whacc-1.3.8/whacc/figures/fig_3_model_compare.py
--rw-r--r--   0 phil       (501) staff       (20)    18580 2022-10-31 00:33:54.000000 whacc-1.3.8/whacc/figures/fig_3_model_compare_V2.py
--rw-r--r--   0 phil       (501) staff       (20)     3039 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/get_feature_names.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.880743 whacc-1.3.8/whacc/figures/load/
--rw-r--r--   0 phil       (501) staff       (20)     1936 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/load/load.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.881665 whacc-1.3.8/whacc/figures/not_using/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-22 13:38:53.000000 whacc-1.3.8/whacc/figures/not_using/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    13634 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/figures/not_using/simulation_simple.py
--rw-r--r--   0 phil       (501) staff       (20)     3118 2022-12-12 21:51:34.000000 whacc-1.3.8/whacc/figures/pretty_plots.py
--rw-r--r--   0 phil       (501) staff       (20)        2 2022-07-25 16:53:43.000000 whacc-1.3.8/whacc/figures/top4_critical_errors_.py
--rw-r--r--   0 phil       (501) staff       (20)    25739 2022-11-17 02:13:24.000000 whacc-1.3.8/whacc/figures/what_features_look_like.py
--rw-r--r--   0 phil       (501) staff       (20)     3460 2022-11-16 20:01:53.000000 whacc-1.3.8/whacc/figures/whisker_images.py
--rw-r--r--   0 phil       (501) staff       (20)    88984 2022-07-14 16:42:39.000000 whacc-1.3.8/whacc/image_tools.py
--rw-r--r--   0 phil       (501) staff       (20)    14284 2022-11-04 05:26:34.000000 whacc-1.3.8/whacc/model_maker.py
--rw-r--r--   0 phil       (501) staff       (20)    31801 2022-11-01 19:56:21.000000 whacc-1.3.8/whacc/pole_tracker.py
--rw-r--r--   0 phil       (501) staff       (20)    11487 2022-12-22 00:05:14.000000 whacc-1.3.8/whacc/retrain_LGBM.py
--rw-r--r--   0 phil       (501) staff       (20)    20059 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/run_in_terminal_template.py
--rw-r--r--   0 phil       (501) staff       (20)     9126 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/subset_h5_generator.py
--rw-r--r--   0 phil       (501) staff       (20)     8912 2022-11-04 20:01:59.000000 whacc-1.3.8/whacc/touch_curation_GUI.py
--rw-r--r--   0 phil       (501) staff       (20)    12699 2022-05-10 20:03:18.000000 whacc-1.3.8/whacc/transfer_learning.py
--rw-r--r--   0 phil       (501) staff       (20)   119266 2022-12-16 21:40:31.000000 whacc-1.3.8/whacc/utils.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:43.883265 whacc-1.3.8/whacc/whacc_data/
--rw-r--r--   0 phil       (501) staff       (20)    10244 2022-12-15 23:36:29.000000 whacc-1.3.8/whacc/whacc_data/.DS_Store
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.8/whacc/whacc_data/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.001437 whacc-1.3.8/whacc/whacc_data/feature_data/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.8/whacc/whacc_data/feature_data/__init__.py
--rw-r--r--   0 phil       (501) staff       (20) 32920909 2022-05-10 20:03:19.000000 whacc-1.3.8/whacc/whacc_data/feature_data/feature_data_dict.pkl
--rw-r--r--   0 phil       (501) staff       (20)   210662 2022-08-10 04:11:52.000000 whacc-1.3.8/whacc/whacc_data/feature_data/start_end_nan_locations.pkl
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.041004 whacc-1.3.8/whacc/whacc_data/final_model/
--rw-r--r--   0 phil       (501) staff       (20)    10244 2022-12-23 01:38:04.000000 whacc-1.3.8/whacc/whacc_data/final_model/.DS_Store
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.044400 whacc-1.3.8/whacc/whacc_data/final_model/final_resnet50V2_HEAD/
--rw-r--r--   0 phil       (501) staff       (20)    51419 2022-09-02 19:26:49.000000 whacc-1.3.8/whacc/whacc_data/final_model/final_resnet50V2_HEAD/final_CNN_model_head.pkl
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.065890 whacc-1.3.8/whacc/whacc_data/final_model/light_GBM_model/
--rw-r--r--   0 phil       (501) staff       (20)     6148 2022-12-15 23:36:34.000000 whacc-1.3.8/whacc/whacc_data/final_model/light_GBM_model/.DS_Store
--rwx------   0 phil       (501) staff       (20)  6882830 2022-10-25 07:26:04.000000 whacc-1.3.8/whacc/whacc_data/final_model/light_GBM_model/FINAL_WHACC_MODEL_016_model.pkl
--rwxr-xr-x   0 phil       (501) staff       (20)     1706 2022-05-10 21:57:51.000000 whacc-1.3.8/whacc/whacc_data/template_img.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-12 22:51:44.140166 whacc-1.3.8/whacc.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)     2344 2023-01-12 22:51:43.000000 whacc-1.3.8/whacc.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     8024 2023-01-12 22:51:43.000000 whacc-1.3.8/whacc.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-01-12 22:51:43.000000 whacc-1.3.8/whacc.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2022-11-06 05:53:08.000000 whacc-1.3.8/whacc.egg-info/not-zip-safe
--rw-r--r--   0 phil       (501) staff       (20)       15 2023-01-12 22:51:43.000000 whacc-1.3.8/whacc.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        6 2023-01-12 22:51:43.000000 whacc-1.3.8/whacc.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.492154 whacc-1.3.9/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-05-10 20:03:18.000000 whacc-1.3.9/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      289 2022-11-05 19:49:52.000000 whacc-1.3.9/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)     2389 2023-01-13 19:25:54.491839 whacc-1.3.9/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1580 2023-01-12 22:54:03.000000 whacc-1.3.9/README.md
+-rw-r--r--   0 phil       (501) staff       (20)      274 2022-05-10 20:03:18.000000 whacc-1.3.9/full_requirements.txt
+-rw-r--r--   0 phil       (501) staff       (20)      801 2022-05-10 20:03:18.000000 whacc-1.3.9/lfs-files.txt
+-rw-r--r--   0 phil       (501) staff       (20)      420 2022-11-16 22:36:32.000000 whacc-1.3.9/requirements.txt
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-01-13 19:25:54.492286 whacc-1.3.9/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     2582 2023-01-13 19:25:41.000000 whacc-1.3.9/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.112167 whacc-1.3.9/whacc/
+-rw-r--r--   0 phil       (501) staff       (20)    14340 2023-01-06 21:33:26.000000 whacc-1.3.9/whacc/.DS_Store
+-rw-r--r--   0 phil       (501) staff       (20)    12288 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/.gitattributes.swp
+-rw-r--r--   0 phil       (501) staff       (20)      341 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.142092 whacc-1.3.9/whacc/__pycache__/
+-rw-r--r--   0 phil       (501) staff       (20)      365 2022-05-10 21:02:15.000000 whacc-1.3.9/whacc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    16027 2022-10-25 23:40:12.000000 whacc-1.3.9/whacc/__pycache__/analysis.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    18536 2022-11-09 19:12:35.000000 whacc-1.3.9/whacc/__pycache__/feature_maker.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    50852 2022-07-14 16:43:58.000000 whacc-1.3.9/whacc/__pycache__/image_tools.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    11135 2022-11-04 05:27:07.000000 whacc-1.3.9/whacc/__pycache__/model_maker.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    20173 2022-11-01 19:56:48.000000 whacc-1.3.9/whacc/__pycache__/pole_tracker.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)     7125 2022-12-21 18:51:26.000000 whacc-1.3.9/whacc/__pycache__/retrain_LGBM.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)     7485 2022-05-10 21:02:15.000000 whacc-1.3.9/whacc/__pycache__/subset_h5_generator.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)     6713 2022-11-04 21:23:44.000000 whacc-1.3.9/whacc/__pycache__/touch_curation_GUI.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)     9716 2022-05-10 21:04:08.000000 whacc-1.3.9/whacc/__pycache__/transfer_learning.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    78359 2023-01-13 19:25:48.000000 whacc-1.3.9/whacc/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    25062 2022-10-25 23:35:45.000000 whacc-1.3.9/whacc/analysis.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.233907 whacc-1.3.9/whacc/examples/
+-rw-r--r--   0 phil       (501) staff       (20)     2931 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/0.5 before batch processing.py
+-rw-r--r--   0 phil       (501) staff       (20)     2519 2022-10-31 23:50:36.000000 whacc-1.3.9/whacc/examples/1_make_h5_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     1202 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/2_predict_touches_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     3137 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/3_make_subset_H5_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     5182 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/4_augment_H5_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     1931 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/5_split_data_for_retrain_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     3133 2022-05-10 21:10:53.000000 whacc-1.3.9/whacc/examples/6_retrain_example.py
+-rw-r--r--   0 phil       (501) staff       (20)      343 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/7.5_convert_h5_to_features.py
+-rw-r--r--   0 phil       (501) staff       (20)     6702 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/7_select_TL_trials.py
+-rw-r--r--   0 phil       (501) staff       (20)     8541 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/8_make_feature_data.py
+-rw-r--r--   0 phil       (501) staff       (20)      900 2023-01-06 21:35:15.000000 whacc-1.3.9/whacc/examples/9_re_train_GBM_EXAMPLE.py
+-rw-r--r--   0 phil       (501) staff       (20)    80894 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/CNN_+lightGBM_V5_Testing_GPU_RAM_limits_V2.py
+-rw-r--r--   0 phil       (501) staff       (20)    31926 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/SCRATCH5.py
+-rw-r--r--   0 phil       (501) staff       (20)     9462 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/TL_10_20_30.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2021-04-02 17:08:45.000000 whacc-1.3.9/whacc/examples/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      608 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/add_pole_times.py
+-rw-r--r--   0 phil       (501) staff       (20)     6516 2022-10-27 22:57:01.000000 whacc-1.3.9/whacc/examples/best_T1V1t2_model.py
+-rw-r--r--   0 phil       (501) staff       (20)     2024 2022-07-20 20:27:10.000000 whacc-1.3.9/whacc/examples/colors.py
+-rw-r--r--   0 phil       (501) staff       (20)    22067 2022-12-16 18:22:47.000000 whacc-1.3.9/whacc/examples/compare_models_for_feature_selection.py
+-rw-r--r--   0 phil       (501) staff       (20)    47144 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/convert_h5_to_feature_h5.py
+-rw-r--r--   0 phil       (501) staff       (20)     2135 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/copy_temp.py
+-rw-r--r--   0 phil       (501) staff       (20)    15933 2022-07-27 22:42:00.000000 whacc-1.3.9/whacc/examples/define_in_range.py
+-rw-r--r--   0 phil       (501) staff       (20)     7938 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/diff_h5_creator.py
+-rw-r--r--   0 phil       (501) staff       (20)     1765 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/error_analysis_example.py
+-rw-r--r--   0 phil       (501) staff       (20)    11718 2022-07-18 16:29:23.000000 whacc-1.3.9/whacc/examples/final_CNN_performance_with_final_mathcing_datasets.py
+-rw-r--r--   0 phil       (501) staff       (20)     2081 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/full_pipeline.py
+-rw-r--r--   0 phil       (501) staff       (20)     4738 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/full_pipeline_no_transfer_learning.py
+-rw-r--r--   0 phil       (501) staff       (20)    64731 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/gists.py
+-rw-r--r--   0 phil       (501) staff       (20)      351 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/gui_example.py
+-rw-r--r--   0 phil       (501) staff       (20)     1039 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/h5_tester.py
+-rw-r--r--   0 phil       (501) staff       (20)    21539 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/heat_map_plotter.py
+-rw-r--r--   0 phil       (501) staff       (20)    19294 2022-07-12 20:31:05.000000 whacc-1.3.9/whacc/examples/heat_mapper_boost_mods.py
+-rw-r--r--   0 phil       (501) staff       (20)    21698 2022-10-12 23:12:01.000000 whacc-1.3.9/whacc/examples/heatmap_maker.py
+-rw-r--r--   0 phil       (501) staff       (20)     8594 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/load_all_predictions_from_all_100_final_models_for_cloud.py
+-rw-r--r--   0 phil       (501) staff       (20)    51448 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/lstm_transfer_learning_lstm_using_subsets_v3.py
+-rw-r--r--   0 phil       (501) staff       (20)      848 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/make_master_training_H5_example.py
+-rw-r--r--   0 phil       (501) staff       (20)    27736 2022-11-14 18:35:39.000000 whacc-1.3.9/whacc/examples/make_new_data_and train.py
+-rw-r--r--   0 phil       (501) staff       (20)    35432 2022-07-29 17:01:48.000000 whacc-1.3.9/whacc/examples/pack_samsons_data.py
+-rw-r--r--   0 phil       (501) staff       (20)     2034 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/re_pole_down.py
+-rw-r--r--   0 phil       (501) staff       (20)    52560 2022-12-21 17:10:15.000000 whacc-1.3.9/whacc/examples/redo_all_data.py
+-rw-r--r--   0 phil       (501) staff       (20)    21737 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/run_all_model.py
+-rw-r--r--   0 phil       (501) staff       (20)    13587 2022-07-26 17:45:35.000000 whacc-1.3.9/whacc/examples/scratch4.py
+-rw-r--r--   0 phil       (501) staff       (20)   177391 2022-08-04 05:25:56.000000 whacc-1.3.9/whacc/examples/scratch8.py
+-rw-r--r--   0 phil       (501) staff       (20)   127311 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/scratch_3.py
+-rw-r--r--   0 phil       (501) staff       (20)    12424 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/subset_to_altered_for_training.py
+-rw-r--r--   0 phil       (501) staff       (20)     4500 2022-10-27 20:23:28.000000 whacc-1.3.9/whacc/examples/temp_TVt1_and_TVt2_model_directories.py
+-rw-r--r--   0 phil       (501) staff       (20)    13881 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/test_training_with_worst_trials.py
+-rw-r--r--   0 phil       (501) staff       (20)    28149 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/testing_LSTM_model_defnitions.py
+-rw-r--r--   0 phil       (501) staff       (20)    16560 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/testing_batch_predicting.py
+-rw-r--r--   0 phil       (501) staff       (20)     5833 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/examples/var_rename_scratch.py
+-rw-r--r--   0 phil       (501) staff       (20)    37211 2022-11-08 21:58:45.000000 whacc-1.3.9/whacc/feature_maker.py
+-rw-r--r--   0 phil       (501) staff       (20)    31109 2022-05-10 21:52:37.000000 whacc-1.3.9/whacc/feature_maker_temp.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.255701 whacc-1.3.9/whacc/figures/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-23 02:21:16.000000 whacc-1.3.9/whacc/figures/CNN_plots.py
+-rw-r--r--   0 phil       (501) staff       (20)     3806 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/FIG_2_border_touches_explained.py
+-rw-r--r--   0 phil       (501) staff       (20)     7974 2022-10-25 17:14:30.000000 whacc-1.3.9/whacc/figures/FIG_2_pie_graph_percentages.py
+-rw-r--r--   0 phil       (501) staff       (20)     4607 2022-10-28 20:21:01.000000 whacc-1.3.9/whacc/figures/FIG_2_pie_graph_percentages_V2.py
+-rw-r--r--   0 phil       (501) staff       (20)     4060 2022-08-03 20:27:24.000000 whacc-1.3.9/whacc/figures/PSTH neuron compare.py
+-rw-r--r--   0 phil       (501) staff       (20)    14690 2022-10-17 17:21:34.000000 whacc-1.3.9/whacc/figures/PSTH_V1.py
+-rw-r--r--   0 phil       (501) staff       (20)    17331 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/SHAP_histograms.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.9/whacc/figures/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.258728 whacc-1.3.9/whacc/figures/__pycache__/
+-rw-r--r--   0 phil       (501) staff       (20)      159 2022-05-13 18:55:43.000000 whacc-1.3.9/whacc/figures/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)     1886 2022-11-16 19:00:17.000000 whacc-1.3.9/whacc/figures/__pycache__/pretty_plots.cpython-38.pyc
+-rw-r--r--   0 phil       (501) staff       (20)    22218 2022-11-18 04:31:35.000000 whacc-1.3.9/whacc/figures/all agree analysis fig V2.py
+-rw-r--r--   0 phil       (501) staff       (20)     6503 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/all agree analysis.py
+-rw-r--r--   0 phil       (501) staff       (20)    16803 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/error_analysis_explained_critical_errors.py
+-rw-r--r--   0 phil       (501) staff       (20)     1873 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/error_type_analysis.py
+-rw-r--r--   0 phil       (501) staff       (20)     3601 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/features_with_video.py
+-rw-r--r--   0 phil       (501) staff       (20)    10434 2022-10-27 20:30:32.000000 whacc-1.3.9/whacc/figures/fig_3_model_compare.py
+-rw-r--r--   0 phil       (501) staff       (20)    18580 2022-10-31 00:33:54.000000 whacc-1.3.9/whacc/figures/fig_3_model_compare_V2.py
+-rw-r--r--   0 phil       (501) staff       (20)     3039 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/get_feature_names.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.259991 whacc-1.3.9/whacc/figures/load/
+-rw-r--r--   0 phil       (501) staff       (20)     1936 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/load/load.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.262837 whacc-1.3.9/whacc/figures/not_using/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-22 13:38:53.000000 whacc-1.3.9/whacc/figures/not_using/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    13634 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/figures/not_using/simulation_simple.py
+-rw-r--r--   0 phil       (501) staff       (20)     3118 2022-12-12 21:51:34.000000 whacc-1.3.9/whacc/figures/pretty_plots.py
+-rw-r--r--   0 phil       (501) staff       (20)        2 2022-07-25 16:53:43.000000 whacc-1.3.9/whacc/figures/top4_critical_errors_.py
+-rw-r--r--   0 phil       (501) staff       (20)    25739 2022-11-17 02:13:24.000000 whacc-1.3.9/whacc/figures/what_features_look_like.py
+-rw-r--r--   0 phil       (501) staff       (20)     3460 2022-11-16 20:01:53.000000 whacc-1.3.9/whacc/figures/whisker_images.py
+-rw-r--r--   0 phil       (501) staff       (20)    88984 2022-07-14 16:42:39.000000 whacc-1.3.9/whacc/image_tools.py
+-rw-r--r--   0 phil       (501) staff       (20)    14284 2022-11-04 05:26:34.000000 whacc-1.3.9/whacc/model_maker.py
+-rw-r--r--   0 phil       (501) staff       (20)    31801 2022-11-01 19:56:21.000000 whacc-1.3.9/whacc/pole_tracker.py
+-rw-r--r--   0 phil       (501) staff       (20)    11487 2022-12-22 00:05:14.000000 whacc-1.3.9/whacc/retrain_LGBM.py
+-rw-r--r--   0 phil       (501) staff       (20)    20059 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/run_in_terminal_template.py
+-rw-r--r--   0 phil       (501) staff       (20)     9126 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/subset_h5_generator.py
+-rw-r--r--   0 phil       (501) staff       (20)     8912 2022-11-04 20:01:59.000000 whacc-1.3.9/whacc/touch_curation_GUI.py
+-rw-r--r--   0 phil       (501) staff       (20)    12699 2022-05-10 20:03:18.000000 whacc-1.3.9/whacc/transfer_learning.py
+-rw-r--r--   0 phil       (501) staff       (20)   120095 2023-01-13 19:23:05.000000 whacc-1.3.9/whacc/utils.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.266553 whacc-1.3.9/whacc/whacc_data/
+-rw-r--r--   0 phil       (501) staff       (20)    10244 2023-01-13 18:57:56.000000 whacc-1.3.9/whacc/whacc_data/.DS_Store
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.9/whacc/whacc_data/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.417532 whacc-1.3.9/whacc/whacc_data/feature_data/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-15 16:49:01.000000 whacc-1.3.9/whacc/whacc_data/feature_data/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20) 32920909 2022-05-10 20:03:19.000000 whacc-1.3.9/whacc/whacc_data/feature_data/feature_data_dict.pkl
+-rw-r--r--   0 phil       (501) staff       (20)   210662 2022-08-10 04:11:52.000000 whacc-1.3.9/whacc/whacc_data/feature_data/start_end_nan_locations.pkl
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.429745 whacc-1.3.9/whacc/whacc_data/final_model/
+-rw-r--r--   0 phil       (501) staff       (20)    10244 2022-12-23 01:38:04.000000 whacc-1.3.9/whacc/whacc_data/final_model/.DS_Store
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.431009 whacc-1.3.9/whacc/whacc_data/final_model/final_resnet50V2_HEAD/
+-rw-r--r--   0 phil       (501) staff       (20)    51419 2022-09-02 19:26:49.000000 whacc-1.3.9/whacc/whacc_data/final_model/final_resnet50V2_HEAD/final_CNN_model_head.pkl
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.435905 whacc-1.3.9/whacc/whacc_data/final_model/light_GBM_model/
+-rw-r--r--   0 phil       (501) staff       (20)     6148 2022-12-15 23:36:34.000000 whacc-1.3.9/whacc/whacc_data/final_model/light_GBM_model/.DS_Store
+-rwx------   0 phil       (501) staff       (20)  6882830 2022-10-25 07:26:04.000000 whacc-1.3.9/whacc/whacc_data/final_model/light_GBM_model/FINAL_WHACC_MODEL_016_model.pkl
+-rwxr-xr-x   0 phil       (501) staff       (20)     1706 2022-05-10 21:57:51.000000 whacc-1.3.9/whacc/whacc_data/template_img.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-13 19:25:54.486027 whacc-1.3.9/whacc.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)     2389 2023-01-13 19:25:53.000000 whacc-1.3.9/whacc.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     8024 2023-01-13 19:25:54.000000 whacc-1.3.9/whacc.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-01-13 19:25:53.000000 whacc-1.3.9/whacc.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2022-11-06 05:53:08.000000 whacc-1.3.9/whacc.egg-info/not-zip-safe
+-rw-r--r--   0 phil       (501) staff       (20)       15 2023-01-13 19:25:53.000000 whacc-1.3.9/whacc.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        6 2023-01-13 19:25:53.000000 whacc-1.3.9/whacc.egg-info/top_level.txt
```

### Comparing `whacc-1.3.8/LICENSE` & `whacc-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/PKG-INFO` & `whacc-1.3.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-Metadata-Version: 2.1
-Name: whacc
-Version: 1.3.8
-Summary: Automatic and customizable pipeline for creating a CNN + light GBM model to predict whiskers contacting objects
-Home-page: https://github.com/hireslab/whacc
-Author: Phillip Maire
-Author-email: phillip.maire@gmail.com
-License: MIT
-Description: ![](./pictures/whacc-logo-v1.png) <br />
-        
-        WhACC is a tool for automated touched image classification. 
-        
-        Many neuroscience labs (e.g. [Hires Lab](https://www.hireslab.org/)) use tasks that involve whisker active touch against thin movable poles to study diverse questions of sensory and motor coding. Since neurons operate at temporal resolutions of milliseconds, determining precise whisker contact periods is essential. Yet, accurately classifying the precise moment of touch is time-consuming and labor intensive. 
-        
-        ## [Walkthrough: Google CoLab](https://colab.research.google.com/drive/1pgdpc0IWkce07Sto6AolQTGoXKCW_mes?authuser=1&pli=1#scrollTo=UAIbs6IlTTfj)  
-        
-        ![](./pictures/trial_animation.gif) <br />
-        *Single example trial lasting 4 seconds. Example video (left) along with whisker traces, decomposed components, and spikes recorded from L5 (right). How do we identify the precise millisecond frame when touch occurs?*
-        
-        
-        ## Flow diagram of WhACC video pre-processing and design implementation
-        ![](./pictures/WhACC figure 1.png) <br />
-        
-        ## Touch frame scoring and variation in human curation
-        ![](./pictures/WhACC figure 2.png) <br />
-        
-        ## Feature engineering and selection
-        ![](./pictures/WhACC figure 3.png) <br />
-        
-        ## Data selection and model performance
-        ![](./pictures/WhACC figure 4.png) <br />
-        
-        ## WhACC shows expert human level performance
-        ![](./pictures/WhACC figure 5.png) <br />
-        
-        
-        ## Code contributors:
-        WhACC code and software was originally developed by Phillip Maire and Jonathan Cheung in the laboratory of [Samuel Andrew Hires](https://www.hireslab.org/). 
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+![](./pictures/whacc-logo-v1.png) <br />
+
+WhACC is a tool for automated touched image classification. 
+
+Many neuroscience labs (e.g. [Hires Lab](https://www.hireslab.org/)) use tasks that involve whisker active touch against thin movable poles to study diverse questions of sensory and motor coding. Since neurons operate at temporal resolutions of milliseconds, determining precise whisker contact periods is essential. Yet, accurately classifying the precise moment of touch is time-consuming and labor intensive. 
+
+## [Walkthrough: Google CoLab](https://colab.research.google.com/drive/1pgdpc0IWkce07Sto6AolQTGoXKCW_mes?authuser=1&pli=1#scrollTo=UAIbs6IlTTfj)  
+
+![](./pictures/trial_animation.gif) <br />
+*Single example trial lasting 4 seconds. Example video (left) along with whisker traces, decomposed components, and spikes recorded from L5 (right). How do we identify the precise millisecond frame when touch occurs?*
+
+
+## Flow diagram of WhACC video pre-processing and design implementation
+
+![](./pictures/WhACC_figure_1.png) <br />
+
+## Touch frame scoring and variation in human curation
+
+![](./pictures/WhACC_figure_2.png) <br />
+
+## Feature engineering and selection
+
+![](./pictures/WhACC_figure_3.png) <br />
+
+## Data selection and model performance
+
+![](./pictures/WhACC_figure_4.png) <br />
+
+## WhACC shows expert human level performance
+
+![](./pictures/WhACC_figure_5.png) <br />
+
+
+## Code contributors:
+WhACC code and software was originally developed by Phillip Maire and Jonathan Cheung in the laboratory of [Samuel Andrew Hires](https://www.hireslab.org/).
```

### Comparing `whacc-1.3.8/README.md` & `whacc-1.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,50 @@
-![](./pictures/whacc-logo-v1.png) <br />
-
-WhACC is a tool for automated touched image classification. 
-
-Many neuroscience labs (e.g. [Hires Lab](https://www.hireslab.org/)) use tasks that involve whisker active touch against thin movable poles to study diverse questions of sensory and motor coding. Since neurons operate at temporal resolutions of milliseconds, determining precise whisker contact periods is essential. Yet, accurately classifying the precise moment of touch is time-consuming and labor intensive. 
-
-## [Walkthrough: Google CoLab](https://colab.research.google.com/drive/1pgdpc0IWkce07Sto6AolQTGoXKCW_mes?authuser=1&pli=1#scrollTo=UAIbs6IlTTfj)  
-
-![](./pictures/trial_animation.gif) <br />
-*Single example trial lasting 4 seconds. Example video (left) along with whisker traces, decomposed components, and spikes recorded from L5 (right). How do we identify the precise millisecond frame when touch occurs?*
-
-
-## Flow diagram of WhACC video pre-processing and design implementation
-![](./pictures/WhACC figure 1.png) <br />
-
-## Touch frame scoring and variation in human curation
-![](./pictures/WhACC figure 2.png) <br />
-
-## Feature engineering and selection
-![](./pictures/WhACC figure 3.png) <br />
-
-## Data selection and model performance
-![](./pictures/WhACC figure 4.png) <br />
-
-## WhACC shows expert human level performance
-![](./pictures/WhACC figure 5.png) <br />
-
-
-## Code contributors:
-WhACC code and software was originally developed by Phillip Maire and Jonathan Cheung in the laboratory of [Samuel Andrew Hires](https://www.hireslab.org/). 
+Metadata-Version: 2.1
+Name: whacc
+Version: 1.3.9
+Summary: Automatic and customizable pipeline for creating a CNN + light GBM model to predict whiskers contacting objects
+Home-page: https://github.com/hireslab/whacc
+Author: Phillip Maire
+Author-email: phillip.maire@gmail.com
+License: MIT
+Description: ![](./pictures/whacc-logo-v1.png) <br />
+        
+        WhACC is a tool for automated touched image classification. 
+        
+        Many neuroscience labs (e.g. [Hires Lab](https://www.hireslab.org/)) use tasks that involve whisker active touch against thin movable poles to study diverse questions of sensory and motor coding. Since neurons operate at temporal resolutions of milliseconds, determining precise whisker contact periods is essential. Yet, accurately classifying the precise moment of touch is time-consuming and labor intensive. 
+        
+        ## [Walkthrough: Google CoLab](https://colab.research.google.com/drive/1pgdpc0IWkce07Sto6AolQTGoXKCW_mes?authuser=1&pli=1#scrollTo=UAIbs6IlTTfj)  
+        
+        ![](./pictures/trial_animation.gif) <br />
+        *Single example trial lasting 4 seconds. Example video (left) along with whisker traces, decomposed components, and spikes recorded from L5 (right). How do we identify the precise millisecond frame when touch occurs?*
+        
+        
+        ## Flow diagram of WhACC video pre-processing and design implementation
+        
+        ![](./pictures/WhACC_figure_1.png) <br />
+        
+        ## Touch frame scoring and variation in human curation
+        
+        ![](./pictures/WhACC_figure_2.png) <br />
+        
+        ## Feature engineering and selection
+        
+        ![](./pictures/WhACC_figure_3.png) <br />
+        
+        ## Data selection and model performance
+        
+        ![](./pictures/WhACC_figure_4.png) <br />
+        
+        ## WhACC shows expert human level performance
+        
+        ![](./pictures/WhACC_figure_5.png) <br />
+        
+        
+        ## Code contributors:
+        WhACC code and software was originally developed by Phillip Maire and Jonathan Cheung in the laboratory of [Samuel Andrew Hires](https://www.hireslab.org/). 
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `whacc-1.3.8/lfs-files.txt` & `whacc-1.3.9/lfs-files.txt`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/setup.py` & `whacc-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 remove_list = ['final_model/final_resnet50V2_full_model',
                'whacc_data/training_data',
                'final_model/extra_LGBM_models']
 include_files = list(utils.lister_it(include_files, remove_string=remove_list))
 
 setup(name='whacc',
-      version='1.3.08',
+      version='1.3.09',
       author="Phillip Maire",
       license='MIT',
       description='Automatic and customizable pipeline for creating a CNN + light GBM model to predict whiskers contacting objects',
       packages=find_packages(),
       author_email='phillip.maire@gmail.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

### Comparing `whacc-1.3.8/whacc/.DS_Store` & `whacc-1.3.9/whacc/.DS_Store`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/.gitattributes.swp` & `whacc-1.3.9/whacc/.gitattributes.swp`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/analysis.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/analysis.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/feature_maker.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/feature_maker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/image_tools.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/image_tools.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/model_maker.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/model_maker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/pole_tracker.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/pole_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/retrain_LGBM.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/retrain_LGBM.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/subset_h5_generator.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/subset_h5_generator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/touch_curation_GUI.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/touch_curation_GUI.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/transfer_learning.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/transfer_learning.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/__pycache__/utils.cpython-38.pyc` & `whacc-1.3.9/whacc/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Dec 16 21:40:31 2022 UTC, .py size: 119266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 550d 0d0a 0000 0000 cfe5 9c63 e2d1 0100  U..........c....
+00000000: 550d 0d0a 0000 0000 99af c163 1fd5 0100  U..........c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 f205 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 0206 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c08 5a09 6400 6404 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0b 5a0b 6400 6404 6c0c 5a0c 6400  d.l.Z.d.d.l.Z.d.
 00000080: 6405 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6400  d.l.m.Z.m.Z...d.
 00000090: 6404 6c10 6d11 5a12 0100 6400 6404 6c13  d.l.m.Z...d.d.l.
@@ -16,4843 +16,4883 @@
 000000f0: 6d1f 5a1f 6d20 5a20 0100 6400 6404 6c21  m.Z.m Z ..d.d.l!
 00000100: 5a21 6400 6408 6c22 6d23 5a23 0100 6400  Z!d.d.l"m#Z#..d.
 00000110: 6409 6c24 6d25 5a25 6d24 5a24 0100 6400  d.l$m%Z%m$Z$..d.
 00000120: 6404 6c26 5a26 6400 6404 6c27 5a27 6400  d.l&Z&d.d.l'Z'd.
 00000130: 6404 6c28 5a28 6400 640a 6c29 6d2a 5a2a  d.l(Z(d.d.l)m*Z*
 00000140: 0100 6400 6404 6c2b 5a2c 6400 640b 6c2d  ..d.d.l+Z,d.d.l-
 00000150: 6d2e 5a2e 0100 640c 640d 8400 5a2f 9001  m.Z...d.d...Z/..
-00000160: 6413 640f 6410 8401 5a30 6411 6412 8400  d.d.d...Z0d.d...
+00000160: 6415 640f 6410 8401 5a30 6411 6412 8400  d.d.d...Z0d.d...
 00000170: 5a31 6413 6414 6702 6415 6416 6603 6417  Z1d.d.g.d.d.f.d.
 00000180: 6418 8401 5a32 6419 641a 8400 5a33 9001  d...Z2d.d...Z3..
-00000190: 6414 641c 641d 8401 5a34 641e 641f 8400  d.d.d...Z4d.d...
-000001a0: 5a35 6420 6421 8400 5a36 9001 6415 6422  Z5d d!..Z6..d.d"
-000001b0: 6423 8401 5a37 9001 6416 6424 6425 8401  d#..Z7..d.d$d%..
-000001c0: 5a38 9001 6417 6426 6427 8401 5a39 9001  Z8..d.d&d'..Z9..
-000001d0: 6418 6429 642a 8401 5a3a 9001 6419 642b  d.d)d*..Z:..d.d+
-000001e0: 642c 8401 5a3b 642d 642e 8400 5a3c 642f  d,..Z;d-d...Z<d/
-000001f0: 6430 8400 5a3d 6431 6432 8400 5a3e 9001  d0..Z=d1d2..Z>..
-00000200: 641a 6433 6434 8401 5a3f 6435 6436 8400  d.d3d4..Z?d5d6..
-00000210: 5a40 6437 6438 8400 5a41 6439 643a 8400  Z@d7d8..ZAd9d:..
-00000220: 5a42 9001 641b 643b 643c 8401 5a43 643d  ZB..d.d;d<..ZCd=
-00000230: 643e 8400 5a44 643f 6440 8400 5a45 6441  d>..ZDd?d@..ZEdA
-00000240: 6442 8400 5a46 6443 6444 8400 5a47 6445  dB..ZFdCdD..ZGdE
-00000250: 6446 8400 5a48 9001 641c 6447 6448 8401  dF..ZH..d.dGdH..
-00000260: 5a49 6449 644a 8400 5a4a 9001 641d 644e  ZIdIdJ..ZJ..d.dN
-00000270: 644f 8401 5a4b 9001 641e 6451 6452 8401  dO..ZK..d.dQdR..
-00000280: 5a4c 9001 641f 6453 6454 8401 5a4d 9001  ZL..d.dSdT..ZM..
-00000290: 6420 6456 6457 8401 5a4e 9001 6421 6459  d dVdW..ZN..d!dY
-000002a0: 645a 8401 5a4f 645b 645c 8400 5a50 645d  dZ..ZOd[d\..ZPd]
-000002b0: 645e 8400 5a51 9001 6422 645f 6460 8401  d^..ZQ..d"d_d`..
-000002c0: 5a52 6461 6458 6462 6463 6704 6601 6464  ZRdadXdbdcg.f.dd
-000002d0: 6465 8401 5a53 9001 6423 6467 6468 8401  de..ZS..d#dgdh..
-000002e0: 5a54 6469 646a 8400 5a55 646b 646c 8400  ZTdidj..ZUdkdl..
-000002f0: 5a56 646d 646e 8400 5a57 646f 6470 8400  ZVdmdn..ZWdodp..
-00000300: 5a58 9001 6424 6473 6474 8401 5a59 6475  ZX..d$dsdt..ZYdu
-00000310: 6476 8400 5a5a 9001 6425 6478 6479 8401  dv..ZZ..d%dxdy..
-00000320: 5a5b 9001 6426 647a 647b 8401 5a5c 9001  Z[..d&dzd{..Z\..
-00000330: 6427 647c 647d 8401 5a5d 9001 6428 647e  d'd|d}..Z]..d(d~
-00000340: 647f 8401 5a5e 9001 6429 6480 6481 8401  d...Z^..d)d.d...
-00000350: 5a5f 6482 6483 8400 5a60 6484 6485 8400  Z_d.d...Z`d.d...
-00000360: 5a61 6486 6487 8400 5a62 6488 6489 8400  Zad.d...Zbd.d...
-00000370: 5a63 648a 648b 8400 5a64 648c 648d 8400  Zcd.d...Zdd.d...
-00000380: 5a65 9001 642a 648f 6490 8401 5a66 6491  Ze..d*d.d...Zfd.
-00000390: 6492 8400 5a67 6493 6494 8400 5a68 9001  d...Zgd.d...Zh..
-000003a0: 642b 6495 6496 8401 5a69 9001 642c 6497  d+d.d...Zi..d,d.
-000003b0: 6498 8401 5a6a 9001 642d 656b 6499 9c01  d...Zj..d-ekd...
-000003c0: 649a 649b 8405 5a6c 649c 649d 8400 5a6d  d.d...Zld.d...Zm
-000003d0: 9001 642e 649f 64a0 8401 5a6e 9001 642f  ..d.d.d...Zn..d/
-000003e0: 64a1 64a2 8401 5a6f 9001 6430 64a3 64a4  d.d...Zo..d0d.d.
-000003f0: 8401 5a70 9001 6431 64a5 64a6 8401 5a71  ..Zp..d1d.d...Zq
-00000400: 9001 6432 64a7 64a8 8401 5a72 64a9 64aa  ..d2d.d...Zrd.d.
-00000410: 8400 5a73 64ab 64ac 8400 5a74 64ad 64ae  ..Zsd.d...Ztd.d.
-00000420: 8400 5a75 64af 64b0 8400 5a76 64b1 64ae  ..Zud.d...Zvd.d.
-00000430: 8400 5a75 9001 6433 64b2 64b3 8401 5a77  ..Zu..d3d.d...Zw
-00000440: 64b4 64b5 8400 5a78 64b6 64b7 8400 5a79  d.d...Zxd.d...Zy
-00000450: 64b8 64b9 8400 5a7a 9001 6434 64ba 64bb  d.d...Zz..d4d.d.
-00000460: 8401 5a7b 64bc 64bd 8400 5a7c 9001 6435  ..Z{d.d...Z|..d5
-00000470: 64be 64bf 8401 5a7d 9001 6436 64c0 64c1  d.d...Z}..d6d.d.
-00000480: 8401 5a7e 9001 6437 64c3 64c4 8401 5a7f  ..Z~..d7d.d...Z.
-00000490: 64c5 64c6 8400 5a80 9001 6438 64c7 64c8  d.d...Z...d8d.d.
-000004a0: 8401 5a81 9001 6439 64c9 64ca 8401 5a82  ..Z...d9d.d...Z.
-000004b0: 64cb 64cc 8400 5a83 64cd 64ce 8400 5a84  d.d...Z.d.d...Z.
-000004c0: 64cf 64d0 8400 5a85 64d1 64d2 8400 5a86  d.d...Z.d.d...Z.
-000004d0: 64d3 64d4 8400 5a87 64d5 64d6 8400 5a88  d.d...Z.d.d...Z.
-000004e0: 64d7 64d8 8400 5a89 64d9 64da 8400 5a8a  d.d...Z.d.d...Z.
-000004f0: 64db 64dc 8400 5a8b 9001 643a 64de 64df  d.d...Z...d:d.d.
-00000500: 8401 5a8c 64e0 64e1 8400 5a8d 9001 643b  ..Z.d.d...Z...d;
-00000510: 64e2 64e3 8401 5a8e 9001 643c 64e4 64e5  d.d...Z...d<d.d.
-00000520: 8401 5a8f 64e6 64e7 8400 5a90 64e8 64e9  ..Z.d.d...Z.d.d.
-00000530: 8400 5a91 64ea 64eb 8400 5a92 9001 643d  ..Z.d.d...Z...d=
-00000540: 64ec 64ed 8401 5a93 9001 643e 64ef 64f0  d.d...Z...d>d.d.
-00000550: 8401 5a94 6414 6414 6416 6455 6704 6601  ..Z.d.d.d.dUg.f.
-00000560: 64f1 64f2 8401 5a95 64f3 64f4 8400 5a96  d.d...Z.d.d...Z.
-00000570: 64f5 64f6 8400 5a97 64f7 64f8 8400 5a98  d.d...Z.d.d...Z.
-00000580: 9001 643f 64fa 64fb 8401 5a99 9001 6440  ..d?d.d...Z...d@
-00000590: 64fc 64fd 8401 5a9a 64fe 64ff 8400 5a9b  d.d...Z.d.d...Z.
-000005a0: 9001 6441 9001 6400 9001 6401 8401 5a9c  ..dA..d...d...Z.
-000005b0: 9001 6442 9001 6403 9001 6404 8401 5a9d  ..dB..d...d...Z.
-000005c0: 9001 6405 9001 6406 8400 5a9e 9001 6407  ..d...d...Z...d.
-000005d0: 9001 6408 8400 5a9f 9001 6409 9001 640a  ..d...Z...d...d.
-000005e0: 8400 5aa0 9001 6443 9001 640b 9001 640c  ..Z...dC..d...d.
-000005f0: 8401 5aa1 9001 640d 9001 640e 8400 5aa2  ..Z...d...d...Z.
-00000600: 9001 640f 9001 6410 8400 5aa3 9001 6444  ..d...d...Z...dD
-00000610: 9001 6411 9001 6412 8401 5aa4 6404 5300  ..d...d...Z.d.S.
-00000620: 2845 0100 00e9 0000 0000 2902 da18 636f  (E........)...co
-00000630: 6e76 6572 745f 6835 5f74 6f5f 6665 6174  nvert_h5_to_feat
-00000640: 7572 655f 6835 da1c 7374 616e 6461 7264  ure_h5..standard
-00000650: 5f66 6561 7475 7265 5f67 656e 6572 6174  _feature_generat
-00000660: 696f 6e32 2901 da0c 506f 6c65 5472 6163  ion2)...PoleTrac
-00000670: 6b69 6e67 2901 da0b 6d6f 6465 6c5f 6d61  king)...model_ma
-00000680: 6b65 724e 2902 da09 6e61 7473 6f72 7465  kerN)...natsorte
-00000690: 64da 026e 7329 01da 0b69 6d61 6765 5f74  d..ns)...image_t
-000006a0: 6f6f 6c73 2902 da07 6d65 6466 696c 74da  ools)...medfilt.
-000006b0: 096d 6564 6669 6c74 3264 2901 da04 7471  .medfilt2d)...tq
-000006c0: 646d 2902 da09 7469 6d65 6465 6c74 61da  dm)...timedelta.
-000006d0: 0864 6174 6574 696d 6529 01da 0450 6174  .datetime)...Pat
-000006e0: 6829 01da 075a 6970 4669 6c65 6302 0000  h)...ZipFilec...
-000006f0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000700: 0043 0000 0073 2400 0000 7400 6a01 7c00  .C...s$...t.j.|.
-00000710: 6a02 7c01 6401 8d02 0100 7400 6a01 7c00  j.|.d.....t.j.|.
-00000720: 6a03 7c01 6401 8d02 0100 6400 5300 2902  j.|.d.....d.S.).
-00000730: 4e29 01da 067a 6f72 6465 7229 04da 0370  N)...zorder)...p
-00000740: 6c74 da04 7365 7470 da05 6c69 6e65 73da  lt..setp..lines.
-00000750: 0b63 6f6c 6c65 6374 696f 6e73 2902 da02  .collections)...
-00000760: 6178 7210 0000 00a9 0072 1600 0000 fa39  axr......r.....9
-00000770: 2f55 7365 7273 2f70 6869 6c2f 4472 6f70  /Users/phil/Drop
-00000780: 626f 782f 4849 5245 535f 4c41 422f 4769  box/HIRES_LAB/Gi
-00000790: 7448 7562 2f77 6861 6363 2f77 6861 6363  tHub/whacc/whacc
-000007a0: 2f75 7469 6c73 2e70 7972 1000 0000 3900  /utils.pyr....9.
-000007b0: 0000 7304 0000 0000 0110 0172 1000 0000  ..s........r....
-000007c0: e92a 0000 0063 0400 0000 0000 0000 0000  .*...c..........
-000007d0: 0000 0b00 0000 0600 0000 4300 0000 73d4  ..........C...s.
-000007e0: 0000 0074 0083 007d 0467 007d 0574 017c  ...t...}.g.}.t.|
-000007f0: 0083 0144 005d 507d 0674 02a0 037c 06a1  ...D.]P}.t...|..
-00000800: 017d 0674 046a 05a0 067c 03a1 0101 0074  .}.t.j...|.....t
-00000810: 046a 05a0 077c 046a 0864 0119 007c 066a  .j...|.j.d...|.j
-00000820: 0864 0119 00a1 027d 077c 047c 0719 007d  .d.....}.|.|...}
-00000830: 0874 046a 097c 067c 083c 007c 05a0 0a7c  .t.j.|.|.<.|...|
-00000840: 06a1 0101 0071 127e 0674 0b74 017c 0583  .....q.~.t.t.|..
-00000850: 0183 0144 005d 565c 027d 097d 0a74 04a0  ...D.]V\.}.}.t..
-00000860: 0c7c 007c 0919 007c 057c 0919 0067 02a1  .|.|...|.|...g..
-00000870: 017c 007c 093c 0074 04a0 0d7c 017c 0919  .|.|.<.t...|.|..
-00000880: 007c 017c 0919 0067 02a1 017c 017c 093c  .|.|...g...|.|.<
-00000890: 0074 04a0 0d7c 027c 0919 007c 027c 0919  .t...|.|...|.|..
-000008a0: 0067 02a1 017c 027c 093c 0071 727c 007c  .g...|.|.<.qr|.|
-000008b0: 017c 0266 0353 00a9 024e 7201 0000 0029  .|.f.S...Nr....)
-000008c0: 0eda 156c 6f61 645f 6e61 6e5f 626f 7264  ...load_nan_bord
-000008d0: 6572 5f69 6e64 6578 720b 0000 00da 0463  er_indexr......c
-000008e0: 6f70 79da 0864 6565 7063 6f70 79da 026e  opy..deepcopy..n
-000008f0: 70da 0672 616e 646f 6dda 0473 6565 64da  p..random..seed.
-00000900: 0663 686f 6963 65da 0573 6861 7065 da03  .choice..shape..
-00000910: 6e61 6eda 0661 7070 656e 64da 0965 6e75  nan..append..enu
-00000920: 6d65 7261 7465 da06 7673 7461 636b da0b  merate..vstack..
-00000930: 636f 6e63 6174 656e 6174 6529 0bda 0574  concatenate)...t
-00000940: 7674 5f78 da05 7476 745f 79da 0674 7674  vt_x..tvt_y..tvt
-00000950: 5f66 6e5a 0a6e 756d 7079 5f73 6565 645a  _fnZ.numpy_seedZ
-00000960: 156e 616e 5f61 7272 6179 5f62 6f72 6465  .nan_array_borde
-00000970: 725f 696e 6473 5a0b 7476 745f 785f 6e61  r_indsZ.tvt_x_na
-00000980: 6e65 64da 0464 6174 61da 0469 6e64 735a  ned..data..indsZ
-00000990: 1172 6570 6c61 6365 5f77 6974 685f 6e61  .replace_with_na
-000009a0: 6e73 da01 695a 086e 616e 5f64 6174 6172  ns..iZ.nan_datar
-000009b0: 1600 0000 7216 0000 0072 1700 0000 da0b  ....r....r......
-000009c0: 4e41 4e69 6679 5f64 6174 613d 0000 0073  NANify_data=...s
-000009d0: 1e00 0000 0001 0601 0401 0c01 0a01 0c01  ................
-000009e0: 1a01 0801 0a01 0c01 0202 1401 1a01 1a01  ................
-000009f0: 1c01 722d 0000 0063 0200 0000 0000 0000  ..r-...c........
-00000a00: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
-00000a10: 73d0 0000 0074 00a0 017c 00a1 017d 0264  s....t...|...}.d
-00000a20: 017c 017c 021a 0017 007d 0374 00a0 027c  .|.|.....}.t...|
-00000a30: 02a1 017d 0474 0374 047c 0083 0183 0144  ...}.t.t.|.....D
-00000a40: 005d 185c 027d 055c 027d 067d 077c 057c  .].\.}.\.}.}.|.|
-00000a50: 047c 067c 0785 023c 0071 2c74 00a0 0574  .|.|...<.q,t...t
-00000a60: 067c 0483 017c 0314 00a1 017d 047c 0464  .|...|.....}.|.d
-00000a70: 007c 0185 0219 007d 0467 007d 0874 0774  .|.....}.g.}.t.t
-00000a80: 087c 0083 0183 0144 005d 187d 097c 08a0  .|.....D.].}.|..
-00000a90: 0974 00a0 057c 097c 046b 02a1 01a1 0101  .t...|.|.k......
-00000aa0: 0071 7474 00a0 057c 08a1 017d 0867 007d  .qtt...|...}.g.}
-00000ab0: 0a7c 0844 005d 267d 0b74 0a7c 0b64 0283  .|.D.]&}.t.|.d..
-00000ac0: 0264 0219 007d 0c7c 0aa0 0964 0364 0484  .d...}.|...d.d..
-00000ad0: 007c 0c44 0083 01a1 0101 0071 a07c 087c  .|.D.......q.|.|
-00000ae0: 0a66 0253 0029 054e e901 0000 0072 0100  .f.S.).N.....r..
-00000af0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00000b00: 0000 0005 0000 0053 0000 0073 1e00 0000  .......S...s....
-00000b10: 6700 7c00 5d16 7d01 7400 a001 7c01 a101  g.|.].}.t...|...
-00000b20: 7204 7402 7c01 8301 9102 7104 5300 7216  r.t.|.....q.S.r.
-00000b30: 0000 0029 0372 1d00 0000 da03 616c 6cda  ...).r......all.
-00000b40: 036c 656e a902 da02 2e30 da01 6b72 1600  .len.....0..kr..
-00000b50: 0000 7216 0000 0072 1700 0000 da0a 3c6c  ..r....r......<l
-00000b60: 6973 7463 6f6d 703e 6100 0000 7306 0000  istcomp>a...s...
-00000b70: 0006 0002 000a 007a 2171 7569 636b 5f73  .......z!quick_s
-00000b80: 706c 6974 6572 2e3c 6c6f 6361 6c73 3e2e  pliter.<locals>.
-00000b90: 3c6c 6973 7463 6f6d 703e 290b 721d 0000  <listcomp>).r...
-00000ba0: 00da 0373 756d da04 6f6e 6573 7224 0000  ...sum..onesr$..
-00000bb0: 00da 0d6c 6f6f 705f 7365 676d 656e 7473  ...loop_segments
-00000bc0: da07 6173 6172 7261 79da 046c 6973 74da  ..asarray..list.
-00000bd0: 0572 616e 6765 7230 0000 0072 2300 0000  .ranger0...r#...
-00000be0: da12 6772 6f75 705f 636f 6e73 6563 7574  ..group_consecut
-00000bf0: 6976 6573 290d 5a0a 7370 6c69 745f 6e75  ives).Z.split_nu
-00000c00: 6d73 da09 6c65 6e5f 6172 7261 795a 066c  ms..len_arrayZ.l
-00000c10: 5f6e 756d 73da 0563 6f75 6e74 722b 0000  _nums..countr+..
-00000c20: 00da 0269 69da 0269 31da 0269 325a 1062  ...ii..i1..i2Z.b
-00000c30: 6f6f 6c5f 696e 6473 5f61 7272 6179 7372  ool_inds_arraysr
-00000c40: 3300 0000 da0a 6672 616d 655f 6e75 6d73  3.....frame_nums
-00000c50: da01 62da 0262 3272 1600 0000 7216 0000  ..b..b2r....r...
-00000c60: 0072 1700 0000 da0d 7175 6963 6b5f 7370  .r......quick_sp
-00000c70: 6c69 7465 724f 0000 0073 2000 0000 0001  literO...s .....
-00000c80: 0a01 0c02 0a01 1801 0e01 1201 0c02 0401  ................
-00000c90: 1001 1601 0a02 0401 0801 0e01 1602 7244  ..............rD
-00000ca0: 0000 00e9 0700 0000 e903 0000 0054 e902  .............T..
-00000cb0: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00000cc0: 1400 0000 0600 0000 4300 0000 739c 0100  ........C...s...
-00000cd0: 0074 0064 0183 0101 0074 0183 005c 037d  .t.d.....t...\.}
-00000ce0: 057d 067d 0764 0264 0384 007c 0644 0083  .}.}.d.d...|.D..
-00000cf0: 017d 0874 0064 0483 0101 0074 027c 0083  .}.t.d.....t.|..
-00000d00: 0144 005d fc7d 0974 037c 0964 0583 027d  .D.].}.t.|.d...}
-00000d10: 0a74 037c 097c 0183 027d 0b74 047c 0274  .t.|.|...}.t.|.t
-00000d20: 057c 0b83 0183 025c 027d 0c7d 0d74 06a0  .|.....\.}.}.t..
-00000d30: 077c 0b64 066b 02a1 0164 076b 0472 8a74  .|.d.k...d.k.r.t
-00000d40: 007c 0964 0817 0083 0101 0064 0973 8a74  .|.d.......d.s.t
-00000d50: 087c 0964 0817 0083 0182 017c 0c5c 027d  .|.d.......|.\.}
-00000d60: 0e7d 0f74 06a0 097c 0564 0719 007c 0a7c  .}.t...|.d...|.|
-00000d70: 0e19 0066 02a1 017c 0564 073c 0074 06a0  ...f...|.d.<.t..
-00000d80: 0a7c 0664 0719 007c 0b7c 0e19 0066 02a1  .|.d...|.|...f..
-00000d90: 017c 0664 073c 0074 06a0 0a7c 0764 0719  .|.d.<.t...|.d..
-00000da0: 007c 0d64 0719 0066 02a1 017c 0764 073c  .|.d...f...|.d.<
-00000db0: 0074 06a0 097c 0564 0a19 007c 0a7c 0f19  .t...|.d...|.|..
-00000dc0: 0066 02a1 017c 0564 0a3c 0074 06a0 0a7c  .f...|.d.<.t...|
-00000dd0: 0664 0a19 007c 0b7c 0f19 0066 02a1 017c  .d...|.|...f...|
-00000de0: 0664 0a3c 0074 06a0 0a7c 0764 0a19 007c  .d.<.t...|.d...|
-00000df0: 0d64 0a19 0066 02a1 017c 0764 0a3c 0071  .d...f...|.d.<.q
-00000e00: 327c 0390 0172 5074 0064 0b83 0101 0074  2|...rPt.d.....t
-00000e10: 0b7c 057c 067c 0783 035c 037d 057d 067d  .|.|.|...\.}.}.}
-00000e20: 0767 007d 1074 0c7c 0683 0144 005d 325c  .g.}.t.|...D.]2\
-00000e30: 027d 117d 1274 06a0 0d7c 12a1 017c 0414  .}.}.t...|...|..
-00000e40: 007d 1364 0a7c 1364 007c 087c 1119 0085  .}.d.|.d.|.|....
-00000e50: 023c 007c 10a0 0e7c 13a1 0101 0090 0171  .<.|...|.......q
-00000e60: 5c7c 057c 067c 077c 1066 0453 0029 0c4e  \|.|.|.|.f.S.).N
-00000e70: 7a21 6c6f 6164 696e 6720 6f72 6967 696e  z!loading origin
-00000e80: 616c 2074 7261 696e 696e 6720 6461 7461  al training data
-00000e90: 2e2e 2e63 0100 0000 0000 0000 0000 0000  ...c............
-00000ea0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00000eb0: 0067 007c 005d 0c7d 0174 007c 0183 0191  .g.|.].}.t.|....
-00000ec0: 0271 0453 0072 1600 0000 a901 7230 0000  .q.S.r......r0..
-00000ed0: 0072 3100 0000 7216 0000 0072 1600 0000  .r1...r....r....
-00000ee0: 7217 0000 0072 3400 0000 6900 0000 7304  r....r4...i...s.
-00000ef0: 0000 0006 0002 007a 326c 6f61 645f 7472  .......z2load_tr
-00000f00: 6169 6e69 6e67 5f61 6e64 5f63 7572 6174  aining_and_curat
-00000f10: 6564 5f64 6174 612e 3c6c 6f63 616c 733e  ed_data.<locals>
-00000f20: 2e3c 6c69 7374 636f 6d70 3e7a 1c6c 6f61  .<listcomp>z.loa
-00000f30: 6469 6e67 2079 6f75 7220 6375 7261 7465  ding your curate
-00000f40: 6420 6461 7461 2e2e 2eda 1366 696e 616c  d data.....final
-00000f50: 5f66 6561 7475 7265 735f 3231 3035 e9ff  _features_2105..
-00000f60: ffff ff72 0100 0000 7a24 2074 6869 7320  ...r....z$ this 
-00000f70: 6669 6c65 2068 6173 202d 3127 7320 696e  file has -1's in
-00000f80: 2069 7473 206c 6162 656c 732e 2e2e 4672   its labels...Fr
-00000f90: 2e00 0000 7a45 4e41 4e69 6679 696e 6720  ....zENANifying 
-00000fa0: 6461 7461 2074 6869 7320 6973 206d 656d  data this is mem
-00000fb0: 6f72 7920 696e 7465 6e73 6976 6520 616e  ory intensive an
-00000fc0: 6420 6d61 7920 7461 6b65 2075 7020 746f  d may take up to
-00000fd0: 2031 2d32 206d 696e 2e2e 2e29 0fda 0570   1-2 min...)...p
-00000fe0: 7269 6e74 da12 6c6f 6164 5f74 7261 696e  rint..load_train
-00000ff0: 696e 675f 6461 7461 720b 0000 00da 0667  ing_datar......g
-00001000: 6574 6b65 7972 4400 0000 7230 0000 0072  etkeyrD...r0...r
-00001010: 1d00 0000 7235 0000 00da 0e41 7373 6572  ....r5.....Asser
-00001020: 7469 6f6e 4572 726f 7272 2500 0000 7226  tionErrorr%...r&
-00001030: 0000 0072 2d00 0000 7224 0000 00da 096f  ...r-...r$.....o
-00001040: 6e65 735f 6c69 6b65 7223 0000 0029 14da  nes_liker#...)..
-00001050: 0768 355f 6c69 7374 5a0a 6c61 6265 6c73  .h5_listZ.labels
-00001060: 5f6b 6579 5a0f 7472 6169 6e5f 7661 6c5f  _keyZ.train_val_
-00001070: 7370 6c69 745a 0c6e 616e 5f69 6679 5f64  splitZ.nan_ify_d
-00001080: 6174 615a 0f6e 6577 5f64 6174 615f 7765  ataZ.new_data_we
-00001090: 6967 6874 7227 0000 0072 2800 0000 7229  ightr'...r(...r)
-000010a0: 0000 005a 076f 675f 6c65 6e73 da02 6835  ...Z.og_lens..h5
-000010b0: 722a 0000 00da 066c 6162 656c 735a 0962  r*.....labelsZ.b
-000010c0: 6f6f 6c5f 696e 6473 7241 0000 0072 3f00  ool_indsrA...r?.
-000010d0: 0000 7240 0000 005a 0574 7674 5f77 722c  ..r@...Z.tvt_wr,
-000010e0: 0000 0072 3300 0000 da01 7872 1600 0000  ...r3.....xr....
-000010f0: 7216 0000 0072 1700 0000 da1e 6c6f 6164  r....r......load
-00001100: 5f74 7261 696e 696e 675f 616e 645f 6375  _training_and_cu
-00001110: 7261 7465 645f 6461 7461 6600 0000 7336  rated_dataf...s6
-00001120: 0000 0000 0108 010c 010e 0308 010c 010a  ................
-00001130: 010a 0112 0212 010c 0110 0208 011a 011a  ................
-00001140: 011a 021a 011a 011c 0106 0108 0112 0204  ................
-00001150: 0110 010e 0110 010e 0272 5400 0000 6302  .........rT...c.
-00001160: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001170: 0000 0043 0000 0073 3a00 0000 7400 7c00  ...C...s:...t.|.
-00001180: 6401 6402 8d02 7d00 7401 7c00 8301 6403  d.d...}.t.|...d.
-00001190: 6b02 7222 7c00 7c01 1400 7d00 6e14 7401  k.r"|.|...}.n.t.
-000011a0: 7c00 8301 7c01 6b02 7336 7402 6404 8301  |...|.k.s6t.d...
-000011b0: 8201 7c00 5300 2905 4e54 a901 da10 7375  ..|.S.).NT....su
-000011c0: 7070 7265 7373 5f77 6172 6e69 6e67 722e  ppress_warningr.
-000011d0: 0000 007a 5527 5f73 696e 676c 655f 746f  ...zU'_single_to
-000011e0: 5f6c 6973 745f 696e 7075 745f 6368 6563  _list_input_chec
-000011f0: 6b65 7227 206c 656e 6774 6820 6f66 2069  ker' length of i
-00001200: 6e70 7574 206c 6973 7420 616e 6420 7468  nput list and th
-00001210: 6520 7365 7420 7271 7569 726d 656e 7420  e set rquirment 
-00001220: 646f 6e74 206d 6174 6368 2903 da09 6d61  dont match)...ma
-00001230: 6b65 5f6c 6973 7472 3000 0000 724e 0000  ke_listr0...rN..
-00001240: 0029 025a 0369 6e5f 5a08 6c65 6e5f 6c69  .).Z.in_Z.len_li
-00001250: 7374 7216 0000 0072 1600 0000 7217 0000  str....r....r...
-00001260: 00da 1d5f 7369 6e67 6c65 5f74 6f5f 6c69  ..._single_to_li
-00001270: 7374 5f69 6e70 7574 5f63 6865 636b 6572  st_input_checker
-00001280: 8a00 0000 730a 0000 0000 010c 020c 010a  ....s...........
-00001290: 0214 0172 5800 0000 4663 0200 0000 0000  ...rX...Fc......
-000012a0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000012b0: 0000 734e 0000 0074 007c 0064 0183 027d  ..sN...t.|.d...}
-000012c0: 0074 007c 0164 0183 027d 0174 017c 0064  .t.|.d...}.t.|.d
-000012d0: 0219 007c 0164 0219 0083 0201 0074 027c  ...|.d.......t.|
-000012e0: 0064 0319 007c 0164 0319 0083 0201 0074  .d...|.d.......t
-000012f0: 037c 0064 0419 007c 0164 0419 0083 0201  .|.d...|.d......
-00001300: 0064 0053 0029 054e 7246 0000 0072 0100  .d.S.).NrF...r..
-00001310: 0000 722e 0000 0072 4700 0000 2904 7258  ..r....rG...).rX
-00001320: 0000 00da 1564 6f77 6e6c 6f61 645f 7265  .....download_re
-00001330: 736e 6574 5f6d 6f64 656c da16 646f 776e  snet_model..down
-00001340: 6c6f 6164 5f74 7261 696e 696e 675f 6461  load_training_da
-00001350: 7461 da1a 646f 776e 6c6f 6164 5f65 7874  ta..download_ext
-00001360: 7261 5f4c 4742 4d5f 6d6f 6465 6c73 2902  ra_LGBM_models).
-00001370: da09 6f76 6572 7772 6974 655a 0d64 6f77  ..overwriteZ.dow
-00001380: 6e6c 6f61 645f 696e 6473 7216 0000 0072  nload_indsr....r
-00001390: 1600 0000 7217 0000 00da 1764 6f77 6e6c  ....r......downl
-000013a0: 6f61 645f 616c 6c5f 7768 6163 635f 6461  oad_all_whacc_da
-000013b0: 7461 9300 0000 730a 0000 0000 020a 010a  ta....s.........
-000013c0: 0212 0112 0172 5d00 0000 6300 0000 0000  .....r]...c.....
-000013d0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
-000013e0: 0000 0073 6a00 0000 7400 8300 7401 6a02  ...sj...t...t.j.
-000013f0: 1700 6401 1700 7d00 7401 6a03 a004 7c00  ..d...}.t.j...|.
-00001400: a101 732a 7405 6402 8301 0100 7406 8300  ..s*t.d.....t...
-00001410: 0100 7407 7c00 7401 6a02 1700 6403 1700  ..t.|.t.j...d...
-00001420: 8301 7d01 7407 7c00 7401 6a02 1700 6404  ..}.t.|.t.j...d.
-00001430: 1700 8301 7d02 7407 7c00 7401 6a02 1700  ....}.t.|.t.j...
-00001440: 6405 1700 8301 7d03 7c01 7c02 7c03 6603  d.....}.|.|.|.f.
-00001450: 5300 2906 4e7a 192f 7768 6163 635f 6461  S.).Nz./whacc_da
-00001460: 7461 2f74 7261 696e 696e 675f 6461 7461  ta/training_data
-00001470: 7a37 4175 746f 2064 6f77 6e6c 6f61 6469  z7Auto downloadi
-00001480: 6e67 2074 7261 696e 696e 6720 6461 7461  ng training data
-00001490: 2c20 7468 6973 2077 696c 6c20 6f6e 6c79  , this will only
-000014a0: 2072 756e 206f 6e63 657a 0974 7674 5f78   run oncez.tvt_x
-000014b0: 2e70 6b6c 7a09 7476 745f 792e 706b 6c7a  .pklz.tvt_y.pklz
-000014c0: 0a74 7674 5f66 6e2e 706b 6c29 08da 0e67  .tvt_fn.pkl)...g
-000014d0: 6574 5f77 6861 6363 5f70 6174 68da 026f  et_whacc_path..o
-000014e0: 73da 0373 6570 da04 7061 7468 da05 6973  s..sep..path..is
-000014f0: 6469 7272 4b00 0000 725a 0000 00da 086c  dirrK...rZ.....l
-00001500: 6f61 645f 6f62 6a29 04da 0262 6472 2700  oad_obj)...bdr'.
-00001510: 0000 7228 0000 0072 2900 0000 7216 0000  ..r(...r)...r...
-00001520: 0072 1600 0000 7217 0000 0072 4c00 0000  .r....r....rL...
-00001530: 9d00 0000 7310 0000 0000 0110 010c 0108  ....s...........
-00001540: 0106 0212 0112 0112 0272 4c00 0000 6300  .........rL...c.
-00001550: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001560: 0000 0043 0000 0073 2a00 0000 7400 8300  ...C...s*...t...
-00001570: 7d00 6401 6402 6702 7c00 6403 3c00 6404  }.d.d.g.|.d.<.d.
-00001580: 6701 7c00 6405 3c00 6406 6701 7c00 6407  g.|.d.<.d.g.|.d.
-00001590: 3c00 7c00 5300 2908 4e7a 4968 7474 7073  <.|.S.).NzIhttps
-000015a0: 3a2f 2f77 7777 2e64 726f 7062 6f78 2e63  ://www.dropbox.c
-000015b0: 6f6d 2f73 682f 6b6e 7136 6c61 3566 6375  om/sh/knq6la5fcu
-000015c0: 3733 7a6b 352f 4141 4251 754d 6d78 6d34  73zk5/AABQuMmxm4
-000015d0: 6d73 5662 5749 6464 6c39 7831 7633 613f  msVbWIddl9x1v3a?
-000015e0: 646c 3d31 7a4e 6874 7470 733a 2f2f 7777  dl=1zNhttps://ww
-000015f0: 772e 6472 6f70 626f 782e 636f 6d2f 732f  w.dropbox.com/s/
-00001600: 6b30 3339 3874 6368 676b 3230 6c6b 762f  k0398tchgk20lkv/
-00001610: 6669 6e61 6c5f 7265 736e 6574 3530 5632  final_resnet50V2
-00001620: 5f66 756c 6c5f 6d6f 6465 6c2e 7a69 703f  _full_model.zip?
-00001630: 646c 3d31 da0c 7265 736e 6574 5f6d 6f64  dl=1..resnet_mod
-00001640: 656c 7a49 6874 7470 733a 2f2f 7777 772e  elzIhttps://www.
-00001650: 6472 6f70 626f 782e 636f 6d2f 7368 2f30  dropbox.com/sh/0
-00001660: 3775 6176 6c6f 7869 3375 676e 6a79 2f41  7uavloxi3ugnjy/A
-00001670: 4141 4255 346e 7352 6b4a 4a34 5474 6b42  AABU4nsRkJJ4TtkB
-00001680: 4778 6837 7a49 4861 3f64 6c3d 31da 1873  Gxh7zIHa?dl=1..s
-00001690: 706c 6974 5f62 795f 7472 6961 6c5f 3231  plit_by_trial_21
-000016a0: 3035 5f64 6174 617a 4968 7474 7073 3a2f  05_datazIhttps:/
-000016b0: 2f77 7777 2e64 726f 7062 6f78 2e63 6f6d  /www.dropbox.com
-000016c0: 2f73 682f 6c35 7975 7733 7232 6871 6468  /sh/l5yuw3r2hqdh
-000016d0: 7277 302f 4141 4253 7132 4c39 3236 3563  rw0/AABSq2L9265c
-000016e0: 577a 4173 3641 674a 4f53 3956 613f 646c  WzAs6AgJOS9Va?dl
-000016f0: 3d31 da11 6578 7472 615f 4c47 424d 5f6d  =1..extra_LGBM_m
-00001700: 6f64 656c 7329 01da 0464 6963 74a9 01da  odels)...dict...
-00001710: 0164 7216 0000 0072 1600 0000 7217 0000  .dr....r....r...
-00001720: 00da 1264 6f77 6e6c 6f61 645f 6461 7461  ...download_data
-00001730: 5f64 6963 74aa 0000 0073 0e00 0000 0001  _dict....s......
-00001740: 0601 0201 02ff 0802 0a01 0a01 726b 0000  ............rk..
-00001750: 0063 0200 0000 0000 0000 0000 0000 0700  .c..............
-00001760: 0000 0900 0000 4300 0000 73b4 0000 0074  ......C...s....t
-00001770: 0083 007d 0274 0183 0074 026a 0317 0064  ...}.t...t.j...d
-00001780: 0117 007d 037c 0364 0064 0285 0219 007d  ...}.|.d.d.....}
-00001790: 0474 026a 04a0 057c 04a1 0172 4a7c 0072  .t.j...|...rJ|.r
-000017a0: 3e74 06a0 077c 04a1 0101 006e 0c74 0864  >t...|.....n.t.d
-000017b0: 0383 0101 0064 0053 0074 0864 0483 0101  .....d.S.t.d....
-000017c0: 007c 0264 0519 007c 0119 007d 0574 096a  .|.d...|...}.t.j
-000017d0: 0aa0 0b7c 057c 03a1 0201 0074 0c7c 0364  ...|.|.....t.|.d
-000017e0: 0683 028f 1a7d 0674 0864 0783 0101 007c  .....}.t.d.....|
-000017f0: 066a 0d7c 0464 088d 0101 0057 0035 0051  .j.|.d.....W.5.Q
-00001800: 0052 0058 0074 0864 0983 0101 0074 02a0  .R.X.t.d.....t..
-00001810: 0e7c 03a1 0101 0074 0864 0a83 0101 0064  .|.....t.d.....d
-00001820: 0053 0029 0b4e 7a2d 2f77 6861 6363 5f64  .S.).Nz-/whacc_d
-00001830: 6174 612f 6669 6e61 6c5f 6d6f 6465 6c2f  ata/final_model/
-00001840: 6578 7472 615f 4c47 424d 5f6d 6f64 656c  extra_LGBM_model
-00001850: 732e 7a69 70e9 fcff ffff 7a5a 6578 7472  s.zip.....zZextr
-00001860: 615f 4c47 424d 5f6d 6f64 656c 7320 6973  a_LGBM_models is
-00001870: 2061 6c72 6561 6479 2064 6f77 6e6c 6f61   already downloa
-00001880: 6465 642c 2069 6620 796f 7520 7761 6e74  ded, if you want
-00001890: 2074 6f20 6f76 6572 7772 6974 6520 6974   to overwrite it
-000018a0: 2073 6574 206f 7665 7277 7269 7465 2074   set overwrite t
-000018b0: 6f20 5472 7565 7a20 646f 776e 6c6f 6164  o Truez download
-000018c0: 696e 6720 6578 7472 615f 4c47 424d 5f6d  ing extra_LGBM_m
-000018d0: 6f64 656c 732e 2e2e 7267 0000 00da 0172  odels...rg.....r
-000018e0: fa12 756e 7a69 7070 696e 6720 6669 6c65  ..unzipping file
-000018f0: 202e 2e2e a901 7261 0000 00fa 1564 656c   .....ra.....del
-00001900: 6574 696e 6720 7a69 7020 6669 6c65 202e  eting zip file .
-00001910: 2e2e da04 446f 6e65 a90f 726b 0000 0072  ....Done..rk...r
-00001920: 5e00 0000 725f 0000 0072 6000 0000 7261  ^...r_...r`...ra
-00001930: 0000 0072 6200 0000 da06 7368 7574 696c  ...rb.....shutil
-00001940: da06 726d 7472 6565 724b 0000 00da 0675  ..rmtreerK.....u
-00001950: 726c 6c69 62da 0772 6571 7565 7374 da0b  rllib..request..
-00001960: 7572 6c72 6574 7269 6576 6572 0f00 0000  urlretriever....
-00001970: da0a 6578 7472 6163 7461 6c6c da06 7265  ..extractall..re
-00001980: 6d6f 7665 a907 5a0f 6f76 6572 7772 6974  move..Z.overwrit
-00001990: 655f 6d6f 6465 6c5a 086c 696e 6b5f 696e  e_modelZ.link_in
-000019a0: 6472 6a00 0000 da08 6669 6c65 6e61 6d65  drj.....filename
-000019b0: da03 6473 74da 0375 726c 5a06 7a69 704f  ..dst..urlZ.zipO
-000019c0: 626a 7216 0000 0072 1600 0000 7217 0000  bjr....r....r...
-000019d0: 0072 5b00 0000 b300 0000 7322 0000 0000  .r[.......s"....
-000019e0: 0106 0110 010c 010c 0104 010c 0208 0104  ................
-000019f0: 0208 010c 010e 010c 0108 0116 0108 010a  ................
-00001a00: 0172 5b00 0000 6302 0000 0000 0000 0000  .r[...c.........
-00001a10: 0000 0007 0000 0009 0000 0043 0000 0073  ...........C...s
-00001a20: b400 0000 7400 8300 7d02 7401 8300 7402  ....t...}.t...t.
-00001a30: 6a03 1700 6401 1700 7d03 7c03 6400 6402  j...d...}.|.d.d.
-00001a40: 8502 1900 7d04 7402 6a04 a005 7c04 a101  ....}.t.j...|...
-00001a50: 724a 7c00 723e 7406 a007 7c04 a101 0100  rJ|.r>t...|.....
-00001a60: 6e0c 7408 6403 8301 0100 6400 5300 7408  n.t.d.....d.S.t.
-00001a70: 6404 8301 0100 7c02 6405 1900 7c01 1900  d.....|.d...|...
-00001a80: 7d05 7409 6a0a a00b 7c05 7c03 a102 0100  }.t.j...|.|.....
-00001a90: 740c 7c03 6406 8302 8f1a 7d06 7408 6407  t.|.d.....}.t.d.
-00001aa0: 8301 0100 7c06 6a0d 7c04 6408 8d01 0100  ....|.j.|.d.....
-00001ab0: 5700 3500 5100 5200 5800 7408 6409 8301  W.5.Q.R.X.t.d...
-00001ac0: 0100 7402 a00e 7c03 a101 0100 7408 640a  ..t...|.....t.d.
-00001ad0: 8301 0100 6400 5300 290b 4e7a 1d2f 7768  ....d.S.).Nz./wh
-00001ae0: 6163 635f 6461 7461 2f74 7261 696e 696e  acc_data/trainin
-00001af0: 675f 6461 7461 2e7a 6970 726c 0000 007a  g_data.ziprl...z
-00001b00: 5674 7261 696e 696e 6720 6461 7461 2069  Vtraining data i
-00001b10: 7320 616c 7265 6164 7920 646f 776e 6c6f  s already downlo
-00001b20: 6164 6564 2c20 6966 2079 6f75 2077 616e  aded, if you wan
-00001b30: 7420 746f 206f 7665 7277 7269 7465 2069  t to overwrite i
-00001b40: 7420 7365 7420 6f76 6572 7772 6974 6520  t set overwrite 
-00001b50: 746f 2054 7275 657a 2264 6f77 6e6c 6f61  to Truez"downloa
-00001b60: 6469 6e67 2074 7261 696e 696e 6720 6461  ding training da
-00001b70: 7461 2028 3347 4229 2e2e 2e72 6600 0000  ta (3GB)...rf...
-00001b80: 726d 0000 0072 6e00 0000 726f 0000 0072  rm...rn...ro...r
-00001b90: 7000 0000 7271 0000 0072 7200 0000 727a  p...rq...rr...rz
-00001ba0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00001bb0: 0000 725a 0000 00c9 0000 0073 2200 0000  ..rZ.......s"...
-00001bc0: 0001 0601 1001 0c01 0c01 0401 0c02 0801  ................
-00001bd0: 0402 0801 0c01 0e01 0c01 0801 1601 0801  ................
-00001be0: 0a01 725a 0000 0063 0200 0000 0000 0000  ..rZ...c........
-00001bf0: 0000 0000 0700 0000 0900 0000 4300 0000  ............C...
-00001c00: 73b4 0000 0074 0083 007d 0274 0183 0074  s....t...}.t...t
-00001c10: 026a 0317 0064 0117 007d 037c 0364 0064  .j...d...}.|.d.d
-00001c20: 0285 0219 007d 0474 026a 04a0 057c 04a1  .....}.t.j...|..
-00001c30: 0172 4a7c 0072 3e74 06a0 077c 04a1 0101  .rJ|.r>t...|....
-00001c40: 006e 0c74 0864 0383 0101 0064 0053 0074  .n.t.d.....d.S.t
-00001c50: 0864 0483 0101 007c 0264 0519 007c 0119  .d.....|.d...|..
-00001c60: 007d 0574 096a 0aa0 0b7c 057c 03a1 0201  .}.t.j...|.|....
-00001c70: 0074 0c7c 0364 0683 028f 1a7d 0674 0864  .t.|.d.....}.t.d
-00001c80: 0783 0101 007c 066a 0d7c 0464 088d 0101  .....|.j.|.d....
-00001c90: 0057 0035 0051 0052 0058 0074 0864 0983  .W.5.Q.R.X.t.d..
-00001ca0: 0101 0074 02a0 0e7c 03a1 0101 0074 0864  ...t...|.....t.d
-00001cb0: 0a83 0101 0064 0053 0029 0b4e 7a37 2f77  .....d.S.).Nz7/w
-00001cc0: 6861 6363 5f64 6174 612f 6669 6e61 6c5f  hacc_data/final_
-00001cd0: 6d6f 6465 6c2f 6669 6e61 6c5f 7265 736e  model/final_resn
-00001ce0: 6574 3530 5632 5f66 756c 6c5f 6d6f 6465  et50V2_full_mode
-00001cf0: 6c2e 7a69 7072 6c00 0000 7a4e 6d6f 6465  l.ziprl...zNmode
-00001d00: 6c20 6973 2061 6c72 6561 6479 2064 6f77  l is already dow
-00001d10: 6e6c 6f61 6465 642c 2069 6620 796f 7520  nloaded, if you 
-00001d20: 7761 6e74 2074 6f20 6f76 6572 7772 6974  want to overwrit
-00001d30: 6520 6974 2073 6574 206f 7665 7277 7269  e it set overwri
-00001d40: 7465 2074 6f20 5472 7565 7a25 646f 776e  te to Truez%down
-00001d50: 6c6f 6164 696e 6720 6d6f 6465 6c20 7a69  loading model zi
-00001d60: 7020 6669 6c65 2028 3130 306d 6229 2e2e  p file (100mb)..
-00001d70: 2e72 6500 0000 726d 0000 0072 6e00 0000  .re...rm...rn...
-00001d80: 726f 0000 0072 7000 0000 7271 0000 0072  ro...rp...rq...r
-00001d90: 7200 0000 727a 0000 0072 1600 0000 7216  r...rz...r....r.
-00001da0: 0000 0072 1700 0000 7259 0000 00df 0000  ...r....rY......
-00001db0: 0073 2200 0000 0001 0602 1001 0c01 0c01  .s".............
-00001dc0: 0401 0c02 0801 0401 0801 0c01 0e01 0c01  ................
-00001dd0: 0801 1601 0801 0a01 7259 0000 00e9 6400  ........rY....d.
-00001de0: 0000 6304 0000 0000 0000 0000 0000 000e  ..c.............
-00001df0: 0000 0007 0000 0043 0000 0073 1201 0000  .......C...s....
-00001e00: 7400 7c00 6401 8302 7d04 7c03 6400 6b08  t.|.d...}.|.d.k.
-00001e10: 721c 7401 a002 7c04 a101 7d03 7401 a003  r.t...|...}.t...
-00001e20: 7c03 a101 a004 7405 a101 7d03 7400 7c00  |.....t...}.t.|.
-00001e30: 6402 8302 7d05 6403 7d06 7c02 7242 6404  d...}.d.}.|.rBd.
-00001e40: 7d06 7406 7c04 6403 8302 7d07 7401 a007  }.t.|.d...}.t...
-00001e50: 7c07 6404 1900 6400 6405 8502 1900 a101  |.d...d.d.......
-00001e60: 7c07 6404 1900 1700 a004 7408 a101 7d08  |.d.......t...}.
-00001e70: 7401 a003 7c05 a101 7c08 7c06 6602 1900  t...|...|.|.f...
-00001e80: a004 7409 a101 7d09 7401 6a0a 7c09 7c03  ..t...}.t.j.|.|.
-00001e90: 3c00 7401 a00b 7c09 a101 7d0a 7401 a00c  <.t...|...}.t...
-00001ea0: 7c03 a101 72ba 7c0a 6400 7401 a00d 7c03  |...r.|.d.t...|.
-00001eb0: a101 0b00 8502 1900 7d0a 7401 a00e 7401  ........}.t...t.
-00001ec0: a00f 6404 7410 7c0a 8301 6403 1800 7c01  ..d.t.|...d...|.
-00001ed0: a103 a101 a004 7408 a101 7d0b 7c0a 7c0b  ......t...}.|.|.
-00001ee0: 1900 a004 7408 a101 7d0c 7411 7c0c 8301  ....t...}.t.|...
-00001ef0: 7d0d 7410 7c0d 8301 7410 7c0c 8301 6b03  }.t.|...t.|...k.
-00001f00: 9001 720e 7412 a013 6406 a101 0100 7c0d  ..r.t...d.....|.
-00001f10: 5300 2907 4e72 4100 0000 da0d 6c6f 6361  S.).NrA.....loca
-00001f20: 7469 6f6e 735f 785f 7972 2e00 0000 7201  tions_x_yr....r.
-00001f30: 0000 0072 4700 0000 7a68 6c65 7373 2076  ...rG...zhless v
-00001f40: 6961 626c 6520 7472 6961 6c73 2074 6861  iable trials tha
-00001f50: 6e20 7265 7175 6573 7465 642c 2065 7665  n requested, eve
-00001f60: 7279 7468 696e 6720 7769 6c6c 2077 6f72  rything will wor
-00001f70: 6b20 6669 6e65 2062 7574 2074 6865 7265  k fine but there
-00001f80: 2077 696c 6c20 6265 206c 6573 7320 7472   will be less tr
-00001f90: 6961 6c73 2069 6e20 7468 6520 6f75 7470  ials in the outp
-00001fa0: 7574 2914 724d 0000 0072 1d00 0000 da0a  ut).rM...r......
-00001fb0: 7a65 726f 735f 6c69 6b65 7238 0000 00da  zeros_liker8....
-00001fc0: 0661 7374 7970 65da 0462 6f6f 6c72 3700  .astype..boolr7.
-00001fd0: 0000 da04 6d65 616e da03 696e 74da 0566  ....mean..int..f
-00001fe0: 6c6f 6174 7222 0000 00da 0761 7267 736f  loatr".....argso
-00001ff0: 7274 da03 616e 7972 3500 0000 da05 726f  rt..anyr5.....ro
-00002000: 756e 64da 086c 696e 7370 6163 6572 3000  und..linspacer0.
-00002010: 0000 da11 756e 6971 7565 5f6b 6565 705f  ....unique_keep_
-00002020: 6f72 6465 72da 0877 6172 6e69 6e67 73da  order..warnings.
-00002030: 0477 6172 6e29 0e72 5100 0000 5a0a 6e75  .warn).rQ...Z.nu
-00002040: 6d5f 7669 6465 6f73 5a07 6571 7561 6c5f  m_videosZ.equal_
-00002050: 785a 1269 6e64 735f 746f 5f62 6164 5f74  xZ.inds_to_bad_t
-00002060: 7269 616c 7372 4100 0000 727f 0000 005a  rialsrA...r....Z
-00002070: 0678 795f 696e 645a 0366 6e6c da03 6d69  .xy_indZ.fnl..mi
-00002080: 645a 0778 5f70 6f6c 6573 5a0a 6172 675f  dZ.x_polesZ.arg_
-00002090: 7870 6f6c 6573 da03 6964 78da 036f 7574  xpoles..idx..out
-000020a0: 5a05 755f 6f75 7472 1600 0000 7216 0000  Z.u_outr....r...
-000020b0: 0072 1700 0000 da1a 6571 7561 6c5f 6469  .r......equal_di
-000020c0: 7374 616e 6365 5f70 6f6c 655f 7361 6d70  stance_pole_samp
-000020d0: 6c65 f500 0000 732e 0000 0000 010a 0108  le....s.........
-000020e0: 010a 0110 010a 0104 0104 0104 010a 0224  ...............$
-000020f0: 0118 010a 020a 010a 0114 0222 020e 0108  ..........."....
-00002100: 0112 0104 0102 ff04 0272 9000 0000 6309  .........r....c.
-00002110: 0000 0000 0000 0000 0000 0026 0000 000a  ...........&....
-00002120: 0000 0003 0000 0073 1a04 0000 7400 7c03  .......s....t.|.
-00002130: 8301 7d09 7401 6a02 a003 7c00 a101 7401  ..}.t.j...|...t.
-00002140: 6a04 1700 6401 1700 7401 6a02 a005 7c00  j...d...t.j...|.
-00002150: a101 6400 6402 8502 1900 1700 7d0a 7c05  ..d.d.......}.|.
-00002160: 6400 6b08 7246 7401 6a02 a003 7c00 a101  d.k.rFt.j...|...
-00002170: 7d05 7c06 6400 6b08 7268 7c05 7401 6a04  }.|.d.k.rh|.t.j.
-00002180: 1700 6403 1700 7401 6a02 a005 7c00 a101  ..d...t.j...|...
-00002190: 1700 7d06 7401 6a02 a006 7c06 a101 7292  ..}.t.j...|...r.
-000021a0: 7c07 7388 7407 6404 7c06 1700 6405 1700  |.s.t.d.|...d...
-000021b0: 8301 8201 7401 a008 7c06 a101 0100 7409  ....t...|.....t.
-000021c0: 7c05 8301 0100 740a 7c00 6406 6407 8303  |.....t.|.d.d...
-000021d0: 8900 6408 6409 640a 640b 6704 7d0b 8700  ..d.d.d.d.g.}...
-000021e0: 6601 640c 640d 8408 7c0b 4400 8301 7d0c  f.d.d...|.D...}.
-000021f0: 740b a00c 7c0c a101 73d6 7407 640e 8301  t...|...s.t.d...
-00002200: 8201 640f 6701 7d0b 8700 6601 6410 640d  ..d.g.}...f.d.d.
-00002210: 8408 7c0b 4400 8301 7d0d 8801 6400 6b08  ..|.D...}...d.k.
-00002220: 9001 7210 640f 8800 6b07 9001 7210 6411  ..r.d...k...r.d.
-00002230: 9001 7310 7407 6412 8301 8201 740b a00d  ..s.t.d.....t...
-00002240: 7c02 7c01 1800 6701 7c09 1400 a101 7d0e  |.|...g.|.....}.
-00002250: 7c08 6400 6b08 9001 7238 740e a00f a100  |.d.k...r8t.....
-00002260: 7d0f 6e08 7410 7c08 8301 7d0f 6700 7d10  }.n.t.|...}.g.}.
-00002270: 6700 7d11 6700 7d12 6413 7d13 7c13 7c02  g.}.g.}.d.}.|.|.
-00002280: 7c01 1800 6b04 9001 7278 7c02 7c01 1800  |...k...rx|.|...
-00002290: 7d13 7411 a012 6414 7413 7c13 8301 1700  }.t...d.t.|.....
-000022a0: a101 0100 740b a00d 7414 7415 7c00 640a  ....t...t.t.|.d.
-000022b0: 8302 6415 8302 a101 6400 6400 8502 7c03  ..d.....d.d...|.
-000022c0: 6602 1900 7d14 7416 a017 7c00 6416 a102  f...}.t...|.d...
-000022d0: 8f9c 7d15 7418 7419 7c14 6407 1900 7c14  ..}.t.t.|.d...|.
-000022e0: 6406 1900 8302 8301 4400 5d7e 5c02 7d16  d.......D.]~\.}.
-000022f0: 5c02 7d17 7d18 640f 8800 6b06 9001 72f2  \.}.}.d...k...r.
-00002300: 7c10 a01a 7c15 640f 1900 7c17 7c18 8502  |...|.d...|.|...
-00002310: 1900 7c01 7c02 8502 1900 a101 0100 7c15  ..|.|.........|.
-00002320: 640b 1900 7c17 7c18 8502 1900 7c01 7c02  d...|.|.....|.|.
-00002330: 8502 1900 7d19 7c11 a01a 7c19 a101 0100  ....}.|...|.....
-00002340: 741b 7c0f a01c 7c19 a101 7c13 8302 7d1a  t.|...|...|...}.
-00002350: 7c1a 6417 6b04 6406 1400 7d1a 7c12 a01a  |.d.k.d...}.|...
-00002360: 7c1a a101 0100 9001 71be 5700 3500 5100  |.......q.W.5.Q.
-00002370: 5200 5800 640f 8800 6b06 9002 725c 740b  R.X.d...k...r\t.
-00002380: a01d 7c10 a101 7d10 740b a01d 7c11 a101  ..|...}.t...|...
-00002390: 7d11 740b a01e 7c12 a101 7d12 7416 a017  }.t...|...}.t...
-000023a0: 7c06 6418 a102 8f3e 7d1b 7c0e 7c1b 640a  |.d....>}.|.|.d.
-000023b0: 3c00 7c12 7c1b 6419 3c00 7415 7c00 6408  <.|.|.d.<.t.|.d.
-000023c0: 8302 7c1b 6408 3c00 640f 8800 6b06 9002  ..|.d.<.d...k...
-000023d0: 72ae 7c10 7c1b 640f 3c00 7c11 7c1b 640b  r.|.|.d.<.|.|.d.
-000023e0: 3c00 5700 3500 5100 5200 5800 640f 8800  <.W.5.Q.R.X.d...
-000023f0: 6b07 9004 7216 740b a00d 741f 7415 7c00  k...r.t...t.t.|.
-00002400: 6409 8302 8301 a101 7c03 1900 7d1c 8701  d.......|...}...
-00002410: 6601 641a 640d 8408 7c1c 4400 8301 7d1c  f.d.d...|.D...}.
-00002420: 740b a020 7c01 641b 1800 7c02 a102 7d1d  t.. |.d...|...}.
-00002430: 7421 8801 7415 7c00 6408 8302 7c1d 6415  t!..t.|.d...|.d.
-00002440: 641c 8d04 7d1e 7401 6a02 a005 7c0a a101  d...}.t.j...|...
-00002450: 7c1e 5f22 7c1c 7c1e 5f23 7c1e a024 a100  |._"|.|._#|..$..
-00002460: 0100 7c1e 6a25 7d1f 7c1f a026 641d 641e  ..|.j%}.|..&d.d.
-00002470: a102 7d20 7427 a028 7c1f 7c20 a102 0100  ..} t'.(|.| ....
-00002480: 740b a029 7c1d a101 7d19 6406 7c19 641b  t..)|...}.d.|.d.
-00002490: 641b 7c02 1700 7c01 1800 8502 3c00 740b  d.|...|.....<.t.
-000024a0: a00d 742a 7c19 8301 7400 7c1c 8301 1400  ..t*|...t.|.....
-000024b0: a101 a02b 742c a101 7d21 7400 7415 7c06  ...+t,..}!t.t.|.
-000024c0: 6419 8302 8301 7d22 7c22 740b a02d 7c21  d.....}"|"t..-|!
-000024d0: a101 6b02 9003 73b4 7407 641f 8301 8201  ..k...s.t.d.....
-000024e0: 740b a02e 7c21 a101 6407 1900 7d23 7416  t...|!..d...}#t.
-000024f0: a017 7c06 6420 a102 8f2e 7d24 7416 a017  ..|.d ....}$t...
-00002500: 7c20 6416 a102 8f16 7d25 7c25 640f 1900  | d.....}%|%d...
-00002510: 7c23 1900 7c24 640f 3c00 5700 3500 5100  |#..|$d.<.W.5.Q.
-00002520: 5200 5800 5700 3500 5100 5200 5800 7401  R.X.W.5.Q.R.X.t.
-00002530: a008 7c1f a101 0100 7401 a008 7c20 a101  ..|.....t...| ..
-00002540: 0100 6400 5300 2921 4e5a 0d54 454d 505f  ..d.S.)!NZ.TEMP_
-00002550: 544c 5f44 4154 415f e9fd ffff ff5a 0854  TL_DATA_.....Z.T
-00002560: 4c5f 4441 5441 5f7a 0546 696c 6520 7a3a  L_DATA_z.File z:
-00002570: 2065 7869 7374 732c 2073 6574 206f 7665   exists, set ove
-00002580: 7277 7269 7465 2074 6f20 5472 7565 206f  rwrite to True o
-00002590: 6620 796f 7520 7761 6e74 2074 6f20 6f76  f you want to ov
-000025a0: 6572 7772 6974 6520 6974 722e 0000 0072  erwrite itr....r
-000025b0: 0100 0000 da0c 7465 6d70 6c61 7465 5f69  ......template_i
-000025c0: 6d67 da0f 6675 6c6c 5f66 696c 655f 6e61  mg..full_file_na
-000025d0: 6d65 7372 4100 0000 7249 0000 0063 0100  mesrA...rI...c..
-000025e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000025f0: 0000 1300 0000 7314 0000 0067 007c 005d  ......s....g.|.]
-00002600: 0c7d 017c 0188 006b 0691 0271 0453 0072  .}.|...k...q.S.r
-00002610: 1600 0000 7216 0000 0072 3100 0000 a901  ....r....r1.....
-00002620: da04 6b65 7973 7216 0000 0072 1700 0000  ..keysr....r....
-00002630: 7234 0000 0023 0100 0073 0400 0000 0600  r4...#...s......
-00002640: 0200 7a2f 6d61 6b65 5f74 7261 6e73 6665  ..z/make_transfe
-00002650: 725f 6c65 6172 6e69 6e67 5f64 6174 612e  r_learning_data.
-00002660: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00002670: 6d70 3e7a 8127 7465 6d70 6c61 7465 5f69  mp>z.'template_i
-00002680: 6d67 272c 2027 6675 6c6c 5f66 696c 655f  mg', 'full_file_
-00002690: 6e61 6d65 7327 2c20 2766 696e 616c 5f66  names', 'final_f
-000026a0: 6561 7475 7265 735f 3231 3035 2720 616e  eatures_2105' an
-000026b0: 6420 2766 7261 6d65 5f6e 756d 7327 206d  d 'frame_nums' m
-000026c0: 7573 7420 6265 2070 7265 7365 6e74 2c20  ust be present, 
-000026d0: 736f 6d65 7468 696e 6720 6973 2077 726f  something is wro
-000026e0: 6e67 2077 6974 6820 7468 6520 4835 2066  ng with the H5 f
-000026f0: 696c 652e 2e2e da06 696d 6167 6573 6301  ile.....imagesc.
-00002700: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00002710: 0000 0013 0000 0073 1400 0000 6700 7c00  .......s....g.|.
-00002720: 5d0c 7d01 7c01 8800 6b06 9102 7104 5300  ].}.|...k...q.S.
-00002730: 7216 0000 0072 1600 0000 7231 0000 0072  r....r....r1...r
-00002740: 9400 0000 7216 0000 0072 1700 0000 7234  ....r....r....r4
-00002750: 0000 0028 0100 0073 0400 0000 0600 0200  ...(...s........
-00002760: 467a 2d27 696d 6167 6573 2720 6b65 7920  Fz-'images' key 
-00002770: 6e6f 7420 7072 6573 656e 7420 706c 6561  not present plea
-00002780: 7365 2073 6574 2027 7669 645f 6469 7227  se set 'vid_dir'
-00002790: e905 0000 007a 746c 656e 6774 6820 6f66  .....ztlength of
-000027a0: 2073 6571 7565 6e74 6961 6c20 6672 616d   sequential fram
-000027b0: 6573 2073 656c 6563 7465 6420 6973 2073  es selected is s
-000027c0: 6d61 6c6c 6572 2074 6861 6e20 7468 6520  maller than the 
-000027d0: 6465 6661 756c 7420 736d 6f6f 7468 696e  default smoothin
-000027e0: 6720 6b65 726e 656c 206f 6620 352c 2073  g kernel of 5, s
-000027f0: 6574 7469 6e67 2073 6d6f 6f74 6869 6e67  etting smoothing
-00002800: 206b 6572 6e65 6c20 746f 2054 726d 0000   kernel to Trm..
-00002810: 00e7 0000 0000 0000 e03f da01 7772 5200  .........?..wrR.
-00002820: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00002830: 0000 0005 0000 0013 0000 0073 1e00 0000  ...........s....
-00002840: 6700 7c00 5d16 7d01 7400 8800 7401 6a02  g.|.].}.t...t.j.
-00002850: 1700 7c01 1700 8301 9102 7104 5300 7216  ..|.......q.S.r.
-00002860: 0000 0029 03da 096e 6f72 6d5f 7061 7468  ...)...norm_path
-00002870: 725f 0000 0072 6000 0000 2902 7232 0000  r_...r`...).r2..
-00002880: 005a 0376 6964 2901 da07 7669 645f 6469  .Z.vid)...vid_di
-00002890: 7272 1600 0000 7217 0000 0072 3400 0000  rr....r....r4...
-000028a0: 5801 0000 7304 0000 0006 0002 0072 4700  X...s........rG.
-000028b0: 0000 2904 da0f 7669 6465 6f5f 6469 7265  ..)...video_dire
-000028c0: 6374 6f72 79da 1674 656d 706c 6174 655f  ctory..template_
-000028d0: 706e 675f 6675 6c6c 5f6e 616d 65da 1173  png_full_name..s
-000028e0: 656c 6563 745f 6672 616d 655f 696e 6473  elect_frame_inds
-000028f0: da1b 736b 6970 5f63 6865 636b 5f69 665f  ..skip_check_if_
-00002900: 4650 535f 6973 5f61 6e5f 696e 74fa 032e  FPS_is_an_int...
-00002910: 6835 fa08 5f33 6c61 672e 6835 7a25 4c65  h5.._3lag.h5z%Le
-00002920: 6e67 7468 206f 6620 6c61 6265 6c73 2061  ngth of labels a
-00002930: 6e64 2069 6e64 7320 646f 6e27 7420 6d61  nd inds don't ma
-00002940: 7463 68fa 0272 2b29 2f72 3000 0000 725f  tch..r+)/r0...r_
-00002950: 0000 0072 6100 0000 da07 6469 726e 616d  ...ra.....dirnam
-00002960: 6572 6000 0000 da08 6261 7365 6e61 6d65  er`.....basename
-00002970: da06 6973 6669 6c65 724e 0000 0072 7900  ..isfilerN...ry.
-00002980: 0000 da09 6d61 6b65 5f70 6174 68da 0d70  ....make_path..p
-00002990: 7269 6e74 5f68 355f 6b65 7973 721d 0000  rint_h5_keysr...
-000029a0: 0072 2f00 0000 7238 0000 0072 0500 0000  .r/...r8...r....
-000029b0: da14 6c6f 6164 5f66 696e 616c 5f6c 6967  ..load_final_lig
-000029c0: 6874 5f47 424d 7263 0000 0072 8b00 0000  ht_GBMrc...r....
-000029d0: 728c 0000 00da 0373 7472 7237 0000 0072  r......strr7...r
-000029e0: 4d00 0000 da04 6835 7079 da04 4669 6c65  M.....h5py..File
-000029f0: 7224 0000 00da 037a 6970 7223 0000 00da  r$.....zipr#....
-00002a00: 0673 6d6f 6f74 68da 0770 7265 6469 6374  .smooth..predict
-00002a10: 7225 0000 0072 2600 0000 da12 6835 5f73  r%...r&.....h5_s
-00002a20: 7472 696e 675f 7377 6974 6368 6572 da06  tring_switcher..
-00002a30: 6172 616e 6765 7204 0000 005a 0e73 6176  aranger....Z.sav
-00002a40: 655f 6261 7365 5f6e 616d 65da 0b76 6964  e_base_name..vid
-00002a50: 656f 5f66 696c 6573 5a12 7472 6163 6b5f  eo_filesZ.track_
-00002a60: 616c 6c5f 616e 645f 7361 7665 da0c 6675  all_and_save..fu
-00002a70: 6c6c 5f68 355f 6e61 6d65 da07 7265 706c  ll_h5_name..repl
-00002a80: 6163 6572 0800 0000 da0f 636f 6e76 6572  acer......conver
-00002a90: 745f 746f 5f33 6c61 6772 8000 0000 7239  t_to_3lagr....r9
-00002aa0: 0000 0072 8100 0000 7282 0000 0072 3500  ...r....r....r5.
-00002ab0: 0000 da05 7768 6572 6529 2672 5100 0000  ....where)&rQ...
-00002ac0: 5a0b 7374 6172 745f 6672 616d 655a 0965  Z.start_frameZ.e
-00002ad0: 6e64 5f66 7261 6d65 5a12 6571 7561 6c5f  nd_frameZ.equal_
-00002ae0: 785f 7472 6961 6c5f 696e 6473 729b 0000  x_trial_indsr...
-00002af0: 00da 0862 6173 655f 6469 725a 1566 696e  ...base_dirZ.fin
-00002b00: 616c 5f74 7269 6d6d 6564 5f68 355f 6e61  al_trimmed_h5_na
-00002b10: 6d65 725c 0000 005a 146d 6f64 656c 5f66  mer\...Z.model_f
-00002b20: 756c 6c5f 6669 6c65 5f6e 616d 655a 166e  ull_file_nameZ.n
-00002b30: 756d 5f74 7269 616c 735f 7065 725f 7365  um_trials_per_se
-00002b40: 7373 696f 6eda 0b6e 6577 5f68 355f 6e61  ssion..new_h5_na
-00002b50: 6d65 5a0a 6368 6563 6b5f 6b65 7973 5a0f  meZ.check_keysZ.
-00002b60: 6368 6563 6b5f 6b65 7973 5f6e 6565 645a  check_keys_needZ
-00002b70: 1363 6865 636b 5f6b 6579 735f 6e6f 5f72  .check_keys_no_r
-00002b80: 6572 756e 5a0e 6e65 775f 6672 616d 655f  erunZ.new_frame_
-00002b90: 6e75 6d73 da03 6d6f 6472 9600 0000 7249  nums..modr....rI
-00002ba0: 0000 005a 0b70 7265 645f 6c61 6265 6c73  ...Z.pred_labels
-00002bb0: 5a09 736d 6f6f 7468 5f62 795a 096c 6f6f  Z.smooth_byZ.loo
-00002bc0: 705f 7365 6773 5a06 685f 7265 6164 722c  p_segsZ.h_readr,
-00002bd0: 0000 00da 026b 31da 026b 3272 5300 0000  .....k1..k2rS...
-00002be0: da01 79da 0168 5a0f 7365 6c65 6374 6564  ..y..hZ.selected
-00002bf0: 5f76 6964 656f 7372 9e00 0000 da02 7074  _videosr......pt
-00002c00: da05 6835 5f69 6eda 0768 355f 336c 6167  ..h5_in..h5_3lag
-00002c10: 722b 0000 00da 014c 5a05 696e 6473 325a  r+.....LZ.inds2Z
-00002c20: 0568 5f64 7374 5a05 685f 7372 6372 1600  .h_dstZ.h_srcr..
-00002c30: 0000 2902 7295 0000 0072 9b00 0000 7217  ..).r....r....r.
-00002c40: 0000 00da 1b6d 616b 655f 7472 616e 7366  .....make_transf
-00002c50: 6572 5f6c 6561 726e 696e 675f 6461 7461  er_learning_data
-00002c60: 1201 0000 73a6 0000 0000 0208 022a 0108  ....s........*..
-00002c70: 010c 0108 011a 010c 0114 010a 0108 020c  ................
-00002c80: 020c 0112 0104 0102 ff06 0102 ff04 0306  ................
-00002c90: 0112 0414 010e 0214 010a 010a 0208 0104  ................
-00002ca0: 0104 0104 0204 010e 0108 0104 0104 0102  ................
-00002cb0: ff04 ff04 0322 020e 0122 010a 011e 0118  ....."..."......
-00002cc0: 010a 0110 010c 0118 010a 010a 010a 010a  ................
-00002cd0: 020e 0108 0108 010e 010a 0108 0112 020a  ................
-00002ce0: 0118 0112 0110 040c 0102 0002 ff06 020e  ................
-00002cf0: 0106 0108 0306 020c 010c 020a 0114 011c  ................
-00002d00: 010e 0118 010e 020e 010e 0124 010a 0172  ...........$...r
-00002d10: c100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00002d20: 0006 0000 0006 0000 0043 0000 0073 8600  .........C...s..
-00002d30: 0000 6700 7d01 7400 7c00 8301 4400 5d74  ..g.}.t.|...D.]t
-00002d40: 7d02 7401 a002 7c02 a101 7d03 7c03 a003  }.t...|...}.|...
-00002d50: a100 6401 6b02 720c 7404 7c03 a005 6402  ..d.k.r.t.|...d.
-00002d60: a101 8301 7d04 7c03 a005 6403 a101 7d05  ....}.|...d...}.
-00002d70: 7c05 7404 7c05 8301 6b02 7376 7406 6404  |.t.|...k.svt.d.
-00002d80: 7407 6a08 a009 7c02 a101 1700 6405 1700  t.j...|.....d...
-00002d90: 740a 7c04 8301 1700 8301 0100 7c01 a00b  t.|.........|...
-00002da0: 6401 a101 0100 710c 7c01 a00b 6406 a101  d.....q.|...d...
-00002db0: 0100 710c 7c01 5300 2907 4e54 7245 0000  ..q.|.S.).NTrE..
-00002dc0: 0072 9700 0000 7a09 666f 7220 6669 6c65  .r....z.for file
-00002dd0: 207a 5820 4650 5320 6973 206e 6f74 2061   zX FPS is not a
-00002de0: 6e20 696e 7465 6765 722c 2074 6869 7320  n integer, this 
-00002df0: 7573 7561 6c6c 7920 696e 6469 6361 7465  usually indicate
-00002e00: 7320 6120 7072 6f62 6c65 6d20 7769 7468  s a problem with
-00002e10: 2074 6865 2076 6964 656f 2e20 544f 5441   the video. TOTA
-00002e20: 4c20 4652 414d 4553 203d 2046 290c 720b  L FRAMES = F).r.
-00002e30: 0000 00da 0363 7632 da0c 5669 6465 6f43  .....cv2..VideoC
-00002e40: 6170 7475 7265 da08 6973 4f70 656e 6564  apture..isOpened
-00002e50: 7284 0000 00da 0367 6574 724b 0000 0072  r......getrK...r
-00002e60: 5f00 0000 7261 0000 0072 a400 0000 72a9  _...ra...r....r.
-00002e70: 0000 0072 2300 0000 2906 72b1 0000 005a  ...r#...).r....Z
-00002e80: 0862 6164 5f69 6e64 73da 0a76 6964 656f  .bad_inds..video
-00002e90: 5f66 696c 65da 0576 6964 656f da0d 6672  _file..video..fr
-00002ea0: 616d 655f 6e75 6d62 6572 73da 0366 7073  ame_numbers..fps
-00002eb0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00002ec0: 2c63 6865 636b 5f76 6964 735f 666f 725f  ,check_vids_for_
-00002ed0: 6973 7375 6573 5f62 6173 6564 5f6f 6e5f  issues_based_on_
-00002ee0: 4650 535f 6173 5f61 6e5f 696e 7477 0100  FPS_as_an_intw..
-00002ef0: 0073 1e00 0000 0001 0401 0c01 0a01 0c01  .s..............
-00002f00: 0e01 0a01 0c01 1001 02ff 0202 06fe 0603  ................
-00002f10: 0c04 0c01 72ca 0000 0063 0100 0000 0000  ....r....c......
-00002f20: 0000 0000 0000 0300 0000 0500 0000 0300  ................
-00002f30: 0000 7338 0000 0074 006a 0188 0064 0164  ..s8...t.j...d.d
-00002f40: 028d 0264 0319 007d 0174 00a0 0287 0066  ...d...}.t.....f
-00002f50: 0164 0464 0584 0874 037c 0183 0144 0083  .d.d...t.|...D..
-00002f60: 01a1 01a0 0474 05a1 017d 027c 0253 0029  .....t...}.|.S.)
-00002f70: 064e 5429 01da 0c72 6574 7572 6e5f 696e  .NT)...return_in
-00002f80: 6465 7872 2e00 0000 6301 0000 0000 0000  dexr....c.......
-00002f90: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00002fa0: 0073 1400 0000 6700 7c00 5d0c 7d01 8800  .s....g.|.].}...
-00002fb0: 7c01 1900 9102 7104 5300 7216 0000 0072  |.....q.S.r....r
-00002fc0: 1600 0000 2902 7232 0000 00da 0569 6e64  ....).r2.....ind
-00002fd0: 6578 a901 7253 0000 0072 1600 0000 7217  ex..rS...r....r.
-00002fe0: 0000 0072 3400 0000 9e01 0000 7304 0000  ...r4.......s...
-00002ff0: 0006 0002 007a 2575 6e69 7175 655f 6b65  .....z%unique_ke
-00003000: 6570 5f6f 7264 6572 2e3c 6c6f 6361 6c73  ep_order.<locals
-00003010: 3e2e 3c6c 6973 7463 6f6d 703e 2906 721d  >.<listcomp>).r.
-00003020: 0000 00da 0675 6e69 7175 6572 3800 0000  .....uniquer8...
-00003030: da06 736f 7274 6564 7281 0000 0072 8400  ..sortedr....r..
-00003040: 0000 2903 7253 0000 005a 0769 6e64 6578  ..).rS...Z.index
-00003050: 6573 728f 0000 0072 1600 0000 72cd 0000  esr....r....r...
-00003060: 0072 1700 0000 728a 0000 009c 0100 0073  .r....r........s
-00003070: 0600 0000 0001 1201 2201 728a 0000 0063  ........".r....c
-00003080: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003090: 0500 0000 0300 0000 7326 0000 0064 01a0  ........s&...d..
-000030a0: 0088 00a0 0164 02a1 01a1 0189 0074 0287  .....d.......t..
-000030b0: 0066 0164 0364 0484 0864 0544 0083 0183  .f.d.d...d.D....
-000030c0: 0153 0029 064e da00 fa01 2363 0100 0000  .S.).N....#c....
-000030d0: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-000030e0: 3300 0000 7324 0000 007c 005d 1c7d 0174  3...s$...|.].}.t
-000030f0: 0088 007c 017c 0164 0017 0085 0219 0064  ...|.|.d.......d
-00003100: 0183 0256 0001 0071 0264 0253 0029 0372  ...V...q.d.S.).r
-00003110: 4700 0000 e910 0000 004e 2901 7284 0000  G........N).r...
-00003120: 0029 0272 3200 0000 722c 0000 00a9 0172  .).r2...r,.....r
-00003130: bc00 0000 7216 0000 0072 1700 0000 da09  ....r....r......
-00003140: 3c67 656e 6578 7072 3ea4 0100 0073 0400  <genexpr>....s..
-00003150: 0000 0400 0200 7a1d 6865 785f 746f 5f72  ......z.hex_to_r
-00003160: 6762 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  gb.<locals>.<gen
-00003170: 6578 7072 3e29 0372 0100 0000 7247 0000  expr>).r....rG..
-00003180: 00e9 0400 0000 2903 da04 6a6f 696e da05  ......)...join..
-00003190: 7370 6c69 7472 3900 0000 72d3 0000 0072  splitr9...r....r
-000031a0: 1600 0000 72d3 0000 0072 1700 0000 da0a  ....r....r......
-000031b0: 6865 785f 746f 5f72 6762 a201 0000 7304  hex_to_rgb....s.
-000031c0: 0000 0000 0110 0172 d800 0000 6303 0000  .......r....c...
-000031d0: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-000031e0: 0043 0000 0073 a600 0000 7400 7c00 8301  .C...s....t.|...
-000031f0: 7400 7401 7c00 8301 8301 6b02 731c 7402  t.t.|.....k.s.t.
-00003200: 6401 8301 8201 7400 7c01 8301 7400 7401  d.....t.|...t.t.
-00003210: 7c01 8301 8301 6b02 7338 7402 6402 8301  |.....k.s8t.d...
-00003220: 8201 7c02 6403 6b08 7244 7c00 7d02 6700  ..|.d.k.rD|.}.g.
-00003230: 7d03 7c01 4400 5d4a 7d04 7c04 7c00 6b06  }.|.D.]J}.|.|.k.
-00003240: 728a 7403 a004 7c04 a101 738a 7c04 7c00  r.t...|...s.|.|.
-00003250: 6b02 7d05 7c03 a005 7403 a006 7c05 a101  k.}.|...t...|...
-00003260: 6404 1900 6404 1900 a007 7408 a101 a101  d...d.....t.....
-00003270: 0100 714c 7c03 a005 7403 6a09 a101 0100  ..qL|...t.j.....
-00003280: 714c 740a 7c02 7c03 8302 7d06 7c06 5300  qLt.|.|...}.|.S.
-00003290: 2905 6195 0500 000a 0a20 2020 2050 6172  ).a......    Par
-000032a0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-000032b0: 2d2d 2d2d 2d2d 0a20 2020 2073 7263 5f64  ------.    src_d
-000032c0: 6174 615f 696e 6473 203a 2020 636f 6d65  ata_inds :  come
-000032d0: 2066 726f 6d20 7468 6520 6461 7461 2079   from the data y
-000032e0: 6f75 2077 616e 7420 746f 2075 7365 3b20  ou want to use; 
-000032f0: 696e 6473 2c20 7472 6961 6c20 6e75 6d73  inds, trial nums
-00003300: 206f 7220 6672 616d 6520 6e75 6d73 2c20   or frame nums, 
-00003310: 6f72 2072 6177 2069 6e64 733b 206d 7573  or raw inds; mus
-00003320: 7420 6265 2075 6e69 7175 650a 2020 2020  t be unique.    
-00003330: 6461 7461 5f74 6f5f 6d61 7463 685f 696e  data_to_match_in
-00003340: 6473 203a 2027 7372 635f 6461 7461 5f69  ds : 'src_data_i
-00003350: 6e64 7327 2077 696c 6c20 6265 2066 6f72  nds' will be for
-00003360: 6365 6420 746f 206d 6174 6368 2027 6461  ced to match 'da
-00003370: 7461 5f74 6f5f 6d61 7463 685f 696e 6473  ta_to_match_inds
-00003380: 2720 696e 6465 782c 206c 656e 6774 6820  ' index, length 
-00003390: 616e 6420 6f72 6465 722c 2069 6e64 732c  and order, inds,
-000033a0: 2074 7269 616c 206e 756d 7320 6f72 2066   trial nums or f
-000033b0: 7261 6d65 206e 756d 732c 206f 7220 7261  rame nums, or ra
-000033c0: 7720 696e 6473 3b20 6d75 7374 2062 6520  w inds; must be 
-000033d0: 756e 6971 7565 0a20 2020 2064 6174 6120  unique.    data 
-000033e0: 3a20 6d61 7463 6865 7320 2764 6174 615f  : matches 'data_
-000033f0: 746f 5f6d 6174 6368 5f69 6e64 7327 2062  to_match_inds' b
-00003400: 7574 2069 7320 7468 6520 6163 7461 756c  ut is the actaul
-00003410: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00003420: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 696e    -------.    in
-00003430: 6465 7820 6461 7461 2066 726f 6d20 6461  dex data from da
-00003440: 7461 2061 7272 6179 2027 6461 7461 2720  ta array 'data' 
-00003450: 7468 6174 206d 6174 6368 6573 2074 6865  that matches the
-00003460: 206c 656e 6774 6820 6f66 2027 6461 7461   length of 'data
-00003470: 5f74 6f5f 6d61 7463 685f 696e 6473 270a  _to_match_inds'.
-00003480: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-00003490: 2020 5f5f 5f5f 5f5f 5f5f 0a20 2020 2064    ________.    d
-000034a0: 6174 615f 696e 6473 203d 2020 2020 2020  ata_inds =      
-000034b0: 6e70 2e61 7361 7272 6179 285b 3132 2c20  np.asarray([12, 
-000034c0: 3131 2c20 3133 2c20 3134 2c20 3135 2c20  11, 13, 14, 15, 
-000034d0: 2020 2020 2031 375d 290a 2020 2020 6d61       17]).    ma
-000034e0: 7463 685f 7365 745f 696e 6473 203d 206e  tch_set_inds = n
-000034f0: 702e 6173 6172 7261 7928 5b31 312c 2031  p.asarray([11, 1
-00003500: 322c 2020 2020 2031 342c 2031 352c 2031  2,     14, 15, 1
-00003510: 362c 2020 3137 2c20 2031 382c 2020 3139  6,  17,  18,  19
-00003520: 2c20 2032 305d 290a 2020 2020 6461 7461  ,  20]).    data
-00003530: 203d 206e 702e 6173 6172 7261 7928 5b39   = np.asarray([9
-00003540: 2c38 2c32 2c33 2c34 2c37 2c35 2c36 2c34  ,8,2,3,4,7,5,6,4
-00003550: 2c35 2c36 2c37 2c38 2c39 2c39 322c 312c  ,5,6,7,8,9,92,1,
-00003560: 312c 3536 2c33 332c 3434 2c35 352c 3636  1,56,33,44,55,66
-00003570: 2c37 375d 290a 0a20 2020 206f 7574 203d  ,77])..    out =
-00003580: 2075 7469 6c73 2e69 6e74 6572 7365 6374   utils.intersect
-00003590: 5f64 6174 615f 7769 7468 5f6e 616e 7328  _data_with_nans(
-000035a0: 6461 7461 5f69 6e64 732c 206d 6174 6368  data_inds, match
-000035b0: 5f73 6574 5f69 6e64 732c 2064 6174 613d  _set_inds, data=
-000035c0: 4e6f 6e65 290a 2020 2020 7072 696e 7428  None).    print(
-000035d0: 6e70 2e76 7374 6163 6b28 286f 7574 2c20  np.vstack((out, 
-000035e0: 6d61 7463 685f 7365 745f 696e 6473 2929  match_set_inds))
-000035f0: 290a 0a20 2020 206f 7574 203d 2075 7469  )..    out = uti
-00003600: 6c73 2e69 6e74 6572 7365 6374 5f64 6174  ls.intersect_dat
-00003610: 615f 7769 7468 5f6e 616e 7328 6d61 7463  a_with_nans(matc
-00003620: 685f 7365 745f 696e 6473 2c20 6461 7461  h_set_inds, data
-00003630: 5f69 6e64 732c 2064 6174 613d 4e6f 6e65  _inds, data=None
-00003640: 290a 2020 2020 7072 696e 7428 6e70 2e76  ).    print(np.v
-00003650: 7374 6163 6b28 286f 7574 2c20 6461 7461  stack((out, data
-00003660: 5f69 6e64 7329 2929 0a0a 2020 2020 6461  _inds)))..    da
-00003670: 7461 5f69 6e64 735f 6461 7461 203d 2064  ta_inds_data = d
-00003680: 6174 615b 6461 7461 5f69 6e64 735d 0a20  ata[data_inds]. 
-00003690: 2020 206d 6174 6368 5f73 6574 5f69 6e64     match_set_ind
-000036a0: 735f 6461 7461 203d 2064 6174 615b 6d61  s_data = data[ma
-000036b0: 7463 685f 7365 745f 696e 6473 5d0a 2020  tch_set_inds].  
-000036c0: 2020 6f75 7420 3d20 7574 696c 732e 696e    out = utils.in
-000036d0: 7465 7273 6563 745f 6461 7461 5f77 6974  tersect_data_wit
-000036e0: 685f 6e61 6e73 2864 6174 615f 696e 6473  h_nans(data_inds
-000036f0: 2c20 6d61 7463 685f 7365 745f 696e 6473  , match_set_inds
-00003700: 2c20 6461 7461 3d64 6174 615f 696e 6473  , data=data_inds
-00003710: 5f64 6174 6129 0a20 2020 2070 7269 6e74  _data).    print
-00003720: 286e 702e 7673 7461 636b 2828 6f75 742c  (np.vstack((out,
-00003730: 206d 6174 6368 5f73 6574 5f69 6e64 735f   match_set_inds_
-00003740: 6461 7461 2929 290a 0a20 2020 2064 6174  data)))..    dat
-00003750: 615f 696e 6473 5f64 6174 6120 3d20 6461  a_inds_data = da
-00003760: 7461 5b64 6174 615f 696e 6473 5d0a 2020  ta[data_inds].  
-00003770: 2020 6d61 7463 685f 7365 745f 696e 6473    match_set_inds
-00003780: 5f64 6174 6120 3d20 6461 7461 5b6d 6174  _data = data[mat
-00003790: 6368 5f73 6574 5f69 6e64 735d 0a20 2020  ch_set_inds].   
-000037a0: 206f 7574 203d 2075 7469 6c73 2e69 6e74   out = utils.int
-000037b0: 6572 7365 6374 5f64 6174 615f 7769 7468  ersect_data_with
-000037c0: 5f6e 616e 7328 6d61 7463 685f 7365 745f  _nans(match_set_
-000037d0: 696e 6473 2c20 6461 7461 5f69 6e64 732c  inds, data_inds,
-000037e0: 2064 6174 613d 6d61 7463 685f 7365 745f   data=match_set_
-000037f0: 696e 6473 5f64 6174 6129 0a20 2020 2070  inds_data).    p
-00003800: 7269 6e74 286e 702e 7673 7461 636b 2828  rint(np.vstack((
-00003810: 6f75 742c 2064 6174 615f 696e 6473 5f64  out, data_inds_d
-00003820: 6174 6129 2929 0a0a 2020 2020 7a32 6461  ata)))..    z2da
-00003830: 7461 5f69 6e64 7320 636f 6e74 6169 6e73  ta_inds contains
-00003840: 2064 7570 6c69 6361 7465 732c 2074 6869   duplicates, thi
-00003850: 7320 6973 206e 6f74 2061 6c6c 6f77 6564  s is not allowed
-00003860: 7a37 6d61 7463 685f 7365 745f 696e 6473  z7match_set_inds
-00003870: 2063 6f6e 7461 696e 7320 6475 706c 6963   contains duplic
-00003880: 6174 6573 2c20 7468 6973 2069 7320 6e6f  ates, this is no
-00003890: 7420 616c 6c6f 7765 644e 7201 0000 0029  t allowedNr....)
-000038a0: 0b72 3000 0000 da03 7365 7472 4e00 0000  .r0.....setrN...
-000038b0: 721d 0000 00da 0569 736e 616e 7223 0000  r......isnanr#..
-000038c0: 0072 b500 0000 7281 0000 0072 8500 0000  .r....r....r....
-000038d0: 7222 0000 00da 0f69 6e64 6578 5f77 6974  r".....index_wit
-000038e0: 685f 6e61 6e73 2907 5a0d 7372 635f 6461  h_nans).Z.src_da
-000038f0: 7461 5f69 6e64 735a 1264 6174 615f 746f  ta_indsZ.data_to
-00003900: 5f6d 6174 6368 5f69 6e64 7372 2a00 0000  _match_indsr*...
-00003910: 5a0a 6d61 7463 685f 696e 6473 7233 0000  Z.match_indsr3..
-00003920: 0072 5300 0000 728f 0000 0072 1600 0000  .rS...r....r....
-00003930: 7216 0000 0072 1700 0000 da18 696e 7465  r....r......inte
-00003940: 7273 6563 745f 6461 7461 5f77 6974 685f  rsect_data_with_
-00003950: 6e61 6e73 a701 0000 7320 0000 0000 241c  nans....s ....$.
-00003960: 0108 0106 ff08 0102 ff04 0208 0104 0104  ................
-00003970: 0108 0112 0108 0120 020e 010a 0172 dc00  ....... .....r..
-00003980: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00003990: 0000 0003 0000 0003 0000 0073 1200 0000  ...........s....
-000039a0: 8700 6601 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
-000039b0: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000039c0: 0000 0200 0000 0500 0000 1300 0000 7328  ..............s(
-000039d0: 0000 0067 007c 005d 207d 0174 00a0 017c  ...g.|.] }.t...|
-000039e0: 01a1 0172 1874 006a 026e 0a88 0074 037c  ...r.t.j.n...t.|
-000039f0: 0183 0119 0091 0271 0453 0072 1600 0000  .......q.S.r....
-00003a00: 2904 721d 0000 0072 da00 0000 7222 0000  ).r....r....r"..
-00003a10: 0072 8400 0000 7231 0000 0072 cd00 0000  .r....r1...r....
-00003a20: 7216 0000 0072 1700 0000 7234 0000 00fb  r....r....r4....
-00003a30: 0100 0073 0400 0000 0600 0200 7a23 696e  ...s........z#in
-00003a40: 6465 785f 7769 7468 5f6e 616e 732e 3c6c  dex_with_nans.<l
-00003a50: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00003a60: 3e72 1600 0000 2902 7253 0000 0072 2b00  >r....).rS...r+.
-00003a70: 0000 7216 0000 0072 cd00 0000 7217 0000  ..r....r....r...
-00003a80: 0072 db00 0000 fa01 0000 7302 0000 0000  .r........s.....
-00003a90: 0172 db00 0000 6302 0000 0000 0000 0000  .r....c.........
-00003aa0: 0000 0007 0000 0005 0000 0043 0000 0073  ...........C...s
-00003ab0: 4e00 0000 7400 6a01 7c00 7c01 6401 6402  N...t.j.|.|.d.d.
-00003ac0: 8d03 5c03 7d02 7d03 7d04 7400 a002 7c00  ..\.}.}.}.t...|.
-00003ad0: a101 7400 6a03 1400 7d05 7c03 7c05 7c03  ..t.j...}.|.|.|.
-00003ae0: 3c00 7400 a002 7c01 a101 7400 6a03 1400  <.t...|...t.j...
-00003af0: 7d06 7c04 7c06 7c04 3c00 7c05 7c06 6602  }.|.|.|.<.|.|.f.
-00003b00: 5300 2903 4e54 2901 da0e 7265 7475 726e  S.).NT)...return
-00003b10: 5f69 6e64 6963 6573 2904 721d 0000 00da  _indices).r.....
-00003b20: 0b69 6e74 6572 7365 6374 3164 724f 0000  .intersect1drO..
-00003b30: 0072 2200 0000 2907 da04 6172 7231 da04  .r"...)...arr1..
-00003b40: 6172 7232 da01 6172 4200 0000 da01 6372  arr2..arB.....cr
-00003b50: 4300 0000 da02 6332 7216 0000 0072 1600  C.....c2r....r..
-00003b60: 0000 7217 0000 00da 1369 6e74 6572 7365  ..r......interse
-00003b70: 6374 5f77 6974 685f 6e61 6e73 fe01 0000  ct_with_nans....
-00003b80: 730c 0000 0000 0116 0110 0108 0110 0108  s...............
-00003b90: 0172 e400 0000 6301 0000 0000 0000 0000  .r....c.........
-00003ba0: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
-00003bb0: 6200 0000 7400 a001 7c00 a101 a002 7403  b...t...|.....t.
-00003bc0: a101 7d00 7c00 7400 a004 7c00 a101 3800  ..}.|.t...|...8.
-00003bd0: 7d00 7400 a005 7400 a006 7407 7c00 8301  }.t...t...t.|...
-00003be0: a101 6401 7400 a006 7407 7c00 8301 a101  ..d.t...t.|.....
-00003bf0: 1400 6602 a101 7d01 7400 6a08 7c00 7c01  ..f...}.t.j.|.|.
-00003c00: 6402 6403 8d03 7d02 7400 a009 7c02 a101  d.d...}.t...|...
-00003c10: 7d03 7c03 5300 2904 4e72 4a00 0000 da05  }.|.S.).NrJ.....
-00003c20: 7661 6c69 64a9 01da 046d 6f64 6529 0a72  valid....mode).r
-00003c30: 1d00 0000 7238 0000 0072 8100 0000 7285  ....r8...r....r.
-00003c40: 0000 00da 0761 7665 7261 6765 da06 6873  .....average..hs
-00003c50: 7461 636b 7236 0000 0072 3000 0000 da08  tackr6...r0.....
-00003c60: 636f 6e76 6f6c 7665 da06 6172 676d 6178  convolve..argmax
-00003c70: 2904 7253 0000 00da 0473 7465 705a 0964  ).rS.....stepZ.d
-00003c80: 6172 795f 7374 6570 5a09 7374 6570 5f69  ary_stepZ.step_i
-00003c90: 6e64 7872 1600 0000 7216 0000 0072 1700  ndxr....r....r..
-00003ca0: 0000 da0f 6669 6e64 5f73 7465 705f 6f6e  ....find_step_on
-00003cb0: 7365 7407 0200 0073 0c00 0000 0001 1001  set....s........
-00003cc0: 0e01 2601 1001 0a01 72ed 0000 0063 0200  ..&.....r....c..
-00003cd0: 0000 0000 0000 0000 0000 0700 0000 0a00  ................
-00003ce0: 0000 4300 0000 739e 0000 0074 007c 0064  ..C...s....t.|.d
-00003cf0: 0164 028d 027d 007c 0164 036b 0872 2474  .d...}.|.d.k.r$t
-00003d00: 017c 0064 0419 0083 0101 0064 0353 0074  .|.d.......d.S.t
-00003d10: 027c 0083 0144 005d 6c5c 027d 027d 0374  .|...D.]l\.}.}.t
-00003d20: 03a0 047c 0364 05a1 028f 527d 047a 147c  ...|.d....R}.z.|
-00003d30: 047c 0119 0064 0364 0385 0219 007d 0557  .|...d.d.....}.W
-00003d40: 006e 1401 0001 0001 007c 047c 0119 007d  .n.......|.|...}
-00003d50: 0559 006e 0258 007c 0264 046b 0272 8074  .Y.n.X.|.d.k.r.t
-00003d60: 05a0 067c 05a1 017d 066e 0e74 05a0 077c  ...|...}.n.t...|
-00003d70: 067c 0566 02a1 017d 0657 0035 0051 0052  .|.f...}.W.5.Q.R
-00003d80: 0058 0071 2c7c 0653 0029 067a b60a 2020  .X.q,|.S.).z..  
-00003d90: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00003da0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00003db0: 6835 5f6c 6973 7420 3a20 6c69 7374 0a20  h5_list : list. 
-00003dc0: 2020 2020 2020 206c 6973 7420 6f66 2066         list of f
-00003dd0: 756c 6c20 7061 7468 7320 746f 2048 3520  ull paths to H5 
-00003de0: 6669 6c65 2873 292e 0a20 2020 206b 6579  file(s)..    key
-00003df0: 5f6e 616d 6520 3a20 7374 720a 2020 2020  _name : str.    
-00003e00: 2020 2020 6465 6661 756c 7420 276c 6162      default 'lab
-00003e10: 656c 7327 2c20 7468 6520 6b65 7920 746f  els', the key to
-00003e20: 2067 6574 2074 6865 2064 6174 6120 6672   get the data fr
-00003e30: 6f6d 2074 6865 2048 3520 6669 6c65 0a20  om the H5 file. 
-00003e40: 2020 2054 7255 0000 004e 7201 0000 0072     TrU...Nr....r
-00003e50: 6d00 0000 2908 7257 0000 0072 a700 0000  m...).rW...r....
-00003e60: 7224 0000 0072 aa00 0000 72ab 0000 0072  r$...r....r....r
-00003e70: 1d00 0000 7238 0000 0072 2600 0000 2907  ....r8...r&...).
-00003e80: 7250 0000 005a 086b 6579 5f6e 616d 6572  rP...Z.key_namer
-00003e90: 2c00 0000 7233 0000 0072 bc00 0000 7253  ,...r3...r....rS
-00003ea0: 0000 0072 8f00 0000 7216 0000 0072 1600  ...r....r....r..
-00003eb0: 0000 7217 0000 0072 4d00 0000 1002 0000  ..r....rM.......
-00003ec0: 731c 0000 0000 0a0c 0108 010c 0104 0110  s...............
-00003ed0: 010e 0102 0114 0106 010e 0208 010c 021a  ................
-00003ee0: 0172 4d00 0000 6302 0000 0000 0000 0000  .rM...c.........
-00003ef0: 0000 0011 0000 0007 0000 0043 0000 0073  ...........C...s
-00003f00: 7a01 0000 7400 7401 7c01 6401 8302 8301  z...t.t.|.d.....
-00003f10: 7d02 7402 7c02 8301 7402 7403 a004 7c02  }.t.|...t.t...|.
-00003f20: a101 8301 6b02 732c 7405 6402 8301 8201  ....k.s,t.d.....
-00003f30: 7401 7c01 6403 8302 7d03 7406 7c03 8301  t.|.d...}.t.|...
-00003f40: 7d04 7401 7c01 6404 8302 7d05 7407 7c00  }.t.|.d...}.t.|.
-00003f50: 6405 1900 8301 6701 7407 7c00 6406 1900  d.....g.t.|.d...
-00003f60: 8301 1400 7d06 7c00 6407 1900 6408 1900  ....}.|.d...d...
-00003f70: 7d07 7403 a008 6409 640a 8400 7c00 640b  }.t...d.d...|.d.
-00003f80: 1900 4400 8301 a101 7d08 7403 6a09 7c08  ..D.....}.t.j.|.
-00003f90: 640c 1900 7c08 640d 1900 6702 640e 640f  d...|.d...g.d.d.
-00003fa0: 8d02 7d09 7a1c 740a 7c07 7c04 7403 a00b  ..}.z.t.|.|.t...
-00003fb0: 7402 7c07 8301 a101 6410 8d03 7d0a 5700  t.|.....d...}.W.
-00003fc0: 6e20 0100 0100 0100 740c 6411 8301 0100  n ......t.d.....
-00003fd0: 6412 73d8 7405 6413 8301 8201 5900 6e02  d.s.t.d.....Y.n.
-00003fe0: 5800 6700 7d0b 7403 a008 740d 7c05 6414  X.g.}.t...t.|.d.
-00003ff0: 8302 a101 7d0c 7403 a008 740d 7c06 6414  ....}.t...t.|.d.
-00004000: 8302 a101 7d0d 740e 7c0a 8301 4400 5d60  ....}.t.|...D.]`
-00004010: 5c02 7d0e 7d0f 7403 a00f 7c0f a101 9001  \.}.}.t...|.....
-00004020: 733c 7c09 7c0d 640e 7c0f 6602 1900 7c0d  s<|.|.d.|.f...|.
-00004030: 6414 7c0f 6602 1900 8502 1900 7d10 6e22  d.|.f.......}.n"
-00004040: 7403 a010 7c0c 6414 7c0e 6602 1900 7c0c  t...|.d.|.f...|.
-00004050: 640e 7c0e 6602 1900 1800 a101 6415 1400  d.|.f.......d...
-00004060: 7d10 7c0b a011 7c10 a101 0100 9001 710a  }.|...|.......q.
-00004070: 7403 a012 7c0b a101 7d0b 7c0b 5300 2916  t...|...}.|.S.).
-00004080: 7a76 0a20 2020 2049 2074 6869 6e6b 2074  zv.    I think t
-00004090: 6869 7320 6973 2074 6865 2077 6f72 6b69  his is the worki
-000040a0: 6e67 2076 6572 7369 6f6e 0a20 2020 2050  ng version.    P
-000040b0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000040c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 203a  --------.    c :
-000040d0: 0a20 2020 2068 3520 3a0a 0a20 2020 2052  .    h5 :..    R
-000040e0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-000040f0: 2d2d 0a0a 2020 2020 7293 0000 00fa 7579  --..    r.....uy
-00004100: 6f75 7220 6835 2066 696c 6520 6861 7320  our h5 file has 
-00004110: 6475 706c 6963 6174 6520 7669 6465 6f20  duplicate video 
-00004120: 6669 6c65 7320 7468 6174 2069 7420 7072  files that it pr
-00004130: 6f63 6573 7365 642c 2079 6f75 2077 696c  ocessed, you wil
-00004140: 6c20 6861 7665 2074 6f20 6372 6561 7465  l have to create
-00004150: 2061 206e 6577 2048 3520 6669 6c65 2061   a new H5 file a
-00004160: 6e64 2073 7461 7274 206f 7665 722c 2073  nd start over, s
-00004170: 6f72 7279 da0e 6669 6c65 5f6e 616d 655f  orry..file_name_
-00004180: 6e75 6d73 7241 0000 00da 0174 7233 0000  numsrA.....tr3..
-00004190: 00da 046d 6574 61da 0d75 7365 6454 7269  ...meta..usedTri
-000041a0: 616c 4e75 6d73 6301 0000 0000 0000 0000  alNumsc.........
-000041b0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-000041c0: 1600 0000 6700 7c00 5d0e 7d01 7c01 6a00  ....g.|.].}.|.j.
-000041d0: a001 a100 9102 7104 5300 7216 0000 00a9  ......q.S.r.....
-000041e0: 02da 0154 da07 666c 6174 7465 6ea9 0272  ...T..flatten..r
-000041f0: 3200 0000 da04 746d 7031 7216 0000 0072  2.....tmp1r....r
-00004200: 1600 0000 7217 0000 0072 3400 0000 7402  ....r....r4...t.
-00004210: 0000 7304 0000 0006 0002 007a 3155 6172  ..s........z1Uar
-00004220: 7261 795f 6365 6c6c 5f6c 6162 656c 735f  ray_cell_labels_
-00004230: 746f 5f48 355f 6669 6c65 2e3c 6c6f 6361  to_H5_file.<loca
-00004240: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da05  ls>.<listcomp>..
-00004250: 535f 6374 6be9 0a00 0000 e90d 0000 0072  S_ctk..........r
-00004260: 0100 0000 a901 da04 6178 6973 a901 722a  ........axis..r*
-00004270: 0000 007a 9469 2063 6861 6e67 6564 2061  ...z.i changed a
-00004280: 626f 7665 2063 6f64 6520 7468 6973 2069  bove code this i
-00004290: 7320 6a75 7374 2069 6e20 6361 7365 2069  s just in case i
-000042a0: 7420 6661 696c 732c 2079 6f75 2063 616e  t fails, you can
-000042b0: 2063 6861 6e67 6520 7468 6520 6162 6f76   change the abov
-000042c0: 6520 6c69 6e65 2022 6461 7461 3d6e 702e  e line "data=np.
-000042d0: 6172 616e 6765 286c 656e 2868 5f74 7269  arange(len(h_tri
-000042e0: 616c 7329 2922 2074 6f20 2264 6174 613d  als))" to "data=
-000042f0: 6e70 2e61 7261 6e67 6528 6c65 6e28 775f  np.arange(len(w_
-00004300: 7472 6961 6c73 2929 2246 7a19 7365 6520  trials))"Fz.see 
-00004310: 6162 6f76 6520 7072 696e 7465 6420 6d65  above printed me
-00004320: 7373 6167 6572 2e00 0000 724a 0000 0029  ssager....rJ...)
-00004330: 1372 af00 0000 724d 0000 0072 3000 0000  .r....rM...r0...
-00004340: 721d 0000 0072 ce00 0000 724e 0000 0072  r....r....rN...r
-00004350: 8a00 0000 7284 0000 0072 3800 0000 da06  ....r....r8.....
-00004360: 6e61 6e73 756d 72dc 0000 0072 b000 0000  nansumr....r....
-00004370: 724b 0000 0072 3700 0000 7224 0000 0072  rK...r7...r$...r
-00004380: da00 0000 7236 0000 0072 2300 0000 7226  ....r6...r#...r&
-00004390: 0000 0029 1172 e200 0000 7251 0000 0072  ...).r....rQ...r
-000043a0: 9300 0000 da0f 775f 7472 6961 6c73 5f66  ......w_trials_f
-000043b0: 7261 6d65 73da 0877 5f74 7269 616c 73da  rames..w_trials.
-000043c0: 0c77 5f66 7261 6d65 5f6e 756d 73da 0c68  .w_frame_nums..h
-000043d0: 5f66 7261 6d65 5f6e 756d 73da 0868 5f74  _frame_nums..h_t
-000043e0: 7269 616c 7372 f800 0000 5a08 685f 6c61  rialsr....Z.h_la
-000043f0: 6265 6c73 5a19 696e 645f 6875 6d61 6e5f  belsZ.ind_human_
-00004400: 746f 5f77 6861 6363 5f74 7269 616c 735a  to_whacc_trialsZ
-00004410: 1c6d 6174 6368 696e 675f 6c61 6265 6c73  .matching_labels
-00004420: 5f66 6f72 5f77 6861 6363 5f68 35da 0477  _for_whacc_h5..w
-00004430: 5f66 6eda 0468 5f66 6e72 2c00 0000 7233  _fn..h_fnr,...r3
-00004440: 0000 0072 5300 0000 7216 0000 0072 1600  ...rS...r....r..
-00004450: 0000 7217 0000 00da 1d55 6172 7261 795f  ..r......Uarray_
-00004460: 6365 6c6c 5f6c 6162 656c 735f 746f 5f48  cell_labels_to_H
-00004470: 355f 6669 6c65 5f02 0000 7340 0000 0000  5_file_...s@....
-00004480: 0c0e 010c 0102 ff0a 0102 ff04 020a 0108  ................
-00004490: 010a 021a 010c 0118 011a 0102 010a 0106  ................
-000044a0: ff0c 0206 0102 0102 ff04 0212 0204 0110  ................
-000044b0: 0110 0210 010c 011e 0222 010e 010a 0172  .........".....r
-000044c0: 0601 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000044d0: 0011 0000 0007 0000 0043 0000 0073 4c01  .........C...sL.
-000044e0: 0000 7400 7c02 7401 8302 7214 7402 7c01  ..t.|.t...r.t.|.
-000044f0: 7c02 8302 0100 7403 7402 7c01 6401 8302  |.....t.t.|.d...
-00004500: 8301 7d03 7404 7c03 8301 7404 7405 a006  ..}.t.|...t.t...
-00004510: 7c03 a101 8301 6b02 7340 7407 6402 8301  |.....k.s@t.d...
-00004520: 8201 7402 7c01 6403 8302 7d04 7408 7c04  ..t.|.d...}.t.|.
-00004530: 8301 7d05 7402 7c01 6404 8302 7d06 7409  ..}.t.|.d...}.t.
-00004540: 7c00 6405 1900 8301 6701 7409 7c00 6406  |.d.....g.t.|.d.
-00004550: 1900 8301 1400 7d07 7c00 6407 1900 6408  ......}.|.d...d.
-00004560: 1900 7d08 7405 a00a 6409 640a 8400 7c00  ..}.t...d.d...|.
-00004570: 640b 1900 4400 8301 a101 7d09 740b 7c05  d...D.....}.t.|.
-00004580: 7c08 7405 a00c 7404 7c05 8301 a101 640c  |.t...t.|.....d.
-00004590: 8d03 7d0a 6700 7d0b 7405 a00a 740d 7c06  ..}.g.}.t...t.|.
-000045a0: 640d 8302 a101 7d0c 7405 a00a 740d 7c07  d.....}.t...t.|.
-000045b0: 640d 8302 a101 7d0d 740e 7c0a 8301 4400  d.....}.t.|...D.
-000045c0: 5d5e 5c02 7d0e 7d0f 7405 a00f 7c0f a101  ]^\.}.}.t...|...
-000045d0: 9001 7310 7c02 7c0c 640e 7c0f 6602 1900  ..s.|.|.d.|.f...
-000045e0: 7c0c 640d 7c0f 6602 1900 8502 1900 7d10  |.d.|.f.......}.
-000045f0: 6e22 7405 a010 7c0d 640d 7c0e 6602 1900  n"t...|.d.|.f...
-00004600: 7c0d 640e 7c0e 6602 1900 1800 a101 640f  |.d.|.f.......d.
-00004610: 1400 7d10 7c0b a011 7c10 a101 0100 71de  ..}.|...|.....q.
-00004620: 7405 a012 7c0b a101 7d0b 7c0b 5300 2910  t...|...}.|.S.).
-00004630: 4e72 9300 0000 72ee 0000 0072 ef00 0000  Nr....r....r....
-00004640: 7241 0000 0072 f000 0000 7233 0000 0072  rA...r....r3...r
-00004650: f100 0000 72f2 0000 0063 0100 0000 0000  ....r....c......
-00004660: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00004670: 0000 7316 0000 0067 007c 005d 0e7d 017c  ..s....g.|.].}.|
-00004680: 016a 00a0 01a1 0091 0271 0453 0072 1600  .j.......q.S.r..
-00004690: 0000 72f3 0000 0072 f600 0000 7216 0000  ..r....r....r...
-000046a0: 0072 1600 0000 7217 0000 0072 3400 0000  .r....r....r4...
-000046b0: 9902 0000 7304 0000 0006 0002 007a 2668  ....s........z&h
-000046c0: 355f 746f 5f55 5f61 7272 6179 5f63 656c  5_to_U_array_cel
-000046d0: 6c2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  l.<locals>.<list
-000046e0: 636f 6d70 3e72 f800 0000 72fd 0000 0072  comp>r....r....r
-000046f0: 2e00 0000 7201 0000 0072 4a00 0000 2913  ....r....rJ...).
-00004700: da0a 6973 696e 7374 616e 6365 72a9 0000  ..isinstancer...
-00004710: 0072 4d00 0000 72af 0000 0072 3000 0000  .rM...r....r0...
-00004720: 721d 0000 0072 ce00 0000 724e 0000 0072  r....r....rN...r
-00004730: 8a00 0000 7284 0000 0072 3800 0000 72dc  ....r....r8...r.
-00004740: 0000 0072 b000 0000 7237 0000 0072 2400  ...r....r7...r$.
-00004750: 0000 72da 0000 0072 3600 0000 7223 0000  ..r....r6...r#..
-00004760: 0072 2600 0000 2911 72e2 0000 0072 5100  .r&...).r....rQ.
-00004770: 0000 5a08 775f 6c61 6265 6c73 7293 0000  ..Z.w_labelsr...
-00004780: 0072 ff00 0000 7200 0100 0072 0101 0000  .r....r....r....
-00004790: 7202 0100 0072 0301 0000 72f8 0000 005a  r....r....r....Z
-000047a0: 1969 6e64 5f77 6861 6363 5f74 6f5f 6875  .ind_whacc_to_hu
-000047b0: 6d61 6e5f 7472 6961 6c73 5a18 6d61 7463  man_trialsZ.matc
-000047c0: 6869 6e67 5f6c 6162 656c 735f 666f 725f  hing_labels_for_
-000047d0: 6365 6c6c 7204 0100 0072 0501 0000 722c  cellr....r....r,
-000047e0: 0000 0072 3300 0000 7253 0000 0072 1600  ...r3...rS...r..
-000047f0: 0000 7216 0000 0072 1700 0000 da12 6835  ..r....r......h5
-00004800: 5f74 6f5f 555f 6172 7261 795f 6365 6c6c  _to_U_array_cell
-00004810: 8c02 0000 7332 0000 0000 010a 010a 010e  ....s2..........
-00004820: 010c 0102 ff0a 0102 ff04 030a 0108 010a  ................
-00004830: 021a 010c 0118 0318 0204 0110 0110 0210  ................
-00004840: 010c 011e 0222 010c 010a 0172 0801 0000  .....".....r....
-00004850: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00004860: 0004 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00004870: 7401 7c00 7c01 8302 8301 5300 a901 4e29  t.|.|.....S...N)
-00004880: 0272 3700 0000 da0e 6368 756e 6b5f 7365  .r7.....chunk_se
-00004890: 676d 656e 7473 a902 723c 0000 00da 0a63  gments..r<.....c
-000048a0: 6875 6e6b 5f73 697a 6572 1600 0000 7216  hunk_sizer....r.
-000048b0: 0000 0072 1700 0000 da13 6c6f 6f70 5f73  ...r......loop_s
-000048c0: 6567 6d65 6e74 5f63 6875 6e6b 73e0 0200  egment_chunks...
-000048d0: 0073 0200 0000 0001 720d 0100 0063 0200  .s......r....c..
-000048e0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-000048f0: 0000 4300 0000 732c 0000 007c 0167 017c  ..C...s,...|.g.|
-00004900: 007c 011a 0014 007d 027c 007c 0116 0064  .|.....}.|.|...d
-00004910: 016b 0472 287c 02a0 007c 007c 0116 00a1  .k.r(|...|.|....
-00004920: 0101 007c 0253 0072 1900 0000 2901 7223  ...|.S.r....).r#
-00004930: 0000 0029 0372 3c00 0000 720c 0100 0072  ...).r<...r....r
-00004940: 8f00 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00004950: 0000 0072 0a01 0000 e402 0000 7308 0000  ...r........s...
-00004960: 0000 010e 010c 010e 0172 0a01 0000 6302  .........r....c.
-00004970: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00004980: 0000 0043 0000 0073 1800 0000 7c00 7c01  ...C...s....|.|.
-00004990: 1a00 6401 7c00 7c01 1600 6402 6b04 1400  ..d.|.|...d.k...
-000049a0: 1700 5300 2903 4e72 2e00 0000 7201 0000  ..S.).Nr....r...
-000049b0: 0072 1600 0000 720b 0100 0072 1600 0000  .r....r....r....
-000049c0: 7216 0000 0072 1700 0000 da0a 6e75 6d5f  r....r......num_
-000049d0: 6368 756e 6b73 eb02 0000 7302 0000 0000  chunks....s.....
-000049e0: 0172 0e01 0000 6304 0000 0000 0000 0000  .r....c.........
-000049f0: 0000 0008 0000 0007 0000 0043 0000 0073  ...........C...s
-00004a00: 9000 0000 7400 a001 7402 7c01 6401 8302  ....t...t.|.d...
-00004a10: a101 7c02 1700 7d01 7c03 6400 6b08 7220  ..|...}.|.d.k.r 
-00004a20: 7c02 7d03 7400 a003 7400 a004 7c02 a101  |.}.t...t...|...
-00004a30: 7400 6a05 1400 7c00 7400 a004 7c03 a101  t.j...|.t...|...
-00004a40: 7400 6a05 1400 6603 a101 7d00 6700 7d04  t.j...f...}.g.}.
-00004a50: 7c01 4400 5d34 7d05 7400 a006 6402 7c05  |.D.]4}.t...d.|.
-00004a60: 7c02 1800 6702 a101 7d06 7c05 7c03 1700  |...g...}.|.|...
-00004a70: 6403 1700 7d07 7c04 a007 7c00 7c06 7c07  d...}.|...|.|.|.
-00004a80: 8502 1900 a101 0100 7150 7400 a001 7c04  ........qPt...|.
-00004a90: a101 5300 2904 4e54 7201 0000 0072 2e00  ..S.).NTr....r..
-00004aa0: 0000 2908 721d 0000 0072 3800 0000 7257  ..).r....r8...rW
-00004ab0: 0000 0072 2600 0000 7236 0000 0072 2200  ...r&...r6...r".
-00004ac0: 0000 da03 6d61 7872 2300 0000 2908 7253  ....maxr#...).rS
-00004ad0: 0000 0072 2b00 0000 5a09 7374 6172 745f  ...r+...Z.start_
-00004ae0: 7061 645a 0765 6e64 5f70 6164 5a05 785f  padZ.end_padZ.x_
-00004af0: 6f75 7472 3300 0000 723f 0000 0072 4000  outr3...r?...r@.
-00004b00: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00004b10: 00da 0d63 7574 5f77 6974 685f 6e61 6e73  ...cut_with_nans
-00004b20: ef02 0000 7314 0000 0000 0114 0108 0104  ....s...........
-00004b30: 0128 0104 0108 0112 010c 0114 0172 1001  .(...........r..
-00004b40: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00004b50: 0000 0005 0000 0043 0000 0073 8000 0000  .......C...s....
-00004b60: 7400 7c00 8301 7d00 7401 7402 7c00 6401  t.|...}.t.t.|.d.
-00004b70: 1900 8301 8301 0100 6402 7403 7402 7c00  ........d.t.t.|.
-00004b80: 6401 1900 8301 8301 a004 a100 6b06 7248  d...........k.rH
-00004b90: 7401 6403 8301 0100 6404 6405 8400 7c00  t.d.....d.d...|.
-00004ba0: 4400 8301 7d01 6e34 7402 7c00 6401 1900  D...}.n4t.|.d...
-00004bb0: 8301 7403 6b02 7270 7401 6406 8301 0100  ..t.k.rpt.d.....
-00004bc0: 6407 6405 8400 7c00 4400 8301 7d01 6e0c  d.d...|.D...}.n.
-00004bd0: 7401 6408 8301 0100 7c00 5300 7c01 5300  t.d.....|.S.|.S.
-00004be0: 2909 4e72 0100 0000 da05 6279 7465 737a  ).Nr......bytesz
-00004bf0: 2544 4543 4f44 4520 7377 6974 6368 696e  %DECODE switchin
-00004c00: 6720 6672 6f6d 2062 7974 6573 2074 6f20  g from bytes to 
-00004c10: 7374 7269 6e67 6301 0000 0000 0000 0000  stringc.........
-00004c20: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
-00004c30: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
-00004c40: 6400 6401 a102 9102 7104 5300 a902 da05  d.d.....q.S.....
-00004c50: 6173 6369 69da 0669 676e 6f72 6529 01da  ascii..ignore)..
-00004c60: 0664 6563 6f64 6572 3100 0000 7216 0000  .decoder1...r...
-00004c70: 0072 1600 0000 7217 0000 0072 3400 0000  .r....r....r4...
-00004c80: 0103 0000 7304 0000 0006 0002 007a 2668  ....s........z&h
-00004c90: 355f 7374 7269 6e67 5f73 7769 7463 6865  5_string_switche
-00004ca0: 722e 3c6c 6f63 616c 733e 2e3c 6c69 7374  r.<locals>.<list
-00004cb0: 636f 6d70 3e7a 2545 4e43 4f44 4520 7377  comp>z%ENCODE sw
-00004cc0: 6974 6368 696e 6720 6672 6f6d 2073 7472  itching from str
-00004cd0: 696e 6720 746f 2062 7974 6573 6301 0000  ing to bytesc...
-00004ce0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00004cf0: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-00004d00: 7d01 7c01 a000 6400 6401 a102 9102 7104  }.|...d.d.....q.
-00004d10: 5300 7212 0100 00a9 01da 0665 6e63 6f64  S.r........encod
-00004d20: 6572 3100 0000 7216 0000 0072 1600 0000  er1...r....r....
-00004d30: 7217 0000 0072 3400 0000 0403 0000 7304  r....r4.......s.
-00004d40: 0000 0006 0002 007a 2b6e 6f74 2062 7974  .......z+not byt
-00004d50: 6573 206f 7220 7374 7269 6e67 2066 6f72  es or string for
-00004d60: 6d61 742c 2072 6574 7572 6e69 6e67 2069  mat, returning i
-00004d70: 6e70 7574 2905 7257 0000 0072 4b00 0000  nput).rW...rK...
-00004d80: da04 7479 7065 72a9 0000 00da 056c 6f77  ..typer......low
-00004d90: 6572 2902 da07 6c69 7374 5f69 6e72 8f00  er)...list_inr..
-00004da0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00004db0: 0072 af00 0000 fc02 0000 7316 0000 0000  .r........s.....
-00004dc0: 0108 0110 0118 0108 0110 0110 0108 0110  ................
-00004dd0: 0208 0104 0172 af00 0000 e910 2700 00da  .....r......'...
-00004de0: 0659 4841 545f 5f72 d000 0000 6305 0000  .YHAT__r....c...
-00004df0: 0000 0000 0000 0000 000f 0000 000b 0000  ................
-00004e00: 0043 0000 0073 c200 0000 7400 7c00 6401  .C...s....t.|.d.
-00004e10: 8302 4400 5db2 7d05 7401 7c05 8301 7d06  ..D.].}.t.|...}.
-00004e20: 7400 7c01 6401 8302 4400 5d9a 7d07 7402  t.|.d...D.].}.t.
-00004e30: a003 7c07 6402 a102 8f50 7d08 6700 7d09  ..|.d....P}.g.}.
-00004e40: 7404 7c08 6403 1900 6a05 8301 6404 1900  t.|.d...j...d...
-00004e50: 7d0a 7406 7c0a 7c02 8302 4400 5d28 5c02  }.t.|.|...D.](\.
-00004e60: 7d0b 7d0c 7c08 6403 1900 7c0b 7c0c 8502  }.}.|.d...|.|...
-00004e70: 1900 7d0d 7c09 a007 7c06 a008 7c0d a101  ..}.|...|...|...
-00004e80: a101 0100 7152 5700 3500 5100 5200 5800  ....qRW.5.Q.R.X.
-00004e90: 7409 a00a 7c09 a101 7d09 7c03 740b 6a0c  t...|...}.|.t.j.
-00004ea0: a00d 7c05 a101 a00e 6405 a101 6404 1900  ..|.....d...d...
-00004eb0: 1700 7c04 1700 7d0e 740f 7c07 7c0e 7c09  ..|...}.t.|.|.|.
-00004ec0: 8303 0100 7120 710a 6400 5300 2906 4e54  ....q q.d.S.).NT
-00004ed0: 726d 0000 0072 4900 0000 7201 0000 00da  rm...rI...r.....
-00004ee0: 012e 2910 7257 0000 0072 6300 0000 72aa  ..).rW...rc...r.
-00004ef0: 0000 0072 ab00 0000 7239 0000 0072 2100  ...r....r9...r!.
-00004f00: 0000 720d 0100 0072 2300 0000 72ae 0000  ..r....r#...r...
-00004f10: 0072 1d00 0000 7226 0000 0072 5f00 0000  .r....r&...r_...
-00004f20: 7261 0000 0072 a400 0000 72d7 0000 00da  ra...r....r.....
-00004f30: 106f 7665 7277 7269 7465 5f68 355f 6b65  .overwrite_h5_ke
-00004f40: 7929 0f5a 086d 6f64 5f6c 6973 7472 5000  y).Z.mod_listrP.
-00004f50: 0000 720c 0100 005a 0c66 726f 6e74 5f61  ..r....Z.front_a
-00004f60: 7070 656e 645a 0b62 6163 6b5f 6170 7065  ppendZ.back_appe
-00004f70: 6e64 5a07 6d6f 645f 7374 7272 b800 0000  ndZ.mod_strr....
-00004f80: 7251 0000 0072 bc00 0000 da04 7968 6174  rQ...r......yhat
-00004f90: da08 6c65 6e5f 6461 7461 723f 0000 0072  ..len_datar?...r
-00004fa0: 4000 0000 da02 6664 da09 7772 6974 655f  @.....fd..write_
-00004fb0: 6b65 7972 1600 0000 7216 0000 0072 1700  keyr....r....r..
-00004fc0: 0000 da10 666f 6f5f 7072 6564 6963 745f  ....foo_predict_
-00004fd0: 6d6f 6473 1903 0000 7318 0000 0000 010e  mods....s.......
-00004fe0: 0108 010e 010e 0104 0112 0112 0110 011c  ................
-00004ff0: 010a 011e 0172 2301 0000 da09 7465 6d70  .....r#.....temp
-00005000: 5f79 6861 7463 0400 0000 0000 0000 0000  _yhatc..........
-00005010: 0000 0b00 0000 0a00 0000 4300 0000 738a  ..........C...s.
-00005020: 0000 0074 007c 0183 0144 005d 7c7d 0474  ...t.|...D.]|}.t
-00005030: 01a0 027c 0464 01a1 028f 667d 0567 007d  ...|.d....f}.g.}
-00005040: 0674 037c 0564 0219 006a 0483 0164 0319  .t.|.d...j...d..
-00005050: 007d 0774 057c 077c 0383 0244 005d 285c  .}.t.|.|...D.](\
-00005060: 027d 087d 097c 0564 0219 007c 087c 0985  .}.}.|.d...|.|..
-00005070: 0219 007d 0a7c 06a0 067c 00a0 077c 0aa1  ...}.|...|...|..
-00005080: 01a1 0101 0071 3a74 08a0 097c 06a1 017d  .....q:t...|...}
-00005090: 0674 0a7c 047c 027c 0683 0301 0057 0035  .t.|.|.|.....W.5
-000050a0: 0051 0052 0058 0071 0864 0053 0029 044e  .Q.R.X.q.d.S.).N
-000050b0: 726d 0000 0072 4900 0000 7201 0000 0029  rm...rI...r....)
-000050c0: 0bda 0767 6574 5f68 3573 72aa 0000 0072  ...get_h5sr....r
-000050d0: ab00 0000 7239 0000 0072 2100 0000 720d  ....r9...r!...r.
-000050e0: 0100 0072 2300 0000 72ae 0000 0072 1d00  ...r#...r....r..
-000050f0: 0000 7225 0000 0072 1e01 0000 290b 72b8  ..r%...r....).r.
-00005100: 0000 00da 0668 355f 6469 7272 2201 0000  .....h5_dirr"...
-00005110: 720c 0100 0072 5100 0000 72bc 0000 0072  r....rQ...r....r
-00005120: 1f01 0000 7220 0100 0072 3f00 0000 7240  ....r ...r?...r@
-00005130: 0000 0072 2101 0000 7216 0000 0072 1600  ...r!...r....r..
-00005140: 0000 7217 0000 00da 0e66 6f6f 5f70 7265  ..r......foo_pre
-00005150: 6469 6374 5f76 3228 0300 0073 1200 0000  dict_v2(...s....
-00005160: 0001 0c01 0e01 0401 1201 1201 1001 1201  ................
-00005170: 0a01 7227 0100 0063 0300 0000 0000 0000  ..r'...c........
-00005180: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-00005190: 7334 0000 0074 007c 0183 0144 005d 267d  s4...t.|...D.]&}
-000051a0: 0374 01a0 027c 0364 01a1 027d 047c 00a0  .t...|.d...}.|..
-000051b0: 037c 04a1 017d 0574 047c 037c 027c 0583  .|...}.t.|.|.|..
-000051c0: 0301 0071 0864 0053 0029 024e 7249 0000  ...q.d.S.).NrI..
-000051d0: 0029 0572 2501 0000 7208 0000 00da 1a67  .).r%...r......g
-000051e0: 6574 5f68 355f 6b65 795f 616e 645f 636f  et_h5_key_and_co
-000051f0: 6e63 6174 656e 6174 6572 ae00 0000 721e  ncatenater....r.
-00005200: 0100 0029 0672 b800 0000 7226 0100 0072  ...).r....r&...r
-00005210: 2201 0000 7251 0000 0072 2101 0000 721f  "...rQ...r!...r.
-00005220: 0100 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00005230: 0000 da0b 666f 6f5f 7072 6564 6963 7434  ....foo_predict4
-00005240: 0300 0073 0800 0000 0014 0c01 0c01 0a01  ...s............
-00005250: 7229 0100 0072 2e00 0000 6304 0000 0000  r)...r....c.....
-00005260: 0000 0000 0000 000d 0000 0007 0000 0043  ...............C
-00005270: 0000 0073 8001 0000 7400 a001 7400 a002  ...s....t...t...
-00005280: 7c02 a101 7c03 6401 1800 1400 6402 1b00  |...|.d.....d...
-00005290: a101 a003 7404 a101 7d04 7400 a002 7c02  ....t...}.t...|.
-000052a0: a101 7c03 1400 7d02 7400 a002 7c00 6a05  ..|...}.t...|.j.
-000052b0: 6403 6402 8502 1900 a101 7d05 7c01 7c04  d.d.......}.|.|.
-000052c0: 1800 7d01 7c01 a006 a100 7d06 7c01 7400  ..}.|.....}.|.t.
-000052d0: a002 7c02 a101 1700 7d07 7c07 a006 a100  ..|.....}.|.....
-000052e0: 7d08 6404 7c01 7c01 6404 6b00 3c00 7400  }.d.|.|.d.k.<.t.
-000052f0: a002 7c05 a101 7c07 7c05 6b04 1900 7c07  ..|...|.|.k...|.
-00005300: 7c07 7c05 6b04 3c00 7c01 7c06 1800 7d09  |.|.k.<.|.|...}.
-00005310: 7c00 7c01 6404 1900 7c07 6404 1900 8502  |.|.d...|.d.....
-00005320: 7c01 6401 1900 7c07 6401 1900 8502 6405  |.d...|.d.....d.
-00005330: 6603 1900 a003 6406 a101 7d0a 7407 7c0a  f.....d...}.t.|.
-00005340: 6a05 8301 7d0b 7c02 a008 a100 7c0b 6403  j...}.|.....|.d.
-00005350: 6402 8502 3c00 7400 6a09 6a0a 6407 7c0b  d...<.t.j.j.d.|.
-00005360: 6408 8d02 a003 6406 a101 7d0c 740b 7c0b  d.....d...}.t.|.
-00005370: 8301 6402 6b04 9001 723e 7c0a 7c0c 7c09  ..d.k...r>|.|.|.
-00005380: 6404 1900 7c09 6404 1900 7c0a 6a05 6404  d...|.d...|.j.d.
-00005390: 1900 1700 8502 7c09 6401 1900 7c09 6401  ......|.d...|.d.
-000053a0: 1900 7c0a 6a05 6401 1900 1700 8502 6405  ..|.j.d.......d.
-000053b0: 6603 3c00 6e38 7c0a 7c0c 7c09 6404 1900  f.<.n8|.|.|.d...
-000053c0: 7c09 6404 1900 7c0a 6a05 6404 1900 1700  |.d...|.j.d.....
-000053d0: 8502 7c09 6401 1900 7c09 6401 1900 7c0a  ..|.d...|.d...|.
-000053e0: 6a05 6401 1900 1700 8502 6602 3c00 7c0c  j.d.......f.<.|.
-000053f0: 7c06 7c08 6603 5300 2909 61b8 0100 0054  |.|.f.S.).a....T
-00005400: 6869 7320 6973 2061 6e20 6163 6365 7373  his is an access
-00005410: 6f72 7920 6675 6e63 7469 6f6e 2074 6f20  ory function to 
-00005420: 7472 6163 6b20 746f 2069 6d70 726f 7665  track to improve
-00005430: 2074 7261 636b 696e 6720 7370 6565 642e   tracking speed.
-00005440: 2054 6869 7320 6372 6f70 7320 7468 6520   This crops the 
-00005450: 696e 6974 6961 6c20 6c61 7267 6520 696d  initial large im
-00005460: 6167 6520 696e 746f 2061 2073 6d61 6c6c  age into a small
-00005470: 6572 206f 6e65 2c20 6261 7365 6420 6f6e  er one, based on
-00005480: 2074 6865 2069 6e66 6c61 7469 6f6e 2072   the inflation r
-00005490: 6174 652e 0a20 2020 2020 2020 2049 6e66  ate..        Inf
-000054a0: 6c61 7469 6f6e 2072 6174 6520 6f66 2033  lation rate of 3
-000054b0: 203d 2033 2078 2033 2074 656d 706c 6174   = 3 x 3 templat
-000054c0: 6520 696d 6167 6520 7369 7a65 2061 726f  e image size aro
-000054d0: 756e 6420 7468 6520 6669 7273 7420 6775  und the first gu
-000054e0: 6573 7365 6420 706f 6c65 206c 6f63 6174  essed pole locat
-000054f0: 696f 6e2e 0a0a 2020 2020 2020 2020 5061  ion...        Pa
-00005500: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00005510: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00005520: 2020 2020 696d 203a 0a0a 2020 2020 2020      im :..      
-00005530: 2020 6372 6f70 5f74 6f70 5f6c 6566 7420    crop_top_left 
-00005540: 3a0a 0a20 2020 2020 2020 2073 697a 655f  :..        size_
-00005550: 6372 6f70 203a 0a0a 2020 2020 2020 2020  crop :..        
-00005560: 696e 666c 6174 696f 6e20 3a0a 2020 2020  inflation :.    
-00005570: 2020 2020 2020 2020 2028 4465 6661 756c           (Defaul
-00005580: 7420 7661 6c75 6520 3d20 3329 0a0a 2020  t value = 3)..  
-00005590: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-000055a0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20        -------.. 
-000055b0: 2020 2020 2020 2072 2e00 0000 7247 0000         r....rG..
-000055c0: 004e 7201 0000 002e da05 7569 6e74 38e9  .Nr.......uint8.
-000055d0: 0001 0000 2901 da04 7369 7a65 290c 721d  ....)...size).r.
-000055e0: 0000 00da 0566 6c6f 6f72 7238 0000 0072  .....floorr8...r
-000055f0: 8100 0000 7284 0000 0072 2100 0000 721b  ....r....r!...r.
-00005600: 0000 0072 3900 0000 da06 746f 6c69 7374  ...r9.....tolist
-00005610: 721e 0000 00da 0772 616e 6469 6e74 7230  r......randintr0
-00005620: 0000 0029 0dda 0269 6d5a 0d63 726f 705f  ...)...imZ.crop_
-00005630: 746f 705f 6c65 6674 5a09 7369 7a65 5f63  top_leftZ.size_c
-00005640: 726f 705a 0969 6e66 6c61 7469 6f6e 5a0f  ropZ.inflationZ.
-00005650: 696e 666c 6174 696f 6e5f 7368 6966 745a  inflation_shiftZ
-00005660: 0769 6d73 6861 7065 da0e 6372 6f70 5f74  .imshape..crop_t
-00005670: 6f70 5f6c 6566 7432 5a11 6372 6f70 5f62  op_left2Z.crop_b
-00005680: 6f74 746f 6d5f 7269 6768 74da 1263 726f  ottom_right..cro
-00005690: 705f 626f 7474 6f6d 5f72 6967 6874 325a  p_bottom_right2Z
-000056a0: 0654 4c5f 6164 6a5a 0963 5f63 726f 7070  .TL_adjZ.c_cropp
-000056b0: 6564 5a08 6372 6f70 5f64 696d 5a0d 6372  edZ.crop_dimZ.cr
-000056c0: 6f70 7065 645f 696d 6167 6572 1600 0000  opped_imager....
-000056d0: 7216 0000 0072 1700 0000 da18 6372 6f70  r....r......crop
-000056e0: 5f69 6d61 6765 5f66 726f 6d5f 746f 705f  _image_from_top_
-000056f0: 6c65 6674 4e03 0000 7336 0000 0000 1322  leftN...s6....."
-00005700: 020e 0114 0308 0108 010e 0108 030c 011a  ................
-00005710: 0308 0226 0102 ff04 040a 0110 0116 020e  ...&............
-00005720: 0202 ff32 0102 ff06 0402 ff1a 0106 0010  ...2............
-00005730: ff06 0372 3301 0000 7296 0000 0063 0300  ...r3...r....c..
-00005740: 0000 0000 0000 0000 0000 1800 0000 0e00  ................
-00005750: 0000 0300 0000 7392 0100 0074 00a0 017c  ......s....t...|
-00005760: 0064 01a1 027d 0374 00a0 017c 0064 02a1  .d...}.t...|.d..
-00005770: 027d 0474 00a0 017c 0064 03a1 027d 0574  .}.t...|.d...}.t
-00005780: 027c 056a 0364 0064 0485 0219 0083 017d  .|.j.d.d.......}
-00005790: 0687 0066 0164 0564 0684 0874 00a0 017c  ...f.d.d...t...|
-000057a0: 0064 07a1 0244 0083 017d 0774 006a 047c  .d...D...}.t.j.|
-000057b0: 0064 087c 0664 0919 007c 0664 0a19 0064  .d.|.d...|.d...d
-000057c0: 0b64 0b64 0b64 0874 056a 066a 0774 056a  .d.d.d.t.j.j.t.j
-000057d0: 066a 087c 0264 0c64 0d8d 0c7d 0874 097c  .j.|.d.d...}.t.|
-000057e0: 007c 086a 0a83 0201 0074 097c 007c 086a  .|.j.....t.|.|.j
-000057f0: 0b83 0201 0074 097c 0064 0e83 0201 0074  .....t.|.d.....t
-00005800: 0c74 0d74 0e7c 0383 0174 0f7c 0383 0164  .t.t.|...t.|...d
-00005810: 0f8d 0283 0144 005d d05c 027d 095c 027d  .....D.].\.}.\.}
-00005820: 0a7d 0b7c 077c 0919 007d 0c74 10a0 117c  .}.|.|...}.t...|
-00005830: 0ca1 017d 0d7c 047c 0a7c 0b85 0219 007d  ...}.|.|.|.....}
-00005840: 0e7c 0da0 12a1 0064 086b 0272 fa74 1364  .|.....d.k.r.t.d
-00005850: 1083 0101 0074 147c 0da0 1564 11a1 0183  .....t.|...d....
-00005860: 017d 0f67 007d 1074 167c 0f83 0144 005d  .}.g.}.t.|...D.]
-00005870: 507d 117c 0da0 1774 106a 187c 11a1 0201  P}.|...t.j.|....
-00005880: 007c 0da0 19a1 005c 027d 127d 137c 0e7c  .|.....\.}.}.|.|
-00005890: 1119 007d 1474 1a7c 137c 1464 0a19 007c  ...}.t.|.|.d...|
-000058a0: 1464 0919 0067 027c 0683 035c 037d 157d  .d...g.|...\.}.}
-000058b0: 167d 177c 10a0 1b7c 15a1 0101 0090 0171  .}.|...|.......q
-000058c0: 1474 1ca0 1d7c 10a1 017d 107c 08a0 1e7c  .t...|...}.|...|
-000058d0: 1064 1274 1ca0 1f7c 106a 0364 0919 00a1  .d.t...|.j.d....
-000058e0: 0114 00a1 0201 0071 bc64 0053 0029 134e  .......q.d.S.).N
-000058f0: 7241 0000 0072 7f00 0000 7292 0000 0072  rA...r....r....r
-00005900: 4700 0000 6301 0000 0000 0000 0000 0000  G...c...........
-00005910: 0002 0000 0009 0000 0013 0000 0073 2a00  .............s*.
-00005920: 0000 6700 7c00 5d22 7d01 8800 7400 6a01  ..g.|.]"}...t.j.
-00005930: 1700 7400 6a02 a003 7c01 a004 6400 6401  ..t.j...|...d.d.
-00005940: a102 a101 1700 9102 7104 5300 7212 0100  ........q.S.r...
-00005950: 0029 0572 5f00 0000 7260 0000 0072 6100  .).r_...r`...ra.
-00005960: 0000 72a4 0000 0072 1501 0000 7231 0000  ..r....r....r1..
-00005970: 00a9 01da 066d 7034 5f62 6472 1600 0000  .....mp4_bdr....
-00005980: 7217 0000 0072 3400 0000 8b03 0000 7304  r....r4.......s.
-00005990: 0000 0006 0002 007a 3669 6e73 6572 745f  .......z6insert_
-000059a0: 696d 6167 6573 5f69 6e74 6f5f 6665 6174  images_into_feat
-000059b0: 7572 655f 6461 7461 5f68 352e 3c6c 6f63  ure_data_h5.<loc
-000059c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-000059d0: 9300 0000 4672 0100 0000 722e 0000 0054  ....Fr....r....T
-000059e0: 5a05 5452 4153 4829 0bda 186f 7665 7277  Z.TRASH)...overw
-000059f0: 7269 7465 5f69 665f 6669 6c65 5f65 7869  rite_if_file_exi
-00005a00: 7374 73da 0e6d 6178 5f69 6d67 5f68 6569  sts..max_img_hei
-00005a10: 6768 74da 0d6d 6178 5f69 6d67 5f77 6964  ght..max_img_wid
-00005a20: 7468 da20 636c 6f73 655f 616e 645f 6f70  th. close_and_op
-00005a30: 656e 5f6f 6e5f 6561 6368 5f69 7465 7261  en_on_each_itera
-00005a40: 7469 6f6e da0d 636f 6c6f 725f 6368 616e  tion..color_chan
-00005a50: 6e65 6cda 1261 6464 5f74 6f5f 6578 6973  nel..add_to_exis
-00005a60: 7469 6e67 5f48 35da 1a69 676e 6f72 655f  ting_H5..ignore_
-00005a70: 696d 6167 655f 7261 6e67 655f 7761 726e  image_range_warn
-00005a80: 696e 67da 0964 7479 7065 5f69 6d67 da0c  ing..dtype_img..
-00005a90: 6474 7970 655f 6c61 6265 6c73 da0e 696d  dtype_labels..im
-00005aa0: 6167 655f 6b65 795f 6e61 6d65 da0e 6c61  age_key_name..la
-00005ab0: 6265 6c5f 6b65 795f 6e61 6d65 da0a 6d75  bel_key_name..mu
-00005ac0: 6c74 6970 6c69 6572 a901 da05 746f 7461  ltiplier....tota
-00005ad0: 6c7a 1865 7272 6f72 206f 7065 6e69 6e67  lz.error opening
-00005ae0: 2076 6964 656f 2066 696c 6572 4500 0000   video filerE...
-00005af0: 724a 0000 0029 2072 0800 0000 7228 0100  rJ...) r....r(..
-00005b00: 0072 3900 0000 7221 0000 00da 1468 355f  .r9...r!.....h5_
-00005b10: 6974 6572 6174 6976 655f 6372 6561 746f  iterative_creato
-00005b20: 7272 aa00 0000 da03 6835 74da 0853 5444  rr......h5t..STD
-00005b30: 5f55 3842 45da 0953 5444 5f49 3332 4c45  _U8BE..STD_I32LE
-00005b40: da0a 6465 6c5f 6835 5f6b 6579 5a07 696d  ..del_h5_keyZ.im
-00005b50: 675f 6b65 7972 4001 0000 7224 0000 0072  g_keyr@...r$...r
-00005b60: 0b00 0000 7237 0000 0072 3000 0000 72c2  ....r7...r0...r.
-00005b70: 0000 0072 c300 0000 72c4 0000 0072 4b00  ...r....r....rK.
-00005b80: 0000 7284 0000 0072 c500 0000 723a 0000  ..r....r....r:..
-00005b90: 0072 d900 0000 5a13 4341 505f 5052 4f50  .r....Z.CAP_PROP
-00005ba0: 5f50 4f53 5f46 5241 4d45 53da 0472 6561  _POS_FRAMES..rea
-00005bb0: 6472 3301 0000 7223 0000 0072 1d00 0000  dr3...r#...r....
-00005bc0: 7238 0000 00da 0961 6464 5f74 6f5f 6835  r8.....add_to_h5
-00005bd0: 7236 0000 0029 1872 5100 0000 7235 0100  r6...).rQ...r5..
-00005be0: 005a 0969 6d61 6765 5f6b 6579 7241 0000  .Z.image_keyrA..
-00005bf0: 0072 7f00 0000 7292 0000 005a 0869 6d67  .r....r....Z.img
-00005c00: 5f73 697a 655a 086d 7034 5f6c 6973 745a  _sizeZ.mp4_listZ
-00005c10: 0a68 355f 6372 6561 746f 7272 2c00 0000  .h5_creatorr,...
-00005c20: 72b9 0000 0072 ba00 0000 72c6 0000 0072  r....r....r....r
-00005c30: c700 0000 5a0c 746d 705f 6c6f 6361 7469  ....Z.tmp_locati
-00005c40: 6f6e 72c8 0000 0072 9600 0000 da02 666e  onr....r......fn
-00005c50: da07 7375 6363 6573 735a 086f 675f 6672  ..successZ.og_fr
-00005c60: 616d 65da 096c 6f63 6174 696f 6e73 5a08  ame..locationsZ.
-00005c70: 6372 6f70 5f69 6d67 7231 0100 0072 3201  crop_imgr1...r2.
-00005c80: 0000 7216 0000 0072 3401 0000 7217 0000  ..r....r4...r...
-00005c90: 00da 2269 6e73 6572 745f 696d 6167 6573  .."insert_images
-00005ca0: 5f69 6e74 6f5f 6665 6174 7572 655f 6461  _into_feature_da
-00005cb0: 7461 5f68 3585 0300 0073 5400 0000 0001  ta_h5....sT.....
-00005cc0: 0c02 0c01 0c01 1201 0a01 0aff 0603 0601  ................
-00005cd0: 0201 0601 0601 0201 0201 0201 0201 0601  ................
-00005ce0: 0601 0201 02f5 060d 0c01 0c01 0a02 2401  ..............$.
-00005cf0: 0801 0a01 0c01 0c01 0801 0e01 0401 0c01  ................
-00005d00: 0e01 0c01 0801 0401 0e01 02fe 0a03 0e01  ................
-00005d10: 0a01 724e 0100 0063 0100 0000 0000 0000  ..rN...c........
-00005d20: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00005d30: 7314 0000 0074 007c 0083 0101 0074 017c  s....t.|.....t.|
-00005d40: 0083 0101 0064 0053 0072 0901 0000 2902  .....d.S.r....).
-00005d50: 7274 0000 0072 a600 0000 a901 5a06 6469  rt...r......Z.di
-00005d60: 725f 696e 7216 0000 0072 1600 0000 7217  r_inr....r....r.
-00005d70: 0000 00da 0963 6c65 6172 5f64 6972 b303  .....clear_dir..
-00005d80: 0000 7304 0000 0000 0108 0172 5001 0000  ..s........rP...
-00005d90: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00005da0: 0003 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
-00005db0: 6a01 a002 7c00 a101 7216 7403 a004 7c00  j...|...r.t...|.
-00005dc0: a101 0100 6400 5300 7209 0100 0029 0572  ....d.S.r....).r
-00005dd0: 5f00 0000 7261 0000 0072 6200 0000 7273  _...ra...rb...rs
-00005de0: 0000 0072 7400 0000 724f 0100 0072 1600  ...rt...rO...r..
-00005df0: 0000 7216 0000 0072 1700 0000 7274 0000  ..r....r....rt..
-00005e00: 00b8 0300 0073 0400 0000 0001 0c01 7274  .....s........rt
-00005e10: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00005e20: 0500 0000 0600 0000 4300 0000 736a 0000  ........C...sj..
-00005e30: 0064 017d 027c 0164 006b 0272 1274 006a  .d.}.|.d.k.r.t.j
-00005e40: 017d 017c 0064 0219 0064 036b 0273 2a7c  .}.|.d...d.k.s*|
-00005e50: 0064 0219 0064 046b 0272 2e7c 017d 0264  .d...d.k.r.|.}.d
-00005e60: 04a0 0264 0564 0684 007c 00a0 0364 03a1  ...d.d...|...d..
-00005e70: 0144 0083 01a1 017d 0364 0764 0684 007c  .D.....}.d.d...|
-00005e80: 03a0 0364 04a1 0144 0083 017d 047c 027c  ...d...D...}.|.|
-00005e90: 01a0 027c 04a1 0117 0053 0029 084e 72d0  ...|.....S.).Nr.
-00005ea0: 0000 0072 0100 0000 fa01 2ffa 015c 6301  ...r....../..\c.
-00005eb0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00005ec0: 0000 0053 0000 0073 1c00 0000 6700 7c00  ...S...s....g.|.
-00005ed0: 5d14 7d01 7400 7c01 8301 6400 6b04 7204  ].}.t.|...d.k.r.
-00005ee0: 7c01 9102 7104 5300 a901 7201 0000 0072  |...q.S...r....r
-00005ef0: 4800 0000 7231 0000 0072 1600 0000 7216  H...r1...r....r.
-00005f00: 0000 0072 1700 0000 7234 0000 00c3 0300  ...r....r4......
-00005f10: 0073 0600 0000 0600 0200 0c00 7a1d 6e6f  .s..........z.no
-00005f20: 726d 5f70 6174 682e 3c6c 6f63 616c 733e  rm_path.<locals>
-00005f30: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
-00005f40: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00005f50: 5300 0000 731c 0000 0067 007c 005d 147d  S...s....g.|.].}
-00005f60: 0174 007c 0183 0164 006b 0472 047c 0191  .t.|...d.k.r.|..
-00005f70: 0271 0453 0072 5301 0000 7248 0000 0072  .q.S.rS...rH...r
-00005f80: 3100 0000 7216 0000 0072 1600 0000 7217  1...r....r....r.
-00005f90: 0000 0072 3400 0000 c403 0000 7306 0000  ...r4.......s...
-00005fa0: 0006 0002 000c 0029 0472 5f00 0000 7260  .......).r_...r`
-00005fb0: 0000 0072 d600 0000 72d7 0000 0029 05da  ...r....r....)..
-00005fc0: 0770 6174 685f 696e 7260 0000 005a 0961  .path_inr`...Z.a
-00005fd0: 6464 5f73 7461 7274 5a08 746d 705f 6c69  dd_startZ.tmp_li
-00005fe0: 7374 5a0a 6669 6e61 6c5f 6c69 7374 7216  stZ.final_listr.
-00005ff0: 0000 0072 1600 0000 7217 0000 0072 9a00  ...r....r....r..
-00006000: 0000 bd03 0000 7310 0000 0000 0104 0108  ......s.........
-00006010: 0106 0118 0104 011a 0114 0172 9a00 0000  ...........r....
-00006020: 7249 0000 00da 0c46 445f 5f6f 7269 6769  rI.....FD__origi
-00006030: 6e61 6cda 0843 4e4e 5f70 7265 6463 0200  nal..CNN_predc..
-00006040: 0000 0000 0000 0000 0000 0500 0000 0900  ................
-00006050: 0000 4300 0000 7358 0000 0074 0083 007d  ..C...sX...t...}
-00006060: 027c 0164 016b 0872 1267 007d 0174 01a0  .|.d.k.r.g.}.t..
-00006070: 027c 0064 02a1 028f 307d 037c 03a0 03a1  .|.d....0}.|....
-00006080: 0044 005d 207d 047c 047c 016b 0772 287c  .D.] }.|.|.k.r(|
-00006090: 037c 0419 0064 0164 0185 0219 007c 027c  .|...d.d.....|.|
-000060a0: 043c 0071 2857 0035 0051 0052 0058 007c  .<.q(W.5.Q.R.X.|
-000060b0: 0253 0029 037a b50a 0a20 2020 2050 6172  .S.).z...    Par
-000060c0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-000060d0: 2d2d 2d2d 2d2d 0a20 2020 2068 355f 696e  ------.    h5_in
-000060e0: 203a 0a20 2020 2065 7863 6c75 6465 5f6b   :.    exclude_k
-000060f0: 6579 7320 3a20 6279 2064 6566 6175 6c74  eys : by default
-00006100: 2065 7863 6c75 6465 7320 616c 6c20 7468   excludes all th
-00006110: 6520 616c 7267 6520 6461 7461 2069 6e20  e alrge data in 
-00006120: 7468 6520 4835 2066 696c 652c 2073 6574  the H5 file, set
-00006130: 2074 6f20 225b 5d22 2074 6f20 6765 7420   to "[]" to get 
-00006140: 7468 6520 656e 7469 7265 2048 350a 0a20  the entire H5.. 
-00006150: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00006160: 2d2d 2d2d 2d2d 0a0a 2020 2020 4e72 6d00  ------..    Nrm.
-00006170: 0000 2904 7268 0000 0072 aa00 0000 72ab  ..).rh...r....r.
-00006180: 0000 0072 9500 0000 2905 72be 0000 005a  ...r....).r....Z
-00006190: 0c65 7863 6c75 6465 5f6b 6579 7372 6a00  .exclude_keysrj.
-000061a0: 0000 72bc 0000 0072 3300 0000 7216 0000  ..r....r3...r...
-000061b0: 0072 1600 0000 7217 0000 00da 0a68 355f  .r....r......h5_
-000061c0: 746f 5f64 6963 74c8 0300 0073 1000 0000  to_dict....s....
-000061d0: 000c 0601 0801 0401 0e01 0c01 0801 2001  .............. .
-000061e0: 7257 0100 00da 0473 616d 6563 0300 0000  rW.....samec....
-000061f0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00006200: 4300 0000 732e 0000 007c 0164 016b 0272  C...s....|.d.k.r
-00006210: 0c7c 0053 0074 00a0 017c 01a1 017c 011b  .|.S.t...|...|..
-00006220: 007d 0374 006a 027c 007c 037c 0264 028d  .}.t.j.|.|.|.d..
-00006230: 037d 047c 0453 0029 034e 722e 0000 0072  .}.|.S.).Nr....r
-00006240: e600 0000 2903 721d 0000 0072 3600 0000  ....).r....r6...
-00006250: 72ea 0000 0029 0572 bb00 0000 da06 7769  r....).r......wi
-00006260: 6e64 6f77 72e7 0000 00da 0362 6f78 5a08  ndowr......boxZ.
-00006270: 795f 736d 6f6f 7468 7216 0000 0072 1600  y_smoothr....r..
-00006280: 0000 7217 0000 0072 ad00 0000 de03 0000  ..r....r........
-00006290: 730a 0000 0000 0108 0104 010e 0110 0172  s..............r
-000062a0: ad00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000062b0: 0001 0000 0004 0000 0043 0000 0073 1600  .........C...s..
-000062c0: 0000 7400 7c00 8301 6a01 6401 6401 6402  ..t.|...j.d.d.d.
-000062d0: 8d02 0100 6400 5300 a903 4e54 a902 da07  ....d.S...NT....
-000062e0: 7061 7265 6e74 73da 0865 7869 7374 5f6f  parents..exist_o
-000062f0: 6b29 0272 0e00 0000 da05 6d6b 6469 7229  k).r......mkdir)
-00006300: 015a 076e 616d 655f 696e 7216 0000 0072  .Z.name_inr....r
-00006310: 1600 0000 7217 0000 0072 a600 0000 e603  ....r....r......
-00006320: 0000 7302 0000 0000 0172 a600 0000 6301  ..s......r....c.
-00006330: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00006340: 0000 0043 0000 0073 1400 0000 7400 7c00  ...C...s....t.|.
-00006350: 7401 6a02 7401 6a03 4200 6401 8d02 5300  t.j.t.j.B.d...S.
-00006360: 2902 4e29 015a 0361 6c67 2904 7206 0000  ).N).Z.alg).r...
-00006370: 0072 0700 0000 da05 464c 4f41 545a 0855  .r......FLOATZ.U
-00006380: 4e53 4947 4e45 4472 cd00 0000 7216 0000  NSIGNEDr....r...
-00006390: 0072 1600 0000 7217 0000 00da 0473 6f72  .r....r......sor
-000063a0: 74ea 0300 0073 0200 0000 0001 7261 0100  t....s......ra..
-000063b0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-000063c0: 0000 0b00 0000 4300 0000 7356 0000 007c  ......C...sV...|
-000063d0: 0174 00a0 017c 01a1 011b 007d 0174 027c  .t...|.....}.t.|
-000063e0: 0083 017d 0274 006a 036a 047c 027c 0264  ...}.t.j.j.|.|.d
-000063f0: 0164 028d 037d 0374 00a0 057c 0374 00a0  .d...}.t...|.t..
-00006400: 067c 0274 00a0 077c 0164 0064 0385 0219  .|.t...|.d.d....
-00006410: 00a1 0114 00a1 01a0 0864 04a1 01a1 027d  .........d.....}
-00006420: 047c 0453 0029 054e 46a9 0172 b300 0000  .|.S.).NF..r....
-00006430: 724a 0000 0072 8400 0000 2909 721d 0000  rJ...r....).r...
-00006440: 0072 3500 0000 7230 0000 0072 1e00 0000  .r5...r0...r....
-00006450: 7220 0000 0072 d700 0000 da04 6365 696c  r ...r......ceil
-00006460: da06 6375 6d73 756d 7281 0000 0029 0572  ..cumsumr....).r
-00006470: 5300 0000 da0b 7370 6c69 745f 7261 7469  S.....split_rati
-00006480: 6f72 c000 0000 5a0a 6d69 7865 645f 696e  or....Z.mixed_in
-00006490: 6473 728f 0000 0072 1600 0000 7216 0000  dsr....r....r...
-000064a0: 0072 1700 0000 da0f 7370 6c69 745f 6c69  .r......split_li
-000064b0: 7374 5f69 6e64 73ef 0300 0073 0a00 0000  st_inds....s....
-000064c0: 0001 0e01 0801 1201 2a01 7266 0100 0063  ........*.rf...c
-000064d0: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-000064e0: 0600 0000 4300 0000 7342 0000 0074 007c  ....C...sB...t.|
-000064f0: 007c 0183 027d 0267 007d 037c 0244 005d  .|...}.g.}.|.D.]
-00006500: 2a7d 0467 007d 057c 0444 005d 127d 067c  *}.g.}.|.D.].}.|
-00006510: 05a0 017c 007c 0619 00a1 0101 0071 1e7c  ...|.|.......q.|
-00006520: 03a0 017c 05a1 0101 0071 127c 0353 0072  ...|.....q.|.S.r
-00006530: 0901 0000 2902 7266 0100 0072 2300 0000  ....).rf...r#...
-00006540: 2907 7253 0000 0072 6501 0000 722b 0000  ).rS...re...r+..
-00006550: 0072 8f00 0000 7233 0000 0072 f700 0000  .r....r3...r....
-00006560: 72ba 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00006570: 1700 0000 da0a 7370 6c69 745f 6c69 7374  ......split_list
-00006580: f703 0000 7310 0000 0000 010a 0104 0108  ....s...........
-00006590: 0104 0108 0110 010c 0172 6701 0000 da0a  .........rg.....
-000065a0: 7968 6174 5f70 726f 6261 721f 0100 0063  yhat_probar....c
-000065b0: 0600 0000 0000 0000 0000 0000 0d00 0000  ................
-000065c0: 0a00 0000 4300 0000 73ce 0000 0074 007c  ....C...s....t.|
-000065d0: 0083 017d 0074 01a0 02a1 007d 067c 0164  ...}.t.....}.|.d
-000065e0: 006b 0872 1e7c 066a 037d 017c 0044 005d  .k.r.|.j.}.|.D.]
-000065f0: a67d 0774 047c 0783 0101 0074 057c 077c  .}.t.|.....t.|.|
-00006600: 0483 027d 0874 057c 077c 0583 027d 097c  ...}.t.|.|...}.|
-00006610: 0373 747c 0873 4e7c 0972 7474 06a0 0764  .st|.sN|.rtt...d
-00006620: 017c 0717 0064 0217 0074 087c 0883 0117  .|...d...t.|....
-00006630: 0064 0317 0074 087c 0983 0117 00a1 0101  .d...t.|........
-00006640: 0074 09a0 0a7c 0764 04a1 028f 427d 0a74  .t...|.d....B}.t
-00006650: 0ba0 0c7c 0764 05a1 027d 0b7c 06a0 0d7c  ...|.d...}.|...|
-00006660: 0ba1 017d 0c7c 0272 be74 0e7c 077c 047c  ...}.|.r.t.|.|.|
-00006670: 0c83 0301 0074 0e7c 077c 057c 0c7c 016b  .....t.|.|.|.|.k
-00006680: 04a0 0f74 10a1 0183 0301 0057 0035 0051  ...t.......W.5.Q
-00006690: 0052 0058 0071 2264 0053 0029 064e 7a1d  .R.X.q"d.S.).Nz.
-000066a0: 0a4b 4559 2045 5849 5354 5320 4e4f 5420  .KEY EXISTS NOT 
-000066b0: 5752 4954 5449 4e47 2046 4f52 207a 320a  WRITTING FOR z2.
-000066c0: 6f76 6572 7772 6974 655f 6966 5f65 7869  overwrite_if_exi
-000066d0: 7374 7320 6973 2046 414c 5345 0a70 726f  sts is FALSE.pro
-000066e0: 6261 5f6b 6579 2065 7869 7374 202d 2d3e  ba_key exist -->
-000066f0: 207a 160a 6c61 6265 6c5f 6b65 7920 6578   z..label_key ex
-00006700: 6973 7473 202d 2d3e 2072 a200 0000 7249  ists --> r....rI
-00006710: 0000 0029 1172 5700 0000 7205 0000 0072  ...).rW...r....r
-00006720: a800 0000 5a1d 4649 4e41 4c5f 5448 5245  ....Z.FINAL_THRE
-00006730: 5348 4f4c 445f 7769 7468 5f37 5f73 6d6f  SHOLD_with_7_smo
-00006740: 6f74 6872 4b00 0000 da0d 6835 5f6b 6579  othrK.....h5_key
-00006750: 5f65 7869 7374 7372 8b00 0000 728c 0000  _existsr....r...
-00006760: 0072 a900 0000 72aa 0000 0072 ab00 0000  .r....r....r....
-00006770: 7208 0000 0072 2801 0000 72ae 0000 0072  r....r(...r....r
-00006780: 1e01 0000 7281 0000 0072 8400 0000 290d  ....r....r....).
-00006790: 5a0a 6835 5f69 6e5f 6c69 7374 da06 7468  Z.h5_in_list..th
-000067a0: 7265 7368 da0b 7772 6974 655f 746f 5f68  resh..write_to_h
-000067b0: 35da 136f 7665 7277 7269 7465 5f69 665f  5..overwrite_if_
-000067c0: 6578 6973 7473 5a09 7072 6f62 615f 6b65  existsZ.proba_ke
-000067d0: 79da 096c 6162 656c 5f6b 6579 72b8 0000  y..label_keyr...
-000067e0: 0072 be00 0000 72f7 0000 00da 0474 6d70  .r....r......tmp
-000067f0: 3272 bc00 0000 7253 0000 0072 1f01 0000  2r....rS...r....
-00006800: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00006810: 1a6d 616b 655f 6669 6e61 6c5f 7072 6564  .make_final_pred
-00006820: 6963 7469 6f6e 735f 4742 4d02 0400 0073  ictions_GBM....s
-00006830: 3200 0000 0002 0801 0801 0801 0601 0801  2...............
-00006840: 0801 0a01 0a01 0401 0801 0401 0c01 02ff  ................
-00006850: 0401 02ff 0201 06ff 02ff 0403 0e01 0c01  ................
-00006860: 0a01 0401 0c01 726f 0100 0063 0100 0000  ......ro...c....
-00006870: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00006880: 4300 0000 73ce 0000 0074 007c 0074 0183  C...s....t.|.t..
-00006890: 0272 1c74 0264 0183 0101 0074 037c 0083  .r.t.d.....t.|..
-000068a0: 0101 006e ae74 007c 0074 0483 0272 627a  ...n.t.|.t...rbz
-000068b0: 2474 05a0 0674 07a0 087c 00a1 01a1 017d  $t...t...|.....}
-000068c0: 0074 0264 0283 0101 0074 097c 0083 0101  .t.d.....t.|....
-000068d0: 0057 0071 ca01 0001 0001 0074 0264 0383  .W.q.......t.d..
-000068e0: 0101 0059 0071 ca58 006e 6874 0a7c 0083  ...Y.q.X.nht.|..
-000068f0: 016a 0b74 076a 0c6b 0272 8474 0264 0483  .j.t.j.k.r.t.d..
-00006900: 0101 0074 097c 0083 0101 006e 467a 2474  ...t.|.....nFz$t
-00006910: 0264 0574 0d74 0a7c 0083 0183 0117 0064  .d.t.t.|.......d
-00006920: 0617 0083 0101 0074 0e7c 0083 0101 0057  .......t.|.....W
-00006930: 006e 2001 0001 0001 0074 0264 0783 0101  .n ......t.d....
-00006940: 0074 0274 0a7c 0083 0183 0101 0059 006e  .t.t.|.......Y.n
-00006950: 0258 0064 0053 0029 084e 7a0c 7479 7065  .X.d.S.).Nz.type
-00006960: 2069 7320 6469 6374 7a41 7479 7065 2069   is dictzAtype i
-00006970: 7320 6c69 7374 2c20 636f 6e76 6572 7469  s list, converti
-00006980: 6e67 2061 2063 6f70 7920 746f 206e 756d  ng a copy to num
-00006990: 7079 2061 7272 6179 2074 6f20 7072 696e  py array to prin
-000069a0: 7420 7468 6973 2069 6e66 6f7a 7074 7970  t this infozptyp
-000069b0: 6520 6973 2061 206c 6973 7420 7468 6174  e is a list that
-000069c0: 2063 616e 2774 2062 6520 636f 6e76 6572   can't be conver
-000069d0: 7465 6420 746f 2061 206e 756d 7079 2061  ted to a numpy a
-000069e0: 7272 6179 2066 6f72 2070 7269 6e74 696e  rray for printin
-000069f0: 6720 696e 666f 206f 7220 6d61 7962 6520  g info or maybe 
-00006a00: 6461 7461 2066 6f72 6d61 7420 6973 206e  data format is n
-00006a10: 6f74 2063 6f6d 7061 7469 626c 657a 1074  ot compatiblez.t
-00006a20: 7970 6520 6973 206e 7020 6172 7261 797a  ype is np arrayz
-00006a30: 0874 7970 6520 6973 207a 2b20 7769 6c6c  .type is z+ will
-00006a40: 2074 7279 2070 7269 6e74 696e 6720 7573   try printing us
-00006a50: 696e 6720 2267 6574 5f63 6c61 7373 5f69  ing "get_class_i
-00006a60: 6e66 6f32 2220 7a2b 6361 6e74 2066 696e  nfo2" z+cant fin
-00006a70: 6420 6f75 7420 7768 6174 2074 6f20 646f  d out what to do
-00006a80: 2077 6974 6820 696e 7075 7420 6f66 2074   with input of t
-00006a90: 7970 6529 0f72 0701 0000 7268 0000 0072  ype).r....rh...r
-00006aa0: 4b00 0000 da0d 6765 745f 6469 6374 5f69  K.....get_dict_i
-00006ab0: 6e66 6f72 3900 0000 721b 0000 0072 1c00  nfor9...r....r..
-00006ac0: 0000 721d 0000 0072 3800 0000 da08 6e70  ..r....r8.....np
-00006ad0: 5f73 7461 7473 7218 0100 00da 0a5f 5f6d  _statsr......__m
-00006ae0: 6f64 756c 655f 5fda 085f 5f6e 616d 655f  odule__..__name_
-00006af0: 5f72 a900 0000 da0f 6765 745f 636c 6173  _r......get_clas
-00006b00: 735f 696e 666f 3272 cd00 0000 7216 0000  s_info2r....r...
-00006b10: 0072 1600 0000 7217 0000 00da 0469 6e66  .r....r......inf
-00006b20: 6f19 0400 0073 2a00 0000 0001 0a01 0801  o....s*.........
-00006b30: 0a01 0a01 0201 1001 0801 0c01 0601 0201  ................
-00006b40: 02ff 0c03 1001 0801 0a02 0201 1801 0c01  ................
-00006b50: 0601 0801 7275 0100 00fa 1341 6d65 7269  ....ru.....Ameri
-00006b60: 6361 2f4c 6f73 5f41 6e67 656c 6573 6301  ca/Los_Angelesc.
-00006b70: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00006b80: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
-00006b90: 7c00 a101 7d01 7400 6a02 a003 7404 a005  |...}.t.j...t...
-00006ba0: a100 a101 7d02 7c02 a006 7c01 a101 7d03  ....}.|...|...}.
-00006bb0: 7c03 a007 6401 a101 7d04 7c04 5300 2902  |...d...}.|.S.).
-00006bc0: 4e7a 1125 595f 256d 5f25 645f 2548 5f25  Nz.%Y_%m_%d_%H_%
-00006bd0: 4d5f 2553 2908 da04 7079 747a da08 7469  M_%S)...pytz..ti
-00006be0: 6d65 7a6f 6e65 da03 7574 63da 086c 6f63  mezone..utc..loc
-00006bf0: 616c 697a 6572 0d00 0000 da06 7574 636e  alizer......utcn
-00006c00: 6f77 da0a 6173 7469 6d65 7a6f 6e65 da08  ow..astimezone..
-00006c10: 7374 7266 7469 6d65 2905 5a10 7469 6d65  strftime).Z.time
-00006c20: 5f7a 6f6e 655f 7374 7269 6e67 da02 747a  _zone_string..tz
-00006c30: 5a06 6c6f 635f 6474 5a0c 6375 7272 656e  Z.loc_dtZ.curren
-00006c40: 745f 7469 6d65 5a0e 746f 6461 7973 5f76  t_timeZ.todays_v
-00006c50: 6572 7369 6f6e 7216 0000 0072 1600 0000  ersionr....r....
-00006c60: 7217 0000 00da 0f67 6574 5f74 696d 655f  r......get_time_
-00006c70: 7374 7269 6e67 3204 0000 730a 0000 0000  string2...s.....
-00006c80: 010a 0110 010a 010a 0172 7f01 0000 6309  .........r....c.
-00006c90: 0000 0000 0000 0000 0000 002c 0000 0009  ...........,....
-00006ca0: 0000 0003 0000 0073 1a06 0000 7400 8300  .......s....t...
-00006cb0: 7d09 7401 6a02 a003 7401 6a02 a004 7c00  }.t.j...t.j...|.
-00006cc0: a101 a101 7d0a 7c03 6401 6b08 722a 7405  ....}.|.d.k.r*t.
-00006cd0: a006 a100 7d03 6700 6700 6700 6700 6700  ....}.g.g.g.g.g.
-00006ce0: 6700 6700 6700 6402 9c08 7d0b 6401 7d0c  g.g.g.d...}.d.}.
-00006cf0: 6403 7d0d 7c0d 9001 72c6 7407 a008 7409  d.}.|...r.t...t.
-00006d00: 7c00 6404 8302 a101 7d0e 7407 a00a 7407  |.d.....}.t...t.
-00006d10: a00b 6405 6406 8400 7c0e 4400 8301 a101  ..d.d...|.D.....
-00006d20: a101 7d0f 7c0e 7c0f 1900 7d0e 740c 7c0e  ..}.|.|...}.t.|.
-00006d30: 8301 6407 6b02 7298 740d 6408 8301 0100  ..d.k.r.t.d.....
-00006d40: 7c0c 5300 740e 7c0e 6407 1900 8301 7d10  |.S.t.|.d.....}.
-00006d50: 7401 6a02 a00f 7c0e 6407 1900 a101 7d11  t.j...|.d.....}.
-00006d60: 7c07 9001 7246 7c10 6409 1900 9001 7346  |...rF|.d.....sF
-00006d70: 7410 7c10 640a 1900 8301 4400 5d6c 5c02  t.|.d.....D.]l\.
-00006d80: 7d12 7d13 7c13 72d0 7c11 7401 6a11 1700  }.}.|.r.|.t.j...
-00006d90: 7401 6a02 a003 7c10 640b 1900 7c12 1900  t.j...|.d...|...
-00006da0: a101 1700 7d14 7c14 a012 7c0a 7c0a 640c  ....}.|...|.|.d.
-00006db0: 1700 a102 7d15 7413 7401 6a02 a00f 7c15  ....}.t.t.j...|.
-00006dc0: a101 8301 6a14 6403 6403 640d 8d02 0100  ....j.d.d.d.....
-00006dd0: 7415 a016 7c14 7c15 a102 0100 6403 7c10  t...|.|.....d.|.
-00006de0: 640e 1900 7c12 3c00 71d0 6403 7c10 6409  d...|.<.q.d.|.d.
-00006df0: 3c00 7417 7c00 7401 6a02 a004 7c00 a101  <.t.|.t.j...|...
-00006e00: 640f 1700 8302 0100 7407 a018 7c10 640e  d.......t...|.d.
-00006e10: 1900 6403 6b02 a101 9001 72c0 7c0e 6407  ..d.k.....r.|.d.
-00006e20: 1900 7d14 7415 a016 7c14 7c14 a012 7c0a  ..}.t...|.|...|.
-00006e30: 7c0a 640f 1700 a102 a102 0100 7401 6a02  |.d.........t.j.
-00006e40: a00f 7c14 a101 7401 6a11 1700 6410 1700  ..|...t.j...d...
-00006e50: 7d14 7415 a016 7c14 7c14 a012 7c0a 7c0a  }.t...|.|...|.|.
-00006e60: 640f 1700 a102 a102 0100 7148 6411 7d0d  d.........qHd.}.
-00006e70: 7148 7419 a019 a100 7d16 7c16 6701 7d17  qHt.....}.|.g.}.
-00006e80: 7401 6a02 a01a 7c01 a101 9001 72ec 7415  t.j...|.....r.t.
-00006e90: a01b 7c01 a101 0100 7413 7c01 8301 6a14  ..|.....t.|...j.
-00006ea0: 6403 6403 640d 8d02 0100 7401 6a11 6410  d.d.d.....t.j.d.
-00006eb0: 1700 7d14 7c01 7c14 1700 7d18 7415 a01c  ..}.|.|...}.t...
-00006ec0: 7c11 7c14 1700 7c18 a102 0100 7407 a01d  |.|...|.....t...
-00006ed0: 7c10 640e 1900 6411 6b02 a101 6407 1900  |.d...d.k...d...
-00006ee0: 6401 7c02 8502 1900 7d19 7c19 4400 5d34  d.|.....}.|.D.]4
-00006ef0: 7d1a 7401 6a11 7401 6a02 a003 7c10 640b  }.t.j.t.j...|.d.
-00006f00: 1900 7c1a 1900 a101 1700 7d14 7415 a01c  ..|.......}.t...
-00006f10: 7c11 7c14 1700 7c01 7c14 1700 a102 0100  |.|...|.|.......
-00006f20: 9002 7142 7c17 a01e 7419 a019 a100 a101  ..qB|...t.......
-00006f30: 0100 741f 7c01 7c18 7c06 7c08 6412 8d04  ..t.|.|.|.|.d...
-00006f40: 7d1b 7c1b a020 a100 0100 7c17 a01e 7419  }.|.. ....|...t.
-00006f50: a019 a100 a101 0100 7c1b 6a21 7d1c 7c1c  ........|.j!}.|.
-00006f60: a012 6413 6414 a102 7d1d 7422 a023 7c1c  ..d.d...}.t".#|.
-00006f70: 7c1d a102 0100 7c17 a01e 7419 a019 a100  |.....|...t.....
-00006f80: a101 0100 7c1d a012 6413 6415 a102 7d1e  ....|...d.d...}.
-00006f90: 7422 6a24 6416 7c1d 6417 6418 8d03 7d1f  t"j$d.|.d.d...}.
-00006fa0: 7425 7c03 7c1f 7c1e 8303 0100 7c17 a01e  t%|.|.|.....|...
-00006fb0: 7419 a019 a100 a101 0100 7426 7c19 6407  t.........t&|.d.
-00006fc0: 1900 6419 1700 8301 641a 1700 7426 7c19  ..d.....d...t&|.
-00006fd0: 641b 1900 6419 1700 8301 1700 641c 1700  d...d.......d...
-00006fe0: 7426 740c 7c10 640e 1900 8301 8301 1700  t&t.|.d.........
-00006ff0: 7d20 7c1c a012 6413 641d 7c20 1700 6413  } |...d.d.| ..d.
-00007000: 1700 a102 7d21 7427 7c1e 7c21 6403 6403  ....}!t'|.|!d.d.
-00007010: 641e 8d04 0100 7422 a028 7c1e 641f a102  d.....t".(|.d...
-00007020: a029 a100 7d22 742a 7c21 641f 7c22 8303  .)..}"t*|!d.|"..
-00007030: 0100 7c17 a01e 7419 a019 a100 a101 0100  ..|...t.........
-00007040: 742b 7c1c 7c21 8302 0100 7c04 9003 72be  t+|.|!....|...r.
-00007050: 7422 a028 7c1d 6420 a102 7d23 742a 7c21  t".(|.d ..}#t*|!
-00007060: 6420 7c23 8303 0100 7e23 7401 a02c 7c1d  d |#....~#t..,|.
-00007070: a101 0100 7c05 9003 72e8 7422 a028 7c1e  ....|...r.t".(|.
-00007080: 6421 a102 7d24 742a 7c21 6421 7c24 8303  d!..}$t*|!d!|$..
-00007090: 0100 7e24 7401 a02c 7c1e a101 0100 7401  ..~$t..,|.....t.
-000070a0: 6a02 a00f 7c0e 6407 1900 a101 7401 6a11  j...|.d.....t.j.
-000070b0: 1700 7d14 7c14 a012 7c0a 7c0a 640f 1700  ..}.|...|.|.d...
-000070c0: a102 7401 6a02 a003 7c21 a101 1700 7d25  ..t.j...|!....}%
-000070d0: 7415 a01c 7c21 7c25 a102 0100 7c19 4400  t...|!|%....|.D.
-000070e0: 5d12 7d26 6403 7c10 640e 1900 7c26 3c00  ].}&d.|.d...|&<.
-000070f0: 9004 7134 742d 7c10 7c0e 6407 1900 8302  ..q4t-|.|.d.....
-00007100: 0100 7c19 4400 5d5a 7d1a 7c11 7401 6a11  ..|.D.]Z}.|.t.j.
-00007110: 1700 7401 6a02 a003 7c10 640b 1900 7c1a  ..t.j...|.d...|.
-00007120: 1900 a101 1700 7d14 7c14 a012 7c0a 7c0a  ......}.|...|.|.
-00007130: 6422 1700 a102 7d27 7413 7401 6a02 a00f  d"....}'t.t.j...
-00007140: 7c27 a101 8301 6a14 6403 6403 640d 8d02  |'....j.d.d.d...
-00007150: 0100 7415 a016 7c14 7c27 a102 0100 9004  ..t...|.|'......
-00007160: 715a 7c17 a01e 7419 a019 a100 a101 0100  qZ|...t.........
-00007170: 7407 a02e 7c17 a101 7d28 6423 6424 6425  t...|...}(d#d$d%
-00007180: 6426 6427 6428 6429 6707 7d29 642a 742f  d&d'd(d)g.})d*t/
-00007190: 642b 642c 8400 7c29 4400 8301 8301 1400  d+d,..|)D.......
-000071a0: 8900 740d 642d 8301 0100 642e a030 8700  ..t.d-....d..0..
-000071b0: 6601 642f 6406 8408 7431 7c28 7c29 7c28  f.d/d...t1|(|)|(
-000071c0: 740c 7c19 8301 1b00 8303 4400 8301 a101  t.|.......D.....
-000071d0: 7d2a 740d 7c2a 8301 0100 740d 6430 8301  }*t.|*....t.d0..
-000071e0: 0100 740d 8800 7426 7432 7433 7407 a034  ..t...t&t2t3t..4
-000071f0: 7c28 a101 8301 6431 8d01 8301 a035 6432  |(....d1.....5d2
-00007200: a101 6407 1900 1700 6433 1700 7426 7432  ..d.....d3..t&t2
-00007210: 7407 a034 7c28 a101 740c 7c19 8301 1b00  t..4|(..t.|.....
-00007220: 6431 8d01 8301 a035 6432 a101 6407 1900  d1.....5d2..d...
-00007230: 1700 8301 0100 7407 a036 7c28 740c 7c19  ......t..6|(t.|.
-00007240: 8301 6701 6602 a101 7d28 7c0c 6401 6b08  ..g.f...}(|.d.k.
-00007250: 9005 72c4 7437 6a38 7c28 6401 6401 6401  ..r.t7j8|(d.d.d.
-00007260: 8502 6602 1900 7c29 6434 8d02 7d0c 6e28  ..f...|)d4..}.n(
-00007270: 7437 6a38 7c28 6401 6401 6401 8502 6602  t7j8|(d.d.d...f.
-00007280: 1900 7c29 6434 8d02 7d2b 7c0c 6a1e 7c2b  ..|)d4..}+|.j.|+
-00007290: 6403 6435 8d02 7d0c 742d 7c0c 7401 6a02  d.d5..}.t-|.t.j.
-000072a0: a004 7c00 a101 640f 1700 7401 6a11 1700  ..|...d...t.j...
-000072b0: 6436 1700 7c09 1700 6437 1700 8302 0100  d6..|...d7......
-000072c0: 7144 6401 5300 2938 61e3 0100 000a 2020  qDd.S.)8a.....  
-000072d0: 2020 7573 6520 7574 696c 732e 6d61 6b65    use utils.make
-000072e0: 5f6d 7034 5f6c 6973 745f 6469 6374 2074  _mp4_list_dict t
-000072f0: 6f20 6d61 6b65 206c 6973 7473 206f 6620  o make lists of 
-00007300: 7468 6520 6d70 3420 6669 6c65 7320 6669  the mp4 files fi
-00007310: 7273 742c 2069 7420 6361 6e20 6265 2072  rst, it can be r
-00007320: 756e 206f 6e20 7468 6520 6d61 7374 6572  un on the master
-00007330: 2064 6972 6563 746f 7279 2061 6e64 2077   directory and w
-00007340: 696c 6c20 696e 6465 7820 616c 6c20 666f  ill index all fo
-00007350: 6c64 6572 7320 7769 7468 204d 5034 2066  lders with MP4 f
-00007360: 696c 6573 0a20 2020 2050 6172 616d 6574  iles.    Paramet
-00007370: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00007380: 2d2d 0a20 2020 2062 6420 3a0a 2020 2020  --.    bd :.    
-00007390: 6c6f 6361 6c5f 7465 6d70 5f64 6972 203a  local_temp_dir :
-000073a0: 0a20 2020 2076 6964 656f 5f62 6174 6368  .    video_batch
-000073b0: 5f73 697a 6520 3a0a 2020 2020 5245 534e  _size :.    RESN
-000073c0: 4554 5f4d 4f44 454c 203a 0a20 2020 2063  ET_MODEL :.    c
-000073d0: 6f70 795f 696d 6167 655f 6669 6c65 735f  opy_image_files_
-000073e0: 746f 5f66 696e 616c 5f68 3520 3a0a 2020  to_final_h5 :.  
-000073f0: 2020 636f 7079 5f66 6561 7475 7265 5f64    copy_feature_d
-00007400: 6174 615f 746f 5f66 696e 616c 5f68 3520  ata_to_final_h5 
-00007410: 3a20 636f 7079 2074 6865 2032 3034 3820  : copy the 2048 
-00007420: 6f72 6967 696e 616c 2066 6561 7475 7265  original feature
-00007430: 2064 6174 6120 746f 2074 6865 2066 696e   data to the fin
-00007440: 616c 2048 352c 206f 6e6c 7920 6e65 6564  al H5, only need
-00007450: 6564 2066 6f72 206d 6f64 656c 2074 6573  ed for model tes
-00007460: 7469 6e67 2061 6e64 2062 7569 6c64 696e  ting and buildin
-00007470: 670a 2020 2020 6375 7374 6f6d 5f69 6d61  g.    custom_ima
-00007480: 6765 5f65 7874 7261 6374 5f73 697a 6520  ge_extract_size 
-00007490: 3a0a 0a20 2020 2052 6574 7572 6e73 0a20  :..    Returns. 
-000074a0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-000074b0: 4e29 085a 096e 756d 5f66 696c 6573 5a12  N).Z.num_filesZ.
-000074c0: 7469 6d65 5f63 6f70 795f 746f 5f6c 6f63  time_copy_to_loc
-000074d0: 616c 5a08 7469 6d65 5f61 6c6c 5a0d 7469  alZ.time_allZ.ti
-000074e0: 6d65 5f74 6f5f 7472 6163 6b5a 0c74 696d  me_to_trackZ.tim
-000074f0: 655f 746f 5f33 6c61 675a 1074 696d 655f  e_to_3lagZ.time_
-00007500: 746f 5f66 6561 7475 7265 735a 1474 696d  to_featuresZ.tim
-00007510: 655f 746f 5f61 6c6c 5f66 6561 7475 7265  e_to_all_feature
-00007520: 735a 1474 696d 655f 746f 5f63 7574 5f66  sZ.time_to_cut_f
-00007530: 6561 7475 7265 7354 fa23 2a66 696c 655f  eaturesT.#*file_
-00007540: 6c69 7374 5f66 6f72 5f62 6174 6368 5f70  list_for_batch_p
-00007550: 726f 6365 7373 696e 672e 706b 6c63 0100  rocessing.pklc..
-00007560: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00007570: 0000 5300 0000 7318 0000 0067 007c 005d  ..S...s....g.|.]
-00007580: 107d 0174 006a 01a0 027c 01a1 0191 0271  .}.t.j...|.....q
-00007590: 0453 0072 1600 0000 2903 725f 0000 0072  .S.r....).r_...r
-000075a0: 6100 0000 da08 6765 7463 7469 6d65 7231  a.....getctimer1
-000075b0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000075c0: 0000 7234 0000 005f 0400 0073 0400 0000  ..r4..._...s....
-000075d0: 0600 0200 7a31 6261 7463 685f 7072 6f63  ....z1batch_proc
-000075e0: 6573 735f 7669 6465 6f73 5f6f 6e5f 636f  ess_videos_on_co
-000075f0: 6c61 622e 3c6c 6f63 616c 733e 2e3c 6c69  lab.<locals>.<li
-00007600: 7374 636f 6d70 3e72 0100 0000 7a13 4649  stcomp>r....z.FI
-00007610: 4e49 5348 4544 2050 524f 4345 5353 494e  NISHED PROCESSIN
-00007620: 47da 1862 6164 5f76 6964 735f 6861 7665  G..bad_vids_have
-00007630: 5f62 6565 6e5f 6d6f 7665 64da 1646 5053  _been_moved..FPS
-00007640: 5f63 6865 636b 5f62 6164 5f76 6964 5f69  _check_bad_vid_i
-00007650: 6e64 73da 096d 7034 5f6e 616d 6573 5a09  nds..mp4_namesZ.
-00007660: 5f42 4144 5f4d 5034 7372 5c01 0000 da0c  _BAD_MP4sr\.....
-00007670: 6973 5f70 726f 6365 7373 6564 5a09 5f46  is_processedZ._F
-00007680: 494e 4953 4845 447a 1074 656d 706c 6174  INISHEDz.templat
-00007690: 655f 696d 672e 706e 6746 2904 729c 0000  e_img.pngF).r...
-000076a0: 0072 9d00 0000 da19 6375 7374 6f6d 5f69  .r......custom_i
-000076b0: 6d61 6765 5f65 7874 7261 6374 5f73 697a  mage_extract_siz
-000076c0: 6572 9f00 0000 72a0 0000 0072 a100 0000  er....r....r....
-000076d0: 7a10 5f66 6561 7475 7265 5f64 6174 612e  z._feature_data.
-000076e0: 6835 69f4 0100 0072 5200 0000 2901 726d  h5i....rR...).rm
-000076f0: 0100 0072 2e00 0000 5a04 5f74 6f5f 724a  ...r....Z._to_rJ
-00007700: 0000 005a 045f 6f66 5f5a 125f 6669 6e61  ...Z._of_Z._fina
-00007710: 6c5f 746f 5f63 6f6d 6269 6e65 5f29 035a  l_to_combine_).Z
-00007720: 1077 7269 7465 5f74 6f5f 7468 6973 5f68  .write_to_this_h
-00007730: 355a 1177 7269 7465 5f66 696e 616c 5f74  5Z.write_final_t
-00007740: 6f5f 6835 5a0e 6465 6c65 7465 5f74 656d  o_h5Z.delete_tem
-00007750: 705f 6835 7256 0100 0072 9600 0000 7255  p_h5rV...r....rU
-00007760: 0100 005a 0e5f 4649 4e49 5348 4544 5f4d  ...Z._FINISHED_M
-00007770: 5034 737a 1263 6f70 7920 6d70 3473 2074  P4sz.copy mp4s t
-00007780: 6f20 6c6f 6361 6c7a 0e74 7261 636b 2074  o localz.track t
-00007790: 6865 2070 6f6c 657a 0f63 6f6e 7665 7274  he polez.convert
-000077a0: 2074 6f20 336c 6167 7a19 6372 6561 7465   to 3lagz.create
-000077b0: 2066 6561 7475 7265 2064 6174 6120 2843   feature data (C
-000077c0: 4e4e 297a 1565 6e67 696e 6565 7220 616c  NN)z.engineer al
-000077d0: 6c20 6665 6174 7572 6573 7a26 636f 7079  l featuresz&copy
-000077e0: 2020 6835 2061 6e64 206d 7034 7320 746f    h5 and mp4s to
-000077f0: 2066 696e 616c 2064 6573 7469 6e61 7469   final destinati
-00007800: 6f6e 7a0f 6e75 6d62 6572 206f 6620 6669  onz.number of fi
-00007810: 6c65 73fa 0120 6301 0000 0000 0000 0000  les.. c.........
-00007820: 0000 0002 0000 0003 0000 0073 0000 0073  ...........s...s
-00007830: 1a00 0000 7c00 5d12 7d01 7400 7c01 8301  ....|.].}.t.|...
-00007840: 6400 1700 5600 0100 7102 6401 5300 2902  d...V...q.d.S.).
-00007850: 72d5 0000 004e 7248 0000 0072 3100 0000  r....NrH...r1...
-00007860: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00007870: d400 0000 e804 0000 7304 0000 0004 0002  ........s.......
-00007880: 007a 3062 6174 6368 5f70 726f 6365 7373  .z0batch_process
-00007890: 5f76 6964 656f 735f 6f6e 5f63 6f6c 6162  _videos_on_colab
-000078a0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000078b0: 7072 3e7a 3c6f 7065 7261 7469 6f6e 2020  pr>z<operation  
-000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000078e0: 6f74 616c 2020 2020 2070 6572 2066 696c  otal     per fil
-000078f0: 6572 d000 0000 6301 0000 0000 0000 0000  er....c.........
-00007900: 0000 0004 0000 0007 0000 0013 0000 0073  ...............s
-00007910: 5e00 0000 6700 7c00 5d56 5c03 7d01 7d02  ^...g.|.]V\.}.}.
-00007920: 7d03 7c02 8800 1700 6400 7400 8800 8301  }.|.....d.t.....
-00007930: 8502 1900 7401 7402 7c01 6401 8d01 8301  ....t.t.|.d.....
-00007940: a003 6402 a101 6403 1900 1700 6404 1700  ..d...d.....d...
-00007950: 7401 7402 7c03 6401 8d01 8301 a003 6402  t.t.|.d.......d.
-00007960: a101 6403 1900 1700 6405 1700 9102 7104  ..d.....d.....q.
-00007970: 5300 2906 4ea9 01da 0773 6563 6f6e 6473  S.).N....seconds
-00007980: 721d 0100 0072 0100 0000 fa03 2020 20da  r....r......   .
-00007990: 010a 2904 7230 0000 0072 a900 0000 720c  ..).r0...r....r.
-000079a0: 0000 0072 d700 0000 2904 7232 0000 0072  ...r....).r2...r
-000079b0: 3300 0000 72ba 0000 00da 026b 33a9 01da  3...r......k3...
-000079c0: 096c 656e 5f73 7061 6365 7216 0000 0072  .len_spacer....r
-000079d0: 1700 0000 7234 0000 00ea 0400 0073 1400  ....r4.......s..
-000079e0: 0000 0601 08ff 2401 02ff 0401 02ff 0201  ......$.........
-000079f0: 16ff 0201 02ff 7a3c 544f 5441 4c20 2020  ......z<TOTAL   
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 746f 7461 6c20 2020 2020 7065 7220    total     per 
-00007a30: 6669 6c65 7288 0100 0072 1d01 0000 728a  filer....r....r.
-00007a40: 0100 0029 01da 0763 6f6c 756d 6e73 2901  ...)...columns).
-00007a50: 5a0c 6967 6e6f 7265 5f69 6e64 6578 5a08  Z.ignore_indexZ.
-00007a60: 7469 6d65 5f64 665f fa04 2e70 6b6c 2939  time_df_...pkl)9
-00007a70: 727f 0100 0072 5f00 0000 7261 0000 0072  r....r_...ra...r
-00007a80: a400 0000 da08 6e6f 726d 7061 7468 7205  ......normpathr.
-00007a90: 0000 005a 106c 6f61 645f 6669 6e61 6c5f  ...Z.load_final_
-00007aa0: 6d6f 6465 6c72 1d00 0000 7238 0000 00da  modelr....r8....
-00007ab0: 0967 6574 5f66 696c 6573 da04 666c 6970  .get_files..flip
-00007ac0: 7286 0000 0072 3000 0000 724b 0000 0072  r....r0...rK...r
-00007ad0: 6300 0000 72a3 0000 0072 2400 0000 7260  c...r....r$...r`
-00007ae0: 0000 0072 b300 0000 720e 0000 0072 5f01  ...r....r....r_.
-00007af0: 0000 7273 0000 00da 046d 6f76 65da 1563  ..rs.....move..c
-00007b00: 6f70 795f 666f 6c64 6572 5f73 7472 7563  opy_folder_struc
-00007b10: 7475 7265 722f 0000 00da 0474 696d 65da  turer/.....time.
-00007b20: 0665 7869 7374 7372 7400 0000 721b 0000  .existsrt...r...
-00007b30: 0072 b500 0000 7223 0000 0072 0400 0000  .r....r#...r....
-00007b40: 5a13 7472 6163 6b5f 616c 6c5f 616e 645f  Z.track_all_and_
-00007b50: 7361 7665 6a72 b200 0000 7208 0000 0072  savejr....r....r
-00007b60: b400 0000 5a13 496d 6167 6542 6174 6368  ....Z.ImageBatch
-00007b70: 4765 6e65 7261 746f 7272 0200 0000 72a9  Generatorr....r.
-00007b80: 0000 0072 0300 0000 7228 0100 0072 f500  ...r....r(...r..
-00007b90: 0000 721e 0100 00da 1c63 6f70 795f 6f76  ..r......copy_ov
-00007ba0: 6572 5f61 6c6c 5f6e 6f6e 5f69 6d61 6765  er_all_non_image
-00007bb0: 5f6b 6579 7372 7900 0000 da08 7361 7665  _keysry.....save
-00007bc0: 5f6f 626a da04 6469 6666 720f 0100 0072  _obj..diffr....r
-00007bd0: d600 0000 72ac 0000 0072 0c00 0000 7284  ....r....r....r.
-00007be0: 0000 0072 3500 0000 72d7 0000 0072 2600  ...r5...r....r&.
-00007bf0: 0000 da02 7064 5a09 4461 7461 4672 616d  ....pdZ.DataFram
-00007c00: 6529 2c72 6400 0000 5a0e 6c6f 6361 6c5f  e),rd...Z.local_
-00007c10: 7465 6d70 5f64 6972 5a10 7669 6465 6f5f  temp_dirZ.video_
-00007c20: 6261 7463 685f 7369 7a65 5a0c 5245 534e  batch_sizeZ.RESN
-00007c30: 4554 5f4d 4f44 454c 5a1c 636f 7079 5f69  ET_MODELZ.copy_i
-00007c40: 6d61 6765 5f66 696c 6573 5f74 6f5f 6669  mage_files_to_fi
-00007c50: 6e61 6c5f 6835 5a1d 636f 7079 5f66 6561  nal_h5Z.copy_fea
-00007c60: 7475 7265 5f64 6174 615f 746f 5f66 696e  ture_data_to_fin
-00007c70: 616c 5f68 3572 8601 0000 5a16 736b 6970  al_h5r....Z.skip
-00007c80: 5f69 665f 4650 535f 6973 5f6e 6f74 5f69  _if_FPS_is_not_i
-00007c90: 6e74 729f 0000 005a 0874 696d 655f 7374  ntr....Z.time_st
-00007ca0: 725a 0c62 645f 6261 7365 5f6e 616d 655a  rZ.bd_base_nameZ
-00007cb0: 0974 696d 655f 6469 6374 5a07 7469 6d65  .time_dictZ.time
-00007cc0: 5f64 665a 0e67 7261 625f 6669 6c65 5f6c  _dfZ.grab_file_l
-00007cd0: 6973 745a 126c 6973 745f 6f66 5f66 696c  istZ.list_of_fil
-00007ce0: 655f 6469 6374 7372 2b00 0000 da09 6669  e_dictsr+.....fi
-00007cf0: 6c65 5f64 6963 7472 3501 0000 5a05 6261  le_dictr5...Z.ba
-00007d00: 645f 695a 0669 735f 6261 6472 5300 0000  d_iZ.is_badrS...
-00007d10: 5a0b 6261 645f 6d70 345f 6469 72da 0573  Z.bad_mp4_dir..s
-00007d20: 7461 7274 5a09 7469 6d65 5f6c 6973 745a  tartZ.time_listZ
-00007d30: 0c74 656d 706c 6174 655f 6469 725a 1470  .template_dirZ.p
-00007d40: 726f 6365 7373 5f74 6865 7365 5f76 6964  rocess_these_vid
-00007d50: 656f 7372 2c00 0000 5a02 5054 72be 0000  eosr,...Z.PTr...
-00007d60: 0072 bf00 0000 5a0f 6835 5f66 6561 7475  .r....Z.h5_featu
-00007d70: 7265 5f64 6174 615a 0669 6e5f 6765 6e5a  re_dataZ.in_genZ
-00007d80: 0966 696c 655f 6e75 6d73 5a08 6835 5f66  .file_numsZ.h5_f
-00007d90: 696e 616c 7256 0100 0072 9600 0000 7255  inalrV...r....rU
-00007da0: 0100 0072 7c00 0000 7233 0000 005a 0d66  ...r|...r3...Z.f
-00007db0: 696e 616c 5f6d 7034 5f64 6972 5a0a 7469  inal_mp4_dirZ.ti
-00007dc0: 6d65 5f61 7272 6179 5a0c 6466 5f6e 616d  me_arrayZ.df_nam
-00007dd0: 655f 6c69 7374 5a08 746f 5f70 7269 6e74  e_listZ.to_print
-00007de0: 5a06 746d 705f 6466 7216 0000 0072 8d01  Z.tmp_dfr....r..
-00007df0: 0000 7217 0000 00da 1d62 6174 6368 5f70  ..r......batch_p
-00007e00: 726f 6365 7373 5f76 6964 656f 735f 6f6e  rocess_videos_on
-00007e10: 5f63 6f6c 6162 3a04 0000 73ec 0000 0000  _colab:...s.....
-00007e20: 1506 0114 0208 0108 010a 0102 0002 0002  ................
-00007e30: ff06 0204 0304 0106 0210 031a 0108 010c  ................
-00007e40: 0108 0104 030c 0210 0210 0214 0104 011e  ................
-00007e50: 0110 011a 020c 010e 0108 0316 0214 0108  ................
-00007e60: 0118 0116 011a 0206 0108 0106 020e 010a  ................
-00007e70: 0112 020a 0108 0110 011e 0208 011a 0118  ................
-00007e80: 010e 0306 0102 0102 fe06 0408 010e 0306  ................
-00007e90: 010c 010c 010e 040c 0110 010c 010e 0f28  ...............(
-00007ea0: 010a ff06 0214 0208 0102 ff06 0210 010c  ................
-00007eb0: 020e 060a 0206 010c 010c 0102 030a 0406  ................
-00007ec0: 010c 010c 0102 010a 0116 011c 010c 0208  ................
-00007ed0: 0110 010e 0308 011e 0110 011a 0110 010e  ................
-00007ee0: 020a 0108 0102 0002 0102 fe04 0416 0108  ................
-00007ef0: 010e 0212 fe08 0308 0108 012a 0124 ff06  ...........*.$..
-00007f00: 0314 010a 011c 021a 010e 0172 9e01 0000  ...........r....
-00007f10: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00007f20: 0006 0000 0043 0000 0073 6000 0000 7400  .....C...s`...t.
-00007f30: 7c00 6401 8302 7d02 7c02 4400 5d4c 7d03  |.d...}.|.D.]L}.
-00007f40: 7401 7c03 8301 7d04 7402 a003 7c04 6402  t.|...}.t...|.d.
-00007f50: 1900 6403 6b02 a101 720e 7404 7400 7405  ..d.k...r.t.t.t.
-00007f60: 6a06 a007 7c03 a101 6404 8302 8301 7d05  j...|...d.....}.
-00007f70: 7408 7c05 8301 6405 6b04 720e 7409 7c05  t.|...d.k.r.t.|.
-00007f80: 7c01 6406 8d02 0100 710e 6407 5300 2908  |.d.....q.d.S.).
-00007f90: 613b 0100 000a 0a20 2020 2050 6172 616d  a;.....    Param
-00007fa0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00007fb0: 2d2d 2d2d 0a20 2020 2062 6420 3a20 6a75  ----.    bd : ju
-00007fc0: 7374 2070 7574 2079 6f75 7220 6261 7365  st put your base
-00007fd0: 2064 6972 6563 746f 7279 2c20 6974 2077   directory, it w
-00007fe0: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
-00007ff0: 7920 6c6f 6164 2074 6865 2070 6b6c 2066  y load the pkl f
-00008000: 696c 6520 616e 6420 6368 6563 6b20 6966  ile and check if
-00008010: 2061 6c6c 2074 6865 2076 6964 656f 7320   all the videos 
-00008020: 6172 6520 7072 6f63 6573 7365 640a 2020  are processed.  
-00008030: 2020 6966 2074 6861 7420 6973 2074 6865    if that is the
-00008040: 2063 6173 6520 6974 2077 696c 6c20 636f   case it will co
-00008050: 6d62 696e 6520 7468 656d 2061 6e64 2062  mbine them and b
-00008060: 7920 6465 6661 756c 740a 2020 2020 6465  y default.    de
-00008070: 6c65 7465 5f65 7874 7261 5f66 696c 6573  lete_extra_files
-00008080: 203a 2064 656c 6574 6520 7468 6520 6669   : delete the fi
-00008090: 6c65 7320 6166 7465 7220 636f 6d62 696e  les after combin
-000080a0: 696e 6720 7468 6520 6669 6e61 6c20 6f6e  ing the final on
-000080b0: 652e 0a20 2020 2052 6574 7572 6e73 0a20  e..    Returns. 
-000080c0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-000080d0: 7280 0100 0072 8501 0000 547a 142a 5f66  r....r....Tz.*_f
-000080e0: 696e 616c 5f74 6f5f 636f 6d62 696e 655f  inal_to_combine_
-000080f0: 2a72 0100 0000 2901 da12 6465 6c65 7465  *r....)...delete
-00008100: 5f65 7874 7261 5f66 696c 6573 4e29 0a72  _extra_filesN).r
-00008110: 9201 0000 7263 0000 0072 1d00 0000 722f  ....rc...r....r/
-00008120: 0000 0072 6101 0000 725f 0000 0072 6100  ...ra...r_...ra.
-00008130: 0000 72a3 0000 0072 3000 0000 da11 636f  ..r....r0.....co
-00008140: 6d62 696e 655f 6669 6e61 6c5f 6835 7329  mbine_final_h5s)
-00008150: 0672 6400 0000 729f 0100 005a 1166 696e  .rd...r....Z.fin
-00008160: 6973 6865 645f 7365 7373 696f 6e73 da01  ished_sessions..
-00008170: 6672 9c01 0000 da17 6835 5f66 696c 655f  fr......h5_file_
-00008180: 6c69 7374 5f74 6f5f 636f 6d62 696e 6572  list_to_combiner
-00008190: 1600 0000 7216 0000 0072 1700 0000 da16  ....r....r......
-000081a0: 6175 746f 5f63 6f6d 6269 6e65 5f66 696e  auto_combine_fin
-000081b0: 616c 5f68 3573 5a05 0000 730e 0000 0000  al_h5sZ...s.....
-000081c0: 0c0a 0108 0108 0112 0116 010c 0172 a301  .............r..
-000081d0: 0000 6302 0000 0000 0000 0000 0000 000e  ..c.............
-000081e0: 0000 000d 0000 0043 0000 0073 1603 0000  .......C...s....
-000081f0: 7400 7c00 8301 7d00 7c00 6401 1900 a001  t.|...}.|.d.....
-00008200: 6402 a101 6401 1900 6403 1700 7d02 7402  d...d...d...}.t.
-00008210: 6a03 7c02 6404 6405 6406 6404 6407 6407  j.|.d.d.d.d.d.d.
-00008220: 6407 7404 6a05 6a06 7404 6a05 6a06 6408  d.t.j.j.t.j.j.d.
-00008230: 6409 8d0b 7d03 7407 7c00 8301 4400 5d48  d...}.t.|...D.]H
-00008240: 7d04 7404 a008 7c04 640a a102 8f32 7d05  }.t...|.d....2}.
-00008250: 7c05 6408 1900 6400 6400 8502 1900 7d06  |.d...d.d.....}.
-00008260: 7c03 a009 7c06 740a a00b 7c06 6a0c 6401  |...|.t...|.j.d.
-00008270: 1900 a101 640b 1400 a102 0100 5700 3500  ....d.......W.5.
-00008280: 5100 5200 5800 714e 7404 a008 7c02 640c  Q.R.X.qNt...|.d.
-00008290: a102 9001 8f6a 7d05 7c05 640d 3d00 740d  .....j}.|.d.=.t.
-000082a0: 7c00 6401 1900 640e 8302 9001 725c 740e  |.d...d.....r\t.
-000082b0: 7407 7c00 8301 8301 4400 5d90 5c02 7d07  t.|.....D.].\.}.
-000082c0: 7d04 7402 a00f 7c04 640e a102 7d08 7c07  }.t...|.d...}.|.
-000082d0: 6401 6b02 9001 721c 7410 7c08 6a0c 8301  d.k...r.t.|.j...
-000082e0: 7d09 6400 7c09 6401 3c00 7c05 6a11 640e  }.d.|.d.<.|.j.d.
-000082f0: 740a a00c 7c08 a101 7404 6a05 6a12 7c09  t...|...t.j.j.|.
-00008300: 6404 7c08 640f 8d06 0100 71ca 7c05 640e  d.|.d.....q.|.d.
-00008310: 1900 6a13 7c05 640e 1900 6a0c 6401 1900  ..j.|.d...j.d...
-00008320: 7c08 6a0c 6401 1900 1700 6401 6410 8d02  |.j.d.....d.d...
-00008330: 0100 7c08 7c05 640e 1900 7c08 6a0c 6401  ..|.|.d...|.j.d.
-00008340: 1900 0b00 6400 8502 3c00 71ca 740d 7c00  ....d...<.q.t.|.
-00008350: 6401 1900 6411 8302 9002 720c 740e 7407  d...d.....r.t.t.
-00008360: 7c00 8301 8301 4400 5d92 5c02 7d07 7d04  |.....D.].\.}.}.
-00008370: 7402 a00f 7c04 6411 a102 7d0a 7c07 6401  t...|.d...}.|.d.
-00008380: 6b02 9001 72ca 7410 7c0a 6a0c 8301 7d09  k...r.t.|.j...}.
-00008390: 6400 7c09 6401 3c00 7c05 6a11 6411 740a  d.|.d.<.|.j.d.t.
-000083a0: a00c 7c0a a101 7404 6a05 6a12 7c09 6404  ..|...t.j.j.|.d.
-000083b0: 7c0a 640f 8d06 0100 6e3e 7c05 6411 1900  |.d.....n>|.d...
-000083c0: 6a13 7c05 6411 1900 6a0c 6401 1900 7c0a  j.|.d...j.d...|.
-000083d0: 6a0c 6401 1900 1700 6401 6410 8d02 0100  j.d.....d.d.....
-000083e0: 7c0a 7c05 6411 1900 7c0a 6a0c 6401 1900  |.|.d...|.j.d...
-000083f0: 0b00 6400 8502 3c00 9001 7178 5700 3500  ..d...<...qxW.5.
-00008400: 5100 5200 5800 6412 6413 6414 6415 640d  Q.R.X.d.d.d.d.d.
-00008410: 6416 6417 6418 6419 6709 7d0b 6700 7d0c  d.d.d.d.g.}.g.}.
-00008420: 7c00 4400 5d1c 7d04 7c0c a014 7402 a00f  |.D.].}.|...t...
-00008430: 7415 7c04 8301 641a a102 a101 0100 9002  t.|...d.........
-00008440: 7134 740a a016 7c0c a101 7d0c 7417 7c02  q4t...|...}.t.|.
-00008450: 641a 7c0c 8303 0100 7404 a008 7c02 640c  d.|.....t...|.d.
-00008460: a102 8f4c 7d05 7407 7c0b 8301 4400 5d3c  ...L}.t.|...D.]<
-00008470: 7d04 740d 7c00 6401 1900 7c04 8302 9002  }.t.|.d...|.....
-00008480: 727e 7402 a00f 7c00 7c04 a102 7d0d 7c04  r~t...|.|...}.|.
-00008490: 6414 6b02 9002 72b0 7410 7c0d 8301 7d0d  d.k...r.t.|...}.
-000084a0: 7c0d 7c05 7c04 3c00 9002 717e 5700 3500  |.|.|.<...q~W.5.
-000084b0: 5100 5200 5800 7417 7c02 641b 7402 a00f  Q.R.X.t.|.d.t...
-000084c0: 7c00 6401 1900 641b a102 8303 0100 7417  |.d...d.......t.
-000084d0: 7c02 641c 7402 a00f 7c00 6401 1900 641c  |.d.t...|.d...d.
-000084e0: a102 8303 0100 7c01 9003 7212 7c00 4400  ......|...r.|.D.
-000084f0: 5d10 7d04 7418 a019 7c04 a101 0100 9003  ].}.t...|.......
-00008500: 7100 6400 5300 291d 4e72 0100 0000 da05  q.d.S.).Nr......
-00008510: 6669 6e61 6c7a 1166 696e 616c 5f63 6f6d  finalz.final_com
-00008520: 6269 6e65 642e 6835 5472 2e00 0000 6939  bined.h5Tr....i9
-00008530: 0800 0046 7249 0000 0029 0a72 3601 0000  ...FrI...).r6...
-00008540: 7237 0100 0072 3801 0000 7239 0100 0072  r7...r8...r9...r
-00008550: 3a01 0000 723b 0100 0072 3c01 0000 723d  :...r;...r<...r=
-00008560: 0100 0072 3e01 0000 723f 0100 0072 6d00  ...r>...r?...rm.
-00008570: 0000 724a 0000 0072 a200 0000 7252 0000  ..rJ...r....rR..
-00008580: 0072 9600 0000 2903 da08 6d61 7873 6861  .r....)...maxsha
-00008590: 7065 da06 6368 756e 6b73 722a 0000 0072  pe..chunksr*...r
-000085a0: fb00 0000 7255 0100 0072 ef00 0000 7241  ....rU...r....rA
-000085b0: 0000 0072 9300 0000 da08 696e 5f72 616e  ...r......in_ran
-000085c0: 6765 727f 0000 00da 0d6d 6178 5f76 616c  ger......max_val
-000085d0: 5f73 7461 636b 7256 0100 0072 8601 0000  _stackrV...r....
-000085e0: da19 7472 6961 6c5f 6e75 6d73 5f61 6e64  ..trial_nums_and
-000085f0: 5f66 7261 6d65 5f6e 756d 7372 9200 0000  _frame_numsr....
-00008600: 7241 0100 0029 1a72 6101 0000 72d7 0000  rA...).ra...r...
-00008610: 0072 0800 0000 7244 0100 0072 aa00 0000  .r....rD...r....
-00008620: 7245 0100 00da 0a49 4545 455f 4633 324c  rE.....IEEE_F32L
-00008630: 4572 0b00 0000 72ab 0000 0072 4a01 0000  Er....r....rJ...
-00008640: 721d 0000 0072 3600 0000 7221 0000 0072  r....r6...r!...r
-00008650: 6901 0000 7224 0000 0072 2801 0000 7239  i...r$...r(...r9
-00008660: 0000 00da 0e63 7265 6174 655f 6461 7461  .....create_data
-00008670: 7365 7472 4601 0000 da06 7265 7369 7a65  setrF.....resize
-00008680: 7223 0000 0072 a900 0000 72e9 0000 0072  r#...r....r....r
-00008690: 1e01 0000 725f 0000 0072 7900 0000 290e  ....r_...ry...).
-000086a0: 72a2 0100 0072 9f01 0000 724b 0100 00da  r....r....rK....
-000086b0: 0368 3563 7233 0000 0072 bc00 0000 7249  .h5cr3...r....rI
-000086c0: 0000 0072 2c00 0000 7296 0000 005a 096d  ...r,...r....Z.m
-000086d0: 6178 5f73 6861 7065 7255 0100 0072 9500  ax_shaperU...r..
-000086e0: 0000 72a9 0100 0072 8f00 0000 7216 0000  ..r....r....r...
-000086f0: 0072 1600 0000 7217 0000 0072 a001 0000  .r....r....r....
-00008700: 7205 0000 7396 0000 0000 0108 0116 0106  r...s...........
-00008710: 0102 0102 0102 0102 0102 0102 0102 0106  ................
-00008720: 0106 0102 f606 0c0c 010e 0110 0128 0210  .............(..
-00008730: 0106 0110 0114 010c 010a 010a 0108 0206  ................
-00008740: 0108 0106 0102 0102 0102 fb08 0726 011a  .............&..
-00008750: 0210 0114 010c 010a 010a 0108 0206 0108  ................
-00008760: 0106 0102 0102 0102 fb08 0726 0126 020a  ...........&.&..
-00008770: 0102 0002 0002 0002 ff04 0204 0108 011a  ................
-00008780: 010a 010c 020e 010c 0110 010c 010a 0108  ................
-00008790: 0116 0206 010e ff04 0218 0206 0108 0172  ...............r
-000087a0: a001 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000087b0: 0005 0000 0006 0000 0043 0000 0073 f400  .........C...s..
-000087c0: 0000 7c00 a000 6401 6402 a102 0100 7c00  ..|...d.d.....|.
-000087d0: 6402 1700 6403 1700 7d03 7401 6a02 a003  d...d...}.t.j...
-000087e0: 7c03 a101 724a 7c01 734a 7404 a005 6404  |...rJ|.sJt...d.
-000087f0: a101 0100 7404 a005 6405 7c00 1700 a101  ....t...d.|.....
-00008800: 0100 7406 7c00 8301 0100 6ea6 7401 6a02  ..t.|.....n.t.j.
-00008810: a003 7c03 a101 726a 7401 a007 7c03 a101  ..|...rjt...|...
-00008820: 0100 7408 a009 7c02 a101 0100 740a 8300  ..t...|.....t...
-00008830: 7d04 7c00 7c04 6406 3c00 740b 740c a00c  }.|.|.d.<.t.t...
-00008840: 7c00 6407 1700 a101 8301 7c04 6408 3c00  |.d.......|.d.<.
-00008850: 740d a00e 740d a00f 7c04 6408 1900 a101  t...t...|.d.....
-00008860: 6409 a102 7c04 640a 3c00 640b 7c04 640c  d...|.d.<.d.|.d.
-00008870: 3c00 7406 640d 8301 0100 7410 7c04 6408  <.t.d.....t.|.d.
-00008880: 1900 8301 7c04 640e 3c00 6409 7c04 640f  ....|.d.<.d.|.d.
-00008890: 3c00 6410 6411 8400 7c04 6408 1900 4400  <.d.d...|.d...D.
-000088a0: 8301 7c04 6408 3c00 7411 7c04 7c03 8302  ..|.d.<.t.|.|...
-000088b0: 0100 6412 5300 2913 6100 0200 000a 0a20  ..d.S.).a...... 
-000088c0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-000088d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000088e0: 2076 6964 656f 5f64 6972 6563 746f 7279   video_directory
-000088f0: 203a 2020 7769 6c6c 206c 6f6f 6b20 696e   :  will look in
-00008900: 2061 6c6c 2073 7562 2064 6972 6563 746f   all sub directo
-00008910: 7269 6573 7320 7265 6375 7269 766c 790a  riess recurivly.
-00008920: 2020 2020 6f76 6572 7772 6974 6520 3a20      overwrite : 
-00008930: 6966 2054 7275 6520 7769 6c6c 2064 656c  if True will del
-00008940: 6574 6520 6669 6c65 2069 6620 6578 6973  ete file if exis
-00008950: 7473 0a20 2020 2074 696d 655f 736c 6565  ts.    time_slee
-00008960: 705f 6265 7477 6565 6e5f 6465 6c65 7465  p_between_delete
-00008970: 5f66 6f72 5f63 6c6f 7564 5f75 7064 6174  _for_cloud_updat
-00008980: 6520 3a20 6861 636b 7920 736f 6c75 7469  e : hacky soluti
-00008990: 6f6e 2074 6f20 676f 6f67 6c65 2064 7269  on to google dri
-000089a0: 7665 2063 6163 6865 2069 7373 7565 2077  ve cache issue w
-000089b0: 6865 7265 2074 6865 206d 6f64 6966 6965  here the modifie
-000089c0: 6420 6461 7461 2074 696d 650a 2020 2020  d data time.    
-000089d0: 646f 6573 206e 6f74 2075 7064 6174 6520  does not update 
-000089e0: 7769 7468 6f75 7420 6120 7469 6d65 2062  without a time b
-000089f0: 7566 6665 7220 6166 7465 7220 6265 696e  uffer after bein
-00008a00: 6720 6465 6c65 7465 2e20 6f6e 6c79 2072  g delete. only r
-00008a10: 656c 6976 656e 7420 666f 7220 6966 2079  elivent for if y
-00008a20: 6f75 2061 7265 206f 7665 7277 7269 7469  ou are overwriti
-00008a30: 6e67 2065 7869 7374 696e 6720 6669 6c65  ng existing file
-00008a40: 732c 2049 0a20 2020 206b 6e6f 7720 3330  s, I.    know 30
-00008a50: 2073 6563 6f6e 6473 2077 6f72 6b73 2068   seconds works h
-00008a60: 6572 652c 2061 6e6e 6f79 696e 6720 6275  ere, annoying bu
-00008a70: 7420 6e6f 7420 7468 6174 2062 6967 206f  t not that big o
-00008a80: 6620 6120 6465 616c 2061 7420 7468 6520  f a deal at the 
-00008a90: 656e 6420 6f66 2074 6865 2064 6179 0a0a  end of the day..
-00008aa0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00008ab0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2072 5201  -------..    rR.
-00008ac0: 0000 7251 0100 007a 2266 696c 655f 6c69  ..rQ...z"file_li
-00008ad0: 7374 5f66 6f72 5f62 6174 6368 5f70 726f  st_for_batch_pro
-00008ae0: 6365 7373 696e 672e 706b 6c61 5801 0000  cessing.pklaX...
-00008af0: 7761 726e 696e 6720 6669 6c65 2061 6c72  warning file alr
-00008b00: 6561 6479 2065 7869 7374 7321 2069 6620  eady exists! if 
-00008b10: 796f 7520 6f76 6572 7772 6974 6520 6120  you overwrite a 
-00008b20: 7061 7274 6961 6c6c 7920 7072 6f63 6573  partially proces
-00008b30: 7365 6420 6469 7265 6374 6f72 792c 2079  sed directory, y
-00008b40: 6f75 2077 696c 6c20 6578 7065 7269 656e  ou will experien
-00008b50: 6365 2069 7373 7565 7320 6c69 6b65 206f  ce issues like o
-00008b60: 7665 7277 7269 7465 2065 7272 6f72 732c  verwrite errors,
-00008b70: 2061 6e64 2079 6f75 276c 6c20 6c6f 7365   and you'll lose
-00008b80: 2079 6f75 7220 7072 6f67 7265 7373 2e20   your progress. 
-00008b90: 6966 2079 6f75 2061 7265 2073 7572 6520  if you are sure 
-00008ba0: 796f 7520 7761 6e74 2074 6f20 6f76 6572  you want to over
-00008bb0: 7772 6974 6520 6d61 6b65 2073 7572 6520  write make sure 
-00008bc0: 746f 2064 656c 6574 6520 7468 6520 636f  to delete the co
-00008bd0: 7272 6573 706f 6e64 696e 6720 275f 4649  rresponding '_FI
-00008be0: 4e49 5348 4544 2720 6469 7265 6374 6f72  NISHED' director
-00008bf0: 792c 2061 6e64 2069 6620 6e65 6365 7373  y, and if necess
-00008c00: 6172 7920 6d6f 7665 2074 6865 206d 7034  ary move the mp4
-00008c10: 7320 6261 636b 2074 6f20 7468 6520 7072  s back to the pr
-00008c20: 6f63 6573 7369 6e67 2066 6f6c 6465 7220  ocessing folder 
-00008c30: 616e 6420 7365 7420 6f76 6572 7772 6974  and set overwrit
-00008c40: 6520 3d20 5472 7565 7a41 7468 6973 2061  e = TruezAthis a
-00008c50: 626f 7665 206d 6573 7361 6765 2069 7320  bove message is 
-00008c60: 696e 2072 6566 6572 656e 6365 2074 6f20  in reference to 
-00008c70: 7468 6520 666f 6c6c 6f77 696e 6720 6469  the following di
-00008c80: 7265 6374 6f72 792e 2e2e 0a5a 166f 7269  rectory....Z.ori
-00008c90: 6769 6e61 6c5f 6d70 345f 6469 7265 6374  ginal_mp4_direct
-00008ca0: 6f72 797a 062f 2a2e 6d70 3472 8401 0000  oryz./*.mp4r....
-00008cb0: 4672 8501 0000 7a45 796f 7520 6361 6e20  Fr....zEyou can 
-00008cc0: 7075 7420 616e 7920 6e6f 7465 7320 6865  put any notes he
-00008cd0: 7265 2064 6972 6563 746c 7920 6672 6f6d  re directly from
-00008ce0: 2074 6865 2074 6578 7420 6669 6c65 2069   the text file i
-00008cf0: 6620 796f 7520 7761 6e74 2074 6f5a 054e  f you want toZ.N
-00008d00: 4f54 4553 7a52 5065 7266 6f72 6d69 6e67  OTESzRPerforming
-00008d10: 2069 6e69 7469 616c 2063 6865 636b 2074   initial check t
-00008d20: 6f20 7365 6520 6966 2073 6f6d 6520 4d50  o see if some MP
-00008d30: 3473 2061 7265 2022 6261 6422 2062 7920  4s are "bad" by 
-00008d40: 7465 7374 696e 6720 6966 2046 5053 2069  testing if FPS i
-00008d50: 7320 616e 2069 6e74 7283 0100 0072 8201  s an intr....r..
-00008d60: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00008d70: 0000 0006 0000 0053 0000 0073 1800 0000  .......S...s....
-00008d80: 6700 7c00 5d10 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
-00008d90: a102 9102 7104 5300 2902 7252 0100 0072  ....q.S.).rR...r
-00008da0: 5101 0000 7262 0100 0072 3100 0000 7216  Q...rb...r1...r.
-00008db0: 0000 0072 1600 0000 7217 0000 0072 3400  ...r....r....r4.
-00008dc0: 0000 1506 0000 7304 0000 0006 0002 007a  ......s........z
-00008dd0: 266d 616b 655f 6d70 345f 6c69 7374 5f64  &make_mp4_list_d
-00008de0: 6963 742e 3c6c 6f63 616c 733e 2e3c 6c69  ict.<locals>.<li
-00008df0: 7374 636f 6d70 3e4e 2912 72b3 0000 0072  stcomp>N).r....r
-00008e00: 5f00 0000 7261 0000 0072 a500 0000 728b  _...ra...r....r.
-00008e10: 0000 0072 8c00 0000 724b 0000 0072 7900  ...r....rK...ry.
-00008e20: 0000 7296 0100 00da 0573 6c65 6570 7268  ..r......sleeprh
-00008e30: 0000 0072 6101 0000 da04 676c 6f62 721d  ...ra.....globr.
-00008e40: 0000 00da 0466 756c 6c72 2100 0000 72ca  .....fullr!...r.
-00008e50: 0000 0072 9901 0000 2905 729c 0000 0072  ...r....).r....r
-00008e60: 5c00 0000 5a2a 7469 6d65 5f73 6c65 6570  \...Z*time_sleep
-00008e70: 5f62 6574 7765 656e 5f64 656c 6574 655f  _between_delete_
-00008e80: 666f 725f 636c 6f75 645f 7570 6461 7465  for_cloud_update
-00008e90: 724b 0100 005a 0474 6d70 6472 1600 0000  rK...Z.tmpdr....
-00008ea0: 7216 0000 0072 1700 0000 da12 6d61 6b65  r....r......make
-00008eb0: 5f6d 7034 5f6c 6973 745f 6469 6374 ee05  _mp4_list_dict..
-00008ec0: 0000 7326 0000 0000 100c 010c 0210 010a  ..s&............
-00008ed0: 040e 010a 030c 010a 010a 0106 0108 0116  ................
-00008ee0: 011a 0108 0108 0110 0108 0116 0272 b101  .............r..
-00008ef0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00008f00: 0000 0003 0000 0043 0000 0073 1c00 0000  .......C...s....
-00008f10: 7c00 6401 6400 8502 1900 6402 6b03 7218  |.d.d.....d.k.r.
-00008f20: 7c00 6402 1700 5300 7c00 5300 2903 4e72  |.d...S.|.S.).Nr
-00008f30: 6c00 0000 7290 0100 0072 1600 0000 2901  l...r....r....).
-00008f40: da04 6e61 6d65 7216 0000 0072 1600 0000  ..namer....r....
-00008f50: 7217 0000 00da 0a5f 6368 6563 6b5f 706b  r......_check_pk
-00008f60: 6c1a 0600 0073 0600 0000 0001 1001 0801  l....s..........
-00008f70: 72b3 0100 0063 0200 0000 0000 0000 0000  r....c..........
-00008f80: 0000 0300 0000 0900 0000 4300 0000 732e  ..........C...s.
-00008f90: 0000 0074 0074 017c 0183 0164 0183 028f  ...t.t.|...d....
-00008fa0: 167d 0274 026a 037c 007c 0264 0264 038d  .}.t.j.|.|.d.d..
-00008fb0: 0301 0057 0035 0051 0052 0058 0064 0053  ...W.5.Q.R.X.d.S
-00008fc0: 0029 044e da02 7762 72d5 0000 0029 01da  .).N..wbr....)..
-00008fd0: 0870 726f 746f 636f 6c29 04da 046f 7065  .protocol)...ope
-00008fe0: 6e72 b301 0000 da06 7069 636b 6c65 da04  nr......pickle..
-00008ff0: 6475 6d70 2903 da03 6f62 6a72 b201 0000  dump)...objr....
-00009000: 72a1 0100 0072 1600 0000 7216 0000 0072  r....r....r....r
-00009010: 1700 0000 7299 0100 0020 0600 0073 0400  ....r.... ...s..
-00009020: 0000 0001 1002 7299 0100 0063 0100 0000  ......r....c....
-00009030: 0000 0000 0000 0000 0200 0000 0a00 0000  ................
-00009040: 4300 0000 7330 0000 0074 0074 017c 0083  C...s0...t.t.|..
-00009050: 0164 0183 028f 187d 0174 02a0 037c 01a1  .d.....}.t...|..
-00009060: 0157 0002 0035 0051 0052 00a3 0053 0051  .W...5.Q.R...S.Q
-00009070: 0052 0058 0064 0053 0029 024e da02 7262  .R.X.d.S.).N..rb
-00009080: 2904 72b6 0100 0072 b301 0000 72b7 0100  ).r....r....r...
-00009090: 00da 046c 6f61 6429 0272 b201 0000 72a1  ...load).r....r.
-000090a0: 0100 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000090b0: 0000 7263 0000 0026 0600 0073 0400 0000  ..rc...&...s....
-000090c0: 0001 1001 7263 0000 0063 0000 0000 0000  ....rc...c......
-000090d0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000090e0: 0000 7312 0000 0074 006a 01a0 0274 036a  ..s....t.j...t.j
-000090f0: 04a1 017d 007c 0053 0072 0901 0000 2905  ...}.|.S.r....).
-00009100: 725f 0000 0072 6100 0000 72a3 0000 00da  r_...ra...r.....
-00009110: 0577 6861 6363 da08 5f5f 6669 6c65 5f5f  .whacc..__file__
-00009120: 726f 0000 0072 1600 0000 7216 0000 0072  ro...r....r....r
-00009130: 1700 0000 725e 0000 002b 0600 0073 0400  ....r^...+...s..
-00009140: 0000 0001 0e01 725e 0000 0063 0000 0000  ......r^...c....
-00009150: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00009160: 4300 0000 7330 0000 0074 0083 0064 0117  C...s0...t...d..
-00009170: 007d 0074 017c 0064 0217 0083 017d 0174  .}.t.|.d.....}.t
-00009180: 02a0 037c 0164 0319 00a1 0164 0419 007c  ...|.d.....d...|
-00009190: 0164 053c 007c 0153 0029 064e fa19 2f77  .d.<.|.S.).N../w
-000091a0: 6861 6363 5f64 6174 612f 6665 6174 7572  hacc_data/featur
-000091b0: 655f 6461 7461 2f7a 1566 6561 7475 7265  e_data/z.feature
-000091c0: 5f64 6174 615f 6469 6374 2e70 6b6c 5a1c  _data_dict.pklZ.
-000091d0: 6669 6e61 6c5f 7365 6c65 6374 6564 5f66  final_selected_f
-000091e0: 6561 7475 7265 735f 626f 6f6c 7201 0000  eatures_boolr...
-000091f0: 005a 1766 696e 616c 5f73 656c 6563 7465  .Z.final_selecte
-00009200: 645f 6665 6174 7572 6573 2904 725e 0000  d_features).r^..
-00009210: 0072 6300 0000 721d 0000 0072 b500 0000  .rc...r....r....
-00009220: 2902 7253 0000 0072 6a00 0000 7216 0000  ).rS...rj...r...
-00009230: 0072 1600 0000 7217 0000 00da 116c 6f61  .r....r......loa
-00009240: 645f 6665 6174 7572 655f 6461 7461 3006  d_feature_data0.
-00009250: 0000 7308 0000 0000 010a 010c 0116 0172  ..s............r
-00009260: bf01 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00009270: 0002 0000 0003 0000 0043 0000 0073 1a00  .........C...s..
-00009280: 0000 7400 8300 6401 1700 7d00 7401 7c00  ..t...d...}.t.|.
-00009290: 6402 1700 8301 7d01 7c01 5300 2903 4e72  d.....}.|.S.).Nr
-000092a0: be01 0000 7a1b 7374 6172 745f 656e 645f  ....z.start_end_
-000092b0: 6e61 6e5f 6c6f 6361 7469 6f6e 732e 706b  nan_locations.pk
-000092c0: 6c29 0272 5e00 0000 7263 0000 0029 0272  l).r^...rc...).r
-000092d0: 5300 0000 5a09 6172 7261 795f 6f75 7472  S...Z.array_outr
-000092e0: 1600 0000 7216 0000 0072 1700 0000 721a  ....r....r....r.
-000092f0: 0000 0037 0600 0073 0600 0000 0001 0a01  ...7...s........
-00009300: 0c01 721a 0000 0072 d500 0000 6301 0000  ..r....r....c...
-00009310: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00009320: 0043 0000 0073 3600 0000 7400 8300 7d01  .C...s6...t...}.
-00009330: 7c01 6401 1900 7d02 7401 a002 7c02 7c00  |.d...}.t...|.|.
-00009340: 6b05 a101 6402 1900 7d03 6403 6404 8400  k...d...}.d.d...
-00009350: 7403 6405 8301 4400 8301 7d04 7c03 5300  t.d...D...}.|.S.
-00009360: 2906 61d6 0100 000a 2020 2020 5061 7261  ).a.....    Para
-00009370: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00009380: 2d2d 2d2d 2d0a 2020 2020 6772 6561 7465  -----.    greate
-00009390: 725f 7468 616e 5f6f 725f 6571 7561 6c5f  r_than_or_equal_
-000093a0: 746f 203a 2030 206d 6561 6e73 2073 656c  to : 0 means sel
-000093b0: 6563 7420 616c 6c20 6665 6174 7572 6573  ect all features
-000093c0: 2c20 3130 206d 6561 6e73 206f 6e6c 7920  , 10 means only 
-000093d0: 7468 6520 6665 6174 7572 6573 2074 6861  the features tha
-000093e0: 7420 7765 7265 2075 7365 2069 6e20 4556  t were use in EV
-000093f0: 4552 5920 7465 7374 0a20 2020 206c 6967  ERY test.    lig
-00009400: 6874 2047 424d 206d 6f64 656c 2e20 4e6f  ht GBM model. No
-00009410: 7465 3a20 7468 6520 7361 7665 204c 6967  te: the save Lig
-00009420: 6874 2047 424d 2028 6d6f 6465 6c29 2069  ht GBM (model) i
-00009430: 7320 7472 6169 6e65 6420 6f6e 2067 7265  s trained on gre
-00009440: 6174 6572 5f74 6861 6e5f 6f72 5f65 7175  ater_than_or_equ
-00009450: 616c 5f74 6f20 3d20 342c 2073 6f20 796f  al_to = 4, so yo
-00009460: 7520 6361 6e20 6368 616e 6765 2074 6869  u can change thi
-00009470: 730a 2020 2020 6275 7420 796f 7520 7769  s.    but you wi
-00009480: 6c6c 206e 6565 6420 746f 2072 6574 7261  ll need to retra
-00009490: 696e 2074 6865 206c 6967 6874 2047 424d  in the light GBM
-000094a0: 2028 6d6f 6465 6c29 2e0a 2020 2020 5265   (model)..    Re
-000094b0: 7475 726e 7320 6b65 6570 5f66 6561 7475  turns keep_featu
-000094c0: 7265 735f 696e 6465 7820 3a20 696e 6465  res_index : inde
-000094d0: 7820 746f 2074 6865 2067 6961 6e74 2027  x to the giant '
-000094e0: 3834 2c30 3039 2720 6665 6174 7572 6573  84,009' features
-000094f0: 2c20 6e6f 7465 2067 7265 6174 6572 5f74  , note greater_t
-00009500: 6861 6e5f 6f72 5f65 7175 616c 5f74 6f20  han_or_equal_to 
-00009510: 3d20 3420 7265 7475 726e 2033 3039 350a  = 4 return 3095.
-00009520: 2020 2020 6665 6174 7572 6573 0a20 2020      features.   
-00009530: 202d 2d2d 2d2d 2d2d 0a20 2020 205a 1366   -------.    Z.f
-00009540: 6561 7475 7265 735f 7573 6564 5f6f 665f  eatures_used_of_
-00009550: 3130 7201 0000 0063 0100 0000 0000 0000  10r....c........
-00009560: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00009570: 731c 0000 0067 007c 005d 147d 017c 0174  s....g.|.].}.|.t
-00009580: 006b 0672 1464 006e 0264 0191 0271 0453  .k.r.d.n.d...q.S
-00009590: 0029 0254 4672 cd00 0000 7231 0000 0072  .).TFr....r1...r
-000095a0: 1600 0000 7216 0000 0072 1700 0000 7234  ....r....r....r4
-000095b0: 0000 0052 0600 0073 0400 0000 0600 0200  ...R...s........
-000095c0: 7a29 6765 745f 7365 6c65 6374 6564 5f66  z)get_selected_f
-000095d0: 6561 7475 7265 732e 3c6c 6f63 616c 733e  eatures.<locals>
-000095e0: 2e3c 6c69 7374 636f 6d70 3e69 2948 0100  .<listcomp>i)H..
-000095f0: 2904 72bf 0100 0072 1d00 0000 72b5 0000  ).r....r....r...
-00009600: 0072 3a00 0000 2905 5a18 6772 6561 7465  .r:...).Z.greate
-00009610: 725f 7468 616e 5f6f 725f 6571 7561 6c5f  r_than_or_equal_
-00009620: 746f 7221 0100 005a 1266 6561 7475 7265  tor!...Z.feature
-00009630: 735f 6f75 745f 6f66 5f31 305a 136b 6565  s_out_of_10Z.kee
-00009640: 705f 6665 6174 7572 6573 5f69 6e64 6578  p_features_index
-00009650: 5a18 6665 6174 7572 6573 5f75 7365 645f  Z.features_used_
-00009660: 6f66 5f31 305f 626f 6f6c 7216 0000 0072  of_10_boolr....r
-00009670: 1600 0000 7217 0000 00da 1567 6574 5f73  ....r......get_s
-00009680: 656c 6563 7465 645f 6665 6174 7572 6573  elected_features
-00009690: 4106 0000 730a 0000 0000 0c06 0108 0212  A...s...........
-000096a0: 0212 0172 c001 0000 6300 0000 0000 0000  ...r....c.......
-000096b0: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
-000096c0: 0073 6600 0000 7a4a 7400 7401 8300 6a02  .sf...zJt.t...j.
-000096d0: 8301 7d00 7401 8300 6a02 6a03 7d01 6401  ..}.t...j.j.}.d.
-000096e0: 7c00 6b06 7226 5700 6402 5300 7c01 6403  |.k.r&W.d.S.|.d.
-000096f0: 6b02 7234 5700 6402 5300 7c01 6404 6b02  k.r4W.d.S.|.d.k.
-00009700: 7242 5700 6405 5300 5700 6405 5300 5700  rBW.d.S.W.d.S.W.
-00009710: 6e16 0400 7404 6b0a 7260 0100 0100 0100  n...t.k.r`......
-00009720: 5900 6405 5300 5800 6400 5300 2906 4e5a  Y.d.S.X.d.S.).NZ
-00009730: 0563 6f6c 6162 545a 135a 4d51 496e 7465  .colabTZ.ZMQInte
-00009740: 7261 6374 6976 6553 6865 6c6c 5a18 5465  ractiveShellZ.Te
-00009750: 726d 696e 616c 496e 7465 7261 6374 6976  rminalInteractiv
-00009760: 6553 6865 6c6c 4629 0572 a900 0000 da0b  eShellF).r......
-00009770: 6765 745f 6970 7974 686f 6eda 095f 5f63  get_ipython..__c
-00009780: 6c61 7373 5f5f 7273 0100 00da 094e 616d  lass__rs.....Nam
-00009790: 6545 7272 6f72 2902 72e2 0000 00da 0573  eError).r......s
-000097a0: 6865 6c6c 7216 0000 0072 1600 0000 7217  hellr....r....r.
-000097b0: 0000 00da 0a69 736e 6f74 6562 6f6f 6b56  .....isnotebookV
-000097c0: 0600 0073 1800 0000 0001 0201 0c01 0a01  ...s............
-000097d0: 0801 0601 0801 0601 0801 0602 0a01 0e01  ................
-000097e0: 72c5 0100 0063 0100 0000 0000 0000 0000  r....c..........
-000097f0: 0000 0400 0000 0700 0000 4300 0000 733c  ..........C...s<
-00009800: 0000 0074 00a0 017c 00a1 017d 0174 00a0  ...t...|...}.t..
-00009810: 0164 0167 0174 0274 00a0 037c 01a1 0183  .d.g.t.t...|....
-00009820: 0117 00a1 017d 027c 017c 0217 007d 0364  .....}.|.|...}.d
-00009830: 027c 037c 0364 036b 023c 007c 0353 0029  .|.|.d.k.<.|.S.)
-00009840: 044e 7201 0000 0072 4600 0000 724a 0000  .Nr....rF...rJ..
-00009850: 0029 0472 1d00 0000 7238 0000 0072 3900  .).r....r8...r9.
-00009860: 0000 729a 0100 0029 0472 5300 0000 72e1  ..r....).rS...r.
-00009870: 0000 0072 4200 0000 72e2 0000 0072 1600  ...rB...r....r..
-00009880: 0000 7216 0000 0072 1700 0000 da1d 666f  ..r....r......fo
-00009890: 7572 5f63 6c61 7373 5f6c 6162 656c 735f  ur_class_labels_
-000098a0: 6672 6f6d 5f62 696e 6172 796c 0600 0073  from_binaryl...s
-000098b0: 0a00 0000 0001 0a01 1a01 0801 0c01 72c6  ..............r.
-000098c0: 0100 0063 0300 0000 0000 0000 0000 0000  ...c............
-000098d0: 0500 0000 0a00 0000 4300 0000 734e 0000  ........C...sN..
-000098e0: 0074 00a0 017c 0064 01a1 028f 387d 0374  .t...|.d....8}.t
-000098f0: 02a0 0374 047c 03a0 05a1 0083 01a1 017d  ...t.|.........}
-00009900: 047c 0272 2c74 067c 0483 0101 007c 0172  .|.r,t.|.....|.r
-00009910: 407c 0457 0002 0035 0051 0052 00a3 0053  @|.W...5.Q.R...S
-00009920: 0057 0035 0051 0052 0058 0064 0053 0029  .W.5.Q.R.X.d.S.)
-00009930: 024e 726d 0000 0029 0772 aa00 0000 72ab  .Nrm...).r....r.
-00009940: 0000 0072 1b00 0000 721c 0000 0072 3900  ...r....r....r9.
-00009950: 0000 7295 0000 00da 1470 7269 6e74 5f6c  ..r......print_l
-00009960: 6973 745f 7769 7468 5f69 6e64 7329 055a  ist_with_inds).Z
-00009970: 0668 3566 696c 65da 0b72 6574 7572 6e5f  .h5file..return_
-00009980: 6c69 7374 da08 646f 5f70 7269 6e74 72bc  list..do_printr.
-00009990: 0000 0072 5300 0000 7216 0000 0072 1600  ...rS...r....r..
-000099a0: 0000 7217 0000 0072 a700 0000 7406 0000  ..r....r....t...
-000099b0: 730c 0000 0000 010e 0112 0104 0108 0104  s...............
-000099c0: 0172 a700 0000 6304 0000 0000 0000 0000  .r....c.........
-000099d0: 0000 0006 0000 000c 0000 0043 0000 0073  ...........C...s
-000099e0: 9c00 0000 7c03 6400 6b08 720c 7c02 7d03  ....|.d.k.r.|.}.
-000099f0: 7400 a001 7c00 6401 a102 8f7a 7d04 7400  t...|.d....z}.t.
-00009a00: a001 7c01 6402 a102 8f62 7d05 7a20 7c04  ..|.d....b}.z |.
-00009a10: 7c02 1900 6400 6400 8502 1900 7c05 7c03  |...d.d.....|.|.
-00009a20: 1900 6400 6400 8502 3c00 5700 6e3a 0100  ..d.d...<.W.n:..
-00009a30: 0100 0100 7c05 6a02 7c03 7403 a004 7c04  ....|.j.|.t...|.
-00009a40: 7c02 1900 6400 6400 8502 1900 a101 7c04  |...d.d.......|.
-00009a50: 7c02 1900 6400 6400 8502 1900 6403 8d03  |...d.d.....d...
-00009a60: 0100 5900 6e02 5800 5700 3500 5100 5200  ..Y.n.X.W.5.Q.R.
-00009a70: 5800 5700 3500 5100 5200 5800 6400 5300  X.W.5.Q.R.X.d.S.
-00009a80: 2904 4e72 6d00 0000 72a2 0000 00a9 0272  ).Nrm...r......r
-00009a90: 2100 0000 722a 0000 0029 0572 aa00 0000  !...r*...).r....
-00009aa0: 72ab 0000 0072 ab01 0000 721d 0000 0072  r....r....r....r
-00009ab0: 2100 0000 2906 5a0f 6835 5f74 6f5f 636f  !...).Z.h5_to_co
-00009ac0: 7079 5f66 726f 6d5a 0d68 355f 746f 5f63  py_fromZ.h5_to_c
-00009ad0: 6f70 795f 746f 5a19 6c61 6265 6c5f 7374  opy_toZ.label_st
-00009ae0: 7269 6e67 5f74 6f5f 636f 7079 5f66 726f  ring_to_copy_fro
-00009af0: 6d5a 176c 6162 656c 5f73 7472 696e 675f  mZ.label_string_
-00009b00: 746f 5f63 6f70 795f 746f 72bc 0000 00da  to_copy_tor.....
-00009b10: 0268 3272 1600 0000 7216 0000 0072 1700  .h2r....r....r..
-00009b20: 0000 da19 636f 7079 5f68 355f 6b65 795f  ....copy_h5_key_
-00009b30: 746f 5f61 6e6f 7468 6572 5f68 357d 0600  to_another_h5}..
-00009b40: 0073 1400 0000 0001 0801 0401 0e01 0e01  .s..............
-00009b50: 0201 2001 0601 1a01 0eff 72cc 0100 0029  .. .......r....)
-00009b60: 01da 0672 6574 7572 6e63 0400 0000 0000  ...returnc......
-00009b70: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
-00009b80: 0000 730c 0100 0074 007c 0083 0164 016b  ..s....t.|...d.k
-00009b90: 0272 1874 0164 0283 0101 007c 0053 0064  .r.t.d.....|.S.d
-00009ba0: 0364 0484 007d 0474 027c 0174 0383 0272  .d...}.t.|.t...r
-00009bb0: 307c 0167 017d 0174 027c 0274 0383 0272  0|.g.}.t.|.t...r
-00009bc0: 407c 0267 017d 0274 04a0 0564 0567 0174  @|.g.}.t...d.g.t
-00009bd0: 007c 0083 0114 00a1 017d 057c 0144 005d  .|.......}.|.D.]
-00009be0: 187d 0674 04a0 067c 057c 047c 007c 0683  .}.t...|.|.|.|..
-00009bf0: 0266 02a1 017d 0571 5874 046a 077c 0564  .f...}.qXt.j.|.d
-00009c00: 0164 068d 0264 016b 047d 0574 04a0 0564  .d...d.k.}.t...d
-00009c10: 0767 0174 007c 0083 0114 00a1 017d 077c  .g.t.|.......}.|
-00009c20: 0264 006b 0972 d67c 0244 005d 1e7d 0674  .d.k.r.|.D.].}.t
-00009c30: 04a0 067c 0774 04a0 087c 047c 007c 0683  ...|.t...|.|.|..
-00009c40: 02a1 0166 02a1 017d 0771 a474 046a 097c  ...f...}.q.t.j.|
-00009c50: 0764 0164 068d 0264 016b 047d 077c 057c  .d.d...d.k.}.|.|
-00009c60: 0714 007d 087c 086a 0a64 016b 0172 ec67  ...}.|.j.d.k.r.g
-00009c70: 0053 0074 04a0 057c 00a1 017c 0819 007d  .S.t...|...|...}
-00009c80: 097c 0390 0172 087c 097c 0866 0253 007c  .|...r.|.|.f.S.|
-00009c90: 0953 0029 084e 7201 0000 007a 2469 6e5f  .S.).Nr....z$in_
-00009ca0: 6c69 7374 2077 6173 2065 6d70 7479 2c20  list was empty, 
-00009cb0: 7265 7475 726e 696e 6720 696e 5f6c 6973  returning in_lis
-00009cc0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
-00009cd0: 0000 0500 0000 1300 0000 7318 0000 0074  ..........s....t
-00009ce0: 00a0 0187 0066 0164 0164 0284 087c 0044  .....f.d.d...|.D
-00009cf0: 0083 01a1 0153 0029 034e 6301 0000 0000  .....S.).Nc.....
-00009d00: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-00009d10: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00009d20: 8800 7c01 6b06 9102 7104 5300 7216 0000  ..|.k...q.S.r...
-00009d30: 0072 1600 0000 2902 7232 0000 00da 0673  .r....).r2.....s
-00009d40: 7472 696e 67a9 01da 0a63 6d70 5f73 7472  tring....cmp_str
-00009d50: 696e 6772 1600 0000 7217 0000 0072 3400  ingr....r....r4.
-00009d60: 0000 8f06 0000 7304 0000 0006 0002 007a  ......s........z
-00009d70: 3c6c 6973 7465 725f 6974 2e3c 6c6f 6361  <lister_it.<loca
-00009d80: 6c73 3e2e 696e 6465 785f 6c69 7374 5f6f  ls>.index_list_o
-00009d90: 665f 7374 7269 6e67 732e 3c6c 6f63 616c  f_strings.<local
-00009da0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0272  s>.<listcomp>).r
-00009db0: 1d00 0000 7238 0000 0029 025a 0869 6e5f  ....r8...).Z.in_
-00009dc0: 6c69 7374 3272 d001 0000 7216 0000 0072  list2r....r....r
-00009dd0: cf01 0000 7217 0000 00da 1569 6e64 6578  ....r......index
-00009de0: 5f6c 6973 745f 6f66 5f73 7472 696e 6773  _list_of_strings
-00009df0: 8e06 0000 7302 0000 0000 017a 286c 6973  ....s......z(lis
-00009e00: 7465 725f 6974 2e3c 6c6f 6361 6c73 3e2e  ter_it.<locals>.
-00009e10: 696e 6465 785f 6c69 7374 5f6f 665f 7374  index_list_of_st
-00009e20: 7269 6e67 7346 72fb 0000 0054 290b 7230  ringsFr....T).r0
-00009e30: 0000 0072 4b00 0000 7207 0100 0072 a900  ...rK...r....r..
-00009e40: 0000 721d 0000 0072 3800 0000 7225 0000  ..r....r8...r%..
-00009e50: 0072 3500 0000 da06 696e 7665 7274 da07  .r5.....invert..
-00009e60: 7072 6f64 7563 7472 2c01 0000 290a 5a07  productr,...).Z.
-00009e70: 696e 5f6c 6973 74da 0c6b 6565 705f 7374  in_list..keep_st
-00009e80: 7269 6e67 73da 0d72 656d 6f76 655f 7374  rings..remove_st
-00009e90: 7269 6e67 5a11 7265 7475 726e 5f62 6f6f  ringZ.return_boo
-00009ea0: 6c5f 696e 6465 7872 d101 0000 5a06 6b65  l_indexr....Z.ke
-00009eb0: 6570 5f69 7233 0000 005a 0872 656d 6f76  ep_ir3...Z.remov
-00009ec0: 655f 6972 2b00 0000 728f 0000 0072 1600  e_ir+...r....r..
-00009ed0: 0000 7216 0000 0072 1700 0000 da09 6c69  ..r....r......li
-00009ee0: 7374 6572 5f69 7489 0600 0073 3000 0000  ster_it....s0...
-00009ef0: 0001 0c01 0801 0402 0803 0a00 0601 0a00  ................
-00009f00: 0602 1401 0801 1601 1202 1401 0801 0801  ................
-00009f10: 1c01 1202 0801 0a01 0402 0e01 0601 0801  ................
-00009f20: 72d6 0100 0063 0100 0000 0000 0000 0000  r....c..........
-00009f30: 0000 0400 0000 0900 0000 4300 0000 7346  ..........C...sF
-00009f40: 0000 0074 00a0 017c 0064 01a1 028f 307d  ...t...|.d....0}
-00009f50: 0174 027c 0164 0219 0064 0064 0085 0219  .t.|.d...d.d....
-00009f60: 0083 0144 005d 145c 027d 027d 0374 03a0  ...D.].\.}.}.t..
-00009f70: 047c 027c 03a1 0201 0071 2257 0035 0051  .|.|.....q"W.5.Q
-00009f80: 0052 0058 0064 0053 0029 034e 726d 0000  .R.X.d.S.).Nrm..
-00009f90: 0072 a801 0000 2905 72aa 0000 0072 ab00  .r....).r....r..
-00009fa0: 0000 7224 0000 0072 1100 0000 da04 706c  ..r$...r......pl
-00009fb0: 6f74 2904 da07 6835 5f66 696c 65da 0268  ot)...h5_file..h
-00009fc0: 6672 2c00 0000 7233 0000 0072 1600 0000  fr,...r3...r....
-00009fd0: 7216 0000 0072 1700 0000 da1b 706c 6f74  r....r......plot
-00009fe0: 5f70 6f6c 655f 7472 6163 6b69 6e67 5f6d  _pole_tracking_m
-00009ff0: 6178 5f76 616c 73d0 0600 0073 0600 0000  ax_vals....s....
-0000a000: 0001 0e01 1c01 72da 0100 00e9 2800 0000  ......r.....(...
-0000a010: 6305 0000 0000 0000 0000 0000 0018 0000  c...............
-0000a020: 0006 0000 0043 0000 0073 ee02 0000 6401  .....C...s....d.
-0000a030: 6402 8400 7d05 6700 7d06 6700 7d07 6700  d...}.g.}.g.}.g.
-0000a040: 7d08 6700 7d09 7400 7c00 8301 4400 5dda  }.g.}.t.|...D.].
-0000a050: 7d0a 7c02 6403 6b08 7298 7c0a 6404 1900  }.|.d.k.r.|.d...
-0000a060: 6405 6b03 7298 7401 7402 7403 6406 7c0a  d.k.r.t.t.t.d.|.
-0000a070: 1700 8301 8301 8301 7d0b 7c09 a004 7c0b  ........}.|...|.
-0000a080: a005 6407 a101 6408 1900 a101 0100 7c06  ..d...d.......|.
-0000a090: a004 7c0a a101 0100 7c05 7403 6406 7c06  ..|.....|.t.d.|.
-0000a0a0: 6409 1900 1700 8301 8301 5c02 7d0c 7d0d  d.........\.}.}.
-0000a0b0: 7c07 a004 7c0c a101 0100 7c08 a004 7c0d  |...|.....|...|.
-0000a0c0: a101 0100 7120 7c02 7220 7401 7402 7403  ....q |.r t.t.t.
-0000a0d0: 6406 7c0a 1700 8301 8301 8301 7d0b 7c09  d.|.........}.|.
-0000a0e0: a004 7c0b a005 6407 a101 6408 1900 a101  ..|...d...d.....
-0000a0f0: 0100 7c06 a004 7c0a a101 0100 7c05 7403  ..|...|.....|.t.
-0000a100: 6406 7c06 6409 1900 1700 8301 8301 5c02  d.|.d.........\.
-0000a110: 7d0c 7d0d 7c07 a004 7c0c a101 0100 7c08  }.}.|...|.....|.
-0000a120: a004 7c0d a101 0100 7120 640a 7406 640b  ..|.....q d.t.d.
-0000a130: 640c 8400 7c06 4400 8301 8301 1400 7d0e  d...|.D.......}.
-0000a140: 640a 7406 640d 640c 8400 7c09 4400 8301  d.t.d.d...|.D...
-0000a150: 8301 1400 7d0f 640a 7406 640e 640c 8400  ....}.d.t.d.d...
-0000a160: 7c07 4400 8301 8301 1400 7d10 7c01 6400  |.D.......}.|.d.
-0000a170: 6b08 9001 7258 7407 a008 7409 7c06 8301  k...rXt...t.|...
-0000a180: a101 7d11 6eac 640f 7c01 a00a a100 6b06  ..}.n.d.|.....k.
-0000a190: 9001 7272 7407 a00b 7c09 a101 7d11 6e92  ..rrt...|...}.n.
-0000a1a0: 6410 7c01 a00a a100 6b06 9001 738e 6411  d.|.....k...s.d.
-0000a1b0: 7c01 a00a a100 6b06 9001 72dc 7407 6a0c  |.....k...r.t.j.
-0000a1c0: 6a0d 6412 7407 6a0e 6413 8d02 0100 7407  j.d.t.j.d.....t.
-0000a1d0: a00f 6414 6415 8400 7c07 4400 8301 a101  ..d.d...|.D.....
-0000a1e0: 7d0b 7407 6a10 7c0b 7c0b 6400 6b02 3c00  }.t.j.|.|.d.k.<.
-0000a1f0: 6416 6415 8400 7c0b 4400 8301 7d0b 7407  d.d...|.D...}.t.
-0000a200: a00b 7c0b a101 7d11 6e28 6417 7c01 a00a  ..|...}.n(d.|...
-0000a210: a100 6b06 9001 72f6 7407 a00b 7c06 a101  ..k...r.t...|...
-0000a220: 7d11 6e0e 7407 a008 7409 7c06 8301 a101  }.n.t...t.|.....
-0000a230: 7d11 7c11 4400 5dd2 7d12 7c06 7c12 1900  }.|.D.].}.|.|...
-0000a240: 7d13 7c09 7c12 1900 7d14 7c07 7c12 1900  }.|.|...}.|.|...
-0000a250: 7d15 7403 6406 7c06 7c12 1900 1700 8301  }.t.d.|.|.......
-0000a260: 7d16 7401 7c16 8301 7d17 7c13 7c0e 1700  }.t.|...}.|.|...
-0000a270: 6400 7409 7c0e 8301 8502 1900 7d13 7c14  d.t.|.......}.|.
-0000a280: 7c0f 1700 6400 7409 7c0f 8301 8502 1900  |...d.t.|.......
-0000a290: 7d14 7c15 7c10 1700 6400 7409 7c10 8301  }.|.|...d.t.|...
-0000a2a0: 8502 1900 7d15 7409 7c17 8301 7c04 6b04  ....}.t.|...|.k.
-0000a2b0: 9002 729a 6418 7c17 7c04 0b00 6400 8502  ..r.d.|.|...d...
-0000a2c0: 1900 1700 7d17 6e12 6419 7c17 7c04 0b00  ....}.n.d.|.|...
-0000a2d0: 6400 8502 1900 1700 7d17 7411 7c13 641a  d.......}.t.|.d.
-0000a2e0: 1700 7c14 1700 641b 1700 7c08 7c12 1900  ..|...d...|.|...
-0000a2f0: 1700 641c 1700 7c15 1700 641b 1700 7c17  ..d...|...d...|.
-0000a300: 1700 8301 0100 9002 7108 7c03 9002 72ea  ........q.|...r.
-0000a310: 7c06 7c09 6602 5300 6400 5300 291d 4e63  |.|.f.S.d.S.).Nc
-0000a320: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-0000a330: 0600 0000 5300 0000 735c 0000 0064 007d  ....S...s\...d.}
-0000a340: 017a 3274 0074 017c 0083 0183 017d 0264  .z2t.t.|.....}.d
-0000a350: 017d 0174 027c 0083 016a 0374 046a 056b  .}.t.|...j.t.j.k
-0000a360: 0272 3474 007c 006a 0683 017d 0264 027d  .r4t.|.j...}.d.}
-0000a370: 0157 006e 1c01 0001 0001 007c 0164 006b  .W.n.......|.d.k
-0000a380: 0872 4e64 037d 0264 047d 0159 006e 0258  .rNd.}.d.}.Y.n.X
-0000a390: 007c 027c 0166 0253 00a9 054e da06 6c65  .|.|.f.S...N..le
-0000a3a0: 6e67 7468 7a06 7368 6170 6520 da04 4e6f  ngthz.shape ..No
-0000a3b0: 6e65 7a06 4e6f 6e65 2020 a907 72a9 0000  nez.None  ..r...
-0000a3c0: 0072 3000 0000 7218 0100 0072 7201 0000  .r0...r....rr...
-0000a3d0: 721d 0000 0072 7301 0000 7221 0000 00a9  r....rs...r!....
-0000a3e0: 035a 0478 5f69 6e5a 0977 6869 6368 5f6f  .Z.x_inZ.which_o
-0000a3f0: 6e65 5a10 6c65 6e5f 6f72 5f73 6861 7065  neZ.len_or_shape
-0000a400: 5f6f 7574 7216 0000 0072 1600 0000 7217  _outr....r....r.
-0000a410: 0000 00da 1067 6574 5f6c 656e 5f6f 725f  .....get_len_or_
-0000a420: 7368 6170 65fa 0600 0073 1800 0000 0001  shape....s......
-0000a430: 0401 0201 0c01 0401 1001 0a01 0801 0601  ................
-0000a440: 0801 0401 0a01 7a29 6765 745f 636c 6173  ......z)get_clas
-0000a450: 735f 696e 666f 322e 3c6c 6f63 616c 733e  s_info2.<locals>
-0000a460: 2e67 6574 5f6c 656e 5f6f 725f 7368 6170  .get_len_or_shap
-0000a470: 6546 7201 0000 00da 015f fa02 632e fa01  eFr......_..c...
-0000a480: 27e9 feff ffff 724a 0000 0072 8701 0000  '.....rJ...r....
-0000a490: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-0000a4a0: 0003 0000 0073 0000 0073 1600 0000 7c00  .....s...s....|.
-0000a4b0: 5d0e 7d01 7400 7c01 8301 5600 0100 7102  ].}.t.|...V...q.
-0000a4c0: 6400 5300 7209 0100 0072 4800 0000 7231  d.S.r....rH...r1
-0000a4d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-0000a4e0: 0000 72d4 0000 001d 0700 0073 0400 0000  ..r........s....
-0000a4f0: 0400 0200 7a22 6765 745f 636c 6173 735f  ....z"get_class_
-0000a500: 696e 666f 322e 3c6c 6f63 616c 733e 2e3c  info2.<locals>.<
-0000a510: 6765 6e65 7870 723e 6301 0000 0000 0000  genexpr>c.......
-0000a520: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
-0000a530: 0073 1600 0000 7c00 5d0e 7d01 7400 7c01  .s....|.].}.t.|.
-0000a540: 8301 5600 0100 7102 6400 5300 7209 0100  ..V...q.d.S.r...
-0000a550: 0072 4800 0000 7231 0000 0072 1600 0000  .rH...r1...r....
-0000a560: 7216 0000 0072 1700 0000 72d4 0000 001e  r....r....r.....
-0000a570: 0700 0073 0400 0000 0400 0200 6301 0000  ...s........c...
-0000a580: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-0000a590: 0073 0000 0073 1600 0000 7c00 5d0e 7d01  .s...s....|.].}.
-0000a5a0: 7400 7c01 8301 5600 0100 7102 6400 5300  t.|...V...q.d.S.
-0000a5b0: 7209 0100 0072 4800 0000 7231 0000 0072  r....rH...r1...r
-0000a5c0: 1600 0000 7216 0000 0072 1700 0000 72d4  ....r....r....r.
-0000a5d0: 0000 001f 0700 0073 0400 0000 0400 0200  .......s........
-0000a5e0: 7218 0100 0072 3000 0000 7221 0000 0072  r....r0...r!...r
-0000a5f0: 1401 0000 2901 da08 6361 7465 676f 7279  ....)...category
-0000a600: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-0000a610: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
-0000a620: 7c00 5d0c 7d01 7400 7c01 8301 9102 7104  |.].}.t.|.....q.
-0000a630: 5300 7216 0000 0029 01da 0465 7661 6c72  S.r....)...evalr
-0000a640: 3100 0000 7216 0000 0072 1600 0000 7217  1...r....r....r.
-0000a650: 0000 0072 3400 0000 2607 0000 7304 0000  ...r4...&...s...
-0000a660: 0006 0002 007a 2367 6574 5f63 6c61 7373  .....z#get_class
-0000a670: 5f69 6e66 6f32 2e3c 6c6f 6361 6c73 3e2e  _info2.<locals>.
-0000a680: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-0000a690: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-0000a6a0: 0000 0073 1600 0000 6700 7c00 5d0e 7d01  ...s....g.|.].}.
-0000a6b0: 7400 a001 7c01 a101 9102 7104 5300 7216  t...|.....q.S.r.
-0000a6c0: 0000 0029 0272 1d00 0000 720f 0100 0029  ...).r....r....)
-0000a6d0: 0272 3200 0000 5a03 6969 6972 1600 0000  .r2...Z.iiir....
-0000a6e0: 7216 0000 0072 1700 0000 7234 0000 0028  r....r....r4...(
-0000a6f0: 0700 0073 0400 0000 0600 0200 72b2 0100  ...s........r...
-0000a700: 00fa 032e 2e2e fa02 3e20 fa0a 2074 7970  ........> .. typ
-0000a710: 652d 3e20 2020 fa02 2020 fa05 2d3e 2020  e->   ..  ..->  
-0000a720: 2029 12da 0364 6972 72a9 0000 0072 1801   )...dirr....r..
-0000a730: 0000 72e7 0100 0072 2300 0000 72d7 0000  ..r....r#...r...
-0000a740: 0072 0f01 0000 721d 0000 0072 b000 0000  .r....r....r....
-0000a750: 7230 0000 0072 1901 0000 7286 0000 0072  r0...r....r....r
-0000a760: 8b00 0000 da0e 6669 6c74 6572 7761 726e  ......filterwarn
-0000a770: 696e 6773 da19 5669 7369 626c 6544 6570  ings..VisibleDep
-0000a780: 7265 6361 7469 6f6e 5761 726e 696e 6772  recationWarningr
-0000a790: 3800 0000 7222 0000 0072 4b00 0000 2918  8...r"...rK...).
-0000a7a0: 72e2 0000 005a 0773 6f72 745f 6279 da17  r....Z.sort_by..
-0000a7b0: 696e 636c 7564 655f 756e 6465 7273 636f  include_undersco
-0000a7c0: 7265 5f76 6172 73da 1472 6574 7572 6e5f  re_vars..return_
-0000a7d0: 6e61 6d65 5f61 6e64 5f74 7970 65da 0c65  name_and_type..e
-0000a7e0: 6e64 5f70 7265 765f 6c65 6e72 e101 0000  nd_prev_lenr....
-0000a7f0: da05 6e61 6d65 73da 0c6c 656e 5f6f 725f  ..names..len_or_
-0000a800: 7368 6170 65da 166c 656e 5f6f 725f 7368  shape..len_or_sh
-0000a810: 6170 655f 7768 6963 685f 6f6e 65da 0d74  ape_which_one..t
-0000a820: 7970 655f 746f 5f70 7269 6e74 7233 0000  ype_to_printr3..
-0000a830: 0072 f700 0000 72e1 0000 0072 4200 0000  .r....r....rB...
-0000a840: 728e 0100 00da 0e6c 656e 5f73 7061 6365  r......len_space
-0000a850: 5f74 7970 65da 0f6c 656e 5f73 7061 6365  _type..len_space
-0000a860: 5f73 6861 7065 da09 696e 645f 6172 7261  _shape..ind_arra
-0000a870: 7972 2c00 0000 72b9 0000 0072 ba00 0000  yr,...r....r....
-0000a880: da02 6b35 7253 0000 0072 8c01 0000 7216  ..k5rS...r....r.
-0000a890: 0000 0072 1600 0000 7217 0000 0072 7401  ...r....r....rt.
-0000a8a0: 0000 f906 0000 7366 0000 0000 0108 0e04  ......sf........
-0000a8b0: 0104 0104 0104 020c 0114 0214 0114 010a  ................
-0000a8c0: 0118 010a 010c 0104 0114 0114 010a 0118  ................
-0000a8d0: 010a 010c 0116 0116 0116 010a 0110 010e  ................
-0000a8e0: 010c 011c 0112 0114 010e 010e 010c 010e  ................
-0000a8f0: 010c 020e 0208 0108 0108 0108 0110 0108  ................
-0000a900: 0114 0114 0114 010e 0114 0212 0130 0106  .............0..
-0000a910: 0172 7401 0000 6305 0000 0000 0000 0000  .rt...c.........
-0000a920: 0000 0018 0000 0006 0000 0043 0000 0073  ...........C...s
-0000a930: 4402 0000 6401 6402 8400 7d05 6700 7d06  D...d.d...}.g.}.
-0000a940: 6700 7d07 6700 7d08 6700 7d09 7400 7c00  g.}.g.}.g.}.t.|.
-0000a950: 8301 4400 5dda 7d0a 7c02 6403 6b08 7298  ..D.].}.|.d.k.r.
-0000a960: 7c0a 6404 1900 6405 6b03 7298 7401 7402  |.d...d.k.r.t.t.
-0000a970: 7403 6406 7c0a 1700 8301 8301 8301 7d0b  t.d.|.........}.
-0000a980: 7c09 a004 7c0b a005 6407 a101 6408 1900  |...|...d...d...
-0000a990: a101 0100 7c06 a004 7c0a a101 0100 7c05  ....|...|.....|.
-0000a9a0: 7403 6406 7c06 6409 1900 1700 8301 8301  t.d.|.d.........
-0000a9b0: 5c02 7d0c 7d0d 7c07 a004 7c0c a101 0100  \.}.}.|...|.....
-0000a9c0: 7c08 a004 7c0d a101 0100 7120 7c02 7220  |...|.....q |.r 
-0000a9d0: 7401 7402 7403 6406 7c0a 1700 8301 8301  t.t.t.d.|.......
-0000a9e0: 8301 7d0b 7c09 a004 7c0b a005 6407 a101  ..}.|...|...d...
-0000a9f0: 6408 1900 a101 0100 7c06 a004 7c0a a101  d.......|...|...
-0000aa00: 0100 7c05 7403 6406 7c06 6409 1900 1700  ..|.t.d.|.d.....
-0000aa10: 8301 8301 5c02 7d0c 7d0d 7c07 a004 7c0c  ....\.}.}.|...|.
-0000aa20: a101 0100 7c08 a004 7c0d a101 0100 7120  ....|...|.....q 
-0000aa30: 640a 7406 640b 640c 8400 7c06 4400 8301  d.t.d.d...|.D...
-0000aa40: 8301 1400 7d0e 640a 7406 640d 640c 8400  ....}.d.t.d.d...
-0000aa50: 7c09 4400 8301 8301 1400 7d0f 640a 7406  |.D.......}.d.t.
-0000aa60: 640e 640c 8400 7c07 4400 8301 8301 1400  d.d...|.D.......
-0000aa70: 7d10 7c01 9001 7250 7407 a008 7c09 a101  }.|...rPt...|...
-0000aa80: 7d11 6e0a 7407 a008 7c06 a101 7d11 7c11  }.n.t...|...}.|.
-0000aa90: 4400 5dd2 7d12 7c06 7c12 1900 7d13 7c09  D.].}.|.|...}.|.
-0000aaa0: 7c12 1900 7d14 7c07 7c12 1900 7d15 7403  |...}.|.|...}.t.
-0000aab0: 6406 7c06 7c12 1900 1700 8301 7d16 7401  d.|.|.......}.t.
-0000aac0: 7c16 8301 7d17 7c13 7c0e 1700 6400 7409  |...}.|.|...d.t.
-0000aad0: 7c0e 8301 8502 1900 7d13 7c14 7c0f 1700  |.......}.|.|...
-0000aae0: 6400 7409 7c0f 8301 8502 1900 7d14 7c15  d.t.|.......}.|.
-0000aaf0: 7c10 1700 6400 7409 7c10 8301 8502 1900  |...d.t.|.......
-0000ab00: 7d15 7409 7c17 8301 7c04 6b04 9001 72f0  }.t.|...|.k...r.
-0000ab10: 640f 7c17 7c04 0b00 6400 8502 1900 1700  d.|.|...d.......
-0000ab20: 7d17 6e12 6410 7c17 7c04 0b00 6400 8502  }.n.d.|.|...d...
-0000ab30: 1900 1700 7d17 740a 7c13 6411 1700 7c14  ....}.t.|.d...|.
-0000ab40: 1700 6412 1700 7c08 7c12 1900 1700 6413  ..d...|.|.....d.
-0000ab50: 1700 7c15 1700 6412 1700 7c17 1700 8301  ..|...d...|.....
-0000ab60: 0100 9001 715e 7c03 9002 7240 7c06 7c09  ....q^|...r@|.|.
-0000ab70: 6602 5300 6400 5300 2914 4e63 0100 0000  f.S.d.S.).Nc....
-0000ab80: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-0000ab90: 5300 0000 735c 0000 0064 007d 017a 3274  S...s\...d.}.z2t
-0000aba0: 0074 017c 0083 0183 017d 0264 017d 0174  .t.|.....}.d.}.t
-0000abb0: 027c 0083 016a 0374 046a 056b 0272 3474  .|...j.t.j.k.r4t
-0000abc0: 007c 006a 0683 017d 0264 027d 0157 006e  .|.j...}.d.}.W.n
-0000abd0: 1c01 0001 0001 007c 0164 006b 0872 4e64  .......|.d.k.rNd
-0000abe0: 037d 0264 047d 0159 006e 0258 007c 027c  .}.d.}.Y.n.X.|.|
-0000abf0: 0166 0253 0072 dc01 0000 72df 0100 0072  .f.S.r....r....r
-0000ac00: e001 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-0000ac10: 0000 0072 e101 0000 4207 0000 7318 0000  ...r....B...s...
-0000ac20: 0000 0104 0102 010c 0104 0110 010a 0108  ................
-0000ac30: 0106 0108 0104 010a 017a 2867 6574 5f63  .........z(get_c
-0000ac40: 6c61 7373 5f69 6e66 6f2e 3c6c 6f63 616c  lass_info.<local
-0000ac50: 733e 2e67 6574 5f6c 656e 5f6f 725f 7368  s>.get_len_or_sh
-0000ac60: 6170 6546 7201 0000 0072 e201 0000 72e3  apeFr....r....r.
-0000ac70: 0100 0072 e401 0000 72e5 0100 0072 4a00  ...r....r....rJ.
-0000ac80: 0000 7287 0100 0063 0100 0000 0000 0000  ..r....c........
-0000ac90: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-0000aca0: 7316 0000 007c 005d 0e7d 0174 007c 0183  s....|.].}.t.|..
-0000acb0: 0156 0001 0071 0264 0053 0072 0901 0000  .V...q.d.S.r....
-0000acc0: 7248 0000 0072 3100 0000 7216 0000 0072  rH...r1...r....r
-0000acd0: 1600 0000 7217 0000 0072 d400 0000 6507  ....r....r....e.
-0000ace0: 0000 7304 0000 0004 0002 007a 2167 6574  ..s........z!get
-0000acf0: 5f63 6c61 7373 5f69 6e66 6f2e 3c6c 6f63  _class_info.<loc
-0000ad00: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
-0000ad10: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-0000ad20: 0000 0073 0000 0073 1600 0000 7c00 5d0e  ...s...s....|.].
-0000ad30: 7d01 7400 7c01 8301 5600 0100 7102 6400  }.t.|...V...q.d.
-0000ad40: 5300 7209 0100 0072 4800 0000 7231 0000  S.r....rH...r1..
-0000ad50: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-0000ad60: 72d4 0000 0066 0700 0073 0400 0000 0400  r....f...s......
-0000ad70: 0200 6301 0000 0000 0000 0000 0000 0002  ..c.............
-0000ad80: 0000 0003 0000 0073 0000 0073 1600 0000  .......s...s....
-0000ad90: 7c00 5d0e 7d01 7400 7c01 8301 5600 0100  |.].}.t.|...V...
-0000ada0: 7102 6400 5300 7209 0100 0072 4800 0000  q.d.S.r....rH...
-0000adb0: 7231 0000 0072 1600 0000 7216 0000 0072  r1...r....r....r
-0000adc0: 1700 0000 72d4 0000 0067 0700 0073 0400  ....r....g...s..
-0000add0: 0000 0400 0200 72e8 0100 0072 e901 0000  ......r....r....
-0000ade0: 72ea 0100 0072 eb01 0000 72ec 0100 0029  r....r....r....)
-0000adf0: 0b72 ed01 0000 72a9 0000 0072 1801 0000  .r....r....r....
-0000ae00: 72e7 0100 0072 2300 0000 72d7 0000 0072  r....r#...r....r
-0000ae10: 0f01 0000 721d 0000 0072 8600 0000 7230  ....r....r....r0
-0000ae20: 0000 0072 4b00 0000 2918 72e2 0000 00da  ...rK...).r.....
-0000ae30: 0c73 6f72 745f 6279 5f74 7970 6572 f001  .sort_by_typer..
-0000ae40: 0000 72f1 0100 0072 f201 0000 72e1 0100  ..r....r....r...
-0000ae50: 0072 f301 0000 72f4 0100 0072 f501 0000  .r....r....r....
-0000ae60: 72f6 0100 0072 3300 0000 72f7 0000 0072  r....r3...r....r
-0000ae70: e100 0000 7242 0000 0072 8e01 0000 72f7  ....rB...r....r.
-0000ae80: 0100 0072 f801 0000 72f9 0100 0072 2c00  ...r....r....r,.
-0000ae90: 0000 72b9 0000 0072 ba00 0000 72fa 0100  ..r....r....r...
-0000aea0: 0072 5300 0000 728c 0100 0072 1600 0000  .rS...r....r....
-0000aeb0: 7216 0000 0072 1700 0000 da0e 6765 745f  r....r......get_
-0000aec0: 636c 6173 735f 696e 666f 4107 0000 7352  class_infoA...sR
-0000aed0: 0000 0000 0108 0e04 0104 0104 0104 020c  ................
-0000aee0: 0114 0214 0114 010a 0118 010a 010c 0104  ................
-0000aef0: 0114 0114 010a 0118 010a 010c 0116 0116  ................
-0000af00: 0116 0106 010c 020a 0208 0108 0108 0108  ................
-0000af10: 0110 0108 0114 0114 0114 010e 0114 0212  ................
-0000af20: 0130 0106 0172 fc01 0000 6305 0000 0000  .0...r....c.....
-0000af30: 0000 0000 0000 0012 0000 0009 0000 0043  ...............C
-0000af40: 0000 0073 1202 0000 6700 7d05 6700 7d06  ...s....g.}.g.}.
-0000af50: 7c00 a000 a100 4400 5d86 7d07 7c02 6401  |.....D.].}.|.d.
-0000af60: 6b08 7260 7401 7c07 8301 6402 1900 6403  k.r`t.|...d...d.
-0000af70: 6b03 7260 7401 7402 7c00 7c07 1900 8301  k.r`t.t.|.|.....
-0000af80: 8301 7d08 7c06 a003 7c08 a004 6404 a101  ..}.|...|...d...
-0000af90: 6405 1900 a101 0100 7c05 a003 7401 7c07  d.......|...t.|.
-0000afa0: 8301 a101 0100 7110 7c02 7210 7401 7402  ......q.|.r.t.t.
-0000afb0: 7c00 7c07 1900 8301 8301 7d08 7c06 a003  |.|.......}.|...
-0000afc0: 7c08 a004 6404 a101 6405 1900 a101 0100  |...d...d.......
-0000afd0: 7c05 a003 7401 7c07 8301 a101 0100 7110  |...t.|.......q.
-0000afe0: 6406 7405 6407 6408 8400 7c05 4400 8301  d.t.d.d...|.D...
-0000aff0: 8301 1400 7d09 6406 7405 6409 6408 8400  ....}.d.t.d.d...
-0000b000: 7c06 4400 8301 8301 1400 7d0a 7c01 72d4  |.D.......}.|.r.
-0000b010: 7406 a007 7c06 a101 7d0b 6e0a 7406 a007  t...|...}.n.t...
-0000b020: 7c05 a101 7d0b 7c0b 4400 9001 5d1a 7d0c  |...}.|.D...].}.
-0000b030: 7c05 7c0c 1900 7d0d 7c06 7c0c 1900 7d0e  |.|...}.|.|...}.
-0000b040: 7a14 7401 7c00 7c05 7c0c 1900 1900 8301  z.t.|.|.|.......
-0000b050: 7d0f 5700 6e20 0100 0100 0100 7401 7c00  }.W.n ......t.|.
-0000b060: 7408 7c05 7c0c 1900 8301 1900 8301 7d0f  t.|.|.........}.
-0000b070: 5900 6e02 5800 7c0d 7c09 1700 6400 7409  Y.n.X.|.|...d.t.
-0000b080: 7c09 8301 8502 1900 7d0d 7c0e 7c0a 1700  |.......}.|.|...
-0000b090: 6400 7409 7c0a 8301 8502 1900 7d0e 7409  d.t.|.......}.t.
-0000b0a0: 7c0f 8301 7c04 6b04 9001 7278 640a 7c0f  |...|.k...rxd.|.
-0000b0b0: 7c04 0b00 6400 8502 1900 1700 7d0f 6e12  |...d.......}.n.
-0000b0c0: 640b 7c0f 7c04 0b00 6400 8502 1900 1700  d.|.|...d.......
-0000b0d0: 7d0f 640c 7c0e 6b06 9001 72ac 7401 7c00  }.d.|.k...r.t.|.
-0000b0e0: 7c05 7c0c 1900 1900 6a0a 8301 7d10 640d  |.|.....j...}.d.
-0000b0f0: 7d11 6e32 7a1c 7401 7409 7c00 7c05 7c0c  }.n2z.t.t.|.|.|.
-0000b100: 1900 1900 8301 8301 7d10 640e 7d11 5700  ........}.d.}.W.
-0000b110: 6e14 0100 0100 0100 640f 7d11 6410 7d10  n.......d.}.d.}.
-0000b120: 5900 6e02 5800 740b 7c0d 6411 1700 7c0e  Y.n.X.t.|.d...|.
-0000b130: 1700 7c11 1700 7c10 1700 6412 1700 7c0f  ..|...|...d...|.
-0000b140: 1700 8301 0100 71e2 7c03 9002 720e 7c05  ......q.|...r.|.
-0000b150: 7c06 6602 5300 6400 5300 2913 4e46 7201  |.f.S.d.S.).NFr.
-0000b160: 0000 0072 e201 0000 72e4 0100 0072 e501  ...r....r....r..
-0000b170: 0000 7287 0100 0063 0100 0000 0000 0000  ..r....c........
-0000b180: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-0000b190: 7316 0000 007c 005d 0e7d 0174 007c 0183  s....|.].}.t.|..
-0000b1a0: 0156 0001 0071 0264 0053 0072 0901 0000  .V...q.d.S.r....
-0000b1b0: 7248 0000 0072 3100 0000 7216 0000 0072  rH...r1...r....r
-0000b1c0: 1600 0000 7217 0000 0072 d400 0000 8b07  ....r....r......
-0000b1d0: 0000 7304 0000 0004 0002 007a 2067 6574  ..s........z get
-0000b1e0: 5f64 6963 745f 696e 666f 2e3c 6c6f 6361  _dict_info.<loca
-0000b1f0: 6c73 3e2e 3c67 656e 6578 7072 3e63 0100  ls>.<genexpr>c..
-0000b200: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-0000b210: 0000 7300 0000 7316 0000 007c 005d 0e7d  ..s...s....|.].}
-0000b220: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
-0000b230: 0072 0901 0000 7248 0000 0072 3100 0000  .r....rH...r1...
-0000b240: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-0000b250: d400 0000 8c07 0000 7304 0000 0004 0002  ........s.......
-0000b260: 0072 e801 0000 72e9 0100 007a 0d6e 756d  .r....r....z.num
-0000b270: 7079 2e6e 6461 7272 6179 7a0b 2020 2073  py.ndarrayz.   s
-0000b280: 6861 7065 2d3e 207a 0920 2020 6c65 6e2d  hape-> z.   len-
-0000b290: 3e20 7a09 2020 204e 6f6e 652d 3e72 de01  > z.   None->r..
-0000b2a0: 0000 72ea 0100 0072 eb01 0000 290c 7295  ..r....r....).r.
-0000b2b0: 0000 0072 a900 0000 7218 0100 0072 2300  ...r....r....r#.
-0000b2c0: 0000 72d7 0000 0072 0f01 0000 721d 0000  ..r....r....r...
-0000b2d0: 0072 8600 0000 7285 0000 0072 3000 0000  .r....r....r0...
-0000b2e0: 7221 0000 0072 4b00 0000 2912 72e2 0000  r!...rK...).r...
-0000b2f0: 0072 fb01 0000 72f0 0100 0072 f101 0000  .r....r....r....
-0000b300: 72f2 0100 0072 f301 0000 72f6 0100 0072  r....r....r....r
-0000b310: 3300 0000 72f7 0000 0072 8e01 0000 72f7  3...r....r....r.
-0000b320: 0100 0072 f901 0000 722c 0000 0072 b900  ...r....r,...r..
-0000b330: 0000 72ba 0000 0072 8c01 0000 5a02 6b34  ..r....r....Z.k4
-0000b340: 5a06 6b34 5f73 7472 7216 0000 0072 1600  Z.k4_strr....r..
-0000b350: 0000 7217 0000 0072 7001 0000 7f07 0000  ..r....rp.......
-0000b360: 7350 0000 0000 0104 0104 010c 0118 0110  sP..............
-0000b370: 0114 0110 0104 0110 0114 0110 0116 0116  ................
-0000b380: 0104 010c 020a 020a 0108 0108 0102 0114  ................
-0000b390: 0106 011a 0114 0114 020e 0114 0212 020a  ................
-0000b3a0: 0112 0106 0202 0114 0108 0106 0104 010a  ................
-0000b3b0: 0222 0106 0172 7001 0000 6302 0000 0000  ."...rp...c.....
-0000b3c0: 0000 0000 0000 0009 0000 0004 0000 0043  ...............C
-0000b3d0: 0000 0073 b600 0000 6700 7d02 6700 7d03  ...s....g.}.g.}.
-0000b3e0: 7c02 7d04 7c03 7d05 6401 7d06 7400 7c00  |.}.|.}.d.}.t.|.
-0000b3f0: 8301 4400 5d62 5c02 7d07 7d08 7c08 7c06  ..D.]b\.}.}.|.|.
-0000b400: 6b02 724c 7401 a002 7c08 a101 7376 7c02  k.rLt...|...sv|.
-0000b410: a003 7c08 a101 0100 7c03 a003 7c07 a101  ..|.....|...|...
-0000b420: 0100 6e2a 7401 a002 7c08 a101 7376 7c08  ..n*t...|...sv|.
-0000b430: 6701 7d02 7c07 6701 7d03 7c04 a003 7c02  g.}.|.g.}.|...|.
-0000b440: a101 0100 7c05 a003 7c03 a101 0100 7c08  ....|...|.....|.
-0000b450: 7c01 1700 7d06 711c 7c04 6700 6b02 728a  |...}.q.|.g.k.r.
-0000b460: 6e24 7c04 6402 1900 6700 6b02 72ae 7c04  n$|.d...g.k.r.|.
-0000b470: 6403 6401 8502 1900 7d04 7c05 6403 6401  d.d.....}.|.d.d.
-0000b480: 8502 1900 7d05 7c04 7c05 6602 5300 2904  ....}.|.|.f.S.).
-0000b490: 7a7a 0a0a 2020 2020 5061 7261 6d65 7465  zz..    Paramete
-0000b4a0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000b4b0: 2d0a 2020 2020 7661 6c73 203a 0a20 2020  -.    vals :.   
-0000b4c0: 2020 2020 200a 2020 2020 7374 6570 203a       .    step :
-0000b4d0: 0a20 2020 2020 2020 2020 2844 6566 6175  .         (Defau
-0000b4e0: 6c74 2076 616c 7565 203d 2031 290a 0a20  lt value = 1).. 
-0000b4f0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-0000b500: 2d2d 2d2d 2d2d 0a0a 2020 2020 4e72 0100  ------..    Nr..
-0000b510: 0000 722e 0000 0029 0472 2400 0000 721d  ..r....).r$...r.
-0000b520: 0000 0072 da00 0000 7223 0000 0029 09da  ...r....r#...)..
-0000b530: 0476 616c 7372 ec00 0000 da03 7275 6e5a  .valsr......runZ
-0000b540: 0772 756e 5f69 6e64 da06 7265 7375 6c74  .run_ind..result
-0000b550: 5a0a 7265 7375 6c74 5f69 6e64 5a06 6578  Z.result_indZ.ex
-0000b560: 7065 6374 7233 0000 00da 0176 7216 0000  pectr3.....vr...
-0000b570: 0072 1600 0000 7217 0000 0072 3b00 0000  .r....r....r;...
-0000b580: da07 0000 732c 0000 0000 0e04 0104 0104  ....s,..........
-0000b590: 0104 0104 0110 0108 010a 030a 010c 020a  ................
-0000b5a0: 0106 0106 010a 010a 010a 0208 0102 010c  ................
-0000b5b0: 010c 010c 0172 3b00 0000 6302 0000 0000  .....r;...c.....
-0000b5c0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-0000b5d0: 0000 0073 5600 0000 6700 7d02 7400 7c00  ...sV...g.}.t.|.
-0000b5e0: 7401 6a02 6a03 1700 8301 a004 6401 a101  t.j.j.......d...
-0000b5f0: 4400 5d22 7d03 7c02 a005 7406 7c03 6a07  D.]"}.|...t.|.j.
-0000b600: 8301 7401 6a02 6a03 1700 7c03 6a08 1700  ..t.j.j...|.j...
-0000b610: a101 0100 711a 7c02 a009 a100 0100 7c01  ....q.|.......|.
-0000b620: 7252 740a 7c02 8301 0100 7c02 5300 2902  rRt.|.....|.S.).
-0000b630: 7a56 0a0a 2020 2020 5061 7261 6d65 7465  zV..    Paramete
-0000b640: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000b650: 2d0a 2020 2020 6261 7365 5f64 6972 203a  -.    base_dir :
-0000b660: 0a20 2020 2020 2020 200a 0a20 2020 2052  .        ..    R
-0000b670: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0000b680: 2d2d 0a0a 2020 2020 7a04 2a2e 6835 290b  --..    z.*.h5).
-0000b690: 720e 0000 0072 5f00 0000 7261 0000 0072  r....r_...ra...r
-0000b6a0: 6000 0000 da05 7267 6c6f 6272 2300 0000  `.....rglobr#...
-0000b6b0: 72a9 0000 00da 0670 6172 656e 7472 b201  r......parentr..
-0000b6c0: 0000 7261 0100 0072 c701 0000 2904 72b6  ..ra...r....).r.
-0000b6d0: 0000 005a 0d70 7269 6e74 5f68 355f 6c69  ...Z.print_h5_li
-0000b6e0: 7374 5a0c 4835 5f66 696c 655f 6c69 7374  stZ.H5_file_list
-0000b6f0: 7261 0000 0072 1600 0000 7216 0000 0072  ra...r....r....r
-0000b700: 1700 0000 7225 0100 0004 0800 0073 0e00  ....r%.......s..
-0000b710: 0000 000c 0401 1a01 2001 0801 0401 0801  ........ .......
-0000b720: 7225 0100 0063 0200 0000 0000 0000 0000  r%...c..........
-0000b730: 0000 0400 0000 0700 0000 4300 0000 7360  ..........C...s`
-0000b740: 0000 0074 007c 007c 0183 0244 005d 485c  ...t.|.|...D.]H\
-0000b750: 027d 027d 037a 1e7c 03a0 0174 026a 036a  .}.}.z.|...t.j.j
-0000b760: 04a1 0164 0119 007c 026b 0673 2e74 0582  ...d...|.k.s.t..
-0000b770: 0157 0071 0a01 0001 0001 0074 0664 0283  .W.q.......t.d..
-0000b780: 0101 0064 0364 046b 0273 4c74 0582 0159  ...d.d.k.sLt...Y
-0000b790: 0071 0a58 0071 0a74 0664 0583 0101 0064  .q.X.q.t.d.....d
-0000b7a0: 0653 0029 077a 740a 0a20 2020 2050 6172  .S.).zt..    Par
-0000b7b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0000b7c0: 2d2d 2d2d 2d2d 0a20 2020 2048 355f 6c69  ------.    H5_li
-0000b7d0: 7374 5f4c 4142 203a 0a20 2020 2020 2020  st_LAB :.       
-0000b7e0: 200a 2020 2020 4835 5f6c 6973 745f 494d   .    H5_list_IM
-0000b7f0: 4720 3a0a 2020 2020 2020 2020 0a0a 2020  G :.        ..  
-0000b800: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0000b810: 2d2d 2d2d 2d0a 0a20 2020 2072 4a00 0000  -----..    rJ...
-0000b820: 7a43 444f 204e 4f54 2043 4f4e 5449 4e55  zCDO NOT CONTINU
-0000b830: 4520 2d2d 2d20 736f 6d65 2066 696c 6573  E --- some files
-0000b840: 2064 6f20 6e6f 7420 6d61 7463 6820 6f6e   do not match on
-0000b850: 2079 6f75 7220 6c69 7374 7320 7472 7920   your lists try 
-0000b860: 6167 6169 6e72 2e00 0000 7201 0000 007a  againr....r....z
-0000b870: 1379 6179 2074 6865 7920 616c 6c20 6d61  .yay they all ma
-0000b880: 7463 6821 4e29 0772 ac00 0000 72d7 0000  tch!N).r....r...
-0000b890: 0072 5f00 0000 7261 0000 0072 6000 0000  .r_...ra...r`...
-0000b8a0: 724e 0000 0072 4b00 0000 2904 5a0b 4835  rN...rK...).Z.H5
-0000b8b0: 5f6c 6973 745f 4c41 425a 0b48 355f 6c69  _list_LABZ.H5_li
-0000b8c0: 7374 5f49 4d47 5a06 6835 5f4c 4142 5a06  st_IMGZ.h5_LABZ.
-0000b8d0: 6835 5f49 4d47 7216 0000 0072 1600 0000  h5_IMGr....r....
-0000b8e0: 7217 0000 00da 1963 6865 636b 5f69 665f  r......check_if_
-0000b8f0: 6669 6c65 5f6c 6973 7473 5f6d 6174 6368  file_lists_match
-0000b900: 1908 0000 730e 0000 0000 0e12 0102 011e  ....s...........
-0000b910: 0106 0108 0114 0172 0302 0000 6301 0000  .......r....c...
-0000b920: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-0000b930: 0043 0000 0073 1600 0000 6401 6402 8400  .C...s....d.d...
-0000b940: 7400 7c00 8301 4400 8301 7d01 6403 5300  t.|...D...}.d.S.
-0000b950: 2904 7a55 0a0a 2020 2020 5061 7261 6d65  ).zU..    Parame
-0000b960: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000b970: 2d2d 2d0a 2020 2020 6c69 7374 5f69 6e20  ---.    list_in 
-0000b980: 3a0a 2020 2020 2020 2020 0a0a 2020 2020  :.        ..    
-0000b990: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000b9a0: 2d2d 2d0a 0a20 2020 2063 0100 0000 0000  ---..    c......
-0000b9b0: 0000 0000 0000 0300 0000 0700 0000 5300  ..............S.
-0000b9c0: 0000 7332 0000 0067 007c 005d 2a5c 027d  ..s2...g.|.]*\.}
-0000b9d0: 017d 0274 0074 017c 0183 0164 0017 007c  .}.t.t.|...d...|
-0000b9e0: 02a0 0274 036a 046a 05a1 0164 0119 0017  ...t.j.j...d....
-0000b9f0: 0083 0191 0271 0453 00a9 0272 8701 0000  .....q.S...r....
-0000ba00: 724a 0000 00a9 0672 4b00 0000 72a9 0000  rJ.....rK...r...
-0000ba10: 0072 d700 0000 725f 0000 0072 6100 0000  .r....r_...ra...
-0000ba20: 7260 0000 00a9 0372 3200 0000 722c 0000  r`.....r2...r,..
-0000ba30: 0072 3300 0000 7216 0000 0072 1600 0000  .r3...r....r....
-0000ba40: 7217 0000 0072 3400 0000 3c08 0000 7304  r....r4...<...s.
-0000ba50: 0000 0006 0006 007a 2870 7269 6e74 5f6c  .......z(print_l
-0000ba60: 6973 745f 7769 7468 5f69 6e64 732e 3c6c  ist_with_inds.<l
-0000ba70: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-0000ba80: 3e4e a901 7224 0000 0029 0272 1a01 0000  >N..r$...).r....
-0000ba90: 72e2 0100 0072 1600 0000 7216 0000 0072  r....r....r....r
-0000baa0: 1700 0000 72c7 0100 0030 0800 0073 0200  ....r....0...s..
-0000bab0: 0000 000c 72c7 0100 0063 0100 0000 0000  ....r....c......
-0000bac0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-0000bad0: 0000 7322 0000 0074 0064 0183 0101 0074  ..s"...t.d.....t
-0000bae0: 01a0 017c 0064 0217 00a1 017d 0174 027c  ...|.d.....}.t.|
-0000baf0: 0183 0101 007c 0153 0029 03fa 5c0a 0a20  .....|.S.)..\.. 
-0000bb00: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000bb10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000bb20: 206d 6f64 656c 5f73 6176 655f 6469 7220   model_save_dir 
-0000bb30: 3a0a 2020 2020 2020 2020 0a0a 2020 2020  :.        ..    
-0000bb40: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000bb50: 2d2d 2d0a 0a20 2020 20fa 2a54 6865 7365  ---..    .*These
-0000bb60: 2061 7265 2061 6c6c 2074 6865 206d 6f64   are all the mod
-0000bb70: 656c 7320 746f 2063 686f 6f73 6520 6672  els to choose fr
-0000bb80: 6f6d 2e2e 2efa 072f 2a2e 636b 7074 2903  om...../*.ckpt).
-0000bb90: 724b 0000 0072 af01 0000 72c7 0100 0029  rK...r....r....)
-0000bba0: 02da 0e6d 6f64 656c 5f73 6176 655f 6469  ...model_save_di
-0000bbb0: 72da 106d 6f64 656c 5f32 5f6c 6f61 645f  r..model_2_load_
-0000bbc0: 616c 6c72 1600 0000 7216 0000 0072 1700  allr....r....r..
-0000bbd0: 0000 da0e 6765 745f 6d6f 6465 6c5f 6c69  ....get_model_li
-0000bbe0: 7374 3f08 0000 7308 0000 0000 0c08 010e  st?...s.........
-0000bbf0: 0108 0172 0d02 0000 6302 0000 0000 0000  ...r....c.......
-0000bc00: 0000 0000 0006 0000 0006 0000 0043 0000  .............C..
-0000bc10: 0073 5c00 0000 6700 7d02 7400 a001 7c00  .s\...g.}.t...|.
-0000bc20: a101 4400 5d26 5c03 7d03 7d04 7d05 7402  ..D.]&\.}.}.}.t.
-0000bc30: a002 7c03 6401 1700 7c01 1700 a101 720e  ..|.d...|.....r.
-0000bc40: 7c02 a003 7c03 a101 0100 710e 7a0c 7404  |...|.....q.z.t.
-0000bc50: 7c02 8301 7d02 5700 6e14 0100 0100 0100  |...}.W.n.......
-0000bc60: 7405 7c02 8301 7d02 5900 6e02 5800 7c02  t.|...}.Y.n.X.|.
-0000bc70: 5300 2902 6157 0100 0065 6e74 6572 2062  S.).aW...enter b
-0000bc80: 6173 6520 6469 7265 6374 6f72 7920 616e  ase directory an
-0000bc90: 6420 7365 6172 6368 2074 6572 6d20 746f  d search term to
-0000bca0: 2066 696e 6420 616c 6c20 7468 6520 6469   find all the di
-0000bcb0: 7265 6374 6f72 6965 7320 696e 2062 6173  rectories in bas
-0000bcc0: 6520 6469 7265 6374 6f72 790a 2020 2020  e directory.    
-0000bcd0: 2020 7769 7468 2066 696c 6573 206d 6174    with files mat
-0000bce0: 6368 696e 6720 7468 6520 7365 6172 6368  ching the search
-0000bcf0: 5f74 6572 6d2e 206f 7574 7075 7420 6120  _term. output a 
-0000bd00: 736f 7274 6564 206c 6973 7420 6f66 2064  sorted list of d
-0000bd10: 6972 6563 746f 7269 6573 2e0a 2020 2020  irectories..    
-0000bd20: 2020 652e 672e 202d 3e20 7265 6375 7273    e.g. -> recurs
-0000bd30: 6976 655f 6469 725f 6669 6e64 6572 2827  ive_dir_finder('
-0000bd40: 2f63 6f6e 7465 6e74 2f6d 7964 726f 7062  /content/mydropb
-0000bd50: 6f78 2f27 2c20 272a 2e6d 7034 2729 0a0a  ox/', '*.mp4')..
-0000bd60: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000bd70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000bd80: 2020 6261 7365 5f70 6174 6820 3a0a 2020    base_path :.  
-0000bd90: 2020 2020 2020 0a20 2020 2073 6561 7263        .    searc
-0000bda0: 685f 7465 726d 203a 0a20 2020 2020 2020  h_term :.       
-0000bdb0: 200a 0a20 2020 2052 6574 7572 6e73 0a20   ..    Returns. 
-0000bdc0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-0000bdd0: 7251 0100 0029 0672 5f00 0000 da04 7761  rQ...).r_.....wa
-0000bde0: 6c6b 72af 0100 0072 2300 0000 7206 0000  lkr....r#...r...
-0000bdf0: 0072 cf00 0000 2906 da09 6261 7365 5f70  .r....)...base_p
-0000be00: 6174 68da 0b73 6561 7263 685f 7465 726d  ath..search_term
-0000be10: 5a10 6d61 7463 6869 6e67 5f66 6f6c 6465  Z.matching_folde
-0000be20: 7273 da04 726f 6f74 da04 6469 7273 da05  rs..root..dirs..
-0000be30: 6669 6c65 7372 1600 0000 7216 0000 0072  filesr....r....r
-0000be40: 1700 0000 da14 7265 6375 7273 6976 655f  ......recursive_
-0000be50: 6469 725f 6669 6e64 6572 5108 0000 7312  dir_finderQ...s.
-0000be60: 0000 0000 1004 0114 0112 010c 0102 010c  ................
-0000be70: 0106 010e 0172 1402 0000 6301 0000 0000  .....r....c.....
-0000be80: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-0000be90: 0000 0073 3000 0000 7400 6401 8301 0100  ...s0...t.d.....
-0000bea0: 7401 7402 a002 7c00 6402 1700 a101 8301  t.t...|.d.......
-0000beb0: 7d01 6403 6404 8400 7403 7c01 8301 4400  }.d.d...t.|...D.
-0000bec0: 8301 7d02 7c01 5300 2905 7208 0200 0072  ..}.|.S.).r....r
-0000bed0: 0902 0000 720a 0200 0063 0100 0000 0000  ....r....c......
-0000bee0: 0000 0000 0000 0300 0000 0700 0000 5300  ..............S.
-0000bef0: 0000 7332 0000 0067 007c 005d 2a5c 027d  ..s2...g.|.]*\.}
-0000bf00: 017d 0274 0074 017c 0183 0164 0017 007c  .}.t.t.|...d...|
-0000bf10: 02a0 0274 036a 046a 05a1 0164 0119 0017  ...t.j.j...d....
-0000bf20: 0083 0191 0271 0453 0072 0402 0000 7205  .....q.S.r....r.
-0000bf30: 0200 0072 0602 0000 7216 0000 0072 1600  ...r....r....r..
-0000bf40: 0000 7217 0000 0072 3400 0000 7b08 0000  ..r....r4...{...
-0000bf50: 7304 0000 0006 0006 007a 2267 6574 5f6d  s........z"get_m
-0000bf60: 6f64 656c 5f6c 6973 742e 3c6c 6f63 616c  odel_list.<local
-0000bf70: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
-0000bf80: 4b00 0000 72cf 0000 0072 af01 0000 7224  K...r....r....r$
-0000bf90: 0000 0029 0372 0b02 0000 720c 0200 0072  ...).r....r....r
-0000bfa0: e201 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-0000bfb0: 0000 0072 0d02 0000 6c08 0000 7308 0000  ...r....l...s...
-0000bfc0: 0000 0c08 0112 0212 0163 0200 0000 0000  .........c......
-0000bfd0: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-0000bfe0: 0000 7348 0000 0067 007d 0274 007c 0074  ..sH...g.}.t.|.t
-0000bff0: 016a 0217 0083 01a0 037c 01a1 0144 005d  .j.......|...D.]
-0000c000: 227d 037c 02a0 0474 057c 036a 0683 0174  "}.|...t.|.j...t
-0000c010: 016a 076a 0217 007c 036a 0817 00a1 0101  .j.j...|.j......
-0000c020: 0071 187c 02a0 09a1 0001 007c 0253 0029  .q.|.......|.S.)
-0000c030: 0161 db01 0000 0a62 6173 655f 6469 7220  .a.....base_dir 
-0000c040: 3d20 272f 636f 6e74 656e 742f 6764 7269  = '/content/gdri
-0000c050: 7665 2f4d 7920 4472 6976 652f 4c49 4748  ve/My Drive/LIGH
-0000c060: 545f 4742 4d2f 4645 4154 5552 455f 4441  T_GBM/FEATURE_DA
-0000c070: 5441 2f27 0a6e 756d 5f66 6f6c 6465 7273  TA/'.num_folders
-0000c080: 5f64 6565 7020 3d20 310a 6669 6c65 5f6c  _deep = 1.file_l
-0000c090: 6973 7420 3d20 5b5d 0a66 6f72 2069 2c20  ist = [].for i, 
-0000c0a0: 7061 7468 2069 6e20 656e 756d 6572 6174  path in enumerat
-0000c0b0: 6528 5061 7468 2862 6173 655f 6469 7220  e(Path(base_dir 
-0000c0c0: 2b20 6f73 2e73 6570 292e 7267 6c6f 6228  + os.sep).rglob(
-0000c0d0: 2727 2929 3a0a 2020 7820 3d20 7374 7228  '')):.  x = str(
-0000c0e0: 7061 7468 2e70 6172 656e 7429 202b 206f  path.parent) + o
-0000c0f0: 732e 7061 7468 2e73 6570 202b 2070 6174  s.path.sep + pat
-0000c100: 682e 6e61 6d65 0a20 2069 6620 6920 3d3d  h.name.  if i ==
-0000c110: 303a 0a20 2020 2066 696c 655f 6c69 7374  0:.    file_list
-0000c120: 2e61 7070 656e 6428 7829 0a20 2020 2063  .append(x).    c
-0000c130: 6e74 203d 206c 656e 2878 2e73 706c 6974  nt = len(x.split
-0000c140: 286f 732e 7365 7029 290a 2020 6966 2028  (os.sep)).  if (
-0000c150: 6c65 6e28 782e 7370 6c69 7428 6f73 2e73  len(x.split(os.s
-0000c160: 6570 2929 2d63 6e74 293c 3d6e 756d 5f66  ep))-cnt)<=num_f
-0000c170: 6f6c 6465 7273 5f64 6565 703a 0a20 2020  olders_deep:.   
-0000c180: 2066 696c 655f 6c69 7374 2e61 7070 656e   file_list.appen
-0000c190: 6428 7829 0a6c 6973 7428 7365 7428 6669  d(x).list(set(fi
-0000c1a0: 6c65 5f6c 6973 7429 290a 0a20 2020 2050  le_list))..    P
-0000c1b0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0000c1c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2062 6173  --------.    bas
-0000c1d0: 655f 6469 7220 3a0a 2020 2020 2020 2020  e_dir :.        
-0000c1e0: 0a20 2020 2073 6561 7263 685f 7465 726d  .    search_term
-0000c1f0: 203a 0a0a 2020 2020 5265 7475 726e 730a   :..    Returns.
-0000c200: 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020      -------..   
-0000c210: 2029 0a72 0e00 0000 725f 0000 0072 6000   ).r....r_...r`.
-0000c220: 0000 7201 0200 0072 2300 0000 72a9 0000  ..r....r#...r...
-0000c230: 0072 0202 0000 7261 0000 0072 b201 0000  .r....ra...r....
-0000c240: 7261 0100 0029 0472 b600 0000 7210 0200  ra...).r....r...
-0000c250: 00da 0966 696c 655f 6c69 7374 7261 0000  ...file_listra..
-0000c260: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-0000c270: 7292 0100 007f 0800 0073 0a00 0000 0018  r........s......
-0000c280: 0401 1802 2001 0801 7292 0100 0063 0100  .... ...r....c..
-0000c290: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-0000c2a0: 0000 4300 0000 7318 0000 0074 006a 017c  ..C...s....t.j.|
-0000c2b0: 0064 0164 0264 038d 037d 0174 027c 0183  .d.d.d...}.t.|..
-0000c2c0: 0153 0029 0461 f501 0000 7468 6973 2066  .S.).a....this f
-0000c2d0: 756e 6374 696f 6e20 7368 6f75 6c64 2062  unction should b
-0000c2e0: 6520 6361 6c6c 6564 2069 6e73 7465 6164  e called instead
-0000c2f0: 206f 6620 6469 7265 6374 2073 7069 6f2e   of direct spio.
-0000c300: 6c6f 6164 6d61 740a 2020 2020 6173 2069  loadmat.    as i
-0000c310: 7420 6375 7265 7320 7468 6520 7072 6f62  t cures the prob
-0000c320: 6c65 6d20 6f66 206e 6f74 2070 726f 7065  lem of not prope
-0000c330: 726c 7920 7265 636f 7665 7269 6e67 2070  rly recovering p
-0000c340: 7974 686f 6e20 6469 6374 696f 6e61 7269  ython dictionari
-0000c350: 6573 0a20 2020 2066 726f 6d20 6d61 7420  es.    from mat 
-0000c360: 6669 6c65 732e 2049 7420 6361 6c6c 7320  files. It calls 
-0000c370: 7468 6520 6675 6e63 7469 6f6e 2063 6865  the function che
-0000c380: 636b 206b 6579 7320 746f 2063 7572 6520  ck keys to cure 
-0000c390: 616c 6c20 656e 7472 6965 730a 2020 2020  all entries.    
-0000c3a0: 7768 6963 6820 6172 6520 7374 696c 6c20  which are still 
-0000c3b0: 6d61 742d 6f62 6a65 6374 730a 0a20 2020  mat-objects..   
-0000c3c0: 2069 6620 7468 6973 2064 6f65 736e 7420   if this doesnt 
-0000c3d0: 776f 726b 2074 7279 2074 6869 730a 2020  work try this.  
-0000c3e0: 2020 696d 706f 7274 206d 6174 3733 0a20    import mat73. 
-0000c3f0: 2020 2066 726f 6d20 7768 6163 6320 696d     from whacc im
-0000c400: 706f 7274 2075 7469 6c73 0a20 2020 206d  port utils.    m
-0000c410: 6174 5f66 696c 6520 3d20 272f 5573 6572  at_file = '/User
-0000c420: 732f 7068 696c 2f44 726f 7062 6f78 2f55  s/phil/Dropbox/U
-0000c430: 5f31 3931 3032 385f 3131 3534 2e6d 6174  _191028_1154.mat
-0000c440: 270a 2020 2020 6461 7461 5f64 6963 7420  '.    data_dict 
-0000c450: 3d20 6d61 7437 332e 6c6f 6164 6d61 7428  = mat73.loadmat(
-0000c460: 6d61 745f 6669 6c65 290a 0a20 2020 2050  mat_file)..    P
-0000c470: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0000c480: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 696c  --------.    fil
-0000c490: 656e 616d 6520 3a0a 2020 2020 2020 2020  ename :.        
-0000c4a0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0000c4b0: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2046    -------..    F
-0000c4c0: 5429 025a 1073 7472 7563 745f 6173 5f72  T).Z.struct_as_r
-0000c4d0: 6563 6f72 645a 0a73 7175 6565 7a65 5f6d  ecordZ.squeeze_m
-0000c4e0: 6529 03da 0473 7069 6fda 076c 6f61 646d  e)...spio..loadm
-0000c4f0: 6174 da0b 5f63 6865 636b 5f6b 6579 7329  at.._check_keys)
-0000c500: 0272 7b00 0000 722a 0000 0072 1600 0000  .r{...r*...r....
-0000c510: 7216 0000 0072 1700 0000 7217 0200 00a9  r....r....r.....
-0000c520: 0800 0073 0400 0000 0015 1001 7217 0200  ...s........r...
-0000c530: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-0000c540: 0000 0400 0000 4300 0000 7332 0000 007c  ......C...s2...|
-0000c550: 0044 005d 287d 0174 007c 007c 0119 0074  .D.](}.t.|.|...t
-0000c560: 016a 026a 036a 0483 0272 0474 057c 007c  .j.j.j...r.t.|.|
-0000c570: 0119 0083 017c 007c 013c 0071 047c 0053  .....|.|.<.q.|.S
-0000c580: 0029 017a c463 6865 636b 7320 6966 2065  .).z.checks if e
-0000c590: 6e74 7269 6573 2069 6e20 6469 6374 696f  ntries in dictio
-0000c5a0: 6e61 7279 2061 7265 206d 6174 2d6f 626a  nary are mat-obj
-0000c5b0: 6563 7473 2e20 4966 2079 6573 0a20 2020  ects. If yes.   
-0000c5c0: 2074 6f64 6963 7420 6973 2063 616c 6c65   todict is calle
-0000c5d0: 6420 746f 2063 6861 6e67 6520 7468 656d  d to change them
-0000c5e0: 2074 6f20 6e65 7374 6564 2064 6963 7469   to nested dicti
-0000c5f0: 6f6e 6172 6965 730a 0a20 2020 2050 6172  onaries..    Par
-0000c600: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0000c610: 2d2d 2d2d 2d2d 0a20 2020 2064 6963 7420  ------.    dict 
-0000c620: 3a0a 2020 2020 2020 2020 0a0a 2020 2020  :.        ..    
-0000c630: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000c640: 2d2d 2d0a 0a20 2020 2029 0672 0701 0000  ---..    ).r....
-0000c650: 7216 0200 00da 066d 6174 6c61 62da 0b6d  r......matlab..m
-0000c660: 696f 355f 7061 7261 6d73 da0a 6d61 745f  io5_params..mat_
-0000c670: 7374 7275 6374 da07 5f74 6f64 6963 7429  struct.._todict)
-0000c680: 0272 6800 0000 da03 6b65 7972 1600 0000  .rh.....keyr....
-0000c690: 7216 0000 0072 1700 0000 7218 0200 00c2  r....r....r.....
-0000c6a0: 0800 0073 0800 0000 000d 0801 1401 1201  ...s............
-0000c6b0: 7218 0200 0063 0100 0000 0000 0000 0000  r....c..........
-0000c6c0: 0000 0400 0000 0400 0000 4300 0000 7344  ..........C...sD
-0000c6d0: 0000 0069 007d 017c 006a 0044 005d 347d  ...i.}.|.j.D.]4}
-0000c6e0: 027c 006a 017c 0219 007d 0374 027c 0374  .|.j.|...}.t.|.t
-0000c6f0: 036a 046a 056a 0683 0272 3674 077c 0383  .j.j.j...r6t.|..
-0000c700: 017c 017c 023c 0071 0a7c 037c 017c 023c  .|.|.<.q.|.|.|.<
-0000c710: 0071 0a7c 0153 0029 017a 9d41 2072 6563  .q.|.S.).z.A rec
-0000c720: 7572 7369 7665 2066 756e 6374 696f 6e20  ursive function 
-0000c730: 7768 6963 6820 636f 6e73 7472 7563 7473  which constructs
-0000c740: 2066 726f 6d20 6d61 746f 626a 6563 7473   from matobjects
-0000c750: 206e 6573 7465 6420 6469 6374 696f 6e61   nested dictiona
-0000c760: 7269 6573 0a0a 2020 2020 5061 7261 6d65  ries..    Parame
-0000c770: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000c780: 2d2d 2d0a 2020 2020 6d61 746f 626a 203a  ---.    matobj :
-0000c790: 0a20 2020 2020 2020 200a 0a20 2020 2052  .        ..    R
-0000c7a0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0000c7b0: 2d2d 0a0a 2020 2020 2908 5a0b 5f66 6965  --..    ).Z._fie
-0000c7c0: 6c64 6e61 6d65 73da 085f 5f64 6963 745f  ldnames..__dict_
-0000c7d0: 5f72 0701 0000 7216 0200 0072 1902 0000  _r....r....r....
-0000c7e0: 721a 0200 0072 1b02 0000 721c 0200 0029  r....r....r....)
-0000c7f0: 045a 066d 6174 6f62 6a72 6800 0000 da04  .Z.matobjrh.....
-0000c800: 7374 7267 da04 656c 656d 7216 0000 0072  strg..elemr....r
-0000c810: 1600 0000 7217 0000 0072 1c02 0000 d508  ....r....r......
-0000c820: 0000 730e 0000 0000 0c04 010a 010a 0110  ..s.............
-0000c830: 010e 020a 0172 1c02 0000 6302 0000 0000  .....r....c.....
-0000c840: 0000 0000 0000 0005 0000 0009 0000 0003  ................
-0000c850: 0000 0073 9e00 0000 6700 7d02 7c00 4400  ...s....g.}.|.D.
-0000c860: 5d2a 8900 7c02 a000 7401 7402 a003 8700  ]*..|...t.t.....
-0000c870: 6601 6401 6402 8408 7c00 4400 8301 a101  f.d.d...|.D.....
-0000c880: 6403 1900 8301 a101 0100 7108 7a34 7401  d.........q.z4t.
-0000c890: 7402 6a04 7c02 6403 6404 8d02 8301 7d03  t.j.|.d.d.....}.
-0000c8a0: 7405 7c03 8301 4400 5d14 5c02 7d04 8900  t.|...D.].\.}...
-0000c8b0: 7401 8800 8301 7c03 7c04 3c00 7150 5700  t.....|.|.<.qPW.
-0000c8c0: 6e1a 0100 0100 0100 7401 7402 a004 7c02  n.......t.t...|.
-0000c8d0: a101 8301 7d03 5900 6e02 5800 7c01 7296  ....}.Y.n.X.|.r.
-0000c8e0: 7c03 7406 a004 7c00 a101 6602 5300 7c03  |.t...|...f.S.|.
-0000c8f0: 5300 6400 5300 2905 4e63 0100 0000 0000  S.d.S.).Nc......
-0000c900: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-0000c910: 0000 7314 0000 0067 007c 005d 0c7d 0188  ..s....g.|.].}..
-0000c920: 007c 016b 0291 0271 0453 0072 1600 0000  .|.k...q.S.r....
-0000c930: 7216 0000 0029 0272 3200 0000 da02 6b6b  r....).r2.....kk
-0000c940: a901 7233 0000 0072 1600 0000 7217 0000  ..r3...r....r...
-0000c950: 0072 3400 0000 ee08 0000 7304 0000 0006  .r4.......s.....
-0000c960: 0002 007a 2467 6574 5f69 6e64 735f 6f66  ...z$get_inds_of
-0000c970: 5f69 6e64 732e 3c6c 6f63 616c 733e 2e3c  _inds.<locals>.<
-0000c980: 6c69 7374 636f 6d70 3e72 0100 0000 72fb  listcomp>r....r.
-0000c990: 0000 0029 0772 2300 0000 7239 0000 0072  ...).r#...r9...r
-0000c9a0: 1d00 0000 72b5 0000 0072 ce00 0000 7224  ....r....r....r$
-0000c9b0: 0000 0072 9b01 0000 2905 72e1 0000 005a  ...r....).r....Z
-0000c9c0: 1272 6574 7572 6e5f 756e 6971 7565 5f6c  .return_unique_l
-0000c9d0: 6973 74da 0261 32da 0c69 6e64 735f 6f66  ist..a2..inds_of
-0000c9e0: 5f69 6e64 7372 2c00 0000 7216 0000 0072  _indsr,...r....r
-0000c9f0: 2202 0000 7217 0000 00da 1067 6574 5f69  "...r......get_i
-0000ca00: 6e64 735f 6f66 5f69 6e64 73eb 0800 0073  nds_of_inds....s
-0000ca10: 1800 0000 0001 0401 0801 2801 0201 1201  ..........(.....
-0000ca20: 1001 1201 0601 1401 0401 0e02 7225 0200  ............r%..
-0000ca30: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-0000ca40: 0000 0700 0000 4300 0000 737a 0000 007c  ......C...sz...|
-0000ca50: 0164 011b 0074 007c 0164 011b 0083 016b  .d...t.|.d.....k
-0000ca60: 0373 1c74 0164 0283 0182 0174 02a0 0374  .s.t.d.....t...t
-0000ca70: 02a0 047c 0064 0364 03a1 03a1 017d 027c  ...|.d.d.....}.|
-0000ca80: 027c 0164 0485 0219 007c 0264 047c 010b  .|.d.....|.d.|..
-0000ca90: 0085 0219 0018 0074 057c 0183 011b 007d  .......t.|.....}
-0000caa0: 0374 02a0 067c 0364 036b 04a1 0164 0319  .t...|.d.k...d..
-0000cab0: 007c 0164 0518 0064 011b 0017 007d 037c  .|.d...d.....}.|
-0000cac0: 03a0 0764 06a1 0153 0029 077a e80a 0a20  ...d...S.).z... 
-0000cad0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000cae0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000caf0: 2078 203a 2061 7272 6179 0a20 2020 204e   x : array.    N
-0000cb00: 203a 2077 696e 646f 7720 7369 7a65 0a0a   : window size..
-0000cb10: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000cb20: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 7475  -------.    retu
-0000cb30: 726e 7320 696e 6469 6365 7320 6f66 2061  rns indices of a
-0000cb40: 7272 6179 7320 7768 6572 6520 6172 7261  rrays where arra
-0000cb50: 7920 3e30 2077 6974 6820 626f 7264 6572  y >0 with border
-0000cb60: 7320 6f66 2028 284e 202d 2031 2920 2f20  s of ((N - 1) / 
-0000cb70: 3229 2c20 736f 2078 203d 205b 302c 2030  2), so x = [0, 0
-0000cb80: 2c20 302c 2031 2c20 302c 2030 2c20 305d  , 0, 1, 0, 0, 0]
-0000cb90: 2061 6e64 204e 203d 2033 0a20 2020 2072   and N = 3.    r
-0000cba0: 6574 7572 6e73 205b 322c 2033 2c20 345d  eturns [2, 3, 4]
-0000cbb0: 0a20 2020 2072 4700 0000 7a4d 4e20 6d75  .    rG...zMN mu
-0000cbc0: 7374 2062 6520 616e 206f 6464 206e 756d  st be an odd num
-0000cbd0: 6265 7220 736f 2074 6861 7420 7468 6572  ber so that ther
-0000cbe0: 6520 6172 6520 6571 7561 6c20 6e75 6d62  e are equal numb
-0000cbf0: 6572 206f 6620 706f 696e 7473 206f 6e20  er of points on 
-0000cc00: 6561 6368 2073 6964 6572 0100 0000 4e72  each sider....Nr
-0000cc10: 2e00 0000 7284 0000 0029 0872 8800 0000  ....r....).r....
-0000cc20: 724e 0000 0072 1d00 0000 7264 0100 00da  rN...r....rd....
-0000cc30: 0669 6e73 6572 7472 8500 0000 72b5 0000  .insertr....r...
-0000cc40: 0072 8100 0000 2904 7253 0000 00da 014e  .r....).rS.....N
-0000cc50: 7264 0100 0072 e100 0000 7216 0000 0072  rd...r....r....r
-0000cc60: 1600 0000 7217 0000 00da 1069 6e64 735f  ....r......inds_
-0000cc70: 6172 6f75 6e64 5f69 6e64 73fb 0800 0073  around_inds....s
-0000cc80: 0a00 0000 000d 1c01 1401 2201 1e01 7228  .........."...r(
-0000cc90: 0200 0063 0200 0000 0000 0000 0000 0000  ...c............
-0000cca0: 0200 0000 0600 0000 4300 0000 7370 0000  ........C...sp..
-0000ccb0: 0074 007c 0083 017d 0064 0167 017c 0017  .t.|...}.d.g.|..
-0000ccc0: 007d 0074 01a0 027c 00a1 017d 007c 00a0  .}.t...|...}.|..
-0000ccd0: 0374 04a1 017d 007c 0172 4a74 007c 0064  .t...}.|.rJt.|.d
-0000cce0: 0264 0385 0219 0083 0174 007c 0064 0464  .d.......t.|.d.d
-0000ccf0: 0285 0219 0083 0167 0253 0074 0574 007c  .......g.S.t.t.|
-0000cd00: 0064 0264 0385 0219 0083 0174 007c 0064  .d.d.......t.|.d
-0000cd10: 0464 0285 0219 0083 0183 0253 0064 0253  .d.........S.d.S
-0000cd20: 0029 0561 ab01 0000 0a0a 2020 2020 5061  .).a......    Pa
-0000cd30: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0000cd40: 2d2d 2d2d 2d2d 2d0a 2020 2020 6672 616d  -------.    fram
-0000cd50: 655f 6e75 6d5f 6172 7261 7920 3a0a 2020  e_num_array :.  
-0000cd60: 2020 6e75 6d20 6f66 2066 7261 6d65 7320    num of frames 
-0000cd70: 696e 2065 6163 6820 7472 6961 6c20 696e  in each trial in
-0000cd80: 2061 206c 6973 740a 2020 2020 5265 7475   a list.    Retu
-0000cd90: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0000cda0: 2020 2020 3220 6c69 7374 7320 7769 7468      2 lists with
-0000cdb0: 2074 6865 2070 726f 7065 7220 696e 6465   the proper inde
-0000cdc0: 7820 666f 7220 7075 6c6c 696e 6720 7468  x for pulling th
-0000cdd0: 6f73 6520 7472 6961 6c73 206f 7574 206f  ose trials out o
-0000cde0: 6e65 2062 7920 6f6e 6520 696e 2061 2066  ne by one in a f
-0000cdf0: 6f72 206c 6f6f 700a 2020 2020 4578 616d  or loop.    Exam
-0000ce00: 706c 6573 0a20 2020 205f 5f5f 5f5f 5f5f  ples.    _______
-0000ce10: 5f0a 2020 2020 6133 203d 205b 302c 2031  _.    a3 = [0, 1
-0000ce20: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
-0000ce30: 2037 2c20 385d 0a20 2020 2066 7261 6d65   7, 8].    frame
-0000ce40: 5f6e 756d 5f61 7272 6179 203d 205b 342c  _num_array = [4,
-0000ce50: 2035 5d0a 2020 2020 666f 7220 6931 2c20   5].    for i1, 
-0000ce60: 6932 2069 6e20 6c6f 6f70 5f73 6567 6d65  i2 in loop_segme
-0000ce70: 6e74 7328 6672 616d 655f 6e75 6d5f 6172  nts(frame_num_ar
-0000ce80: 7261 7929 3a0a 2020 2020 2020 2020 7072  ray):.        pr
-0000ce90: 696e 7428 6133 5b69 313a 6932 5d29 0a0a  int(a3[i1:i2])..
-0000cea0: 2020 2020 2320 3e3e 3e5b 302c 2031 2c20      # >>>[0, 1, 
-0000ceb0: 322c 2033 5d0a 2020 2020 2320 3e3e 3e5b  2, 3].    # >>>[
-0000cec0: 342c 2035 2c20 362c 2037 2c20 385d 0a20  4, 5, 6, 7, 8]. 
-0000ced0: 2020 2072 0100 0000 4e72 4a00 0000 722e     r....NrJ...r.
-0000cee0: 0000 0029 0672 3900 0000 721d 0000 0072  ...).r9...r....r
-0000cef0: 6401 0000 7281 0000 0072 8400 0000 72ac  d...r....r....r.
-0000cf00: 0000 0029 025a 0f66 7261 6d65 5f6e 756d  ...).Z.frame_num
-0000cf10: 5f61 7272 6179 5a0c 7265 7475 726e 6173  _arrayZ.returnas
-0000cf20: 6c69 7374 7216 0000 0072 1600 0000 7217  listr....r....r.
-0000cf30: 0000 0072 3700 0000 0f09 0000 730e 0000  ...r7.......s...
-0000cf40: 0000 1408 010a 010a 010a 0104 0120 0272  ............. .r
-0000cf50: 3700 0000 6302 0000 0000 0000 0000 0000  7...c...........
-0000cf60: 000d 0000 000b 0000 0043 0000 0073 ec00  .........C...s..
-0000cf70: 0000 6700 7d02 6401 6402 8400 7c00 4400  ..g.}.d.d...|.D.
-0000cf80: 8301 7d03 7400 7c03 6403 8302 5c02 7d04  ..}.t.|.d...\.}.
-0000cf90: 7d05 6404 6402 8400 7c00 4400 8301 7d06  }.d.d...|.D...}.
-0000cfa0: 7401 a002 7c06 a101 7401 a002 7c04 a101  t...|...t...|...
-0000cfb0: 1900 7d06 7403 7c04 8301 4400 5d7a 5c02  ..}.t.|...D.]z\.
-0000cfc0: 7d07 7d08 7401 a004 6700 a101 7d09 7403  }.}.t...g...}.t.
-0000cfd0: 7c08 8301 4400 5d54 5c02 7d0a 7d0b 7405  |...D.]T\.}.}.t.
-0000cfe0: a006 7c00 7c0b 1900 6405 a102 8f36 7d0c  ..|.|...d....6}.
-0000cff0: 7c09 6a07 729e 7401 a008 7c09 7c0c 6406  |.j.r.t...|.|.d.
-0000d000: 1900 6407 6407 8502 1900 6702 a101 6e0e  ..d.d.....g...n.
-0000d010: 7c0c 6406 1900 6407 6407 8502 1900 7d09  |.d...d.d.....}.
-0000d020: 5700 3500 5100 5200 5800 7164 7c02 a009  W.5.Q.R.X.qd|...
-0000d030: 7c09 a101 0100 714a 7c01 72e0 7c02 7c05  |.....qJ|.r.|.|.
-0000d040: 7c06 6408 6407 6407 8502 6602 1900 6603  |.d.d.d...f...f.
-0000d050: 5300 7c02 7c05 6602 5300 6407 5300 2909  S.|.|.f.S.d.S.).
-0000d060: 7a92 0a20 2020 206a 7573 7420 7573 6564  z..    just used
-0000d070: 2074 6f20 6765 7420 6172 7261 7920 6f66   to get array of
-0000d080: 2063 6f6e 7461 6374 732c 206e 6f74 206d   contacts, not m
-0000d090: 6561 6e74 2074 6f20 6265 2075 7365 6420  eant to be used 
-0000d0a0: 6c6f 6e67 2074 6572 6d0a 2020 2020 5061  long term.    Pa
-0000d0b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0000d0c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 616c 6c5f  -------.    all_
-0000d0d0: 6835 7320 3a0a 0a20 2020 2052 6574 7572  h5s :..    Retur
-0000d0e0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  ns.    -------..
-0000d0f0: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-0000d100: 0002 0000 0006 0000 0053 0000 0073 2c00  .........S...s,.
-0000d110: 0000 6700 7c00 5d24 7d01 7c01 a000 7401  ..g.|.]$}.|...t.
-0000d120: 6a02 6a03 a101 6400 1900 6a00 6401 6402  j.j...d...j.d.d.
-0000d130: 6403 8d02 6400 1900 9102 7104 5300 2904  d...d.....q.S.).
-0000d140: 724a 0000 0072 e201 0000 722e 0000 0029  rJ...r....r....)
-0000d150: 01da 086d 6178 7370 6c69 7429 0472 d700  ...maxsplit).r..
-0000d160: 0000 725f 0000 0072 6100 0000 7260 0000  ..r_...ra...r`..
-0000d170: 0072 3100 0000 7216 0000 0072 1600 0000  .r1...r....r....
-0000d180: 7217 0000 0072 3400 0000 4c09 0000 7304  r....r4...L...s.
-0000d190: 0000 0006 0002 007a 285f 6765 745f 6875  .......z(_get_hu
-0000d1a0: 6d61 6e5f 636f 6e74 6163 7473 5f2e 3c6c  man_contacts_.<l
-0000d1b0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-0000d1c0: 3e54 6301 0000 0000 0000 0000 0000 0002  >Tc.............
-0000d1d0: 0000 0007 0000 0053 0000 0073 2000 0000  .......S...s ...
-0000d1e0: 6700 7c00 5d18 7d01 7400 6a01 a002 7400  g.|.].}.t.j...t.
-0000d1f0: 6a01 a003 7c01 a101 a101 9102 7104 5300  j...|.......q.S.
-0000d200: 7216 0000 0029 0472 5f00 0000 7261 0000  r....).r_...ra..
-0000d210: 0072 a400 0000 72a3 0000 0072 3100 0000  .r....r....r1...
-0000d220: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-0000d230: 3400 0000 4f09 0000 7304 0000 0006 0002  4...O...s.......
-0000d240: 0072 6d00 0000 7252 0000 004e 7201 0000  .rm...rR...Nr...
-0000d250: 0029 0a72 2502 0000 721d 0000 0072 3800  .).r%...r....r8.
-0000d260: 0000 7224 0000 00da 0561 7272 6179 72aa  ..r$.....arrayr.
-0000d270: 0000 0072 ab00 0000 722c 0100 0072 2500  ...r....r,...r%.
-0000d280: 0000 7223 0000 0029 0d5a 0761 6c6c 5f68  ..r#...).Z.all_h
-0000d290: 3573 5a14 7265 7475 726e 5f63 7572 6174  5sZ.return_curat
-0000d2a0: 6f72 5f6e 616d 6573 da06 685f 636f 6e74  or_names..h_cont
-0000d2b0: 72e1 0000 0072 2402 0000 5a12 6c69 7374  r....r$...Z.list
-0000d2c0: 5f6f 665f 756e 6971 5f66 696c 6573 5a0d  _of_uniq_filesZ.
-0000d2d0: 6375 7261 746f 725f 6e61 6d65 7372 2c00  curator_namesr,.
-0000d2e0: 0000 7233 0000 0072 f700 0000 723e 0000  ..r3...r....r>..
-0000d2f0: 0072 2102 0000 72bc 0000 0072 1600 0000  .r!...r....r....
-0000d300: 7216 0000 0072 1700 0000 da14 5f67 6574  r....r......_get
-0000d310: 5f68 756d 616e 5f63 6f6e 7461 6374 735f  _human_contacts_
-0000d320: 4009 0000 731c 0000 0000 0b04 010e 010e  @...s...........
-0000d330: 020e 0114 0110 010a 0110 0112 013c 010c  .............<..
-0000d340: 0104 0116 0272 2c02 0000 e950 0000 0063  .....r,....P...c
-0000d350: 0500 0000 0000 0000 0000 0000 1300 0000  ................
-0000d360: 0a00 0000 0300 0000 7318 0200 0067 007d  ........s....g.}
-0000d370: 0574 007c 017c 0283 0244 0090 015d bc5c  .t.|.|...D...].\
-0000d380: 027d 067d 0774 017c 076a 0283 0164 016b  .}.}.t.|.j...d.k
-0000d390: 0272 3474 03a0 047c 077c 0766 02a1 017d  .r4t...|.|.f...}
-0000d3a0: 0774 05a0 067c 0664 02a1 0290 018f 847d  .t...|.d.......}
-0000d3b0: 0874 036a 077c 0764 0364 048d 027d 0974  .t.j.|.d.d...}.t
-0000d3c0: 036a 087c 0764 0364 048d 027d 0a7c 0a64  .j.|.d.d...}.|.d
-0000d3d0: 056b 0464 0114 007d 0a74 097c 097c 0364  .k.d...}.t.|.|.d
-0000d3e0: 0614 0064 0117 0083 0289 0074 0a88 0083  ...d.......t....
-0000d3f0: 015c 027d 0b7d 0c7c 0b44 005d 127d 0d7c  .\.}.}.|.D.].}.|
-0000d400: 05a0 0b74 017c 0d83 01a1 0101 0071 8e87  ...t.|.......q..
-0000d410: 0066 0164 0764 0884 0874 03a0 0c74 0d64  .f.d.d...t...t.d
-0000d420: 097c 0464 0117 0083 02a1 0144 0083 017d  .|.d.......D...}
-0000d430: 0e7c 0e73 de74 0e64 0a74 0188 0083 0164  .|.s.t.d.t.....d
-0000d440: 0b7c 0464 0c67 0583 0182 0174 03a0 077c  .|.d.g.....t...|
-0000d450: 0ea1 017d 0e74 03a0 0f67 00a1 017d 0f74  ...}.t...g...}.t
-0000d460: 03a0 0f67 00a1 017d 1064 037d 1174 1088  ...g...}.d.}.t..
-0000d470: 0083 0144 005d ac7d 127c 1164 0137 007d  ...D.].}.|.d.7.}
-0000d480: 117c 0f6a 1190 0172 5c74 036a 127c 0f7c  .|.j...r\t.j.|.|
-0000d490: 0864 0d19 007c 1219 0064 0e64 0e64 0e85  .d...|...d.d.d..
-0000d4a0: 0264 0e64 0e85 0264 0366 0419 0066 0264  .d.d...d.f...f.d
-0000d4b0: 0364 048d 027d 0f74 03a0 0b7c 107c 097c  .d...}.t...|.|.|
-0000d4c0: 1219 00a1 027d 106e 287c 0864 0d19 007c  .....}.n(|.d...|
-0000d4d0: 1219 0064 0e64 0e64 0e85 0264 0e64 0e85  ...d.d.d...d.d..
-0000d4e0: 0264 0366 0419 007d 0f7c 0a7c 1219 007d  .d.f...}.|.|...}
-0000d4f0: 107c 117c 0e6b 0590 0172 087c 00a0 137c  .|.|.k...r.|...|
-0000d500: 0f7c 10a1 0201 0074 03a0 0f67 00a1 017d  .|.....t...g...}
-0000d510: 0f74 03a0 0f67 00a1 017d 1064 037d 1190  .t...g...}.d.}..
-0000d520: 0171 087c 00a0 137c 0f7c 10a1 0201 0057  .q.|...|.|.....W
-0000d530: 0035 0051 0052 0058 0071 0e74 05a0 067c  .5.Q.R.X.q.t...|
-0000d540: 006a 1464 0fa1 028f 327d 087c 086a 1564  .j.d....2}.|.j.d
-0000d550: 1074 03a0 027c 05a1 017c 0564 118d 0301  .t...|...|.d....
-0000d560: 007c 086a 1564 1274 03a0 0288 00a1 0188  .|.j.d.t........
-0000d570: 0064 118d 0301 0057 0035 0051 0052 0058  .d.....W.5.Q.R.X
-0000d580: 0064 0e53 0029 1361 7b05 0000 0a20 2020  .d.S.).a{....   
-0000d590: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000d5a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2068  ----------.    h
-0000d5b0: 3563 203a 2068 3520 6372 6561 746f 7220  5c : h5 creator 
-0000d5c0: 636c 6173 730a 2020 2020 616c 6c5f 6835  class.    all_h5
-0000d5d0: 735f 696d 6773 203a 206c 6973 7420 6f66  s_imgs : list of
-0000d5e0: 2068 3573 2077 6974 6820 696d 6167 6573   h5s with images
-0000d5f0: 0a20 2020 2068 5f63 6f6e 7420 3a20 6120  .    h_cont : a 
-0000d600: 7465 6e73 6f72 206f 6620 6875 6d61 6e20  tensor of human 
-0000d610: 636f 6e74 6163 7473 2070 656f 706c 6520  contacts people 
-0000d620: 6279 2066 7261 6d65 7320 7472 6961 6c20  by frames trial 
-0000d630: 4835 2066 696c 6573 2028 646f 776e 2072  H5 files (down r
-0000d640: 6967 6874 2064 6565 7029 0a20 2020 2062  ight deep).    b
-0000d650: 6f72 6465 7273 203a 2066 6f72 2074 6f75  orders : for tou
-0000d660: 6368 2030 3030 3030 3131 3130 3030 3030  ch 0000011100000
-0000d670: 2069 7420 7769 6c6c 2066 696e 6420 7468   it will find th
-0000d680: 6520 3131 3120 696e 2069 7420 616e 6420  e 111 in it and 
-0000d690: 6765 7420 616c 6c20 7468 6520 626f 7264  get all the bord
-0000d6a0: 6572 696e 6720 6172 6561 7320 6172 6f75  ering areas arou
-0000d6b0: 6e64 2069 742e 2070 6f69 6e74 7320 6172  nd it. points ar
-0000d6c0: 650a 2020 2020 756e 6971 7565 2073 6f20  e.    unique so 
-0000d6d0: 3030 3030 3031 3131 3030 3030 3020 616e  0000011100000 an
-0000d6e0: 6420 3030 3030 3031 3031 3030 3030 3020  d 0000010100000 
-0000d6f0: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
-0000d700: 7361 6d65 2069 6e64 6578 0a20 2020 206d  same index.    m
-0000d710: 6178 5f70 6163 6b5f 7661 6c20 3a20 7370  ax_pack_val : sp
-0000d720: 6565 6473 2075 7020 7468 6520 7072 6f63  eeds up the proc
-0000d730: 6573 7320 6279 2074 7261 6e73 6665 7272  ess by transferr
-0000d740: 696e 6720 6461 7461 2069 6e20 6368 756e  ing data in chun
-0000d750: 6b73 206f 6620 7468 6973 206d 6178 2073  ks of this max s
-0000d760: 697a 6520 696e 7374 6561 6420 6f66 2062  ize instead of b
-0000d770: 7569 6c64 696e 6720 7468 656d 2061 6c6c  uilding them all
-0000d780: 2075 7020 696e 206d 656d 6f72 790a 2020   up in memory.  
-0000d790: 2020 6974 2773 2061 206d 6178 2069 6e73    it's a max ins
-0000d7a0: 7465 6164 206f 6620 6120 7365 7420 7661  tead of a set va
-0000d7b0: 6c75 6520 6265 6361 7573 6520 6974 2063  lue because it c
-0000d7c0: 616e 2062 6520 6966 2074 6865 206c 656e  an be if the len
-0000d7d0: 2849 4d41 4745 5329 256d 6178 5f70 6163  (IMAGES)%max_pac
-0000d7e0: 6b5f 7661 6c20 6973 2065 7175 616c 2074  k_val is equal t
-0000d7f0: 6f20 3020 6f72 2031 2069 7420 7769 6c6c  o 0 or 1 it will
-0000d800: 2063 7261 7368 2c20 736f 2049 2063 616c   crash, so I cal
-0000d810: 6375 6c61 7465 2069 740a 2020 2020 736f  culate it.    so
-0000d820: 2074 6861 7420 6974 2077 6f6e 7420 6372   that it wont cr
-0000d830: 6173 682e 0a0a 2020 2020 5265 7475 726e  ash...    Return
-0000d840: 730a 2020 2020 2d2d 2d2d 2d2d 2d63 7265  s.    -------cre
-0000d850: 6174 655f 6d61 7374 6572 5f64 6174 6173  ate_master_datas
-0000d860: 6574 0a20 2020 2073 6176 6573 2061 6e20  et.    saves an 
-0000d870: 4835 2066 696c 650a 2020 2020 4578 616d  H5 file.    Exam
-0000d880: 706c 6573 0a20 2020 205f 5f5f 5f5f 5f5f  ples.    _______
-0000d890: 5f0a 0a20 2020 2061 6c6c 5f68 3573 203d  _..    all_h5s =
-0000d8a0: 2075 7469 6c73 2e67 6574 5f68 3573 2827   utils.get_h5s('
-0000d8b0: 2f63 6f6e 7465 6e74 2f67 6472 6976 652f  /content/gdrive/
-0000d8c0: 4d79 2044 7269 7665 2f43 6f6c 6162 2064  My Drive/Colab d
-0000d8d0: 6174 612f 6375 7261 7469 6f6e 5f66 6f72  ata/curation_for
-0000d8e0: 5f61 7574 6f5f 6375 7261 746f 722f 6669  _auto_curator/fi
-0000d8f0: 6e69 7368 6564 5f63 6f6e 7461 6374 732f  nished_contacts/
-0000d900: 2729 0a20 2020 2061 6c6c 5f68 3573 5f69  ').    all_h5s_i
-0000d910: 6d67 7320 3d20 7574 696c 732e 6765 745f  mgs = utils.get_
-0000d920: 6835 7328 272f 636f 6e74 656e 742f 6764  h5s('/content/gd
-0000d930: 7269 7665 2f4d 7920 4472 6976 652f 436f  rive/My Drive/Co
-0000d940: 6c61 6220 6461 7461 2f63 7572 6174 696f  lab data/curatio
-0000d950: 6e5f 666f 725f 6175 746f 5f63 7572 6174  n_for_auto_curat
-0000d960: 6f72 2f48 355f 6461 7461 2f27 290a 2020  or/H5_data/').  
-0000d970: 2020 685f 636f 6e74 203d 2075 7469 6c73    h_cont = utils
-0000d980: 2e5f 6765 745f 6875 6d61 6e5f 636f 6e74  ._get_human_cont
-0000d990: 6163 7473 5f28 616c 6c5f 6835 7329 0a20  acts_(all_h5s). 
-0000d9a0: 2020 2068 3563 203d 2069 6d61 6765 5f74     h5c = image_t
-0000d9b0: 6f6f 6c73 2e68 355f 6974 6572 6174 6976  ools.h5_iterativ
-0000d9c0: 655f 6372 6561 746f 7228 272f 636f 6e74  e_creator('/cont
-0000d9d0: 656e 742f 6764 7269 7665 2f4d 7920 4472  ent/gdrive/My Dr
-0000d9e0: 6976 652f 436f 6c61 6220 6461 7461 2f63  ive/Colab data/c
-0000d9f0: 7572 6174 696f 6e5f 666f 725f 6175 746f  uration_for_auto
-0000da00: 5f63 7572 6174 6f72 2f74 6573 745f 5f5f  _curator/test___
-0000da10: 5f5f 2e68 3527 2c0a 2020 2020 2020 2020  __.h5',.        
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da40: 2020 206f 7665 7277 7269 7465 5f69 665f     overwrite_if_
-0000da50: 6669 6c65 5f65 7869 7374 7320 3d20 5472  file_exists = Tr
-0000da60: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000da90: 6f6c 6f72 5f63 6861 6e6e 656c 203d 2046  olor_channel = F
-0000daa0: 616c 7365 290a 2020 2020 7574 696c 732e  alse).    utils.
-0000dab0: 6372 6561 7465 5f6d 6173 7465 725f 6461  create_master_da
-0000dac0: 7461 7365 7428 6835 632c 2061 6c6c 5f68  taset(h5c, all_h
-0000dad0: 3573 5f69 6d67 732c 2068 5f63 6f6e 742c  5s_imgs, h_cont,
-0000dae0: 2062 6f72 6465 7273 203d 2038 302c 206d   borders = 80, m
-0000daf0: 6178 5f70 6163 6b5f 7661 6c20 3d20 3130  ax_pack_val = 10
-0000db00: 3029 0a20 2020 2072 2e00 0000 726d 0000  0).    r....rm..
-0000db10: 0072 0100 0000 72fb 0000 0072 9800 0000  .r....r....r....
-0000db20: 7247 0000 0063 0100 0000 0000 0000 0000  rG...c..........
-0000db30: 0000 0200 0000 0400 0000 1300 0000 7320  ..............s 
-0000db40: 0000 0067 007c 005d 187d 0174 0088 0083  ...g.|.].}.t....
-0000db50: 017c 0116 0064 006b 0572 047c 0191 0271  .|...d.k.r.|...q
-0000db60: 0453 0029 0172 4700 0000 7248 0000 0072  .S.).rG...rH...r
-0000db70: 3100 0000 a901 7242 0000 0072 1600 0000  1.....rB...r....
-0000db80: 7217 0000 0072 3400 0000 8509 0000 7306  r....r4.......s.
-0000db90: 0000 0006 0002 0010 007a 2963 7265 6174  .........z)creat
-0000dba0: 655f 6d61 7374 6572 5f64 6174 6173 6574  e_master_dataset
-0000dbb0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-0000dbc0: 6f6d 703e 7246 0000 007a 1c63 686f 7365  omp>rF...z.chose
-0000dbd0: 6e20 4835 2066 696c 6520 6861 7320 7661  n H5 file has va
-0000dbe0: 6c75 6520 6f66 207a 1520 616e 6420 6d61  lue of z. and ma
-0000dbf0: 785f 7061 636b 5f76 616c 2069 7320 7a2c  x_pack_val is z,
-0000dc00: 2069 6e63 7265 6173 6520 6d61 785f 7061   increase max_pa
-0000dc10: 636b 5f76 616c 2074 6f20 7072 6576 656e  ck_val to preven
-0000dc20: 7420 7468 6973 2065 7272 6f72 7296 0000  t this errorr...
-0000dc30: 004e 72a2 0000 0072 4100 0000 72ca 0100  .Nr....rA...r...
-0000dc40: 005a 0e69 6e64 735f 6578 7472 6163 7465  .Z.inds_extracte
-0000dc50: 6429 1672 ac00 0000 7230 0000 0072 2100  d).r....r0...r!.
-0000dc60: 0000 721d 0000 0072 2500 0000 72aa 0000  ..r....r%...r...
-0000dc70: 0072 ab00 0000 720f 0100 0072 8300 0000  .r....r....r....
-0000dc80: 7228 0200 0072 3b00 0000 7223 0000 0072  r(...r;...r#...r
-0000dc90: 9301 0000 723a 0000 0072 4e00 0000 722a  ....r:...rN...r*
-0000dca0: 0200 0072 0b00 0000 722c 0100 0072 2600  ...r....r,...r&.
-0000dcb0: 0000 724a 0100 005a 1168 355f 6675 6c6c  ..rJ...Z.h5_full
-0000dcc0: 5f66 696c 655f 6e61 6d65 72ab 0100 0029  _file_namer....)
-0000dcd0: 1372 ad01 0000 5a0c 616c 6c5f 6835 735f  .r....Z.all_h5s_
-0000dce0: 696d 6773 722b 0200 00da 0762 6f72 6465  imgsr+.....borde
-0000dcf0: 7273 5a0c 6d61 785f 7061 636b 5f76 616c  rsZ.max_pack_val
-0000dd00: 7241 0000 0072 3300 0000 72ba 0000 0072  rA...r3...r....r
-0000dd10: bc00 0000 5a0f 6d61 785f 6875 6d61 6e5f  ....Z.max_human_
-0000dd20: 6c61 6265 6c5a 106d 6561 6e5f 6875 6d61  labelZ.mean_huma
-0000dd30: 6e5f 6c61 6265 6c72 f700 0000 72e2 0100  n_labelr....r...
-0000dd40: 0072 6e01 0000 5a0c 7061 636b 5f65 7665  .rn...Z.pack_eve
-0000dd50: 7279 5f78 da08 6e65 775f 696d 6773 5a0a  ry_x..new_imgsZ.
-0000dd60: 6e65 775f 6c61 6265 6c73 5a04 636e 7472  new_labelsZ.cntr
-0000dd70: 728c 0100 0072 1600 0000 722e 0200 0072  r....r....r....r
-0000dd80: 1700 0000 da15 6372 6561 7465 5f6d 6173  ......create_mas
-0000dd90: 7465 725f 6461 7461 7365 745d 0900 0073  ter_dataset]...s
-0000dda0: 4800 0000 001b 0401 1401 0e01 0e01 1001  H...............
-0000ddb0: 0e01 0e01 0c01 1201 0c01 0801 1002 2201  ..............".
-0000ddc0: 1201 02ff 0602 0a03 0a01 0a01 0401 0c01  ................
-0000ddd0: 0801 0801 2e01 1202 2001 0801 0a01 0c01  ........ .......
-0000dde0: 0a01 0a01 0801 1802 1001 1601 7231 0200  ............r1..
-0000ddf0: 0063 0100 0000 0000 0000 0000 0000 0600  .c..............
-0000de00: 0000 0700 0000 4300 0000 737a 0000 0064  ......C...sz...d
-0000de10: 0164 0284 007c 00a0 0064 03a1 0164 0464  .d...|...d...d.d
-0000de20: 0585 0219 0044 0083 017d 0174 0183 007d  .....D...}.t...}
-0000de30: 0264 047c 0264 063c 0064 077c 0264 083c  .d.|.d.<.d.|.d.<
-0000de40: 0064 097c 0264 0a3c 0067 007d 037c 0144  .d.|.d.<.g.}.|.D
-0000de50: 005d 327d 047c 04a0 0064 0ba1 0164 0c19  .]2}.|...d...d..
-0000de60: 007d 057c 03a0 0274 037c 04a0 0064 0ba1  .}.|...t.|...d..
-0000de70: 0164 0d19 0083 017c 027c 0519 0014 00a1  .d.....|.|......
-0000de80: 0101 0071 427c 0353 0029 0e75 8903 0000  ...qB|.S.).u....
-0000de90: 0a20 2045 7861 6d70 6c65 0a20 202d 2d2d  .  Example.  ---
-0000dea0: 2d2d 2d2d 0a20 2069 6d70 6f72 7420 7265  ----.  import re
-0000deb0: 0a20 2069 6d70 6f72 7420 6d61 7470 6c6f  .  import matplo
-0000dec0: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-0000ded0: 6c74 0a20 2066 6f72 206b 2069 6e20 7261  lt.  for k in ra
-0000dee0: 6e67 6528 3829 3a0a 2020 2020 5320 3d20  nge(8):.    S = 
-0000def0: 2774 6573 7420 272a 3130 2a2a 6b0a 2020  'test '*10**k.  
-0000df00: 2020 7332 203d 2027 7465 7374 270a 2020    s2 = 'test'.  
-0000df10: 2020 2574 696d 6520 5b6d 2e73 7461 7274    %time [m.start
-0000df20: 2829 2066 6f72 206d 2069 6e20 7265 2e66  () for m in re.f
-0000df30: 696e 6469 7465 7228 5332 2c20 5329 5d0a  inditer(S2, S)].
-0000df40: 0a20 2023 2074 6865 6e20 636f 7079 2069  .  # then copy i
-0000df50: 7420 696e 746f 2061 2073 7472 696e 6720  t into a string 
-0000df60: 6c69 6b65 2062 656c 6f77 0a0a 2020 7478  like below..  tx
-0000df70: 7420 3d20 2727 270a 2020 4350 5520 7469  t = '''.  CPU ti
-0000df80: 6d65 733a 2075 7365 7220 3020 6e73 2c20  mes: user 0 ns, 
-0000df90: 7379 733a 2039 2e30 3520 6d73 2c20 746f  sys: 9.05 ms, to
-0000dfa0: 7461 6c3a 2039 2e30 3520 6d73 0a20 2057  tal: 9.05 ms.  W
-0000dfb0: 616c 6c20 7469 6d65 3a20 392e 3031 206d  all time: 9.01 m
-0000dfc0: 730a 2020 4350 5520 7469 6d65 733a 2075  s.  CPU times: u
-0000dfd0: 7365 7220 3132 20c2 b573 2c20 7379 733a  ser 12 ..s, sys:
-0000dfe0: 2031 20c2 b573 2c20 746f 7461 6c3a 2031   1 ..s, total: 1
-0000dff0: 3320 c2b5 730a 2020 5761 6c6c 2074 696d  3 ..s.  Wall tim
-0000e000: 653a 2031 352e 3720 c2b5 730a 2020 4350  e: 15.7 ..s.  CP
-0000e010: 5520 7469 6d65 733a 2075 7365 7220 3438  U times: user 48
-0000e020: 20c2 b573 2c20 7379 733a 2033 20c2 b573   ..s, sys: 3 ..s
-0000e030: 2c20 746f 7461 6c3a 2035 3120 c2b5 730a  , total: 51 ..s.
-0000e040: 2020 5761 6c6c 2074 696d 653a 2035 362e    Wall time: 56.
-0000e050: 3320 c2b5 730a 2020 4350 5520 7469 6d65  3 ..s.  CPU time
-0000e060: 733a 2075 7365 7220 3238 3120 c2b5 732c  s: user 281 ..s,
-0000e070: 2073 7973 3a20 3020 6e73 2c20 746f 7461   sys: 0 ns, tota
-0000e080: 6c3a 2032 3831 20c2 b573 0a20 2057 616c  l: 281 ..s.  Wal
-0000e090: 6c20 7469 6d65 3a20 3238 3720 c2b5 730a  l time: 287 ..s.
-0000e0a0: 2020 4350 5520 7469 6d65 733a 2075 7365    CPU times: use
-0000e0b0: 7220 322e 3432 206d 732c 2073 7973 3a20  r 2.42 ms, sys: 
-0000e0c0: 3020 6e73 2c20 746f 7461 6c3a 2032 2e34  0 ns, total: 2.4
-0000e0d0: 3220 6d73 0a20 2057 616c 6c20 7469 6d65  2 ms.  Wall time
-0000e0e0: 3a20 322e 3433 206d 730a 2020 4350 5520  : 2.43 ms.  CPU 
-0000e0f0: 7469 6d65 733a 2075 7365 7220 3231 2e38  times: user 21.8
-0000e100: 206d 732c 2073 7973 3a20 3232 20c2 b573   ms, sys: 22 ..s
-0000e110: 2c20 746f 7461 6c3a 2032 312e 3820 6d73  , total: 21.8 ms
-0000e120: 0a20 2057 616c 6c20 7469 6d65 3a20 3231  .  Wall time: 21
-0000e130: 2e32 206d 730a 2020 4350 5520 7469 6d65  .2 ms.  CPU time
-0000e140: 733a 2075 7365 7220 3139 3820 6d73 2c20  s: user 198 ms, 
-0000e150: 7379 733a 2032 312e 3520 6d73 2c20 746f  sys: 21.5 ms, to
-0000e160: 7461 6c3a 2032 3139 206d 730a 2020 5761  tal: 219 ms.  Wa
-0000e170: 6c6c 2074 696d 653a 2032 3134 206d 730a  ll time: 214 ms.
-0000e180: 2020 4350 5520 7469 6d65 733a 2075 7365    CPU times: use
-0000e190: 7220 312e 3833 2073 2c20 7379 733a 2031  r 1.83 s, sys: 1
-0000e1a0: 3931 206d 732c 2074 6f74 616c 3a20 322e  91 ms, total: 2.
-0000e1b0: 3032 2073 0a20 2057 616c 6c20 7469 6d65  02 s.  Wall time
-0000e1c0: 3a20 322e 3032 2073 0a20 2027 2727 0a20  : 2.02 s.  '''. 
-0000e1d0: 2064 6174 6120 3d20 6765 745f 7469 6d65   data = get_time
-0000e1e0: 5f69 7428 7478 7429 0a20 2061 7820 3d20  _it(txt).  ax = 
-0000e1f0: 706c 742e 706c 6f74 2864 6174 615b 313a  plt.plot(data[1:
-0000e200: 5d29 0a20 2070 6c74 2e79 7363 616c 6528  ]).  plt.yscale(
-0000e210: 276c 6f67 2729 0a20 2063 0100 0000 0000  'log').  c......
-0000e220: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-0000e230: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-0000e240: 01a0 0064 00a1 0164 0119 0091 0271 0453  ...d...d.....q.S
-0000e250: 0029 0272 8b01 0000 7201 0000 0029 0172  .).r....r....).r
-0000e260: d700 0000 7231 0000 0072 1600 0000 7216  ....r1...r....r.
-0000e270: 0000 0072 1700 0000 7234 0000 00c5 0900  ...r....r4......
-0000e280: 0073 0400 0000 0600 0200 7a1f 6765 745f  .s........z.get_
-0000e290: 7469 6d65 5f69 742e 3c6c 6f63 616c 733e  time_it.<locals>
-0000e2a0: 2e3c 6c69 7374 636f 6d70 3e7a 0b57 616c  .<listcomp>z.Wal
-0000e2b0: 6c20 7469 6d65 3a20 722e 0000 004e da01  l time: r....N..
-0000e2c0: 7367 fca9 f1d2 4d62 503f da02 6d73 678d  sg....MbP?..msg.
-0000e2d0: edb5 a0f7 c6b0 3e75 0300 0000 c2b5 7372  ......>u......sr
-0000e2e0: 8701 0000 724a 0000 0072 0100 0000 2904  ....rJ...r....).
-0000e2f0: 72d7 0000 0072 6800 0000 7223 0000 0072  r....rh...r#...r
-0000e300: 8500 0000 2906 da03 7478 74da 0476 6172  ....)...txt..var
-0000e310: 7372 e100 0000 722a 0000 0072 3300 0000  sr....r*...r3...
-0000e320: da05 756e 6974 7372 1600 0000 7216 0000  ..unitsr....r...
-0000e330: 0072 1700 0000 da0b 6765 745f 7469 6d65  .r......get_time
-0000e340: 5f69 74a2 0900 0073 1400 0000 0023 1c01  _it....s.....#..
-0000e350: 0601 0801 0801 0801 0401 0801 0e01 2201  ..............".
-0000e360: 7237 0200 0063 0200 0000 0000 0000 0000  r7...c..........
-0000e370: 0000 0700 0000 0a00 0000 4300 0000 731a  ..........C...s.
-0000e380: 0100 0067 007d 0274 00a0 017c 0064 01a1  ...g.}.t...|.d..
-0000e390: 028f f87d 037c 03a0 02a1 0044 005d 247d  ...}.|.....D.]$}
-0000e3a0: 047c 03a0 037c 04a1 0172 347c 02a0 0464  .|...|...r4|...d
-0000e3b0: 02a1 0101 0071 1a7c 02a0 0464 03a1 0101  .....q.|...d....
-0000e3c0: 0071 1a74 057c 0283 0172 fc74 0664 0483  .q.t.|...r.t.d..
-0000e3d0: 0101 007c 0064 0517 007d 0574 00a0 017c  ...|.d...}.t...|
-0000e3e0: 0064 0517 0064 06a1 028f 627d 067c 03a0  .d...d....b}.|..
-0000e3f0: 02a1 0044 005d 427d 047c 03a0 037c 04a1  ...D.]B}.|...|..
-0000e400: 0172 a474 0664 077c 0417 0064 0817 0083  .r.t.d.|...d....
-0000e410: 0101 007c 066a 077c 047c 037c 0419 0064  ...|.j.|.|.|...d
-0000e420: 098d 0201 0071 7274 0664 0a7c 0417 0064  .....qrt.d.|...d
-0000e430: 0b17 0083 0101 0071 727c 06a0 08a1 0001  .......qr|......
-0000e440: 007c 03a0 08a1 0001 0057 0035 0051 0052  .|.......W.5.Q.R
-0000e450: 0058 007c 0172 fa74 0664 0c83 0101 0074  .X.|.r.t.d.....t
-0000e460: 09a0 0a7c 00a1 0101 0074 0664 0d83 0101  ...|.....t.d....
-0000e470: 0074 09a0 0b7c 057c 00a1 0201 006e 0874  .t...|.|.....n.t
-0000e480: 0664 0e83 0101 0057 0035 0051 0052 0058  .d.....W.5.Q.R.X
-0000e490: 0074 0664 0f83 0101 0064 0053 0029 104e  .t.d.....d.S.).N
-0000e4a0: 72e1 0000 0072 0100 0000 722e 0000 007a  r....r....r....z
-0000e4b0: 2543 6f72 7275 7074 2066 696c 6520 666f  %Corrupt file fo
-0000e4c0: 756e 642c 2063 7265 6174 696e 6720 6e65  und, creating ne
-0000e4d0: 7720 6669 6c65 da03 544d 5072 9900 0000  w file..TMPr....
-0000e4e0: 7a0b 4164 6469 6e67 206b 6579 207a 1720  z.Adding key z. 
-0000e4f0: 746f 206e 6577 2074 656d 7020 4835 2066  to new temp H5 f
-0000e500: 696c 652e 2e2e 72fd 0000 007a 072a 2a2a  ile...r....z.***
-0000e510: 4b65 7920 7a22 2077 6173 2063 6f72 7275  Key z" was corru
-0000e520: 7074 2c20 736b 6970 7069 6e67 2074 6869  pt, skipping thi
-0000e530: 7320 6b65 792e 2e2e 7a18 4465 6c65 7469  s key...z.Deleti
-0000e540: 6e67 2063 6f72 7275 7074 2048 3520 6669  ng corrupt H5 fi
-0000e550: 6c65 7a15 7265 6e61 6d69 6e67 206e 6577  lez.renaming new
-0000e560: 2068 3520 6669 6c65 207a 1446 696c 6520   h5 file z.File 
-0000e570: 6973 204e 4f54 2063 6f72 7275 7074 215a  is NOT corrupt!Z
-0000e580: 0846 494e 4953 4845 4429 0c72 aa00 0000  .FINISHED).r....
-0000e590: 72ab 0000 0072 9500 0000 72c5 0000 0072  r....r....r....r
-0000e5a0: 2300 0000 7287 0000 0072 4b00 0000 72ab  #...r....rK...r.
-0000e5b0: 0100 00da 0563 6c6f 7365 725f 0000 0072  .....closer_...r
-0000e5c0: 7900 0000 da06 7265 6e61 6d65 2907 5a07  y.....rename).Z.
-0000e5d0: 4835 5f66 696c 655a 1164 6f5f 6465 6c5f  H5_fileZ.do_del_
-0000e5e0: 616e 645f 7265 6e61 6d65 5a07 7473 745f  and_renameZ.tst_
-0000e5f0: 636f 7272 d901 0000 7233 0000 005a 0a48  corr....r3...Z.H
-0000e600: 355f 6669 6c65 544d 505a 0368 6632 7216  5_fileTMPZ.hf2r.
-0000e610: 0000 0072 1600 0000 7217 0000 00da 2173  ...r....r.....!s
-0000e620: 6176 655f 7768 6174 5f69 735f 6c65 6674  ave_what_is_left
-0000e630: 5f6f 665f 796f 7572 5f68 355f 6669 6c65  _of_your_h5_file
-0000e640: d109 0000 7330 0000 0000 0104 010e 010c  ....s0..........
-0000e650: 010a 010c 020c 0108 0108 0108 0112 010c  ................
-0000e660: 010a 0110 0114 0212 0108 0112 0104 0108  ................
-0000e670: 010a 0108 010e 0212 0172 3b02 0000 6304  .........r;...c.
-0000e680: 0000 0000 0000 0000 0000 000c 0000 0009  ................
-0000e690: 0000 0043 0000 0073 e200 0000 7400 6a01  ...C...s....t.j.
-0000e6a0: 7c01 6401 6402 8d02 7d04 7402 a003 7c00  |.d.d...}.t...|.
-0000e6b0: 6403 a102 8fa2 7d05 7c05 6404 1900 6405  d.....}.|.d...d.
-0000e6c0: 6405 8502 1900 7d06 7404 7405 7406 7c06  d.....}.t.t.t.|.
-0000e6d0: 8301 7407 7c06 8301 6406 8d02 8301 4400  ..t.|...d.....D.
-0000e6e0: 5d72 5c02 7d07 5c02 7d08 7d09 7c05 6407  ]r\.}.\.}.}.|.d.
-0000e6f0: 1900 7c08 7c09 8502 1900 7d0a 7407 7c0a  ..|.|.....}.t.|.
-0000e700: 6a08 8301 6408 6b02 728a 7c0a 6405 6405  j...d.k.r.|.d.d.
-0000e710: 8502 6405 6405 8502 6405 6405 8502 6409  ..d.d...d.d...d.
-0000e720: 6604 1900 7d0a 7400 6a09 7c0a 640a 6409  f...}.t.j.|.d.d.
-0000e730: 640b 8d03 7d0b 7c04 a00a 7c0b 740b a00c  d...}.|...|.t...
-0000e740: 7c0b 6a08 6409 1900 a101 640c 1400 a102  |.j.d.....d.....
-0000e750: 0100 7144 5700 3500 5100 5200 5800 740d  ..qDW.5.Q.R.X.t.
-0000e760: 7c00 7c01 640d 640d 8304 0100 740d 7c00  |.|.d.d.....t.|.
-0000e770: 7c01 6404 6404 8304 0100 6405 5300 290e  |.d.d.....d.S.).
-0000e780: 7ae1 0a0a 2020 2020 5061 7261 6d65 7465  z...    Paramete
-0000e790: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000e7a0: 2d0a 2020 2020 6620 3a20 6835 2066 696c  -.    f : h5 fil
-0000e7b0: 6520 7769 7468 2053 494e 474c 4520 4652  e with SINGLE FR
-0000e7c0: 414d 4553 2074 6869 7320 6973 206d 6561  AMES this is mea
-0000e7d0: 6e74 2074 6f20 6265 2061 2074 6573 7420  nt to be a test 
-0000e7e0: 7072 6f67 7261 6d2e 2069 6620 7573 6564  program. if used
-0000e7f0: 206c 6f6e 6720 7465 726d 2049 2077 696c   long term I wil
-0000e800: 6c20 6368 616e 6765 2074 6869 7320 7061  l change this pa
-0000e810: 7274 0a20 2020 2066 3220 3a0a 2020 2020  rt.    f2 :.    
-0000e820: 6275 6666 6572 203a 0a20 2020 2073 6869  buffer :.    shi
-0000e830: 6674 5f74 6f5f 7468 655f 7269 6768 745f  ft_to_the_right_
-0000e840: 6279 203a 0a0a 2020 2020 5265 7475 726e  by :..    Return
-0000e850: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20  s.    -------.. 
-0000e860: 2020 2054 a901 7236 0100 0072 6d00 0000     T..r6...rm...
-0000e870: 7241 0000 004e 7242 0100 0072 9600 0000  rA...NrB...r....
-0000e880: 72d5 0000 0072 0100 0000 7247 0000 00a9  r....r....rG....
-0000e890: 02da 0662 7566 6665 72da 1573 6869 6674  ...buffer..shift
-0000e8a0: 5f74 6f5f 7468 655f 7269 6768 745f 6279  _to_the_right_by
-0000e8b0: 724a 0000 0072 5200 0000 290e 7208 0000  rJ...rR...).r...
-0000e8c0: 0072 4401 0000 72aa 0000 0072 ab00 0000  .rD...r....r....
-0000e8d0: 7224 0000 0072 0b00 0000 7237 0000 0072  r$...r....r7...r
-0000e8e0: 3000 0000 7221 0000 005a 0e73 7461 636b  0...r!...Z.stack
-0000e8f0: 5f69 6d67 735f 6c61 6772 4a01 0000 721d  _imgs_lagrJ...r.
-0000e900: 0000 0072 3600 0000 72cc 0100 0029 0c72  ...r6...r....).r
-0000e910: a101 0000 da02 6632 723e 0200 0072 3f02  ......f2r>...r?.
-0000e920: 0000 72ad 0100 0072 bc00 0000 7253 0000  ..r....r....rS..
-0000e930: 0072 3e00 0000 72b9 0000 0072 ba00 0000  .r>...r....r....
-0000e940: da02 7832 7230 0200 0072 1600 0000 7216  ..x2r0...r....r.
-0000e950: 0000 0072 1700 0000 da12 7374 6163 6b5f  ...r......stack_
-0000e960: 6c61 675f 6835 5f6d 616b 6572 ef09 0000  lag_h5_maker....
-0000e970: 7316 0000 0000 0e0e 010e 0110 0124 0110  s............$..
-0000e980: 010e 011c 0110 0128 030e 0172 4202 0000  .......(...rB...
-0000e990: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
-0000e9a0: 0009 0000 0043 0000 0073 be00 0000 7400  .....C...s....t.
-0000e9b0: a001 7c00 6401 a102 8fa8 7d01 7402 7403  ..|.d.....}.t.t.
-0000e9c0: 7c01 6402 1900 6a04 6403 1900 8301 8301  |.d...j.d.......
-0000e9d0: 4400 5d8a 7d02 7405 a006 7c01 6402 1900  D.].}.t...|.d...
-0000e9e0: 7c02 1900 a101 7d03 7403 6404 8301 4400  |.....}.t.d...D.
-0000e9f0: 5d6a 7d04 7c03 a007 7408 a101 7d03 7c03  ]j}.|...t...}.|.
-0000ea00: 6405 6405 8502 6405 6405 8502 7c04 6603  d.d...d.d...|.f.
-0000ea10: 1900 7c03 6405 6405 8502 6405 6405 8502  ..|.d.d...d.d...
-0000ea20: 6406 6603 1900 1800 7d05 7c05 6407 1700  d.f.....}.|.d...
-0000ea30: 6404 1b00 a007 7409 6a0a a101 7d05 7c05  d.....t.j...}.|.
-0000ea40: 7c01 6402 1900 7c02 6405 6405 8502 6405  |.d...|.d.d...d.
-0000ea50: 6405 8502 7c04 6604 3c00 7142 7124 5700  d...|.f.<.qBq$W.
-0000ea60: 3500 5100 5200 5800 6405 5300 2908 6167  5.Q.R.X.d.S.).ag
-0000ea70: 0100 000a 2020 2020 6e65 6564 2074 6f20  ....    need to 
-0000ea80: 7573 6520 7468 6520 7374 6163 6b5f 6c61  use the stack_la
-0000ea90: 675f 6835 5f6d 616b 6572 2066 6972 7374  g_h5_maker first
-0000eaa0: 2061 6e64 2074 6865 6e20 7365 6e64 2061   and then send a
-0000eab0: 2063 6f70 7920 6f66 2074 6861 7420 696e   copy of that in
-0000eac0: 746f 2074 6869 7320 6f6e 6520 6167 6169  to this one agai
-0000ead0: 6e20 7468 6573 6520 7072 6f67 7261 6d20  n these program 
-0000eae0: 6172 6520 6f6e 6c79 2061 2074 656d 700a  are only a temp.
-0000eaf0: 2020 2020 736f 6c75 7469 6f6e 2c20 6966      solution, if
-0000eb00: 2077 6520 7573 6520 7468 6573 6520 6d65   we use these me
-0000eb10: 7468 6f64 7320 666f 7220 7468 6520 6d61  thods for the ma
-0000eb20: 696e 206d 6f64 656c 2074 6865 6e20 4920  in model then I 
-0000eb30: 7769 6c6c 206d 616b 6520 7573 696e 6720  will make using 
-0000eb40: 7468 656d 206d 6f72 6520 666c 7569 6420  them more fluid 
-0000eb50: 616e 6420 6e6f 7420 6465 7065 6e64 206f  and not depend o
-0000eb60: 6e20 6f6e 6520 616e 6f74 6865 720a 2020  n one another.  
-0000eb70: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000eb80: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000eb90: 6633 203a 2074 6865 2066 696c 6520 6672  f3 : the file fr
-0000eba0: 6f6d 2073 7461 636b 5f6c 6167 5f68 355f  om stack_lag_h5_
-0000ebb0: 6d61 6b65 7220 6f75 7470 7574 0a0a 2020  maker output..  
-0000ebc0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0000ebd0: 2d2d 2d2d 2d0a 2020 2020 72a2 0000 0072  -----.    r....r
-0000ebe0: 9600 0000 7201 0000 0072 4700 0000 4e72  ....r....rG...Nr
-0000ebf0: 4a00 0000 e9ff 0000 0029 0b72 aa00 0000  J........).r....
-0000ec00: 72ab 0000 0072 0b00 0000 723a 0000 0072  r....r....r:...r
-0000ec10: 2100 0000 721b 0000 0072 1c00 0000 7281  !...r....r....r.
-0000ec20: 0000 0072 8500 0000 721d 0000 0072 2a01  ...r....r....r*.
-0000ec30: 0000 2906 da02 6633 72bc 0000 0072 2c00  ..)...f3r....r,.
-0000ec40: 0000 7233 0000 005a 0569 6d67 5f69 72e1  ..r3...Z.img_ir.
-0000ec50: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-0000ec60: 0000 da11 6469 6666 5f6c 6167 5f68 355f  ....diff_lag_h5_
-0000ec70: 6d61 6b65 720c 0a00 0073 1000 0000 000c  maker....s......
-0000ec80: 0e01 1a01 1201 0c01 0a01 2c01 1401 7245  ..........,...rE
-0000ec90: 0200 0063 0200 0000 0000 0000 0000 0000  ...c............
-0000eca0: 0900 0000 0900 0000 4300 0000 73ba 0000  ........C...s...
-0000ecb0: 0074 006a 017c 0164 0164 028d 027d 0274  .t.j.|.d.d...}.t
-0000ecc0: 02a0 037c 0064 03a1 028f 8c7d 037c 0364  ...|.d.....}.|.d
-0000ecd0: 0419 0064 0064 0085 0219 007d 0474 0474  ...d.d.....}.t.t
-0000ece0: 0574 067c 0483 0174 077c 0483 0164 058d  .t.|...t.|...d..
-0000ecf0: 0283 0144 005d 5c5c 027d 055c 027d 067d  ...D.]\\.}.\.}.}
-0000ed00: 077c 0364 0619 007c 067c 0785 0219 007d  .|.d...|.|.....}
-0000ed10: 0874 08a0 097c 0864 0064 0085 0264 0064  .t...|.d.d...d.d
-0000ed20: 0085 0264 0064 0085 0264 0066 0419 0064  ...d.d...d.f...d
-0000ed30: 07a1 027d 087c 02a0 0a7c 0874 08a0 0b7c  ...}.|...|.t...|
-0000ed40: 086a 0c64 0819 00a1 0164 0914 00a1 0201  .j.d.....d......
-0000ed50: 0071 4457 0035 0051 0052 0058 0074 0d7c  .qDW.5.Q.R.X.t.|
-0000ed60: 007c 0183 0201 0064 0053 0029 0a4e 5472  .|.....d.S.).NTr
-0000ed70: 3c02 0000 726d 0000 0072 4100 0000 7242  <...rm...rA...rB
-0000ed80: 0100 0072 9600 0000 7246 0000 0072 0100  ...r....rF...r..
-0000ed90: 0000 724a 0000 0029 0e72 0800 0000 7244  ..rJ...).r....rD
-0000eda0: 0100 0072 aa00 0000 72ab 0000 0072 2400  ...r....r....r$.
-0000edb0: 0000 720b 0000 0072 3700 0000 7230 0000  ..r....r7...r0..
-0000edc0: 0072 1d00 0000 da04 7469 6c65 724a 0100  .r......tilerJ..
-0000edd0: 0072 3600 0000 7221 0000 0072 9801 0000  .r6...r!...r....
-0000ede0: a909 72a1 0100 0072 4002 0000 72ad 0100  ..r....r@...r...
-0000edf0: 0072 bc00 0000 7253 0000 0072 3e00 0000  .r....rS...r>...
-0000ee00: 72b9 0000 0072 ba00 0000 7230 0200 0072  r....r....r0...r
-0000ee10: 1600 0000 7216 0000 0072 1700 0000 da21  ....r....r.....!
-0000ee20: 6578 7061 6e64 5f73 696e 676c 655f 6672  expand_single_fr
-0000ee30: 616d 655f 746f 5f33 5f63 6f6c 6f72 5f68  ame_to_3_color_h
-0000ee40: 3522 0a00 0073 1000 0000 0001 0e01 0e01  5"...s..........
-0000ee50: 1001 2401 1001 2401 2803 7248 0200 0063  ..$...$.(.rH...c
-0000ee60: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-0000ee70: 0a00 0000 4300 0000 733c 0100 0074 007c  ....C...s<...t.|
-0000ee80: 0064 0164 0264 038d 037d 0274 017c 0264  .d.d.d...}.t.|.d
-0000ee90: 0464 058d 027d 0274 017c 0264 0664 058d  .d...}.t.|.d.d..
-0000eea0: 027d 0274 02a0 037c 0064 07a1 028f 647d  .}.t...|.d....d}
-0000eeb0: 0374 02a0 037c 0164 08a1 028f 4c7d 047c  .t...|.d....L}.|
-0000eec0: 0244 005d 407d 057a 167c 046a 047c 057c  .D.]@}.z.|.j.|.|
-0000eed0: 037c 0519 0064 098d 0201 0057 0071 4601  .|...d.....W.qF.
-0000eee0: 0001 0001 007c 047c 053d 007c 046a 047c  .....|.|.=.|.j.|
-0000eef0: 057c 037c 0519 0064 098d 0201 0059 0071  .|.|...d.....Y.q
-0000ef00: 4658 0071 4657 0035 0051 0052 0058 0057  FX.qFW.5.Q.R.X.W
-0000ef10: 0035 0051 0052 0058 0064 0a7c 026b 0790  .5.Q.R.X.d.|.k..
-0000ef20: 0172 3864 0b7c 026b 0690 0172 3874 05a0  .r8d.|.k...r8t..
-0000ef30: 067c 0067 0164 0ba1 027d 0674 02a0 037c  .|.g.d...}.t...|
-0000ef40: 0164 08a1 028f 687d 037a 247c 036a 0464  .d....h}.z$|.j.d
-0000ef50: 0a7c 0664 0c64 0d64 0d85 0266 0219 00a0  .|.d.d.d...f....
-0000ef60: 0774 08a1 0164 098d 0201 0057 006e 3c01  .t...d.....W.n<.
-0000ef70: 0001 0001 007c 0364 0a3d 0074 09a0 0a64  .....|.d.=.t...d
-0000ef80: 0ea1 0101 007c 036a 0464 0a7c 0664 0c64  .....|.j.d.|.d.d
-0000ef90: 0d64 0d85 0266 0219 00a0 0774 08a1 0164  .d...f.....t...d
-0000efa0: 098d 0201 0059 006e 0258 0057 0035 0051  .....Y.n.X.W.5.Q
-0000efb0: 0052 0058 0064 0d53 0029 0f7a 620a 0a20  .R.X.d.S.).zb.. 
-0000efc0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000efd0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000efe0: 2066 203a 2073 6f75 7263 650a 2020 2020   f : source.    
-0000eff0: 6632 203a 2064 6573 7469 6e61 7469 6f6e  f2 : destination
-0000f000: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0000f010: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2054    -------..    T
-0000f020: 46a9 0272 c801 0000 72c9 0100 005a 064d  F..r....r....Z.M
-0000f030: 4f44 454c 5f29 0172 d501 0000 7296 0000  ODEL_).r....r...
-0000f040: 0072 6d00 0000 72a2 0000 0072 fd00 0000  .rm...r....r....
-0000f050: 7241 0000 0072 a901 0000 722e 0000 004e  rA...r....r....N
-0000f060: 7247 0000 0029 0b72 a700 0000 72d6 0100  rG...).r....r...
-0000f070: 0072 aa00 0000 72ab 0000 0072 ab01 0000  .r....r....r....
-0000f080: 7208 0000 0072 2801 0000 7281 0000 0072  r....r(...r....r
-0000f090: 8400 0000 7296 0100 0072 ae01 0000 2907  ....r....r....).
-0000f0a0: 72a1 0100 0072 4002 0000 5a07 6b5f 6e61  r....r@...Z.k_na
-0000f0b0: 6d65 7372 bc00 0000 72cb 0100 00da 026b  mesr....r......k
-0000f0c0: 6e5a 0474 6e66 6e72 1600 0000 7216 0000  nZ.tnfnr....r...
-0000f0d0: 0072 1700 0000 7298 0100 0031 0a00 0073  .r....r....1...s
-0000f0e0: 2800 0000 000c 0e01 0c01 0c01 0e01 0e01  (...............
-0000f0f0: 0801 0201 1601 0601 0601 2e07 1401 0e01  ................
-0000f100: 0e01 0201 2401 0601 0601 0a01 7298 0100  ....$.......r...
-0000f110: 0063 0300 0000 0000 0000 0000 0000 0400  .c..............
-0000f120: 0000 0900 0000 4300 0000 7350 0000 0074  ......C...sP...t
-0000f130: 00a0 017c 0064 01a1 028f 3a7d 037a 127c  ...|.d....:}.z.|
-0000f140: 036a 027c 027c 0164 028d 0201 0057 006e  .j.|.|.d.....W.n
-0000f150: 2001 0001 0001 007c 037c 023d 007c 036a   ......|.|.=.|.j
-0000f160: 027c 027c 0164 028d 0201 0059 006e 0258  .|.|.d.....Y.n.X
-0000f170: 0057 0035 0051 0052 0058 0064 0053 0029  .W.5.Q.R.X.d.S.)
-0000f180: 034e 72a2 0000 0072 fd00 0000 2903 72aa  .Nr....r....).r.
-0000f190: 0000 0072 ab00 0000 72ab 0100 0029 0472  ...r....r....).r
-0000f1a0: d801 0000 722a 0000 005a 0964 6174 615f  ....r*...Z.data_
-0000f1b0: 6e61 6d65 72bc 0000 0072 1600 0000 7216  namer....r....r.
-0000f1c0: 0000 0072 1700 0000 da11 666f 7263 655f  ...r......force_
-0000f1d0: 7772 6974 655f 746f 5f68 3559 0a00 0073  write_to_h5Y...s
-0000f1e0: 0c00 0000 0001 0e01 0201 1201 0601 0601  ................
-0000f1f0: 724b 0200 0063 0200 0000 0000 0000 0000  rK...c..........
-0000f200: 0000 0900 0000 0900 0000 4300 0000 73c2  ..........C...s.
-0000f210: 0000 0074 006a 017c 0164 0164 0264 038d  ...t.j.|.d.d.d..
-0000f220: 037d 0274 02a0 037c 0064 04a1 028f 927d  .}.t...|.d.....}
-0000f230: 037a 187c 0364 0519 0064 0664 0064 0085  .z.|.d...d.d.d..
-0000f240: 0266 0219 007d 0457 006e 1c01 0001 0001  .f...}.W.n......
-0000f250: 007c 0364 0719 0064 0064 0085 0219 007d  .|.d...d.d.....}
-0000f260: 0459 006e 0258 0074 0474 0574 067c 0483  .Y.n.X.t.t.t.|..
-0000f270: 0174 077c 0483 0164 088d 0283 0144 005d  .t.|...d.....D.]
-0000f280: 3c5c 027d 055c 027d 067d 077c 0364 0919  <\.}.\.}.}.|.d..
-0000f290: 007c 067c 0785 0219 0064 0a19 007d 087c  .|.|.....d...}.|
-0000f2a0: 02a0 087c 0874 09a0 0a7c 086a 0b64 0b19  ...|.t...|.j.d..
-0000f2b0: 00a1 0164 0c14 00a1 0201 0071 6c57 0035  ...d.......qlW.5
-0000f2c0: 0051 0052 0058 0074 0c7c 007c 0183 0201  .Q.R.X.t.|.|....
-0000f2d0: 0064 0053 0029 0d4e 5446 2902 7236 0100  .d.S.).NTF).r6..
-0000f2e0: 0072 3a01 0000 726d 0000 0072 a901 0000  .r:...rm...r....
-0000f2f0: 722e 0000 0072 4100 0000 7242 0100 0072  r....rA...rB...r
-0000f300: 9600 0000 2902 2e72 4a00 0000 7201 0000  ....)..rJ...r...
-0000f310: 0072 4a00 0000 290d 7208 0000 0072 4401  .rJ...).r....rD.
-0000f320: 0000 72aa 0000 0072 ab00 0000 7224 0000  ..r....r....r$..
-0000f330: 0072 0b00 0000 7237 0000 0072 3000 0000  .r....r7...r0...
-0000f340: 724a 0100 0072 1d00 0000 7236 0000 0072  rJ...r....r6...r
-0000f350: 2100 0000 7298 0100 0072 4702 0000 7216  !...r....rG...r.
-0000f360: 0000 0072 1600 0000 7217 0000 00da 2172  ...r....r.....!r
-0000f370: 6564 7563 655f 746f 5f73 696e 676c 655f  educe_to_single_
-0000f380: 6672 616d 655f 6672 6f6d 5f63 6f6c 6f72  frame_from_color
-0000f390: 620a 0000 7314 0000 0000 0110 010e 0102  b...s...........
-0000f3a0: 0118 0106 0116 0124 0114 0228 0372 4c02  .......$...(.rL.
-0000f3b0: 0000 6301 0000 0000 0000 0000 0000 0008  ..c.............
-0000f3c0: 0000 0007 0000 0043 0000 0073 1e01 0000  .......C...s....
-0000f3d0: 6401 6402 8400 7d01 7400 7c00 8301 4400  d.d...}.t.|...D.
-0000f3e0: 9001 5d06 7d02 7c01 7c02 8301 7d03 7401  ..].}.|.|...}.t.
-0000f3f0: 6a02 a003 7c02 a101 6400 6403 8502 1900  j...|...d.d.....
-0000f400: 6404 1700 7d04 7c03 6405 1700 7401 6a04  d...}.|.d...t.j.
-0000f410: 1700 7d05 7401 6a02 a005 7c05 a101 735a  ..}.t.j...|...sZ
-0000f420: 7401 a006 7c05 a101 0100 7c05 7c04 1700  t...|.....|.|...
-0000f430: 7d06 7407 7c02 7c06 8302 0100 7401 6a02  }.t.|.|.....t.j.
-0000f440: a003 7c02 a101 6400 6403 8502 1900 6406  ..|...d.d.....d.
-0000f450: 1700 7d04 7c03 6407 1700 7401 6a04 1700  ..}.|.d...t.j...
-0000f460: 7d05 7401 6a02 a005 7c05 a101 73a8 7401  }.t.j...|...s.t.
-0000f470: a006 7c05 a101 0100 7c05 7c04 1700 7d06  ..|.....|.|...}.
-0000f480: 7408 7c02 7c06 6408 6409 640a 8d04 0100  t.|.|.d.d.d.....
-0000f490: 7401 6a02 a003 7c06 a101 6400 6403 8502  t.j...|...d.d...
-0000f4a0: 1900 640b 1700 7d04 7c03 640c 1700 7401  ..d...}.|.d...t.
-0000f4b0: 6a04 1700 7d05 7401 6a02 a005 7c05 a101  j...}.t.j...|...
-0000f4c0: 73fc 7401 a006 7c05 a101 0100 7c05 7c04  s.t...|.....|.|.
-0000f4d0: 1700 7d07 7409 a00a 7c06 7c07 a102 0100  ..}.t...|.|.....
-0000f4e0: 740b 7c07 8301 0100 7110 6400 5300 290d  t.|.....q.d.S.).
-0000f4f0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-0000f500: 0000 0300 0000 5300 0000 732a 0000 0074  ......S...s*...t
-0000f510: 0074 017c 0083 016a 02a0 03a1 0083 017d  .t.|...j.......}
-0000f520: 0174 0074 017c 0183 016a 02a0 03a1 0083  .t.t.|...j......
-0000f530: 0174 046a 0517 0053 0072 0901 0000 2906  .t.j...S.r....).
-0000f540: 72a9 0000 0072 0e00 0000 7202 0200 00da  r....r....r.....
-0000f550: 0861 6273 6f6c 7574 6572 5f00 0000 7260  .absoluter_...r`
-0000f560: 0000 0029 0272 a101 0000 72f7 0000 0072  ...).r....r....r
-0000f570: 1600 0000 7216 0000 0072 1700 0000 da0b  ....r....r......
-0000f580: 6c61 7374 5f66 6f6c 6465 7275 0a00 0073  last_folderu...s
-0000f590: 0400 0000 0001 1201 7a26 6d61 6b65 5f61  ........z&make_a
-0000f5a0: 6c6c 5f48 355f 7479 7065 732e 3c6c 6f63  ll_H5_types.<loc
-0000f5b0: 616c 733e 2e6c 6173 745f 666f 6c64 6572  als>.last_folder
-0000f5c0: 7291 0000 007a 0b5f 7265 6775 6c61 722e  r....z._regular.
-0000f5d0: 6835 da07 7265 6775 6c61 7272 a100 0000  h5..regularr....
-0000f5e0: 5a04 336c 6167 7247 0000 0072 0100 0000  Z.3lagrG...r....
-0000f5f0: 723d 0200 007a 085f 6469 6666 2e68 355a  r=...z._diff.h5Z
-0000f600: 0933 6c61 675f 6469 6666 290c 7225 0100  .3lag_diff).r%..
-0000f610: 0072 5f00 0000 7261 0000 0072 a400 0000  .r_...ra...r....
-0000f620: 7260 0000 0072 6200 0000 725f 0100 0072  r`...rb...r_...r
-0000f630: 4802 0000 7242 0200 0072 7300 0000 721b  H...rB...rs...r.
-0000f640: 0000 0072 4502 0000 2908 da10 6261 7365  ...rE...)...base
-0000f650: 5f64 6972 5f61 6c6c 5f68 3573 724e 0200  _dir_all_h5srN..
-0000f660: 0072 a101 0000 5a06 6261 7365 5f66 72a4  .r....Z.base_fr.
-0000f670: 0000 00da 0762 6173 6564 6972 7240 0200  .....basedirr@..
-0000f680: 0072 4402 0000 7216 0000 0072 1600 0000  .rD...r....r....
-0000f690: 7217 0000 00da 116d 616b 655f 616c 6c5f  r......make_all_
-0000f6a0: 4835 5f74 7970 6573 740a 0000 732c 0000  H5_typest...s,..
-0000f6b0: 0000 0108 040e 0108 0118 010e 010c 010a  ................
-0000f6c0: 0108 010a 0218 010e 010c 010a 0108 0210  ................
-0000f6d0: 0218 010e 010c 010a 0108 010c 0172 5202  .............rR.
-0000f6e0: 0000 6301 0000 0000 0000 0000 0000 0010  ..c.............
-0000f6f0: 0000 0007 0000 0043 0000 0073 a401 0000  .......C...s....
-0000f700: 6700 7d01 7400 a001 7c00 a101 7d02 7c01  g.}.t...|...}.|.
-0000f710: a002 7c02 a101 0100 7403 7c02 8301 7d03  ..|.....t.|...}.
-0000f720: 7c01 a002 7c03 a101 0100 7400 a001 7c03  |...|.....t...|.
-0000f730: a101 7d04 6401 7c04 7c04 6402 6b03 3c00  ..}.d.|.|.d.k.<.
-0000f740: 6403 7c04 7c04 6402 6b02 3c00 7c01 a002  d.|.|.d.k.<.|...
-0000f750: 7c04 a101 0100 7400 a001 7c03 a101 7d05  |.....t...|...}.
-0000f760: 6401 7c05 7c05 6404 6b03 3c00 6403 7c05  d.|.|.d.k.<.d.|.
-0000f770: 7c05 6404 6b02 3c00 7c01 a002 7c05 a101  |.d.k.<.|...|...
-0000f780: 0100 7400 a001 7c03 a101 7d06 6401 7c06  ..t...|...}.d.|.
-0000f790: 7c06 6403 6b02 3c00 6403 7c06 7c06 6402  |.d.k.<.d.|.|.d.
-0000f7a0: 6b02 3c00 6402 7c06 7c06 6404 6b02 3c00  k.<.d.|.|.d.k.<.
-0000f7b0: 7c01 a002 7c06 a101 0100 7400 a001 7c03  |...|.....t...|.
-0000f7c0: a101 7d07 7c07 6400 6405 8502 1900 6402  ..}.|.d.d.....d.
-0000f7d0: 6b02 7d08 7404 a002 6406 7c08 a102 7d09  k.}.t...d.|...}.
-0000f7e0: 7c07 6400 6405 8502 1900 6404 6b02 7d0a  |.d.d.....d.k.}.
-0000f7f0: 7404 a002 6406 7c0a a102 7d0b 7c07 6404  t...d.|...}.|.d.
-0000f800: 6b02 7d0a 6404 7c07 7c09 3c00 6407 7c07  k.}.d.|.|.<.d.|.
-0000f810: 7c0a 3c00 6408 7c07 7c0b 3c00 7c01 a002  |.<.d.|.|.<.|...
-0000f820: 7c07 a101 0100 7400 a001 7c07 a101 7d0c  |.....t...|...}.
-0000f830: 6401 7c0c 7c0c 6402 6b02 3c00 6401 7c0c  d.|.|.d.k.<.d.|.
-0000f840: 7c0c 6408 6b02 3c00 6402 7c0c 7c0c 6404  |.d.k.<.d.|.|.d.
-0000f850: 6b02 3c00 6404 7c0c 7c0c 6407 6b02 3c00  k.<.d.|.|.d.k.<.
-0000f860: 7c01 a002 7c0c a101 0100 6408 6403 6407  |...|.....d.d.d.
-0000f870: 6401 6404 6402 6409 6707 7d0d 6700 7d0e  d.d.d.d.g.}.g.}.
-0000f880: 7c0d 4400 5d14 7d0f 7c0e a002 7c01 7c0f  |.D.].}.|...|.|.
-0000f890: 1900 a101 0100 9001 7184 7404 a005 7c0e  ........q.t...|.
-0000f8a0: a101 5300 290a 4e72 0100 0000 7247 0000  ..S.).Nr....rG..
-0000f8b0: 0072 2e00 0000 7246 0000 0072 4a00 0000  .r....rF...rJ...
-0000f8c0: 4672 d500 0000 7297 0000 00e9 0600 0000  Fr....r.........
-0000f8d0: 2906 721b 0000 0072 1c00 0000 7223 0000  ).r....r....r#..
-0000f8e0: 0072 c601 0000 721d 0000 0072 3800 0000  .r....r....r8...
-0000f8f0: 2910 722a 0200 00da 0a61 6c6c 5f6c 6162  ).r*.....all_lab
-0000f900: 656c 73da 0278 3172 4102 0000 da02 7833  els..x1rA.....x3
-0000f910: da02 7834 da02 7835 da02 7836 da0a 6f6e  ..x4..x5..x6..on
-0000f920: 7365 745f 696e 6473 da19 626f 6f6c 5f69  set_inds..bool_i
-0000f930: 6e64 735f 6f6e 655f 6166 7465 725f 6f6e  nds_one_after_on
-0000f940: 7365 74da 0b6f 6666 7365 745f 696e 6473  set..offset_inds
-0000f950: da1a 626f 6f6c 5f69 6e64 735f 6f6e 655f  ..bool_inds_one_
-0000f960: 6166 7465 725f 6f66 6673 6574 da02 7837  after_offset..x7
-0000f970: 5a06 7265 736f 7274 5a07 615f 6669 6e61  Z.resortZ.a_fina
-0000f980: 6c72 2c00 0000 7216 0000 0072 1600 0000  lr,...r....r....
-0000f990: 7217 0000 00da 1e67 6574 5f61 6c6c 5f6c  r......get_all_l
-0000f9a0: 6162 656c 5f74 7970 6573 5f66 726f 6d5f  abel_types_from_
-0000f9b0: 6172 7261 7993 0a00 0073 4e00 0000 0001  array....sN.....
-0000f9c0: 0401 0a01 0a02 0801 0a02 0a01 0c01 0c01  ................
-0000f9d0: 0a02 0a01 0c01 0c01 0a02 0a01 0c01 0c01  ................
-0000f9e0: 0c01 0a02 0a01 1001 0c01 1001 0c01 0801  ................
-0000f9f0: 0801 0801 0801 0a02 0a01 0c01 0c01 0c01  ................
-0000fa00: 0c01 0a02 1202 0401 0801 1202 725f 0200  ............r_..
-0000fa10: 0063 0100 0000 0000 0000 0000 0000 1100  .c..............
-0000fa20: 0000 0a00 0000 4300 0000 736e 0200 0074  ......C...sn...t
-0000fa30: 007c 0083 0144 0090 025d 5e7d 0164 01a0  .|...D...]^}.d..
-0000fa40: 0174 026a 03a0 047c 01a1 01a0 0564 02a1  .t.j...|.....d..
-0000fa50: 01a1 017d 0274 026a 06a0 017c 01a0 0574  ...}.t.j...|...t
-0000fa60: 026a 06a1 0164 0064 0385 0219 00a1 0174  .j...d.d.......t
-0000fa70: 026a 0617 0064 0417 0074 026a 0617 007d  .j...d...t.j...}
-0000fa80: 0374 026a 03a0 077c 03a1 0173 6874 02a0  .t.j...|...sht..
-0000fa90: 087c 03a1 0101 007c 037c 0217 007d 0474  .|.....|.|...}.t
-0000faa0: 09a0 0a7c 0164 05a1 0290 018f 327d 0574  ...|.d......2}.t
-0000fab0: 0ba0 0c7c 0564 0619 0064 0064 0085 0219  ...|.d...d.d....
-0000fac0: 00a1 017d 0674 0d7c 0683 017d 0774 0ba0  ...}.t.|...}.t..
-0000fad0: 0c7c 07a1 017d 0864 077c 087c 0864 086b  .|...}.d.|.|.d.k
-0000fae0: 033c 0064 097c 087c 0864 086b 023c 0074  .<.d.|.|.d.k.<.t
-0000faf0: 0ba0 0c7c 07a1 017d 0964 077c 097c 0964  ...|...}.d.|.|.d
-0000fb00: 0a6b 033c 0064 097c 097c 0964 0a6b 023c  .k.<.d.|.|.d.k.<
-0000fb10: 0074 0ba0 0c7c 07a1 017d 0a64 077c 0a7c  .t...|...}.d.|.|
-0000fb20: 0a64 096b 023c 0064 097c 0a7c 0a64 086b  .d.k.<.d.|.|.d.k
-0000fb30: 023c 0064 087c 0a7c 0a64 0a6b 023c 0074  .<.d.|.|.d.k.<.t
-0000fb40: 0ba0 0c7c 07a1 017d 0b7c 0b64 0064 0b85  ...|...}.|.d.d..
-0000fb50: 0219 0064 086b 027d 0c74 0ea0 0f64 0c7c  ...d.k.}.t...d.|
-0000fb60: 0ca1 027d 0d7c 0b64 0064 0b85 0219 0064  ...}.|.d.d.....d
-0000fb70: 0a6b 027d 0e74 0ea0 0f64 0c7c 0ea1 027d  .k.}.t...d.|...}
-0000fb80: 0f7c 0b64 0a6b 027d 0e64 0a7c 0b7c 0d3c  .|.d.k.}.d.|.|.<
-0000fb90: 0064 0d7c 0b7c 0e3c 0064 0e7c 0b7c 0f3c  .d.|.|.<.d.|.|.<
-0000fba0: 0074 0ba0 0c7c 0ba1 017d 1064 077c 107c  .t...|...}.d.|.|
-0000fbb0: 1064 086b 023c 0064 077c 107c 1064 0e6b  .d.k.<.d.|.|.d.k
-0000fbc0: 023c 0064 087c 107c 1064 0a6b 023c 0064  .<.d.|.|.d.k.<.d
-0000fbd0: 0a7c 107c 1064 0d6b 023c 0057 0035 0051  .|.|.d.k.<.W.5.Q
-0000fbe0: 0052 0058 0074 09a0 0a7c 0464 0fa1 028f  .R.X.t...|.d....
-0000fbf0: a07d 057c 056a 1064 1074 0ea0 117c 06a1  .}.|.j.d.t...|..
-0000fc00: 017c 0664 118d 0301 007c 056a 1064 1274  .|.d.....|.j.d.t
-0000fc10: 0ea0 117c 07a1 017c 0764 118d 0301 007c  ...|...|.d.....|
-0000fc20: 056a 1064 1374 0ea0 117c 08a1 017c 0864  .j.d.t...|...|.d
-0000fc30: 118d 0301 007c 056a 1064 1474 0ea0 117c  .....|.j.d.t...|
-0000fc40: 09a1 017c 0964 118d 0301 007c 056a 1064  ...|.d.....|.j.d
-0000fc50: 1574 0ea0 117c 0aa1 017c 0a64 118d 0301  .t...|...|.d....
-0000fc60: 007c 056a 1064 1674 0ea0 117c 0ba1 017c  .|.j.d.t...|...|
-0000fc70: 0b64 118d 0301 007c 056a 1064 1774 0ea0  .d.....|.j.d.t..
-0000fc80: 117c 10a1 017c 1064 118d 0301 0057 0035  .|...|.d.....W.5
-0000fc90: 0051 0052 0058 0071 0864 0053 0029 184e  .Q.R.X.q.d.S.).N
-0000fca0: 7a0c 5f41 4c54 5f4c 4142 454c 532e 721d  z._ALT_LABELS.r.
-0000fcb0: 0100 0072 e501 0000 da0a 414c 545f 4c41  ...r......ALT_LA
-0000fcc0: 4245 4c53 726d 0000 0072 5200 0000 7201  BELSrm...rR...r.
-0000fcd0: 0000 0072 4700 0000 722e 0000 0072 4600  ...rG...r....rF.
-0000fce0: 0000 724a 0000 0046 72d5 0000 0072 9700  ..rJ...Fr....r..
-0000fcf0: 0000 7299 0000 007a 195b 302c 2031 5d2d  ..r....z.[0, 1]-
-0000fd00: 2028 6e6f 2074 6f75 6368 2c20 746f 7563   (no touch, touc
-0000fd10: 6829 72ca 0100 007a 2d5b 302c 2031 2c20  h)r....z-[0, 1, 
-0000fd20: 322c 2033 5d2d 2028 6e6f 2074 6f75 6368  2, 3]- (no touch
-0000fd30: 2c20 746f 7563 682c 206f 6e73 6574 2c20  , touch, onset, 
-0000fd40: 6f66 6673 6574 7a1a 5b30 2c20 315d 2d20  offsetz.[0, 1]- 
-0000fd50: 286e 6f74 206f 6e73 6574 2c20 6f6e 7365  (not onset, onse
-0000fd60: 7429 7a1c 5b30 2c20 315d 2d20 286e 6f74  t)z.[0, 1]- (not
-0000fd70: 206f 6666 7365 742c 206f 6666 7365 7429   offset, offset)
-0000fd80: 7a24 5b30 2c20 312c 2032 5d2d 2028 6e6f  z$[0, 1, 2]- (no
-0000fd90: 2065 7665 6e74 2c20 6f6e 7365 742c 206f   event, onset, o
-0000fda0: 6666 7365 7429 7a57 5b30 2c20 312c 2032  ffset)zW[0, 1, 2
-0000fdb0: 2c20 332c 2034 2c20 355d 2d20 286e 6f20  , 3, 4, 5]- (no 
-0000fdc0: 746f 7563 682c 2074 6f75 6368 2c20 6f6e  touch, touch, on
-0000fdd0: 7365 742c 206f 6e65 2061 6674 6572 206f  set, one after o
-0000fde0: 6e73 6574 2c20 6f66 6673 6574 2c20 6f6e  nset, offset, on
-0000fdf0: 6520 6166 7465 7220 6f66 6673 6574 297a  e after offset)z
-0000fe00: 385b 302c 2031 2c20 322c 2033 5d2d 2028  8[0, 1, 2, 3]- (
-0000fe10: 6e6f 2074 6f75 6368 2c20 746f 7563 682c  no touch, touch,
-0000fe20: 206f 6e65 2061 6674 6572 206f 6e73 6574   one after onset
-0000fe30: 2c20 6f66 6673 6574 2929 1272 2501 0000  , offset)).r%...
-0000fe40: 72d6 0000 0072 5f00 0000 7261 0000 0072  r....r_...ra...r
-0000fe50: a400 0000 72d7 0000 0072 6000 0000 7262  ....r....r`...rb
-0000fe60: 0000 0072 5f01 0000 72aa 0000 0072 ab00  ...r_...r....r..
-0000fe70: 0000 721b 0000 0072 1c00 0000 72c6 0100  ..r....r....r...
-0000fe80: 0072 1d00 0000 7223 0000 0072 ab01 0000  .r....r#...r....
-0000fe90: 7221 0000 0029 1172 5002 0000 72a1 0100  r!...).rP...r...
-0000fea0: 0072 a400 0000 7251 0200 0072 b700 0000  .r....rQ...r....
-0000feb0: 72bc 0000 0072 5502 0000 7241 0200 0072  r....rU...rA...r
-0000fec0: 5602 0000 7257 0200 0072 5802 0000 7259  V...rW...rX...rY
-0000fed0: 0200 0072 5a02 0000 725b 0200 0072 5c02  ...rZ...r[...r\.
-0000fee0: 0000 725d 0200 0072 5e02 0000 7216 0000  ..r]...r^...r...
-0000fef0: 0072 1600 0000 7217 0000 00da 136d 616b  .r....r......mak
-0000ff00: 655f 616c 745f 6c61 6265 6c73 5f68 3573  e_alt_labels_h5s
-0000ff10: c60a 0000 7358 0000 0000 010e 0118 012c  ....sX.........,
-0000ff20: 010c 010a 0108 0210 0216 0208 020a 010c  ................
-0000ff30: 010c 020a 010c 010c 020a 010c 010c 010c  ................
-0000ff40: 020a 0110 010c 0110 010c 0108 0108 0108  ................
-0000ff50: 0108 020a 010c 010c 010c 0116 020e 0116  ................
-0000ff60: 0116 0116 0116 0116 0106 0108 0002 ff06  ................
-0000ff70: 0272 6102 0000 6301 0000 0000 0000 0000  .ra...c.........
-0000ff80: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-0000ff90: 1600 0000 7400 7401 7c00 6401 1900 8301  ....t.t.|.d.....
-0000ffa0: 6a02 7c00 8e00 8301 5300 7219 0000 0029  j.|.....S.r....)
-0000ffb0: 0372 3900 0000 72d9 0000 00da 0c69 6e74  .r9...r......int
-0000ffc0: 6572 7365 6374 696f 6e72 6900 0000 7216  ersectionri...r.
-0000ffd0: 0000 0072 1600 0000 7217 0000 00da 0f69  ...r....r......i
-0000ffe0: 6e74 6572 7365 6374 5f6c 6973 7473 fc0a  ntersect_lists..
-0000fff0: 0000 7302 0000 0000 0172 6302 0000 e9c8  ..s......rc.....
-00010000: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00010010: 1000 0000 0a00 0000 4300 0000 73e0 0000  ........C...s...
-00010020: 0067 007d 057c 0044 005d ca7d 0674 00a0  .g.}.|.D.].}.t..
-00010030: 017c 0664 01a1 028f b47d 0774 02a0 037c  .|.d.....}.t...|
-00010040: 0764 0219 0064 0064 0085 0219 00a1 017d  .d...d.d.......}
-00010050: 087c 0764 0319 0064 0464 0064 0085 0266  .|.d...d.d.d...f
-00010060: 0219 007d 0974 0474 057c 0983 0183 0144  ...}.t.t.|.....D
-00010070: 005d 545c 027d 0a5c 027d 0b7d 0c7c 0764  .]T\.}.\.}.}.|.d
-00010080: 0519 0064 0064 0085 027c 0a66 0219 007c  ...d.d...|.f...|
-00010090: 0b17 007d 0d7c 0d64 0619 007c 0117 007d  ...}.|.d...|...}
-000100a0: 0e7c 0d64 0419 007c 0217 007d 0f74 067c  .|.d...|...}.t.|
-000100b0: 0f7c 0c67 0283 017d 0f64 047c 087c 0e7c  .|.g...}.d.|.|.|
-000100c0: 0f85 023c 0071 507c 0372 ba7c 087c 0764  ...<.qP|.r.|.|.d
-000100d0: 0219 0064 0064 0085 023c 007c 0472 c87c  ...d.d...<.|.r.|
-000100e0: 05a0 077c 08a1 0101 0057 0035 0051 0052  ...|.....W.5.Q.R
-000100f0: 0058 0071 087c 0472 dc7c 0553 0064 0053  .X.q.|.r.|.S.d.S
-00010100: 0029 074e 72a2 0000 0072 a701 0000 72a9  .).Nr....r....r.
-00010110: 0100 0072 2e00 0000 da0a 706f 6c65 5f74  ...r......pole_t
-00010120: 696d 6573 7201 0000 0029 0872 aa00 0000  imesr....).r....
-00010130: 72ab 0000 0072 1d00 0000 7280 0000 0072  r....r....r....r
-00010140: 2400 0000 7237 0000 00da 036d 696e 7223  $...r7.....minr#
-00010150: 0000 0029 105a 0748 355f 6c69 7374 5a0b  ...).Z.H5_listZ.
-00010160: 706f 6c65 5f75 705f 6164 645a 0d70 6f6c  pole_up_addZ.pol
-00010170: 655f 646f 776e 5f61 6464 726b 0100 00da  e_down_addrk....
-00010180: 0f72 6574 7572 6e5f 696e 5f72 616e 6765  .return_in_range
-00010190: 5a0c 616c 6c5f 696e 5f72 616e 6765 7233  Z.all_in_ranger3
-000101a0: 0000 0072 d901 0000 da0c 6e65 775f 696e  ...r......new_in
-000101b0: 5f72 616e 6765 724b 0100 0072 2c00 0000  _rangerK...r,...
-000101c0: 723f 0000 0072 4000 0000 7253 0000 0072  r?...r@...rS...r
-000101d0: 5502 0000 7241 0200 0072 1600 0000 7216  U...rA...r....r.
-000101e0: 0000 0072 1700 0000 da0c 6765 745f 696e  ...r......get_in
-000101f0: 5f72 616e 6765 000b 0000 7322 0000 0000  _range....s"....
-00010200: 0104 0108 010e 0116 0114 0118 0118 010c  ................
-00010210: 010c 010c 010e 0104 0110 0104 0116 0104  ................
-00010220: 0172 6902 0000 6301 0000 0000 0000 0000  .ri...c.........
-00010230: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
-00010240: 6800 0000 7400 a001 7c00 6401 a102 8f52  h...t...|.d....R
-00010250: 7d01 6402 7c01 a002 a100 6b06 722c 7c01  }.d.|.....k.r,|.
-00010260: 6402 1900 6400 6400 8502 1900 7d02 6e2e  d...d.d.....}.n.
-00010270: 6403 7c01 a002 a100 6b06 724e 7c01 6403  d.|.....k.rN|.d.
-00010280: 1900 6404 6400 6400 8502 6602 1900 7d02  ..d.d.d...f...}.
-00010290: 6e0c 6405 735a 7403 6406 8301 8201 5700  n.d.sZt.d.....W.
-000102a0: 3500 5100 5200 5800 7c02 5300 2907 4e72  5.Q.R.X.|.S.).Nr
-000102b0: a200 0000 7241 0000 0072 a901 0000 722e  ....rA...r....r.
-000102c0: 0000 0046 7a4a 6835 2066 696c 6520 7072  ...FzJh5 file pr
-000102d0: 6f76 6964 6564 2064 6f65 7320 6e6f 7420  ovided does not 
-000102e0: 6861 7665 2027 6672 616d 655f 6e75 6d73  have 'frame_nums
-000102f0: 2720 6f72 2027 7472 6961 6c5f 6e75 6d73  ' or 'trial_nums
-00010300: 5f61 6e64 5f66 7261 6d65 5f6e 756d 7327  _and_frame_nums'
-00010310: 2904 72aa 0000 0072 ab00 0000 7295 0000  ).r....r....r...
-00010320: 0072 4e00 0000 2903 72d8 0100 0072 d901  .rN...).r....r..
-00010330: 0000 724b 0100 0072 1600 0000 7216 0000  ..rK...r....r...
-00010340: 0072 1700 0000 da0e 6765 745f 6672 616d  .r......get_fram
-00010350: 655f 6e75 6d73 140b 0000 730e 0000 0000  e_nums....s.....
-00010360: 010e 010c 0112 010c 0116 0216 0172 6a02  .............rj.
-00010370: 0000 6306 0000 0000 0000 0000 0000 000f  ..c.............
-00010380: 0000 0009 0000 0043 0000 0073 fa00 0000  .......C...s....
-00010390: 7400 a001 7c00 6401 a102 8fca 7d06 7c05  t...|.d.....}.|.
-000103a0: 6400 6b08 7226 7c06 6402 1900 6400 6400  d.k.r&|.d...d.d.
-000103b0: 8502 1900 7d05 7a1a 7402 a003 7c06 6403  ....}.z.t...|.d.
-000103c0: 1900 6400 6400 8502 1900 a101 7d07 5700  ..d.d.......}.W.
-000103d0: 6e22 0100 0100 0100 7402 a003 7c06 6404  n"......t...|.d.
-000103e0: 1900 6400 6400 8502 1900 a101 7d07 5900  ..d.d.......}.Y.
-000103f0: 6e02 5800 7404 7c00 8301 7d08 7405 7406  n.X.t.|...}.t.t.
-00010400: 7c08 8301 8301 4400 5d58 5c02 7d09 5c02  |.....D.]X\.}.\.
-00010410: 7d0a 7d0b 7c05 6400 6400 8502 7c09 6602  }.}.|.d.d...|.f.
-00010420: 1900 7c0a 1700 7d0c 7c0c 6405 1900 7c01  ..|...}.|.d...|.
-00010430: 1700 7d0d 7c0c 6406 1900 7c02 1800 7d0e  ..}.|.d...|...}.
-00010440: 7407 7c0e 7c0b 6702 8301 7d0e 6406 7c07  t.|.|.g...}.d.|.
-00010450: 7408 7c0d 8301 7408 7c0e 8301 8502 3c00  t.|...t.|.....<.
-00010460: 7178 5700 3500 5100 5200 5800 7c03 72ee  qxW.5.Q.R.X.|.r.
-00010470: 7409 7c00 6403 7c07 6407 8d03 0100 7c04  t.|.d.|.d.....|.
-00010480: 72f6 7c07 5300 6400 5300 2908 4e72 a200  r.|.S.d.S.).Nr..
-00010490: 0000 7265 0200 0072 a701 0000 7252 0000  ..re...r....rR..
-000104a0: 0072 0100 0000 722e 0000 0029 01da 086e  .r....r....)...n
-000104b0: 6577 5f64 6174 6129 0a72 aa00 0000 72ab  ew_data).r....r.
-000104c0: 0000 0072 1d00 0000 7280 0000 0072 6a02  ...r....r....rj.
-000104d0: 0000 7224 0000 0072 3700 0000 7266 0200  ..r$...r7...rf..
-000104e0: 0072 8400 0000 721e 0100 0029 0f72 d801  .r....r....).r..
-000104f0: 0000 5a10 706f 6c65 5f75 705f 7365 745f  ..Z.pole_up_set_
-00010500: 7469 6d65 5a18 706f 6c65 5f64 6f77 6e5f  timeZ.pole_down_
-00010510: 6164 645f 746f 5f74 7269 6767 6572 726b  add_to_triggerrk
-00010520: 0100 0072 6702 0000 7265 0200 0072 d901  ...rg...re...r..
-00010530: 0000 7268 0200 0072 4b01 0000 722c 0000  ..rh...rK...r,..
-00010540: 0072 3f00 0000 7240 0000 0072 bd00 0000  .r?...r@...r....
-00010550: 7255 0200 0072 4102 0000 7216 0000 0072  rU...rA...r....r
-00010560: 1600 0000 7217 0000 00da 0f64 6566 696e  ....r......defin
-00010570: 655f 696e 5f72 616e 6765 1f0b 0000 7324  e_in_range....s$
-00010580: 0000 0000 020e 0108 0110 0202 011a 0106  ................
-00010590: 011c 0208 0118 0114 010c 010c 010c 0120  ............... 
-000105a0: 0104 010e 0104 0172 6c02 0000 6304 0000  .......rl...c...
-000105b0: 0000 0000 0000 0000 0006 0000 0009 0000  ................
-000105c0: 0043 0000 0073 7800 0000 7400 7c00 6401  .C...sx...t.|.d.
-000105d0: 6402 6403 8d03 7d04 7401 a002 7c00 6404  d.d...}.t...|.d.
-000105e0: a102 8f54 7d05 7c01 7c04 6b06 7246 7c03  ...T}.|.|.k.rF|.
-000105f0: 7246 7403 6405 8301 0100 7c05 7c01 3d00  rFt.d.....|.|.=.
-00010600: 7c05 6a04 7c01 7c02 6406 8d02 0100 6e24  |.j.|.|.d.....n$
-00010610: 7c01 7c04 6b06 725c 7c03 735c 7403 6407  |.|.k.r\|.s\t.d.
-00010620: 8301 0100 6e0e 7c05 6a04 7c01 7c02 6406  ....n.|.j.|.|.d.
-00010630: 8d02 0100 5700 3500 5100 5200 5800 6400  ....W.5.Q.R.X.d.
-00010640: 5300 2908 4e54 4672 4902 0000 72a2 0000  S.).NTFrI...r...
-00010650: 007a 286b 6579 2061 6c72 6561 6479 2065  .z(key already e
-00010660: 7869 7374 732c 206f 7665 7277 7269 7469  xists, overwriti
-00010670: 6e67 2076 616c 7565 2e2e 2e72 fd00 0000  ng value...r....
-00010680: 7a5d 6b65 7920 616c 7265 6164 7920 6578  z]key already ex
-00010690: 6973 7473 2c20 4e4f 5420 6f76 6572 7772  ists, NOT overwr
-000106a0: 6974 696e 6720 7661 6c75 652e 2e2e 2c20  iting value..., 
-000106b0: 0a73 6574 2027 6f76 6572 7772 6974 655f  .set 'overwrite_
-000106c0: 6966 5f65 7869 7374 7327 2074 6f20 5472  if_exists' to Tr
-000106d0: 7565 2074 6f20 6f76 6572 7772 6974 6529  ue to overwrite)
-000106e0: 0572 a700 0000 72aa 0000 0072 ab00 0000  .r....r....r....
-000106f0: 724b 0000 0072 ab01 0000 2906 72d8 0100  rK...r....).r...
-00010700: 0072 1d02 0000 da06 7661 6c75 6573 726c  .r......valuesrl
-00010710: 0100 005a 0861 6c6c 5f6b 6579 7372 bc00  ...Z.all_keysr..
-00010720: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00010730: 0072 4a01 0000 370b 0000 7312 0000 0000  .rJ...7...s.....
-00010740: 010e 010e 010c 0108 0106 0110 010c 010a  ................
-00010750: 0272 4a01 0000 6301 0000 0000 0000 0000  .rJ...c.........
-00010760: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00010770: 2a00 0000 7c00 a000 a100 7d00 7401 a002  *...|.....}.t...
-00010780: 7c00 a101 7c00 1800 7d01 7401 a003 7c01  |...|...}.t...|.
-00010790: 7c00 6602 a101 6a04 7d02 7c02 5300 7209  |.f...j.}.|.S.r.
-000107a0: 0100 0029 0572 f500 0000 721d 0000 0072  ...).r....r....r
-000107b0: 4f00 0000 7225 0000 0072 f400 0000 2903  O...r%...r....).
-000107c0: da04 7072 6564 5a09 7a65 726f 5f70 7265  ..predZ.zero_pre
-000107d0: 6472 5300 0000 7216 0000 0072 1600 0000  drS...r....r....
-000107e0: 7217 0000 00da 2162 6f6f 6c5f 7072 6564  r.....!bool_pred
-000107f0: 5f74 6f5f 636c 6173 735f 7072 6564 5f66  _to_class_pred_f
-00010800: 6f72 6d61 7469 6e67 440b 0000 7308 0000  ormatingD...s...
-00010810: 0000 0108 010e 0110 0172 6f02 0000 6302  .........ro...c.
-00010820: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00010830: 0000 0043 0000 0073 bc01 0000 7400 a001  ...C...s....t...
-00010840: 7c00 a101 7d02 7402 6a03 a004 a100 7d03  |...}.t.j.....}.
-00010850: 7405 7c03 a006 a100 8301 7d04 7c01 7c04  t.|.......}.|.|.
-00010860: 6401 1900 6b02 733c 7c01 7c03 7c04 6401  d...k.s<|.|.|.d.
-00010870: 1900 1900 6b02 7258 6401 7c02 7c02 6402  ....k.rXd.|.|.d.
-00010880: 6b05 3c00 6403 7c02 7c02 6404 6b05 3c00  k.<.d.|.|.d.k.<.
-00010890: 9001 6e60 7c01 7c04 6403 1900 6b02 7374  ..n`|.|.d...k.st
-000108a0: 7c01 7c03 7c04 6403 1900 1900 6b02 7290  |.|.|.d.....k.r.
-000108b0: 6401 7c02 7c02 6405 6b05 3c00 6403 7c02  d.|.|.d.k.<.d.|.
-000108c0: 7c02 6404 6b05 3c00 9001 6e28 7c01 7c04  |.d.k.<...n(|.|.
-000108d0: 6404 1900 6b02 73ac 7c01 7c03 7c04 6404  d...k.s.|.|.|.d.
-000108e0: 1900 1900 6b02 72c0 7407 6406 7c01 1700  ....k.r.t.d.|...
-000108f0: 6407 1700 8301 0100 6400 5300 7c01 7c04  d.......d.S.|.|.
-00010900: 6405 1900 6b02 73dc 7c01 7c03 7c04 6405  d...k.s.|.|.|.d.
-00010910: 1900 1900 6b02 72e6 7407 6408 8301 0100  ....k.r.t.d.....
-00010920: 6ed2 7c01 7c04 6402 1900 6b02 9001 7306  n.|.|.d...k...s.
-00010930: 7c01 7c03 7c04 6402 1900 1900 6b02 9001  |.|.|.d.....k...
-00010940: 721a 7407 6406 7c01 1700 6407 1700 8301  r.t.d.|...d.....
-00010950: 0100 6400 5300 7c01 7c04 6409 1900 6b02  ..d.S.|.|.d...k.
-00010960: 9001 733a 7c01 7c03 7c04 6409 1900 1900  ..s:|.|.|.d.....
-00010970: 6b02 9001 724e 7407 6406 7c01 1700 6407  k...rNt.d.|...d.
-00010980: 1700 8301 0100 6400 5300 7c01 7c04 640a  ......d.S.|.|.d.
-00010990: 1900 6b02 9001 736e 7c01 7c03 7c04 640a  ..k...sn|.|.|.d.
-000109a0: 1900 1900 6b02 9001 72ac 6401 7c02 7c02  ....k...r.d.|.|.
-000109b0: 6405 6b05 3c00 7c02 6404 6b02 7d05 7408  d.k.<.|.d.k.}.t.
-000109c0: a009 7c05 6403 6400 8502 1900 640b a102  ..|.d.d.....d...
-000109d0: 7d05 6403 7c02 7c05 3c00 6403 7c02 7c02  }.d.|.|.<.d.|.|.
-000109e0: 6404 6b02 3c00 6e0c 740a 640c 7c01 1700  d.k.<.n.t.d.|...
-000109f0: 8301 8201 7c02 5300 290d 4e72 0100 0000  ....|.S.).Nr....
-00010a00: 72d5 0000 0072 2e00 0000 7247 0000 0072  r....r....rG...r
-00010a10: 4600 0000 7a15 6361 6e20 6e6f 7420 636f  F...z.can not co
-00010a20: 6e76 6572 7420 7479 7065 207a 0f20 7265  nvert type z. re
-00010a30: 7475 726e 696e 6720 4e6f 6e65 7a1d 616c  turning Nonez.al
-00010a40: 7265 6164 7920 696e 2074 6865 2063 6f72  ready in the cor
-00010a50: 7265 6374 2066 6f72 6d61 7472 9700 0000  rect formatr....
-00010a60: 7253 0200 0046 7a24 6b65 7920 646f 6573  rS...Fz$key does
-00010a70: 206e 6f74 206d 6174 6368 2e20 696e 7661   not match. inva
-00010a80: 6c69 6420 6b65 7920 2d2d 3e20 290b 721b  lid key --> ).r.
-00010a90: 0000 0072 1c00 0000 72bc 0100 0072 0500  ...r....r....r..
-00010aa0: 0000 5a1b 6c61 6265 6c5f 6e61 6d69 6e67  ..Z.label_naming
-00010ab0: 5f73 686f 7274 6861 6e64 5f64 6963 7472  _shorthand_dictr
-00010ac0: 3900 0000 7295 0000 0072 4b00 0000 721d  9...r....rK...r.
-00010ad0: 0000 0072 2300 0000 da0a 5661 6c75 6545  ...r#.....ValueE
-00010ae0: 7272 6f72 2906 7242 0000 0072 1d02 0000  rror).rB...r....
-00010af0: 72e1 0000 005a 096e 616d 655f 6469 6374  r....Z.name_dict
-00010b00: 7295 0000 005a 146f 6e65 5f74 6f5f 7468  r....Z.one_to_th
-00010b10: 655f 6c65 6674 5f69 6e64 7372 1600 0000  e_left_indsr....
-00010b20: 7216 0000 0072 1700 0000 da1d 636f 6e76  r....r......conv
-00010b30: 6572 745f 6c61 6265 6c73 5f62 6163 6b5f  ert_labels_back_
-00010b40: 746f 5f62 696e 6172 794b 0b00 0073 3800  to_binaryK...s8.
-00010b50: 0000 0001 0a06 0a01 0c01 1c01 0c01 1002  ................
-00010b60: 1c01 0c01 1002 1c01 1001 0401 1c01 0a01  ................
-00010b70: 2001 1001 0401 2001 1001 0401 2001 0c01   ..... ..... ...
-00010b80: 0801 1401 0801 0e02 0c01 7271 0200 0063  ..........rq...c
-00010b90: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00010ba0: 0300 0000 4300 0000 7326 0000 0064 017d  ....C...s&...d.}
-00010bb0: 0074 00a0 017c 00a1 01a0 02a1 007d 0174  .t...|.......}.t
-00010bc0: 037c 0183 0101 0074 0364 0283 0101 0064  .|.....t.d.....d
-00010bd0: 0053 0029 034e 7a32 7079 7468 6f6e 3320  .S.).Nz2python3 
-00010be0: 222f 5573 6572 732f 7068 696c 2f44 726f  "/Users/phil/Dro
-00010bf0: 7062 6f78 2f55 5044 4154 455f 5748 4143  pbox/UPDATE_WHAC
-00010c00: 435f 5059 5049 2e70 7922 7a7b 706c 6561  C_PYPI.py"z{plea
-00010c10: 7365 2072 6566 6572 2074 6f20 7468 6520  se refer to the 
-00010c20: 6f70 656e 2074 6572 6d69 6e61 6c20 7769  open terminal wi
-00010c30: 6e64 6f77 2066 6f72 2066 7572 7468 6572  ndow for further
-00010c40: 2064 6574 6169 6c73 0a72 6572 756e 2075   details.rerun u
-00010c50: 7469 6c73 2e64 6f77 6e6c 6f61 645f 7265  tils.download_re
-00010c60: 736e 6574 5f6d 6f64 656c 2829 2074 6f20  snet_model() to 
-00010c70: 7075 7420 7468 6520 6d6f 6465 6c20 6669  put the model fi
-00010c80: 6c65 2062 6163 6b29 0472 5f00 0000 da05  le back).r_.....
-00010c90: 706f 7065 6e72 4901 0000 724b 0000 0029  popenrI...rK...)
-00010ca0: 0272 5300 0000 728f 0000 0072 1600 0000  .rS...r....r....
-00010cb0: 7216 0000 0072 1700 0000 da0c 7570 6461  r....r......upda
-00010cc0: 7465 5f77 6861 6363 720b 0000 730c 0000  te_whaccr...s...
-00010cd0: 0000 0804 010e 0108 0102 0102 ff72 7302  .............rs.
-00010ce0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00010cf0: 0000 0005 0000 0043 0000 0073 a400 0000  .......C...s....
-00010d00: 7400 7c00 7401 8302 739c 7c01 7316 7402  t.|.t...s.|.s.t.
-00010d10: 6401 8301 0100 7403 7c00 8301 7404 6a05  d.....t.|...t.j.
-00010d20: 6b08 722c 7c00 6701 7d02 6e6c 6402 7406  k.r,|.g.}.nld.t.
-00010d30: 7403 7c00 8301 8301 a007 a100 6b06 724a  t.|.........k.rJ
-00010d40: 7401 7c00 8301 7d02 6e4e 7403 7c00 8301  t.|...}.nNt.|...
-00010d50: 6a08 7404 6a09 6b02 7280 7402 7403 7c00  j.t.j.k.r.t.t.|.
-00010d60: 8301 8301 0100 6403 7398 740a 6404 7406  ......d.s.t.d.t.
-00010d70: 7403 7c00 8301 8301 1700 8301 8201 6e18  t.|...........n.
-00010d80: 7400 7c00 7406 8302 7292 7c00 6701 7d02  t.|.t...r.|.g.}.
-00010d90: 6e06 7c00 6701 7d02 7c02 5300 7c00 5300  n.|.g.}.|.S.|.S.
-00010da0: 6400 5300 2905 4e7a 5e69 6e70 7574 2069  d.S.).Nz^input i
-00010db0: 7320 7375 7070 6f73 6564 2074 6f20 6265  s supposed to be
-00010dc0: 2061 206c 6973 742c 2063 6f6e 7665 7274   a list, convert
-00010dd0: 696e 6720 6974 2062 7574 2075 7365 7220  ing it but user 
-00010de0: 7368 6f75 6c64 2064 6f20 7468 6973 2074  should do this t
-00010df0: 6f20 7375 7070 7265 7373 2074 6869 7320  o suppress this 
-00010e00: 7761 726e 696e 6772 2a02 0000 467a 5473  warningr*...FzTs
-00010e10: 6565 206d 6f64 756c 6520 7768 6163 632e  ee module whacc.
-00010e20: 7574 696c 732e 6d61 6b65 5f6c 6973 742c  utils.make_list,
-00010e30: 2077 6520 6861 7665 206e 6f74 206f 6666   we have not off
-00010e40: 6963 6961 6c20 7072 6f74 6f63 6f6c 2066  icial protocol f
-00010e50: 6f72 2074 6869 7320 696e 7075 7420 7479  or this input ty
-00010e60: 7065 2029 0b72 0701 0000 7239 0000 0072  pe ).r....r9...r
-00010e70: 4b00 0000 7218 0100 0072 1d00 0000 da04  K...r....r......
-00010e80: 7374 725f 72a9 0000 0072 1901 0000 7272  str_r....r....rr
-00010e90: 0100 0072 7301 0000 724e 0000 0029 0372  ...rs...rN...).r
-00010ea0: 5300 0000 7256 0000 0072 4102 0000 7216  S...rV...rA...r.
-00010eb0: 0000 0072 1600 0000 7217 0000 0072 5700  ...r....r....rW.
-00010ec0: 0000 810b 0000 7322 0000 0000 010a 0104  ......s"........
-00010ed0: 0108 010e 0108 0314 010a 0110 010c 010a  ................
-00010ee0: 0106 ff0a 020a 0108 0206 0104 0272 5700  .............rW.
-00010ef0: 0000 da07 696e 6469 6365 7363 0300 0000  ....indicesc....
-00010f00: 0000 0000 0000 0000 0700 0000 0500 0000  ................
-00010f10: 4300 0000 736e 0000 007c 006a 007c 016a  C...sn...|.j.|.j
-00010f20: 0002 007d 037d 0474 01a0 027c 04a1 017d  ...}.}.t...|...}
-00010f30: 057c 0074 01a0 027c 037c 0418 0064 0117  .|.t...|.|...d..
-00010f40: 00a1 0164 0064 0085 0264 0066 0219 007c  ...d.d...d.f...|
-00010f50: 0517 0019 007c 016b 02a0 0364 01a1 017d  .....|.k...d...}
-00010f60: 067c 0264 026b 0272 5e74 01a0 047c 06a1  .|.d.k.r^t...|..
-00010f70: 0164 0319 0053 007c 0264 046b 0272 6a7c  .d...S.|.d.k.rj|
-00010f80: 0653 0064 0053 0029 054e 722e 0000 0072  .S.d.S.).Nr....r
-00010f90: 7502 0000 7201 0000 0072 8200 0000 2905  u...r....r....).
-00010fa0: 722c 0100 0072 1d00 0000 72b0 0000 0072  r,...r....r....r
-00010fb0: 2f00 0000 72b5 0000 0029 07da 0361 7272  /...r....)...arr
-00010fc0: da03 7365 71da 0b72 6574 7572 6e5f 7479  ..seq..return_ty
-00010fd0: 7065 5a02 4e61 5a04 4e73 6571 5a05 725f  peZ.NaZ.NseqZ.r_
-00010fe0: 7365 71da 014d 7216 0000 0072 1600 0000  seq..Mr....r....
-00010ff0: 7217 0000 00da 1573 6561 7263 685f 7365  r......search_se
-00011000: 7175 656e 6365 5f6e 756d 7079 980b 0000  quence_numpy....
-00011010: 730e 0000 0000 010e 010a 0130 0208 010e  s..........0....
-00011020: 0108 0172 7a02 0000 6303 0000 0000 0000  ...rz...c.......
-00011030: 0000 0000 000e 0000 0009 0000 0043 0000  .............C..
-00011040: 0073 aa00 0000 6700 7d03 7400 7c02 8301  .s....g.}.t.|...
-00011050: 6401 1700 7d04 7401 7402 7c00 8301 8301  d...}.t.t.|.....
-00011060: 4400 5d56 5c02 7d05 5c02 7d06 7d07 7c01  D.]V\.}.\.}.}.|.
-00011070: 7c06 7c07 8502 1900 7d08 7403 7c08 6402  |.|.....}.t.|.d.
-00011080: 6403 8d02 5c02 7d09 7d0a 7404 a005 6404  d...\.}.}.t...d.
-00011090: 6405 8400 7c09 4400 8301 7404 a006 6401  d...|.D...t...d.
-000110a0: 7c04 7c04 a103 a102 5c02 7d0b 7d0c 7c03  |.|.....\.}.}.|.
-000110b0: a007 7c0b a101 0100 711c 7404 a008 7c03  ..|.....q.t...|.
-000110c0: a101 7d03 7c03 7404 a008 7c02 a101 1400  ..}.|.t...|.....
-000110d0: 7d03 7404 a009 7404 a00a 7404 6a0b 7c03  }.t...t...t.j.|.
-000110e0: 6401 6406 8d02 a101 a101 7d0d 7c0d 5300  d.d.......}.|.S.
-000110f0: 2907 4e72 2e00 0000 7201 0000 0029 0172  ).Nr....r....).r
-00011100: ec00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00011110: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00011120: 0000 6700 7c00 5d0c 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-00011130: 9102 7104 5300 7216 0000 0072 4800 0000  ..q.S.r....rH...
-00011140: 7231 0000 0072 1600 0000 7216 0000 0072  r1...r....r....r
-00011150: 1700 0000 7234 0000 00a9 0b00 0073 0400  ....r4.......s..
-00011160: 0000 0600 0200 7a3b 6669 6e64 5f74 7269  ......z;find_tri
-00011170: 616c 735f 7769 7468 5f73 7573 7069 6369  als_with_suspici
-00011180: 6f75 735f 7072 6564 6963 7469 6f6e 732e  ous_predictions.
-00011190: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000111a0: 6d70 3e72 fb00 0000 290c 7230 0000 0072  mp>r....).r0...r
-000111b0: 2400 0000 7237 0000 0072 3b00 0000 721d  $...r7...r;...r.
-000111c0: 0000 00da 0968 6973 746f 6772 616d 7289  .....histogramr.
-000111d0: 0000 0072 2300 0000 7238 0000 0072 9301  ...r#...r8...r..
-000111e0: 0000 7286 0000 00da 076e 616e 6d65 616e  ..r......nanmean
-000111f0: 290e 7241 0000 005a 0970 7265 645f 626f  ).rA...Z.pred_bo
-00011200: 6f6c 5a0b 746d 705f 7765 6967 6874 735a  olZ.tmp_weightsZ
-00011210: 0861 6c6c 5f6c 656e 73da 0462 696e 7372  .all_lens..binsr
-00011220: 2c00 0000 72b9 0000 0072 ba00 0000 72fd  ,...r....r....r.
-00011230: 0100 0072 e100 0000 7242 0000 0072 bb00  ...r....rB...r..
-00011240: 0000 7253 0000 005a 1d73 6f72 7465 645f  ..rS...Z.sorted_
-00011250: 776f 7273 745f 6573 7469 6d61 7465 645f  worst_estimated_
-00011260: 7472 6961 6c73 7216 0000 0072 1600 0000  trialsr....r....
-00011270: 7217 0000 00da 2766 696e 645f 7472 6961  r.....'find_tria
-00011280: 6c73 5f77 6974 685f 7375 7370 6963 696f  ls_with_suspicio
-00011290: 7573 5f70 7265 6469 6374 696f 6e73 a30b  us_predictions..
-000112a0: 0000 7316 0000 0000 0104 010c 0118 010c  ..s.............
-000112b0: 0110 0124 010c 010a 020e 011a 0172 7e02  ...$.........r~.
-000112c0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000112d0: 0000 0003 0000 0043 0000 0073 3800 0000  .......C...s8...
-000112e0: 7400 6a01 a002 7c00 a101 721a 7400 6a01  t.j...|...r.t.j.
-000112f0: a003 7c00 a101 7d00 6e1a 7400 6a01 a004  ..|...}.n.t.j...
-00011300: 7c00 a101 7228 6e0c 6401 7334 7405 6402  |...r(n.d.s4t.d.
-00011310: 8301 8201 7c00 5300 2903 4e46 7a1c 7468  ....|.S.).NFz.th
-00011320: 6973 2069 7320 6e6f 7420 6120 7061 7468  is is not a path
-00011330: 206f 7220 6120 6669 6c65 2906 725f 0000   or a file).r_..
-00011340: 0072 6100 0000 72a5 0000 0072 a300 0000  .ra...r....r....
-00011350: 7262 0000 0072 4e00 0000 2901 da06 7374  rb...rN...)...st
-00011360: 725f 696e 7216 0000 0072 1600 0000 7217  r_inr....r....r.
-00011370: 0000 00da 0b61 7373 6572 745f 7061 7468  .....assert_path
-00011380: b20b 0000 730c 0000 0000 010c 010e 010c  ....s...........
-00011390: 0102 020c 0172 8002 0000 6301 0000 0000  .....r....c.....
-000113a0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000113b0: 0000 0073 4e00 0000 7400 7c00 8301 7d00  ...sN...t.|...}.
-000113c0: 7401 a002 a100 6401 6b02 7220 7403 a004  t.....d.k.r t...
-000113d0: 7c00 a101 0100 6e2a 7401 a002 a100 6402  |.....n*t.....d.
-000113e0: 6b02 723c 7405 a006 6403 7c00 6702 a101  k.r<t...d.|.g...
-000113f0: 0100 6e0e 7405 a006 6404 7c00 6702 a101  ..n.t...d.|.g...
-00011400: 0100 6400 5300 2905 4eda 0757 696e 646f  ..d.S.).N..Windo
-00011410: 7773 da06 4461 7277 696e 72b6 0100 007a  ws..Darwinr....z
-00011420: 0878 6467 2d6f 7065 6e29 0772 8002 0000  .xdg-open).r....
-00011430: da08 706c 6174 666f 726d da06 7379 7374  ..platform..syst
-00011440: 656d 725f 0000 005a 0973 7461 7274 6669  emr_...Z.startfi
-00011450: 6c65 da0a 7375 6270 726f 6365 7373 da05  le..subprocess..
-00011460: 506f 7065 6e72 6f00 0000 7216 0000 0072  Popenro...r....r
-00011470: 1600 0000 7217 0000 00da 0b6f 7065 6e5f  ....r......open_
-00011480: 666f 6c64 6572 bc0b 0000 730c 0000 0000  folder....s.....
-00011490: 0108 010c 010c 010c 0110 0272 8702 0000  ...........r....
-000114a0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000114b0: 0004 0000 0043 0000 0073 3c00 0000 7c00  .....C...s<...|.
-000114c0: 6a00 6401 1900 6401 6b02 7222 7401 7402  j.d...d.k.r"t.t.
-000114d0: a003 7c00 a101 7c01 6402 8d02 7d02 6e16  ..|...|.d...}.n.
-000114e0: 7404 7402 a003 7c00 a101 7c01 6401 6702  t.t...|...|.d.g.
-000114f0: 6402 8d02 7d02 7c02 5300 2903 4e72 2e00  d...}.|.S.).Nr..
-00011500: 0000 2901 5a0b 6b65 726e 656c 5f73 697a  ..).Z.kernel_siz
-00011510: 6529 0572 2100 0000 7209 0000 0072 1b00  e).r!...r....r..
-00011520: 0000 721c 0000 0072 0a00 0000 2903 da0c  ..r....r....)...
-00011530: 7072 6564 5f62 6f6f 6c5f 696e da0e 6b65  pred_bool_in..ke
-00011540: 726e 656c 5f73 697a 655f 696e da0d 7072  rnel_size_in..pr
-00011550: 6564 5f62 6f6f 6c5f 6f75 7472 1600 0000  ed_bool_outr....
-00011560: 7216 0000 0072 1700 0000 da19 6d65 6466  r....r......medf
-00011570: 696c 745f 636f 6e66 6964 656e 6365 5f73  ilt_confidence_s
-00011580: 636f 7265 73c6 0b00 0073 0800 0000 0001  cores....s......
-00011590: 0e01 1402 1601 728b 0200 0072 9800 0000  ......r....r....
-000115a0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000115b0: 0004 0000 0043 0000 0073 3200 0000 7c00  .....C...s2...|.
-000115c0: 6a00 6401 1900 6401 6b02 7220 7c00 7c01  j.d...d.k.r |.|.
-000115d0: 6b04 6401 1400 a001 a100 7d02 6e0e 7402  k.d.......}.n.t.
-000115e0: 6a03 7c00 6401 6402 8d02 7d02 7c02 5300  j.|.d.d...}.|.S.
-000115f0: 2903 4e72 2e00 0000 72fb 0000 0029 0472  ).Nr....r....).r
-00011600: 2100 0000 72f5 0000 0072 1d00 0000 72eb  !...r....r....r.
-00011610: 0000 0029 0372 8802 0000 da09 7468 7265  ...).r......thre
-00011620: 7368 5f69 6e72 8a02 0000 7216 0000 0072  sh_inr....r....r
-00011630: 1600 0000 7217 0000 00da 1963 6f6e 6669  ....r......confi
-00011640: 6465 6e63 655f 7363 6f72 655f 746f 5f63  dence_score_to_c
-00011650: 6c61 7373 ce0b 0000 7308 0000 0000 010e  lass....s.......
-00011660: 0112 020e 0272 8d02 0000 6304 0000 0000  .....r....c.....
-00011670: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-00011680: 0000 0073 3c00 0000 7400 7c00 7c03 8302  ...s<...t.|.|...
-00011690: 7d04 7401 7c04 7c02 8302 7d04 6401 a002  }.t.|.|...}.d...
-000116a0: 7c01 a003 6402 a101 6403 1900 a003 6404  |...d...d.....d.
-000116b0: a101 a101 7d05 7404 7c04 7c05 8302 7d04  ....}.t.|.|...}.
-000116c0: 7c04 5300 2905 4e72 e201 0000 da02 5f5f  |.S.).Nr......__
-000116d0: 7246 0000 0072 8701 0000 2905 728b 0200  rF...r....).r...
-000116e0: 0072 8d02 0000 72d6 0000 0072 d700 0000  .r....r....r....
-000116f0: 7271 0200 0029 0672 8802 0000 5a0b 6b65  rq...).r....Z.ke
-00011700: 795f 6e61 6d65 5f69 6e72 8c02 0000 7289  y_name_inr....r.
-00011710: 0200 0072 8a02 0000 5a06 4c5f 6b65 795f  ...r....Z.L_key_
-00011720: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00011730: 1970 726f 6365 7373 5f63 6f6e 6669 6465  .process_confide
-00011740: 6e63 655f 7363 6f72 6573 d70b 0000 730a  nce_scores....s.
-00011750: 0000 0000 010a 010a 011a 010a 0172 8f02  .............r..
-00011760: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
-00011770: 0000 0008 0000 0043 0000 0073 8000 0000  .......C...s....
-00011780: 7400 6a01 a002 7c00 a101 7d00 7403 7c00  t.j...|...}.t.|.
-00011790: 8301 7403 7400 6a01 6a04 8301 1700 7d02  ..t.t.j.j.....}.
-000117a0: 7405 7c01 8301 6a06 6401 6401 6402 8d02  t.|...j.d.d.d...
-000117b0: 0100 7400 a007 7c00 a101 4400 5d3e 5c03  ..t...|...D.]>\.
-000117c0: 7d03 7d04 7d05 7c04 4400 5d2e 7d06 7400  }.}.}.|.D.].}.t.
-000117d0: 6a01 a008 7c01 7c03 7c02 6400 8502 1900  j...|.|.|.d.....
-000117e0: 7c06 a103 7d07 7405 7c07 8301 6a06 6401  |...}.t.|...j.d.
-000117f0: 6401 6402 8d02 0100 714a 713c 6400 5300  d.d.....qJq<d.S.
-00011800: 725b 0100 0029 0972 5f00 0000 7261 0000  r[...).r_...ra..
-00011810: 00da 0761 6273 7061 7468 7230 0000 0072  ...abspathr0...r
-00011820: 6000 0000 720e 0000 0072 5f01 0000 720e  `...r....r_...r.
-00011830: 0200 0072 d600 0000 2908 da03 7372 6372  ...r....)...srcr
-00011840: 7c00 0000 5a0a 7372 635f 7072 6566 6978  |...Z.src_prefix
-00011850: 7211 0200 0072 1202 0000 7213 0200 0072  r....r....r....r
-00011860: a300 0000 da07 6469 7270 6174 6872 1600  ......dirpathr..
-00011870: 0000 7216 0000 0072 1700 0000 7295 0100  ..r....r....r...
-00011880: 00df 0b00 0073 0e00 0000 0001 0c01 1401  .....s..........
-00011890: 1201 1401 0801 1801 7295 0100 0063 0800  ........r....c..
-000118a0: 0000 0000 0000 0000 0000 0f00 0000 0600  ................
-000118b0: 0000 4300 0000 7350 0100 007c 00a0 0074  ..C...sP...|...t
-000118c0: 016a 02a1 0174 016a 0217 007d 007c 01a0  .j...t.j...}.|..
-000118d0: 0074 016a 02a1 0174 016a 0217 007d 0174  .t.j...t.j...}.t
-000118e0: 037c 0064 0164 028d 027d 0874 047c 087c  .|.d.d...}.t.|.|
-000118f0: 027c 0364 038d 037d 097c 0572 6464 0464  .|.d...}.|.rdd.d
-00011900: 0584 0074 057c 0983 0144 0083 017d 0a7c  ...t.|...D...}.|
-00011910: 0772 607c 0964 0666 0253 0064 0653 0067  .r`|.d.f.S.d.S.g
-00011920: 007d 0b7c 0944 005d 3e7d 0c7c 01a0 067c  .}.|.D.]>}.|...|
-00011930: 0ca0 077c 00a1 01a1 017d 0d74 016a 08a0  ...|.....}.t.j..
-00011940: 097c 0ca1 0172 a074 0a7c 0d83 016a 0b64  .|...r.t.|...j.d
-00011950: 0764 0764 088d 0201 0071 6c7c 0ba0 0c7c  .d.d.....ql|...|
-00011960: 0ca1 0101 0071 6c67 007d 0e74 0d7c 0b7c  .....qlg.}.t.|.|
-00011970: 0664 098d 0244 005d 807d 0c7c 01a0 067c  .d...D.].}.|...|
-00011980: 0ca0 077c 00a1 01a1 017d 0d7c 0ea0 0c7c  ...|.....}.|...|
-00011990: 0da1 0101 007c 0473 ec74 016a 08a0 0e7c  .....|.s.t.j...|
-000119a0: 0da1 0190 0173 2c74 016a 08a0 0e7c 0da1  .....s,t.j...|..
-000119b0: 0190 0172 0474 01a0 0f7c 0da1 0101 0074  ...r.t...|.....t
-000119c0: 0a74 016a 08a0 107c 0da1 0183 016a 0b64  .t.j...|.....j.d
-000119d0: 0764 0764 088d 0201 0074 11a0 127c 0c7c  .d.d.....t...|.|
-000119e0: 0da1 0201 0071 bc7c 0473 bc74 1364 0a7c  .....q.|.s.t.d.|
-000119f0: 0d17 0083 0101 0071 bc7c 0790 0172 4c7c  .......q.|...rL|
-00011a00: 0b7c 0e66 0253 0064 0653 0029 0b61 ee02  .|.f.S.d.S.).a..
-00011a10: 0000 0a0a 2020 2020 5061 7261 6d65 7465  ....    Paramete
-00011a20: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00011a30: 2d0a 2020 2020 7265 7475 726e 5f6c 6973  -.    return_lis
-00011a40: 745f 6f66 5f66 696c 6573 203a 0a20 2020  t_of_files :.   
-00011a50: 2073 7263 203a 2073 6f75 7263 6520 666f   src : source fo
-00011a60: 6c64 6572 0a20 2020 2064 7374 203a 2064  lder.    dst : d
-00011a70: 6573 7469 6e61 7469 6f6e 2066 6f6c 6465  estination folde
-00011a80: 720a 2020 2020 6b65 6570 5f73 7472 696e  r.    keep_strin
-00011a90: 6773 203a 2073 6565 2075 7469 6c73 2e6c  gs : see utils.l
-00011aa0: 6973 7465 725f 6974 2c20 6c69 7374 206f  ister_it, list o
-00011ab0: 6620 7374 7269 6e67 7320 746f 206d 6174  f strings to mat
-00011ac0: 6368 2069 6e20 6f72 6465 7220 746f 2063  ch in order to c
-00011ad0: 6f70 790a 2020 2020 7265 6d6f 7665 5f73  opy.    remove_s
-00011ae0: 7472 696e 6720 3a20 7365 6520 7574 696c  tring : see util
-00011af0: 732e 6c69 7374 6572 5f69 742c 206c 6973  s.lister_it, lis
-00011b00: 7420 6f66 2073 7472 696e 6773 2074 6f20  t of strings to 
-00011b10: 6d61 7463 6820 696e 206f 7264 6572 2074  match in order t
-00011b20: 6f20 6e6f 7420 636f 7079 0a20 2020 206f  o not copy.    o
-00011b30: 7665 7277 7269 7465 203a 2077 696c 6c20  verwrite : will 
-00011b40: 6f76 6572 7772 6974 6520 6669 6c65 7320  overwrite files 
-00011b50: 6966 2074 7275 650a 2020 2020 6a75 7374  if true.    just
-00011b60: 5f70 7269 6e74 5f77 6861 745f 7769 6c6c  _print_what_will
-00011b70: 5f62 655f 636f 7069 6564 203a 2063 616e  _be_copied : can
-00011b80: 206a 7573 7420 7072 696e 7420 7768 6174   just print what
-00011b90: 2077 696c 6c20 6265 2063 6f70 6965 6420   will be copied 
-00011ba0: 746f 2062 6520 7375 7265 2069 7420 6973  to be sure it is
-00011bb0: 2063 6f72 7265 6374 0a20 2020 2064 6973   correct.    dis
-00011bc0: 6162 6c65 5f74 7164 6d20 3a20 6966 2054  able_tqdm : if T
-00011bd0: 7275 6520 6974 2077 696c 6c20 7072 6576  rue it will prev
-00011be0: 656e 7420 7468 6520 5451 444d 206c 6f61  ent the TQDM loa
-00011bf0: 6469 6e67 2062 6172 0a0a 2020 2020 4578  ding bar..    Ex
-00011c00: 616d 706c 6573 0a20 2020 205f 5f5f 5f5f  amples.    _____
-00011c10: 5f5f 5f0a 2020 2020 636f 7079 5f66 696c  ___.    copy_fil
-00011c20: 655f 6669 6c74 6572 2827 2f55 7365 7273  e_filter('/Users
-00011c30: 2f70 6869 6c2f 4465 736b 746f 702f 4641  /phil/Desktop/FA
-00011c40: 4b45 5f66 756c 6c5f 6461 7461 272c 2027  KE_full_data', '
-00011c50: 2f55 7365 7273 2f70 6869 6c2f 4465 736b  /Users/phil/Desk
-00011c60: 746f 702f 6161 6161 6161 6161 6161 272c  top/aaaaaaaaaa',
-00011c70: 206b 6565 705f 7374 7269 6e67 733d 272f   keep_strings='/
-00011c80: 336c 6167 2f27 2c0a 2020 2020 2020 2020  3lag/',.        
-00011c90: 2020 2020 2020 2020 2072 656d 6f76 655f           remove_
-00011ca0: 7374 7269 6e67 3d4e 6f6e 652c 206f 7665  string=None, ove
-00011cb0: 7277 7269 7465 3d54 7275 652c 206a 7573  rwrite=True, jus
-00011cc0: 745f 7072 696e 745f 7768 6174 5f77 696c  t_print_what_wil
-00011cd0: 6c5f 6265 5f63 6f70 6965 643d 4661 6c73  l_be_copied=Fals
-00011ce0: 6529 0a20 2020 2052 6574 7572 6e73 0a20  e).    Returns. 
-00011cf0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-00011d00: da01 2a29 0172 1002 0000 2902 72d4 0100  ..*).r....).r...
-00011d10: 0072 d501 0000 6301 0000 0000 0000 0000  .r....c.........
-00011d20: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
-00011d30: 2400 0000 6700 7c00 5d1c 5c02 7d01 7d02  $...g.|.].\.}.}.
-00011d40: 7400 7401 7c01 8301 6400 1700 7c02 1700  t.t.|...d...|...
-00011d50: 8301 9102 7104 5300 2901 7287 0100 0029  ....q.S.).r....)
-00011d60: 0272 4b00 0000 72a9 0000 0072 0602 0000  .rK...r....r....
-00011d70: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00011d80: 3400 0000 070c 0000 7304 0000 0006 0006  4.......s.......
-00011d90: 007a 2463 6f70 795f 6669 6c65 5f66 696c  .z$copy_file_fil
-00011da0: 7465 722e 3c6c 6f63 616c 733e 2e3c 6c69  ter.<locals>.<li
-00011db0: 7374 636f 6d70 3e4e 5472 5c01 0000 2901  stcomp>NTr\...).
-00011dc0: da07 6469 7361 626c 657a 2c6f 7665 7277  ..disablez,overw
-00011dd0: 7269 7465 203d 2046 616c 7365 3a20 6669  rite = False: fi
-00011de0: 6c65 2065 7869 7374 732c 2073 6b69 7070  le exists, skipp
-00011df0: 696e 672d 2d3e 2029 14da 0672 7374 7269  ing--> )...rstri
-00011e00: 7072 5f00 0000 7260 0000 0072 9201 0000  pr_...r`...r....
-00011e10: 72d6 0100 0072 2400 0000 72d6 0000 0072  r....r$...r....r
-00011e20: d700 0000 7261 0000 0072 6200 0000 720e  ....ra...rb...r.
-00011e30: 0000 0072 5f01 0000 7223 0000 0072 0b00  ...r_...r#...r..
-00011e40: 0000 72a5 0000 0072 7900 0000 72a3 0000  ..r....ry...r...
-00011e50: 0072 7300 0000 da08 636f 7079 6669 6c65  .rs.....copyfile
-00011e60: 724b 0000 0029 0f72 9102 0000 727c 0000  rK...).r....r|..
-00011e70: 0072 d401 0000 72d5 0100 0072 5c00 0000  .r....r....r\...
-00011e80: 5a1e 6a75 7374 5f70 7269 6e74 5f77 6861  Z.just_print_wha
-00011e90: 745f 7769 6c6c 5f62 655f 636f 7069 6564  t_will_be_copied
-00011ea0: 5a0c 6469 7361 626c 655f 7471 646d 5a14  Z.disable_tqdmZ.
-00011eb0: 7265 7475 726e 5f6c 6973 745f 6f66 5f66  return_list_of_f
-00011ec0: 696c 6573 5a12 616c 6c5f 6669 6c65 735f  ilesZ.all_files_
-00011ed0: 616e 645f 6469 7273 5a07 746f 5f63 6f70  and_dirsZ.to_cop
-00011ee0: 7972 e201 0000 5a08 746f 5f63 6f70 7932  yr....Z.to_copy2
-00011ef0: 7233 0000 0072 ba00 0000 5a0c 6669 6e61  r3...r....Z.fina
-00011f00: 6c5f 636f 7069 6564 7216 0000 0072 1600  l_copiedr....r..
-00011f10: 0000 7217 0000 00da 1063 6f70 795f 6669  ..r......copy_fi
-00011f20: 6c65 5f66 696c 7465 72e9 0b00 0073 3800  le_filter....s8.
-00011f30: 0000 0017 1201 1202 0c01 0e02 0401 1201  ................
-00011f40: 0401 0802 0402 0401 0801 1001 0c01 1402  ................
-00011f50: 0c01 0401 1001 1001 0a01 1201 0e01 0a01  ................
-00011f60: 1a01 0e01 0401 0e01 0601 7297 0200 0072  ..........r....r
-00011f70: 6002 0000 6302 0000 0000 0000 0000 0000  `...c...........
-00011f80: 000a 0000 0006 0000 0043 0000 0073 f800  .........C...s..
-00011f90: 0000 6700 7d02 6700 7d03 6700 7d04 7400  ..g.}.g.}.g.}.t.
-00011fa0: 7c00 8301 4400 5dd8 5c02 7d05 7d06 7c06  |...D.].\.}.}.|.
-00011fb0: a001 7402 6a03 a101 7d06 7402 6a04 a005  ..t.j...}.t.j...
-00011fc0: 7c06 a101 7214 7402 6a04 a006 7c06 a101  |...r.t.j...|...
-00011fd0: 7d07 7402 6a03 a007 7c06 a008 7402 6a03  }.t.j...|...t.j.
-00011fe0: a101 6400 6401 8502 1900 a101 7402 6a03  ..d.d.......t.j.
-00011ff0: 1700 7c01 1700 7402 6a03 1700 7d08 7409  ..|...t.j...}.t.
-00012000: 7c08 6402 8302 7d09 6403 7c07 a00a a100  |.d...}.d.|.....
-00012010: 6b06 7290 740b 7c09 6403 6404 8d02 7d09  k.r.t.|.d.d...}.
-00012020: 6e18 6405 7c07 a00a a100 6b06 72a8 740b  n.d.|.....k.r.t.
-00012030: 7c09 6405 6404 8d02 7d09 740c 7c09 8301  |.d.d...}.t.|...
-00012040: 6406 6b02 72d8 7c02 a00d 7c06 a101 0100  d.k.r.|...|.....
-00012050: 7c03 a00d 7c09 6402 1900 a101 0100 7c04  |...|.d.......|.
-00012060: a00d 7c05 a101 0100 7114 740e 6407 7c07  ..|.....q.t.d.|.
-00012070: 1700 6408 1700 8301 0100 0100 71ee 7114  ..d.........q.q.
-00012080: 7c02 7c03 7c04 6603 5300 2909 4e72 e501  |.|.|.f.S.).Nr..
-00012090: 0000 7201 0000 005a 0574 7261 696e 2901  ..r....Z.train).
-000120a0: 72d4 0100 00da 0376 616c 722e 0000 007a  r......valr....z
-000120b0: 0a46 696c 6520 6e61 6d65 207a 1b20 636f  .File name z. co
-000120c0: 756c 6420 6e6f 7420 6669 6e64 2076 616c  uld not find val
-000120d0: 6964 206d 6174 6368 290f 7224 0000 0072  id match).r$...r
-000120e0: 9502 0000 725f 0000 0072 6000 0000 7261  ....r_...r`...ra
-000120f0: 0000 0072 a500 0000 72a4 0000 0072 d600  ...r....r....r..
-00012100: 0000 72d7 0000 0072 2501 0000 7219 0100  ..r....r%...r...
-00012110: 0072 d601 0000 7230 0000 0072 2300 0000  .r....r0...r#...
-00012120: 724b 0000 0029 0a72 1502 0000 5a15 616c  rK...).r....Z.al
-00012130: 745f 6c61 6265 6c5f 666f 6c64 6572 5f6e  t_label_folder_n
-00012140: 616d 655a 0768 355f 696d 6773 5a09 6835  ameZ.h5_imgsZ.h5
-00012150: 5f6c 6162 656c 735a 0d69 6e64 735f 6f66  _labelsZ.inds_of
-00012160: 5f66 696c 6573 722c 0000 0072 3300 0000  _filesr,...r3...
-00012170: 724b 0100 005a 0e61 6c74 5f6c 6162 656c  rK...Z.alt_label
-00012180: 735f 6469 7272 5000 0000 7216 0000 0072  s_dirrP...r....r
-00012190: 1600 0000 7217 0000 00da 2263 6f70 795f  ....r....."copy_
-000121a0: 616c 745f 6c61 6265 6c73 5f62 6173 6564  alt_labels_based
-000121b0: 5f6f 6e5f 6469 7265 6374 6f72 7923 0c00  _on_directory#..
-000121c0: 0073 2800 0000 0001 0401 0401 0401 1001  .s(.............
-000121d0: 0c01 0c01 0c01 2c01 0a01 0c01 0e01 0c01  ......,.........
-000121e0: 0c01 0c01 0a01 0e01 0c02 1001 0601 7299  ..............r.
-000121f0: 0200 0063 0100 0000 0000 0000 0000 0000  ...c............
-00012200: 0100 0000 0600 0000 4300 0000 7380 0000  ........C...s...
-00012210: 0074 0064 0174 01a0 027c 00a1 0183 0201  .t.d.t...|......
-00012220: 0074 0064 0274 01a0 037c 00a1 0183 0201  .t.d.t...|......
-00012230: 0074 0064 0374 01a0 047c 00a1 0183 0201  .t.d.t...|......
-00012240: 0074 0064 047c 006a 0583 0201 0074 0064  .t.d.|.j.....t.d
-00012250: 0574 0674 01a0 077c 00a1 0183 0183 0201  .t.t...|........
-00012260: 0074 0064 0674 087c 0083 0183 0201 007a  .t.d.t.|.......z
-00012270: 1074 0064 077c 006a 0983 0201 0057 006e  .t.d.|.j.....W.n
-00012280: 0c01 0001 0001 0059 006e 0258 0064 0053  .......Y.n.X.d.S
-00012290: 0029 084e 7a04 0a6d 696e 720f 0100 0072  .).Nz..minr....r
-000122a0: 8300 0000 7221 0000 007a 0d6c 656e 206f  ....r!...z.len o
-000122b0: 6620 756e 6971 7565 7218 0100 007a 0644  f uniquer....z.D
-000122c0: 7479 7065 2029 0a72 4b00 0000 721d 0000  type ).rK...r...
-000122d0: 0072 6602 0000 720f 0100 0072 8300 0000  .rf...r....r....
-000122e0: 7221 0000 0072 3000 0000 72ce 0000 0072  r!...r0...r....r
-000122f0: 1801 0000 da05 6474 7970 6529 015a 0669  ......dtype).Z.i
-00012300: 6e5f 6172 7272 1600 0000 7216 0000 0072  n_arrr....r....r
-00012310: 1700 0000 7271 0100 003b 0c00 0073 1400  ....rq...;...s..
-00012320: 0000 0001 1001 1001 1001 0c01 1401 0e01  ................
-00012330: 0201 1001 0601 7271 0100 0063 0200 0000  ......rq...c....
-00012340: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00012350: 4300 0000 7312 0000 007c 0174 007c 0064  C...s....|.t.|.d
-00012360: 0164 0264 038d 036b 0653 0029 044e 5446  .d.d...k.S.).NTF
-00012370: 7249 0200 0029 0172 a700 0000 2902 72be  rI...).r....).r.
-00012380: 0000 00da 066b 6579 5f69 6e72 1600 0000  .....key_inr....
-00012390: 7216 0000 0072 1700 0000 7269 0100 0048  r....r....ri...H
-000123a0: 0c00 0073 0200 0000 0001 7269 0100 0063  ...s......ri...c
-000123b0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000123c0: 0900 0000 4300 0000 732c 0000 0074 007c  ....C...s,...t.|
-000123d0: 007c 0183 0272 2874 01a0 027c 0064 01a1  .|...r(t...|.d..
-000123e0: 028f 0c7d 027c 027c 013d 0057 0035 0051  ...}.|.|.=.W.5.Q
-000123f0: 0052 0058 0064 0053 00a9 024e 72a2 0000  .R.X.d.S...Nr...
-00012400: 00a9 0372 6901 0000 72aa 0000 0072 ab00  ...ri...r....r..
-00012410: 0000 2903 72be 0000 0072 9b02 0000 72bc  ..).r....r....r.
-00012420: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00012430: 0000 7248 0100 004c 0c00 0073 0600 0000  ..rH...L...s....
-00012440: 0001 0a01 0e01 7248 0100 0063 0300 0000  ......rH...c....
-00012450: 0000 0000 0000 0000 0500 0000 0900 0000  ................
-00012460: 4300 0000 7340 0000 0074 007c 007c 0183  C...s@...t.|.|..
-00012470: 027d 0374 01a0 027c 0064 01a1 028f 207d  .}.t...|.d.... }
-00012480: 047c 0372 227c 047c 013d 007c 0264 006b  .|.r"|.|.=.|.d.k
-00012490: 0972 327c 027c 047c 013c 0057 0035 0051  .r2|.|.|.<.W.5.Q
-000124a0: 0052 0058 0064 0053 0072 9c02 0000 729d  .R.X.d.S.r....r.
-000124b0: 0200 0029 0572 be00 0000 729b 0200 0072  ...).r....r....r
-000124c0: 6b02 0000 5a0a 6578 6973 745f 7465 7374  k...Z.exist_test
-000124d0: 72bc 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-000124e0: 1700 0000 721e 0100 0052 0c00 0073 0c00  ....r....R...s..
-000124f0: 0000 0001 0a01 0e01 0401 0601 0801 721e  ..............r.
-00012500: 0100 0063 0100 0000 0000 0000 0000 0000  ...c............
-00012510: 0100 0000 0200 0000 4300 0000 730e 0000  ........C...s...
-00012520: 0064 0164 0284 007c 0044 0083 0153 0029  .d.d...|.D...S.)
-00012530: 034e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00012540: 0000 0006 0000 0053 0000 0073 1800 0000  .......S...s....
-00012550: 6700 7c00 5d10 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
-00012560: a102 9102 7104 5300 7212 0100 0072 1601  ....q.S.r....r..
-00012570: 0000 2902 7232 0000 00da 016e 7216 0000  ..).r2.....nr...
-00012580: 0072 1600 0000 7217 0000 0072 3400 0000  .r....r....r4...
-00012590: 5c0c 0000 7304 0000 0006 0002 007a 3263  \...s........z2c
-000125a0: 6f6e 7665 7274 5f6c 6973 745f 6f66 5f73  onvert_list_of_s
-000125b0: 7472 696e 6773 5f66 6f72 5f68 352e 3c6c  trings_for_h5.<l
-000125c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000125d0: 3e72 1600 0000 2901 721a 0100 0072 1600  >r....).r....r..
-000125e0: 0000 7216 0000 0072 1700 0000 da1e 636f  ..r....r......co
-000125f0: 6e76 6572 745f 6c69 7374 5f6f 665f 7374  nvert_list_of_st
-00012600: 7269 6e67 735f 666f 725f 6835 5b0c 0000  rings_for_h5[...
-00012610: 7302 0000 0000 0172 9f02 0000 6302 0000  s......r....c...
-00012620: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00012630: 0003 0000 0073 1200 0000 8700 6601 6401  .....s......f.d.
-00012640: 6402 8408 7c00 4400 8301 5300 2903 7a55  d...|.D...S.).zU
-00012650: 7265 7475 6e20 696e 6e64 6578 206f 6620  retun inndex of 
-00012660: 6c65 6e67 7468 206c 656e 2861 7272 3129  length len(arr1)
-00012670: 2069 6e73 7465 6164 206f 6620 6e75 6d70   instead of nump
-00012680: 7973 206c 656e 6774 6820 6d69 6e28 5b6c  ys length min([l
-00012690: 656e 2861 7272 3129 2c20 6c65 6e28 6172  en(arr1), len(ar
-000126a0: 7232 295d 2963 0100 0000 0000 0000 0000  r2)])c..........
-000126b0: 0000 0200 0000 0500 0000 1300 0000 7322  ..............s"
-000126c0: 0000 0067 007c 005d 1a7d 0164 0064 0184  ...g.|.].}.d.d..
-000126d0: 0074 0088 0083 0144 0083 017c 0119 0091  .t.....D...|....
-000126e0: 0271 0453 0029 0263 0100 0000 0000 0000  .q.S.).c........
-000126f0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
-00012700: 7316 0000 0069 007c 005d 0e5c 027d 017d  s....i.|.].\.}.}
-00012710: 027c 027c 0193 0271 0453 0072 1600 0000  .|.|...q.S.r....
-00012720: 7216 0000 0029 0372 3200 0000 722c 0000  r....).r2...r,..
-00012730: 0072 0002 0000 7216 0000 0072 1600 0000  .r....r....r....
-00012740: 7217 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
-00012750: 3e61 0c00 0073 0600 0000 0600 0600 0200  >a...s..........
-00012760: 7a2c 696e 7465 7273 6563 745f 616c 6c2e  z,intersect_all.
-00012770: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00012780: 6d70 3e2e 3c64 6963 7463 6f6d 703e 7207  mp>.<dictcomp>r.
-00012790: 0200 0029 0272 3200 0000 7200 0200 00a9  ...).r2...r.....
-000127a0: 0172 e000 0000 7216 0000 0072 1700 0000  .r....r....r....
-000127b0: 7234 0000 0061 0c00 0073 0400 0000 0600  r4...a...s......
-000127c0: 0200 7a21 696e 7465 7273 6563 745f 616c  ..z!intersect_al
-000127d0: 6c2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  l.<locals>.<list
-000127e0: 636f 6d70 3e72 1600 0000 2902 72df 0000  comp>r....).r...
-000127f0: 0072 e000 0000 7216 0000 0072 a102 0000  .r....r....r....
-00012800: 7217 0000 00da 0d69 6e74 6572 7365 6374  r......intersect
-00012810: 5f61 6c6c 5f0c 0000 7302 0000 0000 0272  _all_...s......r
-00012820: a202 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00012830: 0002 0000 0003 0000 0043 0000 0073 2000  .........C...s .
-00012840: 0000 7400 a001 7c00 a101 6a02 6401 1b00  ..t...|...j.d...
-00012850: 7c01 6b04 731c 7403 6402 8301 8201 6400  |.k.s.t.d.....d.
-00012860: 5300 2903 4e69 00ca 9a3b 7a37 7370 6163  S.).Ni...;z7spac
-00012870: 655f 6368 6563 6b20 6675 6e63 7469 6f6e  e_check function
-00012880: 3a20 4742 206c 696d 6974 2072 6561 6368  : GB limit reach
-00012890: 6564 2c20 656e 6469 6e67 2066 756e 6374  ed, ending funct
-000128a0: 696f 6e29 0472 7300 0000 da0a 6469 736b  ion).rs.....disk
-000128b0: 5f75 7361 6765 da04 6672 6565 724e 0000  _usage..freerN..
-000128c0: 0029 0272 6100 0000 5a06 6d69 6e5f 6762  .).ra...Z.min_gb
-000128d0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000128e0: 0b73 7061 6365 5f63 6865 636b 640c 0000  .space_checkd...
-000128f0: 7312 0000 0000 0104 0102 ff04 0102 ff02  s...............
-00012900: 0102 ff06 0102 ff72 a502 0000 2901 7218  .......r....).r.
-00012910: 0000 0029 0246 7201 0000 0029 0246 7201  ...).Fr....).Fr.
-00012920: 0000 0029 0246 7201 0000 0029 0246 7201  ...).Fr....).Fr.
-00012930: 0000 0029 0372 7e00 0000 544e 2905 4e4e  ...).r~...TN).NN
-00012940: 4e46 4e29 014e 2901 4e29 014e 2903 721b  NFN).N).N).N).r.
-00012950: 0100 0072 1c01 0000 72d0 0000 0029 0272  ...r....r....).r
-00012960: 2401 0000 721b 0100 0029 0172 2401 0000  $...r....).r$...
-00012970: 2901 722e 0000 0029 0172 9600 0000 2901  ).r....).r....).
-00012980: 4e29 0172 5801 0000 2905 4e54 4672 6801  N).rX...).NTFrh.
-00012990: 0000 721f 0100 0029 0172 7601 0000 2907  ..r....).rv...).
-000129a0: 7247 0000 004e 5446 4e54 5429 0154 2901  rG...NTFNTT).T).
-000129b0: 4629 0246 7201 0000 0029 0172 d500 0000  F).Fr....).r....
-000129c0: 2902 4654 2901 4e29 0372 d000 0000 4e46  ).FT).N).r....NF
-000129d0: 2904 4e46 4672 db01 0000 2904 5446 4672  ).NFFr....).TFFr
-000129e0: db01 0000 2904 5446 4672 db01 0000 2901  ....).TFFr....).
-000129f0: 722e 0000 0029 0154 2901 72d0 0000 0029  r....).T).r....)
-00012a00: 0146 2901 4629 0146 2902 722d 0200 0072  .F).F).F).r-...r
-00012a10: 7e00 0000 2901 7201 0000 0029 0272 4700  ~...).r....).rG.
-00012a20: 0000 7201 0000 0029 0472 6402 0000 7201  ..r....).rd...r.
-00012a30: 0000 0054 4629 0572 0100 0000 7201 0000  ...TF).r....r...
-00012a40: 0054 464e 2901 4629 0146 2901 7275 0200  .TFN).F).F).ru..
-00012a50: 0029 0172 9800 0000 2902 7298 0000 0072  .).r....).r....r
-00012a60: 2e00 0000 2906 72d0 0000 004e 4646 4646  ....).r....NFFFF
-00012a70: 2901 7260 0200 0029 014e 2901 7247 0000  ).r`...).N).rG..
-00012a80: 0029 a55a 1377 6861 6363 2e66 6561 7475  .).Z.whacc.featu
-00012a90: 7265 5f6d 616b 6572 7202 0000 0072 0300  re_makerr....r..
-00012aa0: 0000 5a12 7768 6163 632e 706f 6c65 5f74  ..Z.whacc.pole_t
-00012ab0: 7261 636b 6572 7204 0000 0072 bc01 0000  rackerr....r....
-00012ac0: 7205 0000 0072 7300 0000 da05 6e75 6d70  r....rs.....nump
-00012ad0: 7972 1d00 0000 725f 0000 00da 0373 7973  yr....r_.....sys
-00012ae0: 72af 0100 005a 076e 6174 736f 7274 7206  r....Z.natsortr.
-00012af0: 0000 0072 0700 0000 5a08 7363 6970 792e  ...r....Z.scipy.
-00012b00: 696f da02 696f 7216 0200 0072 aa00 0000  io..ior....r....
-00012b10: da11 6d61 7470 6c6f 746c 6962 2e70 7970  ..matplotlib.pyp
-00012b20: 6c6f 74da 0670 7970 6c6f 7472 1100 0000  lot..pyplotr....
-00012b30: 5a06 7061 6e64 6173 729b 0100 0072 1b00  Z.pandasr....r..
-00012b40: 0000 7296 0100 0072 0800 0000 7283 0200  ..r....r....r...
-00012b50: 0072 8502 0000 5a0c 7363 6970 792e 7369  .r....Z.scipy.si
-00012b60: 676e 616c 7209 0000 0072 0a00 0000 72b7  gnalr....r....r.
-00012b70: 0100 005a 1174 7164 6d2e 6175 746f 6e6f  ...Z.tqdm.autono
-00012b80: 7465 626f 6f6b 720b 0000 0072 0d00 0000  tebookr....r....
-00012b90: 720c 0000 0072 7701 0000 728b 0000 0072  r....rw...r....r
-00012ba0: c200 0000 da07 7061 7468 6c69 6272 0e00  ......pathlibr..
-00012bb0: 0000 da0e 7572 6c6c 6962 2e72 6571 7565  ....urllib.reque
-00012bc0: 7374 7275 0000 00da 077a 6970 6669 6c65  stru.....zipfile
-00012bd0: 720f 0000 0072 1000 0000 722d 0000 0072  r....r....r-...r
-00012be0: 4400 0000 7254 0000 0072 5800 0000 725d  D...rT...rX...r]
-00012bf0: 0000 0072 4c00 0000 726b 0000 0072 5b00  ...rL...rk...r[.
-00012c00: 0000 725a 0000 0072 5900 0000 7290 0000  ..rZ...rY...r...
-00012c10: 0072 c100 0000 72ca 0000 0072 8a00 0000  .r....r....r....
-00012c20: 72d8 0000 0072 dc00 0000 72db 0000 0072  r....r....r....r
-00012c30: e400 0000 72ed 0000 0072 4d00 0000 7206  ....r....rM...r.
-00012c40: 0100 0072 0801 0000 720d 0100 0072 0a01  ...r....r....r..
-00012c50: 0000 720e 0100 0072 1001 0000 72af 0000  ..r....r....r...
-00012c60: 0072 2301 0000 7227 0100 0072 2901 0000  .r#...r'...r)...
-00012c70: 7233 0100 0072 4e01 0000 7250 0100 0072  r3...rN...rP...r
-00012c80: 7400 0000 729a 0000 0072 5701 0000 72ad  t...r....rW...r.
-00012c90: 0000 0072 a600 0000 7261 0100 0072 6601  ...r....ra...rf.
-00012ca0: 0000 7267 0100 0072 6f01 0000 7275 0100  ..rg...ro...ru..
-00012cb0: 0072 7f01 0000 729e 0100 0072 a301 0000  .r....r....r....
-00012cc0: 72a0 0100 0072 b101 0000 72b3 0100 0072  r....r....r....r
-00012cd0: 9901 0000 7263 0000 0072 5e00 0000 72bf  ....rc...r^...r.
-00012ce0: 0100 0072 1a00 0000 72c0 0100 0072 c501  ...r....r....r..
-00012cf0: 0000 72c6 0100 0072 a700 0000 72cc 0100  ..r....r....r...
-00012d00: 00da 066f 626a 6563 7472 d601 0000 72da  ...objectr....r.
-00012d10: 0100 0072 7401 0000 72fc 0100 0072 7001  ...rt...r....rp.
-00012d20: 0000 723b 0000 0072 2501 0000 7203 0200  ..r;...r%...r...
-00012d30: 0072 c701 0000 720d 0200 0072 1402 0000  .r....r....r....
-00012d40: 7292 0100 0072 1702 0000 7218 0200 0072  r....r....r....r
-00012d50: 1c02 0000 7225 0200 0072 2802 0000 7237  ....r%...r(...r7
-00012d60: 0000 0072 2c02 0000 7231 0200 0072 3702  ...r,...r1...r7.
-00012d70: 0000 723b 0200 0072 4202 0000 7245 0200  ..r;...rB...rE..
-00012d80: 0072 4802 0000 7298 0100 0072 4b02 0000  .rH...r....rK...
-00012d90: 724c 0200 0072 5202 0000 725f 0200 0072  rL...rR...r_...r
-00012da0: 6102 0000 7263 0200 0072 6902 0000 726a  a...rc...ri...rj
-00012db0: 0200 0072 6c02 0000 724a 0100 0072 6f02  ...rl...rJ...ro.
-00012dc0: 0000 7271 0200 0072 7302 0000 7257 0000  ..rq...rs...rW..
-00012dd0: 0072 7a02 0000 727e 0200 0072 8002 0000  .rz...r~...r....
-00012de0: 7287 0200 0072 8b02 0000 728d 0200 0072  r....r....r....r
-00012df0: 8f02 0000 7295 0100 0072 9702 0000 7299  ....r....r....r.
-00012e00: 0200 0072 7101 0000 7269 0100 0072 4801  ...rq...ri...rH.
-00012e10: 0000 721e 0100 0072 9f02 0000 72a2 0200  ..r....r....r...
-00012e20: 0072 a502 0000 7216 0000 0072 1600 0000  .r....r....r....
-00012e30: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
-00012e40: 756c 653e 0100 0000 734e 0100 0010 010c  ule>....sN......
-00012e50: 010c 0108 0208 0108 0108 0108 0110 010c  ................
-00012e60: 0108 010c 0108 0208 0108 010c 0108 0108  ................
-00012e70: 0108 0110 0108 010c 0210 0108 0108 0108  ................
-00012e80: 020c 0108 010c 1808 040c 1208 1714 2408  ..............$.
-00012e90: 090c 0a08 0d08 090c 160c 160c 160c 1d00  ................
-00012ea0: 0100 0000 0002 ff0a 6508 2508 0608 050c  ........e.%.....
-00012eb0: 5308 0408 0908 090c 4f08 2d08 5408 0408  S.......O.-.T...
-00012ec0: 0708 040c 0d08 1d0c 0f0c 0c0c 1a0c 370c  ..............7.
-00012ed0: 2e08 0508 050c 0b14 160c 0808 0408 0508  ................
-00012ee0: 0808 0b00 0100 0002 ff0a 1708 190c 0800  ................
-00012ef0: 0100 0000 0100 0000 0102 fd0a 7f00 7f00  ................
-00012f00: 220c 180c 7c0c 2c08 0608 0608 0508 0508  "...|.,.........
-00012f10: 0708 0a0c 1508 1608 080c 090c 0c12 4708  ..............G.
-00012f20: 290c 480c 3e0c 5b0c 2a0c 1508 1708 0f08  ).H.>.[.*.......
-00012f30: 1208 1b08 130c 2a08 1908 1308 160c 1008  ......*.........
-00012f40: 140c 310c 1d0c 4508 2f0c 1e0c 1d08 1608  ..1...E./.......
-00012f50: 0f08 2808 0908 1208 1f08 3308 3608 040c  ..(.......3.6...
-00012f60: 1408 0b00 0102 ff0a 180c 0d08 0708 2708  ..............'.
-00012f70: 0f0c 170c 0b14 0f08 0a08 0a08 080c 090c  ................
-00012f80: 0808 0a00 0100 0000 0002 ff0e 3a10 180c  ............:...
-00012f90: 0d0c 040c 0610 090c 040c 05              ...........
+00000190: 6416 641c 641d 8401 5a34 641e 641f 8400  d.d.d...Z4d.d...
+000001a0: 5a35 6420 6421 8400 5a36 9001 6417 6422  Z5d d!..Z6..d.d"
+000001b0: 6423 8401 5a37 9001 6418 6424 6425 8401  d#..Z7..d.d$d%..
+000001c0: 5a38 9001 6419 6426 6427 8401 5a39 9001  Z8..d.d&d'..Z9..
+000001d0: 641a 6428 6429 8401 5a3a 9001 641b 642b  d.d(d)..Z:..d.d+
+000001e0: 642c 8401 5a3b 9001 641c 642d 642e 8401  d,..Z;..d.d-d...
+000001f0: 5a3c 642f 6430 8400 5a3d 6431 6432 8400  Z<d/d0..Z=d1d2..
+00000200: 5a3e 6433 6434 8400 5a3f 9001 641d 6435  Z>d3d4..Z?..d.d5
+00000210: 6436 8401 5a40 6437 6438 8400 5a41 6439  d6..Z@d7d8..ZAd9
+00000220: 643a 8400 5a42 643b 643c 8400 5a43 9001  d:..ZBd;d<..ZC..
+00000230: 641e 643d 643e 8401 5a44 643f 6440 8400  d.d=d>..ZDd?d@..
+00000240: 5a45 6441 6442 8400 5a46 6443 6444 8400  ZEdAdB..ZFdCdD..
+00000250: 5a47 6445 6446 8400 5a48 6447 6448 8400  ZGdEdF..ZHdGdH..
+00000260: 5a49 9001 641f 6449 644a 8401 5a4a 644b  ZI..d.dIdJ..ZJdK
+00000270: 644c 8400 5a4b 9001 6420 6450 6451 8401  dL..ZK..d dPdQ..
+00000280: 5a4c 9001 6421 6453 6454 8401 5a4d 9001  ZL..d!dSdT..ZM..
+00000290: 6422 6455 6456 8401 5a4e 9001 6423 6458  d"dUdV..ZN..d#dX
+000002a0: 6459 8401 5a4f 9001 6424 645b 645c 8401  dY..ZO..d$d[d\..
+000002b0: 5a50 645d 645e 8400 5a51 645f 6460 8400  ZPd]d^..ZQd_d`..
+000002c0: 5a52 9001 6425 6461 6462 8401 5a53 6463  ZR..d%dadb..ZSdc
+000002d0: 645a 6464 6465 6704 6601 6466 6467 8401  dZdddeg.f.dfdg..
+000002e0: 5a54 9001 6426 6469 646a 8401 5a55 646b  ZT..d&didj..ZUdk
+000002f0: 646c 8400 5a56 646d 646e 8400 5a57 646f  dl..ZVdmdn..ZWdo
+00000300: 6470 8400 5a58 6471 6472 8400 5a59 9001  dp..ZXdqdr..ZY..
+00000310: 6427 6475 6476 8401 5a5a 6477 6478 8400  d'dudv..ZZdwdx..
+00000320: 5a5b 9001 6428 647a 647b 8401 5a5c 9001  Z[..d(dzd{..Z\..
+00000330: 6429 647c 647d 8401 5a5d 9001 642a 647e  d)d|d}..Z]..d*d~
+00000340: 647f 8401 5a5e 9001 642b 6480 6481 8401  d...Z^..d+d.d...
+00000350: 5a5f 9001 642c 6482 6483 8401 5a60 6484  Z_..d,d.d...Z`d.
+00000360: 6485 8400 5a61 6486 6487 8400 5a62 6488  d...Zad.d...Zbd.
+00000370: 6489 8400 5a63 648a 648b 8400 5a64 648c  d...Zcd.d...Zdd.
+00000380: 648d 8400 5a65 648e 648f 8400 5a66 9001  d...Zed.d...Zf..
+00000390: 642d 6491 6492 8401 5a67 6493 6494 8400  d-d.d...Zgd.d...
+000003a0: 5a68 6495 6496 8400 5a69 9001 642e 6497  Zhd.d...Zi..d.d.
+000003b0: 6498 8401 5a6a 9001 642f 6499 649a 8401  d...Zj..d/d.d...
+000003c0: 5a6b 9001 6430 656c 649b 9c01 649c 649d  Zk..d0eld...d.d.
+000003d0: 8405 5a6d 649e 649f 8400 5a6e 9001 6431  ..Zmd.d...Zn..d1
+000003e0: 64a1 64a2 8401 5a6f 9001 6432 64a3 64a4  d.d...Zo..d2d.d.
+000003f0: 8401 5a70 9001 6433 64a5 64a6 8401 5a71  ..Zp..d3d.d...Zq
+00000400: 9001 6434 64a7 64a8 8401 5a72 9001 6435  ..d4d.d...Zr..d5
+00000410: 64a9 64aa 8401 5a73 64ab 64ac 8400 5a74  d.d...Zsd.d...Zt
+00000420: 64ad 64ae 8400 5a75 64af 64b0 8400 5a76  d.d...Zud.d...Zv
+00000430: 64b1 64b2 8400 5a77 64b3 64b0 8400 5a76  d.d...Zwd.d...Zv
+00000440: 9001 6436 64b4 64b5 8401 5a78 64b6 64b7  ..d6d.d...Zxd.d.
+00000450: 8400 5a79 64b8 64b9 8400 5a7a 64ba 64bb  ..Zyd.d...Zzd.d.
+00000460: 8400 5a7b 9001 6437 64bc 64bd 8401 5a7c  ..Z{..d7d.d...Z|
+00000470: 64be 64bf 8400 5a7d 9001 6438 64c0 64c1  d.d...Z}..d8d.d.
+00000480: 8401 5a7e 9001 6439 64c2 64c3 8401 5a7f  ..Z~..d9d.d...Z.
+00000490: 9001 643a 64c5 64c6 8401 5a80 64c7 64c8  ..d:d.d...Z.d.d.
+000004a0: 8400 5a81 9001 643b 64c9 64ca 8401 5a82  ..Z...d;d.d...Z.
+000004b0: 9001 643c 64cb 64cc 8401 5a83 64cd 64ce  ..d<d.d...Z.d.d.
+000004c0: 8400 5a84 64cf 64d0 8400 5a85 64d1 64d2  ..Z.d.d...Z.d.d.
+000004d0: 8400 5a86 64d3 64d4 8400 5a87 64d5 64d6  ..Z.d.d...Z.d.d.
+000004e0: 8400 5a88 64d7 64d8 8400 5a89 64d9 64da  ..Z.d.d...Z.d.d.
+000004f0: 8400 5a8a 64db 64dc 8400 5a8b 64dd 64de  ..Z.d.d...Z.d.d.
+00000500: 8400 5a8c 9001 643d 64e0 64e1 8401 5a8d  ..Z...d=d.d...Z.
+00000510: 64e2 64e3 8400 5a8e 9001 643e 64e4 64e5  d.d...Z...d>d.d.
+00000520: 8401 5a8f 9001 643f 64e6 64e7 8401 5a90  ..Z...d?d.d...Z.
+00000530: 64e8 64e9 8400 5a91 64ea 64eb 8400 5a92  d.d...Z.d.d...Z.
+00000540: 64ec 64ed 8400 5a93 9001 6440 64ee 64ef  d.d...Z...d@d.d.
+00000550: 8401 5a94 9001 6441 64f1 64f2 8401 5a95  ..Z...dAd.d...Z.
+00000560: 6414 6414 6416 6457 6704 6601 64f3 64f4  d.d.d.dWg.f.d.d.
+00000570: 8401 5a96 64f5 64f6 8400 5a97 64f7 64f8  ..Z.d.d...Z.d.d.
+00000580: 8400 5a98 64f9 64fa 8400 5a99 9001 6442  ..Z.d.d...Z...dB
+00000590: 64fc 64fd 8401 5a9a 9001 6443 64fe 64ff  d.d...Z...dCd.d.
+000005a0: 8401 5a9b 9001 6400 9001 6401 8400 5a9c  ..Z...d...d...Z.
+000005b0: 9001 6444 9001 6402 9001 6403 8401 5a9d  ..dD..d...d...Z.
+000005c0: 9001 6445 9001 6405 9001 6406 8401 5a9e  ..dE..d...d...Z.
+000005d0: 9001 6407 9001 6408 8400 5a9f 9001 6409  ..d...d...Z...d.
+000005e0: 9001 640a 8400 5aa0 9001 640b 9001 640c  ..d...Z...d...d.
+000005f0: 8400 5aa1 9001 6446 9001 640d 9001 640e  ..Z...dF..d...d.
+00000600: 8401 5aa2 9001 640f 9001 6410 8400 5aa3  ..Z...d...d...Z.
+00000610: 9001 6411 9001 6412 8400 5aa4 9001 6447  ..d...d...Z...dG
+00000620: 9001 6413 9001 6414 8401 5aa5 6404 5300  ..d...d...Z.d.S.
+00000630: 2848 0100 00e9 0000 0000 2902 da18 636f  (H........)...co
+00000640: 6e76 6572 745f 6835 5f74 6f5f 6665 6174  nvert_h5_to_feat
+00000650: 7572 655f 6835 da1c 7374 616e 6461 7264  ure_h5..standard
+00000660: 5f66 6561 7475 7265 5f67 656e 6572 6174  _feature_generat
+00000670: 696f 6e32 2901 da0c 506f 6c65 5472 6163  ion2)...PoleTrac
+00000680: 6b69 6e67 2901 da0b 6d6f 6465 6c5f 6d61  king)...model_ma
+00000690: 6b65 724e 2902 da09 6e61 7473 6f72 7465  kerN)...natsorte
+000006a0: 64da 026e 7329 01da 0b69 6d61 6765 5f74  d..ns)...image_t
+000006b0: 6f6f 6c73 2902 da07 6d65 6466 696c 74da  ools)...medfilt.
+000006c0: 096d 6564 6669 6c74 3264 2901 da04 7471  .medfilt2d)...tq
+000006d0: 646d 2902 da09 7469 6d65 6465 6c74 61da  dm)...timedelta.
+000006e0: 0864 6174 6574 696d 6529 01da 0450 6174  .datetime)...Pat
+000006f0: 6829 01da 075a 6970 4669 6c65 6302 0000  h)...ZipFilec...
+00000700: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000710: 0043 0000 0073 2400 0000 7400 6a01 7c00  .C...s$...t.j.|.
+00000720: 6a02 7c01 6401 8d02 0100 7400 6a01 7c00  j.|.d.....t.j.|.
+00000730: 6a03 7c01 6401 8d02 0100 6400 5300 2902  j.|.d.....d.S.).
+00000740: 4e29 01da 067a 6f72 6465 7229 04da 0370  N)...zorder)...p
+00000750: 6c74 da04 7365 7470 da05 6c69 6e65 73da  lt..setp..lines.
+00000760: 0b63 6f6c 6c65 6374 696f 6e73 2902 da02  .collections)...
+00000770: 6178 7210 0000 00a9 0072 1600 0000 fa39  axr......r.....9
+00000780: 2f55 7365 7273 2f70 6869 6c2f 4472 6f70  /Users/phil/Drop
+00000790: 626f 782f 4849 5245 535f 4c41 422f 4769  box/HIRES_LAB/Gi
+000007a0: 7448 7562 2f77 6861 6363 2f77 6861 6363  tHub/whacc/whacc
+000007b0: 2f75 7469 6c73 2e70 7972 1000 0000 3900  /utils.pyr....9.
+000007c0: 0000 7304 0000 0000 0110 0172 1000 0000  ..s........r....
+000007d0: e92a 0000 0063 0400 0000 0000 0000 0000  .*...c..........
+000007e0: 0000 0b00 0000 0600 0000 4300 0000 73d4  ..........C...s.
+000007f0: 0000 0074 0083 007d 0467 007d 0574 017c  ...t...}.g.}.t.|
+00000800: 0083 0144 005d 507d 0674 02a0 037c 06a1  ...D.]P}.t...|..
+00000810: 017d 0674 046a 05a0 067c 03a1 0101 0074  .}.t.j...|.....t
+00000820: 046a 05a0 077c 046a 0864 0119 007c 066a  .j...|.j.d...|.j
+00000830: 0864 0119 00a1 027d 077c 047c 0719 007d  .d.....}.|.|...}
+00000840: 0874 046a 097c 067c 083c 007c 05a0 0a7c  .t.j.|.|.<.|...|
+00000850: 06a1 0101 0071 127e 0674 0b74 017c 0583  .....q.~.t.t.|..
+00000860: 0183 0144 005d 565c 027d 097d 0a74 04a0  ...D.]V\.}.}.t..
+00000870: 0c7c 007c 0919 007c 057c 0919 0067 02a1  .|.|...|.|...g..
+00000880: 017c 007c 093c 0074 04a0 0d7c 017c 0919  .|.|.<.t...|.|..
+00000890: 007c 017c 0919 0067 02a1 017c 017c 093c  .|.|...g...|.|.<
+000008a0: 0074 04a0 0d7c 027c 0919 007c 027c 0919  .t...|.|...|.|..
+000008b0: 0067 02a1 017c 027c 093c 0071 727c 007c  .g...|.|.<.qr|.|
+000008c0: 017c 0266 0353 00a9 024e 7201 0000 0029  .|.f.S...Nr....)
+000008d0: 0eda 156c 6f61 645f 6e61 6e5f 626f 7264  ...load_nan_bord
+000008e0: 6572 5f69 6e64 6578 720b 0000 00da 0463  er_indexr......c
+000008f0: 6f70 79da 0864 6565 7063 6f70 79da 026e  opy..deepcopy..n
+00000900: 70da 0672 616e 646f 6dda 0473 6565 64da  p..random..seed.
+00000910: 0663 686f 6963 65da 0573 6861 7065 da03  .choice..shape..
+00000920: 6e61 6eda 0661 7070 656e 64da 0965 6e75  nan..append..enu
+00000930: 6d65 7261 7465 da06 7673 7461 636b da0b  merate..vstack..
+00000940: 636f 6e63 6174 656e 6174 6529 0bda 0574  concatenate)...t
+00000950: 7674 5f78 da05 7476 745f 79da 0674 7674  vt_x..tvt_y..tvt
+00000960: 5f66 6e5a 0a6e 756d 7079 5f73 6565 645a  _fnZ.numpy_seedZ
+00000970: 156e 616e 5f61 7272 6179 5f62 6f72 6465  .nan_array_borde
+00000980: 725f 696e 6473 5a0b 7476 745f 785f 6e61  r_indsZ.tvt_x_na
+00000990: 6e65 64da 0464 6174 61da 0469 6e64 735a  ned..data..indsZ
+000009a0: 1172 6570 6c61 6365 5f77 6974 685f 6e61  .replace_with_na
+000009b0: 6e73 da01 695a 086e 616e 5f64 6174 6172  ns..iZ.nan_datar
+000009c0: 1600 0000 7216 0000 0072 1700 0000 da0b  ....r....r......
+000009d0: 4e41 4e69 6679 5f64 6174 613d 0000 0073  NANify_data=...s
+000009e0: 1e00 0000 0001 0601 0401 0c01 0a01 0c01  ................
+000009f0: 1a01 0801 0a01 0c01 0202 1401 1a01 1a01  ................
+00000a00: 1c01 722d 0000 0063 0200 0000 0000 0000  ..r-...c........
+00000a10: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
+00000a20: 73d0 0000 0074 00a0 017c 00a1 017d 0264  s....t...|...}.d
+00000a30: 017c 017c 021a 0017 007d 0374 00a0 027c  .|.|.....}.t...|
+00000a40: 02a1 017d 0474 0374 047c 0083 0183 0144  ...}.t.t.|.....D
+00000a50: 005d 185c 027d 055c 027d 067d 077c 057c  .].\.}.\.}.}.|.|
+00000a60: 047c 067c 0785 023c 0071 2c74 00a0 0574  .|.|...<.q,t...t
+00000a70: 067c 0483 017c 0314 00a1 017d 047c 0464  .|...|.....}.|.d
+00000a80: 007c 0185 0219 007d 0467 007d 0874 0774  .|.....}.g.}.t.t
+00000a90: 087c 0083 0183 0144 005d 187d 097c 08a0  .|.....D.].}.|..
+00000aa0: 0974 00a0 057c 097c 046b 02a1 01a1 0101  .t...|.|.k......
+00000ab0: 0071 7474 00a0 057c 08a1 017d 0867 007d  .qtt...|...}.g.}
+00000ac0: 0a7c 0844 005d 267d 0b74 0a7c 0b64 0283  .|.D.]&}.t.|.d..
+00000ad0: 0264 0219 007d 0c7c 0aa0 0964 0364 0484  .d...}.|...d.d..
+00000ae0: 007c 0c44 0083 01a1 0101 0071 a07c 087c  .|.D.......q.|.|
+00000af0: 0a66 0253 0029 054e e901 0000 0072 0100  .f.S.).N.....r..
+00000b00: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000b10: 0000 0005 0000 0053 0000 0073 1e00 0000  .......S...s....
+00000b20: 6700 7c00 5d16 7d01 7400 a001 7c01 a101  g.|.].}.t...|...
+00000b30: 7204 7402 7c01 8301 9102 7104 5300 7216  r.t.|.....q.S.r.
+00000b40: 0000 0029 0372 1d00 0000 da03 616c 6cda  ...).r......all.
+00000b50: 036c 656e a902 da02 2e30 da01 6b72 1600  .len.....0..kr..
+00000b60: 0000 7216 0000 0072 1700 0000 da0a 3c6c  ..r....r......<l
+00000b70: 6973 7463 6f6d 703e 6100 0000 7306 0000  istcomp>a...s...
+00000b80: 0006 0002 000a 007a 2171 7569 636b 5f73  .......z!quick_s
+00000b90: 706c 6974 6572 2e3c 6c6f 6361 6c73 3e2e  pliter.<locals>.
+00000ba0: 3c6c 6973 7463 6f6d 703e 290b 721d 0000  <listcomp>).r...
+00000bb0: 00da 0373 756d da04 6f6e 6573 7224 0000  ...sum..onesr$..
+00000bc0: 00da 0d6c 6f6f 705f 7365 676d 656e 7473  ...loop_segments
+00000bd0: da07 6173 6172 7261 79da 046c 6973 74da  ..asarray..list.
+00000be0: 0572 616e 6765 7230 0000 0072 2300 0000  .ranger0...r#...
+00000bf0: da12 6772 6f75 705f 636f 6e73 6563 7574  ..group_consecut
+00000c00: 6976 6573 290d 5a0a 7370 6c69 745f 6e75  ives).Z.split_nu
+00000c10: 6d73 da09 6c65 6e5f 6172 7261 795a 066c  ms..len_arrayZ.l
+00000c20: 5f6e 756d 73da 0563 6f75 6e74 722b 0000  _nums..countr+..
+00000c30: 00da 0269 69da 0269 31da 0269 325a 1062  ...ii..i1..i2Z.b
+00000c40: 6f6f 6c5f 696e 6473 5f61 7272 6179 7372  ool_inds_arraysr
+00000c50: 3300 0000 da0a 6672 616d 655f 6e75 6d73  3.....frame_nums
+00000c60: da01 62da 0262 3272 1600 0000 7216 0000  ..b..b2r....r...
+00000c70: 0072 1700 0000 da0d 7175 6963 6b5f 7370  .r......quick_sp
+00000c80: 6c69 7465 724f 0000 0073 2000 0000 0001  literO...s .....
+00000c90: 0a01 0c02 0a01 1801 0e01 1201 0c02 0401  ................
+00000ca0: 1001 1601 0a02 0401 0801 0e01 1602 7244  ..............rD
+00000cb0: 0000 00e9 0700 0000 e903 0000 0054 e902  .............T..
+00000cc0: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
+00000cd0: 1400 0000 0600 0000 4300 0000 739c 0100  ........C...s...
+00000ce0: 0074 0064 0183 0101 0074 0183 005c 037d  .t.d.....t...\.}
+00000cf0: 057d 067d 0764 0264 0384 007c 0644 0083  .}.}.d.d...|.D..
+00000d00: 017d 0874 0064 0483 0101 0074 027c 0083  .}.t.d.....t.|..
+00000d10: 0144 005d fc7d 0974 037c 0964 0583 027d  .D.].}.t.|.d...}
+00000d20: 0a74 037c 097c 0183 027d 0b74 047c 0274  .t.|.|...}.t.|.t
+00000d30: 057c 0b83 0183 025c 027d 0c7d 0d74 06a0  .|.....\.}.}.t..
+00000d40: 077c 0b64 066b 02a1 0164 076b 0472 8a74  .|.d.k...d.k.r.t
+00000d50: 007c 0964 0817 0083 0101 0064 0973 8a74  .|.d.......d.s.t
+00000d60: 087c 0964 0817 0083 0182 017c 0c5c 027d  .|.d.......|.\.}
+00000d70: 0e7d 0f74 06a0 097c 0564 0719 007c 0a7c  .}.t...|.d...|.|
+00000d80: 0e19 0066 02a1 017c 0564 073c 0074 06a0  ...f...|.d.<.t..
+00000d90: 0a7c 0664 0719 007c 0b7c 0e19 0066 02a1  .|.d...|.|...f..
+00000da0: 017c 0664 073c 0074 06a0 0a7c 0764 0719  .|.d.<.t...|.d..
+00000db0: 007c 0d64 0719 0066 02a1 017c 0764 073c  .|.d...f...|.d.<
+00000dc0: 0074 06a0 097c 0564 0a19 007c 0a7c 0f19  .t...|.d...|.|..
+00000dd0: 0066 02a1 017c 0564 0a3c 0074 06a0 0a7c  .f...|.d.<.t...|
+00000de0: 0664 0a19 007c 0b7c 0f19 0066 02a1 017c  .d...|.|...f...|
+00000df0: 0664 0a3c 0074 06a0 0a7c 0764 0a19 007c  .d.<.t...|.d...|
+00000e00: 0d64 0a19 0066 02a1 017c 0764 0a3c 0071  .d...f...|.d.<.q
+00000e10: 327c 0390 0172 5074 0064 0b83 0101 0074  2|...rPt.d.....t
+00000e20: 0b7c 057c 067c 0783 035c 037d 057d 067d  .|.|.|...\.}.}.}
+00000e30: 0767 007d 1074 0c7c 0683 0144 005d 325c  .g.}.t.|...D.]2\
+00000e40: 027d 117d 1274 06a0 0d7c 12a1 017c 0414  .}.}.t...|...|..
+00000e50: 007d 1364 0a7c 1364 007c 087c 1119 0085  .}.d.|.d.|.|....
+00000e60: 023c 007c 10a0 0e7c 13a1 0101 0090 0171  .<.|...|.......q
+00000e70: 5c7c 057c 067c 077c 1066 0453 0029 0c4e  \|.|.|.|.f.S.).N
+00000e80: 7a21 6c6f 6164 696e 6720 6f72 6967 696e  z!loading origin
+00000e90: 616c 2074 7261 696e 696e 6720 6461 7461  al training data
+00000ea0: 2e2e 2e63 0100 0000 0000 0000 0000 0000  ...c............
+00000eb0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+00000ec0: 0067 007c 005d 0c7d 0174 007c 0183 0191  .g.|.].}.t.|....
+00000ed0: 0271 0453 0072 1600 0000 a901 7230 0000  .q.S.r......r0..
+00000ee0: 0072 3100 0000 7216 0000 0072 1600 0000  .r1...r....r....
+00000ef0: 7217 0000 0072 3400 0000 6900 0000 7304  r....r4...i...s.
+00000f00: 0000 0006 0002 007a 326c 6f61 645f 7472  .......z2load_tr
+00000f10: 6169 6e69 6e67 5f61 6e64 5f63 7572 6174  aining_and_curat
+00000f20: 6564 5f64 6174 612e 3c6c 6f63 616c 733e  ed_data.<locals>
+00000f30: 2e3c 6c69 7374 636f 6d70 3e7a 1c6c 6f61  .<listcomp>z.loa
+00000f40: 6469 6e67 2079 6f75 7220 6375 7261 7465  ding your curate
+00000f50: 6420 6461 7461 2e2e 2eda 1366 696e 616c  d data.....final
+00000f60: 5f66 6561 7475 7265 735f 3231 3035 e9ff  _features_2105..
+00000f70: ffff ff72 0100 0000 7a24 2074 6869 7320  ...r....z$ this 
+00000f80: 6669 6c65 2068 6173 202d 3127 7320 696e  file has -1's in
+00000f90: 2069 7473 206c 6162 656c 732e 2e2e 4672   its labels...Fr
+00000fa0: 2e00 0000 7a45 4e41 4e69 6679 696e 6720  ....zENANifying 
+00000fb0: 6461 7461 2074 6869 7320 6973 206d 656d  data this is mem
+00000fc0: 6f72 7920 696e 7465 6e73 6976 6520 616e  ory intensive an
+00000fd0: 6420 6d61 7920 7461 6b65 2075 7020 746f  d may take up to
+00000fe0: 2031 2d32 206d 696e 2e2e 2e29 0fda 0570   1-2 min...)...p
+00000ff0: 7269 6e74 da12 6c6f 6164 5f74 7261 696e  rint..load_train
+00001000: 696e 675f 6461 7461 720b 0000 00da 0667  ing_datar......g
+00001010: 6574 6b65 7972 4400 0000 7230 0000 0072  etkeyrD...r0...r
+00001020: 1d00 0000 7235 0000 00da 0e41 7373 6572  ....r5.....Asser
+00001030: 7469 6f6e 4572 726f 7272 2500 0000 7226  tionErrorr%...r&
+00001040: 0000 0072 2d00 0000 7224 0000 00da 096f  ...r-...r$.....o
+00001050: 6e65 735f 6c69 6b65 7223 0000 0029 14da  nes_liker#...)..
+00001060: 0768 355f 6c69 7374 5a0a 6c61 6265 6c73  .h5_listZ.labels
+00001070: 5f6b 6579 5a0f 7472 6169 6e5f 7661 6c5f  _keyZ.train_val_
+00001080: 7370 6c69 745a 0c6e 616e 5f69 6679 5f64  splitZ.nan_ify_d
+00001090: 6174 615a 0f6e 6577 5f64 6174 615f 7765  ataZ.new_data_we
+000010a0: 6967 6874 7227 0000 0072 2800 0000 7229  ightr'...r(...r)
+000010b0: 0000 005a 076f 675f 6c65 6e73 da02 6835  ...Z.og_lens..h5
+000010c0: 722a 0000 00da 066c 6162 656c 735a 0962  r*.....labelsZ.b
+000010d0: 6f6f 6c5f 696e 6473 7241 0000 0072 3f00  ool_indsrA...r?.
+000010e0: 0000 7240 0000 005a 0574 7674 5f77 722c  ..r@...Z.tvt_wr,
+000010f0: 0000 0072 3300 0000 da01 7872 1600 0000  ...r3.....xr....
+00001100: 7216 0000 0072 1700 0000 da1e 6c6f 6164  r....r......load
+00001110: 5f74 7261 696e 696e 675f 616e 645f 6375  _training_and_cu
+00001120: 7261 7465 645f 6461 7461 6600 0000 7336  rated_dataf...s6
+00001130: 0000 0000 0108 010c 010e 0308 010c 010a  ................
+00001140: 010a 0112 0212 010c 0110 0208 011a 011a  ................
+00001150: 011a 021a 011a 011c 0106 0108 0112 0204  ................
+00001160: 0110 010e 0110 010e 0272 5400 0000 6302  .........rT...c.
+00001170: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001180: 0000 0043 0000 0073 3a00 0000 7400 7c00  ...C...s:...t.|.
+00001190: 6401 6402 8d02 7d00 7401 7c00 8301 6403  d.d...}.t.|...d.
+000011a0: 6b02 7222 7c00 7c01 1400 7d00 6e14 7401  k.r"|.|...}.n.t.
+000011b0: 7c00 8301 7c01 6b02 7336 7402 6404 8301  |...|.k.s6t.d...
+000011c0: 8201 7c00 5300 2905 4e54 a901 da10 7375  ..|.S.).NT....su
+000011d0: 7070 7265 7373 5f77 6172 6e69 6e67 722e  ppress_warningr.
+000011e0: 0000 007a 5527 5f73 696e 676c 655f 746f  ...zU'_single_to
+000011f0: 5f6c 6973 745f 696e 7075 745f 6368 6563  _list_input_chec
+00001200: 6b65 7227 206c 656e 6774 6820 6f66 2069  ker' length of i
+00001210: 6e70 7574 206c 6973 7420 616e 6420 7468  nput list and th
+00001220: 6520 7365 7420 7271 7569 726d 656e 7420  e set rquirment 
+00001230: 646f 6e74 206d 6174 6368 2903 da09 6d61  dont match)...ma
+00001240: 6b65 5f6c 6973 7472 3000 0000 724e 0000  ke_listr0...rN..
+00001250: 0029 025a 0369 6e5f 5a08 6c65 6e5f 6c69  .).Z.in_Z.len_li
+00001260: 7374 7216 0000 0072 1600 0000 7217 0000  str....r....r...
+00001270: 00da 1d5f 7369 6e67 6c65 5f74 6f5f 6c69  ..._single_to_li
+00001280: 7374 5f69 6e70 7574 5f63 6865 636b 6572  st_input_checker
+00001290: 8a00 0000 730a 0000 0000 010c 020c 010a  ....s...........
+000012a0: 0214 0172 5800 0000 4663 0200 0000 0000  ...rX...Fc......
+000012b0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000012c0: 0000 734e 0000 0074 007c 0064 0183 027d  ..sN...t.|.d...}
+000012d0: 0074 007c 0164 0183 027d 0174 017c 0064  .t.|.d...}.t.|.d
+000012e0: 0219 007c 0164 0219 0083 0201 0074 027c  ...|.d.......t.|
+000012f0: 0064 0319 007c 0164 0319 0083 0201 0074  .d...|.d.......t
+00001300: 037c 0064 0419 007c 0164 0419 0083 0201  .|.d...|.d......
+00001310: 0064 0053 0029 054e 7246 0000 0072 0100  .d.S.).NrF...r..
+00001320: 0000 722e 0000 0072 4700 0000 2904 7258  ..r....rG...).rX
+00001330: 0000 00da 1564 6f77 6e6c 6f61 645f 7265  .....download_re
+00001340: 736e 6574 5f6d 6f64 656c da16 646f 776e  snet_model..down
+00001350: 6c6f 6164 5f74 7261 696e 696e 675f 6461  load_training_da
+00001360: 7461 da1a 646f 776e 6c6f 6164 5f65 7874  ta..download_ext
+00001370: 7261 5f4c 4742 4d5f 6d6f 6465 6c73 2902  ra_LGBM_models).
+00001380: da09 6f76 6572 7772 6974 655a 0d64 6f77  ..overwriteZ.dow
+00001390: 6e6c 6f61 645f 696e 6473 7216 0000 0072  nload_indsr....r
+000013a0: 1600 0000 7217 0000 00da 1764 6f77 6e6c  ....r......downl
+000013b0: 6f61 645f 616c 6c5f 7768 6163 635f 6461  oad_all_whacc_da
+000013c0: 7461 9300 0000 730a 0000 0000 020a 010a  ta....s.........
+000013d0: 0212 0112 0172 5d00 0000 6300 0000 0000  .....r]...c.....
+000013e0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+000013f0: 0000 0073 6a00 0000 7400 8300 7401 6a02  ...sj...t...t.j.
+00001400: 1700 6401 1700 7d00 7401 6a03 a004 7c00  ..d...}.t.j...|.
+00001410: a101 732a 7405 6402 8301 0100 7406 8300  ..s*t.d.....t...
+00001420: 0100 7407 7c00 7401 6a02 1700 6403 1700  ..t.|.t.j...d...
+00001430: 8301 7d01 7407 7c00 7401 6a02 1700 6404  ..}.t.|.t.j...d.
+00001440: 1700 8301 7d02 7407 7c00 7401 6a02 1700  ....}.t.|.t.j...
+00001450: 6405 1700 8301 7d03 7c01 7c02 7c03 6603  d.....}.|.|.|.f.
+00001460: 5300 2906 4e7a 192f 7768 6163 635f 6461  S.).Nz./whacc_da
+00001470: 7461 2f74 7261 696e 696e 675f 6461 7461  ta/training_data
+00001480: 7a37 4175 746f 2064 6f77 6e6c 6f61 6469  z7Auto downloadi
+00001490: 6e67 2074 7261 696e 696e 6720 6461 7461  ng training data
+000014a0: 2c20 7468 6973 2077 696c 6c20 6f6e 6c79  , this will only
+000014b0: 2072 756e 206f 6e63 657a 0974 7674 5f78   run oncez.tvt_x
+000014c0: 2e70 6b6c 7a09 7476 745f 792e 706b 6c7a  .pklz.tvt_y.pklz
+000014d0: 0a74 7674 5f66 6e2e 706b 6c29 08da 0e67  .tvt_fn.pkl)...g
+000014e0: 6574 5f77 6861 6363 5f70 6174 68da 026f  et_whacc_path..o
+000014f0: 73da 0373 6570 da04 7061 7468 da05 6973  s..sep..path..is
+00001500: 6469 7272 4b00 0000 725a 0000 00da 086c  dirrK...rZ.....l
+00001510: 6f61 645f 6f62 6a29 04da 0262 6472 2700  oad_obj)...bdr'.
+00001520: 0000 7228 0000 0072 2900 0000 7216 0000  ..r(...r)...r...
+00001530: 0072 1600 0000 7217 0000 0072 4c00 0000  .r....r....rL...
+00001540: 9e00 0000 7310 0000 0000 0110 010c 0108  ....s...........
+00001550: 0106 0212 0112 0112 0272 4c00 0000 6300  .........rL...c.
+00001560: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001570: 0000 0043 0000 0073 3400 0000 7400 8300  ...C...s4...t...
+00001580: 7d00 6401 6402 6702 7c00 6403 3c00 6404  }.d.d.g.|.d.<.d.
+00001590: 6701 7c00 6405 3c00 6406 6701 7c00 6407  g.|.d.<.d.g.|.d.
+000015a0: 3c00 6408 6701 7c00 6409 3c00 7c00 5300  <.d.g.|.d.<.|.S.
+000015b0: 290a 4e7a 4968 7474 7073 3a2f 2f77 7777  ).NzIhttps://www
+000015c0: 2e64 726f 7062 6f78 2e63 6f6d 2f73 682f  .dropbox.com/sh/
+000015d0: 6b6e 7136 6c61 3566 6375 3733 7a6b 352f  knq6la5fcu73zk5/
+000015e0: 4141 4251 754d 6d78 6d34 6d73 5662 5749  AABQuMmxm4msVbWI
+000015f0: 6464 6c39 7831 7633 613f 646c 3d31 7a4e  ddl9x1v3a?dl=1zN
+00001600: 6874 7470 733a 2f2f 7777 772e 6472 6f70  https://www.drop
+00001610: 626f 782e 636f 6d2f 732f 6b30 3339 3874  box.com/s/k0398t
+00001620: 6368 676b 3230 6c6b 762f 6669 6e61 6c5f  chgk20lkv/final_
+00001630: 7265 736e 6574 3530 5632 5f66 756c 6c5f  resnet50V2_full_
+00001640: 6d6f 6465 6c2e 7a69 703f 646c 3d31 da0c  model.zip?dl=1..
+00001650: 7265 736e 6574 5f6d 6f64 656c 7a49 6874  resnet_modelzIht
+00001660: 7470 733a 2f2f 7777 772e 6472 6f70 626f  tps://www.dropbo
+00001670: 782e 636f 6d2f 7368 2f30 3775 6176 6c6f  x.com/sh/07uavlo
+00001680: 7869 3375 676e 6a79 2f41 4141 4255 346e  xi3ugnjy/AAABU4n
+00001690: 7352 6b4a 4a34 5474 6b42 4778 6837 7a49  sRkJJ4TtkBGxh7zI
+000016a0: 4861 3f64 6c3d 31da 1873 706c 6974 5f62  Ha?dl=1..split_b
+000016b0: 795f 7472 6961 6c5f 3231 3035 5f64 6174  y_trial_2105_dat
+000016c0: 617a 4968 7474 7073 3a2f 2f77 7777 2e64  azIhttps://www.d
+000016d0: 726f 7062 6f78 2e63 6f6d 2f73 682f 6c35  ropbox.com/sh/l5
+000016e0: 7975 7733 7232 6871 6468 7277 302f 4141  yuw3r2hqdhrw0/AA
+000016f0: 4253 7132 4c39 3236 3563 577a 4173 3641  BSq2L9265cWzAs6A
+00001700: 674a 4f53 3956 613f 646c 3d31 da11 6578  gJOS9Va?dl=1..ex
+00001710: 7472 615f 4c47 424d 5f6d 6f64 656c 737a  tra_LGBM_modelsz
+00001720: 4968 7474 7073 3a2f 2f77 7777 2e64 726f  Ihttps://www.dro
+00001730: 7062 6f78 2e63 6f6d 2f73 682f 6276 3577  pbox.com/sh/bv5w
+00001740: 6563 746c 6275 6761 6365 662f 4141 4175  ectlbugacef/AAAu
+00001750: 7565 524f 6875 5f72 486d 4d5a 6a64 5667  ueROhu_rHmMZjdVg
+00001760: 476c 795f 613f 646c 3d31 da0c 6578 616d  Gly_a?dl=1..exam
+00001770: 706c 655f 4d50 3473 2901 da04 6469 6374  ple_MP4s)...dict
+00001780: a901 da01 6472 1600 0000 7216 0000 0072  ....dr....r....r
+00001790: 1700 0000 da12 646f 776e 6c6f 6164 5f64  ......download_d
+000017a0: 6174 615f 6469 6374 ab00 0000 7310 0000  ata_dict....s...
+000017b0: 0000 0106 0102 0102 ff08 020a 010a 020a  ................
+000017c0: 0272 6c00 0000 6303 0000 0000 0000 0000  .rl...c.........
+000017d0: 0000 0007 0000 0009 0000 0043 0000 0073  ...........C...s
+000017e0: a800 0000 7400 8300 7d03 7401 8300 7402  ....t...}.t...t.
+000017f0: 6a03 1700 6401 1700 7d04 7402 6a04 a005  j...d...}.t.j...
+00001800: 7c00 a101 723e 7c01 7232 7406 a007 7c00  |...r>|.r2t...|.
+00001810: a101 0100 6e0c 7408 6402 8301 0100 6400  ....n.t.d.....d.
+00001820: 5300 7408 6403 8301 0100 7c03 6404 1900  S.t.d.....|.d...
+00001830: 7c02 1900 7d05 7409 6a0a a00b 7c05 7c04  |...}.t.j...|.|.
+00001840: a102 0100 740c 7c04 6405 8302 8f1a 7d06  ....t.|.d.....}.
+00001850: 7408 6406 8301 0100 7c06 6a0d 7c00 6407  t.d.....|.j.|.d.
+00001860: 8d01 0100 5700 3500 5100 5200 5800 7408  ....W.5.Q.R.X.t.
+00001870: 6408 8301 0100 7402 a00e 7c04 a101 0100  d.....t...|.....
+00001880: 7408 6409 8301 0100 6400 5300 290a 4e7a  t.d.....d.S.).Nz
+00001890: 1c2f 7768 6163 635f 6461 7461 2f65 7861  ./whacc_data/exa
+000018a0: 6d70 6c65 5f4d 5034 732e 7a69 707a 5665  mple_MP4s.zipzVe
+000018b0: 7861 6d70 6c65 5f4d 5034 7320 6172 6520  xample_MP4s are 
+000018c0: 616c 7265 6164 7920 646f 776e 6c6f 6164  already download
+000018d0: 6564 2c20 6966 2079 6f75 2077 616e 7420  ed, if you want 
+000018e0: 746f 206f 7665 7277 7269 7465 2069 7420  to overwrite it 
+000018f0: 7365 7420 6f76 6572 7772 6974 6520 746f  set overwrite to
+00001900: 2054 7275 657a 1b64 6f77 6e6c 6f61 6469   Truez.downloadi
+00001910: 6e67 2065 7861 6d70 6c65 5f4d 5034 732e  ng example_MP4s.
+00001920: 2e2e 7268 0000 00da 0172 fa12 756e 7a69  ..rh.....r..unzi
+00001930: 7070 696e 6720 6669 6c65 202e 2e2e a901  pping file .....
+00001940: 7261 0000 00fa 1564 656c 6574 696e 6720  ra.....deleting 
+00001950: 7a69 7020 6669 6c65 202e 2e2e da04 446f  zip file .....Do
+00001960: 6e65 a90f 726c 0000 0072 5e00 0000 725f  ne..rl...r^...r_
+00001970: 0000 0072 6000 0000 7261 0000 0072 6200  ...r`...ra...rb.
+00001980: 0000 da06 7368 7574 696c da06 726d 7472  ....shutil..rmtr
+00001990: 6565 724b 0000 00da 0675 726c 6c69 62da  eerK.....urllib.
+000019a0: 0772 6571 7565 7374 da0b 7572 6c72 6574  .request..urlret
+000019b0: 7269 6576 6572 0f00 0000 da0a 6578 7472  riever......extr
+000019c0: 6163 7461 6c6c da06 7265 6d6f 7665 2907  actall..remove).
+000019d0: da03 6473 7472 5c00 0000 da08 6c69 6e6b  ..dstr\.....link
+000019e0: 5f69 6e64 726b 0000 00da 0866 696c 656e  _indrk.....filen
+000019f0: 616d 65da 0375 726c da06 7a69 704f 626a  ame..url..zipObj
+00001a00: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00001a10: 1564 6f77 6e6c 6f61 645f 6578 616d 706c  .download_exampl
+00001a20: 655f 6d70 3473 b700 0000 7320 0000 0000  e_mp4s....s ....
+00001a30: 0106 0110 010c 0104 010c 0208 0104 0208  ................
+00001a40: 010c 010e 010c 0108 0116 0108 010a 0172  ...............r
+00001a50: 7f00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001a60: 0007 0000 0009 0000 0043 0000 0073 b400  .........C...s..
+00001a70: 0000 7400 8300 7d02 7401 8300 7402 6a03  ..t...}.t...t.j.
+00001a80: 1700 6401 1700 7d03 7c03 6400 6402 8502  ..d...}.|.d.d...
+00001a90: 1900 7d04 7402 6a04 a005 7c04 a101 724a  ..}.t.j...|...rJ
+00001aa0: 7c00 723e 7406 a007 7c04 a101 0100 6e0c  |.r>t...|.....n.
+00001ab0: 7408 6403 8301 0100 6400 5300 7408 6404  t.d.....d.S.t.d.
+00001ac0: 8301 0100 7c02 6405 1900 7c01 1900 7d05  ....|.d...|...}.
+00001ad0: 7409 6a0a a00b 7c05 7c03 a102 0100 740c  t.j...|.|.....t.
+00001ae0: 7c03 6406 8302 8f1a 7d06 7408 6407 8301  |.d.....}.t.d...
+00001af0: 0100 7c06 6a0d 7c04 6408 8d01 0100 5700  ..|.j.|.d.....W.
+00001b00: 3500 5100 5200 5800 7408 6409 8301 0100  5.Q.R.X.t.d.....
+00001b10: 7402 a00e 7c03 a101 0100 7408 640a 8301  t...|.....t.d...
+00001b20: 0100 6400 5300 290b 4e7a 2d2f 7768 6163  ..d.S.).Nz-/whac
+00001b30: 635f 6461 7461 2f66 696e 616c 5f6d 6f64  c_data/final_mod
+00001b40: 656c 2f65 7874 7261 5f4c 4742 4d5f 6d6f  el/extra_LGBM_mo
+00001b50: 6465 6c73 2e7a 6970 e9fc ffff ff7a 5a65  dels.zip.....zZe
+00001b60: 7874 7261 5f4c 4742 4d5f 6d6f 6465 6c73  xtra_LGBM_models
+00001b70: 2069 7320 616c 7265 6164 7920 646f 776e   is already down
+00001b80: 6c6f 6164 6564 2c20 6966 2079 6f75 2077  loaded, if you w
+00001b90: 616e 7420 746f 206f 7665 7277 7269 7465  ant to overwrite
+00001ba0: 2069 7420 7365 7420 6f76 6572 7772 6974   it set overwrit
+00001bb0: 6520 746f 2054 7275 657a 2064 6f77 6e6c  e to Truez downl
+00001bc0: 6f61 6469 6e67 2065 7874 7261 5f4c 4742  oading extra_LGB
+00001bd0: 4d5f 6d6f 6465 6c73 2e2e 2e72 6700 0000  M_models...rg...
+00001be0: 726d 0000 0072 6e00 0000 726f 0000 0072  rm...rn...ro...r
+00001bf0: 7000 0000 7271 0000 0072 7200 0000 a907  p...rq...rr.....
+00001c00: 5a0f 6f76 6572 7772 6974 655f 6d6f 6465  Z.overwrite_mode
+00001c10: 6c72 7b00 0000 726b 0000 0072 7c00 0000  lr{...rk...r|...
+00001c20: 727a 0000 0072 7d00 0000 727e 0000 0072  rz...r}...r~...r
+00001c30: 1600 0000 7216 0000 0072 1700 0000 725b  ....r....r....r[
+00001c40: 0000 00cb 0000 0073 2200 0000 0001 0601  .......s".......
+00001c50: 1001 0c01 0c01 0401 0c02 0801 0402 0801  ................
+00001c60: 0c01 0e01 0c01 0801 1601 0801 0a01 725b  ..............r[
+00001c70: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001c80: 0700 0000 0900 0000 4300 0000 73b4 0000  ........C...s...
+00001c90: 0074 0083 007d 0274 0183 0074 026a 0317  .t...}.t...t.j..
+00001ca0: 0064 0117 007d 037c 0364 0064 0285 0219  .d...}.|.d.d....
+00001cb0: 007d 0474 026a 04a0 057c 04a1 0172 4a7c  .}.t.j...|...rJ|
+00001cc0: 0072 3e74 06a0 077c 04a1 0101 006e 0c74  .r>t...|.....n.t
+00001cd0: 0864 0383 0101 0064 0053 0074 0864 0483  .d.....d.S.t.d..
+00001ce0: 0101 007c 0264 0519 007c 0119 007d 0574  ...|.d...|...}.t
+00001cf0: 096a 0aa0 0b7c 057c 03a1 0201 0074 0c7c  .j...|.|.....t.|
+00001d00: 0364 0683 028f 1a7d 0674 0864 0783 0101  .d.....}.t.d....
+00001d10: 007c 066a 0d7c 0464 088d 0101 0057 0035  .|.j.|.d.....W.5
+00001d20: 0051 0052 0058 0074 0864 0983 0101 0074  .Q.R.X.t.d.....t
+00001d30: 02a0 0e7c 03a1 0101 0074 0864 0a83 0101  ...|.....t.d....
+00001d40: 0064 0053 0029 0b4e 7a1d 2f77 6861 6363  .d.S.).Nz./whacc
+00001d50: 5f64 6174 612f 7472 6169 6e69 6e67 5f64  _data/training_d
+00001d60: 6174 612e 7a69 7072 8000 0000 7a56 7472  ata.zipr....zVtr
+00001d70: 6169 6e69 6e67 2064 6174 6120 6973 2061  aining data is a
+00001d80: 6c72 6561 6479 2064 6f77 6e6c 6f61 6465  lready downloade
+00001d90: 642c 2069 6620 796f 7520 7761 6e74 2074  d, if you want t
+00001da0: 6f20 6f76 6572 7772 6974 6520 6974 2073  o overwrite it s
+00001db0: 6574 206f 7665 7277 7269 7465 2074 6f20  et overwrite to 
+00001dc0: 5472 7565 7a22 646f 776e 6c6f 6164 696e  Truez"downloadin
+00001dd0: 6720 7472 6169 6e69 6e67 2064 6174 6120  g training data 
+00001de0: 2833 4742 292e 2e2e 7266 0000 0072 6d00  (3GB)...rf...rm.
+00001df0: 0000 726e 0000 0072 6f00 0000 7270 0000  ..rn...ro...rp..
+00001e00: 0072 7100 0000 7272 0000 0072 8100 0000  .rq...rr...r....
+00001e10: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001e20: 5a00 0000 e100 0000 7322 0000 0000 0106  Z.......s"......
+00001e30: 0110 010c 010c 0104 010c 0208 0104 0208  ................
+00001e40: 010c 010e 010c 0108 0116 0108 010a 0172  ...............r
+00001e50: 5a00 0000 6302 0000 0000 0000 0000 0000  Z...c...........
+00001e60: 0007 0000 0009 0000 0043 0000 0073 b400  .........C...s..
+00001e70: 0000 7400 8300 7d02 7401 8300 7402 6a03  ..t...}.t...t.j.
+00001e80: 1700 6401 1700 7d03 7c03 6400 6402 8502  ..d...}.|.d.d...
+00001e90: 1900 7d04 7402 6a04 a005 7c04 a101 724a  ..}.t.j...|...rJ
+00001ea0: 7c00 723e 7406 a007 7c04 a101 0100 6e0c  |.r>t...|.....n.
+00001eb0: 7408 6403 8301 0100 6400 5300 7408 6404  t.d.....d.S.t.d.
+00001ec0: 8301 0100 7c02 6405 1900 7c01 1900 7d05  ....|.d...|...}.
+00001ed0: 7409 6a0a a00b 7c05 7c03 a102 0100 740c  t.j...|.|.....t.
+00001ee0: 7c03 6406 8302 8f1a 7d06 7408 6407 8301  |.d.....}.t.d...
+00001ef0: 0100 7c06 6a0d 7c04 6408 8d01 0100 5700  ..|.j.|.d.....W.
+00001f00: 3500 5100 5200 5800 7408 6409 8301 0100  5.Q.R.X.t.d.....
+00001f10: 7402 a00e 7c03 a101 0100 7408 640a 8301  t...|.....t.d...
+00001f20: 0100 6400 5300 290b 4e7a 372f 7768 6163  ..d.S.).Nz7/whac
+00001f30: 635f 6461 7461 2f66 696e 616c 5f6d 6f64  c_data/final_mod
+00001f40: 656c 2f66 696e 616c 5f72 6573 6e65 7435  el/final_resnet5
+00001f50: 3056 325f 6675 6c6c 5f6d 6f64 656c 2e7a  0V2_full_model.z
+00001f60: 6970 7280 0000 007a 4e6d 6f64 656c 2069  ipr....zNmodel i
+00001f70: 7320 616c 7265 6164 7920 646f 776e 6c6f  s already downlo
+00001f80: 6164 6564 2c20 6966 2079 6f75 2077 616e  aded, if you wan
+00001f90: 7420 746f 206f 7665 7277 7269 7465 2069  t to overwrite i
+00001fa0: 7420 7365 7420 6f76 6572 7772 6974 6520  t set overwrite 
+00001fb0: 746f 2054 7275 657a 2564 6f77 6e6c 6f61  to Truez%downloa
+00001fc0: 6469 6e67 206d 6f64 656c 207a 6970 2066  ding model zip f
+00001fd0: 696c 6520 2831 3030 6d62 292e 2e2e 7265  ile (100mb)...re
+00001fe0: 0000 0072 6d00 0000 726e 0000 0072 6f00  ...rm...rn...ro.
+00001ff0: 0000 7270 0000 0072 7100 0000 7272 0000  ..rp...rq...rr..
+00002000: 0072 8100 0000 7216 0000 0072 1600 0000  .r....r....r....
+00002010: 7217 0000 0072 5900 0000 f700 0000 7322  r....rY.......s"
+00002020: 0000 0000 0106 0210 010c 010c 0104 010c  ................
+00002030: 0208 0104 0108 010c 010e 010c 0108 0116  ................
+00002040: 0108 010a 0172 5900 0000 e964 0000 0063  .....rY....d...c
+00002050: 0400 0000 0000 0000 0000 0000 0e00 0000  ................
+00002060: 0700 0000 4300 0000 7312 0100 0074 007c  ....C...s....t.|
+00002070: 0064 0183 027d 047c 0364 006b 0872 1c74  .d...}.|.d.k.r.t
+00002080: 01a0 027c 04a1 017d 0374 01a0 037c 03a1  ...|...}.t...|..
+00002090: 01a0 0474 05a1 017d 0374 007c 0064 0283  ...t...}.t.|.d..
+000020a0: 027d 0564 037d 067c 0272 4264 047d 0674  .}.d.}.|.rBd.}.t
+000020b0: 067c 0464 0383 027d 0774 01a0 077c 0764  .|.d...}.t...|.d
+000020c0: 0419 0064 0064 0585 0219 00a1 017c 0764  ...d.d.......|.d
+000020d0: 0419 0017 00a0 0474 08a1 017d 0874 01a0  .......t...}.t..
+000020e0: 037c 05a1 017c 087c 0666 0219 00a0 0474  .|...|.|.f.....t
+000020f0: 09a1 017d 0974 016a 0a7c 097c 033c 0074  ...}.t.j.|.|.<.t
+00002100: 01a0 0b7c 09a1 017d 0a74 01a0 0c7c 03a1  ...|...}.t...|..
+00002110: 0172 ba7c 0a64 0074 01a0 0d7c 03a1 010b  .r.|.d.t...|....
+00002120: 0085 0219 007d 0a74 01a0 0e74 01a0 0f64  .....}.t...t...d
+00002130: 0474 107c 0a83 0164 0318 007c 01a1 03a1  .t.|...d...|....
+00002140: 01a0 0474 08a1 017d 0b7c 0a7c 0b19 00a0  ...t...}.|.|....
+00002150: 0474 08a1 017d 0c74 117c 0c83 017d 0d74  .t...}.t.|...}.t
+00002160: 107c 0d83 0174 107c 0c83 016b 0390 0172  .|...t.|...k...r
+00002170: 0e74 12a0 1364 06a1 0101 007c 0d53 0029  .t...d.....|.S.)
+00002180: 074e 7241 0000 00da 0d6c 6f63 6174 696f  .NrA.....locatio
+00002190: 6e73 5f78 5f79 722e 0000 0072 0100 0000  ns_x_yr....r....
+000021a0: 7247 0000 007a 686c 6573 7320 7669 6162  rG...zhless viab
+000021b0: 6c65 2074 7269 616c 7320 7468 616e 2072  le trials than r
+000021c0: 6571 7565 7374 6564 2c20 6576 6572 7974  equested, everyt
+000021d0: 6869 6e67 2077 696c 6c20 776f 726b 2066  hing will work f
+000021e0: 696e 6520 6275 7420 7468 6572 6520 7769  ine but there wi
+000021f0: 6c6c 2062 6520 6c65 7373 2074 7269 616c  ll be less trial
+00002200: 7320 696e 2074 6865 206f 7574 7075 7429  s in the output)
+00002210: 1472 4d00 0000 721d 0000 00da 0a7a 6572  .rM...r......zer
+00002220: 6f73 5f6c 696b 6572 3800 0000 da06 6173  os_liker8.....as
+00002230: 7479 7065 da04 626f 6f6c 7237 0000 00da  type..boolr7....
+00002240: 046d 6561 6eda 0369 6e74 da05 666c 6f61  .mean..int..floa
+00002250: 7472 2200 0000 da07 6172 6773 6f72 74da  tr".....argsort.
+00002260: 0361 6e79 7235 0000 00da 0572 6f75 6e64  .anyr5.....round
+00002270: da08 6c69 6e73 7061 6365 7230 0000 00da  ..linspacer0....
+00002280: 1175 6e69 7175 655f 6b65 6570 5f6f 7264  .unique_keep_ord
+00002290: 6572 da08 7761 726e 696e 6773 da04 7761  er..warnings..wa
+000022a0: 726e 290e 7251 0000 005a 0a6e 756d 5f76  rn).rQ...Z.num_v
+000022b0: 6964 656f 735a 0765 7175 616c 5f78 5a12  ideosZ.equal_xZ.
+000022c0: 696e 6473 5f74 6f5f 6261 645f 7472 6961  inds_to_bad_tria
+000022d0: 6c73 7241 0000 0072 8300 0000 5a06 7879  lsrA...r....Z.xy
+000022e0: 5f69 6e64 5a03 666e 6cda 036d 6964 5a07  _indZ.fnl..midZ.
+000022f0: 785f 706f 6c65 735a 0a61 7267 5f78 706f  x_polesZ.arg_xpo
+00002300: 6c65 73da 0369 6478 da03 6f75 745a 0575  les..idx..outZ.u
+00002310: 5f6f 7574 7216 0000 0072 1600 0000 7217  _outr....r....r.
+00002320: 0000 00da 1a65 7175 616c 5f64 6973 7461  .....equal_dista
+00002330: 6e63 655f 706f 6c65 5f73 616d 706c 650d  nce_pole_sample.
+00002340: 0100 0073 2e00 0000 0001 0a01 0801 0a01  ...s............
+00002350: 1001 0a01 0401 0401 0401 0a02 2401 1801  ............$...
+00002360: 0a02 0a01 0a01 1402 2202 0e01 0801 1201  ........".......
+00002370: 0401 02ff 0402 7294 0000 0063 0900 0000  ......r....c....
+00002380: 0000 0000 0000 0000 2600 0000 0a00 0000  ........&.......
+00002390: 0300 0000 731a 0400 0074 007c 0383 017d  ....s....t.|...}
+000023a0: 0974 016a 02a0 037c 00a1 0174 016a 0417  .t.j...|...t.j..
+000023b0: 0064 0117 0074 016a 02a0 057c 00a1 0164  .d...t.j...|...d
+000023c0: 0064 0285 0219 0017 007d 0a7c 0564 006b  .d.......}.|.d.k
+000023d0: 0872 4674 016a 02a0 037c 00a1 017d 057c  .rFt.j...|...}.|
+000023e0: 0664 006b 0872 687c 0574 016a 0417 0064  .d.k.rh|.t.j...d
+000023f0: 0317 0074 016a 02a0 057c 00a1 0117 007d  ...t.j...|.....}
+00002400: 0674 016a 02a0 067c 06a1 0172 927c 0773  .t.j...|...r.|.s
+00002410: 8874 0764 047c 0617 0064 0517 0083 0182  .t.d.|...d......
+00002420: 0174 01a0 087c 06a1 0101 0074 097c 0583  .t...|.....t.|..
+00002430: 0101 0074 0a7c 0064 0664 0783 0389 0064  ...t.|.d.d.....d
+00002440: 0864 0964 0a64 0b67 047d 0b87 0066 0164  .d.d.d.g.}...f.d
+00002450: 0c64 0d84 087c 0b44 0083 017d 0c74 0ba0  .d...|.D...}.t..
+00002460: 0c7c 0ca1 0173 d674 0764 0e83 0182 0164  .|...s.t.d.....d
+00002470: 0f67 017d 0b87 0066 0164 1064 0d84 087c  .g.}...f.d.d...|
+00002480: 0b44 0083 017d 0d88 0164 006b 0890 0172  .D...}...d.k...r
+00002490: 1064 0f88 006b 0790 0172 1064 1190 0173  .d...k...r.d...s
+000024a0: 1074 0764 1283 0182 0174 0ba0 0d7c 027c  .t.d.....t...|.|
+000024b0: 0118 0067 017c 0914 00a1 017d 0e7c 0864  ...g.|.....}.|.d
+000024c0: 006b 0890 0172 3874 0ea0 0fa1 007d 0f6e  .k...r8t.....}.n
+000024d0: 0874 107c 0883 017d 0f67 007d 1067 007d  .t.|...}.g.}.g.}
+000024e0: 1167 007d 1264 137d 137c 137c 027c 0118  .g.}.d.}.|.|.|..
+000024f0: 006b 0490 0172 787c 027c 0118 007d 1374  .k...rx|.|...}.t
+00002500: 11a0 1264 1474 137c 1383 0117 00a1 0101  ...d.t.|........
+00002510: 0074 0ba0 0d74 1474 157c 0064 0a83 0264  .t...t.t.|.d...d
+00002520: 1583 02a1 0164 0064 0085 027c 0366 0219  .....d.d...|.f..
+00002530: 007d 1474 16a0 177c 0064 16a1 028f 9c7d  .}.t...|.d.....}
+00002540: 1574 1874 197c 1464 0719 007c 1464 0619  .t.t.|.d...|.d..
+00002550: 0083 0283 0144 005d 7e5c 027d 165c 027d  .....D.]~\.}.\.}
+00002560: 177d 1864 0f88 006b 0690 0172 f27c 10a0  .}.d...k...r.|..
+00002570: 1a7c 1564 0f19 007c 177c 1885 0219 007c  .|.d...|.|.....|
+00002580: 017c 0285 0219 00a1 0101 007c 1564 0b19  .|.........|.d..
+00002590: 007c 177c 1885 0219 007c 017c 0285 0219  .|.|.....|.|....
+000025a0: 007d 197c 11a0 1a7c 19a1 0101 0074 1b7c  .}.|...|.....t.|
+000025b0: 0fa0 1c7c 19a1 017c 1383 027d 1a7c 1a64  ...|...|...}.|.d
+000025c0: 176b 0464 0614 007d 1a7c 12a0 1a7c 1aa1  .k.d...}.|...|..
+000025d0: 0101 0090 0171 be57 0035 0051 0052 0058  .....q.W.5.Q.R.X
+000025e0: 0064 0f88 006b 0690 0272 5c74 0ba0 1d7c  .d...k...r\t...|
+000025f0: 10a1 017d 1074 0ba0 1d7c 11a1 017d 1174  ...}.t...|...}.t
+00002600: 0ba0 1e7c 12a1 017d 1274 16a0 177c 0664  ...|...}.t...|.d
+00002610: 18a1 028f 3e7d 1b7c 0e7c 1b64 0a3c 007c  ....>}.|.|.d.<.|
+00002620: 127c 1b64 193c 0074 157c 0064 0883 027c  .|.d.<.t.|.d...|
+00002630: 1b64 083c 0064 0f88 006b 0690 0272 ae7c  .d.<.d...k...r.|
+00002640: 107c 1b64 0f3c 007c 117c 1b64 0b3c 0057  .|.d.<.|.|.d.<.W
+00002650: 0035 0051 0052 0058 0064 0f88 006b 0790  .5.Q.R.X.d...k..
+00002660: 0472 1674 0ba0 0d74 1f74 157c 0064 0983  .r.t...t.t.|.d..
+00002670: 0283 01a1 017c 0319 007d 1c87 0166 0164  .....|...}...f.d
+00002680: 1a64 0d84 087c 1c44 0083 017d 1c74 0ba0  .d...|.D...}.t..
+00002690: 207c 0164 1b18 007c 02a1 027d 1d74 2188   |.d...|...}.t!.
+000026a0: 0174 157c 0064 0883 027c 1d64 1564 1c8d  .t.|.d...|.d.d..
+000026b0: 047d 1e74 016a 02a0 057c 0aa1 017c 1e5f  .}.t.j...|...|._
+000026c0: 227c 1c7c 1e5f 237c 1ea0 24a1 0001 007c  "|.|._#|..$....|
+000026d0: 1e6a 257d 1f7c 1fa0 2664 1d64 1ea1 027d  .j%}.|..&d.d...}
+000026e0: 2074 27a0 287c 1f7c 20a1 0201 0074 0ba0   t'.(|.| ....t..
+000026f0: 297c 1da1 017d 1964 067c 1964 1b64 1b7c  )|...}.d.|.d.d.|
+00002700: 0217 007c 0118 0085 023c 0074 0ba0 0d74  ...|.....<.t...t
+00002710: 2a7c 1983 0174 007c 1c83 0114 00a1 01a0  *|...t.|........
+00002720: 2b74 2ca1 017d 2174 0074 157c 0664 1983  +t,..}!t.t.|.d..
+00002730: 0283 017d 227c 2274 0ba0 2d7c 21a1 016b  ...}"|"t..-|!..k
+00002740: 0290 0373 b474 0764 1f83 0182 0174 0ba0  ...s.t.d.....t..
+00002750: 2e7c 21a1 0164 0719 007d 2374 16a0 177c  .|!..d...}#t...|
+00002760: 0664 20a1 028f 2e7d 2474 16a0 177c 2064  .d ....}$t...| d
+00002770: 16a1 028f 167d 257c 2564 0f19 007c 2319  .....}%|%d...|#.
+00002780: 007c 2464 0f3c 0057 0035 0051 0052 0058  .|$d.<.W.5.Q.R.X
+00002790: 0057 0035 0051 0052 0058 0074 01a0 087c  .W.5.Q.R.X.t...|
+000027a0: 1fa1 0101 0074 01a0 087c 20a1 0101 0064  .....t...| ....d
+000027b0: 0053 0029 214e 5a0d 5445 4d50 5f54 4c5f  .S.)!NZ.TEMP_TL_
+000027c0: 4441 5441 5fe9 fdff ffff 5a08 544c 5f44  DATA_.....Z.TL_D
+000027d0: 4154 415f 7a05 4669 6c65 207a 3a20 6578  ATA_z.File z: ex
+000027e0: 6973 7473 2c20 7365 7420 6f76 6572 7772  ists, set overwr
+000027f0: 6974 6520 746f 2054 7275 6520 6f66 2079  ite to True of y
+00002800: 6f75 2077 616e 7420 746f 206f 7665 7277  ou want to overw
+00002810: 7269 7465 2069 7472 2e00 0000 7201 0000  rite itr....r...
+00002820: 00da 0c74 656d 706c 6174 655f 696d 67da  ...template_img.
+00002830: 0f66 756c 6c5f 6669 6c65 5f6e 616d 6573  .full_file_names
+00002840: 7241 0000 0072 4900 0000 6301 0000 0000  rA...rI...c.....
+00002850: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00002860: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+00002870: 7c01 8800 6b06 9102 7104 5300 7216 0000  |...k...q.S.r...
+00002880: 0072 1600 0000 7231 0000 00a9 01da 046b  .r....r1.......k
+00002890: 6579 7372 1600 0000 7217 0000 0072 3400  eysr....r....r4.
+000028a0: 0000 3b01 0000 7304 0000 0006 0002 007a  ..;...s........z
+000028b0: 2f6d 616b 655f 7472 616e 7366 6572 5f6c  /make_transfer_l
+000028c0: 6561 726e 696e 675f 6461 7461 2e3c 6c6f  earning_data.<lo
+000028d0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000028e0: 7a81 2774 656d 706c 6174 655f 696d 6727  z.'template_img'
+000028f0: 2c20 2766 756c 6c5f 6669 6c65 5f6e 616d  , 'full_file_nam
+00002900: 6573 272c 2027 6669 6e61 6c5f 6665 6174  es', 'final_feat
+00002910: 7572 6573 5f32 3130 3527 2061 6e64 2027  ures_2105' and '
+00002920: 6672 616d 655f 6e75 6d73 2720 6d75 7374  frame_nums' must
+00002930: 2062 6520 7072 6573 656e 742c 2073 6f6d   be present, som
+00002940: 6574 6869 6e67 2069 7320 7772 6f6e 6720  ething is wrong 
+00002950: 7769 7468 2074 6865 2048 3520 6669 6c65  with the H5 file
+00002960: 2e2e 2eda 0669 6d61 6765 7363 0100 0000  .....imagesc....
+00002970: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002980: 1300 0000 7314 0000 0067 007c 005d 0c7d  ....s....g.|.].}
+00002990: 017c 0188 006b 0691 0271 0453 0072 1600  .|...k...q.S.r..
+000029a0: 0000 7216 0000 0072 3100 0000 7298 0000  ..r....r1...r...
+000029b0: 0072 1600 0000 7217 0000 0072 3400 0000  .r....r....r4...
+000029c0: 4001 0000 7304 0000 0006 0002 0046 7a2d  @...s........Fz-
+000029d0: 2769 6d61 6765 7327 206b 6579 206e 6f74  'images' key not
+000029e0: 2070 7265 7365 6e74 2070 6c65 6173 6520   present please 
+000029f0: 7365 7420 2776 6964 5f64 6972 27e9 0500  set 'vid_dir'...
+00002a00: 0000 7a74 6c65 6e67 7468 206f 6620 7365  ..ztlength of se
+00002a10: 7175 656e 7469 616c 2066 7261 6d65 7320  quential frames 
+00002a20: 7365 6c65 6374 6564 2069 7320 736d 616c  selected is smal
+00002a30: 6c65 7220 7468 616e 2074 6865 2064 6566  ler than the def
+00002a40: 6175 6c74 2073 6d6f 6f74 6869 6e67 206b  ault smoothing k
+00002a50: 6572 6e65 6c20 6f66 2035 2c20 7365 7474  ernel of 5, sett
+00002a60: 696e 6720 736d 6f6f 7468 696e 6720 6b65  ing smoothing ke
+00002a70: 726e 656c 2074 6f20 5472 6d00 0000 e700  rnel to Trm.....
+00002a80: 0000 0000 00e0 3fda 0177 7252 0000 0063  ......?..wrR...c
+00002a90: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002aa0: 0500 0000 1300 0000 731e 0000 0067 007c  ........s....g.|
+00002ab0: 005d 167d 0174 0088 0074 016a 0217 007c  .].}.t...t.j...|
+00002ac0: 0117 0083 0191 0271 0453 0072 1600 0000  .......q.S.r....
+00002ad0: 2903 da09 6e6f 726d 5f70 6174 6872 5f00  )...norm_pathr_.
+00002ae0: 0000 7260 0000 0029 0272 3200 0000 5a03  ..r`...).r2...Z.
+00002af0: 7669 6429 01da 0776 6964 5f64 6972 7216  vid)...vid_dirr.
+00002b00: 0000 0072 1700 0000 7234 0000 0070 0100  ...r....r4...p..
+00002b10: 0073 0400 0000 0600 0200 7247 0000 0029  .s........rG...)
+00002b20: 04da 0f76 6964 656f 5f64 6972 6563 746f  ...video_directo
+00002b30: 7279 da16 7465 6d70 6c61 7465 5f70 6e67  ry..template_png
+00002b40: 5f66 756c 6c5f 6e61 6d65 da11 7365 6c65  _full_name..sele
+00002b50: 6374 5f66 7261 6d65 5f69 6e64 73da 1b73  ct_frame_inds..s
+00002b60: 6b69 705f 6368 6563 6b5f 6966 5f46 5053  kip_check_if_FPS
+00002b70: 5f69 735f 616e 5f69 6e74 fa03 2e68 35fa  _is_an_int...h5.
+00002b80: 085f 336c 6167 2e68 357a 254c 656e 6774  ._3lag.h5z%Lengt
+00002b90: 6820 6f66 206c 6162 656c 7320 616e 6420  h of labels and 
+00002ba0: 696e 6473 2064 6f6e 2774 206d 6174 6368  inds don't match
+00002bb0: fa02 722b 292f 7230 0000 0072 5f00 0000  ..r+)/r0...r_...
+00002bc0: 7261 0000 00da 0764 6972 6e61 6d65 7260  ra.....dirnamer`
+00002bd0: 0000 00da 0862 6173 656e 616d 65da 0669  .....basename..i
+00002be0: 7366 696c 6572 4e00 0000 7279 0000 00da  sfilerN...ry....
+00002bf0: 096d 616b 655f 7061 7468 da0d 7072 696e  .make_path..prin
+00002c00: 745f 6835 5f6b 6579 7372 1d00 0000 722f  t_h5_keysr....r/
+00002c10: 0000 0072 3800 0000 7205 0000 00da 146c  ...r8...r......l
+00002c20: 6f61 645f 6669 6e61 6c5f 6c69 6768 745f  oad_final_light_
+00002c30: 4742 4d72 6300 0000 728f 0000 0072 9000  GBMrc...r....r..
+00002c40: 0000 da03 7374 7272 3700 0000 724d 0000  ....strr7...rM..
+00002c50: 00da 0468 3570 79da 0446 696c 6572 2400  ...h5py..Filer$.
+00002c60: 0000 da03 7a69 7072 2300 0000 da06 736d  ....zipr#.....sm
+00002c70: 6f6f 7468 da07 7072 6564 6963 7472 2500  ooth..predictr%.
+00002c80: 0000 7226 0000 00da 1268 355f 7374 7269  ..r&.....h5_stri
+00002c90: 6e67 5f73 7769 7463 6865 72da 0661 7261  ng_switcher..ara
+00002ca0: 6e67 6572 0400 0000 5a0e 7361 7665 5f62  nger....Z.save_b
+00002cb0: 6173 655f 6e61 6d65 da0b 7669 6465 6f5f  ase_name..video_
+00002cc0: 6669 6c65 735a 1274 7261 636b 5f61 6c6c  filesZ.track_all
+00002cd0: 5f61 6e64 5f73 6176 65da 0c66 756c 6c5f  _and_save..full_
+00002ce0: 6835 5f6e 616d 65da 0772 6570 6c61 6365  h5_name..replace
+00002cf0: 7208 0000 00da 0f63 6f6e 7665 7274 5f74  r......convert_t
+00002d00: 6f5f 336c 6167 7284 0000 0072 3900 0000  o_3lagr....r9...
+00002d10: 7285 0000 0072 8600 0000 7235 0000 00da  r....r....r5....
+00002d20: 0577 6865 7265 2926 7251 0000 005a 0b73  .where)&rQ...Z.s
+00002d30: 7461 7274 5f66 7261 6d65 5a09 656e 645f  tart_frameZ.end_
+00002d40: 6672 616d 655a 1265 7175 616c 5f78 5f74  frameZ.equal_x_t
+00002d50: 7269 616c 5f69 6e64 7372 9f00 0000 da08  rial_indsr......
+00002d60: 6261 7365 5f64 6972 5a15 6669 6e61 6c5f  base_dirZ.final_
+00002d70: 7472 696d 6d65 645f 6835 5f6e 616d 6572  trimmed_h5_namer
+00002d80: 5c00 0000 5a14 6d6f 6465 6c5f 6675 6c6c  \...Z.model_full
+00002d90: 5f66 696c 655f 6e61 6d65 5a16 6e75 6d5f  _file_nameZ.num_
+00002da0: 7472 6961 6c73 5f70 6572 5f73 6573 7369  trials_per_sessi
+00002db0: 6f6e da0b 6e65 775f 6835 5f6e 616d 655a  on..new_h5_nameZ
+00002dc0: 0a63 6865 636b 5f6b 6579 735a 0f63 6865  .check_keysZ.che
+00002dd0: 636b 5f6b 6579 735f 6e65 6564 5a13 6368  ck_keys_needZ.ch
+00002de0: 6563 6b5f 6b65 7973 5f6e 6f5f 7265 7275  eck_keys_no_reru
+00002df0: 6e5a 0e6e 6577 5f66 7261 6d65 5f6e 756d  nZ.new_frame_num
+00002e00: 73da 036d 6f64 729a 0000 0072 4900 0000  s..modr....rI...
+00002e10: 5a0b 7072 6564 5f6c 6162 656c 735a 0973  Z.pred_labelsZ.s
+00002e20: 6d6f 6f74 685f 6279 5a09 6c6f 6f70 5f73  mooth_byZ.loop_s
+00002e30: 6567 735a 0668 5f72 6561 6472 2c00 0000  egsZ.h_readr,...
+00002e40: da02 6b31 da02 6b32 7253 0000 00da 0179  ..k1..k2rS.....y
+00002e50: da01 685a 0f73 656c 6563 7465 645f 7669  ..hZ.selected_vi
+00002e60: 6465 6f73 72a2 0000 00da 0270 74da 0568  deosr......pt..h
+00002e70: 355f 696e da07 6835 5f33 6c61 6772 2b00  5_in..h5_3lagr+.
+00002e80: 0000 da01 4c5a 0569 6e64 7332 5a05 685f  ....LZ.inds2Z.h_
+00002e90: 6473 745a 0568 5f73 7263 7216 0000 0029  dstZ.h_srcr....)
+00002ea0: 0272 9900 0000 729f 0000 0072 1700 0000  .r....r....r....
+00002eb0: da1b 6d61 6b65 5f74 7261 6e73 6665 725f  ..make_transfer_
+00002ec0: 6c65 6172 6e69 6e67 5f64 6174 612a 0100  learning_data*..
+00002ed0: 0073 a600 0000 0002 0802 2a01 0801 0c01  .s........*.....
+00002ee0: 0801 1a01 0c01 1401 0a01 0802 0c02 0c01  ................
+00002ef0: 1201 0401 02ff 0601 02ff 0403 0601 1204  ................
+00002f00: 1401 0e02 1401 0a01 0a02 0801 0401 0401  ................
+00002f10: 0402 0401 0e01 0801 0401 0401 02ff 04ff  ................
+00002f20: 0403 2202 0e01 2201 0a01 1e01 1801 0a01  .."...".........
+00002f30: 1001 0c01 1801 0a01 0a01 0a01 0a02 0e01  ................
+00002f40: 0801 0801 0e01 0a01 0801 1202 0a01 1801  ................
+00002f50: 1201 1004 0c01 0200 02ff 0602 0e01 0601  ................
+00002f60: 0803 0602 0c01 0c02 0a01 1401 1c01 0e01  ................
+00002f70: 1801 0e02 0e01 0e01 2401 0a01 72c5 0000  ........$...r...
+00002f80: 0063 0100 0000 0000 0000 0000 0000 0600  .c..............
+00002f90: 0000 0600 0000 4300 0000 7386 0000 0067  ......C...s....g
+00002fa0: 007d 0174 007c 0083 0144 005d 747d 0274  .}.t.|...D.]t}.t
+00002fb0: 01a0 027c 02a1 017d 037c 03a0 03a1 0064  ...|...}.|.....d
+00002fc0: 016b 0272 0c74 047c 03a0 0564 02a1 0183  .k.r.t.|...d....
+00002fd0: 017d 047c 03a0 0564 03a1 017d 057c 0574  .}.|...d...}.|.t
+00002fe0: 047c 0583 016b 0273 7674 0664 0474 076a  .|...k.svt.d.t.j
+00002ff0: 08a0 097c 02a1 0117 0064 0517 0074 0a7c  ...|.....d...t.|
+00003000: 0483 0117 0083 0101 007c 01a0 0b64 01a1  .........|...d..
+00003010: 0101 0071 0c7c 01a0 0b64 06a1 0101 0071  ...q.|...d.....q
+00003020: 0c7c 0153 0029 074e 5472 4500 0000 729b  .|.S.).NTrE...r.
+00003030: 0000 007a 0966 6f72 2066 696c 6520 7a58  ...z.for file zX
+00003040: 2046 5053 2069 7320 6e6f 7420 616e 2069   FPS is not an i
+00003050: 6e74 6567 6572 2c20 7468 6973 2075 7375  nteger, this usu
+00003060: 616c 6c79 2069 6e64 6963 6174 6573 2061  ally indicates a
+00003070: 2070 726f 626c 656d 2077 6974 6820 7468   problem with th
+00003080: 6520 7669 6465 6f2e 2054 4f54 414c 2046  e video. TOTAL F
+00003090: 5241 4d45 5320 3d20 4629 0c72 0b00 0000  RAMES = F).r....
+000030a0: da03 6376 32da 0c56 6964 656f 4361 7074  ..cv2..VideoCapt
+000030b0: 7572 65da 0869 734f 7065 6e65 6472 8800  ure..isOpenedr..
+000030c0: 0000 da03 6765 7472 4b00 0000 725f 0000  ....getrK...r_..
+000030d0: 0072 6100 0000 72a8 0000 0072 ad00 0000  .ra...r....r....
+000030e0: 7223 0000 0029 0672 b500 0000 5a08 6261  r#...).r....Z.ba
+000030f0: 645f 696e 6473 da0a 7669 6465 6f5f 6669  d_inds..video_fi
+00003100: 6c65 da05 7669 6465 6fda 0d66 7261 6d65  le..video..frame
+00003110: 5f6e 756d 6265 7273 da03 6670 7372 1600  _numbers..fpsr..
+00003120: 0000 7216 0000 0072 1700 0000 da2c 6368  ..r....r.....,ch
+00003130: 6563 6b5f 7669 6473 5f66 6f72 5f69 7373  eck_vids_for_iss
+00003140: 7565 735f 6261 7365 645f 6f6e 5f46 5053  ues_based_on_FPS
+00003150: 5f61 735f 616e 5f69 6e74 8f01 0000 731e  _as_an_int....s.
+00003160: 0000 0000 0104 010c 010a 010c 010e 010a  ................
+00003170: 010c 0110 0102 ff02 0206 fe06 030c 040c  ................
+00003180: 0172 ce00 0000 6301 0000 0000 0000 0000  .r....c.........
+00003190: 0000 0003 0000 0005 0000 0003 0000 0073  ...............s
+000031a0: 3800 0000 7400 6a01 8800 6401 6402 8d02  8...t.j...d.d...
+000031b0: 6403 1900 7d01 7400 a002 8700 6601 6404  d...}.t.....f.d.
+000031c0: 6405 8408 7403 7c01 8301 4400 8301 a101  d...t.|...D.....
+000031d0: a004 7405 a101 7d02 7c02 5300 2906 4e54  ..t...}.|.S.).NT
+000031e0: 2901 da0c 7265 7475 726e 5f69 6e64 6578  )...return_index
+000031f0: 722e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00003200: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
+00003210: 0000 0067 007c 005d 0c7d 0188 007c 0119  ...g.|.].}...|..
+00003220: 0091 0271 0453 0072 1600 0000 7216 0000  ...q.S.r....r...
+00003230: 0029 0272 3200 0000 da05 696e 6465 78a9  .).r2.....index.
+00003240: 0172 5300 0000 7216 0000 0072 1700 0000  .rS...r....r....
+00003250: 7234 0000 00b6 0100 0073 0400 0000 0600  r4.......s......
+00003260: 0200 7a25 756e 6971 7565 5f6b 6565 705f  ..z%unique_keep_
+00003270: 6f72 6465 722e 3c6c 6f63 616c 733e 2e3c  order.<locals>.<
+00003280: 6c69 7374 636f 6d70 3e29 0672 1d00 0000  listcomp>).r....
+00003290: da06 756e 6971 7565 7238 0000 00da 0673  ..uniquer8.....s
+000032a0: 6f72 7465 6472 8500 0000 7288 0000 0029  ortedr....r....)
+000032b0: 0372 5300 0000 5a07 696e 6465 7865 7372  .rS...Z.indexesr
+000032c0: 9300 0000 7216 0000 0072 d100 0000 7217  ....r....r....r.
+000032d0: 0000 0072 8e00 0000 b401 0000 7306 0000  ...r........s...
+000032e0: 0000 0112 0122 0172 8e00 0000 6301 0000  .....".r....c...
+000032f0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00003300: 0003 0000 0073 2600 0000 6401 a000 8800  .....s&...d.....
+00003310: a001 6402 a101 a101 8900 7402 8700 6601  ..d.......t...f.
+00003320: 6403 6404 8408 6405 4400 8301 8301 5300  d.d...d.D.....S.
+00003330: 2906 4eda 00fa 0123 6301 0000 0000 0000  ).N....#c.......
+00003340: 0000 0000 0002 0000 0006 0000 0033 0000  .............3..
+00003350: 0073 2400 0000 7c00 5d1c 7d01 7400 8800  .s$...|.].}.t...
+00003360: 7c01 7c01 6400 1700 8502 1900 6401 8302  |.|.d.......d...
+00003370: 5600 0100 7102 6402 5300 2903 7247 0000  V...q.d.S.).rG..
+00003380: 00e9 1000 0000 4e29 0172 8800 0000 2902  ......N).r....).
+00003390: 7232 0000 0072 2c00 0000 a901 72c0 0000  r2...r,.....r...
+000033a0: 0072 1600 0000 7217 0000 00da 093c 6765  .r....r......<ge
+000033b0: 6e65 7870 723e bc01 0000 7304 0000 0004  nexpr>....s.....
+000033c0: 0002 007a 1d68 6578 5f74 6f5f 7267 622e  ...z.hex_to_rgb.
+000033d0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+000033e0: 723e 2903 7201 0000 0072 4700 0000 e904  r>).r....rG.....
+000033f0: 0000 0029 03da 046a 6f69 6eda 0573 706c  ...)...join..spl
+00003400: 6974 7239 0000 0072 d700 0000 7216 0000  itr9...r....r...
+00003410: 0072 d700 0000 7217 0000 00da 0a68 6578  .r....r......hex
+00003420: 5f74 6f5f 7267 62ba 0100 0073 0400 0000  _to_rgb....s....
+00003430: 0001 1001 72dc 0000 0063 0300 0000 0000  ....r....c......
+00003440: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
+00003450: 0000 73a6 0000 0074 007c 0083 0174 0074  ..s....t.|...t.t
+00003460: 017c 0083 0183 016b 0273 1c74 0264 0183  .|.....k.s.t.d..
+00003470: 0182 0174 007c 0183 0174 0074 017c 0183  ...t.|...t.t.|..
+00003480: 0183 016b 0273 3874 0264 0283 0182 017c  ...k.s8t.d.....|
+00003490: 0264 036b 0872 447c 007d 0267 007d 037c  .d.k.rD|.}.g.}.|
+000034a0: 0144 005d 4a7d 047c 047c 006b 0672 8a74  .D.]J}.|.|.k.r.t
+000034b0: 03a0 047c 04a1 0173 8a7c 047c 006b 027d  ...|...s.|.|.k.}
+000034c0: 057c 03a0 0574 03a0 067c 05a1 0164 0419  .|...t...|...d..
+000034d0: 0064 0419 00a0 0774 08a1 01a1 0101 0071  .d.....t.......q
+000034e0: 4c7c 03a0 0574 036a 09a1 0101 0071 4c74  L|...t.j.....qLt
+000034f0: 0a7c 027c 0383 027d 067c 0653 0029 0561  .|.|...}.|.S.).a
+00003500: 9505 0000 0a0a 2020 2020 5061 7261 6d65  ......    Parame
+00003510: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00003520: 2d2d 2d0a 2020 2020 7372 635f 6461 7461  ---.    src_data
+00003530: 5f69 6e64 7320 3a20 2063 6f6d 6520 6672  _inds :  come fr
+00003540: 6f6d 2074 6865 2064 6174 6120 796f 7520  om the data you 
+00003550: 7761 6e74 2074 6f20 7573 653b 2069 6e64  want to use; ind
+00003560: 732c 2074 7269 616c 206e 756d 7320 6f72  s, trial nums or
+00003570: 2066 7261 6d65 206e 756d 732c 206f 7220   frame nums, or 
+00003580: 7261 7720 696e 6473 3b20 6d75 7374 2062  raw inds; must b
+00003590: 6520 756e 6971 7565 0a20 2020 2064 6174  e unique.    dat
+000035a0: 615f 746f 5f6d 6174 6368 5f69 6e64 7320  a_to_match_inds 
+000035b0: 3a20 2773 7263 5f64 6174 615f 696e 6473  : 'src_data_inds
+000035c0: 2720 7769 6c6c 2062 6520 666f 7263 6564  ' will be forced
+000035d0: 2074 6f20 6d61 7463 6820 2764 6174 615f   to match 'data_
+000035e0: 746f 5f6d 6174 6368 5f69 6e64 7327 2069  to_match_inds' i
+000035f0: 6e64 6578 2c20 6c65 6e67 7468 2061 6e64  ndex, length and
+00003600: 206f 7264 6572 2c20 696e 6473 2c20 7472   order, inds, tr
+00003610: 6961 6c20 6e75 6d73 206f 7220 6672 616d  ial nums or fram
+00003620: 6520 6e75 6d73 2c20 6f72 2072 6177 2069  e nums, or raw i
+00003630: 6e64 733b 206d 7573 7420 6265 2075 6e69  nds; must be uni
+00003640: 7175 650a 2020 2020 6461 7461 203a 206d  que.    data : m
+00003650: 6174 6368 6573 2027 6461 7461 5f74 6f5f  atches 'data_to_
+00003660: 6d61 7463 685f 696e 6473 2720 6275 7420  match_inds' but 
+00003670: 6973 2074 6865 2061 6374 6175 6c0a 0a20  is the actaul.. 
+00003680: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00003690: 2d2d 2d2d 2d2d 0a20 2020 2069 6e64 6578  ------.    index
+000036a0: 2064 6174 6120 6672 6f6d 2064 6174 6120   data from data 
+000036b0: 6172 7261 7920 2764 6174 6127 2074 6861  array 'data' tha
+000036c0: 7420 6d61 7463 6865 7320 7468 6520 6c65  t matches the le
+000036d0: 6e67 7468 206f 6620 2764 6174 615f 746f  ngth of 'data_to
+000036e0: 5f6d 6174 6368 5f69 6e64 7327 0a0a 2020  _match_inds'..  
+000036f0: 2020 4578 616d 706c 6573 0a20 2020 205f    Examples.    _
+00003700: 5f5f 5f5f 5f5f 5f0a 2020 2020 6461 7461  _______.    data
+00003710: 5f69 6e64 7320 3d20 2020 2020 206e 702e  _inds =      np.
+00003720: 6173 6172 7261 7928 5b31 322c 2031 312c  asarray([12, 11,
+00003730: 2031 332c 2031 342c 2031 352c 2020 2020   13, 14, 15,    
+00003740: 2020 3137 5d29 0a20 2020 206d 6174 6368    17]).    match
+00003750: 5f73 6574 5f69 6e64 7320 3d20 6e70 2e61  _set_inds = np.a
+00003760: 7361 7272 6179 285b 3131 2c20 3132 2c20  sarray([11, 12, 
+00003770: 2020 2020 3134 2c20 3135 2c20 3136 2c20      14, 15, 16, 
+00003780: 2031 372c 2020 3138 2c20 2031 392c 2020   17,  18,  19,  
+00003790: 3230 5d29 0a20 2020 2064 6174 6120 3d20  20]).    data = 
+000037a0: 6e70 2e61 7361 7272 6179 285b 392c 382c  np.asarray([9,8,
+000037b0: 322c 332c 342c 372c 352c 362c 342c 352c  2,3,4,7,5,6,4,5,
+000037c0: 362c 372c 382c 392c 3932 2c31 2c31 2c35  6,7,8,9,92,1,1,5
+000037d0: 362c 3333 2c34 342c 3535 2c36 362c 3737  6,33,44,55,66,77
+000037e0: 5d29 0a0a 2020 2020 6f75 7420 3d20 7574  ])..    out = ut
+000037f0: 696c 732e 696e 7465 7273 6563 745f 6461  ils.intersect_da
+00003800: 7461 5f77 6974 685f 6e61 6e73 2864 6174  ta_with_nans(dat
+00003810: 615f 696e 6473 2c20 6d61 7463 685f 7365  a_inds, match_se
+00003820: 745f 696e 6473 2c20 6461 7461 3d4e 6f6e  t_inds, data=Non
+00003830: 6529 0a20 2020 2070 7269 6e74 286e 702e  e).    print(np.
+00003840: 7673 7461 636b 2828 6f75 742c 206d 6174  vstack((out, mat
+00003850: 6368 5f73 6574 5f69 6e64 7329 2929 0a0a  ch_set_inds)))..
+00003860: 2020 2020 6f75 7420 3d20 7574 696c 732e      out = utils.
+00003870: 696e 7465 7273 6563 745f 6461 7461 5f77  intersect_data_w
+00003880: 6974 685f 6e61 6e73 286d 6174 6368 5f73  ith_nans(match_s
+00003890: 6574 5f69 6e64 732c 2064 6174 615f 696e  et_inds, data_in
+000038a0: 6473 2c20 6461 7461 3d4e 6f6e 6529 0a20  ds, data=None). 
+000038b0: 2020 2070 7269 6e74 286e 702e 7673 7461     print(np.vsta
+000038c0: 636b 2828 6f75 742c 2064 6174 615f 696e  ck((out, data_in
+000038d0: 6473 2929 290a 0a20 2020 2064 6174 615f  ds)))..    data_
+000038e0: 696e 6473 5f64 6174 6120 3d20 6461 7461  inds_data = data
+000038f0: 5b64 6174 615f 696e 6473 5d0a 2020 2020  [data_inds].    
+00003900: 6d61 7463 685f 7365 745f 696e 6473 5f64  match_set_inds_d
+00003910: 6174 6120 3d20 6461 7461 5b6d 6174 6368  ata = data[match
+00003920: 5f73 6574 5f69 6e64 735d 0a20 2020 206f  _set_inds].    o
+00003930: 7574 203d 2075 7469 6c73 2e69 6e74 6572  ut = utils.inter
+00003940: 7365 6374 5f64 6174 615f 7769 7468 5f6e  sect_data_with_n
+00003950: 616e 7328 6461 7461 5f69 6e64 732c 206d  ans(data_inds, m
+00003960: 6174 6368 5f73 6574 5f69 6e64 732c 2064  atch_set_inds, d
+00003970: 6174 613d 6461 7461 5f69 6e64 735f 6461  ata=data_inds_da
+00003980: 7461 290a 2020 2020 7072 696e 7428 6e70  ta).    print(np
+00003990: 2e76 7374 6163 6b28 286f 7574 2c20 6d61  .vstack((out, ma
+000039a0: 7463 685f 7365 745f 696e 6473 5f64 6174  tch_set_inds_dat
+000039b0: 6129 2929 0a0a 2020 2020 6461 7461 5f69  a)))..    data_i
+000039c0: 6e64 735f 6461 7461 203d 2064 6174 615b  nds_data = data[
+000039d0: 6461 7461 5f69 6e64 735d 0a20 2020 206d  data_inds].    m
+000039e0: 6174 6368 5f73 6574 5f69 6e64 735f 6461  atch_set_inds_da
+000039f0: 7461 203d 2064 6174 615b 6d61 7463 685f  ta = data[match_
+00003a00: 7365 745f 696e 6473 5d0a 2020 2020 6f75  set_inds].    ou
+00003a10: 7420 3d20 7574 696c 732e 696e 7465 7273  t = utils.inters
+00003a20: 6563 745f 6461 7461 5f77 6974 685f 6e61  ect_data_with_na
+00003a30: 6e73 286d 6174 6368 5f73 6574 5f69 6e64  ns(match_set_ind
+00003a40: 732c 2064 6174 615f 696e 6473 2c20 6461  s, data_inds, da
+00003a50: 7461 3d6d 6174 6368 5f73 6574 5f69 6e64  ta=match_set_ind
+00003a60: 735f 6461 7461 290a 2020 2020 7072 696e  s_data).    prin
+00003a70: 7428 6e70 2e76 7374 6163 6b28 286f 7574  t(np.vstack((out
+00003a80: 2c20 6461 7461 5f69 6e64 735f 6461 7461  , data_inds_data
+00003a90: 2929 290a 0a20 2020 207a 3264 6174 615f  )))..    z2data_
+00003aa0: 696e 6473 2063 6f6e 7461 696e 7320 6475  inds contains du
+00003ab0: 706c 6963 6174 6573 2c20 7468 6973 2069  plicates, this i
+00003ac0: 7320 6e6f 7420 616c 6c6f 7765 647a 376d  s not allowedz7m
+00003ad0: 6174 6368 5f73 6574 5f69 6e64 7320 636f  atch_set_inds co
+00003ae0: 6e74 6169 6e73 2064 7570 6c69 6361 7465  ntains duplicate
+00003af0: 732c 2074 6869 7320 6973 206e 6f74 2061  s, this is not a
+00003b00: 6c6c 6f77 6564 4e72 0100 0000 290b 7230  llowedNr....).r0
+00003b10: 0000 00da 0373 6574 724e 0000 0072 1d00  .....setrN...r..
+00003b20: 0000 da05 6973 6e61 6e72 2300 0000 72b9  ....isnanr#...r.
+00003b30: 0000 0072 8500 0000 7289 0000 0072 2200  ...r....r....r".
+00003b40: 0000 da0f 696e 6465 785f 7769 7468 5f6e  ....index_with_n
+00003b50: 616e 7329 075a 0d73 7263 5f64 6174 615f  ans).Z.src_data_
+00003b60: 696e 6473 5a12 6461 7461 5f74 6f5f 6d61  indsZ.data_to_ma
+00003b70: 7463 685f 696e 6473 722a 0000 005a 0a6d  tch_indsr*...Z.m
+00003b80: 6174 6368 5f69 6e64 7372 3300 0000 7253  atch_indsr3...rS
+00003b90: 0000 0072 9300 0000 7216 0000 0072 1600  ...r....r....r..
+00003ba0: 0000 7217 0000 00da 1869 6e74 6572 7365  ..r......interse
+00003bb0: 6374 5f64 6174 615f 7769 7468 5f6e 616e  ct_data_with_nan
+00003bc0: 73bf 0100 0073 2000 0000 0024 1c01 0801  s....s ....$....
+00003bd0: 06ff 0801 02ff 0402 0801 0401 0401 0801  ................
+00003be0: 1201 0801 2002 0e01 0a01 72e0 0000 0063  .... .....r....c
+00003bf0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00003c00: 0300 0000 0300 0000 7312 0000 0087 0066  ........s......f
+00003c10: 0164 0164 0284 087c 0144 0083 0153 0029  .d.d...|.D...S.)
+00003c20: 034e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00003c30: 0000 0005 0000 0013 0000 0073 2800 0000  ...........s(...
+00003c40: 6700 7c00 5d20 7d01 7400 a001 7c01 a101  g.|.] }.t...|...
+00003c50: 7218 7400 6a02 6e0a 8800 7403 7c01 8301  r.t.j.n...t.|...
+00003c60: 1900 9102 7104 5300 7216 0000 0029 0472  ....q.S.r....).r
+00003c70: 1d00 0000 72de 0000 0072 2200 0000 7288  ....r....r"...r.
+00003c80: 0000 0072 3100 0000 72d1 0000 0072 1600  ...r1...r....r..
+00003c90: 0000 7217 0000 0072 3400 0000 1302 0000  ..r....r4.......
+00003ca0: 7304 0000 0006 0002 007a 2369 6e64 6578  s........z#index
+00003cb0: 5f77 6974 685f 6e61 6e73 2e3c 6c6f 6361  _with_nans.<loca
+00003cc0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7216  ls>.<listcomp>r.
+00003cd0: 0000 0029 0272 5300 0000 722b 0000 0072  ...).rS...r+...r
+00003ce0: 1600 0000 72d1 0000 0072 1700 0000 72df  ....r....r....r.
+00003cf0: 0000 0012 0200 0073 0200 0000 0001 72df  .......s......r.
+00003d00: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003d10: 0700 0000 0500 0000 4300 0000 734e 0000  ........C...sN..
+00003d20: 0074 006a 017c 007c 0164 0164 028d 035c  .t.j.|.|.d.d...\
+00003d30: 037d 027d 037d 0474 00a0 027c 00a1 0174  .}.}.}.t...|...t
+00003d40: 006a 0314 007d 057c 037c 057c 033c 0074  .j...}.|.|.|.<.t
+00003d50: 00a0 027c 01a1 0174 006a 0314 007d 067c  ...|...t.j...}.|
+00003d60: 047c 067c 043c 007c 057c 0666 0253 0029  .|.|.<.|.|.f.S.)
+00003d70: 034e 5429 01da 0e72 6574 7572 6e5f 696e  .NT)...return_in
+00003d80: 6469 6365 7329 0472 1d00 0000 da0b 696e  dices).r......in
+00003d90: 7465 7273 6563 7431 6472 4f00 0000 7222  tersect1drO...r"
+00003da0: 0000 0029 07da 0461 7272 31da 0461 7272  ...)...arr1..arr
+00003db0: 32da 0161 7242 0000 00da 0163 7243 0000  2..arB.....crC..
+00003dc0: 00da 0263 3272 1600 0000 7216 0000 0072  ...c2r....r....r
+00003dd0: 1700 0000 da13 696e 7465 7273 6563 745f  ......intersect_
+00003de0: 7769 7468 5f6e 616e 7316 0200 0073 0c00  with_nans....s..
+00003df0: 0000 0001 1601 1001 0801 1001 0801 72e8  ..............r.
+00003e00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00003e10: 0400 0000 0800 0000 4300 0000 7362 0000  ........C...sb..
+00003e20: 0074 00a0 017c 00a1 01a0 0274 03a1 017d  .t...|.....t...}
+00003e30: 007c 0074 00a0 047c 00a1 0138 007d 0074  .|.t...|...8.}.t
+00003e40: 00a0 0574 00a0 0674 077c 0083 01a1 0164  ...t...t.|.....d
+00003e50: 0174 00a0 0674 077c 0083 01a1 0114 0066  .t...t.|.......f
+00003e60: 02a1 017d 0174 006a 087c 007c 0164 0264  ...}.t.j.|.|.d.d
+00003e70: 038d 037d 0274 00a0 097c 02a1 017d 037c  ...}.t...|...}.|
+00003e80: 0353 0029 044e 724a 0000 00da 0576 616c  .S.).NrJ.....val
+00003e90: 6964 a901 da04 6d6f 6465 290a 721d 0000  id....mode).r...
+00003ea0: 0072 3800 0000 7285 0000 0072 8900 0000  .r8...r....r....
+00003eb0: da07 6176 6572 6167 65da 0668 7374 6163  ..average..hstac
+00003ec0: 6b72 3600 0000 7230 0000 00da 0863 6f6e  kr6...r0.....con
+00003ed0: 766f 6c76 65da 0661 7267 6d61 7829 0472  volve..argmax).r
+00003ee0: 5300 0000 da04 7374 6570 5a09 6461 7279  S.....stepZ.dary
+00003ef0: 5f73 7465 705a 0973 7465 705f 696e 6478  _stepZ.step_indx
+00003f00: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00003f10: 0f66 696e 645f 7374 6570 5f6f 6e73 6574  .find_step_onset
+00003f20: 1f02 0000 730c 0000 0000 0110 010e 0126  ....s..........&
+00003f30: 0110 010a 0172 f100 0000 6302 0000 0000  .....r....c.....
+00003f40: 0000 0000 0000 0007 0000 000a 0000 0043  ...............C
+00003f50: 0000 0073 9e00 0000 7400 7c00 6401 6402  ...s....t.|.d.d.
+00003f60: 8d02 7d00 7c01 6403 6b08 7224 7401 7c00  ..}.|.d.k.r$t.|.
+00003f70: 6404 1900 8301 0100 6403 5300 7402 7c00  d.......d.S.t.|.
+00003f80: 8301 4400 5d6c 5c02 7d02 7d03 7403 a004  ..D.]l\.}.}.t...
+00003f90: 7c03 6405 a102 8f52 7d04 7a14 7c04 7c01  |.d....R}.z.|.|.
+00003fa0: 1900 6403 6403 8502 1900 7d05 5700 6e14  ..d.d.....}.W.n.
+00003fb0: 0100 0100 0100 7c04 7c01 1900 7d05 5900  ......|.|...}.Y.
+00003fc0: 6e02 5800 7c02 6404 6b02 7280 7405 a006  n.X.|.d.k.r.t...
+00003fd0: 7c05 a101 7d06 6e0e 7405 a007 7c06 7c05  |...}.n.t...|.|.
+00003fe0: 6602 a101 7d06 5700 3500 5100 5200 5800  f...}.W.5.Q.R.X.
+00003ff0: 712c 7c06 5300 2906 7ab6 0a20 2020 2050  q,|.S.).z..    P
+00004000: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00004010: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2068 355f  --------.    h5_
+00004020: 6c69 7374 203a 206c 6973 740a 2020 2020  list : list.    
+00004030: 2020 2020 6c69 7374 206f 6620 6675 6c6c      list of full
+00004040: 2070 6174 6873 2074 6f20 4835 2066 696c   paths to H5 fil
+00004050: 6528 7329 2e0a 2020 2020 6b65 795f 6e61  e(s)..    key_na
+00004060: 6d65 203a 2073 7472 0a20 2020 2020 2020  me : str.       
+00004070: 2064 6566 6175 6c74 2027 6c61 6265 6c73   default 'labels
+00004080: 272c 2074 6865 206b 6579 2074 6f20 6765  ', the key to ge
+00004090: 7420 7468 6520 6461 7461 2066 726f 6d20  t the data from 
+000040a0: 7468 6520 4835 2066 696c 650a 2020 2020  the H5 file.    
+000040b0: 5472 5500 0000 4e72 0100 0000 726d 0000  TrU...Nr....rm..
+000040c0: 0029 0872 5700 0000 72ab 0000 0072 2400  .).rW...r....r$.
+000040d0: 0000 72ae 0000 0072 af00 0000 721d 0000  ..r....r....r...
+000040e0: 0072 3800 0000 7226 0000 0029 0772 5000  .r8...r&...).rP.
+000040f0: 0000 5a08 6b65 795f 6e61 6d65 722c 0000  ..Z.key_namer,..
+00004100: 0072 3300 0000 72c0 0000 0072 5300 0000  .r3...r....rS...
+00004110: 7293 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00004120: 1700 0000 724d 0000 0028 0200 0073 1c00  ....rM...(...s..
+00004130: 0000 000a 0c01 0801 0c01 0401 1001 0e01  ................
+00004140: 0201 1401 0601 0e02 0801 0c02 1a01 724d  ..............rM
+00004150: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00004160: 1100 0000 0700 0000 4300 0000 737a 0100  ........C...sz..
+00004170: 0074 0074 017c 0164 0183 0283 017d 0274  .t.t.|.d.....}.t
+00004180: 027c 0283 0174 0274 03a0 047c 02a1 0183  .|...t.t...|....
+00004190: 016b 0273 2c74 0564 0283 0182 0174 017c  .k.s,t.d.....t.|
+000041a0: 0164 0383 027d 0374 067c 0383 017d 0474  .d...}.t.|...}.t
+000041b0: 017c 0164 0483 027d 0574 077c 0064 0519  .|.d...}.t.|.d..
+000041c0: 0083 0167 0174 077c 0064 0619 0083 0114  ...g.t.|.d......
+000041d0: 007d 067c 0064 0719 0064 0819 007d 0774  .}.|.d...d...}.t
+000041e0: 03a0 0864 0964 0a84 007c 0064 0b19 0044  ...d.d...|.d...D
+000041f0: 0083 01a1 017d 0874 036a 097c 0864 0c19  .....}.t.j.|.d..
+00004200: 007c 0864 0d19 0067 0264 0e64 0f8d 027d  .|.d...g.d.d...}
+00004210: 097a 1c74 0a7c 077c 0474 03a0 0b74 027c  .z.t.|.|.t...t.|
+00004220: 0783 01a1 0164 108d 037d 0a57 006e 2001  .....d...}.W.n .
+00004230: 0001 0001 0074 0c64 1183 0101 0064 1273  .....t.d.....d.s
+00004240: d874 0564 1383 0182 0159 006e 0258 0067  .t.d.....Y.n.X.g
+00004250: 007d 0b74 03a0 0874 0d7c 0564 1483 02a1  .}.t...t.|.d....
+00004260: 017d 0c74 03a0 0874 0d7c 0664 1483 02a1  .}.t...t.|.d....
+00004270: 017d 0d74 0e7c 0a83 0144 005d 605c 027d  .}.t.|...D.]`\.}
+00004280: 0e7d 0f74 03a0 0f7c 0fa1 0190 0173 3c7c  .}.t...|.....s<|
+00004290: 097c 0d64 0e7c 0f66 0219 007c 0d64 147c  .|.d.|.f...|.d.|
+000042a0: 0f66 0219 0085 0219 007d 106e 2274 03a0  .f.......}.n"t..
+000042b0: 107c 0c64 147c 0e66 0219 007c 0c64 0e7c  .|.d.|.f...|.d.|
+000042c0: 0e66 0219 0018 00a1 0164 1514 007d 107c  .f.......d...}.|
+000042d0: 0ba0 117c 10a1 0101 0090 0171 0a74 03a0  ...|.......q.t..
+000042e0: 127c 0ba1 017d 0b7c 0b53 0029 167a 760a  .|...}.|.S.).zv.
+000042f0: 2020 2020 4920 7468 696e 6b20 7468 6973      I think this
+00004300: 2069 7320 7468 6520 776f 726b 696e 6720   is the working 
+00004310: 7665 7273 696f 6e0a 2020 2020 5061 7261  version.    Para
+00004320: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00004330: 2d2d 2d2d 2d0a 2020 2020 6320 3a0a 2020  -----.    c :.  
+00004340: 2020 6835 203a 0a0a 2020 2020 5265 7475    h5 :..    Retu
+00004350: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00004360: 0a20 2020 2072 9700 0000 fa75 796f 7572  .    r.....uyour
+00004370: 2068 3520 6669 6c65 2068 6173 2064 7570   h5 file has dup
+00004380: 6c69 6361 7465 2076 6964 656f 2066 696c  licate video fil
+00004390: 6573 2074 6861 7420 6974 2070 726f 6365  es that it proce
+000043a0: 7373 6564 2c20 796f 7520 7769 6c6c 2068  ssed, you will h
+000043b0: 6176 6520 746f 2063 7265 6174 6520 6120  ave to create a 
+000043c0: 6e65 7720 4835 2066 696c 6520 616e 6420  new H5 file and 
+000043d0: 7374 6172 7420 6f76 6572 2c20 736f 7272  start over, sorr
+000043e0: 79da 0e66 696c 655f 6e61 6d65 5f6e 756d  y..file_name_num
+000043f0: 7372 4100 0000 da01 7472 3300 0000 da04  srA.....tr3.....
+00004400: 6d65 7461 da0d 7573 6564 5472 6961 6c4e  meta..usedTrialN
+00004410: 756d 7363 0100 0000 0000 0000 0000 0000  umsc............
+00004420: 0200 0000 0400 0000 5300 0000 7316 0000  ........S...s...
+00004430: 0067 007c 005d 0e7d 017c 016a 00a0 01a1  .g.|.].}.|.j....
+00004440: 0091 0271 0453 0072 1600 0000 a902 da01  ...q.S.r........
+00004450: 54da 0766 6c61 7474 656e a902 7232 0000  T..flatten..r2..
+00004460: 00da 0474 6d70 3172 1600 0000 7216 0000  ...tmp1r....r...
+00004470: 0072 1700 0000 7234 0000 008c 0200 0073  .r....r4.......s
+00004480: 0400 0000 0600 0200 7a31 5561 7272 6179  ........z1Uarray
+00004490: 5f63 656c 6c5f 6c61 6265 6c73 5f74 6f5f  _cell_labels_to_
+000044a0: 4835 5f66 696c 652e 3c6c 6f63 616c 733e  H5_file.<locals>
+000044b0: 2e3c 6c69 7374 636f 6d70 3eda 0553 5f63  .<listcomp>..S_c
+000044c0: 746b e90a 0000 00e9 0d00 0000 7201 0000  tk..........r...
+000044d0: 00a9 01da 0461 7869 73a9 0172 2a00 0000  .....axis..r*...
+000044e0: 7a94 6920 6368 616e 6765 6420 6162 6f76  z.i changed abov
+000044f0: 6520 636f 6465 2074 6869 7320 6973 206a  e code this is j
+00004500: 7573 7420 696e 2063 6173 6520 6974 2066  ust in case it f
+00004510: 6169 6c73 2c20 796f 7520 6361 6e20 6368  ails, you can ch
+00004520: 616e 6765 2074 6865 2061 626f 7665 206c  ange the above l
+00004530: 696e 6520 2264 6174 613d 6e70 2e61 7261  ine "data=np.ara
+00004540: 6e67 6528 6c65 6e28 685f 7472 6961 6c73  nge(len(h_trials
+00004550: 2929 2220 746f 2022 6461 7461 3d6e 702e  ))" to "data=np.
+00004560: 6172 616e 6765 286c 656e 2877 5f74 7269  arange(len(w_tri
+00004570: 616c 7329 2922 467a 1973 6565 2061 626f  als))"Fz.see abo
+00004580: 7665 2070 7269 6e74 6564 206d 6573 7361  ve printed messa
+00004590: 6765 722e 0000 0072 4a00 0000 2913 72b3  ger....rJ...).r.
+000045a0: 0000 0072 4d00 0000 7230 0000 0072 1d00  ...rM...r0...r..
+000045b0: 0000 72d2 0000 0072 4e00 0000 728e 0000  ..r....rN...r...
+000045c0: 0072 8800 0000 7238 0000 00da 066e 616e  .r....r8.....nan
+000045d0: 7375 6d72 e000 0000 72b4 0000 0072 4b00  sumr....r....rK.
+000045e0: 0000 7237 0000 0072 2400 0000 72de 0000  ..r7...r$...r...
+000045f0: 0072 3600 0000 7223 0000 0072 2600 0000  .r6...r#...r&...
+00004600: 2911 72e6 0000 0072 5100 0000 7297 0000  ).r....rQ...r...
+00004610: 00da 0f77 5f74 7269 616c 735f 6672 616d  ...w_trials_fram
+00004620: 6573 da08 775f 7472 6961 6c73 da0c 775f  es..w_trials..w_
+00004630: 6672 616d 655f 6e75 6d73 da0c 685f 6672  frame_nums..h_fr
+00004640: 616d 655f 6e75 6d73 da08 685f 7472 6961  ame_nums..h_tria
+00004650: 6c73 72fc 0000 005a 0868 5f6c 6162 656c  lsr....Z.h_label
+00004660: 735a 1969 6e64 5f68 756d 616e 5f74 6f5f  sZ.ind_human_to_
+00004670: 7768 6163 635f 7472 6961 6c73 5a1c 6d61  whacc_trialsZ.ma
+00004680: 7463 6869 6e67 5f6c 6162 656c 735f 666f  tching_labels_fo
+00004690: 725f 7768 6163 635f 6835 da04 775f 666e  r_whacc_h5..w_fn
+000046a0: da04 685f 666e 722c 0000 0072 3300 0000  ..h_fnr,...r3...
+000046b0: 7253 0000 0072 1600 0000 7216 0000 0072  rS...r....r....r
+000046c0: 1700 0000 da1d 5561 7272 6179 5f63 656c  ......Uarray_cel
+000046d0: 6c5f 6c61 6265 6c73 5f74 6f5f 4835 5f66  l_labels_to_H5_f
+000046e0: 696c 6577 0200 0073 4000 0000 000c 0e01  ilew...s@.......
+000046f0: 0c01 02ff 0a01 02ff 0402 0a01 0801 0a02  ................
+00004700: 1a01 0c01 1801 1a01 0201 0a01 06ff 0c02  ................
+00004710: 0601 0201 02ff 0402 1202 0401 1001 1002  ................
+00004720: 1001 0c01 1e02 2201 0e01 0a01 720a 0100  ......".....r...
+00004730: 0063 0300 0000 0000 0000 0000 0000 1100  .c..............
+00004740: 0000 0700 0000 4300 0000 734c 0100 0074  ......C...sL...t
+00004750: 007c 0274 0183 0272 1474 027c 017c 0283  .|.t...r.t.|.|..
+00004760: 0201 0074 0374 027c 0164 0183 0283 017d  ...t.t.|.d.....}
+00004770: 0374 047c 0383 0174 0474 05a0 067c 03a1  .t.|...t.t...|..
+00004780: 0183 016b 0273 4074 0764 0283 0182 0174  ...k.s@t.d.....t
+00004790: 027c 0164 0383 027d 0474 087c 0483 017d  .|.d...}.t.|...}
+000047a0: 0574 027c 0164 0483 027d 0674 097c 0064  .t.|.d...}.t.|.d
+000047b0: 0519 0083 0167 0174 097c 0064 0619 0083  .....g.t.|.d....
+000047c0: 0114 007d 077c 0064 0719 0064 0819 007d  ...}.|.d...d...}
+000047d0: 0874 05a0 0a64 0964 0a84 007c 0064 0b19  .t...d.d...|.d..
+000047e0: 0044 0083 01a1 017d 0974 0b7c 057c 0874  .D.....}.t.|.|.t
+000047f0: 05a0 0c74 047c 0583 01a1 0164 0c8d 037d  ...t.|.....d...}
+00004800: 0a67 007d 0b74 05a0 0a74 0d7c 0664 0d83  .g.}.t...t.|.d..
+00004810: 02a1 017d 0c74 05a0 0a74 0d7c 0764 0d83  ...}.t...t.|.d..
+00004820: 02a1 017d 0d74 0e7c 0a83 0144 005d 5e5c  ...}.t.|...D.]^\
+00004830: 027d 0e7d 0f74 05a0 0f7c 0fa1 0190 0173  .}.}.t...|.....s
+00004840: 107c 027c 0c64 0e7c 0f66 0219 007c 0c64  .|.|.d.|.f...|.d
+00004850: 0d7c 0f66 0219 0085 0219 007d 106e 2274  .|.f.......}.n"t
+00004860: 05a0 107c 0d64 0d7c 0e66 0219 007c 0d64  ...|.d.|.f...|.d
+00004870: 0e7c 0e66 0219 0018 00a1 0164 0f14 007d  .|.f.......d...}
+00004880: 107c 0ba0 117c 10a1 0101 0071 de74 05a0  .|...|.....q.t..
+00004890: 127c 0ba1 017d 0b7c 0b53 0029 104e 7297  .|...}.|.S.).Nr.
+000048a0: 0000 0072 f200 0000 72f3 0000 0072 4100  ...r....r....rA.
+000048b0: 0000 72f4 0000 0072 3300 0000 72f5 0000  ..r....r3...r...
+000048c0: 0072 f600 0000 6301 0000 0000 0000 0000  .r....c.........
+000048d0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+000048e0: 1600 0000 6700 7c00 5d0e 7d01 7c01 6a00  ....g.|.].}.|.j.
+000048f0: a001 a100 9102 7104 5300 7216 0000 0072  ......q.S.r....r
+00004900: f700 0000 72fa 0000 0072 1600 0000 7216  ....r....r....r.
+00004910: 0000 0072 1700 0000 7234 0000 00b1 0200  ...r....r4......
+00004920: 0073 0400 0000 0600 0200 7a26 6835 5f74  .s........z&h5_t
+00004930: 6f5f 555f 6172 7261 795f 6365 6c6c 2e3c  o_U_array_cell.<
+00004940: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00004950: 703e 72fc 0000 0072 0101 0000 722e 0000  p>r....r....r...
+00004960: 0072 0100 0000 724a 0000 0029 13da 0a69  .r....rJ...)...i
+00004970: 7369 6e73 7461 6e63 6572 ad00 0000 724d  sinstancer....rM
+00004980: 0000 0072 b300 0000 7230 0000 0072 1d00  ...r....r0...r..
+00004990: 0000 72d2 0000 0072 4e00 0000 728e 0000  ..r....rN...r...
+000049a0: 0072 8800 0000 7238 0000 0072 e000 0000  .r....r8...r....
+000049b0: 72b4 0000 0072 3700 0000 7224 0000 0072  r....r7...r$...r
+000049c0: de00 0000 7236 0000 0072 2300 0000 7226  ....r6...r#...r&
+000049d0: 0000 0029 1172 e600 0000 7251 0000 005a  ...).r....rQ...Z
+000049e0: 0877 5f6c 6162 656c 7372 9700 0000 7203  .w_labelsr....r.
+000049f0: 0100 0072 0401 0000 7205 0100 0072 0601  ...r....r....r..
+00004a00: 0000 7207 0100 0072 fc00 0000 5a19 696e  ..r....r....Z.in
+00004a10: 645f 7768 6163 635f 746f 5f68 756d 616e  d_whacc_to_human
+00004a20: 5f74 7269 616c 735a 186d 6174 6368 696e  _trialsZ.matchin
+00004a30: 675f 6c61 6265 6c73 5f66 6f72 5f63 656c  g_labels_for_cel
+00004a40: 6c72 0801 0000 7209 0100 0072 2c00 0000  lr....r....r,...
+00004a50: 7233 0000 0072 5300 0000 7216 0000 0072  r3...rS...r....r
+00004a60: 1600 0000 7217 0000 00da 1268 355f 746f  ....r......h5_to
+00004a70: 5f55 5f61 7272 6179 5f63 656c 6ca4 0200  _U_array_cell...
+00004a80: 0073 3200 0000 0001 0a01 0a01 0e01 0c01  .s2.............
+00004a90: 02ff 0a01 02ff 0403 0a01 0801 0a02 1a01  ................
+00004aa0: 0c01 1803 1802 0401 1001 1002 1001 0c01  ................
+00004ab0: 1e02 2201 0c01 0a01 720c 0100 0063 0200  ..".....r....c..
+00004ac0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00004ad0: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
+00004ae0: 007c 0183 0283 0153 00a9 014e 2902 7237  .|.....S...N).r7
+00004af0: 0000 00da 0e63 6875 6e6b 5f73 6567 6d65  .....chunk_segme
+00004b00: 6e74 73a9 0272 3c00 0000 da0a 6368 756e  nts..r<.....chun
+00004b10: 6b5f 7369 7a65 7216 0000 0072 1600 0000  k_sizer....r....
+00004b20: 7217 0000 00da 136c 6f6f 705f 7365 676d  r......loop_segm
+00004b30: 656e 745f 6368 756e 6b73 f802 0000 7302  ent_chunks....s.
+00004b40: 0000 0000 0172 1101 0000 6302 0000 0000  .....r....c.....
+00004b50: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00004b60: 0000 0073 2c00 0000 7c01 6701 7c00 7c01  ...s,...|.g.|.|.
+00004b70: 1a00 1400 7d02 7c00 7c01 1600 6401 6b04  ....}.|.|...d.k.
+00004b80: 7228 7c02 a000 7c00 7c01 1600 a101 0100  r(|...|.|.......
+00004b90: 7c02 5300 7219 0000 0029 0172 2300 0000  |.S.r....).r#...
+00004ba0: 2903 723c 0000 0072 1001 0000 7293 0000  ).r<...r....r...
+00004bb0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00004bc0: 720e 0100 00fc 0200 0073 0800 0000 0001  r........s......
+00004bd0: 0e01 0c01 0e01 720e 0100 0063 0200 0000  ......r....c....
+00004be0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00004bf0: 4300 0000 7318 0000 007c 007c 011a 0064  C...s....|.|...d
+00004c00: 017c 007c 0116 0064 026b 0414 0017 0053  .|.|...d.k.....S
+00004c10: 0029 034e 722e 0000 0072 0100 0000 7216  .).Nr....r....r.
+00004c20: 0000 0072 0f01 0000 7216 0000 0072 1600  ...r....r....r..
+00004c30: 0000 7217 0000 00da 0a6e 756d 5f63 6875  ..r......num_chu
+00004c40: 6e6b 7303 0300 0073 0200 0000 0001 7212  nks....s......r.
+00004c50: 0100 0063 0400 0000 0000 0000 0000 0000  ...c............
+00004c60: 0800 0000 0700 0000 4300 0000 7390 0000  ........C...s...
+00004c70: 0074 00a0 0174 027c 0164 0183 02a1 017c  .t...t.|.d.....|
+00004c80: 0217 007d 017c 0364 006b 0872 207c 027d  ...}.|.d.k.r |.}
+00004c90: 0374 00a0 0374 00a0 047c 02a1 0174 006a  .t...t...|...t.j
+00004ca0: 0514 007c 0074 00a0 047c 03a1 0174 006a  ...|.t...|...t.j
+00004cb0: 0514 0066 03a1 017d 0067 007d 047c 0144  ...f...}.g.}.|.D
+00004cc0: 005d 347d 0574 00a0 0664 027c 057c 0218  .]4}.t...d.|.|..
+00004cd0: 0067 02a1 017d 067c 057c 0317 0064 0317  .g...}.|.|...d..
+00004ce0: 007d 077c 04a0 077c 007c 067c 0785 0219  .}.|...|.|.|....
+00004cf0: 00a1 0101 0071 5074 00a0 017c 04a1 0153  .....qPt...|...S
+00004d00: 0029 044e 5472 0100 0000 722e 0000 0029  .).NTr....r....)
+00004d10: 0872 1d00 0000 7238 0000 0072 5700 0000  .r....r8...rW...
+00004d20: 7226 0000 0072 3600 0000 7222 0000 00da  r&...r6...r"....
+00004d30: 036d 6178 7223 0000 0029 0872 5300 0000  .maxr#...).rS...
+00004d40: 722b 0000 005a 0973 7461 7274 5f70 6164  r+...Z.start_pad
+00004d50: 5a07 656e 645f 7061 645a 0578 5f6f 7574  Z.end_padZ.x_out
+00004d60: 7233 0000 0072 3f00 0000 7240 0000 0072  r3...r?...r@...r
+00004d70: 1600 0000 7216 0000 0072 1700 0000 da0d  ....r....r......
+00004d80: 6375 745f 7769 7468 5f6e 616e 7307 0300  cut_with_nans...
+00004d90: 0073 1400 0000 0001 1401 0801 0401 2801  .s............(.
+00004da0: 0401 0801 1201 0c01 1401 7214 0100 0063  ..........r....c
+00004db0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00004dc0: 0500 0000 4300 0000 7380 0000 0074 007c  ....C...s....t.|
+00004dd0: 0083 017d 0074 0174 027c 0064 0119 0083  ...}.t.t.|.d....
+00004de0: 0183 0101 0064 0274 0374 027c 0064 0119  .....d.t.t.|.d..
+00004df0: 0083 0183 01a0 04a1 006b 0672 4874 0164  .........k.rHt.d
+00004e00: 0383 0101 0064 0464 0584 007c 0044 0083  .....d.d...|.D..
+00004e10: 017d 016e 3474 027c 0064 0119 0083 0174  .}.n4t.|.d.....t
+00004e20: 036b 0272 7074 0164 0683 0101 0064 0764  .k.rpt.d.....d.d
+00004e30: 0584 007c 0044 0083 017d 016e 0c74 0164  ...|.D...}.n.t.d
+00004e40: 0883 0101 007c 0053 007c 0153 0029 094e  .....|.S.|.S.).N
+00004e50: 7201 0000 00da 0562 7974 6573 7a25 4445  r......bytesz%DE
+00004e60: 434f 4445 2073 7769 7463 6869 6e67 2066  CODE switching f
+00004e70: 726f 6d20 6279 7465 7320 746f 2073 7472  rom bytes to str
+00004e80: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
+00004e90: 0200 0000 0600 0000 5300 0000 7318 0000  ........S...s...
+00004ea0: 0067 007c 005d 107d 017c 01a0 0064 0064  .g.|.].}.|...d.d
+00004eb0: 01a1 0291 0271 0453 00a9 02da 0561 7363  .....q.S.....asc
+00004ec0: 6969 da06 6967 6e6f 7265 2901 da06 6465  ii..ignore)...de
+00004ed0: 636f 6465 7231 0000 0072 1600 0000 7216  coder1...r....r.
+00004ee0: 0000 0072 1700 0000 7234 0000 0019 0300  ...r....r4......
+00004ef0: 0073 0400 0000 0600 0200 7a26 6835 5f73  .s........z&h5_s
+00004f00: 7472 696e 675f 7377 6974 6368 6572 2e3c  tring_switcher.<
+00004f10: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00004f20: 703e 7a25 454e 434f 4445 2073 7769 7463  p>z%ENCODE switc
+00004f30: 6869 6e67 2066 726f 6d20 7374 7269 6e67  hing from string
+00004f40: 2074 6f20 6279 7465 7363 0100 0000 0000   to bytesc......
+00004f50: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
+00004f60: 0000 7318 0000 0067 007c 005d 107d 017c  ..s....g.|.].}.|
+00004f70: 01a0 0064 0064 01a1 0291 0271 0453 0072  ...d.d.....q.S.r
+00004f80: 1601 0000 a901 da06 656e 636f 6465 7231  ........encoder1
+00004f90: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00004fa0: 0000 7234 0000 001c 0300 0073 0400 0000  ..r4.......s....
+00004fb0: 0600 0200 7a2b 6e6f 7420 6279 7465 7320  ....z+not bytes 
+00004fc0: 6f72 2073 7472 696e 6720 666f 726d 6174  or string format
+00004fd0: 2c20 7265 7475 726e 696e 6720 696e 7075  , returning inpu
+00004fe0: 7429 0572 5700 0000 724b 0000 00da 0474  t).rW...rK.....t
+00004ff0: 7970 6572 ad00 0000 da05 6c6f 7765 7229  yper......lower)
+00005000: 02da 076c 6973 745f 696e 7293 0000 0072  ...list_inr....r
+00005010: 1600 0000 7216 0000 0072 1700 0000 72b3  ....r....r....r.
+00005020: 0000 0014 0300 0073 1600 0000 0001 0801  .......s........
+00005030: 1001 1801 0801 1001 1001 0801 1002 0801  ................
+00005040: 0401 72b3 0000 00e9 1027 0000 da06 5948  ..r......'....YH
+00005050: 4154 5f5f 72d4 0000 0063 0500 0000 0000  AT__r....c......
+00005060: 0000 0000 0000 0f00 0000 0b00 0000 4300  ..............C.
+00005070: 0000 73c2 0000 0074 007c 0064 0183 0244  ..s....t.|.d...D
+00005080: 005d b27d 0574 017c 0583 017d 0674 007c  .].}.t.|...}.t.|
+00005090: 0164 0183 0244 005d 9a7d 0774 02a0 037c  .d...D.].}.t...|
+000050a0: 0764 02a1 028f 507d 0867 007d 0974 047c  .d....P}.g.}.t.|
+000050b0: 0864 0319 006a 0583 0164 0419 007d 0a74  .d...j...d...}.t
+000050c0: 067c 0a7c 0283 0244 005d 285c 027d 0b7d  .|.|...D.](\.}.}
+000050d0: 0c7c 0864 0319 007c 0b7c 0c85 0219 007d  .|.d...|.|.....}
+000050e0: 0d7c 09a0 077c 06a0 087c 0da1 01a1 0101  .|...|...|......
+000050f0: 0071 5257 0035 0051 0052 0058 0074 09a0  .qRW.5.Q.R.X.t..
+00005100: 0a7c 09a1 017d 097c 0374 0b6a 0ca0 0d7c  .|...}.|.t.j...|
+00005110: 05a1 01a0 0e64 05a1 0164 0419 0017 007c  .....d...d.....|
+00005120: 0417 007d 0e74 0f7c 077c 0e7c 0983 0301  ...}.t.|.|.|....
+00005130: 0071 2071 0a64 0053 0029 064e 5472 6d00  .q q.d.S.).NTrm.
+00005140: 0000 7249 0000 0072 0100 0000 da01 2e29  ..rI...r.......)
+00005150: 1072 5700 0000 7263 0000 0072 ae00 0000  .rW...rc...r....
+00005160: 72af 0000 0072 3900 0000 7221 0000 0072  r....r9...r!...r
+00005170: 1101 0000 7223 0000 0072 b200 0000 721d  ....r#...r....r.
+00005180: 0000 0072 2600 0000 725f 0000 0072 6100  ...r&...r_...ra.
+00005190: 0000 72a8 0000 0072 db00 0000 da10 6f76  ..r....r......ov
+000051a0: 6572 7772 6974 655f 6835 5f6b 6579 290f  erwrite_h5_key).
+000051b0: 5a08 6d6f 645f 6c69 7374 7250 0000 0072  Z.mod_listrP...r
+000051c0: 1001 0000 5a0c 6672 6f6e 745f 6170 7065  ....Z.front_appe
+000051d0: 6e64 5a0b 6261 636b 5f61 7070 656e 645a  ndZ.back_appendZ
+000051e0: 076d 6f64 5f73 7472 72bc 0000 0072 5100  .mod_strr....rQ.
+000051f0: 0000 72c0 0000 00da 0479 6861 74da 086c  ..r......yhat..l
+00005200: 656e 5f64 6174 6172 3f00 0000 7240 0000  en_datar?...r@..
+00005210: 00da 0266 64da 0977 7269 7465 5f6b 6579  ...fd..write_key
+00005220: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00005230: 1066 6f6f 5f70 7265 6469 6374 5f6d 6f64  .foo_predict_mod
+00005240: 7331 0300 0073 1800 0000 0001 0e01 0801  s1...s..........
+00005250: 0e01 0e01 0401 1201 1201 1001 1c01 0a01  ................
+00005260: 1e01 7227 0100 00da 0974 656d 705f 7968  ..r'.....temp_yh
+00005270: 6174 6304 0000 0000 0000 0000 0000 000b  atc.............
+00005280: 0000 000a 0000 0043 0000 0073 8a00 0000  .......C...s....
+00005290: 7400 7c01 8301 4400 5d7c 7d04 7401 a002  t.|...D.]|}.t...
+000052a0: 7c04 6401 a102 8f66 7d05 6700 7d06 7403  |.d....f}.g.}.t.
+000052b0: 7c05 6402 1900 6a04 8301 6403 1900 7d07  |.d...j...d...}.
+000052c0: 7405 7c07 7c03 8302 4400 5d28 5c02 7d08  t.|.|...D.](\.}.
+000052d0: 7d09 7c05 6402 1900 7c08 7c09 8502 1900  }.|.d...|.|.....
+000052e0: 7d0a 7c06 a006 7c00 a007 7c0a a101 a101  }.|...|...|.....
+000052f0: 0100 713a 7408 a009 7c06 a101 7d06 740a  ..q:t...|...}.t.
+00005300: 7c04 7c02 7c06 8303 0100 5700 3500 5100  |.|.|.....W.5.Q.
+00005310: 5200 5800 7108 6400 5300 2904 4e72 6d00  R.X.q.d.S.).Nrm.
+00005320: 0000 7249 0000 0072 0100 0000 290b da07  ..rI...r....)...
+00005330: 6765 745f 6835 7372 ae00 0000 72af 0000  get_h5sr....r...
+00005340: 0072 3900 0000 7221 0000 0072 1101 0000  .r9...r!...r....
+00005350: 7223 0000 0072 b200 0000 721d 0000 0072  r#...r....r....r
+00005360: 2500 0000 7222 0100 0029 0b72 bc00 0000  %...r"...).r....
+00005370: da06 6835 5f64 6972 7226 0100 0072 1001  ..h5_dirr&...r..
+00005380: 0000 7251 0000 0072 c000 0000 7223 0100  ..rQ...r....r#..
+00005390: 0072 2401 0000 723f 0000 0072 4000 0000  .r$...r?...r@...
+000053a0: 7225 0100 0072 1600 0000 7216 0000 0072  r%...r....r....r
+000053b0: 1700 0000 da0e 666f 6f5f 7072 6564 6963  ......foo_predic
+000053c0: 745f 7632 4003 0000 7312 0000 0000 010c  t_v2@...s.......
+000053d0: 010e 0104 0112 0112 0110 0112 010a 0172  ...............r
+000053e0: 2b01 0000 6303 0000 0000 0000 0000 0000  +...c...........
+000053f0: 0006 0000 0005 0000 0043 0000 0073 3400  .........C...s4.
+00005400: 0000 7400 7c01 8301 4400 5d26 7d03 7401  ..t.|...D.]&}.t.
+00005410: a002 7c03 6401 a102 7d04 7c00 a003 7c04  ..|.d...}.|...|.
+00005420: a101 7d05 7404 7c03 7c02 7c05 8303 0100  ..}.t.|.|.|.....
+00005430: 7108 6400 5300 2902 4e72 4900 0000 2905  q.d.S.).NrI...).
+00005440: 7229 0100 0072 0800 0000 da1a 6765 745f  r)...r......get_
+00005450: 6835 5f6b 6579 5f61 6e64 5f63 6f6e 6361  h5_key_and_conca
+00005460: 7465 6e61 7465 72b2 0000 0072 2201 0000  tenater....r"...
+00005470: 2906 72bc 0000 0072 2a01 0000 7226 0100  ).r....r*...r&..
+00005480: 0072 5100 0000 7225 0100 0072 2301 0000  .rQ...r%...r#...
+00005490: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+000054a0: 0b66 6f6f 5f70 7265 6469 6374 4c03 0000  .foo_predictL...
+000054b0: 7308 0000 0000 140c 010c 010a 0172 2d01  s............r-.
+000054c0: 0000 722e 0000 0063 0400 0000 0000 0000  ..r....c........
+000054d0: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
+000054e0: 7380 0100 0074 00a0 0174 00a0 027c 02a1  s....t...t...|..
+000054f0: 017c 0364 0118 0014 0064 021b 00a1 01a0  .|.d.....d......
+00005500: 0374 04a1 017d 0474 00a0 027c 02a1 017c  .t...}.t...|...|
+00005510: 0314 007d 0274 00a0 027c 006a 0564 0364  ...}.t...|.j.d.d
+00005520: 0285 0219 00a1 017d 057c 017c 0418 007d  .......}.|.|...}
+00005530: 017c 01a0 06a1 007d 067c 0174 00a0 027c  .|.....}.|.t...|
+00005540: 02a1 0117 007d 077c 07a0 06a1 007d 0864  .....}.|.....}.d
+00005550: 047c 017c 0164 046b 003c 0074 00a0 027c  .|.|.d.k.<.t...|
+00005560: 05a1 017c 077c 056b 0419 007c 077c 077c  ...|.|.k...|.|.|
+00005570: 056b 043c 007c 017c 0618 007d 097c 007c  .k.<.|.|...}.|.|
+00005580: 0164 0419 007c 0764 0419 0085 027c 0164  .d...|.d.....|.d
+00005590: 0119 007c 0764 0119 0085 0264 0566 0319  ...|.d.....d.f..
+000055a0: 00a0 0364 06a1 017d 0a74 077c 0a6a 0583  ...d...}.t.|.j..
+000055b0: 017d 0b7c 02a0 08a1 007c 0b64 0364 0285  .}.|.....|.d.d..
+000055c0: 023c 0074 006a 096a 0a64 077c 0b64 088d  .<.t.j.j.d.|.d..
+000055d0: 02a0 0364 06a1 017d 0c74 0b7c 0b83 0164  ...d...}.t.|...d
+000055e0: 026b 0490 0172 3e7c 0a7c 0c7c 0964 0419  .k...r>|.|.|.d..
+000055f0: 007c 0964 0419 007c 0a6a 0564 0419 0017  .|.d...|.j.d....
+00005600: 0085 027c 0964 0119 007c 0964 0119 007c  ...|.d...|.d...|
+00005610: 0a6a 0564 0119 0017 0085 0264 0566 033c  .j.d.......d.f.<
+00005620: 006e 387c 0a7c 0c7c 0964 0419 007c 0964  .n8|.|.|.d...|.d
+00005630: 0419 007c 0a6a 0564 0419 0017 0085 027c  ...|.j.d.......|
+00005640: 0964 0119 007c 0964 0119 007c 0a6a 0564  .d...|.d...|.j.d
+00005650: 0119 0017 0085 0266 023c 007c 0c7c 067c  .......f.<.|.|.|
+00005660: 0866 0353 0029 0961 b801 0000 5468 6973  .f.S.).a....This
+00005670: 2069 7320 616e 2061 6363 6573 736f 7279   is an accessory
+00005680: 2066 756e 6374 696f 6e20 746f 2074 7261   function to tra
+00005690: 636b 2074 6f20 696d 7072 6f76 6520 7472  ck to improve tr
+000056a0: 6163 6b69 6e67 2073 7065 6564 2e20 5468  acking speed. Th
+000056b0: 6973 2063 726f 7073 2074 6865 2069 6e69  is crops the ini
+000056c0: 7469 616c 206c 6172 6765 2069 6d61 6765  tial large image
+000056d0: 2069 6e74 6f20 6120 736d 616c 6c65 7220   into a smaller 
+000056e0: 6f6e 652c 2062 6173 6564 206f 6e20 7468  one, based on th
+000056f0: 6520 696e 666c 6174 696f 6e20 7261 7465  e inflation rate
+00005700: 2e0a 2020 2020 2020 2020 496e 666c 6174  ..        Inflat
+00005710: 696f 6e20 7261 7465 206f 6620 3320 3d20  ion rate of 3 = 
+00005720: 3320 7820 3320 7465 6d70 6c61 7465 2069  3 x 3 template i
+00005730: 6d61 6765 2073 697a 6520 6172 6f75 6e64  mage size around
+00005740: 2074 6865 2066 6972 7374 2067 7565 7373   the first guess
+00005750: 6564 2070 6f6c 6520 6c6f 6361 7469 6f6e  ed pole location
+00005760: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00005770: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00005780: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00005790: 2069 6d20 3a0a 0a20 2020 2020 2020 2063   im :..        c
+000057a0: 726f 705f 746f 705f 6c65 6674 203a 0a0a  rop_top_left :..
+000057b0: 2020 2020 2020 2020 7369 7a65 5f63 726f          size_cro
+000057c0: 7020 3a0a 0a20 2020 2020 2020 2069 6e66  p :..        inf
+000057d0: 6c61 7469 6f6e 203a 0a20 2020 2020 2020  lation :.       
+000057e0: 2020 2020 2020 2844 6566 6175 6c74 2076        (Default v
+000057f0: 616c 7565 203d 2033 290a 0a20 2020 2020  alue = 3)..     
+00005800: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00005810: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
+00005820: 2020 2020 722e 0000 0072 4700 0000 4e72      r....rG...Nr
+00005830: 0100 0000 2eda 0575 696e 7438 e900 0100  .......uint8....
+00005840: 0029 01da 0473 697a 6529 0c72 1d00 0000  .)...size).r....
+00005850: da05 666c 6f6f 7272 3800 0000 7285 0000  ..floorr8...r...
+00005860: 0072 8800 0000 7221 0000 0072 1b00 0000  .r....r!...r....
+00005870: 7239 0000 00da 0674 6f6c 6973 7472 1e00  r9.....tolistr..
+00005880: 0000 da07 7261 6e64 696e 7472 3000 0000  ....randintr0...
+00005890: 290d da02 696d 5a0d 6372 6f70 5f74 6f70  )...imZ.crop_top
+000058a0: 5f6c 6566 745a 0973 697a 655f 6372 6f70  _leftZ.size_crop
+000058b0: 5a09 696e 666c 6174 696f 6e5a 0f69 6e66  Z.inflationZ.inf
+000058c0: 6c61 7469 6f6e 5f73 6869 6674 5a07 696d  lation_shiftZ.im
+000058d0: 7368 6170 65da 0e63 726f 705f 746f 705f  shape..crop_top_
+000058e0: 6c65 6674 325a 1163 726f 705f 626f 7474  left2Z.crop_bott
+000058f0: 6f6d 5f72 6967 6874 da12 6372 6f70 5f62  om_right..crop_b
+00005900: 6f74 746f 6d5f 7269 6768 7432 5a06 544c  ottom_right2Z.TL
+00005910: 5f61 646a 5a09 635f 6372 6f70 7065 645a  _adjZ.c_croppedZ
+00005920: 0863 726f 705f 6469 6d5a 0d63 726f 7070  .crop_dimZ.cropp
+00005930: 6564 5f69 6d61 6765 7216 0000 0072 1600  ed_imager....r..
+00005940: 0000 7217 0000 00da 1863 726f 705f 696d  ..r......crop_im
+00005950: 6167 655f 6672 6f6d 5f74 6f70 5f6c 6566  age_from_top_lef
+00005960: 7466 0300 0073 3600 0000 0013 2202 0e01  tf...s6....."...
+00005970: 1403 0801 0801 0e01 0803 0c01 1a03 0802  ................
+00005980: 2601 02ff 0404 0a01 1001 1602 0e02 02ff  &...............
+00005990: 3201 02ff 0604 02ff 1a01 0600 10ff 0603  2...............
+000059a0: 7237 0100 0072 9a00 0000 6303 0000 0000  r7...r....c.....
+000059b0: 0000 0000 0000 0018 0000 000e 0000 0003  ................
+000059c0: 0000 0073 9201 0000 7400 a001 7c00 6401  ...s....t...|.d.
+000059d0: a102 7d03 7400 a001 7c00 6402 a102 7d04  ..}.t...|.d...}.
+000059e0: 7400 a001 7c00 6403 a102 7d05 7402 7c05  t...|.d...}.t.|.
+000059f0: 6a03 6400 6404 8502 1900 8301 7d06 8700  j.d.d.......}...
+00005a00: 6601 6405 6406 8408 7400 a001 7c00 6407  f.d.d...t...|.d.
+00005a10: a102 4400 8301 7d07 7400 6a04 7c00 6408  ..D...}.t.j.|.d.
+00005a20: 7c06 6409 1900 7c06 640a 1900 640b 640b  |.d...|.d...d.d.
+00005a30: 640b 6408 7405 6a06 6a07 7405 6a06 6a08  d.d.t.j.j.t.j.j.
+00005a40: 7c02 640c 640d 8d0c 7d08 7409 7c00 7c08  |.d.d...}.t.|.|.
+00005a50: 6a0a 8302 0100 7409 7c00 7c08 6a0b 8302  j.....t.|.|.j...
+00005a60: 0100 7409 7c00 640e 8302 0100 740c 740d  ..t.|.d.....t.t.
+00005a70: 740e 7c03 8301 740f 7c03 8301 640f 8d02  t.|...t.|...d...
+00005a80: 8301 4400 5dd0 5c02 7d09 5c02 7d0a 7d0b  ..D.].\.}.\.}.}.
+00005a90: 7c07 7c09 1900 7d0c 7410 a011 7c0c a101  |.|...}.t...|...
+00005aa0: 7d0d 7c04 7c0a 7c0b 8502 1900 7d0e 7c0d  }.|.|.|.....}.|.
+00005ab0: a012 a100 6408 6b02 72fa 7413 6410 8301  ....d.k.r.t.d...
+00005ac0: 0100 7414 7c0d a015 6411 a101 8301 7d0f  ..t.|...d.....}.
+00005ad0: 6700 7d10 7416 7c0f 8301 4400 5d50 7d11  g.}.t.|...D.]P}.
+00005ae0: 7c0d a017 7410 6a18 7c11 a102 0100 7c0d  |...t.j.|.....|.
+00005af0: a019 a100 5c02 7d12 7d13 7c0e 7c11 1900  ....\.}.}.|.|...
+00005b00: 7d14 741a 7c13 7c14 640a 1900 7c14 6409  }.t.|.|.d...|.d.
+00005b10: 1900 6702 7c06 8303 5c03 7d15 7d16 7d17  ..g.|...\.}.}.}.
+00005b20: 7c10 a01b 7c15 a101 0100 9001 7114 741c  |...|.......q.t.
+00005b30: a01d 7c10 a101 7d10 7c08 a01e 7c10 6412  ..|...}.|...|.d.
+00005b40: 741c a01f 7c10 6a03 6409 1900 a101 1400  t...|.j.d.......
+00005b50: a102 0100 71bc 6400 5300 2913 4e72 4100  ....q.d.S.).NrA.
+00005b60: 0000 7283 0000 0072 9600 0000 7247 0000  ..r....r....rG..
+00005b70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00005b80: 0000 0900 0000 1300 0000 732a 0000 0067  ..........s*...g
+00005b90: 007c 005d 227d 0188 0074 006a 0117 0074  .|.]"}...t.j...t
+00005ba0: 006a 02a0 037c 01a0 0464 0064 01a1 02a1  .j...|...d.d....
+00005bb0: 0117 0091 0271 0453 0072 1601 0000 2905  .....q.S.r....).
+00005bc0: 725f 0000 0072 6000 0000 7261 0000 0072  r_...r`...ra...r
+00005bd0: a800 0000 7219 0100 0072 3100 0000 a901  ....r....r1.....
+00005be0: da06 6d70 345f 6264 7216 0000 0072 1700  ..mp4_bdr....r..
+00005bf0: 0000 7234 0000 00a3 0300 0073 0400 0000  ..r4.......s....
+00005c00: 0600 0200 7a36 696e 7365 7274 5f69 6d61  ....z6insert_ima
+00005c10: 6765 735f 696e 746f 5f66 6561 7475 7265  ges_into_feature
+00005c20: 5f64 6174 615f 6835 2e3c 6c6f 6361 6c73  _data_h5.<locals
+00005c30: 3e2e 3c6c 6973 7463 6f6d 703e 7297 0000  >.<listcomp>r...
+00005c40: 0046 7201 0000 0072 2e00 0000 545a 0554  .Fr....r....TZ.T
+00005c50: 5241 5348 290b da18 6f76 6572 7772 6974  RASH)...overwrit
+00005c60: 655f 6966 5f66 696c 655f 6578 6973 7473  e_if_file_exists
+00005c70: da0e 6d61 785f 696d 675f 6865 6967 6874  ..max_img_height
+00005c80: da0d 6d61 785f 696d 675f 7769 6474 68da  ..max_img_width.
+00005c90: 2063 6c6f 7365 5f61 6e64 5f6f 7065 6e5f   close_and_open_
+00005ca0: 6f6e 5f65 6163 685f 6974 6572 6174 696f  on_each_iteratio
+00005cb0: 6eda 0d63 6f6c 6f72 5f63 6861 6e6e 656c  n..color_channel
+00005cc0: da12 6164 645f 746f 5f65 7869 7374 696e  ..add_to_existin
+00005cd0: 675f 4835 da1a 6967 6e6f 7265 5f69 6d61  g_H5..ignore_ima
+00005ce0: 6765 5f72 616e 6765 5f77 6172 6e69 6e67  ge_range_warning
+00005cf0: da09 6474 7970 655f 696d 67da 0c64 7479  ..dtype_img..dty
+00005d00: 7065 5f6c 6162 656c 73da 0e69 6d61 6765  pe_labels..image
+00005d10: 5f6b 6579 5f6e 616d 65da 0e6c 6162 656c  _key_name..label
+00005d20: 5f6b 6579 5f6e 616d 65da 0a6d 756c 7469  _key_name..multi
+00005d30: 706c 6965 72a9 01da 0574 6f74 616c 7a18  plier....totalz.
+00005d40: 6572 726f 7220 6f70 656e 696e 6720 7669  error opening vi
+00005d50: 6465 6f20 6669 6c65 7245 0000 0072 4a00  deo filerE...rJ.
+00005d60: 0000 2920 7208 0000 0072 2c01 0000 7239  ..) r....r,...r9
+00005d70: 0000 0072 2100 0000 da14 6835 5f69 7465  ...r!.....h5_ite
+00005d80: 7261 7469 7665 5f63 7265 6174 6f72 72ae  rative_creatorr.
+00005d90: 0000 00da 0368 3574 da08 5354 445f 5538  .....h5t..STD_U8
+00005da0: 4245 da09 5354 445f 4933 324c 45da 0a64  BE..STD_I32LE..d
+00005db0: 656c 5f68 355f 6b65 795a 0769 6d67 5f6b  el_h5_keyZ.img_k
+00005dc0: 6579 7244 0100 0072 2400 0000 720b 0000  eyrD...r$...r...
+00005dd0: 0072 3700 0000 7230 0000 0072 c600 0000  .r7...r0...r....
+00005de0: 72c7 0000 0072 c800 0000 724b 0000 0072  r....r....rK...r
+00005df0: 8800 0000 72c9 0000 0072 3a00 0000 72dd  ....r....r:...r.
+00005e00: 0000 005a 1343 4150 5f50 524f 505f 504f  ...Z.CAP_PROP_PO
+00005e10: 535f 4652 414d 4553 da04 7265 6164 7237  S_FRAMES..readr7
+00005e20: 0100 0072 2300 0000 721d 0000 0072 3800  ...r#...r....r8.
+00005e30: 0000 da09 6164 645f 746f 5f68 3572 3600  ....add_to_h5r6.
+00005e40: 0000 2918 7251 0000 0072 3901 0000 5a09  ..).rQ...r9...Z.
+00005e50: 696d 6167 655f 6b65 7972 4100 0000 7283  image_keyrA...r.
+00005e60: 0000 0072 9600 0000 5a08 696d 675f 7369  ...r....Z.img_si
+00005e70: 7a65 5a08 6d70 345f 6c69 7374 5a0a 6835  zeZ.mp4_listZ.h5
+00005e80: 5f63 7265 6174 6f72 722c 0000 0072 bd00  _creatorr,...r..
+00005e90: 0000 72be 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
+00005ea0: 005a 0c74 6d70 5f6c 6f63 6174 696f 6e72  .Z.tmp_locationr
+00005eb0: cc00 0000 729a 0000 00da 0266 6eda 0773  ....r......fn..s
+00005ec0: 7563 6365 7373 5a08 6f67 5f66 7261 6d65  uccessZ.og_frame
+00005ed0: da09 6c6f 6361 7469 6f6e 735a 0863 726f  ..locationsZ.cro
+00005ee0: 705f 696d 6772 3501 0000 7236 0100 0072  p_imgr5...r6...r
+00005ef0: 1600 0000 7238 0100 0072 1700 0000 da22  ....r8...r....."
+00005f00: 696e 7365 7274 5f69 6d61 6765 735f 696e  insert_images_in
+00005f10: 746f 5f66 6561 7475 7265 5f64 6174 615f  to_feature_data_
+00005f20: 6835 9d03 0000 7354 0000 0000 010c 020c  h5....sT........
+00005f30: 010c 0112 010a 010a ff06 0306 0102 0106  ................
+00005f40: 0106 0102 0102 0102 0102 0106 0106 0102  ................
+00005f50: 0102 f506 0d0c 010c 010a 0224 0108 010a  ...........$....
+00005f60: 010c 010c 0108 010e 0104 010c 010e 010c  ................
+00005f70: 0108 0104 010e 0102 fe0a 030e 010a 0172  ...............r
+00005f80: 5201 0000 6301 0000 0000 0000 0000 0000  R...c...........
+00005f90: 0001 0000 0002 0000 0043 0000 0073 1400  .........C...s..
+00005fa0: 0000 7400 7c00 8301 0100 7401 7c00 8301  ..t.|.....t.|...
+00005fb0: 0100 6400 5300 720d 0100 0029 0272 7400  ..d.S.r....).rt.
+00005fc0: 0000 72aa 0000 00a9 015a 0664 6972 5f69  ..r......Z.dir_i
+00005fd0: 6e72 1600 0000 7216 0000 0072 1700 0000  nr....r....r....
+00005fe0: da09 636c 6561 725f 6469 72cb 0300 0073  ..clear_dir....s
+00005ff0: 0400 0000 0001 0801 7254 0100 0063 0100  ........rT...c..
+00006000: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00006010: 0000 4300 0000 731a 0000 0074 006a 01a0  ..C...s....t.j..
+00006020: 027c 00a1 0172 1674 03a0 047c 00a1 0101  .|...r.t...|....
+00006030: 0064 0053 0072 0d01 0000 2905 725f 0000  .d.S.r....).r_..
+00006040: 0072 6100 0000 7262 0000 0072 7300 0000  .ra...rb...rs...
+00006050: 7274 0000 0072 5301 0000 7216 0000 0072  rt...rS...r....r
+00006060: 1600 0000 7217 0000 0072 7400 0000 d003  ....r....rt.....
+00006070: 0000 7304 0000 0000 010c 0172 7400 0000  ..s........rt...
+00006080: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+00006090: 0006 0000 0043 0000 0073 6a00 0000 6401  .....C...sj...d.
+000060a0: 7d02 7c01 6400 6b02 7212 7400 6a01 7d01  }.|.d.k.r.t.j.}.
+000060b0: 7c00 6402 1900 6403 6b02 732a 7c00 6402  |.d...d.k.s*|.d.
+000060c0: 1900 6404 6b02 722e 7c01 7d02 6404 a002  ..d.k.r.|.}.d...
+000060d0: 6405 6406 8400 7c00 a003 6403 a101 4400  d.d...|...d...D.
+000060e0: 8301 a101 7d03 6407 6406 8400 7c03 a003  ....}.d.d...|...
+000060f0: 6404 a101 4400 8301 7d04 7c02 7c01 a002  d...D...}.|.|...
+00006100: 7c04 a101 1700 5300 2908 4e72 d400 0000  |.....S.).Nr....
+00006110: 7201 0000 00fa 012f fa01 5c63 0100 0000  r....../..\c....
+00006120: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00006130: 5300 0000 731c 0000 0067 007c 005d 147d  S...s....g.|.].}
+00006140: 0174 007c 0183 0164 006b 0472 047c 0191  .t.|...d.k.r.|..
+00006150: 0271 0453 00a9 0172 0100 0000 7248 0000  .q.S...r....rH..
+00006160: 0072 3100 0000 7216 0000 0072 1600 0000  .r1...r....r....
+00006170: 7217 0000 0072 3400 0000 db03 0000 7306  r....r4.......s.
+00006180: 0000 0006 0002 000c 007a 1d6e 6f72 6d5f  .........z.norm_
+00006190: 7061 7468 2e3c 6c6f 6361 6c73 3e2e 3c6c  path.<locals>.<l
+000061a0: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+000061b0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+000061c0: 0073 1c00 0000 6700 7c00 5d14 7d01 7400  .s....g.|.].}.t.
+000061d0: 7c01 8301 6400 6b04 7204 7c01 9102 7104  |...d.k.r.|...q.
+000061e0: 5300 7257 0100 0072 4800 0000 7231 0000  S.rW...rH...r1..
+000061f0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00006200: 7234 0000 00dc 0300 0073 0600 0000 0600  r4.......s......
+00006210: 0200 0c00 2904 725f 0000 0072 6000 0000  ....).r_...r`...
+00006220: 72da 0000 0072 db00 0000 2905 da07 7061  r....r....)...pa
+00006230: 7468 5f69 6e72 6000 0000 5a09 6164 645f  th_inr`...Z.add_
+00006240: 7374 6172 745a 0874 6d70 5f6c 6973 745a  startZ.tmp_listZ
+00006250: 0a66 696e 616c 5f6c 6973 7472 1600 0000  .final_listr....
+00006260: 7216 0000 0072 1700 0000 729e 0000 00d5  r....r....r.....
+00006270: 0300 0073 1000 0000 0001 0401 0801 0601  ...s............
+00006280: 1801 0401 1a01 1401 729e 0000 0072 4900  ........r....rI.
+00006290: 0000 da0c 4644 5f5f 6f72 6967 696e 616c  ....FD__original
+000062a0: da08 434e 4e5f 7072 6564 6302 0000 0000  ..CNN_predc.....
+000062b0: 0000 0000 0000 0005 0000 0009 0000 0043  ...............C
+000062c0: 0000 0073 5800 0000 7400 8300 7d02 7c01  ...sX...t...}.|.
+000062d0: 6401 6b08 7212 6700 7d01 7401 a002 7c00  d.k.r.g.}.t...|.
+000062e0: 6402 a102 8f30 7d03 7c03 a003 a100 4400  d....0}.|.....D.
+000062f0: 5d20 7d04 7c04 7c01 6b07 7228 7c03 7c04  ] }.|.|.k.r(|.|.
+00006300: 1900 6401 6401 8502 1900 7c02 7c04 3c00  ..d.d.....|.|.<.
+00006310: 7128 5700 3500 5100 5200 5800 7c02 5300  q(W.5.Q.R.X.|.S.
+00006320: 2903 7ab5 0a0a 2020 2020 5061 7261 6d65  ).z...    Parame
+00006330: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00006340: 2d2d 2d0a 2020 2020 6835 5f69 6e20 3a0a  ---.    h5_in :.
+00006350: 2020 2020 6578 636c 7564 655f 6b65 7973      exclude_keys
+00006360: 203a 2062 7920 6465 6661 756c 7420 6578   : by default ex
+00006370: 636c 7564 6573 2061 6c6c 2074 6865 2061  cludes all the a
+00006380: 6c72 6765 2064 6174 6120 696e 2074 6865  lrge data in the
+00006390: 2048 3520 6669 6c65 2c20 7365 7420 746f   H5 file, set to
+000063a0: 2022 5b5d 2220 746f 2067 6574 2074 6865   "[]" to get the
+000063b0: 2065 6e74 6972 6520 4835 0a0a 2020 2020   entire H5..    
+000063c0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+000063d0: 2d2d 2d0a 0a20 2020 204e 726d 0000 0029  ---..    Nrm...)
+000063e0: 0472 6900 0000 72ae 0000 0072 af00 0000  .ri...r....r....
+000063f0: 7299 0000 0029 0572 c200 0000 5a0c 6578  r....).r....Z.ex
+00006400: 636c 7564 655f 6b65 7973 726b 0000 0072  clude_keysrk...r
+00006410: c000 0000 7233 0000 0072 1600 0000 7216  ....r3...r....r.
+00006420: 0000 0072 1700 0000 da0a 6835 5f74 6f5f  ...r......h5_to_
+00006430: 6469 6374 e003 0000 7310 0000 0000 0c06  dict....s.......
+00006440: 0108 0104 010e 010c 0108 0120 0172 5b01  ........... .r[.
+00006450: 0000 da04 7361 6d65 6303 0000 0000 0000  ....samec.......
+00006460: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+00006470: 0073 2e00 0000 7c01 6401 6b02 720c 7c00  .s....|.d.k.r.|.
+00006480: 5300 7400 a001 7c01 a101 7c01 1b00 7d03  S.t...|...|...}.
+00006490: 7400 6a02 7c00 7c03 7c02 6402 8d03 7d04  t.j.|.|.|.d...}.
+000064a0: 7c04 5300 2903 4e72 2e00 0000 72ea 0000  |.S.).Nr....r...
+000064b0: 0029 0372 1d00 0000 7236 0000 0072 ee00  .).r....r6...r..
+000064c0: 0000 2905 72bf 0000 00da 0677 696e 646f  ..).r......windo
+000064d0: 7772 eb00 0000 da03 626f 785a 0879 5f73  wr......boxZ.y_s
+000064e0: 6d6f 6f74 6872 1600 0000 7216 0000 0072  moothr....r....r
+000064f0: 1700 0000 72b1 0000 00f6 0300 0073 0a00  ....r........s..
+00006500: 0000 0001 0801 0401 0e01 1001 72b1 0000  ............r...
+00006510: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00006520: 0000 0400 0000 4300 0000 7316 0000 0074  ......C...s....t
+00006530: 007c 0083 016a 0164 0164 0164 028d 0201  .|...j.d.d.d....
+00006540: 0064 0053 00a9 034e 54a9 02da 0770 6172  .d.S...NT....par
+00006550: 656e 7473 da08 6578 6973 745f 6f6b 2902  ents..exist_ok).
+00006560: 720e 0000 00da 056d 6b64 6972 2901 5a07  r......mkdir).Z.
+00006570: 6e61 6d65 5f69 6e72 1600 0000 7216 0000  name_inr....r...
+00006580: 0072 1700 0000 72aa 0000 00fe 0300 0073  .r....r........s
+00006590: 0200 0000 0001 72aa 0000 0063 0100 0000  ......r....c....
+000065a0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000065b0: 4300 0000 7314 0000 0074 007c 0074 016a  C...s....t.|.t.j
+000065c0: 0274 016a 0342 0064 018d 0253 0029 024e  .t.j.B.d...S.).N
+000065d0: 2901 5a03 616c 6729 0472 0600 0000 7207  ).Z.alg).r....r.
+000065e0: 0000 00da 0546 4c4f 4154 5a08 554e 5349  .....FLOATZ.UNSI
+000065f0: 474e 4544 72d1 0000 0072 1600 0000 7216  GNEDr....r....r.
+00006600: 0000 0072 1700 0000 da04 736f 7274 0204  ...r......sort..
+00006610: 0000 7302 0000 0000 0172 6501 0000 6302  ..s......re...c.
+00006620: 0000 0000 0000 0000 0000 0005 0000 000b  ................
+00006630: 0000 0043 0000 0073 5600 0000 7c01 7400  ...C...sV...|.t.
+00006640: a001 7c01 a101 1b00 7d01 7402 7c00 8301  ..|.....}.t.|...
+00006650: 7d02 7400 6a03 6a04 7c02 7c02 6401 6402  }.t.j.j.|.|.d.d.
+00006660: 8d03 7d03 7400 a005 7c03 7400 a006 7c02  ..}.t...|.t...|.
+00006670: 7400 a007 7c01 6400 6403 8502 1900 a101  t...|.d.d.......
+00006680: 1400 a101 a008 6404 a101 a102 7d04 7c04  ......d.....}.|.
+00006690: 5300 2905 4e46 a901 72b7 0000 0072 4a00  S.).NF..r....rJ.
+000066a0: 0000 7288 0000 0029 0972 1d00 0000 7235  ..r....).r....r5
+000066b0: 0000 0072 3000 0000 721e 0000 0072 2000  ...r0...r....r .
+000066c0: 0000 72db 0000 00da 0463 6569 6cda 0663  ..r......ceil..c
+000066d0: 756d 7375 6d72 8500 0000 2905 7253 0000  umsumr....).rS..
+000066e0: 00da 0b73 706c 6974 5f72 6174 696f 72c4  ...split_ratior.
+000066f0: 0000 005a 0a6d 6978 6564 5f69 6e64 7372  ...Z.mixed_indsr
+00006700: 9300 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00006710: 0000 00da 0f73 706c 6974 5f6c 6973 745f  .....split_list_
+00006720: 696e 6473 0704 0000 730a 0000 0000 010e  inds....s.......
+00006730: 0108 0112 012a 0172 6a01 0000 6302 0000  .....*.rj...c...
+00006740: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+00006750: 0043 0000 0073 4200 0000 7400 7c00 7c01  .C...sB...t.|.|.
+00006760: 8302 7d02 6700 7d03 7c02 4400 5d2a 7d04  ..}.g.}.|.D.]*}.
+00006770: 6700 7d05 7c04 4400 5d12 7d06 7c05 a001  g.}.|.D.].}.|...
+00006780: 7c00 7c06 1900 a101 0100 711e 7c03 a001  |.|.......q.|...
+00006790: 7c05 a101 0100 7112 7c03 5300 720d 0100  |.....q.|.S.r...
+000067a0: 0029 0272 6a01 0000 7223 0000 0029 0772  .).rj...r#...).r
+000067b0: 5300 0000 7269 0100 0072 2b00 0000 7293  S...ri...r+...r.
+000067c0: 0000 0072 3300 0000 72fb 0000 0072 be00  ...r3...r....r..
+000067d0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000067e0: 00da 0a73 706c 6974 5f6c 6973 740f 0400  ...split_list...
+000067f0: 0073 1000 0000 0001 0a01 0401 0801 0401  .s..............
+00006800: 0801 1001 0c01 726b 0100 00da 0a79 6861  ......rk.....yha
+00006810: 745f 7072 6f62 6172 2301 0000 6306 0000  t_probar#...c...
+00006820: 0000 0000 0000 0000 000d 0000 000a 0000  ................
+00006830: 0043 0000 0073 ce00 0000 7400 7c00 8301  .C...s....t.|...
+00006840: 7d00 7401 a002 a100 7d06 7c01 6400 6b08  }.t.....}.|.d.k.
+00006850: 721e 7c06 6a03 7d01 7c00 4400 5da6 7d07  r.|.j.}.|.D.].}.
+00006860: 7404 7c07 8301 0100 7405 7c07 7c04 8302  t.|.....t.|.|...
+00006870: 7d08 7405 7c07 7c05 8302 7d09 7c03 7374  }.t.|.|...}.|.st
+00006880: 7c08 734e 7c09 7274 7406 a007 6401 7c07  |.sN|.rtt...d.|.
+00006890: 1700 6402 1700 7408 7c08 8301 1700 6403  ..d...t.|.....d.
+000068a0: 1700 7408 7c09 8301 1700 a101 0100 7409  ..t.|.........t.
+000068b0: a00a 7c07 6404 a102 8f42 7d0a 740b a00c  ..|.d....B}.t...
+000068c0: 7c07 6405 a102 7d0b 7c06 a00d 7c0b a101  |.d...}.|...|...
+000068d0: 7d0c 7c02 72be 740e 7c07 7c04 7c0c 8303  }.|.r.t.|.|.|...
+000068e0: 0100 740e 7c07 7c05 7c0c 7c01 6b04 a00f  ..t.|.|.|.|.k...
+000068f0: 7410 a101 8303 0100 5700 3500 5100 5200  t.......W.5.Q.R.
+00006900: 5800 7122 6400 5300 2906 4e7a 1d0a 4b45  X.q"d.S.).Nz..KE
+00006910: 5920 4558 4953 5453 204e 4f54 2057 5249  Y EXISTS NOT WRI
+00006920: 5454 494e 4720 464f 5220 7a32 0a6f 7665  TTING FOR z2.ove
+00006930: 7277 7269 7465 5f69 665f 6578 6973 7473  rwrite_if_exists
+00006940: 2069 7320 4641 4c53 450a 7072 6f62 615f   is FALSE.proba_
+00006950: 6b65 7920 6578 6973 7420 2d2d 3e20 7a16  key exist --> z.
+00006960: 0a6c 6162 656c 5f6b 6579 2065 7869 7374  .label_key exist
+00006970: 7320 2d2d 3e20 72a6 0000 0072 4900 0000  s --> r....rI...
+00006980: 2911 7257 0000 0072 0500 0000 72ac 0000  ).rW...r....r...
+00006990: 005a 1d46 494e 414c 5f54 4852 4553 484f  .Z.FINAL_THRESHO
+000069a0: 4c44 5f77 6974 685f 375f 736d 6f6f 7468  LD_with_7_smooth
+000069b0: 724b 0000 00da 0d68 355f 6b65 795f 6578  rK.....h5_key_ex
+000069c0: 6973 7473 728f 0000 0072 9000 0000 72ad  istsr....r....r.
+000069d0: 0000 0072 ae00 0000 72af 0000 0072 0800  ...r....r....r..
+000069e0: 0000 722c 0100 0072 b200 0000 7222 0100  ..r,...r....r"..
+000069f0: 0072 8500 0000 7288 0000 0029 0d5a 0a68  .r....r....).Z.h
+00006a00: 355f 696e 5f6c 6973 74da 0674 6872 6573  5_in_list..thres
+00006a10: 68da 0b77 7269 7465 5f74 6f5f 6835 da13  h..write_to_h5..
+00006a20: 6f76 6572 7772 6974 655f 6966 5f65 7869  overwrite_if_exi
+00006a30: 7374 735a 0970 726f 6261 5f6b 6579 da09  stsZ.proba_key..
+00006a40: 6c61 6265 6c5f 6b65 7972 bc00 0000 72c2  label_keyr....r.
+00006a50: 0000 0072 fb00 0000 da04 746d 7032 72c0  ...r......tmp2r.
+00006a60: 0000 0072 5300 0000 7223 0100 0072 1600  ...rS...r#...r..
+00006a70: 0000 7216 0000 0072 1700 0000 da1a 6d61  ..r....r......ma
+00006a80: 6b65 5f66 696e 616c 5f70 7265 6469 6374  ke_final_predict
+00006a90: 696f 6e73 5f47 424d 1a04 0000 7332 0000  ions_GBM....s2..
+00006aa0: 0000 0208 0108 0108 0106 0108 0108 010a  ................
+00006ab0: 010a 0104 0108 0104 010c 0102 ff04 0102  ................
+00006ac0: ff02 0106 ff02 ff04 030e 010c 010a 0104  ................
+00006ad0: 010c 0172 7301 0000 6301 0000 0000 0000  ...rs...c.......
+00006ae0: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
+00006af0: 0073 ce00 0000 7400 7c00 7401 8302 721c  .s....t.|.t...r.
+00006b00: 7402 6401 8301 0100 7403 7c00 8301 0100  t.d.....t.|.....
+00006b10: 6eae 7400 7c00 7404 8302 7262 7a24 7405  n.t.|.t...rbz$t.
+00006b20: a006 7407 a008 7c00 a101 a101 7d00 7402  ..t...|.....}.t.
+00006b30: 6402 8301 0100 7409 7c00 8301 0100 5700  d.....t.|.....W.
+00006b40: 71ca 0100 0100 0100 7402 6403 8301 0100  q.......t.d.....
+00006b50: 5900 71ca 5800 6e68 740a 7c00 8301 6a0b  Y.q.X.nht.|...j.
+00006b60: 7407 6a0c 6b02 7284 7402 6404 8301 0100  t.j.k.r.t.d.....
+00006b70: 7409 7c00 8301 0100 6e46 7a24 7402 6405  t.|.....nFz$t.d.
+00006b80: 740d 740a 7c00 8301 8301 1700 6406 1700  t.t.|.......d...
+00006b90: 8301 0100 740e 7c00 8301 0100 5700 6e20  ....t.|.....W.n 
+00006ba0: 0100 0100 0100 7402 6407 8301 0100 7402  ......t.d.....t.
+00006bb0: 740a 7c00 8301 8301 0100 5900 6e02 5800  t.|.......Y.n.X.
+00006bc0: 6400 5300 2908 4e7a 0c74 7970 6520 6973  d.S.).Nz.type is
+00006bd0: 2064 6963 747a 4174 7970 6520 6973 206c   dictzAtype is l
+00006be0: 6973 742c 2063 6f6e 7665 7274 696e 6720  ist, converting 
+00006bf0: 6120 636f 7079 2074 6f20 6e75 6d70 7920  a copy to numpy 
+00006c00: 6172 7261 7920 746f 2070 7269 6e74 2074  array to print t
+00006c10: 6869 7320 696e 666f 7a70 7479 7065 2069  his infozptype i
+00006c20: 7320 6120 6c69 7374 2074 6861 7420 6361  s a list that ca
+00006c30: 6e27 7420 6265 2063 6f6e 7665 7274 6564  n't be converted
+00006c40: 2074 6f20 6120 6e75 6d70 7920 6172 7261   to a numpy arra
+00006c50: 7920 666f 7220 7072 696e 7469 6e67 2069  y for printing i
+00006c60: 6e66 6f20 6f72 206d 6179 6265 2064 6174  nfo or maybe dat
+00006c70: 6120 666f 726d 6174 2069 7320 6e6f 7420  a format is not 
+00006c80: 636f 6d70 6174 6962 6c65 7a10 7479 7065  compatiblez.type
+00006c90: 2069 7320 6e70 2061 7272 6179 7a08 7479   is np arrayz.ty
+00006ca0: 7065 2069 7320 7a2b 2077 696c 6c20 7472  pe is z+ will tr
+00006cb0: 7920 7072 696e 7469 6e67 2075 7369 6e67  y printing using
+00006cc0: 2022 6765 745f 636c 6173 735f 696e 666f   "get_class_info
+00006cd0: 3222 207a 2b63 616e 7420 6669 6e64 206f  2" z+cant find o
+00006ce0: 7574 2077 6861 7420 746f 2064 6f20 7769  ut what to do wi
+00006cf0: 7468 2069 6e70 7574 206f 6620 7479 7065  th input of type
+00006d00: 290f 720b 0100 0072 6900 0000 724b 0000  ).r....ri...rK..
+00006d10: 00da 0d67 6574 5f64 6963 745f 696e 666f  ...get_dict_info
+00006d20: 7239 0000 0072 1b00 0000 721c 0000 0072  r9...r....r....r
+00006d30: 1d00 0000 7238 0000 00da 086e 705f 7374  ....r8.....np_st
+00006d40: 6174 7372 1c01 0000 da0a 5f5f 6d6f 6475  atsr......__modu
+00006d50: 6c65 5f5f da08 5f5f 6e61 6d65 5f5f 72ad  le__..__name__r.
+00006d60: 0000 00da 0f67 6574 5f63 6c61 7373 5f69  .....get_class_i
+00006d70: 6e66 6f32 72d1 0000 0072 1600 0000 7216  nfo2r....r....r.
+00006d80: 0000 0072 1700 0000 da04 696e 666f 3104  ...r......info1.
+00006d90: 0000 732a 0000 0000 010a 0108 010a 010a  ..s*............
+00006da0: 0102 0110 0108 010c 0106 0102 0102 ff0c  ................
+00006db0: 0310 0108 010a 0202 0118 010c 0106 0108  ................
+00006dc0: 0172 7901 0000 fa13 416d 6572 6963 612f  .ry.....America/
+00006dd0: 4c6f 735f 416e 6765 6c65 7363 0100 0000  Los_Angelesc....
+00006de0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00006df0: 4300 0000 7332 0000 0074 00a0 017c 00a1  C...s2...t...|..
+00006e00: 017d 0174 006a 02a0 0374 04a0 05a1 00a1  .}.t.j...t......
+00006e10: 017d 027c 02a0 067c 01a1 017d 037c 03a0  .}.|...|...}.|..
+00006e20: 0764 01a1 017d 047c 0453 0029 024e 7a11  .d...}.|.S.).Nz.
+00006e30: 2559 5f25 6d5f 2564 5f25 485f 254d 5f25  %Y_%m_%d_%H_%M_%
+00006e40: 5329 08da 0470 7974 7ada 0874 696d 657a  S)...pytz..timez
+00006e50: 6f6e 65da 0375 7463 da08 6c6f 6361 6c69  one..utc..locali
+00006e60: 7a65 720d 0000 00da 0675 7463 6e6f 77da  zer......utcnow.
+00006e70: 0a61 7374 696d 657a 6f6e 65da 0873 7472  .astimezone..str
+00006e80: 6674 696d 6529 055a 1074 696d 655f 7a6f  ftime).Z.time_zo
+00006e90: 6e65 5f73 7472 696e 67da 0274 7a5a 066c  ne_string..tzZ.l
+00006ea0: 6f63 5f64 745a 0c63 7572 7265 6e74 5f74  oc_dtZ.current_t
+00006eb0: 696d 655a 0e74 6f64 6179 735f 7665 7273  imeZ.todays_vers
+00006ec0: 696f 6e72 1600 0000 7216 0000 0072 1700  ionr....r....r..
+00006ed0: 0000 da0f 6765 745f 7469 6d65 5f73 7472  ....get_time_str
+00006ee0: 696e 674a 0400 0073 0a00 0000 0001 0a01  ingJ...s........
+00006ef0: 1001 0a01 0a01 7283 0100 0063 0900 0000  ......r....c....
+00006f00: 0000 0000 0000 0000 2c00 0000 0900 0000  ........,.......
+00006f10: 0300 0000 731a 0600 0074 0083 007d 0974  ....s....t...}.t
+00006f20: 016a 02a0 0374 016a 02a0 047c 00a1 01a1  .j...t.j...|....
+00006f30: 017d 0a7c 0364 016b 0872 2a74 05a0 06a1  .}.|.d.k.r*t....
+00006f40: 007d 0367 0067 0067 0067 0067 0067 0067  .}.g.g.g.g.g.g.g
+00006f50: 0067 0064 029c 087d 0b64 017d 0c64 037d  .g.d...}.d.}.d.}
+00006f60: 0d7c 0d90 0172 c674 07a0 0874 097c 0064  .|...r.t...t.|.d
+00006f70: 0483 02a1 017d 0e74 07a0 0a74 07a0 0b64  .....}.t...t...d
+00006f80: 0564 0684 007c 0e44 0083 01a1 01a1 017d  .d...|.D.......}
+00006f90: 0f7c 0e7c 0f19 007d 0e74 0c7c 0e83 0164  .|.|...}.t.|...d
+00006fa0: 076b 0272 9874 0d64 0883 0101 007c 0c53  .k.r.t.d.....|.S
+00006fb0: 0074 0e7c 0e64 0719 0083 017d 1074 016a  .t.|.d.....}.t.j
+00006fc0: 02a0 0f7c 0e64 0719 00a1 017d 117c 0790  ...|.d.....}.|..
+00006fd0: 0172 467c 1064 0919 0090 0173 4674 107c  .rF|.d.....sFt.|
+00006fe0: 1064 0a19 0083 0144 005d 6c5c 027d 127d  .d.....D.]l\.}.}
+00006ff0: 137c 1372 d07c 1174 016a 1117 0074 016a  .|.r.|.t.j...t.j
+00007000: 02a0 037c 1064 0b19 007c 1219 00a1 0117  ...|.d...|......
+00007010: 007d 147c 14a0 127c 0a7c 0a64 0c17 00a1  .}.|...|.|.d....
+00007020: 027d 1574 1374 016a 02a0 0f7c 15a1 0183  .}.t.t.j...|....
+00007030: 016a 1464 0364 0364 0d8d 0201 0074 15a0  .j.d.d.d.....t..
+00007040: 167c 147c 15a1 0201 0064 037c 1064 0e19  .|.|.....d.|.d..
+00007050: 007c 123c 0071 d064 037c 1064 093c 0074  .|.<.q.d.|.d.<.t
+00007060: 177c 0074 016a 02a0 047c 00a1 0164 0f17  .|.t.j...|...d..
+00007070: 0083 0201 0074 07a0 187c 1064 0e19 0064  .....t...|.d...d
+00007080: 036b 02a1 0190 0172 c07c 0e64 0719 007d  .k.....r.|.d...}
+00007090: 1474 15a0 167c 147c 14a0 127c 0a7c 0a64  .t...|.|...|.|.d
+000070a0: 0f17 00a1 02a1 0201 0074 016a 02a0 0f7c  .........t.j...|
+000070b0: 14a1 0174 016a 1117 0064 1017 007d 1474  ...t.j...d...}.t
+000070c0: 15a0 167c 147c 14a0 127c 0a7c 0a64 0f17  ...|.|...|.|.d..
+000070d0: 00a1 02a1 0201 0071 4864 117d 0d71 4874  .......qHd.}.qHt
+000070e0: 19a0 19a1 007d 167c 1667 017d 1774 016a  .....}.|.g.}.t.j
+000070f0: 02a0 1a7c 01a1 0190 0172 ec74 15a0 1b7c  ...|.....r.t...|
+00007100: 01a1 0101 0074 137c 0183 016a 1464 0364  .....t.|...j.d.d
+00007110: 0364 0d8d 0201 0074 016a 1164 1017 007d  .d.....t.j.d...}
+00007120: 147c 017c 1417 007d 1874 15a0 1c7c 117c  .|.|...}.t...|.|
+00007130: 1417 007c 18a1 0201 0074 07a0 1d7c 1064  ...|.....t...|.d
+00007140: 0e19 0064 116b 02a1 0164 0719 0064 017c  ...d.k...d...d.|
+00007150: 0285 0219 007d 197c 1944 005d 347d 1a74  .....}.|.D.]4}.t
+00007160: 016a 1174 016a 02a0 037c 1064 0b19 007c  .j.t.j...|.d...|
+00007170: 1a19 00a1 0117 007d 1474 15a0 1c7c 117c  .......}.t...|.|
+00007180: 1417 007c 017c 1417 00a1 0201 0090 0271  ...|.|.........q
+00007190: 427c 17a0 1e74 19a0 19a1 00a1 0101 0074  B|...t.........t
+000071a0: 1f7c 017c 187c 067c 0864 128d 047d 1b7c  .|.|.|.|.d...}.|
+000071b0: 1ba0 20a1 0001 007c 17a0 1e74 19a0 19a1  .. ....|...t....
+000071c0: 00a1 0101 007c 1b6a 217d 1c7c 1ca0 1264  .....|.j!}.|...d
+000071d0: 1364 14a1 027d 1d74 22a0 237c 1c7c 1da1  .d...}.t".#|.|..
+000071e0: 0201 007c 17a0 1e74 19a0 19a1 00a1 0101  ...|...t........
+000071f0: 007c 1da0 1264 1364 15a1 027d 1e74 226a  .|...d.d...}.t"j
+00007200: 2464 167c 1d64 1764 188d 037d 1f74 257c  $d.|.d.d...}.t%|
+00007210: 037c 1f7c 1e83 0301 007c 17a0 1e74 19a0  .|.|.....|...t..
+00007220: 19a1 00a1 0101 0074 267c 1964 0719 0064  .......t&|.d...d
+00007230: 1917 0083 0164 1a17 0074 267c 1964 1b19  .....d...t&|.d..
+00007240: 0064 1917 0083 0117 0064 1c17 0074 2674  .d.......d...t&t
+00007250: 0c7c 1064 0e19 0083 0183 0117 007d 207c  .|.d.........} |
+00007260: 1ca0 1264 1364 1d7c 2017 0064 1317 00a1  ...d.d.| ..d....
+00007270: 027d 2174 277c 1e7c 2164 0364 0364 1e8d  .}!t'|.|!d.d.d..
+00007280: 0401 0074 22a0 287c 1e64 1fa1 02a0 29a1  ...t".(|.d....).
+00007290: 007d 2274 2a7c 2164 1f7c 2283 0301 007c  .}"t*|!d.|"....|
+000072a0: 17a0 1e74 19a0 19a1 00a1 0101 0074 2b7c  ...t.........t+|
+000072b0: 1c7c 2183 0201 007c 0490 0372 be74 22a0  .|!....|...r.t".
+000072c0: 287c 1d64 20a1 027d 2374 2a7c 2164 207c  (|.d ..}#t*|!d |
+000072d0: 2383 0301 007e 2374 01a0 2c7c 1da1 0101  #....~#t..,|....
+000072e0: 007c 0590 0372 e874 22a0 287c 1e64 21a1  .|...r.t".(|.d!.
+000072f0: 027d 2474 2a7c 2164 217c 2483 0301 007e  .}$t*|!d!|$....~
+00007300: 2474 01a0 2c7c 1ea1 0101 0074 016a 02a0  $t..,|.....t.j..
+00007310: 0f7c 0e64 0719 00a1 0174 016a 1117 007d  .|.d.....t.j...}
+00007320: 147c 14a0 127c 0a7c 0a64 0f17 00a1 0274  .|...|.|.d.....t
+00007330: 016a 02a0 037c 21a1 0117 007d 2574 15a0  .j...|!....}%t..
+00007340: 1c7c 217c 25a1 0201 007c 1944 005d 127d  .|!|%....|.D.].}
+00007350: 2664 037c 1064 0e19 007c 263c 0090 0471  &d.|.d...|&<...q
+00007360: 3474 2d7c 107c 0e64 0719 0083 0201 007c  4t-|.|.d.......|
+00007370: 1944 005d 5a7d 1a7c 1174 016a 1117 0074  .D.]Z}.|.t.j...t
+00007380: 016a 02a0 037c 1064 0b19 007c 1a19 00a1  .j...|.d...|....
+00007390: 0117 007d 147c 14a0 127c 0a7c 0a64 2217  ...}.|...|.|.d".
+000073a0: 00a1 027d 2774 1374 016a 02a0 0f7c 27a1  ...}'t.t.j...|'.
+000073b0: 0183 016a 1464 0364 0364 0d8d 0201 0074  ...j.d.d.d.....t
+000073c0: 15a0 167c 147c 27a1 0201 0090 0471 5a7c  ...|.|'......qZ|
+000073d0: 17a0 1e74 19a0 19a1 00a1 0101 0074 07a0  ...t.........t..
+000073e0: 2e7c 17a1 017d 2864 2364 2464 2564 2664  .|...}(d#d$d%d&d
+000073f0: 2764 2864 2967 077d 2964 2a74 2f64 2b64  'd(d)g.})d*t/d+d
+00007400: 2c84 007c 2944 0083 0183 0114 0089 0074  ,..|)D.........t
+00007410: 0d64 2d83 0101 0064 2ea0 3087 0066 0164  .d-....d..0..f.d
+00007420: 2f64 0684 0874 317c 287c 297c 2874 0c7c  /d...t1|(|)|(t.|
+00007430: 1983 011b 0083 0344 0083 01a1 017d 2a74  .......D.....}*t
+00007440: 0d7c 2a83 0101 0074 0d64 3083 0101 0074  .|*....t.d0....t
+00007450: 0d88 0074 2674 3274 3374 07a0 347c 28a1  ...t&t2t3t..4|(.
+00007460: 0183 0164 318d 0183 01a0 3564 32a1 0164  ...d1.....5d2..d
+00007470: 0719 0017 0064 3317 0074 2674 3274 07a0  .....d3..t&t2t..
+00007480: 347c 28a1 0174 0c7c 1983 011b 0064 318d  4|(..t.|.....d1.
+00007490: 0183 01a0 3564 32a1 0164 0719 0017 0083  ....5d2..d......
+000074a0: 0101 0074 07a0 367c 2874 0c7c 1983 0167  ...t..6|(t.|...g
+000074b0: 0166 02a1 017d 287c 0c64 016b 0890 0572  .f...}(|.d.k...r
+000074c0: c474 376a 387c 2864 0164 0164 0185 0266  .t7j8|(d.d.d...f
+000074d0: 0219 007c 2964 348d 027d 0c6e 2874 376a  ...|)d4..}.n(t7j
+000074e0: 387c 2864 0164 0164 0185 0266 0219 007c  8|(d.d.d...f...|
+000074f0: 2964 348d 027d 2b7c 0c6a 1e7c 2b64 0364  )d4..}+|.j.|+d.d
+00007500: 358d 027d 0c74 2d7c 0c74 016a 02a0 047c  5..}.t-|.t.j...|
+00007510: 00a1 0164 0f17 0074 016a 1117 0064 3617  ...d...t.j...d6.
+00007520: 007c 0917 0064 3717 0083 0201 0071 4464  .|...d7......qDd
+00007530: 0153 0029 3861 e301 0000 0a20 2020 2075  .S.)8a.....    u
+00007540: 7365 2075 7469 6c73 2e6d 616b 655f 6d70  se utils.make_mp
+00007550: 345f 6c69 7374 5f64 6963 7420 746f 206d  4_list_dict to m
+00007560: 616b 6520 6c69 7374 7320 6f66 2074 6865  ake lists of the
+00007570: 206d 7034 2066 696c 6573 2066 6972 7374   mp4 files first
+00007580: 2c20 6974 2063 616e 2062 6520 7275 6e20  , it can be run 
+00007590: 6f6e 2074 6865 206d 6173 7465 7220 6469  on the master di
+000075a0: 7265 6374 6f72 7920 616e 6420 7769 6c6c  rectory and will
+000075b0: 2069 6e64 6578 2061 6c6c 2066 6f6c 6465   index all folde
+000075c0: 7273 2077 6974 6820 4d50 3420 6669 6c65  rs with MP4 file
+000075d0: 730a 2020 2020 5061 7261 6d65 7465 7273  s.    Parameters
+000075e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000075f0: 2020 2020 6264 203a 0a20 2020 206c 6f63      bd :.    loc
+00007600: 616c 5f74 656d 705f 6469 7220 3a0a 2020  al_temp_dir :.  
+00007610: 2020 7669 6465 6f5f 6261 7463 685f 7369    video_batch_si
+00007620: 7a65 203a 0a20 2020 2052 4553 4e45 545f  ze :.    RESNET_
+00007630: 4d4f 4445 4c20 3a0a 2020 2020 636f 7079  MODEL :.    copy
+00007640: 5f69 6d61 6765 5f66 696c 6573 5f74 6f5f  _image_files_to_
+00007650: 6669 6e61 6c5f 6835 203a 0a20 2020 2063  final_h5 :.    c
+00007660: 6f70 795f 6665 6174 7572 655f 6461 7461  opy_feature_data
+00007670: 5f74 6f5f 6669 6e61 6c5f 6835 203a 2063  _to_final_h5 : c
+00007680: 6f70 7920 7468 6520 3230 3438 206f 7269  opy the 2048 ori
+00007690: 6769 6e61 6c20 6665 6174 7572 6520 6461  ginal feature da
+000076a0: 7461 2074 6f20 7468 6520 6669 6e61 6c20  ta to the final 
+000076b0: 4835 2c20 6f6e 6c79 206e 6565 6465 6420  H5, only needed 
+000076c0: 666f 7220 6d6f 6465 6c20 7465 7374 696e  for model testin
+000076d0: 6720 616e 6420 6275 696c 6469 6e67 0a20  g and building. 
+000076e0: 2020 2063 7573 746f 6d5f 696d 6167 655f     custom_image_
+000076f0: 6578 7472 6163 745f 7369 7a65 203a 0a0a  extract_size :..
+00007700: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00007710: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 2908  -------..    N).
+00007720: 5a09 6e75 6d5f 6669 6c65 735a 1274 696d  Z.num_filesZ.tim
+00007730: 655f 636f 7079 5f74 6f5f 6c6f 6361 6c5a  e_copy_to_localZ
+00007740: 0874 696d 655f 616c 6c5a 0d74 696d 655f  .time_allZ.time_
+00007750: 746f 5f74 7261 636b 5a0c 7469 6d65 5f74  to_trackZ.time_t
+00007760: 6f5f 336c 6167 5a10 7469 6d65 5f74 6f5f  o_3lagZ.time_to_
+00007770: 6665 6174 7572 6573 5a14 7469 6d65 5f74  featuresZ.time_t
+00007780: 6f5f 616c 6c5f 6665 6174 7572 6573 5a14  o_all_featuresZ.
+00007790: 7469 6d65 5f74 6f5f 6375 745f 6665 6174  time_to_cut_feat
+000077a0: 7572 6573 54fa 232a 6669 6c65 5f6c 6973  uresT.#*file_lis
+000077b0: 745f 666f 725f 6261 7463 685f 7072 6f63  t_for_batch_proc
+000077c0: 6573 7369 6e67 2e70 6b6c 6301 0000 0000  essing.pklc.....
+000077d0: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+000077e0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+000077f0: 7400 6a01 a002 7c01 a101 9102 7104 5300  t.j...|.....q.S.
+00007800: 7216 0000 0029 0372 5f00 0000 7261 0000  r....).r_...ra..
+00007810: 00da 0867 6574 6374 696d 6572 3100 0000  ...getctimer1...
+00007820: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00007830: 3400 0000 7704 0000 7304 0000 0006 0002  4...w...s.......
+00007840: 007a 3162 6174 6368 5f70 726f 6365 7373  .z1batch_process
+00007850: 5f76 6964 656f 735f 6f6e 5f63 6f6c 6162  _videos_on_colab
+00007860: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00007870: 6f6d 703e 7201 0000 007a 1346 494e 4953  omp>r....z.FINIS
+00007880: 4845 4420 5052 4f43 4553 5349 4e47 da18  HED PROCESSING..
+00007890: 6261 645f 7669 6473 5f68 6176 655f 6265  bad_vids_have_be
+000078a0: 656e 5f6d 6f76 6564 da16 4650 535f 6368  en_moved..FPS_ch
+000078b0: 6563 6b5f 6261 645f 7669 645f 696e 6473  eck_bad_vid_inds
+000078c0: da09 6d70 345f 6e61 6d65 735a 095f 4241  ..mp4_namesZ._BA
+000078d0: 445f 4d50 3473 7260 0100 00da 0c69 735f  D_MP4sr`.....is_
+000078e0: 7072 6f63 6573 7365 645a 095f 4649 4e49  processedZ._FINI
+000078f0: 5348 4544 7a10 7465 6d70 6c61 7465 5f69  SHEDz.template_i
+00007900: 6d67 2e70 6e67 4629 0472 a000 0000 72a1  mg.pngF).r....r.
+00007910: 0000 00da 1963 7573 746f 6d5f 696d 6167  .....custom_imag
+00007920: 655f 6578 7472 6163 745f 7369 7a65 72a3  e_extract_sizer.
+00007930: 0000 0072 a400 0000 72a5 0000 007a 105f  ...r....r....z._
+00007940: 6665 6174 7572 655f 6461 7461 2e68 3569  feature_data.h5i
+00007950: f401 0000 7252 0000 0029 0172 7101 0000  ....rR...).rq...
+00007960: 722e 0000 005a 045f 746f 5f72 4a00 0000  r....Z._to_rJ...
+00007970: 5a04 5f6f 665f 5a12 5f66 696e 616c 5f74  Z._of_Z._final_t
+00007980: 6f5f 636f 6d62 696e 655f 2903 5a10 7772  o_combine_).Z.wr
+00007990: 6974 655f 746f 5f74 6869 735f 6835 5a11  ite_to_this_h5Z.
+000079a0: 7772 6974 655f 6669 6e61 6c5f 746f 5f68  write_final_to_h
+000079b0: 355a 0e64 656c 6574 655f 7465 6d70 5f68  5Z.delete_temp_h
+000079c0: 3572 5a01 0000 729a 0000 0072 5901 0000  5rZ...r....rY...
+000079d0: 5a0e 5f46 494e 4953 4845 445f 4d50 3473  Z._FINISHED_MP4s
+000079e0: 7a12 636f 7079 206d 7034 7320 746f 206c  z.copy mp4s to l
+000079f0: 6f63 616c 7a0e 7472 6163 6b20 7468 6520  ocalz.track the 
+00007a00: 706f 6c65 7a0f 636f 6e76 6572 7420 746f  polez.convert to
+00007a10: 2033 6c61 677a 1963 7265 6174 6520 6665   3lagz.create fe
+00007a20: 6174 7572 6520 6461 7461 2028 434e 4e29  ature data (CNN)
+00007a30: 7a15 656e 6769 6e65 6572 2061 6c6c 2066  z.engineer all f
+00007a40: 6561 7475 7265 737a 2663 6f70 7920 2068  eaturesz&copy  h
+00007a50: 3520 616e 6420 6d70 3473 2074 6f20 6669  5 and mp4s to fi
+00007a60: 6e61 6c20 6465 7374 696e 6174 696f 6e7a  nal destinationz
+00007a70: 0f6e 756d 6265 7220 6f66 2066 696c 6573  .number of files
+00007a80: fa01 2063 0100 0000 0000 0000 0000 0000  .. c............
+00007a90: 0200 0000 0300 0000 7300 0000 731a 0000  ........s...s...
+00007aa0: 007c 005d 127d 0174 007c 0183 0164 0017  .|.].}.t.|...d..
+00007ab0: 0056 0001 0071 0264 0153 0029 0272 d900  .V...q.d.S.).r..
+00007ac0: 0000 4e72 4800 0000 7231 0000 0072 1600  ..NrH...r1...r..
+00007ad0: 0000 7216 0000 0072 1700 0000 72d8 0000  ..r....r....r...
+00007ae0: 0000 0500 0073 0400 0000 0400 0200 7a30  .....s........z0
+00007af0: 6261 7463 685f 7072 6f63 6573 735f 7669  batch_process_vi
+00007b00: 6465 6f73 5f6f 6e5f 636f 6c61 622e 3c6c  deos_on_colab.<l
+00007b10: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00007b20: 7a3c 6f70 6572 6174 696f 6e20 2020 2020  z<operation     
+00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b40: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00007b50: 6c20 2020 2020 7065 7220 6669 6c65 72d4  l     per filer.
+00007b60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00007b70: 0400 0000 0700 0000 1300 0000 735e 0000  ............s^..
+00007b80: 0067 007c 005d 565c 037d 017d 027d 037c  .g.|.]V\.}.}.}.|
+00007b90: 0288 0017 0064 0074 0088 0083 0185 0219  .....d.t........
+00007ba0: 0074 0174 027c 0164 018d 0183 01a0 0364  .t.t.|.d.......d
+00007bb0: 02a1 0164 0319 0017 0064 0417 0074 0174  ...d.....d...t.t
+00007bc0: 027c 0364 018d 0183 01a0 0364 02a1 0164  .|.d.......d...d
+00007bd0: 0319 0017 0064 0517 0091 0271 0453 0029  .....d.....q.S.)
+00007be0: 064e a901 da07 7365 636f 6e64 7372 2101  .N....secondsr!.
+00007bf0: 0000 7201 0000 00fa 0320 2020 da01 0a29  ..r......   ...)
+00007c00: 0472 3000 0000 72ad 0000 0072 0c00 0000  .r0...r....r....
+00007c10: 72db 0000 0029 0472 3200 0000 7233 0000  r....).r2...r3..
+00007c20: 0072 be00 0000 da02 6b33 a901 da09 6c65  .r......k3....le
+00007c30: 6e5f 7370 6163 6572 1600 0000 7217 0000  n_spacer....r...
+00007c40: 0072 3400 0000 0205 0000 7314 0000 0006  .r4.......s.....
+00007c50: 0108 ff24 0102 ff04 0102 ff02 0116 ff02  ...$............
+00007c60: 0102 ff7a 3c54 4f54 414c 2020 2020 2020  ...z<TOTAL      
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00007c90: 6f74 616c 2020 2020 2070 6572 2066 696c  otal     per fil
+00007ca0: 6572 8c01 0000 7221 0100 0072 8e01 0000  er....r!...r....
+00007cb0: 2901 da07 636f 6c75 6d6e 7329 015a 0c69  )...columns).Z.i
+00007cc0: 676e 6f72 655f 696e 6465 785a 0874 696d  gnore_indexZ.tim
+00007cd0: 655f 6466 5ffa 042e 706b 6c29 3972 8301  e_df_...pkl)9r..
+00007ce0: 0000 725f 0000 0072 6100 0000 72a8 0000  ..r_...ra...r...
+00007cf0: 00da 086e 6f72 6d70 6174 6872 0500 0000  ...normpathr....
+00007d00: 5a10 6c6f 6164 5f66 696e 616c 5f6d 6f64  Z.load_final_mod
+00007d10: 656c 721d 0000 0072 3800 0000 da09 6765  elr....r8.....ge
+00007d20: 745f 6669 6c65 73da 0466 6c69 7072 8a00  t_files..flipr..
+00007d30: 0000 7230 0000 0072 4b00 0000 7263 0000  ..r0...rK...rc..
+00007d40: 0072 a700 0000 7224 0000 0072 6000 0000  .r....r$...r`...
+00007d50: 72b7 0000 0072 0e00 0000 7263 0100 0072  r....r....rc...r
+00007d60: 7300 0000 da04 6d6f 7665 da15 636f 7079  s.....move..copy
+00007d70: 5f66 6f6c 6465 725f 7374 7275 6374 7572  _folder_structur
+00007d80: 6572 2f00 0000 da04 7469 6d65 da06 6578  er/.....time..ex
+00007d90: 6973 7473 7274 0000 0072 1b00 0000 72b9  istsrt...r....r.
+00007da0: 0000 0072 2300 0000 7204 0000 005a 1374  ...r#...r....Z.t
+00007db0: 7261 636b 5f61 6c6c 5f61 6e64 5f73 6176  rack_all_and_sav
+00007dc0: 656a 72b6 0000 0072 0800 0000 72b8 0000  ejr....r....r...
+00007dd0: 005a 1349 6d61 6765 4261 7463 6847 656e  .Z.ImageBatchGen
+00007de0: 6572 6174 6f72 7202 0000 0072 ad00 0000  eratorr....r....
+00007df0: 7203 0000 0072 2c01 0000 72f9 0000 0072  r....r,...r....r
+00007e00: 2201 0000 da1c 636f 7079 5f6f 7665 725f  ".....copy_over_
+00007e10: 616c 6c5f 6e6f 6e5f 696d 6167 655f 6b65  all_non_image_ke
+00007e20: 7973 7279 0000 00da 0873 6176 655f 6f62  ysry.....save_ob
+00007e30: 6ada 0464 6966 6672 1301 0000 72da 0000  j..diffr....r...
+00007e40: 0072 b000 0000 720c 0000 0072 8800 0000  .r....r....r....
+00007e50: 7235 0000 0072 db00 0000 7226 0000 00da  r5...r....r&....
+00007e60: 0270 645a 0944 6174 6146 7261 6d65 292c  .pdZ.DataFrame),
+00007e70: 7264 0000 005a 0e6c 6f63 616c 5f74 656d  rd...Z.local_tem
+00007e80: 705f 6469 725a 1076 6964 656f 5f62 6174  p_dirZ.video_bat
+00007e90: 6368 5f73 697a 655a 0c52 4553 4e45 545f  ch_sizeZ.RESNET_
+00007ea0: 4d4f 4445 4c5a 1c63 6f70 795f 696d 6167  MODELZ.copy_imag
+00007eb0: 655f 6669 6c65 735f 746f 5f66 696e 616c  e_files_to_final
+00007ec0: 5f68 355a 1d63 6f70 795f 6665 6174 7572  _h5Z.copy_featur
+00007ed0: 655f 6461 7461 5f74 6f5f 6669 6e61 6c5f  e_data_to_final_
+00007ee0: 6835 728a 0100 005a 1673 6b69 705f 6966  h5r....Z.skip_if
+00007ef0: 5f46 5053 5f69 735f 6e6f 745f 696e 7472  _FPS_is_not_intr
+00007f00: a300 0000 5a08 7469 6d65 5f73 7472 5a0c  ....Z.time_strZ.
+00007f10: 6264 5f62 6173 655f 6e61 6d65 5a09 7469  bd_base_nameZ.ti
+00007f20: 6d65 5f64 6963 745a 0774 696d 655f 6466  me_dictZ.time_df
+00007f30: 5a0e 6772 6162 5f66 696c 655f 6c69 7374  Z.grab_file_list
+00007f40: 5a12 6c69 7374 5f6f 665f 6669 6c65 5f64  Z.list_of_file_d
+00007f50: 6963 7473 722b 0000 00da 0966 696c 655f  ictsr+.....file_
+00007f60: 6469 6374 7239 0100 005a 0562 6164 5f69  dictr9...Z.bad_i
+00007f70: 5a06 6973 5f62 6164 7253 0000 005a 0b62  Z.is_badrS...Z.b
+00007f80: 6164 5f6d 7034 5f64 6972 da05 7374 6172  ad_mp4_dir..star
+00007f90: 745a 0974 696d 655f 6c69 7374 5a0c 7465  tZ.time_listZ.te
+00007fa0: 6d70 6c61 7465 5f64 6972 5a14 7072 6f63  mplate_dirZ.proc
+00007fb0: 6573 735f 7468 6573 655f 7669 6465 6f73  ess_these_videos
+00007fc0: 722c 0000 005a 0250 5472 c200 0000 72c3  r,...Z.PTr....r.
+00007fd0: 0000 005a 0f68 355f 6665 6174 7572 655f  ...Z.h5_feature_
+00007fe0: 6461 7461 5a06 696e 5f67 656e 5a09 6669  dataZ.in_genZ.fi
+00007ff0: 6c65 5f6e 756d 735a 0868 355f 6669 6e61  le_numsZ.h5_fina
+00008000: 6c72 5a01 0000 729a 0000 0072 5901 0000  lrZ...r....rY...
+00008010: 727a 0000 0072 3300 0000 5a0d 6669 6e61  rz...r3...Z.fina
+00008020: 6c5f 6d70 345f 6469 725a 0a74 696d 655f  l_mp4_dirZ.time_
+00008030: 6172 7261 795a 0c64 665f 6e61 6d65 5f6c  arrayZ.df_name_l
+00008040: 6973 745a 0874 6f5f 7072 696e 745a 0674  istZ.to_printZ.t
+00008050: 6d70 5f64 6672 1600 0000 7291 0100 0072  mp_dfr....r....r
+00008060: 1700 0000 da1d 6261 7463 685f 7072 6f63  ......batch_proc
+00008070: 6573 735f 7669 6465 6f73 5f6f 6e5f 636f  ess_videos_on_co
+00008080: 6c61 6252 0400 0073 ec00 0000 0015 0601  labR...s........
+00008090: 1402 0801 0801 0a01 0200 0200 02ff 0602  ................
+000080a0: 0403 0401 0602 1003 1a01 0801 0c01 0801  ................
+000080b0: 0403 0c02 1002 1002 1401 0401 1e01 1001  ................
+000080c0: 1a02 0c01 0e01 0803 1602 1401 0801 1801  ................
+000080d0: 1601 1a02 0601 0801 0602 0e01 0a01 1202  ................
+000080e0: 0a01 0801 1001 1e02 0801 1a01 1801 0e03  ................
+000080f0: 0601 0201 02fe 0604 0801 0e03 0601 0c01  ................
+00008100: 0c01 0e04 0c01 1001 0c01 0e0f 2801 0aff  ............(...
+00008110: 0602 1402 0801 02ff 0602 1001 0c02 0e06  ................
+00008120: 0a02 0601 0c01 0c01 0203 0a04 0601 0c01  ................
+00008130: 0c01 0201 0a01 1601 1c01 0c02 0801 1001  ................
+00008140: 0e03 0801 1e01 1001 1a01 1001 0e02 0a01  ................
+00008150: 0801 0200 0201 02fe 0404 1601 0801 0e02  ................
+00008160: 12fe 0803 0801 0801 2a01 24ff 0603 1401  ........*.$.....
+00008170: 0a01 1c02 1a01 0e01 72a2 0100 0063 0200  ........r....c..
+00008180: 0000 0000 0000 0000 0000 0600 0000 0600  ................
+00008190: 0000 4300 0000 7360 0000 0074 007c 0064  ..C...s`...t.|.d
+000081a0: 0183 027d 027c 0244 005d 4c7d 0374 017c  ...}.|.D.]L}.t.|
+000081b0: 0383 017d 0474 02a0 037c 0464 0219 0064  ...}.t...|.d...d
+000081c0: 036b 02a1 0172 0e74 0474 0074 056a 06a0  .k...r.t.t.t.j..
+000081d0: 077c 03a1 0164 0483 0283 017d 0574 087c  .|...d.....}.t.|
+000081e0: 0583 0164 056b 0472 0e74 097c 057c 0164  ...d.k.r.t.|.|.d
+000081f0: 068d 0201 0071 0e64 0753 0029 0861 3b01  .....q.d.S.).a;.
+00008200: 0000 0a0a 2020 2020 5061 7261 6d65 7465  ....    Paramete
+00008210: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00008220: 2d0a 2020 2020 6264 203a 206a 7573 7420  -.    bd : just 
+00008230: 7075 7420 796f 7572 2062 6173 6520 6469  put your base di
+00008240: 7265 6374 6f72 792c 2069 7420 7769 6c6c  rectory, it will
+00008250: 2061 7574 6f6d 6174 6963 616c 6c79 206c   automatically l
+00008260: 6f61 6420 7468 6520 706b 6c20 6669 6c65  oad the pkl file
+00008270: 2061 6e64 2063 6865 636b 2069 6620 616c   and check if al
+00008280: 6c20 7468 6520 7669 6465 6f73 2061 7265  l the videos are
+00008290: 2070 726f 6365 7373 6564 0a20 2020 2069   processed.    i
+000082a0: 6620 7468 6174 2069 7320 7468 6520 6361  f that is the ca
+000082b0: 7365 2069 7420 7769 6c6c 2063 6f6d 6269  se it will combi
+000082c0: 6e65 2074 6865 6d20 616e 6420 6279 2064  ne them and by d
+000082d0: 6566 6175 6c74 0a20 2020 2064 656c 6574  efault.    delet
+000082e0: 655f 6578 7472 615f 6669 6c65 7320 3a20  e_extra_files : 
+000082f0: 6465 6c65 7465 2074 6865 2066 696c 6573  delete the files
+00008300: 2061 6674 6572 2063 6f6d 6269 6e69 6e67   after combining
+00008310: 2074 6865 2066 696e 616c 206f 6e65 2e0a   the final one..
+00008320: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00008330: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2072 8401  -------..    r..
+00008340: 0000 7289 0100 0054 7a14 2a5f 6669 6e61  ..r....Tz.*_fina
+00008350: 6c5f 746f 5f63 6f6d 6269 6e65 5f2a 7201  l_to_combine_*r.
+00008360: 0000 0029 01da 1264 656c 6574 655f 6578  ...)...delete_ex
+00008370: 7472 615f 6669 6c65 734e 290a 7296 0100  tra_filesN).r...
+00008380: 0072 6300 0000 721d 0000 0072 2f00 0000  .rc...r....r/...
+00008390: 7265 0100 0072 5f00 0000 7261 0000 0072  re...r_...ra...r
+000083a0: a700 0000 7230 0000 00da 1163 6f6d 6269  ....r0.....combi
+000083b0: 6e65 5f66 696e 616c 5f68 3573 2906 7264  ne_final_h5s).rd
+000083c0: 0000 0072 a301 0000 5a11 6669 6e69 7368  ...r....Z.finish
+000083d0: 6564 5f73 6573 7369 6f6e 73da 0166 72a0  ed_sessions..fr.
+000083e0: 0100 00da 1768 355f 6669 6c65 5f6c 6973  .....h5_file_lis
+000083f0: 745f 746f 5f63 6f6d 6269 6e65 7216 0000  t_to_combiner...
+00008400: 0072 1600 0000 7217 0000 00da 1661 7574  .r....r......aut
+00008410: 6f5f 636f 6d62 696e 655f 6669 6e61 6c5f  o_combine_final_
+00008420: 6835 7372 0500 0073 0e00 0000 000c 0a01  h5sr...s........
+00008430: 0801 0801 1201 1601 0c01 72a7 0100 0063  ..........r....c
+00008440: 0200 0000 0000 0000 0000 0000 0e00 0000  ................
+00008450: 0d00 0000 4300 0000 7316 0300 0074 007c  ....C...s....t.|
+00008460: 0083 017d 007c 0064 0119 00a0 0164 02a1  ...}.|.d.....d..
+00008470: 0164 0119 0064 0317 007d 0274 026a 037c  .d...d...}.t.j.|
+00008480: 0264 0464 0564 0664 0464 0764 0764 0774  .d.d.d.d.d.d.d.t
+00008490: 046a 056a 0674 046a 056a 0664 0864 098d  .j.j.t.j.j.d.d..
+000084a0: 0b7d 0374 077c 0083 0144 005d 487d 0474  .}.t.|...D.]H}.t
+000084b0: 04a0 087c 0464 0aa1 028f 327d 057c 0564  ...|.d....2}.|.d
+000084c0: 0819 0064 0064 0085 0219 007d 067c 03a0  ...d.d.....}.|..
+000084d0: 097c 0674 0aa0 0b7c 066a 0c64 0119 00a1  .|.t...|.j.d....
+000084e0: 0164 0b14 00a1 0201 0057 0035 0051 0052  .d.......W.5.Q.R
+000084f0: 0058 0071 4e74 04a0 087c 0264 0ca1 0290  .X.qNt...|.d....
+00008500: 018f 6a7d 057c 0564 0d3d 0074 0d7c 0064  ..j}.|.d.=.t.|.d
+00008510: 0119 0064 0e83 0290 0172 5c74 0e74 077c  ...d.....r\t.t.|
+00008520: 0083 0183 0144 005d 905c 027d 077d 0474  .....D.].\.}.}.t
+00008530: 02a0 0f7c 0464 0ea1 027d 087c 0764 016b  ...|.d...}.|.d.k
+00008540: 0290 0172 1c74 107c 086a 0c83 017d 0964  ...r.t.|.j...}.d
+00008550: 007c 0964 013c 007c 056a 1164 0e74 0aa0  .|.d.<.|.j.d.t..
+00008560: 0c7c 08a1 0174 046a 056a 127c 0964 047c  .|...t.j.j.|.d.|
+00008570: 0864 0f8d 0601 0071 ca7c 0564 0e19 006a  .d.....q.|.d...j
+00008580: 137c 0564 0e19 006a 0c64 0119 007c 086a  .|.d...j.d...|.j
+00008590: 0c64 0119 0017 0064 0164 108d 0201 007c  .d.....d.d.....|
+000085a0: 087c 0564 0e19 007c 086a 0c64 0119 000b  .|.d...|.j.d....
+000085b0: 0064 0085 023c 0071 ca74 0d7c 0064 0119  .d...<.q.t.|.d..
+000085c0: 0064 1183 0290 0272 0c74 0e74 077c 0083  .d.....r.t.t.|..
+000085d0: 0183 0144 005d 925c 027d 077d 0474 02a0  ...D.].\.}.}.t..
+000085e0: 0f7c 0464 11a1 027d 0a7c 0764 016b 0290  .|.d...}.|.d.k..
+000085f0: 0172 ca74 107c 0a6a 0c83 017d 0964 007c  .r.t.|.j...}.d.|
+00008600: 0964 013c 007c 056a 1164 1174 0aa0 0c7c  .d.<.|.j.d.t...|
+00008610: 0aa1 0174 046a 056a 127c 0964 047c 0a64  ...t.j.j.|.d.|.d
+00008620: 0f8d 0601 006e 3e7c 0564 1119 006a 137c  .....n>|.d...j.|
+00008630: 0564 1119 006a 0c64 0119 007c 0a6a 0c64  .d...j.d...|.j.d
+00008640: 0119 0017 0064 0164 108d 0201 007c 0a7c  .....d.d.....|.|
+00008650: 0564 1119 007c 0a6a 0c64 0119 000b 0064  .d...|.j.d.....d
+00008660: 0085 023c 0090 0171 7857 0035 0051 0052  ...<...qxW.5.Q.R
+00008670: 0058 0064 1264 1364 1464 1564 0d64 1664  .X.d.d.d.d.d.d.d
+00008680: 1764 1864 1967 097d 0b67 007d 0c7c 0044  .d.d.g.}.g.}.|.D
+00008690: 005d 1c7d 047c 0ca0 1474 02a0 0f74 157c  .].}.|...t...t.|
+000086a0: 0483 0164 1aa1 02a1 0101 0090 0271 3474  ...d.........q4t
+000086b0: 0aa0 167c 0ca1 017d 0c74 177c 0264 1a7c  ...|...}.t.|.d.|
+000086c0: 0c83 0301 0074 04a0 087c 0264 0ca1 028f  .....t...|.d....
+000086d0: 4c7d 0574 077c 0b83 0144 005d 3c7d 0474  L}.t.|...D.]<}.t
+000086e0: 0d7c 0064 0119 007c 0483 0290 0272 7e74  .|.d...|.....r~t
+000086f0: 02a0 0f7c 007c 04a1 027d 0d7c 0464 146b  ...|.|...}.|.d.k
+00008700: 0290 0272 b074 107c 0d83 017d 0d7c 0d7c  ...r.t.|...}.|.|
+00008710: 057c 043c 0090 0271 7e57 0035 0051 0052  .|.<...q~W.5.Q.R
+00008720: 0058 0074 177c 0264 1b74 02a0 0f7c 0064  .X.t.|.d.t...|.d
+00008730: 0119 0064 1ba1 0283 0301 0074 177c 0264  ...d.......t.|.d
+00008740: 1c74 02a0 0f7c 0064 0119 0064 1ca1 0283  .t...|.d...d....
+00008750: 0301 007c 0190 0372 127c 0044 005d 107d  ...|...r.|.D.].}
+00008760: 0474 18a0 197c 04a1 0101 0090 0371 0064  .t...|.......q.d
+00008770: 0053 0029 1d4e 7201 0000 00da 0566 696e  .S.).Nr......fin
+00008780: 616c 7a11 6669 6e61 6c5f 636f 6d62 696e  alz.final_combin
+00008790: 6564 2e68 3554 722e 0000 0069 3908 0000  ed.h5Tr....i9...
+000087a0: 4672 4900 0000 290a 723a 0100 0072 3b01  FrI...).r:...r;.
+000087b0: 0000 723c 0100 0072 3d01 0000 723e 0100  ..r<...r=...r>..
+000087c0: 0072 3f01 0000 7240 0100 0072 4101 0000  .r?...r@...rA...
+000087d0: 7242 0100 0072 4301 0000 726d 0000 0072  rB...rC...rm...r
+000087e0: 4a00 0000 72a6 0000 0072 5200 0000 729a  J...r....rR...r.
+000087f0: 0000 0029 03da 086d 6178 7368 6170 65da  ...)...maxshape.
+00008800: 0663 6875 6e6b 7372 2a00 0000 72ff 0000  .chunksr*...r...
+00008810: 0072 5901 0000 72f3 0000 0072 4100 0000  .rY...r....rA...
+00008820: 7297 0000 00da 0869 6e5f 7261 6e67 6572  r......in_ranger
+00008830: 8300 0000 da0d 6d61 785f 7661 6c5f 7374  ......max_val_st
+00008840: 6163 6b72 5a01 0000 728a 0100 00da 1974  ackrZ...r......t
+00008850: 7269 616c 5f6e 756d 735f 616e 645f 6672  rial_nums_and_fr
+00008860: 616d 655f 6e75 6d73 7296 0000 0072 4501  ame_numsr....rE.
+00008870: 0000 291a 7265 0100 0072 db00 0000 7208  ..).re...r....r.
+00008880: 0000 0072 4801 0000 72ae 0000 0072 4901  ...rH...r....rI.
+00008890: 0000 da0a 4945 4545 5f46 3332 4c45 720b  ....IEEE_F32LEr.
+000088a0: 0000 0072 af00 0000 724e 0100 0072 1d00  ...r....rN...r..
+000088b0: 0000 7236 0000 0072 2100 0000 726d 0100  ..r6...r!...rm..
+000088c0: 0072 2400 0000 722c 0100 0072 3900 0000  .r$...r,...r9...
+000088d0: da0e 6372 6561 7465 5f64 6174 6173 6574  ..create_dataset
+000088e0: 724a 0100 00da 0672 6573 697a 6572 2300  rJ.....resizer#.
+000088f0: 0000 72ad 0000 0072 ed00 0000 7222 0100  ..r....r....r"..
+00008900: 0072 5f00 0000 7279 0000 0029 0e72 a601  .r_...ry...).r..
+00008910: 0000 72a3 0100 0072 4f01 0000 da03 6835  ..r....rO.....h5
+00008920: 6372 3300 0000 72c0 0000 0072 4900 0000  cr3...r....rI...
+00008930: 722c 0000 0072 9a00 0000 5a09 6d61 785f  r,...r....Z.max_
+00008940: 7368 6170 6572 5901 0000 7299 0000 0072  shaperY...r....r
+00008950: ad01 0000 7293 0000 0072 1600 0000 7216  ....r....r....r.
+00008960: 0000 0072 1700 0000 72a4 0100 008a 0500  ...r....r.......
+00008970: 0073 9600 0000 0001 0801 1601 0601 0201  .s..............
+00008980: 0201 0201 0201 0201 0201 0201 0601 0601  ................
+00008990: 02f6 060c 0c01 0e01 1001 2802 1001 0601  ..........(.....
+000089a0: 1001 1401 0c01 0a01 0a01 0802 0601 0801  ................
+000089b0: 0601 0201 0201 02fb 0807 2601 1a02 1001  ..........&.....
+000089c0: 1401 0c01 0a01 0a01 0802 0601 0801 0601  ................
+000089d0: 0201 0201 02fb 0807 2601 2602 0a01 0200  ........&.&.....
+000089e0: 0200 0200 02ff 0402 0401 0801 1a01 0a01  ................
+000089f0: 0c02 0e01 0c01 1001 0c01 0a01 0801 1602  ................
+00008a00: 0601 0eff 0402 1802 0601 0801 72a4 0100  ............r...
+00008a10: 0063 0300 0000 0000 0000 0000 0000 0500  .c..............
+00008a20: 0000 0600 0000 4300 0000 73f4 0000 007c  ......C...s....|
+00008a30: 00a0 0064 0164 02a1 0201 007c 0064 0217  ...d.d.....|.d..
+00008a40: 0064 0317 007d 0374 016a 02a0 037c 03a1  .d...}.t.j...|..
+00008a50: 0172 4a7c 0173 4a74 04a0 0564 04a1 0101  .rJ|.sJt...d....
+00008a60: 0074 04a0 0564 057c 0017 00a1 0101 0074  .t...d.|.......t
+00008a70: 067c 0083 0101 006e a674 016a 02a0 037c  .|.....n.t.j...|
+00008a80: 03a1 0172 6a74 01a0 077c 03a1 0101 0074  ...rjt...|.....t
+00008a90: 08a0 097c 02a1 0101 0074 0a83 007d 047c  ...|.....t...}.|
+00008aa0: 007c 0464 063c 0074 0b74 0ca0 0c7c 0064  .|.d.<.t.t...|.d
+00008ab0: 0717 00a1 0183 017c 0464 083c 0074 0da0  .......|.d.<.t..
+00008ac0: 0e74 0da0 0f7c 0464 0819 00a1 0164 09a1  .t...|.d.....d..
+00008ad0: 027c 0464 0a3c 0064 0b7c 0464 0c3c 0074  .|.d.<.d.|.d.<.t
+00008ae0: 0664 0d83 0101 0074 107c 0464 0819 0083  .d.....t.|.d....
+00008af0: 017c 0464 0e3c 0064 097c 0464 0f3c 0064  .|.d.<.d.|.d.<.d
+00008b00: 1064 1184 007c 0464 0819 0044 0083 017c  .d...|.d...D...|
+00008b10: 0464 083c 0074 117c 047c 0383 0201 0064  .d.<.t.|.|.....d
+00008b20: 1253 0029 1361 0002 0000 0a0a 2020 2020  .S.).a......    
+00008b30: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00008b40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7669  ---------.    vi
+00008b50: 6465 6f5f 6469 7265 6374 6f72 7920 3a20  deo_directory : 
+00008b60: 2077 696c 6c20 6c6f 6f6b 2069 6e20 616c   will look in al
+00008b70: 6c20 7375 6220 6469 7265 6374 6f72 6965  l sub directorie
+00008b80: 7373 2072 6563 7572 6976 6c79 0a20 2020  ss recurivly.   
+00008b90: 206f 7665 7277 7269 7465 203a 2069 6620   overwrite : if 
+00008ba0: 5472 7565 2077 696c 6c20 6465 6c65 7465  True will delete
+00008bb0: 2066 696c 6520 6966 2065 7869 7374 730a   file if exists.
+00008bc0: 2020 2020 7469 6d65 5f73 6c65 6570 5f62      time_sleep_b
+00008bd0: 6574 7765 656e 5f64 656c 6574 655f 666f  etween_delete_fo
+00008be0: 725f 636c 6f75 645f 7570 6461 7465 203a  r_cloud_update :
+00008bf0: 2068 6163 6b79 2073 6f6c 7574 696f 6e20   hacky solution 
+00008c00: 746f 2067 6f6f 676c 6520 6472 6976 6520  to google drive 
+00008c10: 6361 6368 6520 6973 7375 6520 7768 6572  cache issue wher
+00008c20: 6520 7468 6520 6d6f 6469 6669 6564 2064  e the modified d
+00008c30: 6174 6120 7469 6d65 0a20 2020 2064 6f65  ata time.    doe
+00008c40: 7320 6e6f 7420 7570 6461 7465 2077 6974  s not update wit
+00008c50: 686f 7574 2061 2074 696d 6520 6275 6666  hout a time buff
+00008c60: 6572 2061 6674 6572 2062 6569 6e67 2064  er after being d
+00008c70: 656c 6574 652e 206f 6e6c 7920 7265 6c69  elete. only reli
+00008c80: 7665 6e74 2066 6f72 2069 6620 796f 7520  vent for if you 
+00008c90: 6172 6520 6f76 6572 7772 6974 696e 6720  are overwriting 
+00008ca0: 6578 6973 7469 6e67 2066 696c 6573 2c20  existing files, 
+00008cb0: 490a 2020 2020 6b6e 6f77 2033 3020 7365  I.    know 30 se
+00008cc0: 636f 6e64 7320 776f 726b 7320 6865 7265  conds works here
+00008cd0: 2c20 616e 6e6f 7969 6e67 2062 7574 206e  , annoying but n
+00008ce0: 6f74 2074 6861 7420 6269 6720 6f66 2061  ot that big of a
+00008cf0: 2064 6561 6c20 6174 2074 6865 2065 6e64   deal at the end
+00008d00: 206f 6620 7468 6520 6461 790a 0a20 2020   of the day..   
+00008d10: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00008d20: 2d2d 2d2d 0a0a 2020 2020 7256 0100 0072  ----..    rV...r
+00008d30: 5501 0000 7a22 6669 6c65 5f6c 6973 745f  U...z"file_list_
+00008d40: 666f 725f 6261 7463 685f 7072 6f63 6573  for_batch_proces
+00008d50: 7369 6e67 2e70 6b6c 6158 0100 0077 6172  sing.pklaX...war
+00008d60: 6e69 6e67 2066 696c 6520 616c 7265 6164  ning file alread
+00008d70: 7920 6578 6973 7473 2120 6966 2079 6f75  y exists! if you
+00008d80: 206f 7665 7277 7269 7465 2061 2070 6172   overwrite a par
+00008d90: 7469 616c 6c79 2070 726f 6365 7373 6564  tially processed
+00008da0: 2064 6972 6563 746f 7279 2c20 796f 7520   directory, you 
+00008db0: 7769 6c6c 2065 7870 6572 6965 6e63 6520  will experience 
+00008dc0: 6973 7375 6573 206c 696b 6520 6f76 6572  issues like over
+00008dd0: 7772 6974 6520 6572 726f 7273 2c20 616e  write errors, an
+00008de0: 6420 796f 7527 6c6c 206c 6f73 6520 796f  d you'll lose yo
+00008df0: 7572 2070 726f 6772 6573 732e 2069 6620  ur progress. if 
+00008e00: 796f 7520 6172 6520 7375 7265 2079 6f75  you are sure you
+00008e10: 2077 616e 7420 746f 206f 7665 7277 7269   want to overwri
+00008e20: 7465 206d 616b 6520 7375 7265 2074 6f20  te make sure to 
+00008e30: 6465 6c65 7465 2074 6865 2063 6f72 7265  delete the corre
+00008e40: 7370 6f6e 6469 6e67 2027 5f46 494e 4953  sponding '_FINIS
+00008e50: 4845 4427 2064 6972 6563 746f 7279 2c20  HED' directory, 
+00008e60: 616e 6420 6966 206e 6563 6573 7361 7279  and if necessary
+00008e70: 206d 6f76 6520 7468 6520 6d70 3473 2062   move the mp4s b
+00008e80: 6163 6b20 746f 2074 6865 2070 726f 6365  ack to the proce
+00008e90: 7373 696e 6720 666f 6c64 6572 2061 6e64  ssing folder and
+00008ea0: 2073 6574 206f 7665 7277 7269 7465 203d   set overwrite =
+00008eb0: 2054 7275 657a 4174 6869 7320 6162 6f76   TruezAthis abov
+00008ec0: 6520 6d65 7373 6167 6520 6973 2069 6e20  e message is in 
+00008ed0: 7265 6665 7265 6e63 6520 746f 2074 6865  reference to the
+00008ee0: 2066 6f6c 6c6f 7769 6e67 2064 6972 6563   following direc
+00008ef0: 746f 7279 2e2e 2e0a 5a16 6f72 6967 696e  tory....Z.origin
+00008f00: 616c 5f6d 7034 5f64 6972 6563 746f 7279  al_mp4_directory
+00008f10: 7a06 2f2a 2e6d 7034 7288 0100 0046 7289  z./*.mp4r....Fr.
+00008f20: 0100 007a 4579 6f75 2063 616e 2070 7574  ...zEyou can put
+00008f30: 2061 6e79 206e 6f74 6573 2068 6572 6520   any notes here 
+00008f40: 6469 7265 6374 6c79 2066 726f 6d20 7468  directly from th
+00008f50: 6520 7465 7874 2066 696c 6520 6966 2079  e text file if y
+00008f60: 6f75 2077 616e 7420 746f 5a05 4e4f 5445  ou want toZ.NOTE
+00008f70: 537a 5250 6572 666f 726d 696e 6720 696e  SzRPerforming in
+00008f80: 6974 6961 6c20 6368 6563 6b20 746f 2073  itial check to s
+00008f90: 6565 2069 6620 736f 6d65 204d 5034 7320  ee if some MP4s 
+00008fa0: 6172 6520 2262 6164 2220 6279 2074 6573  are "bad" by tes
+00008fb0: 7469 6e67 2069 6620 4650 5320 6973 2061  ting if FPS is a
+00008fc0: 6e20 696e 7472 8701 0000 7286 0100 0063  n intr....r....c
+00008fd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00008fe0: 0600 0000 5300 0000 7318 0000 0067 007c  ....S...s....g.|
+00008ff0: 005d 107d 017c 01a0 0064 0064 01a1 0291  .].}.|...d.d....
+00009000: 0271 0453 0029 0272 5601 0000 7255 0100  .q.S.).rV...rU..
+00009010: 0072 6601 0000 7231 0000 0072 1600 0000  .rf...r1...r....
+00009020: 7216 0000 0072 1700 0000 7234 0000 002d  r....r....r4...-
+00009030: 0600 0073 0400 0000 0600 0200 7a26 6d61  ...s........z&ma
+00009040: 6b65 5f6d 7034 5f6c 6973 745f 6469 6374  ke_mp4_list_dict
+00009050: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00009060: 6f6d 703e 4e29 1272 b700 0000 725f 0000  omp>N).r....r_..
+00009070: 0072 6100 0000 72a9 0000 0072 8f00 0000  .ra...r....r....
+00009080: 7290 0000 0072 4b00 0000 7279 0000 0072  r....rK...ry...r
+00009090: 9a01 0000 da05 736c 6565 7072 6900 0000  ......sleepri...
+000090a0: 7265 0100 00da 0467 6c6f 6272 1d00 0000  re.....globr....
+000090b0: da04 6675 6c6c 7221 0000 0072 ce00 0000  ..fullr!...r....
+000090c0: 729d 0100 0029 0572 a000 0000 725c 0000  r....).r....r\..
+000090d0: 005a 2a74 696d 655f 736c 6565 705f 6265  .Z*time_sleep_be
+000090e0: 7477 6565 6e5f 6465 6c65 7465 5f66 6f72  tween_delete_for
+000090f0: 5f63 6c6f 7564 5f75 7064 6174 6572 4f01  _cloud_updaterO.
+00009100: 0000 5a04 746d 7064 7216 0000 0072 1600  ..Z.tmpdr....r..
+00009110: 0000 7217 0000 00da 126d 616b 655f 6d70  ..r......make_mp
+00009120: 345f 6c69 7374 5f64 6963 7406 0600 0073  4_list_dict....s
+00009130: 2600 0000 0010 0c01 0c02 1001 0a04 0e01  &...............
+00009140: 0a03 0c01 0a01 0a01 0601 0801 1601 1a01  ................
+00009150: 0801 0801 1001 0801 1602 72b5 0100 0063  ..........r....c
+00009160: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00009170: 0300 0000 4300 0000 731c 0000 007c 0064  ....C...s....|.d
+00009180: 0164 0085 0219 0064 026b 0372 187c 0064  .d.....d.k.r.|.d
+00009190: 0217 0053 007c 0053 0029 034e 7280 0000  ...S.|.S.).Nr...
+000091a0: 0072 9401 0000 7216 0000 0029 01da 046e  .r....r....)...n
+000091b0: 616d 6572 1600 0000 7216 0000 0072 1700  amer....r....r..
+000091c0: 0000 da0a 5f63 6865 636b 5f70 6b6c 3206  ...._check_pkl2.
+000091d0: 0000 7306 0000 0000 0110 0108 0172 b701  ..s..........r..
+000091e0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+000091f0: 0000 0009 0000 0043 0000 0073 2e00 0000  .......C...s....
+00009200: 7400 7401 7c01 8301 6401 8302 8f16 7d02  t.t.|...d.....}.
+00009210: 7402 6a03 7c00 7c02 6402 6403 8d03 0100  t.j.|.|.d.d.....
+00009220: 5700 3500 5100 5200 5800 6400 5300 2904  W.5.Q.R.X.d.S.).
+00009230: 4eda 0277 6272 d900 0000 2901 da08 7072  N..wbr....)...pr
+00009240: 6f74 6f63 6f6c 2904 da04 6f70 656e 72b7  otocol)...openr.
+00009250: 0100 00da 0670 6963 6b6c 65da 0464 756d  .....pickle..dum
+00009260: 7029 03da 036f 626a 72b6 0100 0072 a501  p)...objr....r..
+00009270: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00009280: 0072 9d01 0000 3806 0000 7304 0000 0000  .r....8...s.....
+00009290: 0110 0272 9d01 0000 6301 0000 0000 0000  ...r....c.......
+000092a0: 0000 0000 0002 0000 000a 0000 0043 0000  .............C..
+000092b0: 0073 3000 0000 7400 7401 7c00 8301 6401  .s0...t.t.|...d.
+000092c0: 8302 8f18 7d01 7402 a003 7c01 a101 5700  ....}.t...|...W.
+000092d0: 0200 3500 5100 5200 a300 5300 5100 5200  ..5.Q.R...S.Q.R.
+000092e0: 5800 6400 5300 2902 4eda 0272 6229 0472  X.d.S.).N..rb).r
+000092f0: ba01 0000 72b7 0100 0072 bb01 0000 da04  ....r....r......
+00009300: 6c6f 6164 2902 72b6 0100 0072 a501 0000  load).r....r....
+00009310: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00009320: 6300 0000 3e06 0000 7304 0000 0000 0110  c...>...s.......
+00009330: 0172 6300 0000 6300 0000 0000 0000 0000  .rc...c.........
+00009340: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00009350: 1200 0000 7400 6a01 a002 7403 6a04 a101  ....t.j...t.j...
+00009360: 7d00 7c00 5300 720d 0100 0029 0572 5f00  }.|.S.r....).r_.
+00009370: 0000 7261 0000 0072 a700 0000 da05 7768  ..ra...r......wh
+00009380: 6163 63da 085f 5f66 696c 655f 5f72 6f00  acc..__file__ro.
+00009390: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000093a0: 0072 5e00 0000 4306 0000 7304 0000 0000  .r^...C...s.....
+000093b0: 010e 0172 5e00 0000 6300 0000 0000 0000  ...r^...c.......
+000093c0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000093d0: 0073 3000 0000 7400 8300 6401 1700 7d00  .s0...t...d...}.
+000093e0: 7401 7c00 6402 1700 8301 7d01 7402 a003  t.|.d.....}.t...
+000093f0: 7c01 6403 1900 a101 6404 1900 7c01 6405  |.d.....d...|.d.
+00009400: 3c00 7c01 5300 2906 4efa 192f 7768 6163  <.|.S.).N../whac
+00009410: 635f 6461 7461 2f66 6561 7475 7265 5f64  c_data/feature_d
+00009420: 6174 612f 7a15 6665 6174 7572 655f 6461  ata/z.feature_da
+00009430: 7461 5f64 6963 742e 706b 6c5a 1c66 696e  ta_dict.pklZ.fin
+00009440: 616c 5f73 656c 6563 7465 645f 6665 6174  al_selected_feat
+00009450: 7572 6573 5f62 6f6f 6c72 0100 0000 5a17  ures_boolr....Z.
+00009460: 6669 6e61 6c5f 7365 6c65 6374 6564 5f66  final_selected_f
+00009470: 6561 7475 7265 7329 0472 5e00 0000 7263  eatures).r^...rc
+00009480: 0000 0072 1d00 0000 72b9 0000 0029 0272  ...r....r....).r
+00009490: 5300 0000 726b 0000 0072 1600 0000 7216  S...rk...r....r.
+000094a0: 0000 0072 1700 0000 da11 6c6f 6164 5f66  ...r......load_f
+000094b0: 6561 7475 7265 5f64 6174 6148 0600 0073  eature_dataH...s
+000094c0: 0800 0000 0001 0a01 0c01 1601 72c3 0100  ............r...
+000094d0: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
+000094e0: 0000 0300 0000 4300 0000 731a 0000 0074  ......C...s....t
+000094f0: 0083 0064 0117 007d 0074 017c 0064 0217  ...d...}.t.|.d..
+00009500: 0083 017d 017c 0153 0029 034e 72c2 0100  ...}.|.S.).Nr...
+00009510: 007a 1b73 7461 7274 5f65 6e64 5f6e 616e  .z.start_end_nan
+00009520: 5f6c 6f63 6174 696f 6e73 2e70 6b6c 2902  _locations.pkl).
+00009530: 725e 0000 0072 6300 0000 2902 7253 0000  r^...rc...).rS..
+00009540: 005a 0961 7272 6179 5f6f 7574 7216 0000  .Z.array_outr...
+00009550: 0072 1600 0000 7217 0000 0072 1a00 0000  .r....r....r....
+00009560: 4f06 0000 7306 0000 0000 010a 010c 0172  O...s..........r
+00009570: 1a00 0000 72d9 0000 0063 0100 0000 0000  ....r....c......
+00009580: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00009590: 0000 7336 0000 0074 0083 007d 017c 0164  ..s6...t...}.|.d
+000095a0: 0119 007d 0274 01a0 027c 027c 006b 05a1  ...}.t...|.|.k..
+000095b0: 0164 0219 007d 0364 0364 0484 0074 0364  .d...}.d.d...t.d
+000095c0: 0583 0144 0083 017d 047c 0353 0029 0661  ...D...}.|.S.).a
+000095d0: d601 0000 0a20 2020 2050 6172 616d 6574  .....    Paramet
+000095e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000095f0: 2d2d 0a20 2020 2067 7265 6174 6572 5f74  --.    greater_t
+00009600: 6861 6e5f 6f72 5f65 7175 616c 5f74 6f20  han_or_equal_to 
+00009610: 3a20 3020 6d65 616e 7320 7365 6c65 6374  : 0 means select
+00009620: 2061 6c6c 2066 6561 7475 7265 732c 2031   all features, 1
+00009630: 3020 6d65 616e 7320 6f6e 6c79 2074 6865  0 means only the
+00009640: 2066 6561 7475 7265 7320 7468 6174 2077   features that w
+00009650: 6572 6520 7573 6520 696e 2045 5645 5259  ere use in EVERY
+00009660: 2074 6573 740a 2020 2020 6c69 6768 7420   test.    light 
+00009670: 4742 4d20 6d6f 6465 6c2e 204e 6f74 653a  GBM model. Note:
+00009680: 2074 6865 2073 6176 6520 4c69 6768 7420   the save Light 
+00009690: 4742 4d20 286d 6f64 656c 2920 6973 2074  GBM (model) is t
+000096a0: 7261 696e 6564 206f 6e20 6772 6561 7465  rained on greate
+000096b0: 725f 7468 616e 5f6f 725f 6571 7561 6c5f  r_than_or_equal_
+000096c0: 746f 203d 2034 2c20 736f 2079 6f75 2063  to = 4, so you c
+000096d0: 616e 2063 6861 6e67 6520 7468 6973 0a20  an change this. 
+000096e0: 2020 2062 7574 2079 6f75 2077 696c 6c20     but you will 
+000096f0: 6e65 6564 2074 6f20 7265 7472 6169 6e20  need to retrain 
+00009700: 7468 6520 6c69 6768 7420 4742 4d20 286d  the light GBM (m
+00009710: 6f64 656c 292e 0a20 2020 2052 6574 7572  odel)..    Retur
+00009720: 6e73 206b 6565 705f 6665 6174 7572 6573  ns keep_features
+00009730: 5f69 6e64 6578 203a 2069 6e64 6578 2074  _index : index t
+00009740: 6f20 7468 6520 6769 616e 7420 2738 342c  o the giant '84,
+00009750: 3030 3927 2066 6561 7475 7265 732c 206e  009' features, n
+00009760: 6f74 6520 6772 6561 7465 725f 7468 616e  ote greater_than
+00009770: 5f6f 725f 6571 7561 6c5f 746f 203d 2034  _or_equal_to = 4
+00009780: 2072 6574 7572 6e20 3330 3935 0a20 2020   return 3095.   
+00009790: 2066 6561 7475 7265 730a 2020 2020 2d2d   features.    --
+000097a0: 2d2d 2d2d 2d0a 2020 2020 5a13 6665 6174  -----.    Z.feat
+000097b0: 7572 6573 5f75 7365 645f 6f66 5f31 3072  ures_used_of_10r
+000097c0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000097d0: 0002 0000 0004 0000 0053 0000 0073 1c00  .........S...s..
+000097e0: 0000 6700 7c00 5d14 7d01 7c01 7400 6b06  ..g.|.].}.|.t.k.
+000097f0: 7214 6400 6e02 6401 9102 7104 5300 2902  r.d.n.d...q.S.).
+00009800: 5446 72d1 0000 0072 3100 0000 7216 0000  TFr....r1...r...
+00009810: 0072 1600 0000 7217 0000 0072 3400 0000  .r....r....r4...
+00009820: 6a06 0000 7304 0000 0006 0002 007a 2967  j...s........z)g
+00009830: 6574 5f73 656c 6563 7465 645f 6665 6174  et_selected_feat
+00009840: 7572 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ures.<locals>.<l
+00009850: 6973 7463 6f6d 703e 6929 4801 0029 0472  istcomp>i)H..).r
+00009860: c301 0000 721d 0000 0072 b900 0000 723a  ....r....r....r:
+00009870: 0000 0029 055a 1867 7265 6174 6572 5f74  ...).Z.greater_t
+00009880: 6861 6e5f 6f72 5f65 7175 616c 5f74 6f72  han_or_equal_tor
+00009890: 2501 0000 5a12 6665 6174 7572 6573 5f6f  %...Z.features_o
+000098a0: 7574 5f6f 665f 3130 5a13 6b65 6570 5f66  ut_of_10Z.keep_f
+000098b0: 6561 7475 7265 735f 696e 6465 785a 1866  eatures_indexZ.f
+000098c0: 6561 7475 7265 735f 7573 6564 5f6f 665f  eatures_used_of_
+000098d0: 3130 5f62 6f6f 6c72 1600 0000 7216 0000  10_boolr....r...
+000098e0: 0072 1700 0000 da15 6765 745f 7365 6c65  .r......get_sele
+000098f0: 6374 6564 5f66 6561 7475 7265 7359 0600  cted_featuresY..
+00009900: 0073 0a00 0000 000c 0601 0802 1202 1201  .s..............
+00009910: 72c4 0100 0063 0000 0000 0000 0000 0000  r....c..........
+00009920: 0000 0200 0000 0800 0000 4300 0000 7366  ..........C...sf
+00009930: 0000 007a 4a74 0074 0183 006a 0283 017d  ...zJt.t...j...}
+00009940: 0074 0183 006a 026a 037d 0164 017c 006b  .t...j.j.}.d.|.k
+00009950: 0672 2657 0064 0253 007c 0164 036b 0272  .r&W.d.S.|.d.k.r
+00009960: 3457 0064 0253 007c 0164 046b 0272 4257  4W.d.S.|.d.k.rBW
+00009970: 0064 0553 0057 0064 0553 0057 006e 1604  .d.S.W.d.S.W.n..
+00009980: 0074 046b 0a72 6001 0001 0001 0059 0064  .t.k.r`......Y.d
+00009990: 0553 0058 0064 0053 0029 064e 5a05 636f  .S.X.d.S.).NZ.co
+000099a0: 6c61 6254 5a13 5a4d 5149 6e74 6572 6163  labTZ.ZMQInterac
+000099b0: 7469 7665 5368 656c 6c5a 1854 6572 6d69  tiveShellZ.Termi
+000099c0: 6e61 6c49 6e74 6572 6163 7469 7665 5368  nalInteractiveSh
+000099d0: 656c 6c46 2905 72ad 0000 00da 0b67 6574  ellF).r......get
+000099e0: 5f69 7079 7468 6f6e da09 5f5f 636c 6173  _ipython..__clas
+000099f0: 735f 5f72 7701 0000 da09 4e61 6d65 4572  s__rw.....NameEr
+00009a00: 726f 7229 0272 e600 0000 da05 7368 656c  ror).r......shel
+00009a10: 6c72 1600 0000 7216 0000 0072 1700 0000  lr....r....r....
+00009a20: da0a 6973 6e6f 7465 626f 6f6b 6e06 0000  ..isnotebookn...
+00009a30: 7318 0000 0000 0102 010c 010a 0108 0106  s...............
+00009a40: 0108 0106 0108 0106 020a 010e 0172 c901  .............r..
+00009a50: 0000 6301 0000 0000 0000 0000 0000 0004  ..c.............
+00009a60: 0000 0007 0000 0043 0000 0073 3c00 0000  .......C...s<...
+00009a70: 7400 a001 7c00 a101 7d01 7400 a001 6401  t...|...}.t...d.
+00009a80: 6701 7402 7400 a003 7c01 a101 8301 1700  g.t.t...|.......
+00009a90: a101 7d02 7c01 7c02 1700 7d03 6402 7c03  ..}.|.|...}.d.|.
+00009aa0: 7c03 6403 6b02 3c00 7c03 5300 2904 4e72  |.d.k.<.|.S.).Nr
+00009ab0: 0100 0000 7246 0000 0072 4a00 0000 2904  ....rF...rJ...).
+00009ac0: 721d 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
+00009ad0: 9e01 0000 2904 7253 0000 0072 e500 0000  ....).rS...r....
+00009ae0: 7242 0000 0072 e600 0000 7216 0000 0072  rB...r....r....r
+00009af0: 1600 0000 7217 0000 00da 1d66 6f75 725f  ....r......four_
+00009b00: 636c 6173 735f 6c61 6265 6c73 5f66 726f  class_labels_fro
+00009b10: 6d5f 6269 6e61 7279 8406 0000 730a 0000  m_binary....s...
+00009b20: 0000 010a 011a 0108 010c 0172 ca01 0000  ...........r....
+00009b30: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
+00009b40: 000a 0000 0043 0000 0073 4e00 0000 7400  .....C...sN...t.
+00009b50: a001 7c00 6401 a102 8f38 7d03 7402 a003  ..|.d....8}.t...
+00009b60: 7404 7c03 a005 a100 8301 a101 7d04 7c02  t.|.........}.|.
+00009b70: 722c 7406 7c04 8301 0100 7c01 7240 7c04  r,t.|.....|.r@|.
+00009b80: 5700 0200 3500 5100 5200 a300 5300 5700  W...5.Q.R...S.W.
+00009b90: 3500 5100 5200 5800 6400 5300 2902 4e72  5.Q.R.X.d.S.).Nr
+00009ba0: 6d00 0000 2907 72ae 0000 0072 af00 0000  m...).r....r....
+00009bb0: 721b 0000 0072 1c00 0000 7239 0000 0072  r....r....r9...r
+00009bc0: 9900 0000 da14 7072 696e 745f 6c69 7374  ......print_list
+00009bd0: 5f77 6974 685f 696e 6473 2905 5a06 6835  _with_inds).Z.h5
+00009be0: 6669 6c65 da0b 7265 7475 726e 5f6c 6973  file..return_lis
+00009bf0: 74da 0864 6f5f 7072 696e 7472 c000 0000  t..do_printr....
+00009c00: 7253 0000 0072 1600 0000 7216 0000 0072  rS...r....r....r
+00009c10: 1700 0000 72ab 0000 008c 0600 0073 0c00  ....r........s..
+00009c20: 0000 0001 0e01 1201 0401 0801 0401 72ab  ..............r.
+00009c30: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00009c40: 0600 0000 0c00 0000 4300 0000 739c 0000  ........C...s...
+00009c50: 007c 0364 006b 0872 0c7c 027d 0374 00a0  .|.d.k.r.|.}.t..
+00009c60: 017c 0064 01a1 028f 7a7d 0474 00a0 017c  .|.d....z}.t...|
+00009c70: 0164 02a1 028f 627d 057a 207c 047c 0219  .d....b}.z |.|..
+00009c80: 0064 0064 0085 0219 007c 057c 0319 0064  .d.d.....|.|...d
+00009c90: 0064 0085 023c 0057 006e 3a01 0001 0001  .d...<.W.n:.....
+00009ca0: 007c 056a 027c 0374 03a0 047c 047c 0219  .|.j.|.t...|.|..
+00009cb0: 0064 0064 0085 0219 00a1 017c 047c 0219  .d.d.......|.|..
+00009cc0: 0064 0064 0085 0219 0064 038d 0301 0059  .d.d.....d.....Y
+00009cd0: 006e 0258 0057 0035 0051 0052 0058 0057  .n.X.W.5.Q.R.X.W
+00009ce0: 0035 0051 0052 0058 0064 0053 0029 044e  .5.Q.R.X.d.S.).N
+00009cf0: 726d 0000 0072 a600 0000 a902 7221 0000  rm...r......r!..
+00009d00: 0072 2a00 0000 2905 72ae 0000 0072 af00  .r*...).r....r..
+00009d10: 0000 72af 0100 0072 1d00 0000 7221 0000  ..r....r....r!..
+00009d20: 0029 065a 0f68 355f 746f 5f63 6f70 795f  .).Z.h5_to_copy_
+00009d30: 6672 6f6d 5a0d 6835 5f74 6f5f 636f 7079  fromZ.h5_to_copy
+00009d40: 5f74 6f5a 196c 6162 656c 5f73 7472 696e  _toZ.label_strin
+00009d50: 675f 746f 5f63 6f70 795f 6672 6f6d 5a17  g_to_copy_fromZ.
+00009d60: 6c61 6265 6c5f 7374 7269 6e67 5f74 6f5f  label_string_to_
+00009d70: 636f 7079 5f74 6f72 c000 0000 da02 6832  copy_tor......h2
+00009d80: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00009d90: 1963 6f70 795f 6835 5f6b 6579 5f74 6f5f  .copy_h5_key_to_
+00009da0: 616e 6f74 6865 725f 6835 9506 0000 7314  another_h5....s.
+00009db0: 0000 0000 0108 0104 010e 010e 0102 0120  ............... 
+00009dc0: 0106 011a 010e ff72 d001 0000 2901 da06  .......r....)...
+00009dd0: 7265 7475 726e 6304 0000 0000 0000 0000  returnc.........
+00009de0: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
+00009df0: 0c01 0000 7400 7c00 8301 6401 6b02 7218  ....t.|...d.k.r.
+00009e00: 7401 6402 8301 0100 7c00 5300 6403 6404  t.d.....|.S.d.d.
+00009e10: 8400 7d04 7402 7c01 7403 8302 7230 7c01  ..}.t.|.t...r0|.
+00009e20: 6701 7d01 7402 7c02 7403 8302 7240 7c02  g.}.t.|.t...r@|.
+00009e30: 6701 7d02 7404 a005 6405 6701 7400 7c00  g.}.t...d.g.t.|.
+00009e40: 8301 1400 a101 7d05 7c01 4400 5d18 7d06  ......}.|.D.].}.
+00009e50: 7404 a006 7c05 7c04 7c00 7c06 8302 6602  t...|.|.|.|...f.
+00009e60: a101 7d05 7158 7404 6a07 7c05 6401 6406  ..}.qXt.j.|.d.d.
+00009e70: 8d02 6401 6b04 7d05 7404 a005 6407 6701  ..d.k.}.t...d.g.
+00009e80: 7400 7c00 8301 1400 a101 7d07 7c02 6400  t.|.......}.|.d.
+00009e90: 6b09 72d6 7c02 4400 5d1e 7d06 7404 a006  k.r.|.D.].}.t...
+00009ea0: 7c07 7404 a008 7c04 7c00 7c06 8302 a101  |.t...|.|.|.....
+00009eb0: 6602 a101 7d07 71a4 7404 6a09 7c07 6401  f...}.q.t.j.|.d.
+00009ec0: 6406 8d02 6401 6b04 7d07 7c05 7c07 1400  d...d.k.}.|.|...
+00009ed0: 7d08 7c08 6a0a 6401 6b01 72ec 6700 5300  }.|.j.d.k.r.g.S.
+00009ee0: 7404 a005 7c00 a101 7c08 1900 7d09 7c03  t...|...|...}.|.
+00009ef0: 9001 7208 7c09 7c08 6602 5300 7c09 5300  ..r.|.|.f.S.|.S.
+00009f00: 2908 4e72 0100 0000 7a24 696e 5f6c 6973  ).Nr....z$in_lis
+00009f10: 7420 7761 7320 656d 7074 792c 2072 6574  t was empty, ret
+00009f20: 7572 6e69 6e67 2069 6e5f 6c69 7374 6302  urning in_listc.
+00009f30: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00009f40: 0000 0013 0000 0073 1800 0000 7400 a001  .......s....t...
+00009f50: 8700 6601 6401 6402 8408 7c00 4400 8301  ..f.d.d...|.D...
+00009f60: a101 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
+00009f70: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00009f80: 7314 0000 0067 007c 005d 0c7d 0188 007c  s....g.|.].}...|
+00009f90: 016b 0691 0271 0453 0072 1600 0000 7216  .k...q.S.r....r.
+00009fa0: 0000 0029 0272 3200 0000 da06 7374 7269  ...).r2.....stri
+00009fb0: 6e67 a901 da0a 636d 705f 7374 7269 6e67  ng....cmp_string
+00009fc0: 7216 0000 0072 1700 0000 7234 0000 00a7  r....r....r4....
+00009fd0: 0600 0073 0400 0000 0600 0200 7a3c 6c69  ...s........z<li
+00009fe0: 7374 6572 5f69 742e 3c6c 6f63 616c 733e  ster_it.<locals>
+00009ff0: 2e69 6e64 6578 5f6c 6973 745f 6f66 5f73  .index_list_of_s
+0000a000: 7472 696e 6773 2e3c 6c6f 6361 6c73 3e2e  trings.<locals>.
+0000a010: 3c6c 6973 7463 6f6d 703e 2902 721d 0000  <listcomp>).r...
+0000a020: 0072 3800 0000 2902 5a08 696e 5f6c 6973  .r8...).Z.in_lis
+0000a030: 7432 72d4 0100 0072 1600 0000 72d3 0100  t2r....r....r...
+0000a040: 0072 1700 0000 da15 696e 6465 785f 6c69  .r......index_li
+0000a050: 7374 5f6f 665f 7374 7269 6e67 73a6 0600  st_of_strings...
+0000a060: 0073 0200 0000 0001 7a28 6c69 7374 6572  .s......z(lister
+0000a070: 5f69 742e 3c6c 6f63 616c 733e 2e69 6e64  _it.<locals>.ind
+0000a080: 6578 5f6c 6973 745f 6f66 5f73 7472 696e  ex_list_of_strin
+0000a090: 6773 4672 ff00 0000 5429 0b72 3000 0000  gsFr....T).r0...
+0000a0a0: 724b 0000 0072 0b01 0000 72ad 0000 0072  rK...r....r....r
+0000a0b0: 1d00 0000 7238 0000 0072 2500 0000 7235  ....r8...r%...r5
+0000a0c0: 0000 00da 0669 6e76 6572 74da 0770 726f  .....invert..pro
+0000a0d0: 6475 6374 7230 0100 0029 0a5a 0769 6e5f  ductr0...).Z.in_
+0000a0e0: 6c69 7374 da0c 6b65 6570 5f73 7472 696e  list..keep_strin
+0000a0f0: 6773 da0d 7265 6d6f 7665 5f73 7472 696e  gs..remove_strin
+0000a100: 675a 1172 6574 7572 6e5f 626f 6f6c 5f69  gZ.return_bool_i
+0000a110: 6e64 6578 72d5 0100 005a 066b 6565 705f  ndexr....Z.keep_
+0000a120: 6972 3300 0000 5a08 7265 6d6f 7665 5f69  ir3...Z.remove_i
+0000a130: 722b 0000 0072 9300 0000 7216 0000 0072  r+...r....r....r
+0000a140: 1600 0000 7217 0000 00da 096c 6973 7465  ....r......liste
+0000a150: 725f 6974 a106 0000 7330 0000 0000 010c  r_it....s0......
+0000a160: 0108 0104 0208 030a 0006 010a 0006 0214  ................
+0000a170: 0108 0116 0112 0214 0108 0108 011c 0112  ................
+0000a180: 0208 010a 0104 020e 0106 0108 0172 da01  .............r..
+0000a190: 0000 6301 0000 0000 0000 0000 0000 0004  ..c.............
+0000a1a0: 0000 0009 0000 0043 0000 0073 4600 0000  .......C...sF...
+0000a1b0: 7400 a001 7c00 6401 a102 8f30 7d01 7402  t...|.d....0}.t.
+0000a1c0: 7c01 6402 1900 6400 6400 8502 1900 8301  |.d...d.d.......
+0000a1d0: 4400 5d14 5c02 7d02 7d03 7403 a004 7c02  D.].\.}.}.t...|.
+0000a1e0: 7c03 a102 0100 7122 5700 3500 5100 5200  |.....q"W.5.Q.R.
+0000a1f0: 5800 6400 5300 2903 4e72 6d00 0000 72ac  X.d.S.).Nrm...r.
+0000a200: 0100 0029 0572 ae00 0000 72af 0000 0072  ...).r....r....r
+0000a210: 2400 0000 7211 0000 00da 0470 6c6f 7429  $...r......plot)
+0000a220: 04da 0768 355f 6669 6c65 da02 6866 722c  ...h5_file..hfr,
+0000a230: 0000 0072 3300 0000 7216 0000 0072 1600  ...r3...r....r..
+0000a240: 0000 7217 0000 00da 1b70 6c6f 745f 706f  ..r......plot_po
+0000a250: 6c65 5f74 7261 636b 696e 675f 6d61 785f  le_tracking_max_
+0000a260: 7661 6c73 e806 0000 7306 0000 0000 010e  vals....s.......
+0000a270: 011c 0172 de01 0000 e928 0000 0063 0500  ...r.....(...c..
+0000a280: 0000 0000 0000 0000 0000 1800 0000 0600  ................
+0000a290: 0000 4300 0000 73ee 0200 0064 0164 0284  ..C...s....d.d..
+0000a2a0: 007d 0567 007d 0667 007d 0767 007d 0867  .}.g.}.g.}.g.}.g
+0000a2b0: 007d 0974 007c 0083 0144 005d da7d 0a7c  .}.t.|...D.].}.|
+0000a2c0: 0264 036b 0872 987c 0a64 0419 0064 056b  .d.k.r.|.d...d.k
+0000a2d0: 0372 9874 0174 0274 0364 067c 0a17 0083  .r.t.t.t.d.|....
+0000a2e0: 0183 0183 017d 0b7c 09a0 047c 0ba0 0564  .....}.|...|...d
+0000a2f0: 07a1 0164 0819 00a1 0101 007c 06a0 047c  ...d.......|...|
+0000a300: 0aa1 0101 007c 0574 0364 067c 0664 0919  .....|.t.d.|.d..
+0000a310: 0017 0083 0183 015c 027d 0c7d 0d7c 07a0  .......\.}.}.|..
+0000a320: 047c 0ca1 0101 007c 08a0 047c 0da1 0101  .|.....|...|....
+0000a330: 0071 207c 0272 2074 0174 0274 0364 067c  .q |.r t.t.t.d.|
+0000a340: 0a17 0083 0183 0183 017d 0b7c 09a0 047c  .........}.|...|
+0000a350: 0ba0 0564 07a1 0164 0819 00a1 0101 007c  ...d...d.......|
+0000a360: 06a0 047c 0aa1 0101 007c 0574 0364 067c  ...|.....|.t.d.|
+0000a370: 0664 0919 0017 0083 0183 015c 027d 0c7d  .d.........\.}.}
+0000a380: 0d7c 07a0 047c 0ca1 0101 007c 08a0 047c  .|...|.....|...|
+0000a390: 0da1 0101 0071 2064 0a74 0664 0b64 0c84  .....q d.t.d.d..
+0000a3a0: 007c 0644 0083 0183 0114 007d 0e64 0a74  .|.D.......}.d.t
+0000a3b0: 0664 0d64 0c84 007c 0944 0083 0183 0114  .d.d...|.D......
+0000a3c0: 007d 0f64 0a74 0664 0e64 0c84 007c 0744  .}.d.t.d.d...|.D
+0000a3d0: 0083 0183 0114 007d 107c 0164 006b 0890  .......}.|.d.k..
+0000a3e0: 0172 5874 07a0 0874 097c 0683 01a1 017d  .rXt...t.|.....}
+0000a3f0: 116e ac64 0f7c 01a0 0aa1 006b 0690 0172  .n.d.|.....k...r
+0000a400: 7274 07a0 0b7c 09a1 017d 116e 9264 107c  rt...|...}.n.d.|
+0000a410: 01a0 0aa1 006b 0690 0173 8e64 117c 01a0  .....k...s.d.|..
+0000a420: 0aa1 006b 0690 0172 dc74 076a 0c6a 0d64  ...k...r.t.j.j.d
+0000a430: 1274 076a 0e64 138d 0201 0074 07a0 0f64  .t.j.d.....t...d
+0000a440: 1464 1584 007c 0744 0083 01a1 017d 0b74  .d...|.D.....}.t
+0000a450: 076a 107c 0b7c 0b64 006b 023c 0064 1664  .j.|.|.d.k.<.d.d
+0000a460: 1584 007c 0b44 0083 017d 0b74 07a0 0b7c  ...|.D...}.t...|
+0000a470: 0ba1 017d 116e 2864 177c 01a0 0aa1 006b  ...}.n(d.|.....k
+0000a480: 0690 0172 f674 07a0 0b7c 06a1 017d 116e  ...r.t...|...}.n
+0000a490: 0e74 07a0 0874 097c 0683 01a1 017d 117c  .t...t.|.....}.|
+0000a4a0: 1144 005d d27d 127c 067c 1219 007d 137c  .D.].}.|.|...}.|
+0000a4b0: 097c 1219 007d 147c 077c 1219 007d 1574  .|...}.|.|...}.t
+0000a4c0: 0364 067c 067c 1219 0017 0083 017d 1674  .d.|.|.......}.t
+0000a4d0: 017c 1683 017d 177c 137c 0e17 0064 0074  .|...}.|.|...d.t
+0000a4e0: 097c 0e83 0185 0219 007d 137c 147c 0f17  .|.......}.|.|..
+0000a4f0: 0064 0074 097c 0f83 0185 0219 007d 147c  .d.t.|.......}.|
+0000a500: 157c 1017 0064 0074 097c 1083 0185 0219  .|...d.t.|......
+0000a510: 007d 1574 097c 1783 017c 046b 0490 0272  .}.t.|...|.k...r
+0000a520: 9a64 187c 177c 040b 0064 0085 0219 0017  .d.|.|...d......
+0000a530: 007d 176e 1264 197c 177c 040b 0064 0085  .}.n.d.|.|...d..
+0000a540: 0219 0017 007d 1774 117c 1364 1a17 007c  .....}.t.|.d...|
+0000a550: 1417 0064 1b17 007c 087c 1219 0017 0064  ...d...|.|.....d
+0000a560: 1c17 007c 1517 0064 1b17 007c 1717 0083  ...|...d...|....
+0000a570: 0101 0090 0271 087c 0390 0272 ea7c 067c  .....q.|...r.|.|
+0000a580: 0966 0253 0064 0053 0029 1d4e 6301 0000  .f.S.d.S.).Nc...
+0000a590: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+0000a5a0: 0053 0000 0073 5c00 0000 6400 7d01 7a32  .S...s\...d.}.z2
+0000a5b0: 7400 7401 7c00 8301 8301 7d02 6401 7d01  t.t.|.....}.d.}.
+0000a5c0: 7402 7c00 8301 6a03 7404 6a05 6b02 7234  t.|...j.t.j.k.r4
+0000a5d0: 7400 7c00 6a06 8301 7d02 6402 7d01 5700  t.|.j...}.d.}.W.
+0000a5e0: 6e1c 0100 0100 0100 7c01 6400 6b08 724e  n.......|.d.k.rN
+0000a5f0: 6403 7d02 6404 7d01 5900 6e02 5800 7c02  d.}.d.}.Y.n.X.|.
+0000a600: 7c01 6602 5300 a905 4eda 066c 656e 6774  |.f.S...N..lengt
+0000a610: 687a 0673 6861 7065 20da 044e 6f6e 657a  hz.shape ..Nonez
+0000a620: 064e 6f6e 6520 20a9 0772 ad00 0000 7230  .None  ..r....r0
+0000a630: 0000 0072 1c01 0000 7276 0100 0072 1d00  ...r....rv...r..
+0000a640: 0000 7277 0100 0072 2100 0000 a903 5a04  ..rw...r!.....Z.
+0000a650: 785f 696e 5a09 7768 6963 685f 6f6e 655a  x_inZ.which_oneZ
+0000a660: 106c 656e 5f6f 725f 7368 6170 655f 6f75  .len_or_shape_ou
+0000a670: 7472 1600 0000 7216 0000 0072 1700 0000  tr....r....r....
+0000a680: da10 6765 745f 6c65 6e5f 6f72 5f73 6861  ..get_len_or_sha
+0000a690: 7065 1207 0000 7318 0000 0000 0104 0102  pe....s.........
+0000a6a0: 010c 0104 0110 010a 0108 0106 0108 0104  ................
+0000a6b0: 010a 017a 2967 6574 5f63 6c61 7373 5f69  ...z)get_class_i
+0000a6c0: 6e66 6f32 2e3c 6c6f 6361 6c73 3e2e 6765  nfo2.<locals>.ge
+0000a6d0: 745f 6c65 6e5f 6f72 5f73 6861 7065 4672  t_len_or_shapeFr
+0000a6e0: 0100 0000 da01 5ffa 0263 2efa 0127 e9fe  ......_..c...'..
+0000a6f0: ffff ff72 4a00 0000 728b 0100 0063 0100  ...rJ...r....c..
+0000a700: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+0000a710: 0000 7300 0000 7316 0000 007c 005d 0e7d  ..s...s....|.].}
+0000a720: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
+0000a730: 0072 0d01 0000 7248 0000 0072 3100 0000  .r....rH...r1...
+0000a740: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+0000a750: d800 0000 3507 0000 7304 0000 0004 0002  ....5...s.......
+0000a760: 007a 2267 6574 5f63 6c61 7373 5f69 6e66  .z"get_class_inf
+0000a770: 6f32 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  o2.<locals>.<gen
+0000a780: 6578 7072 3e63 0100 0000 0000 0000 0000  expr>c..........
+0000a790: 0000 0200 0000 0300 0000 7300 0000 7316  ..........s...s.
+0000a7a0: 0000 007c 005d 0e7d 0174 007c 0183 0156  ...|.].}.t.|...V
+0000a7b0: 0001 0071 0264 0053 0072 0d01 0000 7248  ...q.d.S.r....rH
+0000a7c0: 0000 0072 3100 0000 7216 0000 0072 1600  ...r1...r....r..
+0000a7d0: 0000 7217 0000 0072 d800 0000 3607 0000  ..r....r....6...
+0000a7e0: 7304 0000 0004 0002 0063 0100 0000 0000  s........c......
+0000a7f0: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
+0000a800: 0000 7316 0000 007c 005d 0e7d 0174 007c  ..s....|.].}.t.|
+0000a810: 0183 0156 0001 0071 0264 0053 0072 0d01  ...V...q.d.S.r..
+0000a820: 0000 7248 0000 0072 3100 0000 7216 0000  ..rH...r1...r...
+0000a830: 0072 1600 0000 7217 0000 0072 d800 0000  .r....r....r....
+0000a840: 3707 0000 7304 0000 0004 0002 0072 1c01  7...s........r..
+0000a850: 0000 7230 0000 0072 2100 0000 7218 0100  ..r0...r!...r...
+0000a860: 0029 01da 0863 6174 6567 6f72 7963 0100  .)...categoryc..
+0000a870: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+0000a880: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+0000a890: 0c7d 0174 007c 0183 0191 0271 0453 0072  .}.t.|.....q.S.r
+0000a8a0: 1600 0000 2901 da04 6576 616c 7231 0000  ....)...evalr1..
+0000a8b0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+0000a8c0: 7234 0000 003e 0700 0073 0400 0000 0600  r4...>...s......
+0000a8d0: 0200 7a23 6765 745f 636c 6173 735f 696e  ..z#get_class_in
+0000a8e0: 666f 322e 3c6c 6f63 616c 733e 2e3c 6c69  fo2.<locals>.<li
+0000a8f0: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+0000a900: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+0000a910: 7316 0000 0067 007c 005d 0e7d 0174 00a0  s....g.|.].}.t..
+0000a920: 017c 01a1 0191 0271 0453 0072 1600 0000  .|.....q.S.r....
+0000a930: 2902 721d 0000 0072 1301 0000 2902 7232  ).r....r....).r2
+0000a940: 0000 005a 0369 6969 7216 0000 0072 1600  ...Z.iiir....r..
+0000a950: 0000 7217 0000 0072 3400 0000 4007 0000  ..r....r4...@...
+0000a960: 7304 0000 0006 0002 0072 b601 0000 fa03  s........r......
+0000a970: 2e2e 2efa 023e 20fa 0a20 7479 7065 2d3e  .....> .. type->
+0000a980: 2020 20fa 0220 20fa 052d 3e20 2020 2912     ..  ..->   ).
+0000a990: da03 6469 7272 ad00 0000 721c 0100 0072  ..dirr....r....r
+0000a9a0: eb01 0000 7223 0000 0072 db00 0000 7213  ....r#...r....r.
+0000a9b0: 0100 0072 1d00 0000 72b4 0000 0072 3000  ...r....r....r0.
+0000a9c0: 0000 721d 0100 0072 8a00 0000 728f 0000  ..r....r....r...
+0000a9d0: 00da 0e66 696c 7465 7277 6172 6e69 6e67  ...filterwarning
+0000a9e0: 73da 1956 6973 6962 6c65 4465 7072 6563  s..VisibleDeprec
+0000a9f0: 6174 696f 6e57 6172 6e69 6e67 7238 0000  ationWarningr8..
+0000aa00: 0072 2200 0000 724b 0000 0029 1872 e600  .r"...rK...).r..
+0000aa10: 0000 5a07 736f 7274 5f62 79da 1769 6e63  ..Z.sort_by..inc
+0000aa20: 6c75 6465 5f75 6e64 6572 7363 6f72 655f  lude_underscore_
+0000aa30: 7661 7273 da14 7265 7475 726e 5f6e 616d  vars..return_nam
+0000aa40: 655f 616e 645f 7479 7065 da0c 656e 645f  e_and_type..end_
+0000aa50: 7072 6576 5f6c 656e 72e5 0100 00da 056e  prev_lenr......n
+0000aa60: 616d 6573 da0c 6c65 6e5f 6f72 5f73 6861  ames..len_or_sha
+0000aa70: 7065 da16 6c65 6e5f 6f72 5f73 6861 7065  pe..len_or_shape
+0000aa80: 5f77 6869 6368 5f6f 6e65 da0d 7479 7065  _which_one..type
+0000aa90: 5f74 6f5f 7072 696e 7472 3300 0000 72fb  _to_printr3...r.
+0000aaa0: 0000 0072 e500 0000 7242 0000 0072 9201  ...r....rB...r..
+0000aab0: 0000 da0e 6c65 6e5f 7370 6163 655f 7479  ....len_space_ty
+0000aac0: 7065 da0f 6c65 6e5f 7370 6163 655f 7368  pe..len_space_sh
+0000aad0: 6170 65da 0969 6e64 5f61 7272 6179 722c  ape..ind_arrayr,
+0000aae0: 0000 0072 bd00 0000 72be 0000 00da 026b  ...r....r......k
+0000aaf0: 3572 5300 0000 7290 0100 0072 1600 0000  5rS...r....r....
+0000ab00: 7216 0000 0072 1700 0000 7278 0100 0011  r....r....rx....
+0000ab10: 0700 0073 6600 0000 0001 080e 0401 0401  ...sf...........
+0000ab20: 0401 0402 0c01 1402 1401 1401 0a01 1801  ................
+0000ab30: 0a01 0c01 0401 1401 1401 0a01 1801 0a01  ................
+0000ab40: 0c01 1601 1601 1601 0a01 1001 0e01 0c01  ................
+0000ab50: 1c01 1201 1401 0e01 0e01 0c01 0e01 0c02  ................
+0000ab60: 0e02 0801 0801 0801 0801 1001 0801 1401  ................
+0000ab70: 1401 1401 0e01 1402 1201 3001 0601 7278  ..........0...rx
+0000ab80: 0100 0063 0500 0000 0000 0000 0000 0000  ...c............
+0000ab90: 1800 0000 0600 0000 4300 0000 7344 0200  ........C...sD..
+0000aba0: 0064 0164 0284 007d 0567 007d 0667 007d  .d.d...}.g.}.g.}
+0000abb0: 0767 007d 0867 007d 0974 007c 0083 0144  .g.}.g.}.t.|...D
+0000abc0: 005d da7d 0a7c 0264 036b 0872 987c 0a64  .].}.|.d.k.r.|.d
+0000abd0: 0419 0064 056b 0372 9874 0174 0274 0364  ...d.k.r.t.t.t.d
+0000abe0: 067c 0a17 0083 0183 0183 017d 0b7c 09a0  .|.........}.|..
+0000abf0: 047c 0ba0 0564 07a1 0164 0819 00a1 0101  .|...d...d......
+0000ac00: 007c 06a0 047c 0aa1 0101 007c 0574 0364  .|...|.....|.t.d
+0000ac10: 067c 0664 0919 0017 0083 0183 015c 027d  .|.d.........\.}
+0000ac20: 0c7d 0d7c 07a0 047c 0ca1 0101 007c 08a0  .}.|...|.....|..
+0000ac30: 047c 0da1 0101 0071 207c 0272 2074 0174  .|.....q |.r t.t
+0000ac40: 0274 0364 067c 0a17 0083 0183 0183 017d  .t.d.|.........}
+0000ac50: 0b7c 09a0 047c 0ba0 0564 07a1 0164 0819  .|...|...d...d..
+0000ac60: 00a1 0101 007c 06a0 047c 0aa1 0101 007c  .....|...|.....|
+0000ac70: 0574 0364 067c 0664 0919 0017 0083 0183  .t.d.|.d........
+0000ac80: 015c 027d 0c7d 0d7c 07a0 047c 0ca1 0101  .\.}.}.|...|....
+0000ac90: 007c 08a0 047c 0da1 0101 0071 2064 0a74  .|...|.....q d.t
+0000aca0: 0664 0b64 0c84 007c 0644 0083 0183 0114  .d.d...|.D......
+0000acb0: 007d 0e64 0a74 0664 0d64 0c84 007c 0944  .}.d.t.d.d...|.D
+0000acc0: 0083 0183 0114 007d 0f64 0a74 0664 0e64  .......}.d.t.d.d
+0000acd0: 0c84 007c 0744 0083 0183 0114 007d 107c  ...|.D.......}.|
+0000ace0: 0190 0172 5074 07a0 087c 09a1 017d 116e  ...rPt...|...}.n
+0000acf0: 0a74 07a0 087c 06a1 017d 117c 1144 005d  .t...|...}.|.D.]
+0000ad00: d27d 127c 067c 1219 007d 137c 097c 1219  .}.|.|...}.|.|..
+0000ad10: 007d 147c 077c 1219 007d 1574 0364 067c  .}.|.|...}.t.d.|
+0000ad20: 067c 1219 0017 0083 017d 1674 017c 1683  .|.......}.t.|..
+0000ad30: 017d 177c 137c 0e17 0064 0074 097c 0e83  .}.|.|...d.t.|..
+0000ad40: 0185 0219 007d 137c 147c 0f17 0064 0074  .....}.|.|...d.t
+0000ad50: 097c 0f83 0185 0219 007d 147c 157c 1017  .|.......}.|.|..
+0000ad60: 0064 0074 097c 1083 0185 0219 007d 1574  .d.t.|.......}.t
+0000ad70: 097c 1783 017c 046b 0490 0172 f064 0f7c  .|...|.k...r.d.|
+0000ad80: 177c 040b 0064 0085 0219 0017 007d 176e  .|...d.......}.n
+0000ad90: 1264 107c 177c 040b 0064 0085 0219 0017  .d.|.|...d......
+0000ada0: 007d 1774 0a7c 1364 1117 007c 1417 0064  .}.t.|.d...|...d
+0000adb0: 1217 007c 087c 1219 0017 0064 1317 007c  ...|.|.....d...|
+0000adc0: 1517 0064 1217 007c 1717 0083 0101 0090  ...d...|........
+0000add0: 0171 5e7c 0390 0272 407c 067c 0966 0253  .q^|...r@|.|.f.S
+0000ade0: 0064 0053 0029 144e 6301 0000 0000 0000  .d.S.).Nc.......
+0000adf0: 0000 0000 0003 0000 0006 0000 0053 0000  .............S..
+0000ae00: 0073 5c00 0000 6400 7d01 7a32 7400 7401  .s\...d.}.z2t.t.
+0000ae10: 7c00 8301 8301 7d02 6401 7d01 7402 7c00  |.....}.d.}.t.|.
+0000ae20: 8301 6a03 7404 6a05 6b02 7234 7400 7c00  ..j.t.j.k.r4t.|.
+0000ae30: 6a06 8301 7d02 6402 7d01 5700 6e1c 0100  j...}.d.}.W.n...
+0000ae40: 0100 0100 7c01 6400 6b08 724e 6403 7d02  ....|.d.k.rNd.}.
+0000ae50: 6404 7d01 5900 6e02 5800 7c02 7c01 6602  d.}.Y.n.X.|.|.f.
+0000ae60: 5300 72e0 0100 0072 e301 0000 72e4 0100  S.r....r....r...
+0000ae70: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+0000ae80: 72e5 0100 005a 0700 0073 1800 0000 0001  r....Z...s......
+0000ae90: 0401 0201 0c01 0401 1001 0a01 0801 0601  ................
+0000aea0: 0801 0401 0a01 7a28 6765 745f 636c 6173  ......z(get_clas
+0000aeb0: 735f 696e 666f 2e3c 6c6f 6361 6c73 3e2e  s_info.<locals>.
+0000aec0: 6765 745f 6c65 6e5f 6f72 5f73 6861 7065  get_len_or_shape
+0000aed0: 4672 0100 0000 72e6 0100 0072 e701 0000  Fr....r....r....
+0000aee0: 72e8 0100 0072 e901 0000 724a 0000 0072  r....r....rJ...r
+0000aef0: 8b01 0000 6301 0000 0000 0000 0000 0000  ....c...........
+0000af00: 0002 0000 0003 0000 0073 0000 0073 1600  .........s...s..
+0000af10: 0000 7c00 5d0e 7d01 7400 7c01 8301 5600  ..|.].}.t.|...V.
+0000af20: 0100 7102 6400 5300 720d 0100 0072 4800  ..q.d.S.r....rH.
+0000af30: 0000 7231 0000 0072 1600 0000 7216 0000  ..r1...r....r...
+0000af40: 0072 1700 0000 72d8 0000 007d 0700 0073  .r....r....}...s
+0000af50: 0400 0000 0400 0200 7a21 6765 745f 636c  ........z!get_cl
+0000af60: 6173 735f 696e 666f 2e3c 6c6f 6361 6c73  ass_info.<locals
+0000af70: 3e2e 3c67 656e 6578 7072 3e63 0100 0000  >.<genexpr>c....
+0000af80: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+0000af90: 7300 0000 7316 0000 007c 005d 0e7d 0174  s...s....|.].}.t
+0000afa0: 007c 0183 0156 0001 0071 0264 0053 0072  .|...V...q.d.S.r
+0000afb0: 0d01 0000 7248 0000 0072 3100 0000 7216  ....rH...r1...r.
+0000afc0: 0000 0072 1600 0000 7217 0000 0072 d800  ...r....r....r..
+0000afd0: 0000 7e07 0000 7304 0000 0004 0002 0063  ..~...s........c
+0000afe0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+0000aff0: 0300 0000 7300 0000 7316 0000 007c 005d  ....s...s....|.]
+0000b000: 0e7d 0174 007c 0183 0156 0001 0071 0264  .}.t.|...V...q.d
+0000b010: 0053 0072 0d01 0000 7248 0000 0072 3100  .S.r....rH...r1.
+0000b020: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+0000b030: 0072 d800 0000 7f07 0000 7304 0000 0004  .r........s.....
+0000b040: 0002 0072 ec01 0000 72ed 0100 0072 ee01  ...r....r....r..
+0000b050: 0000 72ef 0100 0072 f001 0000 290b 72f1  ..r....r....).r.
+0000b060: 0100 0072 ad00 0000 721c 0100 0072 eb01  ...r....r....r..
+0000b070: 0000 7223 0000 0072 db00 0000 7213 0100  ..r#...r....r...
+0000b080: 0072 1d00 0000 728a 0000 0072 3000 0000  .r....r....r0...
+0000b090: 724b 0000 0029 1872 e600 0000 da0c 736f  rK...).r......so
+0000b0a0: 7274 5f62 795f 7479 7065 72f4 0100 0072  rt_by_typer....r
+0000b0b0: f501 0000 72f6 0100 0072 e501 0000 72f7  ....r....r....r.
+0000b0c0: 0100 0072 f801 0000 72f9 0100 0072 fa01  ...r....r....r..
+0000b0d0: 0000 7233 0000 0072 fb00 0000 72e5 0000  ..r3...r....r...
+0000b0e0: 0072 4200 0000 7292 0100 0072 fb01 0000  .rB...r....r....
+0000b0f0: 72fc 0100 0072 fd01 0000 722c 0000 0072  r....r....r,...r
+0000b100: bd00 0000 72be 0000 0072 fe01 0000 7253  ....r....r....rS
+0000b110: 0000 0072 9001 0000 7216 0000 0072 1600  ...r....r....r..
+0000b120: 0000 7217 0000 00da 0e67 6574 5f63 6c61  ..r......get_cla
+0000b130: 7373 5f69 6e66 6f59 0700 0073 5200 0000  ss_infoY...sR...
+0000b140: 0001 080e 0401 0401 0401 0402 0c01 1402  ................
+0000b150: 1401 1401 0a01 1801 0a01 0c01 0401 1401  ................
+0000b160: 1401 0a01 1801 0a01 0c01 1601 1601 1601  ................
+0000b170: 0601 0c02 0a02 0801 0801 0801 0801 1001  ................
+0000b180: 0801 1401 1401 1401 0e01 1402 1201 3001  ..............0.
+0000b190: 0601 7200 0200 0063 0500 0000 0000 0000  ..r....c........
+0000b1a0: 0000 0000 1200 0000 0900 0000 4300 0000  ............C...
+0000b1b0: 7312 0200 0067 007d 0567 007d 067c 00a0  s....g.}.g.}.|..
+0000b1c0: 00a1 0044 005d 867d 077c 0264 016b 0872  ...D.].}.|.d.k.r
+0000b1d0: 6074 017c 0783 0164 0219 0064 036b 0372  `t.|...d...d.k.r
+0000b1e0: 6074 0174 027c 007c 0719 0083 0183 017d  `t.t.|.|.......}
+0000b1f0: 087c 06a0 037c 08a0 0464 04a1 0164 0519  .|...|...d...d..
+0000b200: 00a1 0101 007c 05a0 0374 017c 0783 01a1  .....|...t.|....
+0000b210: 0101 0071 107c 0272 1074 0174 027c 007c  ...q.|.r.t.t.|.|
+0000b220: 0719 0083 0183 017d 087c 06a0 037c 08a0  .......}.|...|..
+0000b230: 0464 04a1 0164 0519 00a1 0101 007c 05a0  .d...d.......|..
+0000b240: 0374 017c 0783 01a1 0101 0071 1064 0674  .t.|.......q.d.t
+0000b250: 0564 0764 0884 007c 0544 0083 0183 0114  .d.d...|.D......
+0000b260: 007d 0964 0674 0564 0964 0884 007c 0644  .}.d.t.d.d...|.D
+0000b270: 0083 0183 0114 007d 0a7c 0172 d474 06a0  .......}.|.r.t..
+0000b280: 077c 06a1 017d 0b6e 0a74 06a0 077c 05a1  .|...}.n.t...|..
+0000b290: 017d 0b7c 0b44 0090 015d 1a7d 0c7c 057c  .}.|.D...].}.|.|
+0000b2a0: 0c19 007d 0d7c 067c 0c19 007d 0e7a 1474  ...}.|.|...}.z.t
+0000b2b0: 017c 007c 057c 0c19 0019 0083 017d 0f57  .|.|.|.......}.W
+0000b2c0: 006e 2001 0001 0001 0074 017c 0074 087c  .n ......t.|.t.|
+0000b2d0: 057c 0c19 0083 0119 0083 017d 0f59 006e  .|.........}.Y.n
+0000b2e0: 0258 007c 0d7c 0917 0064 0074 097c 0983  .X.|.|...d.t.|..
+0000b2f0: 0185 0219 007d 0d7c 0e7c 0a17 0064 0074  .....}.|.|...d.t
+0000b300: 097c 0a83 0185 0219 007d 0e74 097c 0f83  .|.......}.t.|..
+0000b310: 017c 046b 0490 0172 7864 0a7c 0f7c 040b  .|.k...rxd.|.|..
+0000b320: 0064 0085 0219 0017 007d 0f6e 1264 0b7c  .d.......}.n.d.|
+0000b330: 0f7c 040b 0064 0085 0219 0017 007d 0f64  .|...d.......}.d
+0000b340: 0c7c 0e6b 0690 0172 ac74 017c 007c 057c  .|.k...r.t.|.|.|
+0000b350: 0c19 0019 006a 0a83 017d 1064 0d7d 116e  .....j...}.d.}.n
+0000b360: 327a 1c74 0174 097c 007c 057c 0c19 0019  2z.t.t.|.|.|....
+0000b370: 0083 0183 017d 1064 0e7d 1157 006e 1401  .....}.d.}.W.n..
+0000b380: 0001 0001 0064 0f7d 1164 107d 1059 006e  .....d.}.d.}.Y.n
+0000b390: 0258 0074 0b7c 0d64 1117 007c 0e17 007c  .X.t.|.d...|...|
+0000b3a0: 1117 007c 1017 0064 1217 007c 0f17 0083  ...|...d...|....
+0000b3b0: 0101 0071 e27c 0390 0272 0e7c 057c 0666  ...q.|...r.|.|.f
+0000b3c0: 0253 0064 0053 0029 134e 4672 0100 0000  .S.d.S.).NFr....
+0000b3d0: 72e6 0100 0072 e801 0000 72e9 0100 0072  r....r....r....r
+0000b3e0: 8b01 0000 6301 0000 0000 0000 0000 0000  ....c...........
+0000b3f0: 0002 0000 0003 0000 0073 0000 0073 1600  .........s...s..
+0000b400: 0000 7c00 5d0e 7d01 7400 7c01 8301 5600  ..|.].}.t.|...V.
+0000b410: 0100 7102 6400 5300 720d 0100 0072 4800  ..q.d.S.r....rH.
+0000b420: 0000 7231 0000 0072 1600 0000 7216 0000  ..r1...r....r...
+0000b430: 0072 1700 0000 72d8 0000 00a3 0700 0073  .r....r........s
+0000b440: 0400 0000 0400 0200 7a20 6765 745f 6469  ........z get_di
+0000b450: 6374 5f69 6e66 6f2e 3c6c 6f63 616c 733e  ct_info.<locals>
+0000b460: 2e3c 6765 6e65 7870 723e 6301 0000 0000  .<genexpr>c.....
+0000b470: 0000 0000 0000 0002 0000 0003 0000 0073  ...............s
+0000b480: 0000 0073 1600 0000 7c00 5d0e 7d01 7400  ...s....|.].}.t.
+0000b490: 7c01 8301 5600 0100 7102 6400 5300 720d  |...V...q.d.S.r.
+0000b4a0: 0100 0072 4800 0000 7231 0000 0072 1600  ...rH...r1...r..
+0000b4b0: 0000 7216 0000 0072 1700 0000 72d8 0000  ..r....r....r...
+0000b4c0: 00a4 0700 0073 0400 0000 0400 0200 72ec  .....s........r.
+0000b4d0: 0100 0072 ed01 0000 7a0d 6e75 6d70 792e  ...r....z.numpy.
+0000b4e0: 6e64 6172 7261 797a 0b20 2020 7368 6170  ndarrayz.   shap
+0000b4f0: 652d 3e20 7a09 2020 206c 656e 2d3e 207a  e-> z.   len-> z
+0000b500: 0920 2020 4e6f 6e65 2d3e 72e2 0100 0072  .   None->r....r
+0000b510: ee01 0000 72ef 0100 0029 0c72 9900 0000  ....r....).r....
+0000b520: 72ad 0000 0072 1c01 0000 7223 0000 0072  r....r....r#...r
+0000b530: db00 0000 7213 0100 0072 1d00 0000 728a  ....r....r....r.
+0000b540: 0000 0072 8900 0000 7230 0000 0072 2100  ...r....r0...r!.
+0000b550: 0000 724b 0000 0029 1272 e600 0000 72ff  ..rK...).r....r.
+0000b560: 0100 0072 f401 0000 72f5 0100 0072 f601  ...r....r....r..
+0000b570: 0000 72f7 0100 0072 fa01 0000 7233 0000  ..r....r....r3..
+0000b580: 0072 fb00 0000 7292 0100 0072 fb01 0000  .r....r....r....
+0000b590: 72fd 0100 0072 2c00 0000 72bd 0000 0072  r....r,...r....r
+0000b5a0: be00 0000 7290 0100 005a 026b 345a 066b  ....r....Z.k4Z.k
+0000b5b0: 345f 7374 7272 1600 0000 7216 0000 0072  4_strr....r....r
+0000b5c0: 1700 0000 7274 0100 0097 0700 0073 5000  ....rt.......sP.
+0000b5d0: 0000 0001 0401 0401 0c01 1801 1001 1401  ................
+0000b5e0: 1001 0401 1001 1401 1001 1601 1601 0401  ................
+0000b5f0: 0c02 0a02 0a01 0801 0801 0201 1401 0601  ................
+0000b600: 1a01 1401 1402 0e01 1402 1202 0a01 1201  ................
+0000b610: 0602 0201 1401 0801 0601 0401 0a02 2201  ..............".
+0000b620: 0601 7274 0100 0063 0200 0000 0000 0000  ..rt...c........
+0000b630: 0000 0000 0900 0000 0400 0000 4300 0000  ............C...
+0000b640: 73b6 0000 0067 007d 0267 007d 037c 027d  s....g.}.g.}.|.}
+0000b650: 047c 037d 0564 017d 0674 007c 0083 0144  .|.}.d.}.t.|...D
+0000b660: 005d 625c 027d 077d 087c 087c 066b 0272  .]b\.}.}.|.|.k.r
+0000b670: 4c74 01a0 027c 08a1 0173 767c 02a0 037c  Lt...|...sv|...|
+0000b680: 08a1 0101 007c 03a0 037c 07a1 0101 006e  .....|...|.....n
+0000b690: 2a74 01a0 027c 08a1 0173 767c 0867 017d  *t...|...sv|.g.}
+0000b6a0: 027c 0767 017d 037c 04a0 037c 02a1 0101  .|.g.}.|...|....
+0000b6b0: 007c 05a0 037c 03a1 0101 007c 087c 0117  .|...|.....|.|..
+0000b6c0: 007d 0671 1c7c 0467 006b 0272 8a6e 247c  .}.q.|.g.k.r.n$|
+0000b6d0: 0464 0219 0067 006b 0272 ae7c 0464 0364  .d...g.k.r.|.d.d
+0000b6e0: 0185 0219 007d 047c 0564 0364 0185 0219  .....}.|.d.d....
+0000b6f0: 007d 057c 047c 0566 0253 0029 047a 7a0a  .}.|.|.f.S.).zz.
+0000b700: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0000b710: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000b720: 2020 2076 616c 7320 3a0a 2020 2020 2020     vals :.      
+0000b730: 2020 0a20 2020 2073 7465 7020 3a0a 2020    .    step :.  
+0000b740: 2020 2020 2020 2028 4465 6661 756c 7420         (Default 
+0000b750: 7661 6c75 6520 3d20 3129 0a0a 2020 2020  value = 1)..    
+0000b760: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0000b770: 2d2d 2d0a 0a20 2020 204e 7201 0000 0072  ---..    Nr....r
+0000b780: 2e00 0000 2904 7224 0000 0072 1d00 0000  ....).r$...r....
+0000b790: 72de 0000 0072 2300 0000 2909 da04 7661  r....r#...)...va
+0000b7a0: 6c73 72f0 0000 00da 0372 756e 5a07 7275  lsr......runZ.ru
+0000b7b0: 6e5f 696e 64da 0672 6573 756c 745a 0a72  n_ind..resultZ.r
+0000b7c0: 6573 756c 745f 696e 645a 0665 7870 6563  esult_indZ.expec
+0000b7d0: 7472 3300 0000 da01 7672 1600 0000 7216  tr3.....vr....r.
+0000b7e0: 0000 0072 1700 0000 723b 0000 00f2 0700  ...r....r;......
+0000b7f0: 0073 2c00 0000 000e 0401 0401 0401 0401  .s,.............
+0000b800: 0401 1001 0801 0a03 0a01 0c02 0a01 0601  ................
+0000b810: 0601 0a01 0a01 0a02 0801 0201 0c01 0c01  ................
+0000b820: 0c01 723b 0000 0063 0200 0000 0000 0000  ..r;...c........
+0000b830: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+0000b840: 7356 0000 0067 007d 0274 007c 0074 016a  sV...g.}.t.|.t.j
+0000b850: 026a 0317 0083 01a0 0464 01a1 0144 005d  .j.......d...D.]
+0000b860: 227d 037c 02a0 0574 067c 036a 0783 0174  "}.|...t.|.j...t
+0000b870: 016a 026a 0317 007c 036a 0817 00a1 0101  .j.j...|.j......
+0000b880: 0071 1a7c 02a0 09a1 0001 007c 0172 5274  .q.|.......|.rRt
+0000b890: 0a7c 0283 0101 007c 0253 0029 027a 560a  .|.....|.S.).zV.
+0000b8a0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0000b8b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000b8c0: 2020 2062 6173 655f 6469 7220 3a0a 2020     base_dir :.  
+0000b8d0: 2020 2020 2020 0a0a 2020 2020 5265 7475        ..    Retu
+0000b8e0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0000b8f0: 0a20 2020 207a 042a 2e68 3529 0b72 0e00  .    z.*.h5).r..
+0000b900: 0000 725f 0000 0072 6100 0000 7260 0000  ..r_...ra...r`..
+0000b910: 00da 0572 676c 6f62 7223 0000 0072 ad00  ...rglobr#...r..
+0000b920: 0000 da06 7061 7265 6e74 72b6 0100 0072  ....parentr....r
+0000b930: 6501 0000 72cb 0100 0029 0472 ba00 0000  e...r....).r....
+0000b940: 5a0d 7072 696e 745f 6835 5f6c 6973 745a  Z.print_h5_listZ
+0000b950: 0c48 355f 6669 6c65 5f6c 6973 7472 6100  .H5_file_listra.
+0000b960: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+0000b970: 0072 2901 0000 1c08 0000 730e 0000 0000  .r).......s.....
+0000b980: 0c04 011a 0120 0108 0104 0108 0172 2901  ..... .......r).
+0000b990: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+0000b9a0: 0000 0007 0000 0043 0000 0073 6000 0000  .......C...s`...
+0000b9b0: 7400 7c00 7c01 8302 4400 5d48 5c02 7d02  t.|.|...D.]H\.}.
+0000b9c0: 7d03 7a1e 7c03 a001 7402 6a03 6a04 a101  }.z.|...t.j.j...
+0000b9d0: 6401 1900 7c02 6b06 732e 7405 8201 5700  d...|.k.s.t...W.
+0000b9e0: 710a 0100 0100 0100 7406 6402 8301 0100  q.......t.d.....
+0000b9f0: 6403 6404 6b02 734c 7405 8201 5900 710a  d.d.k.sLt...Y.q.
+0000ba00: 5800 710a 7406 6405 8301 0100 6406 5300  X.q.t.d.....d.S.
+0000ba10: 2907 7a74 0a0a 2020 2020 5061 7261 6d65  ).zt..    Parame
+0000ba20: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000ba30: 2d2d 2d0a 2020 2020 4835 5f6c 6973 745f  ---.    H5_list_
+0000ba40: 4c41 4220 3a0a 2020 2020 2020 2020 0a20  LAB :.        . 
+0000ba50: 2020 2048 355f 6c69 7374 5f49 4d47 203a     H5_list_IMG :
+0000ba60: 0a20 2020 2020 2020 200a 0a20 2020 2052  .        ..    R
+0000ba70: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0000ba80: 2d2d 0a0a 2020 2020 724a 0000 007a 4344  --..    rJ...zCD
+0000ba90: 4f20 4e4f 5420 434f 4e54 494e 5545 202d  O NOT CONTINUE -
+0000baa0: 2d2d 2073 6f6d 6520 6669 6c65 7320 646f  -- some files do
+0000bab0: 206e 6f74 206d 6174 6368 206f 6e20 796f   not match on yo
+0000bac0: 7572 206c 6973 7473 2074 7279 2061 6761  ur lists try aga
+0000bad0: 696e 722e 0000 0072 0100 0000 7a13 7961  inr....r....z.ya
+0000bae0: 7920 7468 6579 2061 6c6c 206d 6174 6368  y they all match
+0000baf0: 214e 2907 72b0 0000 0072 db00 0000 725f  !N).r....r....r_
+0000bb00: 0000 0072 6100 0000 7260 0000 0072 4e00  ...ra...r`...rN.
+0000bb10: 0000 724b 0000 0029 045a 0b48 355f 6c69  ..rK...).Z.H5_li
+0000bb20: 7374 5f4c 4142 5a0b 4835 5f6c 6973 745f  st_LABZ.H5_list_
+0000bb30: 494d 475a 0668 355f 4c41 425a 0668 355f  IMGZ.h5_LABZ.h5_
+0000bb40: 494d 4772 1600 0000 7216 0000 0072 1700  IMGr....r....r..
+0000bb50: 0000 da19 6368 6563 6b5f 6966 5f66 696c  ....check_if_fil
+0000bb60: 655f 6c69 7374 735f 6d61 7463 6831 0800  e_lists_match1..
+0000bb70: 0073 0e00 0000 000e 1201 0201 1e01 0601  .s..............
+0000bb80: 0801 1401 7207 0200 0063 0100 0000 0000  ....r....c......
+0000bb90: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+0000bba0: 0000 7316 0000 0064 0164 0284 0074 007c  ..s....d.d...t.|
+0000bbb0: 0083 0144 0083 017d 0164 0353 0029 047a  ...D...}.d.S.).z
+0000bbc0: 550a 0a20 2020 2050 6172 616d 6574 6572  U..    Parameter
+0000bbd0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0000bbe0: 0a20 2020 206c 6973 745f 696e 203a 0a20  .    list_in :. 
+0000bbf0: 2020 2020 2020 200a 0a20 2020 2052 6574         ..    Ret
+0000bc00: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+0000bc10: 0a0a 2020 2020 6301 0000 0000 0000 0000  ..    c.........
+0000bc20: 0000 0003 0000 0007 0000 0053 0000 0073  ...........S...s
+0000bc30: 3200 0000 6700 7c00 5d2a 5c02 7d01 7d02  2...g.|.]*\.}.}.
+0000bc40: 7400 7401 7c01 8301 6400 1700 7c02 a002  t.t.|...d...|...
+0000bc50: 7403 6a04 6a05 a101 6401 1900 1700 8301  t.j.j...d.......
+0000bc60: 9102 7104 5300 a902 728b 0100 0072 4a00  ..q.S...r....rJ.
+0000bc70: 0000 a906 724b 0000 0072 ad00 0000 72db  ....rK...r....r.
+0000bc80: 0000 0072 5f00 0000 7261 0000 0072 6000  ...r_...ra...r`.
+0000bc90: 0000 a903 7232 0000 0072 2c00 0000 7233  ....r2...r,...r3
+0000bca0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+0000bcb0: 0000 7234 0000 0054 0800 0073 0400 0000  ..r4...T...s....
+0000bcc0: 0600 0600 7a28 7072 696e 745f 6c69 7374  ....z(print_list
+0000bcd0: 5f77 6974 685f 696e 6473 2e3c 6c6f 6361  _with_inds.<loca
+0000bce0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 4ea9  ls>.<listcomp>N.
+0000bcf0: 0172 2400 0000 2902 721e 0100 0072 e601  .r$...).r....r..
+0000bd00: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+0000bd10: 0072 cb01 0000 4808 0000 7302 0000 0000  .r....H...s.....
+0000bd20: 0c72 cb01 0000 6301 0000 0000 0000 0000  .r....c.........
+0000bd30: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+0000bd40: 2200 0000 7400 6401 8301 0100 7401 a001  "...t.d.....t...
+0000bd50: 7c00 6402 1700 a101 7d01 7402 7c01 8301  |.d.....}.t.|...
+0000bd60: 0100 7c01 5300 2903 fa5c 0a0a 2020 2020  ..|.S.)..\..    
+0000bd70: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000bd80: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6d6f  ---------.    mo
+0000bd90: 6465 6c5f 7361 7665 5f64 6972 203a 0a20  del_save_dir :. 
+0000bda0: 2020 2020 2020 200a 0a20 2020 2052 6574         ..    Ret
+0000bdb0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+0000bdc0: 0a0a 2020 2020 fa2a 5468 6573 6520 6172  ..    .*These ar
+0000bdd0: 6520 616c 6c20 7468 6520 6d6f 6465 6c73  e all the models
+0000bde0: 2074 6f20 6368 6f6f 7365 2066 726f 6d2e   to choose from.
+0000bdf0: 2e2e fa07 2f2a 2e63 6b70 7429 0372 4b00  ..../*.ckpt).rK.
+0000be00: 0000 72b3 0100 0072 cb01 0000 2902 da0e  ..r....r....)...
+0000be10: 6d6f 6465 6c5f 7361 7665 5f64 6972 da10  model_save_dir..
+0000be20: 6d6f 6465 6c5f 325f 6c6f 6164 5f61 6c6c  model_2_load_all
+0000be30: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+0000be40: 0e67 6574 5f6d 6f64 656c 5f6c 6973 7457  .get_model_listW
+0000be50: 0800 0073 0800 0000 000c 0801 0e01 0801  ...s............
+0000be60: 7211 0200 0063 0200 0000 0000 0000 0000  r....c..........
+0000be70: 0000 0600 0000 0600 0000 4300 0000 735c  ..........C...s\
+0000be80: 0000 0067 007d 0274 00a0 017c 00a1 0144  ...g.}.t...|...D
+0000be90: 005d 265c 037d 037d 047d 0574 02a0 027c  .]&\.}.}.}.t...|
+0000bea0: 0364 0117 007c 0117 00a1 0172 0e7c 02a0  .d...|.....r.|..
+0000beb0: 037c 03a1 0101 0071 0e7a 0c74 047c 0283  .|.....q.z.t.|..
+0000bec0: 017d 0257 006e 1401 0001 0001 0074 057c  .}.W.n.......t.|
+0000bed0: 0283 017d 0259 006e 0258 007c 0253 0029  ...}.Y.n.X.|.S.)
+0000bee0: 0261 5701 0000 656e 7465 7220 6261 7365  .aW...enter base
+0000bef0: 2064 6972 6563 746f 7279 2061 6e64 2073   directory and s
+0000bf00: 6561 7263 6820 7465 726d 2074 6f20 6669  earch term to fi
+0000bf10: 6e64 2061 6c6c 2074 6865 2064 6972 6563  nd all the direc
+0000bf20: 746f 7269 6573 2069 6e20 6261 7365 2064  tories in base d
+0000bf30: 6972 6563 746f 7279 0a20 2020 2020 2077  irectory.      w
+0000bf40: 6974 6820 6669 6c65 7320 6d61 7463 6869  ith files matchi
+0000bf50: 6e67 2074 6865 2073 6561 7263 685f 7465  ng the search_te
+0000bf60: 726d 2e20 6f75 7470 7574 2061 2073 6f72  rm. output a sor
+0000bf70: 7465 6420 6c69 7374 206f 6620 6469 7265  ted list of dire
+0000bf80: 6374 6f72 6965 732e 0a20 2020 2020 2065  ctories..      e
+0000bf90: 2e67 2e20 2d3e 2072 6563 7572 7369 7665  .g. -> recursive
+0000bfa0: 5f64 6972 5f66 696e 6465 7228 272f 636f  _dir_finder('/co
+0000bfb0: 6e74 656e 742f 6d79 6472 6f70 626f 782f  ntent/mydropbox/
+0000bfc0: 272c 2027 2a2e 6d70 3427 290a 0a20 2020  ', '*.mp4')..   
+0000bfd0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000bfe0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2062  ----------.    b
+0000bff0: 6173 655f 7061 7468 203a 0a20 2020 2020  ase_path :.     
+0000c000: 2020 200a 2020 2020 7365 6172 6368 5f74     .    search_t
+0000c010: 6572 6d20 3a0a 2020 2020 2020 2020 0a0a  erm :.        ..
+0000c020: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0000c030: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2072 5501  -------..    rU.
+0000c040: 0000 2906 725f 0000 00da 0477 616c 6b72  ..).r_.....walkr
+0000c050: b301 0000 7223 0000 0072 0600 0000 72d3  ....r#...r....r.
+0000c060: 0000 0029 06da 0962 6173 655f 7061 7468  ...)...base_path
+0000c070: da0b 7365 6172 6368 5f74 6572 6d5a 106d  ..search_termZ.m
+0000c080: 6174 6368 696e 675f 666f 6c64 6572 73da  atching_folders.
+0000c090: 0472 6f6f 74da 0464 6972 73da 0566 696c  .root..dirs..fil
+0000c0a0: 6573 7216 0000 0072 1600 0000 7217 0000  esr....r....r...
+0000c0b0: 00da 1472 6563 7572 7369 7665 5f64 6972  ...recursive_dir
+0000c0c0: 5f66 696e 6465 7269 0800 0073 1200 0000  _finderi...s....
+0000c0d0: 0010 0401 1401 1201 0c01 0201 0c01 0601  ................
+0000c0e0: 0e01 7218 0200 0063 0100 0000 0000 0000  ..r....c........
+0000c0f0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+0000c100: 7330 0000 0074 0064 0183 0101 0074 0174  s0...t.d.....t.t
+0000c110: 02a0 027c 0064 0217 00a1 0183 017d 0164  ...|.d.......}.d
+0000c120: 0364 0484 0074 037c 0183 0144 0083 017d  .d...t.|...D...}
+0000c130: 027c 0153 0029 0572 0c02 0000 720d 0200  .|.S.).r....r...
+0000c140: 0072 0e02 0000 6301 0000 0000 0000 0000  .r....c.........
+0000c150: 0000 0003 0000 0007 0000 0053 0000 0073  ...........S...s
+0000c160: 3200 0000 6700 7c00 5d2a 5c02 7d01 7d02  2...g.|.]*\.}.}.
+0000c170: 7400 7401 7c01 8301 6400 1700 7c02 a002  t.t.|...d...|...
+0000c180: 7403 6a04 6a05 a101 6401 1900 1700 8301  t.j.j...d.......
+0000c190: 9102 7104 5300 7208 0200 0072 0902 0000  ..q.S.r....r....
+0000c1a0: 720a 0200 0072 1600 0000 7216 0000 0072  r....r....r....r
+0000c1b0: 1700 0000 7234 0000 0093 0800 0073 0400  ....r4.......s..
+0000c1c0: 0000 0600 0600 7a22 6765 745f 6d6f 6465  ......z"get_mode
+0000c1d0: 6c5f 6c69 7374 2e3c 6c6f 6361 6c73 3e2e  l_list.<locals>.
+0000c1e0: 3c6c 6973 7463 6f6d 703e 2904 724b 0000  <listcomp>).rK..
+0000c1f0: 0072 d300 0000 72b3 0100 0072 2400 0000  .r....r....r$...
+0000c200: 2903 720f 0200 0072 1002 0000 72e6 0100  ).r....r....r...
+0000c210: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+0000c220: 7211 0200 0084 0800 0073 0800 0000 000c  r........s......
+0000c230: 0801 1202 1201 6302 0000 0000 0000 0000  ......c.........
+0000c240: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+0000c250: 4800 0000 6700 7d02 7400 7c00 7401 6a02  H...g.}.t.|.t.j.
+0000c260: 1700 8301 a003 7c01 a101 4400 5d22 7d03  ......|...D.]"}.
+0000c270: 7c02 a004 7405 7c03 6a06 8301 7401 6a07  |...t.|.j...t.j.
+0000c280: 6a02 1700 7c03 6a08 1700 a101 0100 7118  j...|.j.......q.
+0000c290: 7c02 a009 a100 0100 7c02 5300 2901 61db  |.......|.S.).a.
+0000c2a0: 0100 000a 6261 7365 5f64 6972 203d 2027  ....base_dir = '
+0000c2b0: 2f63 6f6e 7465 6e74 2f67 6472 6976 652f  /content/gdrive/
+0000c2c0: 4d79 2044 7269 7665 2f4c 4947 4854 5f47  My Drive/LIGHT_G
+0000c2d0: 424d 2f46 4541 5455 5245 5f44 4154 412f  BM/FEATURE_DATA/
+0000c2e0: 270a 6e75 6d5f 666f 6c64 6572 735f 6465  '.num_folders_de
+0000c2f0: 6570 203d 2031 0a66 696c 655f 6c69 7374  ep = 1.file_list
+0000c300: 203d 205b 5d0a 666f 7220 692c 2070 6174   = [].for i, pat
+0000c310: 6820 696e 2065 6e75 6d65 7261 7465 2850  h in enumerate(P
+0000c320: 6174 6828 6261 7365 5f64 6972 202b 206f  ath(base_dir + o
+0000c330: 732e 7365 7029 2e72 676c 6f62 2827 2729  s.sep).rglob('')
+0000c340: 293a 0a20 2078 203d 2073 7472 2870 6174  ):.  x = str(pat
+0000c350: 682e 7061 7265 6e74 2920 2b20 6f73 2e70  h.parent) + os.p
+0000c360: 6174 682e 7365 7020 2b20 7061 7468 2e6e  ath.sep + path.n
+0000c370: 616d 650a 2020 6966 2069 203d 3d30 3a0a  ame.  if i ==0:.
+0000c380: 2020 2020 6669 6c65 5f6c 6973 742e 6170      file_list.ap
+0000c390: 7065 6e64 2878 290a 2020 2020 636e 7420  pend(x).    cnt 
+0000c3a0: 3d20 6c65 6e28 782e 7370 6c69 7428 6f73  = len(x.split(os
+0000c3b0: 2e73 6570 2929 0a20 2069 6620 286c 656e  .sep)).  if (len
+0000c3c0: 2878 2e73 706c 6974 286f 732e 7365 7029  (x.split(os.sep)
+0000c3d0: 292d 636e 7429 3c3d 6e75 6d5f 666f 6c64  )-cnt)<=num_fold
+0000c3e0: 6572 735f 6465 6570 3a0a 2020 2020 6669  ers_deep:.    fi
+0000c3f0: 6c65 5f6c 6973 742e 6170 7065 6e64 2878  le_list.append(x
+0000c400: 290a 6c69 7374 2873 6574 2866 696c 655f  ).list(set(file_
+0000c410: 6c69 7374 2929 0a0a 2020 2020 5061 7261  list))..    Para
+0000c420: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0000c430: 2d2d 2d2d 2d0a 2020 2020 6261 7365 5f64  -----.    base_d
+0000c440: 6972 203a 0a20 2020 2020 2020 200a 2020  ir :.        .  
+0000c450: 2020 7365 6172 6368 5f74 6572 6d20 3a0a    search_term :.
+0000c460: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0000c470: 202d 2d2d 2d2d 2d2d 0a0a 2020 2020 290a   -------..    ).
+0000c480: 720e 0000 0072 5f00 0000 7260 0000 0072  r....r_...r`...r
+0000c490: 0502 0000 7223 0000 0072 ad00 0000 7206  ....r#...r....r.
+0000c4a0: 0200 0072 6100 0000 72b6 0100 0072 6501  ...ra...r....re.
+0000c4b0: 0000 2904 72ba 0000 0072 1402 0000 da09  ..).r....r......
+0000c4c0: 6669 6c65 5f6c 6973 7472 6100 0000 7216  file_listra...r.
+0000c4d0: 0000 0072 1600 0000 7217 0000 0072 9601  ...r....r....r..
+0000c4e0: 0000 9708 0000 730a 0000 0000 1804 0118  ......s.........
+0000c4f0: 0220 0108 0172 9601 0000 6301 0000 0000  . ...r....c.....
+0000c500: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+0000c510: 0000 0073 1800 0000 7400 6a01 7c00 6401  ...s....t.j.|.d.
+0000c520: 6402 6403 8d03 7d01 7402 7c01 8301 5300  d.d...}.t.|...S.
+0000c530: 2904 61f5 0100 0074 6869 7320 6675 6e63  ).a....this func
+0000c540: 7469 6f6e 2073 686f 756c 6420 6265 2063  tion should be c
+0000c550: 616c 6c65 6420 696e 7374 6561 6420 6f66  alled instead of
+0000c560: 2064 6972 6563 7420 7370 696f 2e6c 6f61   direct spio.loa
+0000c570: 646d 6174 0a20 2020 2061 7320 6974 2063  dmat.    as it c
+0000c580: 7572 6573 2074 6865 2070 726f 626c 656d  ures the problem
+0000c590: 206f 6620 6e6f 7420 7072 6f70 6572 6c79   of not properly
+0000c5a0: 2072 6563 6f76 6572 696e 6720 7079 7468   recovering pyth
+0000c5b0: 6f6e 2064 6963 7469 6f6e 6172 6965 730a  on dictionaries.
+0000c5c0: 2020 2020 6672 6f6d 206d 6174 2066 696c      from mat fil
+0000c5d0: 6573 2e20 4974 2063 616c 6c73 2074 6865  es. It calls the
+0000c5e0: 2066 756e 6374 696f 6e20 6368 6563 6b20   function check 
+0000c5f0: 6b65 7973 2074 6f20 6375 7265 2061 6c6c  keys to cure all
+0000c600: 2065 6e74 7269 6573 0a20 2020 2077 6869   entries.    whi
+0000c610: 6368 2061 7265 2073 7469 6c6c 206d 6174  ch are still mat
+0000c620: 2d6f 626a 6563 7473 0a0a 2020 2020 6966  -objects..    if
+0000c630: 2074 6869 7320 646f 6573 6e74 2077 6f72   this doesnt wor
+0000c640: 6b20 7472 7920 7468 6973 0a20 2020 2069  k try this.    i
+0000c650: 6d70 6f72 7420 6d61 7437 330a 2020 2020  mport mat73.    
+0000c660: 6672 6f6d 2077 6861 6363 2069 6d70 6f72  from whacc impor
+0000c670: 7420 7574 696c 730a 2020 2020 6d61 745f  t utils.    mat_
+0000c680: 6669 6c65 203d 2027 2f55 7365 7273 2f70  file = '/Users/p
+0000c690: 6869 6c2f 4472 6f70 626f 782f 555f 3139  hil/Dropbox/U_19
+0000c6a0: 3130 3238 5f31 3135 342e 6d61 7427 0a20  1028_1154.mat'. 
+0000c6b0: 2020 2064 6174 615f 6469 6374 203d 206d     data_dict = m
+0000c6c0: 6174 3733 2e6c 6f61 646d 6174 286d 6174  at73.loadmat(mat
+0000c6d0: 5f66 696c 6529 0a0a 2020 2020 5061 7261  _file)..    Para
+0000c6e0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0000c6f0: 2d2d 2d2d 2d0a 2020 2020 6669 6c65 6e61  -----.    filena
+0000c700: 6d65 203a 0a20 2020 2020 2020 200a 0a20  me :.        .. 
+0000c710: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0000c720: 2d2d 2d2d 2d2d 0a0a 2020 2020 4654 2902  ------..    FT).
+0000c730: 5a10 7374 7275 6374 5f61 735f 7265 636f  Z.struct_as_reco
+0000c740: 7264 5a0a 7371 7565 657a 655f 6d65 2903  rdZ.squeeze_me).
+0000c750: da04 7370 696f da07 6c6f 6164 6d61 74da  ..spio..loadmat.
+0000c760: 0b5f 6368 6563 6b5f 6b65 7973 2902 727c  ._check_keys).r|
+0000c770: 0000 0072 2a00 0000 7216 0000 0072 1600  ...r*...r....r..
+0000c780: 0000 7217 0000 0072 1b02 0000 c108 0000  ..r....r........
+0000c790: 7304 0000 0000 1510 0172 1b02 0000 6301  s........r....c.
+0000c7a0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+0000c7b0: 0000 0043 0000 0073 3200 0000 7c00 4400  ...C...s2...|.D.
+0000c7c0: 5d28 7d01 7400 7c00 7c01 1900 7401 6a02  ](}.t.|.|...t.j.
+0000c7d0: 6a03 6a04 8302 7204 7405 7c00 7c01 1900  j.j...r.t.|.|...
+0000c7e0: 8301 7c00 7c01 3c00 7104 7c00 5300 2901  ..|.|.<.q.|.S.).
+0000c7f0: 7ac4 6368 6563 6b73 2069 6620 656e 7472  z.checks if entr
+0000c800: 6965 7320 696e 2064 6963 7469 6f6e 6172  ies in dictionar
+0000c810: 7920 6172 6520 6d61 742d 6f62 6a65 6374  y are mat-object
+0000c820: 732e 2049 6620 7965 730a 2020 2020 746f  s. If yes.    to
+0000c830: 6469 6374 2069 7320 6361 6c6c 6564 2074  dict is called t
+0000c840: 6f20 6368 616e 6765 2074 6865 6d20 746f  o change them to
+0000c850: 206e 6573 7465 6420 6469 6374 696f 6e61   nested dictiona
+0000c860: 7269 6573 0a0a 2020 2020 5061 7261 6d65  ries..    Parame
+0000c870: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000c880: 2d2d 2d0a 2020 2020 6469 6374 203a 0a20  ---.    dict :. 
+0000c890: 2020 2020 2020 200a 0a20 2020 2052 6574         ..    Ret
+0000c8a0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+0000c8b0: 0a0a 2020 2020 2906 720b 0100 0072 1a02  ..    ).r....r..
+0000c8c0: 0000 da06 6d61 746c 6162 da0b 6d69 6f35  ....matlab..mio5
+0000c8d0: 5f70 6172 616d 73da 0a6d 6174 5f73 7472  _params..mat_str
+0000c8e0: 7563 74da 075f 746f 6469 6374 2902 7269  uct.._todict).ri
+0000c8f0: 0000 00da 036b 6579 7216 0000 0072 1600  .....keyr....r..
+0000c900: 0000 7217 0000 0072 1c02 0000 da08 0000  ..r....r........
+0000c910: 7308 0000 0000 0d08 0114 0112 0172 1c02  s............r..
+0000c920: 0000 6301 0000 0000 0000 0000 0000 0004  ..c.............
+0000c930: 0000 0004 0000 0043 0000 0073 4400 0000  .......C...sD...
+0000c940: 6900 7d01 7c00 6a00 4400 5d34 7d02 7c00  i.}.|.j.D.]4}.|.
+0000c950: 6a01 7c02 1900 7d03 7402 7c03 7403 6a04  j.|...}.t.|.t.j.
+0000c960: 6a05 6a06 8302 7236 7407 7c03 8301 7c01  j.j...r6t.|...|.
+0000c970: 7c02 3c00 710a 7c03 7c01 7c02 3c00 710a  |.<.q.|.|.|.<.q.
+0000c980: 7c01 5300 2901 7a9d 4120 7265 6375 7273  |.S.).z.A recurs
+0000c990: 6976 6520 6675 6e63 7469 6f6e 2077 6869  ive function whi
+0000c9a0: 6368 2063 6f6e 7374 7275 6374 7320 6672  ch constructs fr
+0000c9b0: 6f6d 206d 6174 6f62 6a65 6374 7320 6e65  om matobjects ne
+0000c9c0: 7374 6564 2064 6963 7469 6f6e 6172 6965  sted dictionarie
+0000c9d0: 730a 0a20 2020 2050 6172 616d 6574 6572  s..    Parameter
+0000c9e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0000c9f0: 0a20 2020 206d 6174 6f62 6a20 3a0a 2020  .    matobj :.  
+0000ca00: 2020 2020 2020 0a0a 2020 2020 5265 7475        ..    Retu
+0000ca10: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0000ca20: 0a20 2020 2029 085a 0b5f 6669 656c 646e  .    ).Z._fieldn
+0000ca30: 616d 6573 da08 5f5f 6469 6374 5f5f 720b  ames..__dict__r.
+0000ca40: 0100 0072 1a02 0000 721d 0200 0072 1e02  ...r....r....r..
+0000ca50: 0000 721f 0200 0072 2002 0000 2904 5a06  ..r....r ...).Z.
+0000ca60: 6d61 746f 626a 7269 0000 00da 0473 7472  matobjri.....str
+0000ca70: 67da 0465 6c65 6d72 1600 0000 7216 0000  g..elemr....r...
+0000ca80: 0072 1700 0000 7220 0200 00ed 0800 0073  .r....r .......s
+0000ca90: 0e00 0000 000c 0401 0a01 0a01 1001 0e02  ................
+0000caa0: 0a01 7220 0200 0063 0200 0000 0000 0000  ..r ...c........
+0000cab0: 0000 0000 0500 0000 0900 0000 0300 0000  ................
+0000cac0: 739e 0000 0067 007d 027c 0044 005d 2a89  s....g.}.|.D.]*.
+0000cad0: 007c 02a0 0074 0174 02a0 0387 0066 0164  .|...t.t.....f.d
+0000cae0: 0164 0284 087c 0044 0083 01a1 0164 0319  .d...|.D.....d..
+0000caf0: 0083 01a1 0101 0071 087a 3474 0174 026a  .......q.z4t.t.j
+0000cb00: 047c 0264 0364 048d 0283 017d 0374 057c  .|.d.d.....}.t.|
+0000cb10: 0383 0144 005d 145c 027d 0489 0074 0188  ...D.].\.}...t..
+0000cb20: 0083 017c 037c 043c 0071 5057 006e 1a01  ...|.|.<.qPW.n..
+0000cb30: 0001 0001 0074 0174 02a0 047c 02a1 0183  .....t.t...|....
+0000cb40: 017d 0359 006e 0258 007c 0172 967c 0374  .}.Y.n.X.|.r.|.t
+0000cb50: 06a0 047c 00a1 0166 0253 007c 0353 0064  ...|...f.S.|.S.d
+0000cb60: 0053 0029 054e 6301 0000 0000 0000 0000  .S.).Nc.........
+0000cb70: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+0000cb80: 1400 0000 6700 7c00 5d0c 7d01 8800 7c01  ....g.|.].}...|.
+0000cb90: 6b02 9102 7104 5300 7216 0000 0072 1600  k...q.S.r....r..
+0000cba0: 0000 2902 7232 0000 00da 026b 6ba9 0172  ..).r2.....kk..r
+0000cbb0: 3300 0000 7216 0000 0072 1700 0000 7234  3...r....r....r4
+0000cbc0: 0000 0006 0900 0073 0400 0000 0600 0200  .......s........
+0000cbd0: 7a24 6765 745f 696e 6473 5f6f 665f 696e  z$get_inds_of_in
+0000cbe0: 6473 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ds.<locals>.<lis
+0000cbf0: 7463 6f6d 703e 7201 0000 0072 ff00 0000  tcomp>r....r....
+0000cc00: 2907 7223 0000 0072 3900 0000 721d 0000  ).r#...r9...r...
+0000cc10: 0072 b900 0000 72d2 0000 0072 2400 0000  .r....r....r$...
+0000cc20: 729f 0100 0029 0572 e500 0000 5a12 7265  r....).r....Z.re
+0000cc30: 7475 726e 5f75 6e69 7175 655f 6c69 7374  turn_unique_list
+0000cc40: da02 6132 da0c 696e 6473 5f6f 665f 696e  ..a2..inds_of_in
+0000cc50: 6473 722c 0000 0072 1600 0000 7226 0200  dsr,...r....r&..
+0000cc60: 0072 1700 0000 da10 6765 745f 696e 6473  .r......get_inds
+0000cc70: 5f6f 665f 696e 6473 0309 0000 7318 0000  _of_inds....s...
+0000cc80: 0000 0104 0108 0128 0102 0112 0110 0112  .......(........
+0000cc90: 0106 0114 0104 010e 0272 2902 0000 6302  .........r)...c.
+0000cca0: 0000 0000 0000 0000 0000 0004 0000 0007  ................
+0000ccb0: 0000 0043 0000 0073 7a00 0000 7c01 6401  ...C...sz...|.d.
+0000ccc0: 1b00 7400 7c01 6401 1b00 8301 6b03 731c  ..t.|.d.....k.s.
+0000ccd0: 7401 6402 8301 8201 7402 a003 7402 a004  t.d.....t...t...
+0000cce0: 7c00 6403 6403 a103 a101 7d02 7c02 7c01  |.d.d.....}.|.|.
+0000ccf0: 6404 8502 1900 7c02 6404 7c01 0b00 8502  d.....|.d.|.....
+0000cd00: 1900 1800 7405 7c01 8301 1b00 7d03 7402  ....t.|.....}.t.
+0000cd10: a006 7c03 6403 6b04 a101 6403 1900 7c01  ..|.d.k...d...|.
+0000cd20: 6405 1800 6401 1b00 1700 7d03 7c03 a007  d...d.....}.|...
+0000cd30: 6406 a101 5300 2907 7ae8 0a0a 2020 2020  d...S.).z...    
+0000cd40: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000cd50: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7820  ---------.    x 
+0000cd60: 3a20 6172 7261 790a 2020 2020 4e20 3a20  : array.    N : 
+0000cd70: 7769 6e64 6f77 2073 697a 650a 0a20 2020  window size..   
+0000cd80: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+0000cd90: 2d2d 2d2d 0a20 2020 2072 6574 7572 6e73  ----.    returns
+0000cda0: 2069 6e64 6963 6573 206f 6620 6172 7261   indices of arra
+0000cdb0: 7973 2077 6865 7265 2061 7272 6179 203e  ys where array >
+0000cdc0: 3020 7769 7468 2062 6f72 6465 7273 206f  0 with borders o
+0000cdd0: 6620 2828 4e20 2d20 3129 202f 2032 292c  f ((N - 1) / 2),
+0000cde0: 2073 6f20 7820 3d20 5b30 2c20 302c 2030   so x = [0, 0, 0
+0000cdf0: 2c20 312c 2030 2c20 302c 2030 5d20 616e  , 1, 0, 0, 0] an
+0000ce00: 6420 4e20 3d20 330a 2020 2020 7265 7475  d N = 3.    retu
+0000ce10: 726e 7320 5b32 2c20 332c 2034 5d0a 2020  rns [2, 3, 4].  
+0000ce20: 2020 7247 0000 007a 4d4e 206d 7573 7420    rG...zMN must 
+0000ce30: 6265 2061 6e20 6f64 6420 6e75 6d62 6572  be an odd number
+0000ce40: 2073 6f20 7468 6174 2074 6865 7265 2061   so that there a
+0000ce50: 7265 2065 7175 616c 206e 756d 6265 7220  re equal number 
+0000ce60: 6f66 2070 6f69 6e74 7320 6f6e 2065 6163  of points on eac
+0000ce70: 6820 7369 6465 7201 0000 004e 722e 0000  h sider....Nr...
+0000ce80: 0072 8800 0000 2908 728c 0000 0072 4e00  .r....).r....rN.
+0000ce90: 0000 721d 0000 0072 6801 0000 da06 696e  ..r....rh.....in
+0000cea0: 7365 7274 7289 0000 0072 b900 0000 7285  sertr....r....r.
+0000ceb0: 0000 0029 0472 5300 0000 da01 4e72 6801  ...).rS.....Nrh.
+0000cec0: 0000 72e5 0000 0072 1600 0000 7216 0000  ..r....r....r...
+0000ced0: 0072 1700 0000 da10 696e 6473 5f61 726f  .r......inds_aro
+0000cee0: 756e 645f 696e 6473 1309 0000 730a 0000  und_inds....s...
+0000cef0: 0000 0d1c 0114 0122 011e 0172 2c02 0000  ......."...r,...
+0000cf00: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+0000cf10: 0006 0000 0043 0000 0073 7000 0000 7400  .....C...sp...t.
+0000cf20: 7c00 8301 7d00 6401 6701 7c00 1700 7d00  |...}.d.g.|...}.
+0000cf30: 7401 a002 7c00 a101 7d00 7c00 a003 7404  t...|...}.|...t.
+0000cf40: a101 7d00 7c01 724a 7400 7c00 6402 6403  ..}.|.rJt.|.d.d.
+0000cf50: 8502 1900 8301 7400 7c00 6404 6402 8502  ......t.|.d.d...
+0000cf60: 1900 8301 6702 5300 7405 7400 7c00 6402  ....g.S.t.t.|.d.
+0000cf70: 6403 8502 1900 8301 7400 7c00 6404 6402  d.......t.|.d.d.
+0000cf80: 8502 1900 8301 8302 5300 6402 5300 2905  ........S.d.S.).
+0000cf90: 61ab 0100 000a 0a20 2020 2050 6172 616d  a......    Param
+0000cfa0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0000cfb0: 2d2d 2d2d 0a20 2020 2066 7261 6d65 5f6e  ----.    frame_n
+0000cfc0: 756d 5f61 7272 6179 203a 0a20 2020 206e  um_array :.    n
+0000cfd0: 756d 206f 6620 6672 616d 6573 2069 6e20  um of frames in 
+0000cfe0: 6561 6368 2074 7269 616c 2069 6e20 6120  each trial in a 
+0000cff0: 6c69 7374 0a20 2020 2052 6574 7572 6e73  list.    Returns
+0000d000: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0000d010: 2032 206c 6973 7473 2077 6974 6820 7468   2 lists with th
+0000d020: 6520 7072 6f70 6572 2069 6e64 6578 2066  e proper index f
+0000d030: 6f72 2070 756c 6c69 6e67 2074 686f 7365  or pulling those
+0000d040: 2074 7269 616c 7320 6f75 7420 6f6e 6520   trials out one 
+0000d050: 6279 206f 6e65 2069 6e20 6120 666f 7220  by one in a for 
+0000d060: 6c6f 6f70 0a20 2020 2045 7861 6d70 6c65  loop.    Example
+0000d070: 730a 2020 2020 5f5f 5f5f 5f5f 5f5f 0a20  s.    ________. 
+0000d080: 2020 2061 3320 3d20 5b30 2c20 312c 2032     a3 = [0, 1, 2
+0000d090: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
+0000d0a0: 2038 5d0a 2020 2020 6672 616d 655f 6e75   8].    frame_nu
+0000d0b0: 6d5f 6172 7261 7920 3d20 5b34 2c20 355d  m_array = [4, 5]
+0000d0c0: 0a20 2020 2066 6f72 2069 312c 2069 3220  .    for i1, i2 
+0000d0d0: 696e 206c 6f6f 705f 7365 676d 656e 7473  in loop_segments
+0000d0e0: 2866 7261 6d65 5f6e 756d 5f61 7272 6179  (frame_num_array
+0000d0f0: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
+0000d100: 2861 335b 6931 3a69 325d 290a 0a20 2020  (a3[i1:i2])..   
+0000d110: 2023 203e 3e3e 5b30 2c20 312c 2032 2c20   # >>>[0, 1, 2, 
+0000d120: 335d 0a20 2020 2023 203e 3e3e 5b34 2c20  3].    # >>>[4, 
+0000d130: 352c 2036 2c20 372c 2038 5d0a 2020 2020  5, 6, 7, 8].    
+0000d140: 7201 0000 004e 724a 0000 0072 2e00 0000  r....NrJ...r....
+0000d150: 2906 7239 0000 0072 1d00 0000 7268 0100  ).r9...r....rh..
+0000d160: 0072 8500 0000 7288 0000 0072 b000 0000  .r....r....r....
+0000d170: 2902 5a0f 6672 616d 655f 6e75 6d5f 6172  ).Z.frame_num_ar
+0000d180: 7261 795a 0c72 6574 7572 6e61 736c 6973  rayZ.returnaslis
+0000d190: 7472 1600 0000 7216 0000 0072 1700 0000  tr....r....r....
+0000d1a0: 7237 0000 0027 0900 0073 0e00 0000 0014  r7...'...s......
+0000d1b0: 0801 0a01 0a01 0a01 0401 2002 7237 0000  .......... .r7..
+0000d1c0: 0063 0200 0000 0000 0000 0000 0000 0d00  .c..............
+0000d1d0: 0000 0b00 0000 4300 0000 73ec 0000 0067  ......C...s....g
+0000d1e0: 007d 0264 0164 0284 007c 0044 0083 017d  .}.d.d...|.D...}
+0000d1f0: 0374 007c 0364 0383 025c 027d 047d 0564  .t.|.d...\.}.}.d
+0000d200: 0464 0284 007c 0044 0083 017d 0674 01a0  .d...|.D...}.t..
+0000d210: 027c 06a1 0174 01a0 027c 04a1 0119 007d  .|...t...|.....}
+0000d220: 0674 037c 0483 0144 005d 7a5c 027d 077d  .t.|...D.]z\.}.}
+0000d230: 0874 01a0 0467 00a1 017d 0974 037c 0883  .t...g...}.t.|..
+0000d240: 0144 005d 545c 027d 0a7d 0b74 05a0 067c  .D.]T\.}.}.t...|
+0000d250: 007c 0b19 0064 05a1 028f 367d 0c7c 096a  .|...d....6}.|.j
+0000d260: 0772 9e74 01a0 087c 097c 0c64 0619 0064  .r.t...|.|.d...d
+0000d270: 0764 0785 0219 0067 02a1 016e 0e7c 0c64  .d.....g...n.|.d
+0000d280: 0619 0064 0764 0785 0219 007d 0957 0035  ...d.d.....}.W.5
+0000d290: 0051 0052 0058 0071 647c 02a0 097c 09a1  .Q.R.X.qd|...|..
+0000d2a0: 0101 0071 4a7c 0172 e07c 027c 057c 0664  ...qJ|.r.|.|.|.d
+0000d2b0: 0864 0764 0785 0266 0219 0066 0353 007c  .d.d...f...f.S.|
+0000d2c0: 027c 0566 0253 0064 0753 0029 097a 920a  .|.f.S.d.S.).z..
+0000d2d0: 2020 2020 6a75 7374 2075 7365 6420 746f      just used to
+0000d2e0: 2067 6574 2061 7272 6179 206f 6620 636f   get array of co
+0000d2f0: 6e74 6163 7473 2c20 6e6f 7420 6d65 616e  ntacts, not mean
+0000d300: 7420 746f 2062 6520 7573 6564 206c 6f6e  t to be used lon
+0000d310: 6720 7465 726d 0a20 2020 2050 6172 616d  g term.    Param
+0000d320: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0000d330: 2d2d 2d2d 0a20 2020 2061 6c6c 5f68 3573  ----.    all_h5s
+0000d340: 203a 0a0a 2020 2020 5265 7475 726e 730a   :..    Returns.
+0000d350: 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020      -------..   
+0000d360: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
+0000d370: 0000 0600 0000 5300 0000 732c 0000 0067  ......S...s,...g
+0000d380: 007c 005d 247d 017c 01a0 0074 016a 026a  .|.]$}.|...t.j.j
+0000d390: 03a1 0164 0019 006a 0064 0164 0264 038d  ...d...j.d.d.d..
+0000d3a0: 0264 0019 0091 0271 0453 0029 0472 4a00  .d.....q.S.).rJ.
+0000d3b0: 0000 72e6 0100 0072 2e00 0000 2901 da08  ..r....r....)...
+0000d3c0: 6d61 7873 706c 6974 2904 72db 0000 0072  maxsplit).r....r
+0000d3d0: 5f00 0000 7261 0000 0072 6000 0000 7231  _...ra...r`...r1
+0000d3e0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+0000d3f0: 0000 7234 0000 0064 0900 0073 0400 0000  ..r4...d...s....
+0000d400: 0600 0200 7a28 5f67 6574 5f68 756d 616e  ....z(_get_human
+0000d410: 5f63 6f6e 7461 6374 735f 2e3c 6c6f 6361  _contacts_.<loca
+0000d420: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 5463  ls>.<listcomp>Tc
+0000d430: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+0000d440: 0700 0000 5300 0000 7320 0000 0067 007c  ....S...s ...g.|
+0000d450: 005d 187d 0174 006a 01a0 0274 006a 01a0  .].}.t.j...t.j..
+0000d460: 037c 01a1 01a1 0191 0271 0453 0072 1600  .|.......q.S.r..
+0000d470: 0000 2904 725f 0000 0072 6100 0000 72a8  ..).r_...ra...r.
+0000d480: 0000 0072 a700 0000 7231 0000 0072 1600  ...r....r1...r..
+0000d490: 0000 7216 0000 0072 1700 0000 7234 0000  ..r....r....r4..
+0000d4a0: 0067 0900 0073 0400 0000 0600 0200 726d  .g...s........rm
+0000d4b0: 0000 0072 5200 0000 4e72 0100 0000 290a  ...rR...Nr....).
+0000d4c0: 7229 0200 0072 1d00 0000 7238 0000 0072  r)...r....r8...r
+0000d4d0: 2400 0000 da05 6172 7261 7972 ae00 0000  $.....arrayr....
+0000d4e0: 72af 0000 0072 3001 0000 7225 0000 0072  r....r0...r%...r
+0000d4f0: 2300 0000 290d 5a07 616c 6c5f 6835 735a  #...).Z.all_h5sZ
+0000d500: 1472 6574 7572 6e5f 6375 7261 746f 725f  .return_curator_
+0000d510: 6e61 6d65 73da 0668 5f63 6f6e 7472 e500  names..h_contr..
+0000d520: 0000 7228 0200 005a 126c 6973 745f 6f66  ..r(...Z.list_of
+0000d530: 5f75 6e69 715f 6669 6c65 735a 0d63 7572  _uniq_filesZ.cur
+0000d540: 6174 6f72 5f6e 616d 6573 722c 0000 0072  ator_namesr,...r
+0000d550: 3300 0000 72fb 0000 0072 3e00 0000 7225  3...r....r>...r%
+0000d560: 0200 0072 c000 0000 7216 0000 0072 1600  ...r....r....r..
+0000d570: 0000 7217 0000 00da 145f 6765 745f 6875  ..r......_get_hu
+0000d580: 6d61 6e5f 636f 6e74 6163 7473 5f58 0900  man_contacts_X..
+0000d590: 0073 1c00 0000 000b 0401 0e01 0e02 0e01  .s..............
+0000d5a0: 1401 1001 0a01 1001 1201 3c01 0c01 0401  ..........<.....
+0000d5b0: 1602 7230 0200 00e9 5000 0000 6305 0000  ..r0....P...c...
+0000d5c0: 0000 0000 0000 0000 0013 0000 000a 0000  ................
+0000d5d0: 0003 0000 0073 1802 0000 6700 7d05 7400  .....s....g.}.t.
+0000d5e0: 7c01 7c02 8302 4400 9001 5dbc 5c02 7d06  |.|...D...].\.}.
+0000d5f0: 7d07 7401 7c07 6a02 8301 6401 6b02 7234  }.t.|.j...d.k.r4
+0000d600: 7403 a004 7c07 7c07 6602 a101 7d07 7405  t...|.|.f...}.t.
+0000d610: a006 7c06 6402 a102 9001 8f84 7d08 7403  ..|.d.......}.t.
+0000d620: 6a07 7c07 6403 6404 8d02 7d09 7403 6a08  j.|.d.d...}.t.j.
+0000d630: 7c07 6403 6404 8d02 7d0a 7c0a 6405 6b04  |.d.d...}.|.d.k.
+0000d640: 6401 1400 7d0a 7409 7c09 7c03 6406 1400  d...}.t.|.|.d...
+0000d650: 6401 1700 8302 8900 740a 8800 8301 5c02  d.......t.....\.
+0000d660: 7d0b 7d0c 7c0b 4400 5d12 7d0d 7c05 a00b  }.}.|.D.].}.|...
+0000d670: 7401 7c0d 8301 a101 0100 718e 8700 6601  t.|.......q...f.
+0000d680: 6407 6408 8408 7403 a00c 740d 6409 7c04  d.d...t...t.d.|.
+0000d690: 6401 1700 8302 a101 4400 8301 7d0e 7c0e  d.......D...}.|.
+0000d6a0: 73de 740e 640a 7401 8800 8301 640b 7c04  s.t.d.t.....d.|.
+0000d6b0: 640c 6705 8301 8201 7403 a007 7c0e a101  d.g.....t...|...
+0000d6c0: 7d0e 7403 a00f 6700 a101 7d0f 7403 a00f  }.t...g...}.t...
+0000d6d0: 6700 a101 7d10 6403 7d11 7410 8800 8301  g...}.d.}.t.....
+0000d6e0: 4400 5dac 7d12 7c11 6401 3700 7d11 7c0f  D.].}.|.d.7.}.|.
+0000d6f0: 6a11 9001 725c 7403 6a12 7c0f 7c08 640d  j...r\t.j.|.|.d.
+0000d700: 1900 7c12 1900 640e 640e 640e 8502 640e  ..|...d.d.d...d.
+0000d710: 640e 8502 6403 6604 1900 6602 6403 6404  d...d.f...f.d.d.
+0000d720: 8d02 7d0f 7403 a00b 7c10 7c09 7c12 1900  ..}.t...|.|.|...
+0000d730: a102 7d10 6e28 7c08 640d 1900 7c12 1900  ..}.n(|.d...|...
+0000d740: 640e 640e 640e 8502 640e 640e 8502 6403  d.d.d...d.d...d.
+0000d750: 6604 1900 7d0f 7c0a 7c12 1900 7d10 7c11  f...}.|.|...}.|.
+0000d760: 7c0e 6b05 9001 7208 7c00 a013 7c0f 7c10  |.k...r.|...|.|.
+0000d770: a102 0100 7403 a00f 6700 a101 7d0f 7403  ....t...g...}.t.
+0000d780: a00f 6700 a101 7d10 6403 7d11 9001 7108  ..g...}.d.}...q.
+0000d790: 7c00 a013 7c0f 7c10 a102 0100 5700 3500  |...|.|.....W.5.
+0000d7a0: 5100 5200 5800 710e 7405 a006 7c00 6a14  Q.R.X.q.t...|.j.
+0000d7b0: 640f a102 8f32 7d08 7c08 6a15 6410 7403  d....2}.|.j.d.t.
+0000d7c0: a002 7c05 a101 7c05 6411 8d03 0100 7c08  ..|...|.d.....|.
+0000d7d0: 6a15 6412 7403 a002 8800 a101 8800 6411  j.d.t.........d.
+0000d7e0: 8d03 0100 5700 3500 5100 5200 5800 640e  ....W.5.Q.R.X.d.
+0000d7f0: 5300 2913 617b 0500 000a 2020 2020 5061  S.).a{....    Pa
+0000d800: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+0000d810: 2d2d 2d2d 2d2d 2d0a 2020 2020 6835 6320  -------.    h5c 
+0000d820: 3a20 6835 2063 7265 6174 6f72 2063 6c61  : h5 creator cla
+0000d830: 7373 0a20 2020 2061 6c6c 5f68 3573 5f69  ss.    all_h5s_i
+0000d840: 6d67 7320 3a20 6c69 7374 206f 6620 6835  mgs : list of h5
+0000d850: 7320 7769 7468 2069 6d61 6765 730a 2020  s with images.  
+0000d860: 2020 685f 636f 6e74 203a 2061 2074 656e    h_cont : a ten
+0000d870: 736f 7220 6f66 2068 756d 616e 2063 6f6e  sor of human con
+0000d880: 7461 6374 7320 7065 6f70 6c65 2062 7920  tacts people by 
+0000d890: 6672 616d 6573 2074 7269 616c 2048 3520  frames trial H5 
+0000d8a0: 6669 6c65 7320 2864 6f77 6e20 7269 6768  files (down righ
+0000d8b0: 7420 6465 6570 290a 2020 2020 626f 7264  t deep).    bord
+0000d8c0: 6572 7320 3a20 666f 7220 746f 7563 6820  ers : for touch 
+0000d8d0: 3030 3030 3031 3131 3030 3030 3020 6974  0000011100000 it
+0000d8e0: 2077 696c 6c20 6669 6e64 2074 6865 2031   will find the 1
+0000d8f0: 3131 2069 6e20 6974 2061 6e64 2067 6574  11 in it and get
+0000d900: 2061 6c6c 2074 6865 2062 6f72 6465 7269   all the borderi
+0000d910: 6e67 2061 7265 6173 2061 726f 756e 6420  ng areas around 
+0000d920: 6974 2e20 706f 696e 7473 2061 7265 0a20  it. points are. 
+0000d930: 2020 2075 6e69 7175 6520 736f 2030 3030     unique so 000
+0000d940: 3030 3131 3130 3030 3030 2061 6e64 2030  0011100000 and 0
+0000d950: 3030 3030 3130 3130 3030 3030 2077 696c  000010100000 wil
+0000d960: 6c20 7265 7475 726e 2074 6865 2073 616d  l return the sam
+0000d970: 6520 696e 6465 780a 2020 2020 6d61 785f  e index.    max_
+0000d980: 7061 636b 5f76 616c 203a 2073 7065 6564  pack_val : speed
+0000d990: 7320 7570 2074 6865 2070 726f 6365 7373  s up the process
+0000d9a0: 2062 7920 7472 616e 7366 6572 7269 6e67   by transferring
+0000d9b0: 2064 6174 6120 696e 2063 6875 6e6b 7320   data in chunks 
+0000d9c0: 6f66 2074 6869 7320 6d61 7820 7369 7a65  of this max size
+0000d9d0: 2069 6e73 7465 6164 206f 6620 6275 696c   instead of buil
+0000d9e0: 6469 6e67 2074 6865 6d20 616c 6c20 7570  ding them all up
+0000d9f0: 2069 6e20 6d65 6d6f 7279 0a20 2020 2069   in memory.    i
+0000da00: 7427 7320 6120 6d61 7820 696e 7374 6561  t's a max instea
+0000da10: 6420 6f66 2061 2073 6574 2076 616c 7565  d of a set value
+0000da20: 2062 6563 6175 7365 2069 7420 6361 6e20   because it can 
+0000da30: 6265 2069 6620 7468 6520 6c65 6e28 494d  be if the len(IM
+0000da40: 4147 4553 2925 6d61 785f 7061 636b 5f76  AGES)%max_pack_v
+0000da50: 616c 2069 7320 6571 7561 6c20 746f 2030  al is equal to 0
+0000da60: 206f 7220 3120 6974 2077 696c 6c20 6372   or 1 it will cr
+0000da70: 6173 682c 2073 6f20 4920 6361 6c63 756c  ash, so I calcul
+0000da80: 6174 6520 6974 0a20 2020 2073 6f20 7468  ate it.    so th
+0000da90: 6174 2069 7420 776f 6e74 2063 7261 7368  at it wont crash
+0000daa0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0000dab0: 2020 202d 2d2d 2d2d 2d2d 6372 6561 7465     -------create
+0000dac0: 5f6d 6173 7465 725f 6461 7461 7365 740a  _master_dataset.
+0000dad0: 2020 2020 7361 7665 7320 616e 2048 3520      saves an H5 
+0000dae0: 6669 6c65 0a20 2020 2045 7861 6d70 6c65  file.    Example
+0000daf0: 730a 2020 2020 5f5f 5f5f 5f5f 5f5f 0a0a  s.    ________..
+0000db00: 2020 2020 616c 6c5f 6835 7320 3d20 7574      all_h5s = ut
+0000db10: 696c 732e 6765 745f 6835 7328 272f 636f  ils.get_h5s('/co
+0000db20: 6e74 656e 742f 6764 7269 7665 2f4d 7920  ntent/gdrive/My 
+0000db30: 4472 6976 652f 436f 6c61 6220 6461 7461  Drive/Colab data
+0000db40: 2f63 7572 6174 696f 6e5f 666f 725f 6175  /curation_for_au
+0000db50: 746f 5f63 7572 6174 6f72 2f66 696e 6973  to_curator/finis
+0000db60: 6865 645f 636f 6e74 6163 7473 2f27 290a  hed_contacts/').
+0000db70: 2020 2020 616c 6c5f 6835 735f 696d 6773      all_h5s_imgs
+0000db80: 203d 2075 7469 6c73 2e67 6574 5f68 3573   = utils.get_h5s
+0000db90: 2827 2f63 6f6e 7465 6e74 2f67 6472 6976  ('/content/gdriv
+0000dba0: 652f 4d79 2044 7269 7665 2f43 6f6c 6162  e/My Drive/Colab
+0000dbb0: 2064 6174 612f 6375 7261 7469 6f6e 5f66   data/curation_f
+0000dbc0: 6f72 5f61 7574 6f5f 6375 7261 746f 722f  or_auto_curator/
+0000dbd0: 4835 5f64 6174 612f 2729 0a20 2020 2068  H5_data/').    h
+0000dbe0: 5f63 6f6e 7420 3d20 7574 696c 732e 5f67  _cont = utils._g
+0000dbf0: 6574 5f68 756d 616e 5f63 6f6e 7461 6374  et_human_contact
+0000dc00: 735f 2861 6c6c 5f68 3573 290a 2020 2020  s_(all_h5s).    
+0000dc10: 6835 6320 3d20 696d 6167 655f 746f 6f6c  h5c = image_tool
+0000dc20: 732e 6835 5f69 7465 7261 7469 7665 5f63  s.h5_iterative_c
+0000dc30: 7265 6174 6f72 2827 2f63 6f6e 7465 6e74  reator('/content
+0000dc40: 2f67 6472 6976 652f 4d79 2044 7269 7665  /gdrive/My Drive
+0000dc50: 2f43 6f6c 6162 2064 6174 612f 6375 7261  /Colab data/cura
+0000dc60: 7469 6f6e 5f66 6f72 5f61 7574 6f5f 6375  tion_for_auto_cu
+0000dc70: 7261 746f 722f 7465 7374 5f5f 5f5f 5f2e  rator/test_____.
+0000dc80: 6835 272c 0a20 2020 2020 2020 2020 2020  h5',.           
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcb0: 6f76 6572 7772 6974 655f 6966 5f66 696c  overwrite_if_fil
+0000dcc0: 655f 6578 6973 7473 203d 2054 7275 652c  e_exists = True,
+0000dcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+0000dd00: 725f 6368 616e 6e65 6c20 3d20 4661 6c73  r_channel = Fals
+0000dd10: 6529 0a20 2020 2075 7469 6c73 2e63 7265  e).    utils.cre
+0000dd20: 6174 655f 6d61 7374 6572 5f64 6174 6173  ate_master_datas
+0000dd30: 6574 2868 3563 2c20 616c 6c5f 6835 735f  et(h5c, all_h5s_
+0000dd40: 696d 6773 2c20 685f 636f 6e74 2c20 626f  imgs, h_cont, bo
+0000dd50: 7264 6572 7320 3d20 3830 2c20 6d61 785f  rders = 80, max_
+0000dd60: 7061 636b 5f76 616c 203d 2031 3030 290a  pack_val = 100).
+0000dd70: 2020 2020 722e 0000 0072 6d00 0000 7201      r....rm...r.
+0000dd80: 0000 0072 ff00 0000 729c 0000 0072 4700  ...r....r....rG.
+0000dd90: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+0000dda0: 0000 0004 0000 0013 0000 0073 2000 0000  ...........s ...
+0000ddb0: 6700 7c00 5d18 7d01 7400 8800 8301 7c01  g.|.].}.t.....|.
+0000ddc0: 1600 6400 6b05 7204 7c01 9102 7104 5300  ..d.k.r.|...q.S.
+0000ddd0: 2901 7247 0000 0072 4800 0000 7231 0000  ).rG...rH...r1..
+0000dde0: 00a9 0172 4200 0000 7216 0000 0072 1700  ...rB...r....r..
+0000ddf0: 0000 7234 0000 009d 0900 0073 0600 0000  ..r4.......s....
+0000de00: 0600 0200 1000 7a29 6372 6561 7465 5f6d  ......z)create_m
+0000de10: 6173 7465 725f 6461 7461 7365 742e 3c6c  aster_dataset.<l
+0000de20: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+0000de30: 3e72 4600 0000 7a1c 6368 6f73 656e 2048  >rF...z.chosen H
+0000de40: 3520 6669 6c65 2068 6173 2076 616c 7565  5 file has value
+0000de50: 206f 6620 7a15 2061 6e64 206d 6178 5f70   of z. and max_p
+0000de60: 6163 6b5f 7661 6c20 6973 207a 2c20 696e  ack_val is z, in
+0000de70: 6372 6561 7365 206d 6178 5f70 6163 6b5f  crease max_pack_
+0000de80: 7661 6c20 746f 2070 7265 7665 6e74 2074  val to prevent t
+0000de90: 6869 7320 6572 726f 7272 9a00 0000 4e72  his errorr....Nr
+0000dea0: a600 0000 7241 0000 0072 ce01 0000 5a0e  ....rA...r....Z.
+0000deb0: 696e 6473 5f65 7874 7261 6374 6564 2916  inds_extracted).
+0000dec0: 72b0 0000 0072 3000 0000 7221 0000 0072  r....r0...r!...r
+0000ded0: 1d00 0000 7225 0000 0072 ae00 0000 72af  ....r%...r....r.
+0000dee0: 0000 0072 1301 0000 7287 0000 0072 2c02  ...r....r....r,.
+0000def0: 0000 723b 0000 0072 2300 0000 7297 0100  ..r;...r#...r...
+0000df00: 0072 3a00 0000 724e 0000 0072 2e02 0000  .r:...rN...r....
+0000df10: 720b 0000 0072 3001 0000 7226 0000 0072  r....r0...r&...r
+0000df20: 4e01 0000 5a11 6835 5f66 756c 6c5f 6669  N...Z.h5_full_fi
+0000df30: 6c65 5f6e 616d 6572 af01 0000 2913 72b1  le_namer....).r.
+0000df40: 0100 005a 0c61 6c6c 5f68 3573 5f69 6d67  ...Z.all_h5s_img
+0000df50: 7372 2f02 0000 da07 626f 7264 6572 735a  sr/.....bordersZ
+0000df60: 0c6d 6178 5f70 6163 6b5f 7661 6c72 4100  .max_pack_valrA.
+0000df70: 0000 7233 0000 0072 be00 0000 72c0 0000  ..r3...r....r...
+0000df80: 005a 0f6d 6178 5f68 756d 616e 5f6c 6162  .Z.max_human_lab
+0000df90: 656c 5a10 6d65 616e 5f68 756d 616e 5f6c  elZ.mean_human_l
+0000dfa0: 6162 656c 72fb 0000 0072 e601 0000 7272  abelr....r....rr
+0000dfb0: 0100 005a 0c70 6163 6b5f 6576 6572 795f  ...Z.pack_every_
+0000dfc0: 78da 086e 6577 5f69 6d67 735a 0a6e 6577  x..new_imgsZ.new
+0000dfd0: 5f6c 6162 656c 735a 0463 6e74 7272 9001  _labelsZ.cntrr..
+0000dfe0: 0000 7216 0000 0072 3202 0000 7217 0000  ..r....r2...r...
+0000dff0: 00da 1563 7265 6174 655f 6d61 7374 6572  ...create_master
+0000e000: 5f64 6174 6173 6574 7509 0000 7348 0000  _datasetu...sH..
+0000e010: 0000 1b04 0114 010e 010e 0110 010e 010e  ................
+0000e020: 010c 0112 010c 0108 0110 0222 0112 0102  ..........."....
+0000e030: ff06 020a 030a 010a 0104 010c 0108 0108  ................
+0000e040: 012e 0112 0220 0108 010a 010c 010a 010a  ..... ..........
+0000e050: 0108 0118 0210 0116 0172 3502 0000 6301  .........r5...c.
+0000e060: 0000 0000 0000 0000 0000 0006 0000 0007  ................
+0000e070: 0000 0043 0000 0073 7a00 0000 6401 6402  ...C...sz...d.d.
+0000e080: 8400 7c00 a000 6403 a101 6404 6405 8502  ..|...d...d.d...
+0000e090: 1900 4400 8301 7d01 7401 8300 7d02 6404  ..D...}.t...}.d.
+0000e0a0: 7c02 6406 3c00 6407 7c02 6408 3c00 6409  |.d.<.d.|.d.<.d.
+0000e0b0: 7c02 640a 3c00 6700 7d03 7c01 4400 5d32  |.d.<.g.}.|.D.]2
+0000e0c0: 7d04 7c04 a000 640b a101 640c 1900 7d05  }.|...d...d...}.
+0000e0d0: 7c03 a002 7403 7c04 a000 640b a101 640d  |...t.|...d...d.
+0000e0e0: 1900 8301 7c02 7c05 1900 1400 a101 0100  ....|.|.........
+0000e0f0: 7142 7c03 5300 290e 7589 0300 000a 2020  qB|.S.).u.....  
+0000e100: 4578 616d 706c 650a 2020 2d2d 2d2d 2d2d  Example.  ------
+0000e110: 2d0a 2020 696d 706f 7274 2072 650a 2020  -.  import re.  
+0000e120: 696d 706f 7274 206d 6174 706c 6f74 6c69  import matplotli
+0000e130: 622e 7079 706c 6f74 2061 7320 706c 740a  b.pyplot as plt.
+0000e140: 2020 666f 7220 6b20 696e 2072 616e 6765    for k in range
+0000e150: 2838 293a 0a20 2020 2053 203d 2027 7465  (8):.    S = 'te
+0000e160: 7374 2027 2a31 302a 2a6b 0a20 2020 2073  st '*10**k.    s
+0000e170: 3220 3d20 2774 6573 7427 0a20 2020 2025  2 = 'test'.    %
+0000e180: 7469 6d65 205b 6d2e 7374 6172 7428 2920  time [m.start() 
+0000e190: 666f 7220 6d20 696e 2072 652e 6669 6e64  for m in re.find
+0000e1a0: 6974 6572 2853 322c 2053 295d 0a0a 2020  iter(S2, S)]..  
+0000e1b0: 2320 7468 656e 2063 6f70 7920 6974 2069  # then copy it i
+0000e1c0: 6e74 6f20 6120 7374 7269 6e67 206c 696b  nto a string lik
+0000e1d0: 6520 6265 6c6f 770a 0a20 2074 7874 203d  e below..  txt =
+0000e1e0: 2027 2727 0a20 2043 5055 2074 696d 6573   '''.  CPU times
+0000e1f0: 3a20 7573 6572 2030 206e 732c 2073 7973  : user 0 ns, sys
+0000e200: 3a20 392e 3035 206d 732c 2074 6f74 616c  : 9.05 ms, total
+0000e210: 3a20 392e 3035 206d 730a 2020 5761 6c6c  : 9.05 ms.  Wall
+0000e220: 2074 696d 653a 2039 2e30 3120 6d73 0a20   time: 9.01 ms. 
+0000e230: 2043 5055 2074 696d 6573 3a20 7573 6572   CPU times: user
+0000e240: 2031 3220 c2b5 732c 2073 7973 3a20 3120   12 ..s, sys: 1 
+0000e250: c2b5 732c 2074 6f74 616c 3a20 3133 20c2  ..s, total: 13 .
+0000e260: b573 0a20 2057 616c 6c20 7469 6d65 3a20  .s.  Wall time: 
+0000e270: 3135 2e37 20c2 b573 0a20 2043 5055 2074  15.7 ..s.  CPU t
+0000e280: 696d 6573 3a20 7573 6572 2034 3820 c2b5  imes: user 48 ..
+0000e290: 732c 2073 7973 3a20 3320 c2b5 732c 2074  s, sys: 3 ..s, t
+0000e2a0: 6f74 616c 3a20 3531 20c2 b573 0a20 2057  otal: 51 ..s.  W
+0000e2b0: 616c 6c20 7469 6d65 3a20 3536 2e33 20c2  all time: 56.3 .
+0000e2c0: b573 0a20 2043 5055 2074 696d 6573 3a20  .s.  CPU times: 
+0000e2d0: 7573 6572 2032 3831 20c2 b573 2c20 7379  user 281 ..s, sy
+0000e2e0: 733a 2030 206e 732c 2074 6f74 616c 3a20  s: 0 ns, total: 
+0000e2f0: 3238 3120 c2b5 730a 2020 5761 6c6c 2074  281 ..s.  Wall t
+0000e300: 696d 653a 2032 3837 20c2 b573 0a20 2043  ime: 287 ..s.  C
+0000e310: 5055 2074 696d 6573 3a20 7573 6572 2032  PU times: user 2
+0000e320: 2e34 3220 6d73 2c20 7379 733a 2030 206e  .42 ms, sys: 0 n
+0000e330: 732c 2074 6f74 616c 3a20 322e 3432 206d  s, total: 2.42 m
+0000e340: 730a 2020 5761 6c6c 2074 696d 653a 2032  s.  Wall time: 2
+0000e350: 2e34 3320 6d73 0a20 2043 5055 2074 696d  .43 ms.  CPU tim
+0000e360: 6573 3a20 7573 6572 2032 312e 3820 6d73  es: user 21.8 ms
+0000e370: 2c20 7379 733a 2032 3220 c2b5 732c 2074  , sys: 22 ..s, t
+0000e380: 6f74 616c 3a20 3231 2e38 206d 730a 2020  otal: 21.8 ms.  
+0000e390: 5761 6c6c 2074 696d 653a 2032 312e 3220  Wall time: 21.2 
+0000e3a0: 6d73 0a20 2043 5055 2074 696d 6573 3a20  ms.  CPU times: 
+0000e3b0: 7573 6572 2031 3938 206d 732c 2073 7973  user 198 ms, sys
+0000e3c0: 3a20 3231 2e35 206d 732c 2074 6f74 616c  : 21.5 ms, total
+0000e3d0: 3a20 3231 3920 6d73 0a20 2057 616c 6c20  : 219 ms.  Wall 
+0000e3e0: 7469 6d65 3a20 3231 3420 6d73 0a20 2043  time: 214 ms.  C
+0000e3f0: 5055 2074 696d 6573 3a20 7573 6572 2031  PU times: user 1
+0000e400: 2e38 3320 732c 2073 7973 3a20 3139 3120  .83 s, sys: 191 
+0000e410: 6d73 2c20 746f 7461 6c3a 2032 2e30 3220  ms, total: 2.02 
+0000e420: 730a 2020 5761 6c6c 2074 696d 653a 2032  s.  Wall time: 2
+0000e430: 2e30 3220 730a 2020 2727 270a 2020 6461  .02 s.  '''.  da
+0000e440: 7461 203d 2067 6574 5f74 696d 655f 6974  ta = get_time_it
+0000e450: 2874 7874 290a 2020 6178 203d 2070 6c74  (txt).  ax = plt
+0000e460: 2e70 6c6f 7428 6461 7461 5b31 3a5d 290a  .plot(data[1:]).
+0000e470: 2020 706c 742e 7973 6361 6c65 2827 6c6f    plt.yscale('lo
+0000e480: 6727 290a 2020 6301 0000 0000 0000 0000  g').  c.........
+0000e490: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+0000e4a0: 1a00 0000 6700 7c00 5d12 7d01 7c01 a000  ....g.|.].}.|...
+0000e4b0: 6400 a101 6401 1900 9102 7104 5300 2902  d...d.....q.S.).
+0000e4c0: 728f 0100 0072 0100 0000 2901 72db 0000  r....r....).r...
+0000e4d0: 0072 3100 0000 7216 0000 0072 1600 0000  .r1...r....r....
+0000e4e0: 7217 0000 0072 3400 0000 dd09 0000 7304  r....r4.......s.
+0000e4f0: 0000 0006 0002 007a 1f67 6574 5f74 696d  .......z.get_tim
+0000e500: 655f 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c  e_it.<locals>.<l
+0000e510: 6973 7463 6f6d 703e 7a0b 5761 6c6c 2074  istcomp>z.Wall t
+0000e520: 696d 653a 2072 2e00 0000 4eda 0173 67fc  ime: r....N..sg.
+0000e530: a9f1 d24d 6250 3fda 026d 7367 8ded b5a0  ...MbP?..msg....
+0000e540: f7c6 b03e 7503 0000 00c2 b573 728b 0100  ...>u......sr...
+0000e550: 0072 4a00 0000 7201 0000 0029 0472 db00  .rJ...r....).r..
+0000e560: 0000 7269 0000 0072 2300 0000 7289 0000  ..ri...r#...r...
+0000e570: 0029 06da 0374 7874 da04 7661 7273 72e5  .)...txt..varsr.
+0000e580: 0000 0072 2a00 0000 7233 0000 00da 0575  ...r*...r3.....u
+0000e590: 6e69 7473 7216 0000 0072 1600 0000 7217  nitsr....r....r.
+0000e5a0: 0000 00da 0b67 6574 5f74 696d 655f 6974  .....get_time_it
+0000e5b0: ba09 0000 7314 0000 0000 231c 0106 0108  ....s.....#.....
+0000e5c0: 0108 0108 0104 0108 010e 0122 0172 3b02  ...........".r;.
+0000e5d0: 0000 6302 0000 0000 0000 0000 0000 0007  ..c.............
+0000e5e0: 0000 000a 0000 0043 0000 0073 1a01 0000  .......C...s....
+0000e5f0: 6700 7d02 7400 a001 7c00 6401 a102 8ff8  g.}.t...|.d.....
+0000e600: 7d03 7c03 a002 a100 4400 5d24 7d04 7c03  }.|.....D.]$}.|.
+0000e610: a003 7c04 a101 7234 7c02 a004 6402 a101  ..|...r4|...d...
+0000e620: 0100 711a 7c02 a004 6403 a101 0100 711a  ..q.|...d.....q.
+0000e630: 7405 7c02 8301 72fc 7406 6404 8301 0100  t.|...r.t.d.....
+0000e640: 7c00 6405 1700 7d05 7400 a001 7c00 6405  |.d...}.t...|.d.
+0000e650: 1700 6406 a102 8f62 7d06 7c03 a002 a100  ..d....b}.|.....
+0000e660: 4400 5d42 7d04 7c03 a003 7c04 a101 72a4  D.]B}.|...|...r.
+0000e670: 7406 6407 7c04 1700 6408 1700 8301 0100  t.d.|...d.......
+0000e680: 7c06 6a07 7c04 7c03 7c04 1900 6409 8d02  |.j.|.|.|...d...
+0000e690: 0100 7172 7406 640a 7c04 1700 640b 1700  ..qrt.d.|...d...
+0000e6a0: 8301 0100 7172 7c06 a008 a100 0100 7c03  ....qr|.......|.
+0000e6b0: a008 a100 0100 5700 3500 5100 5200 5800  ......W.5.Q.R.X.
+0000e6c0: 7c01 72fa 7406 640c 8301 0100 7409 a00a  |.r.t.d.....t...
+0000e6d0: 7c00 a101 0100 7406 640d 8301 0100 7409  |.....t.d.....t.
+0000e6e0: a00b 7c05 7c00 a102 0100 6e08 7406 640e  ..|.|.....n.t.d.
+0000e6f0: 8301 0100 5700 3500 5100 5200 5800 7406  ....W.5.Q.R.X.t.
+0000e700: 640f 8301 0100 6400 5300 2910 4e72 e500  d.....d.S.).Nr..
+0000e710: 0000 7201 0000 0072 2e00 0000 7a25 436f  ..r....r....z%Co
+0000e720: 7272 7570 7420 6669 6c65 2066 6f75 6e64  rrupt file found
+0000e730: 2c20 6372 6561 7469 6e67 206e 6577 2066  , creating new f
+0000e740: 696c 65da 0354 4d50 729d 0000 007a 0b41  ile..TMPr....z.A
+0000e750: 6464 696e 6720 6b65 7920 7a17 2074 6f20  dding key z. to 
+0000e760: 6e65 7720 7465 6d70 2048 3520 6669 6c65  new temp H5 file
+0000e770: 2e2e 2e72 0101 0000 7a07 2a2a 2a4b 6579  ...r....z.***Key
+0000e780: 207a 2220 7761 7320 636f 7272 7570 742c   z" was corrupt,
+0000e790: 2073 6b69 7070 696e 6720 7468 6973 206b   skipping this k
+0000e7a0: 6579 2e2e 2e7a 1844 656c 6574 696e 6720  ey...z.Deleting 
+0000e7b0: 636f 7272 7570 7420 4835 2066 696c 657a  corrupt H5 filez
+0000e7c0: 1572 656e 616d 696e 6720 6e65 7720 6835  .renaming new h5
+0000e7d0: 2066 696c 6520 7a14 4669 6c65 2069 7320   file z.File is 
+0000e7e0: 4e4f 5420 636f 7272 7570 7421 5a08 4649  NOT corrupt!Z.FI
+0000e7f0: 4e49 5348 4544 290c 72ae 0000 0072 af00  NISHED).r....r..
+0000e800: 0000 7299 0000 0072 c900 0000 7223 0000  ..r....r....r#..
+0000e810: 0072 8b00 0000 724b 0000 0072 af01 0000  .r....rK...r....
+0000e820: da05 636c 6f73 6572 5f00 0000 7279 0000  ..closer_...ry..
+0000e830: 00da 0672 656e 616d 6529 075a 0748 355f  ...rename).Z.H5_
+0000e840: 6669 6c65 5a11 646f 5f64 656c 5f61 6e64  fileZ.do_del_and
+0000e850: 5f72 656e 616d 655a 0774 7374 5f63 6f72  _renameZ.tst_cor
+0000e860: 72dd 0100 0072 3300 0000 5a0a 4835 5f66  r....r3...Z.H5_f
+0000e870: 696c 6554 4d50 5a03 6866 3272 1600 0000  ileTMPZ.hf2r....
+0000e880: 7216 0000 0072 1700 0000 da21 7361 7665  r....r.....!save
+0000e890: 5f77 6861 745f 6973 5f6c 6566 745f 6f66  _what_is_left_of
+0000e8a0: 5f79 6f75 725f 6835 5f66 696c 65e9 0900  _your_h5_file...
+0000e8b0: 0073 3000 0000 0001 0401 0e01 0c01 0a01  .s0.............
+0000e8c0: 0c02 0c01 0801 0801 0801 1201 0c01 0a01  ................
+0000e8d0: 1001 1402 1201 0801 1201 0401 0801 0a01  ................
+0000e8e0: 0801 0e02 1201 723f 0200 0063 0400 0000  ......r?...c....
+0000e8f0: 0000 0000 0000 0000 0c00 0000 0900 0000  ................
+0000e900: 4300 0000 73e2 0000 0074 006a 017c 0164  C...s....t.j.|.d
+0000e910: 0164 028d 027d 0474 02a0 037c 0064 03a1  .d...}.t...|.d..
+0000e920: 028f a27d 057c 0564 0419 0064 0564 0585  ...}.|.d...d.d..
+0000e930: 0219 007d 0674 0474 0574 067c 0683 0174  ...}.t.t.t.|...t
+0000e940: 077c 0683 0164 068d 0283 0144 005d 725c  .|...d.....D.]r\
+0000e950: 027d 075c 027d 087d 097c 0564 0719 007c  .}.\.}.}.|.d...|
+0000e960: 087c 0985 0219 007d 0a74 077c 0a6a 0883  .|.....}.t.|.j..
+0000e970: 0164 086b 0272 8a7c 0a64 0564 0585 0264  .d.k.r.|.d.d...d
+0000e980: 0564 0585 0264 0564 0585 0264 0966 0419  .d...d.d...d.f..
+0000e990: 007d 0a74 006a 097c 0a64 0a64 0964 0b8d  .}.t.j.|.d.d.d..
+0000e9a0: 037d 0b7c 04a0 0a7c 0b74 0ba0 0c7c 0b6a  .}.|...|.t...|.j
+0000e9b0: 0864 0919 00a1 0164 0c14 00a1 0201 0071  .d.....d.......q
+0000e9c0: 4457 0035 0051 0052 0058 0074 0d7c 007c  DW.5.Q.R.X.t.|.|
+0000e9d0: 0164 0d64 0d83 0401 0074 0d7c 007c 0164  .d.d.....t.|.|.d
+0000e9e0: 0464 0483 0401 0064 0553 0029 0e7a e10a  .d.....d.S.).z..
+0000e9f0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0000ea00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000ea10: 2020 2066 203a 2068 3520 6669 6c65 2077     f : h5 file w
+0000ea20: 6974 6820 5349 4e47 4c45 2046 5241 4d45  ith SINGLE FRAME
+0000ea30: 5320 7468 6973 2069 7320 6d65 616e 7420  S this is meant 
+0000ea40: 746f 2062 6520 6120 7465 7374 2070 726f  to be a test pro
+0000ea50: 6772 616d 2e20 6966 2075 7365 6420 6c6f  gram. if used lo
+0000ea60: 6e67 2074 6572 6d20 4920 7769 6c6c 2063  ng term I will c
+0000ea70: 6861 6e67 6520 7468 6973 2070 6172 740a  hange this part.
+0000ea80: 2020 2020 6632 203a 0a20 2020 2062 7566      f2 :.    buf
+0000ea90: 6665 7220 3a0a 2020 2020 7368 6966 745f  fer :.    shift_
+0000eaa0: 746f 5f74 6865 5f72 6967 6874 5f62 7920  to_the_right_by 
+0000eab0: 3a0a 0a20 2020 2052 6574 7572 6e73 0a20  :..    Returns. 
+0000eac0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
+0000ead0: 54a9 0172 3a01 0000 726d 0000 0072 4100  T..r:...rm...rA.
+0000eae0: 0000 4e72 4601 0000 729a 0000 0072 d900  ..NrF...r....r..
+0000eaf0: 0000 7201 0000 0072 4700 0000 a902 da06  ..r....rG.......
+0000eb00: 6275 6666 6572 da15 7368 6966 745f 746f  buffer..shift_to
+0000eb10: 5f74 6865 5f72 6967 6874 5f62 7972 4a00  _the_right_byrJ.
+0000eb20: 0000 7252 0000 0029 0e72 0800 0000 7248  ..rR...).r....rH
+0000eb30: 0100 0072 ae00 0000 72af 0000 0072 2400  ...r....r....r$.
+0000eb40: 0000 720b 0000 0072 3700 0000 7230 0000  ..r....r7...r0..
+0000eb50: 0072 2100 0000 5a0e 7374 6163 6b5f 696d  .r!...Z.stack_im
+0000eb60: 6773 5f6c 6167 724e 0100 0072 1d00 0000  gs_lagrN...r....
+0000eb70: 7236 0000 0072 d001 0000 290c 72a5 0100  r6...r....).r...
+0000eb80: 00da 0266 3272 4202 0000 7243 0200 0072  ...f2rB...rC...r
+0000eb90: b101 0000 72c0 0000 0072 5300 0000 723e  ....r....rS...r>
+0000eba0: 0000 0072 bd00 0000 72be 0000 00da 0278  ...r....r......x
+0000ebb0: 3272 3402 0000 7216 0000 0072 1600 0000  2r4...r....r....
+0000ebc0: 7217 0000 00da 1273 7461 636b 5f6c 6167  r......stack_lag
+0000ebd0: 5f68 355f 6d61 6b65 7207 0a00 0073 1600  _h5_maker....s..
+0000ebe0: 0000 000e 0e01 0e01 1001 2401 1001 0e01  ..........$.....
+0000ebf0: 1c01 1001 2803 0e01 7246 0200 0063 0100  ....(...rF...c..
+0000ec00: 0000 0000 0000 0000 0000 0600 0000 0900  ................
+0000ec10: 0000 4300 0000 73be 0000 0074 00a0 017c  ..C...s....t...|
+0000ec20: 0064 01a1 028f a87d 0174 0274 037c 0164  .d.....}.t.t.|.d
+0000ec30: 0219 006a 0464 0319 0083 0183 0144 005d  ...j.d.......D.]
+0000ec40: 8a7d 0274 05a0 067c 0164 0219 007c 0219  .}.t...|.d...|..
+0000ec50: 00a1 017d 0374 0364 0483 0144 005d 6a7d  ...}.t.d...D.]j}
+0000ec60: 047c 03a0 0774 08a1 017d 037c 0364 0564  .|...t...}.|.d.d
+0000ec70: 0585 0264 0564 0585 027c 0466 0319 007c  ...d.d...|.f...|
+0000ec80: 0364 0564 0585 0264 0564 0585 0264 0666  .d.d...d.d...d.f
+0000ec90: 0319 0018 007d 057c 0564 0717 0064 041b  .....}.|.d...d..
+0000eca0: 00a0 0774 096a 0aa1 017d 057c 057c 0164  ...t.j...}.|.|.d
+0000ecb0: 0219 007c 0264 0564 0585 0264 0564 0585  ...|.d.d...d.d..
+0000ecc0: 027c 0466 043c 0071 4271 2457 0035 0051  .|.f.<.qBq$W.5.Q
+0000ecd0: 0052 0058 0064 0553 0029 0861 6701 0000  .R.X.d.S.).ag...
+0000ece0: 0a20 2020 206e 6565 6420 746f 2075 7365  .    need to use
+0000ecf0: 2074 6865 2073 7461 636b 5f6c 6167 5f68   the stack_lag_h
+0000ed00: 355f 6d61 6b65 7220 6669 7273 7420 616e  5_maker first an
+0000ed10: 6420 7468 656e 2073 656e 6420 6120 636f  d then send a co
+0000ed20: 7079 206f 6620 7468 6174 2069 6e74 6f20  py of that into 
+0000ed30: 7468 6973 206f 6e65 2061 6761 696e 2074  this one again t
+0000ed40: 6865 7365 2070 726f 6772 616d 2061 7265  hese program are
+0000ed50: 206f 6e6c 7920 6120 7465 6d70 0a20 2020   only a temp.   
+0000ed60: 2073 6f6c 7574 696f 6e2c 2069 6620 7765   solution, if we
+0000ed70: 2075 7365 2074 6865 7365 206d 6574 686f   use these metho
+0000ed80: 6473 2066 6f72 2074 6865 206d 6169 6e20  ds for the main 
+0000ed90: 6d6f 6465 6c20 7468 656e 2049 2077 696c  model then I wil
+0000eda0: 6c20 6d61 6b65 2075 7369 6e67 2074 6865  l make using the
+0000edb0: 6d20 6d6f 7265 2066 6c75 6964 2061 6e64  m more fluid and
+0000edc0: 206e 6f74 2064 6570 656e 6420 6f6e 206f   not depend on o
+0000edd0: 6e65 2061 6e6f 7468 6572 0a20 2020 2050  ne another.    P
+0000ede0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0000edf0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 3320  --------.    f3 
+0000ee00: 3a20 7468 6520 6669 6c65 2066 726f 6d20  : the file from 
+0000ee10: 7374 6163 6b5f 6c61 675f 6835 5f6d 616b  stack_lag_h5_mak
+0000ee20: 6572 206f 7574 7075 740a 0a20 2020 2052  er output..    R
+0000ee30: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0000ee40: 2d2d 0a20 2020 2072 a600 0000 729a 0000  --.    r....r...
+0000ee50: 0072 0100 0000 7247 0000 004e 724a 0000  .r....rG...NrJ..
+0000ee60: 00e9 ff00 0000 290b 72ae 0000 0072 af00  ......).r....r..
+0000ee70: 0000 720b 0000 0072 3a00 0000 7221 0000  ..r....r:...r!..
+0000ee80: 0072 1b00 0000 721c 0000 0072 8500 0000  .r....r....r....
+0000ee90: 7289 0000 0072 1d00 0000 722e 0100 0029  r....r....r....)
+0000eea0: 06da 0266 3372 c000 0000 722c 0000 0072  ...f3r....r,...r
+0000eeb0: 3300 0000 5a05 696d 675f 6972 e500 0000  3...Z.img_ir....
+0000eec0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+0000eed0: 1164 6966 665f 6c61 675f 6835 5f6d 616b  .diff_lag_h5_mak
+0000eee0: 6572 240a 0000 7310 0000 0000 0c0e 011a  er$...s.........
+0000eef0: 0112 010c 010a 012c 0114 0172 4902 0000  .......,...rI...
+0000ef00: 6302 0000 0000 0000 0000 0000 0009 0000  c...............
+0000ef10: 0009 0000 0043 0000 0073 ba00 0000 7400  .....C...s....t.
+0000ef20: 6a01 7c01 6401 6402 8d02 7d02 7402 a003  j.|.d.d...}.t...
+0000ef30: 7c00 6403 a102 8f8c 7d03 7c03 6404 1900  |.d.....}.|.d...
+0000ef40: 6400 6400 8502 1900 7d04 7404 7405 7406  d.d.....}.t.t.t.
+0000ef50: 7c04 8301 7407 7c04 8301 6405 8d02 8301  |...t.|...d.....
+0000ef60: 4400 5d5c 5c02 7d05 5c02 7d06 7d07 7c03  D.]\\.}.\.}.}.|.
+0000ef70: 6406 1900 7c06 7c07 8502 1900 7d08 7408  d...|.|.....}.t.
+0000ef80: a009 7c08 6400 6400 8502 6400 6400 8502  ..|.d.d...d.d...
+0000ef90: 6400 6400 8502 6400 6604 1900 6407 a102  d.d...d.f...d...
+0000efa0: 7d08 7c02 a00a 7c08 7408 a00b 7c08 6a0c  }.|...|.t...|.j.
+0000efb0: 6408 1900 a101 6409 1400 a102 0100 7144  d.....d.......qD
+0000efc0: 5700 3500 5100 5200 5800 740d 7c00 7c01  W.5.Q.R.X.t.|.|.
+0000efd0: 8302 0100 6400 5300 290a 4e54 7240 0200  ....d.S.).NTr@..
+0000efe0: 0072 6d00 0000 7241 0000 0072 4601 0000  .rm...rA...rF...
+0000eff0: 729a 0000 0072 4600 0000 7201 0000 0072  r....rF...r....r
+0000f000: 4a00 0000 290e 7208 0000 0072 4801 0000  J...).r....rH...
+0000f010: 72ae 0000 0072 af00 0000 7224 0000 0072  r....r....r$...r
+0000f020: 0b00 0000 7237 0000 0072 3000 0000 721d  ....r7...r0...r.
+0000f030: 0000 00da 0474 696c 6572 4e01 0000 7236  .....tilerN...r6
+0000f040: 0000 0072 2100 0000 729c 0100 00a9 0972  ...r!...r......r
+0000f050: a501 0000 7244 0200 0072 b101 0000 72c0  ....rD...r....r.
+0000f060: 0000 0072 5300 0000 723e 0000 0072 bd00  ...rS...r>...r..
+0000f070: 0000 72be 0000 0072 3402 0000 7216 0000  ..r....r4...r...
+0000f080: 0072 1600 0000 7217 0000 00da 2165 7870  .r....r.....!exp
+0000f090: 616e 645f 7369 6e67 6c65 5f66 7261 6d65  and_single_frame
+0000f0a0: 5f74 6f5f 335f 636f 6c6f 725f 6835 3a0a  _to_3_color_h5:.
+0000f0b0: 0000 7310 0000 0000 010e 010e 0110 0124  ..s............$
+0000f0c0: 0110 0124 0128 0372 4c02 0000 6302 0000  ...$.(.rL...c...
+0000f0d0: 0000 0000 0000 0000 0007 0000 000a 0000  ................
+0000f0e0: 0043 0000 0073 3c01 0000 7400 7c00 6401  .C...s<...t.|.d.
+0000f0f0: 6402 6403 8d03 7d02 7401 7c02 6404 6405  d.d...}.t.|.d.d.
+0000f100: 8d02 7d02 7401 7c02 6406 6405 8d02 7d02  ..}.t.|.d.d...}.
+0000f110: 7402 a003 7c00 6407 a102 8f64 7d03 7402  t...|.d....d}.t.
+0000f120: a003 7c01 6408 a102 8f4c 7d04 7c02 4400  ..|.d....L}.|.D.
+0000f130: 5d40 7d05 7a16 7c04 6a04 7c05 7c03 7c05  ]@}.z.|.j.|.|.|.
+0000f140: 1900 6409 8d02 0100 5700 7146 0100 0100  ..d.....W.qF....
+0000f150: 0100 7c04 7c05 3d00 7c04 6a04 7c05 7c03  ..|.|.=.|.j.|.|.
+0000f160: 7c05 1900 6409 8d02 0100 5900 7146 5800  |...d.....Y.qFX.
+0000f170: 7146 5700 3500 5100 5200 5800 5700 3500  qFW.5.Q.R.X.W.5.
+0000f180: 5100 5200 5800 640a 7c02 6b07 9001 7238  Q.R.X.d.|.k...r8
+0000f190: 640b 7c02 6b06 9001 7238 7405 a006 7c00  d.|.k...r8t...|.
+0000f1a0: 6701 640b a102 7d06 7402 a003 7c01 6408  g.d...}.t...|.d.
+0000f1b0: a102 8f68 7d03 7a24 7c03 6a04 640a 7c06  ...h}.z$|.j.d.|.
+0000f1c0: 640c 640d 640d 8502 6602 1900 a007 7408  d.d.d...f.....t.
+0000f1d0: a101 6409 8d02 0100 5700 6e3c 0100 0100  ..d.....W.n<....
+0000f1e0: 0100 7c03 640a 3d00 7409 a00a 640e a101  ..|.d.=.t...d...
+0000f1f0: 0100 7c03 6a04 640a 7c06 640c 640d 640d  ..|.j.d.|.d.d.d.
+0000f200: 8502 6602 1900 a007 7408 a101 6409 8d02  ..f.....t...d...
+0000f210: 0100 5900 6e02 5800 5700 3500 5100 5200  ..Y.n.X.W.5.Q.R.
+0000f220: 5800 640d 5300 290f 7a62 0a0a 2020 2020  X.d.S.).zb..    
+0000f230: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000f240: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6620  ---------.    f 
+0000f250: 3a20 736f 7572 6365 0a20 2020 2066 3220  : source.    f2 
+0000f260: 3a20 6465 7374 696e 6174 696f 6e0a 0a20  : destination.. 
+0000f270: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0000f280: 2d2d 2d2d 2d2d 0a0a 2020 2020 5446 a902  ------..    TF..
+0000f290: 72cc 0100 0072 cd01 0000 5a06 4d4f 4445  r....r....Z.MODE
+0000f2a0: 4c5f 2901 72d9 0100 0072 9a00 0000 726d  L_).r....r....rm
+0000f2b0: 0000 0072 a600 0000 7201 0100 0072 4100  ...r....r....rA.
+0000f2c0: 0000 72ad 0100 0072 2e00 0000 4e72 4700  ..r....r....NrG.
+0000f2d0: 0000 290b 72ab 0000 0072 da01 0000 72ae  ..).r....r....r.
+0000f2e0: 0000 0072 af00 0000 72af 0100 0072 0800  ...r....r....r..
+0000f2f0: 0000 722c 0100 0072 8500 0000 7288 0000  ..r,...r....r...
+0000f300: 0072 9a01 0000 72b2 0100 0029 0772 a501  .r....r....).r..
+0000f310: 0000 7244 0200 005a 076b 5f6e 616d 6573  ..rD...Z.k_names
+0000f320: 72c0 0000 0072 cf01 0000 da02 6b6e 5a04  r....r......knZ.
+0000f330: 746e 666e 7216 0000 0072 1600 0000 7217  tnfnr....r....r.
+0000f340: 0000 0072 9c01 0000 490a 0000 7328 0000  ...r....I...s(..
+0000f350: 0000 0c0e 010c 010c 010e 010e 0108 0102  ................
+0000f360: 0116 0106 0106 012e 0714 010e 010e 0102  ................
+0000f370: 0124 0106 0106 010a 0172 9c01 0000 6303  .$.......r....c.
+0000f380: 0000 0000 0000 0000 0000 0004 0000 0009  ................
+0000f390: 0000 0043 0000 0073 5000 0000 7400 a001  ...C...sP...t...
+0000f3a0: 7c00 6401 a102 8f3a 7d03 7a12 7c03 6a02  |.d....:}.z.|.j.
+0000f3b0: 7c02 7c01 6402 8d02 0100 5700 6e20 0100  |.|.d.....W.n ..
+0000f3c0: 0100 0100 7c03 7c02 3d00 7c03 6a02 7c02  ....|.|.=.|.j.|.
+0000f3d0: 7c01 6402 8d02 0100 5900 6e02 5800 5700  |.d.....Y.n.X.W.
+0000f3e0: 3500 5100 5200 5800 6400 5300 2903 4e72  5.Q.R.X.d.S.).Nr
+0000f3f0: a600 0000 7201 0100 0029 0372 ae00 0000  ....r....).r....
+0000f400: 72af 0000 0072 af01 0000 2904 72dc 0100  r....r....).r...
+0000f410: 0072 2a00 0000 5a09 6461 7461 5f6e 616d  .r*...Z.data_nam
+0000f420: 6572 c000 0000 7216 0000 0072 1600 0000  er....r....r....
+0000f430: 7217 0000 00da 1166 6f72 6365 5f77 7269  r......force_wri
+0000f440: 7465 5f74 6f5f 6835 710a 0000 730c 0000  te_to_h5q...s...
+0000f450: 0000 010e 0102 0112 0106 0106 0172 4f02  .............rO.
+0000f460: 0000 6302 0000 0000 0000 0000 0000 0009  ..c.............
+0000f470: 0000 0009 0000 0043 0000 0073 c200 0000  .......C...s....
+0000f480: 7400 6a01 7c01 6401 6402 6403 8d03 7d02  t.j.|.d.d.d...}.
+0000f490: 7402 a003 7c00 6404 a102 8f92 7d03 7a18  t...|.d.....}.z.
+0000f4a0: 7c03 6405 1900 6406 6400 6400 8502 6602  |.d...d.d.d...f.
+0000f4b0: 1900 7d04 5700 6e1c 0100 0100 0100 7c03  ..}.W.n.......|.
+0000f4c0: 6407 1900 6400 6400 8502 1900 7d04 5900  d...d.d.....}.Y.
+0000f4d0: 6e02 5800 7404 7405 7406 7c04 8301 7407  n.X.t.t.t.|...t.
+0000f4e0: 7c04 8301 6408 8d02 8301 4400 5d3c 5c02  |...d.....D.]<\.
+0000f4f0: 7d05 5c02 7d06 7d07 7c03 6409 1900 7c06  }.\.}.}.|.d...|.
+0000f500: 7c07 8502 1900 640a 1900 7d08 7c02 a008  |.....d...}.|...
+0000f510: 7c08 7409 a00a 7c08 6a0b 640b 1900 a101  |.t...|.j.d.....
+0000f520: 640c 1400 a102 0100 716c 5700 3500 5100  d.......qlW.5.Q.
+0000f530: 5200 5800 740c 7c00 7c01 8302 0100 6400  R.X.t.|.|.....d.
+0000f540: 5300 290d 4e54 4629 0272 3a01 0000 723e  S.).NTF).r:...r>
+0000f550: 0100 0072 6d00 0000 72ad 0100 0072 2e00  ...rm...r....r..
+0000f560: 0000 7241 0000 0072 4601 0000 729a 0000  ..rA...rF...r...
+0000f570: 0029 022e 724a 0000 0072 0100 0000 724a  .)..rJ...r....rJ
+0000f580: 0000 0029 0d72 0800 0000 7248 0100 0072  ...).r....rH...r
+0000f590: ae00 0000 72af 0000 0072 2400 0000 720b  ....r....r$...r.
+0000f5a0: 0000 0072 3700 0000 7230 0000 0072 4e01  ...r7...r0...rN.
+0000f5b0: 0000 721d 0000 0072 3600 0000 7221 0000  ..r....r6...r!..
+0000f5c0: 0072 9c01 0000 724b 0200 0072 1600 0000  .r....rK...r....
+0000f5d0: 7216 0000 0072 1700 0000 da21 7265 6475  r....r.....!redu
+0000f5e0: 6365 5f74 6f5f 7369 6e67 6c65 5f66 7261  ce_to_single_fra
+0000f5f0: 6d65 5f66 726f 6d5f 636f 6c6f 727a 0a00  me_from_colorz..
+0000f600: 0073 1400 0000 0001 1001 0e01 0201 1801  .s..............
+0000f610: 0601 1601 2401 1402 2803 7250 0200 0063  ....$...(.rP...c
+0000f620: 0100 0000 0000 0000 0000 0000 0800 0000  ................
+0000f630: 0700 0000 4300 0000 731e 0100 0064 0164  ....C...s....d.d
+0000f640: 0284 007d 0174 007c 0083 0144 0090 015d  ...}.t.|...D...]
+0000f650: 067d 027c 017c 0283 017d 0374 016a 02a0  .}.|.|...}.t.j..
+0000f660: 037c 02a1 0164 0064 0385 0219 0064 0417  .|...d.d.....d..
+0000f670: 007d 047c 0364 0517 0074 016a 0417 007d  .}.|.d...t.j...}
+0000f680: 0574 016a 02a0 057c 05a1 0173 5a74 01a0  .t.j...|...sZt..
+0000f690: 067c 05a1 0101 007c 057c 0417 007d 0674  .|.....|.|...}.t
+0000f6a0: 077c 027c 0683 0201 0074 016a 02a0 037c  .|.|.....t.j...|
+0000f6b0: 02a1 0164 0064 0385 0219 0064 0617 007d  ...d.d.....d...}
+0000f6c0: 047c 0364 0717 0074 016a 0417 007d 0574  .|.d...t.j...}.t
+0000f6d0: 016a 02a0 057c 05a1 0173 a874 01a0 067c  .j...|...s.t...|
+0000f6e0: 05a1 0101 007c 057c 0417 007d 0674 087c  .....|.|...}.t.|
+0000f6f0: 027c 0664 0864 0964 0a8d 0401 0074 016a  .|.d.d.d.....t.j
+0000f700: 02a0 037c 06a1 0164 0064 0385 0219 0064  ...|...d.d.....d
+0000f710: 0b17 007d 047c 0364 0c17 0074 016a 0417  ...}.|.d...t.j..
+0000f720: 007d 0574 016a 02a0 057c 05a1 0173 fc74  .}.t.j...|...s.t
+0000f730: 01a0 067c 05a1 0101 007c 057c 0417 007d  ...|.....|.|...}
+0000f740: 0774 09a0 0a7c 067c 07a1 0201 0074 0b7c  .t...|.|.....t.|
+0000f750: 0783 0101 0071 1064 0053 0029 0d4e 6301  .....q.d.S.).Nc.
+0000f760: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+0000f770: 0000 0053 0000 0073 2a00 0000 7400 7401  ...S...s*...t.t.
+0000f780: 7c00 8301 6a02 a003 a100 8301 7d01 7400  |...j.......}.t.
+0000f790: 7401 7c01 8301 6a02 a003 a100 8301 7404  t.|...j.......t.
+0000f7a0: 6a05 1700 5300 720d 0100 0029 0672 ad00  j...S.r....).r..
+0000f7b0: 0000 720e 0000 0072 0602 0000 da08 6162  ..r....r......ab
+0000f7c0: 736f 6c75 7465 725f 0000 0072 6000 0000  soluter_...r`...
+0000f7d0: 2902 72a5 0100 0072 fb00 0000 7216 0000  ).r....r....r...
+0000f7e0: 0072 1600 0000 7217 0000 00da 0b6c 6173  .r....r......las
+0000f7f0: 745f 666f 6c64 6572 8d0a 0000 7304 0000  t_folder....s...
+0000f800: 0000 0112 017a 266d 616b 655f 616c 6c5f  .....z&make_all_
+0000f810: 4835 5f74 7970 6573 2e3c 6c6f 6361 6c73  H5_types.<locals
+0000f820: 3e2e 6c61 7374 5f66 6f6c 6465 7272 9500  >.last_folderr..
+0000f830: 0000 7a0b 5f72 6567 756c 6172 2e68 35da  ..z._regular.h5.
+0000f840: 0772 6567 756c 6172 72a5 0000 005a 0433  .regularr....Z.3
+0000f850: 6c61 6772 4700 0000 7201 0000 0072 4102  lagrG...r....rA.
+0000f860: 0000 7a08 5f64 6966 662e 6835 5a09 336c  ..z._diff.h5Z.3l
+0000f870: 6167 5f64 6966 6629 0c72 2901 0000 725f  ag_diff).r)...r_
+0000f880: 0000 0072 6100 0000 72a8 0000 0072 6000  ...ra...r....r`.
+0000f890: 0000 7262 0000 0072 6301 0000 724c 0200  ..rb...rc...rL..
+0000f8a0: 0072 4602 0000 7273 0000 0072 1b00 0000  .rF...rs...r....
+0000f8b0: 7249 0200 0029 08da 1062 6173 655f 6469  rI...)...base_di
+0000f8c0: 725f 616c 6c5f 6835 7372 5202 0000 72a5  r_all_h5srR...r.
+0000f8d0: 0100 005a 0662 6173 655f 6672 a800 0000  ...Z.base_fr....
+0000f8e0: da07 6261 7365 6469 7272 4402 0000 7248  ..basedirrD...rH
+0000f8f0: 0200 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+0000f900: 0000 da11 6d61 6b65 5f61 6c6c 5f48 355f  ....make_all_H5_
+0000f910: 7479 7065 738c 0a00 0073 2c00 0000 0001  types....s,.....
+0000f920: 0804 0e01 0801 1801 0e01 0c01 0a01 0801  ................
+0000f930: 0a02 1801 0e01 0c01 0a01 0802 1002 1801  ................
+0000f940: 0e01 0c01 0a01 0801 0c01 7256 0200 0063  ..........rV...c
+0000f950: 0100 0000 0000 0000 0000 0000 1000 0000  ................
+0000f960: 0700 0000 4300 0000 73a4 0100 0067 007d  ....C...s....g.}
+0000f970: 0174 00a0 017c 00a1 017d 027c 01a0 027c  .t...|...}.|...|
+0000f980: 02a1 0101 0074 037c 0283 017d 037c 01a0  .....t.|...}.|..
+0000f990: 027c 03a1 0101 0074 00a0 017c 03a1 017d  .|.....t...|...}
+0000f9a0: 0464 017c 047c 0464 026b 033c 0064 037c  .d.|.|.d.k.<.d.|
+0000f9b0: 047c 0464 026b 023c 007c 01a0 027c 04a1  .|.d.k.<.|...|..
+0000f9c0: 0101 0074 00a0 017c 03a1 017d 0564 017c  ...t...|...}.d.|
+0000f9d0: 057c 0564 046b 033c 0064 037c 057c 0564  .|.d.k.<.d.|.|.d
+0000f9e0: 046b 023c 007c 01a0 027c 05a1 0101 0074  .k.<.|...|.....t
+0000f9f0: 00a0 017c 03a1 017d 0664 017c 067c 0664  ...|...}.d.|.|.d
+0000fa00: 036b 023c 0064 037c 067c 0664 026b 023c  .k.<.d.|.|.d.k.<
+0000fa10: 0064 027c 067c 0664 046b 023c 007c 01a0  .d.|.|.d.k.<.|..
+0000fa20: 027c 06a1 0101 0074 00a0 017c 03a1 017d  .|.....t...|...}
+0000fa30: 077c 0764 0064 0585 0219 0064 026b 027d  .|.d.d.....d.k.}
+0000fa40: 0874 04a0 0264 067c 08a1 027d 097c 0764  .t...d.|...}.|.d
+0000fa50: 0064 0585 0219 0064 046b 027d 0a74 04a0  .d.....d.k.}.t..
+0000fa60: 0264 067c 0aa1 027d 0b7c 0764 046b 027d  .d.|...}.|.d.k.}
+0000fa70: 0a64 047c 077c 093c 0064 077c 077c 0a3c  .d.|.|.<.d.|.|.<
+0000fa80: 0064 087c 077c 0b3c 007c 01a0 027c 07a1  .d.|.|.<.|...|..
+0000fa90: 0101 0074 00a0 017c 07a1 017d 0c64 017c  ...t...|...}.d.|
+0000faa0: 0c7c 0c64 026b 023c 0064 017c 0c7c 0c64  .|.d.k.<.d.|.|.d
+0000fab0: 086b 023c 0064 027c 0c7c 0c64 046b 023c  .k.<.d.|.|.d.k.<
+0000fac0: 0064 047c 0c7c 0c64 076b 023c 007c 01a0  .d.|.|.d.k.<.|..
+0000fad0: 027c 0ca1 0101 0064 0864 0364 0764 0164  .|.....d.d.d.d.d
+0000fae0: 0464 0264 0967 077d 0d67 007d 0e7c 0d44  .d.d.g.}.g.}.|.D
+0000faf0: 005d 147d 0f7c 0ea0 027c 017c 0f19 00a1  .].}.|...|.|....
+0000fb00: 0101 0090 0171 8474 04a0 057c 0ea1 0153  .....q.t...|...S
+0000fb10: 0029 0a4e 7201 0000 0072 4700 0000 722e  .).Nr....rG...r.
+0000fb20: 0000 0072 4600 0000 724a 0000 0046 72d9  ...rF...rJ...Fr.
+0000fb30: 0000 0072 9b00 0000 e906 0000 0029 0672  ...r.........).r
+0000fb40: 1b00 0000 721c 0000 0072 2300 0000 72ca  ....r....r#...r.
+0000fb50: 0100 0072 1d00 0000 7238 0000 0029 1072  ...r....r8...).r
+0000fb60: 2e02 0000 da0a 616c 6c5f 6c61 6265 6c73  ......all_labels
+0000fb70: da02 7831 7245 0200 00da 0278 33da 0278  ..x1rE.....x3..x
+0000fb80: 34da 0278 35da 0278 36da 0a6f 6e73 6574  4..x5..x6..onset
+0000fb90: 5f69 6e64 73da 1962 6f6f 6c5f 696e 6473  _inds..bool_inds
+0000fba0: 5f6f 6e65 5f61 6674 6572 5f6f 6e73 6574  _one_after_onset
+0000fbb0: da0b 6f66 6673 6574 5f69 6e64 73da 1a62  ..offset_inds..b
+0000fbc0: 6f6f 6c5f 696e 6473 5f6f 6e65 5f61 6674  ool_inds_one_aft
+0000fbd0: 6572 5f6f 6666 7365 74da 0278 375a 0672  er_offset..x7Z.r
+0000fbe0: 6573 6f72 745a 0761 5f66 696e 616c 722c  esortZ.a_finalr,
+0000fbf0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+0000fc00: 0000 da1e 6765 745f 616c 6c5f 6c61 6265  ....get_all_labe
+0000fc10: 6c5f 7479 7065 735f 6672 6f6d 5f61 7272  l_types_from_arr
+0000fc20: 6179 ab0a 0000 734e 0000 0000 0104 010a  ay....sN........
+0000fc30: 010a 0208 010a 020a 010c 010c 010a 020a  ................
+0000fc40: 010c 010c 010a 020a 010c 010c 010c 010a  ................
+0000fc50: 020a 0110 010c 0110 010c 0108 0108 0108  ................
+0000fc60: 0108 010a 020a 010c 010c 010c 010c 010a  ................
+0000fc70: 0212 0204 0108 0112 0272 6302 0000 6301  .........rc...c.
+0000fc80: 0000 0000 0000 0000 0000 0011 0000 000a  ................
+0000fc90: 0000 0043 0000 0073 6e02 0000 7400 7c00  ...C...sn...t.|.
+0000fca0: 8301 4400 9002 5d5e 7d01 6401 a001 7402  ..D...]^}.d...t.
+0000fcb0: 6a03 a004 7c01 a101 a005 6402 a101 a101  j...|.....d.....
+0000fcc0: 7d02 7402 6a06 a001 7c01 a005 7402 6a06  }.t.j...|...t.j.
+0000fcd0: a101 6400 6403 8502 1900 a101 7402 6a06  ..d.d.......t.j.
+0000fce0: 1700 6404 1700 7402 6a06 1700 7d03 7402  ..d...t.j...}.t.
+0000fcf0: 6a03 a007 7c03 a101 7368 7402 a008 7c03  j...|...sht...|.
+0000fd00: a101 0100 7c03 7c02 1700 7d04 7409 a00a  ....|.|...}.t...
+0000fd10: 7c01 6405 a102 9001 8f32 7d05 740b a00c  |.d......2}.t...
+0000fd20: 7c05 6406 1900 6400 6400 8502 1900 a101  |.d...d.d.......
+0000fd30: 7d06 740d 7c06 8301 7d07 740b a00c 7c07  }.t.|...}.t...|.
+0000fd40: a101 7d08 6407 7c08 7c08 6408 6b03 3c00  ..}.d.|.|.d.k.<.
+0000fd50: 6409 7c08 7c08 6408 6b02 3c00 740b a00c  d.|.|.d.k.<.t...
+0000fd60: 7c07 a101 7d09 6407 7c09 7c09 640a 6b03  |...}.d.|.|.d.k.
+0000fd70: 3c00 6409 7c09 7c09 640a 6b02 3c00 740b  <.d.|.|.d.k.<.t.
+0000fd80: a00c 7c07 a101 7d0a 6407 7c0a 7c0a 6409  ..|...}.d.|.|.d.
+0000fd90: 6b02 3c00 6409 7c0a 7c0a 6408 6b02 3c00  k.<.d.|.|.d.k.<.
+0000fda0: 6408 7c0a 7c0a 640a 6b02 3c00 740b a00c  d.|.|.d.k.<.t...
+0000fdb0: 7c07 a101 7d0b 7c0b 6400 640b 8502 1900  |...}.|.d.d.....
+0000fdc0: 6408 6b02 7d0c 740e a00f 640c 7c0c a102  d.k.}.t...d.|...
+0000fdd0: 7d0d 7c0b 6400 640b 8502 1900 640a 6b02  }.|.d.d.....d.k.
+0000fde0: 7d0e 740e a00f 640c 7c0e a102 7d0f 7c0b  }.t...d.|...}.|.
+0000fdf0: 640a 6b02 7d0e 640a 7c0b 7c0d 3c00 640d  d.k.}.d.|.|.<.d.
+0000fe00: 7c0b 7c0e 3c00 640e 7c0b 7c0f 3c00 740b  |.|.<.d.|.|.<.t.
+0000fe10: a00c 7c0b a101 7d10 6407 7c10 7c10 6408  ..|...}.d.|.|.d.
+0000fe20: 6b02 3c00 6407 7c10 7c10 640e 6b02 3c00  k.<.d.|.|.d.k.<.
+0000fe30: 6408 7c10 7c10 640a 6b02 3c00 640a 7c10  d.|.|.d.k.<.d.|.
+0000fe40: 7c10 640d 6b02 3c00 5700 3500 5100 5200  |.d.k.<.W.5.Q.R.
+0000fe50: 5800 7409 a00a 7c04 640f a102 8fa0 7d05  X.t...|.d.....}.
+0000fe60: 7c05 6a10 6410 740e a011 7c06 a101 7c06  |.j.d.t...|...|.
+0000fe70: 6411 8d03 0100 7c05 6a10 6412 740e a011  d.....|.j.d.t...
+0000fe80: 7c07 a101 7c07 6411 8d03 0100 7c05 6a10  |...|.d.....|.j.
+0000fe90: 6413 740e a011 7c08 a101 7c08 6411 8d03  d.t...|...|.d...
+0000fea0: 0100 7c05 6a10 6414 740e a011 7c09 a101  ..|.j.d.t...|...
+0000feb0: 7c09 6411 8d03 0100 7c05 6a10 6415 740e  |.d.....|.j.d.t.
+0000fec0: a011 7c0a a101 7c0a 6411 8d03 0100 7c05  ..|...|.d.....|.
+0000fed0: 6a10 6416 740e a011 7c0b a101 7c0b 6411  j.d.t...|...|.d.
+0000fee0: 8d03 0100 7c05 6a10 6417 740e a011 7c10  ....|.j.d.t...|.
+0000fef0: a101 7c10 6411 8d03 0100 5700 3500 5100  ..|.d.....W.5.Q.
+0000ff00: 5200 5800 7108 6400 5300 2918 4e7a 0c5f  R.X.q.d.S.).Nz._
+0000ff10: 414c 545f 4c41 4245 4c53 2e72 2101 0000  ALT_LABELS.r!...
+0000ff20: 72e9 0100 00da 0a41 4c54 5f4c 4142 454c  r......ALT_LABEL
+0000ff30: 5372 6d00 0000 7252 0000 0072 0100 0000  Srm...rR...r....
+0000ff40: 7247 0000 0072 2e00 0000 7246 0000 0072  rG...r....rF...r
+0000ff50: 4a00 0000 4672 d900 0000 729b 0000 0072  J...Fr....r....r
+0000ff60: 9d00 0000 7a19 5b30 2c20 315d 2d20 286e  ....z.[0, 1]- (n
+0000ff70: 6f20 746f 7563 682c 2074 6f75 6368 2972  o touch, touch)r
+0000ff80: ce01 0000 7a2d 5b30 2c20 312c 2032 2c20  ....z-[0, 1, 2, 
+0000ff90: 335d 2d20 286e 6f20 746f 7563 682c 2074  3]- (no touch, t
+0000ffa0: 6f75 6368 2c20 6f6e 7365 742c 206f 6666  ouch, onset, off
+0000ffb0: 7365 747a 1a5b 302c 2031 5d2d 2028 6e6f  setz.[0, 1]- (no
+0000ffc0: 7420 6f6e 7365 742c 206f 6e73 6574 297a  t onset, onset)z
+0000ffd0: 1c5b 302c 2031 5d2d 2028 6e6f 7420 6f66  .[0, 1]- (not of
+0000ffe0: 6673 6574 2c20 6f66 6673 6574 297a 245b  fset, offset)z$[
+0000fff0: 302c 2031 2c20 325d 2d20 286e 6f20 6576  0, 1, 2]- (no ev
+00010000: 656e 742c 206f 6e73 6574 2c20 6f66 6673  ent, onset, offs
+00010010: 6574 297a 575b 302c 2031 2c20 322c 2033  et)zW[0, 1, 2, 3
+00010020: 2c20 342c 2035 5d2d 2028 6e6f 2074 6f75  , 4, 5]- (no tou
+00010030: 6368 2c20 746f 7563 682c 206f 6e73 6574  ch, touch, onset
+00010040: 2c20 6f6e 6520 6166 7465 7220 6f6e 7365  , one after onse
+00010050: 742c 206f 6666 7365 742c 206f 6e65 2061  t, offset, one a
+00010060: 6674 6572 206f 6666 7365 7429 7a38 5b30  fter offset)z8[0
+00010070: 2c20 312c 2032 2c20 335d 2d20 286e 6f20  , 1, 2, 3]- (no 
+00010080: 746f 7563 682c 2074 6f75 6368 2c20 6f6e  touch, touch, on
+00010090: 6520 6166 7465 7220 6f6e 7365 742c 206f  e after onset, o
+000100a0: 6666 7365 7429 2912 7229 0100 0072 da00  ffset)).r)...r..
+000100b0: 0000 725f 0000 0072 6100 0000 72a8 0000  ..r_...ra...r...
+000100c0: 0072 db00 0000 7260 0000 0072 6200 0000  .r....r`...rb...
+000100d0: 7263 0100 0072 ae00 0000 72af 0000 0072  rc...r....r....r
+000100e0: 1b00 0000 721c 0000 0072 ca01 0000 721d  ....r....r....r.
+000100f0: 0000 0072 2300 0000 72af 0100 0072 2100  ...r#...r....r!.
+00010100: 0000 2911 7254 0200 0072 a501 0000 72a8  ..).rT...r....r.
+00010110: 0000 0072 5502 0000 72bb 0000 0072 c000  ...rU...r....r..
+00010120: 0000 7259 0200 0072 4502 0000 725a 0200  ..rY...rE...rZ..
+00010130: 0072 5b02 0000 725c 0200 0072 5d02 0000  .r[...r\...r]...
+00010140: 725e 0200 0072 5f02 0000 7260 0200 0072  r^...r_...r`...r
+00010150: 6102 0000 7262 0200 0072 1600 0000 7216  a...rb...r....r.
+00010160: 0000 0072 1700 0000 da13 6d61 6b65 5f61  ...r......make_a
+00010170: 6c74 5f6c 6162 656c 735f 6835 73de 0a00  lt_labels_h5s...
+00010180: 0073 5800 0000 0001 0e01 1801 2c01 0c01  .sX.........,...
+00010190: 0a01 0802 1002 1602 0802 0a01 0c01 0c02  ................
+000101a0: 0a01 0c01 0c02 0a01 0c01 0c01 0c02 0a01  ................
+000101b0: 1001 0c01 1001 0c01 0801 0801 0801 0802  ................
+000101c0: 0a01 0c01 0c01 0c01 1602 0e01 1601 1601  ................
+000101d0: 1601 1601 1601 0601 0800 02ff 0602 7265  ..............re
+000101e0: 0200 0063 0100 0000 0000 0000 0000 0000  ...c............
+000101f0: 0100 0000 0400 0000 4300 0000 7316 0000  ........C...s...
+00010200: 0074 0074 017c 0064 0119 0083 016a 027c  .t.t.|.d.....j.|
+00010210: 008e 0083 0153 0072 1900 0000 2903 7239  .....S.r....).r9
+00010220: 0000 0072 dd00 0000 da0c 696e 7465 7273  ...r......inters
+00010230: 6563 7469 6f6e 726a 0000 0072 1600 0000  ectionrj...r....
+00010240: 7216 0000 0072 1700 0000 da0f 696e 7465  r....r......inte
+00010250: 7273 6563 745f 6c69 7374 7314 0b00 0073  rsect_lists....s
+00010260: 0200 0000 0001 7267 0200 00e9 c800 0000  ......rg........
+00010270: 6305 0000 0000 0000 0000 0000 0010 0000  c...............
+00010280: 000a 0000 0043 0000 0073 e000 0000 6700  .....C...s....g.
+00010290: 7d05 7c00 4400 5dca 7d06 7400 a001 7c06  }.|.D.].}.t...|.
+000102a0: 6401 a102 8fb4 7d07 7402 a003 7c07 6402  d.....}.t...|.d.
+000102b0: 1900 6400 6400 8502 1900 a101 7d08 7c07  ..d.d.......}.|.
+000102c0: 6403 1900 6404 6400 6400 8502 6602 1900  d...d.d.d...f...
+000102d0: 7d09 7404 7405 7c09 8301 8301 4400 5d54  }.t.t.|.....D.]T
+000102e0: 5c02 7d0a 5c02 7d0b 7d0c 7c07 6405 1900  \.}.\.}.}.|.d...
+000102f0: 6400 6400 8502 7c0a 6602 1900 7c0b 1700  d.d...|.f...|...
+00010300: 7d0d 7c0d 6406 1900 7c01 1700 7d0e 7c0d  }.|.d...|...}.|.
+00010310: 6404 1900 7c02 1700 7d0f 7406 7c0f 7c0c  d...|...}.t.|.|.
+00010320: 6702 8301 7d0f 6404 7c08 7c0e 7c0f 8502  g...}.d.|.|.|...
+00010330: 3c00 7150 7c03 72ba 7c08 7c07 6402 1900  <.qP|.r.|.|.d...
+00010340: 6400 6400 8502 3c00 7c04 72c8 7c05 a007  d.d...<.|.r.|...
+00010350: 7c08 a101 0100 5700 3500 5100 5200 5800  |.....W.5.Q.R.X.
+00010360: 7108 7c04 72dc 7c05 5300 6400 5300 2907  q.|.r.|.S.d.S.).
+00010370: 4e72 a600 0000 72ab 0100 0072 ad01 0000  Nr....r....r....
+00010380: 722e 0000 00da 0a70 6f6c 655f 7469 6d65  r......pole_time
+00010390: 7372 0100 0000 2908 72ae 0000 0072 af00  sr....).r....r..
+000103a0: 0000 721d 0000 0072 8400 0000 7224 0000  ..r....r....r$..
+000103b0: 0072 3700 0000 da03 6d69 6e72 2300 0000  .r7.....minr#...
+000103c0: 2910 5a07 4835 5f6c 6973 745a 0b70 6f6c  ).Z.H5_listZ.pol
+000103d0: 655f 7570 5f61 6464 5a0d 706f 6c65 5f64  e_up_addZ.pole_d
+000103e0: 6f77 6e5f 6164 6472 6f01 0000 da0f 7265  own_addro.....re
+000103f0: 7475 726e 5f69 6e5f 7261 6e67 655a 0c61  turn_in_rangeZ.a
+00010400: 6c6c 5f69 6e5f 7261 6e67 6572 3300 0000  ll_in_ranger3...
+00010410: 72dd 0100 00da 0c6e 6577 5f69 6e5f 7261  r......new_in_ra
+00010420: 6e67 6572 4f01 0000 722c 0000 0072 3f00  ngerO...r,...r?.
+00010430: 0000 7240 0000 0072 5300 0000 7259 0200  ..r@...rS...rY..
+00010440: 0072 4502 0000 7216 0000 0072 1600 0000  .rE...r....r....
+00010450: 7217 0000 00da 0c67 6574 5f69 6e5f 7261  r......get_in_ra
+00010460: 6e67 6518 0b00 0073 2200 0000 0001 0401  nge....s".......
+00010470: 0801 0e01 1601 1401 1801 1801 0c01 0c01  ................
+00010480: 0c01 0e01 0401 1001 0401 1601 0401 726d  ..............rm
+00010490: 0200 0063 0100 0000 0000 0000 0000 0000  ...c............
+000104a0: 0300 0000 0900 0000 4300 0000 7368 0000  ........C...sh..
+000104b0: 0074 00a0 017c 0064 01a1 028f 527d 0164  .t...|.d....R}.d
+000104c0: 027c 01a0 02a1 006b 0672 2c7c 0164 0219  .|.....k.r,|.d..
+000104d0: 0064 0064 0085 0219 007d 026e 2e64 037c  .d.d.....}.n.d.|
+000104e0: 01a0 02a1 006b 0672 4e7c 0164 0319 0064  .....k.rN|.d...d
+000104f0: 0464 0064 0085 0266 0219 007d 026e 0c64  .d.d...f...}.n.d
+00010500: 0573 5a74 0364 0683 0182 0157 0035 0051  .sZt.d.....W.5.Q
+00010510: 0052 0058 007c 0253 0029 074e 72a6 0000  .R.X.|.S.).Nr...
+00010520: 0072 4100 0000 72ad 0100 0072 2e00 0000  .rA...r....r....
+00010530: 467a 4a68 3520 6669 6c65 2070 726f 7669  FzJh5 file provi
+00010540: 6465 6420 646f 6573 206e 6f74 2068 6176  ded does not hav
+00010550: 6520 2766 7261 6d65 5f6e 756d 7327 206f  e 'frame_nums' o
+00010560: 7220 2774 7269 616c 5f6e 756d 735f 616e  r 'trial_nums_an
+00010570: 645f 6672 616d 655f 6e75 6d73 2729 0472  d_frame_nums').r
+00010580: ae00 0000 72af 0000 0072 9900 0000 724e  ....r....r....rN
+00010590: 0000 0029 0372 dc01 0000 72dd 0100 0072  ...).r....r....r
+000105a0: 4f01 0000 7216 0000 0072 1600 0000 7217  O...r....r....r.
+000105b0: 0000 00da 0e67 6574 5f66 7261 6d65 5f6e  .....get_frame_n
+000105c0: 756d 732c 0b00 0073 0e00 0000 0001 0e01  ums,...s........
+000105d0: 0c01 1201 0c01 1602 1601 726e 0200 0063  ..........rn...c
+000105e0: 0600 0000 0000 0000 0000 0000 0f00 0000  ................
+000105f0: 0900 0000 4300 0000 73fa 0000 0074 00a0  ....C...s....t..
+00010600: 017c 0064 01a1 028f ca7d 067c 0564 006b  .|.d.....}.|.d.k
+00010610: 0872 267c 0664 0219 0064 0064 0085 0219  .r&|.d...d.d....
+00010620: 007d 057a 1a74 02a0 037c 0664 0319 0064  .}.z.t...|.d...d
+00010630: 0064 0085 0219 00a1 017d 0757 006e 2201  .d.......}.W.n".
+00010640: 0001 0001 0074 02a0 037c 0664 0419 0064  .....t...|.d...d
+00010650: 0064 0085 0219 00a1 017d 0759 006e 0258  .d.......}.Y.n.X
+00010660: 0074 047c 0083 017d 0874 0574 067c 0883  .t.|...}.t.t.|..
+00010670: 0183 0144 005d 585c 027d 095c 027d 0a7d  ...D.]X\.}.\.}.}
+00010680: 0b7c 0564 0064 0085 027c 0966 0219 007c  .|.d.d...|.f...|
+00010690: 0a17 007d 0c7c 0c64 0519 007c 0117 007d  ...}.|.d...|...}
+000106a0: 0d7c 0c64 0619 007c 0218 007d 0e74 077c  .|.d...|...}.t.|
+000106b0: 0e7c 0b67 0283 017d 0e64 067c 0774 087c  .|.g...}.d.|.t.|
+000106c0: 0d83 0174 087c 0e83 0185 023c 0071 7857  ...t.|.....<.qxW
+000106d0: 0035 0051 0052 0058 007c 0372 ee74 097c  .5.Q.R.X.|.r.t.|
+000106e0: 0064 037c 0764 078d 0301 007c 0472 f67c  .d.|.d.....|.r.|
+000106f0: 0753 0064 0053 0029 084e 72a6 0000 0072  .S.d.S.).Nr....r
+00010700: 6902 0000 72ab 0100 0072 5200 0000 7201  i...r....rR...r.
+00010710: 0000 0072 2e00 0000 2901 da08 6e65 775f  ...r....)...new_
+00010720: 6461 7461 290a 72ae 0000 0072 af00 0000  data).r....r....
+00010730: 721d 0000 0072 8400 0000 726e 0200 0072  r....r....rn...r
+00010740: 2400 0000 7237 0000 0072 6a02 0000 7288  $...r7...rj...r.
+00010750: 0000 0072 2201 0000 290f 72dc 0100 005a  ...r"...).r....Z
+00010760: 1070 6f6c 655f 7570 5f73 6574 5f74 696d  .pole_up_set_tim
+00010770: 655a 1870 6f6c 655f 646f 776e 5f61 6464  eZ.pole_down_add
+00010780: 5f74 6f5f 7472 6967 6765 7272 6f01 0000  _to_triggerro...
+00010790: 726b 0200 0072 6902 0000 72dd 0100 0072  rk...ri...r....r
+000107a0: 6c02 0000 724f 0100 0072 2c00 0000 723f  l...rO...r,...r?
+000107b0: 0000 0072 4000 0000 72c1 0000 0072 5902  ...r@...r....rY.
+000107c0: 0000 7245 0200 0072 1600 0000 7216 0000  ..rE...r....r...
+000107d0: 0072 1700 0000 da0f 6465 6669 6e65 5f69  .r......define_i
+000107e0: 6e5f 7261 6e67 6537 0b00 0073 2400 0000  n_range7...s$...
+000107f0: 0002 0e01 0801 1002 0201 1a01 0601 1c02  ................
+00010800: 0801 1801 1401 0c01 0c01 0c01 2001 0401  ............ ...
+00010810: 0e01 0401 7270 0200 0063 0400 0000 0000  ....rp...c......
+00010820: 0000 0000 0000 0600 0000 0900 0000 4300  ..............C.
+00010830: 0000 7378 0000 0074 007c 0064 0164 0264  ..sx...t.|.d.d.d
+00010840: 038d 037d 0474 01a0 027c 0064 04a1 028f  ...}.t...|.d....
+00010850: 547d 057c 017c 046b 0672 467c 0372 4674  T}.|.|.k.rF|.rFt
+00010860: 0364 0583 0101 007c 057c 013d 007c 056a  .d.....|.|.=.|.j
+00010870: 047c 017c 0264 068d 0201 006e 247c 017c  .|.|.d.....n$|.|
+00010880: 046b 0672 5c7c 0373 5c74 0364 0783 0101  .k.r\|.s\t.d....
+00010890: 006e 0e7c 056a 047c 017c 0264 068d 0201  .n.|.j.|.|.d....
+000108a0: 0057 0035 0051 0052 0058 0064 0053 0029  .W.5.Q.R.X.d.S.)
+000108b0: 084e 5446 724d 0200 0072 a600 0000 7a28  .NTFrM...r....z(
+000108c0: 6b65 7920 616c 7265 6164 7920 6578 6973  key already exis
+000108d0: 7473 2c20 6f76 6572 7772 6974 696e 6720  ts, overwriting 
+000108e0: 7661 6c75 652e 2e2e 7201 0100 007a 5d6b  value...r....z]k
+000108f0: 6579 2061 6c72 6561 6479 2065 7869 7374  ey already exist
+00010900: 732c 204e 4f54 206f 7665 7277 7269 7469  s, NOT overwriti
+00010910: 6e67 2076 616c 7565 2e2e 2e2c 200a 7365  ng value..., .se
+00010920: 7420 276f 7665 7277 7269 7465 5f69 665f  t 'overwrite_if_
+00010930: 6578 6973 7473 2720 746f 2054 7275 6520  exists' to True 
+00010940: 746f 206f 7665 7277 7269 7465 2905 72ab  to overwrite).r.
+00010950: 0000 0072 ae00 0000 72af 0000 0072 4b00  ...r....r....rK.
+00010960: 0000 72af 0100 0029 0672 dc01 0000 7221  ..r....).r....r!
+00010970: 0200 00da 0676 616c 7565 7372 7001 0000  .....valuesrp...
+00010980: 5a08 616c 6c5f 6b65 7973 72c0 0000 0072  Z.all_keysr....r
+00010990: 1600 0000 7216 0000 0072 1700 0000 724e  ....r....r....rN
+000109a0: 0100 004f 0b00 0073 1200 0000 0001 0e01  ...O...s........
+000109b0: 0e01 0c01 0801 0601 1001 0c01 0a02 724e  ..............rN
+000109c0: 0100 0063 0100 0000 0000 0000 0000 0000  ...c............
+000109d0: 0300 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
+000109e0: 007c 00a0 00a1 007d 0074 01a0 027c 00a1  .|.....}.t...|..
+000109f0: 017c 0018 007d 0174 01a0 037c 017c 0066  .|...}.t...|.|.f
+00010a00: 02a1 016a 047d 027c 0253 0072 0d01 0000  ...j.}.|.S.r....
+00010a10: 2905 72f9 0000 0072 1d00 0000 724f 0000  ).r....r....rO..
+00010a20: 0072 2500 0000 72f8 0000 0029 03da 0470  .r%...r....)...p
+00010a30: 7265 645a 097a 6572 6f5f 7072 6564 7253  redZ.zero_predrS
+00010a40: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00010a50: 0000 da21 626f 6f6c 5f70 7265 645f 746f  ...!bool_pred_to
+00010a60: 5f63 6c61 7373 5f70 7265 645f 666f 726d  _class_pred_form
+00010a70: 6174 696e 675c 0b00 0073 0800 0000 0001  ating\...s......
+00010a80: 0801 0e01 1001 7273 0200 0063 0200 0000  ......rs...c....
+00010a90: 0000 0000 0000 0000 0600 0000 0500 0000  ................
+00010aa0: 4300 0000 73bc 0100 0074 00a0 017c 00a1  C...s....t...|..
+00010ab0: 017d 0274 026a 03a0 04a1 007d 0374 057c  .}.t.j.....}.t.|
+00010ac0: 03a0 06a1 0083 017d 047c 017c 0464 0119  .......}.|.|.d..
+00010ad0: 006b 0273 3c7c 017c 037c 0464 0119 0019  .k.s<|.|.|.d....
+00010ae0: 006b 0272 5864 017c 027c 0264 026b 053c  .k.rXd.|.|.d.k.<
+00010af0: 0064 037c 027c 0264 046b 053c 0090 016e  .d.|.|.d.k.<...n
+00010b00: 607c 017c 0464 0319 006b 0273 747c 017c  `|.|.d...k.st|.|
+00010b10: 037c 0464 0319 0019 006b 0272 9064 017c  .|.d.....k.r.d.|
+00010b20: 027c 0264 056b 053c 0064 037c 027c 0264  .|.d.k.<.d.|.|.d
+00010b30: 046b 053c 0090 016e 287c 017c 0464 0419  .k.<...n(|.|.d..
+00010b40: 006b 0273 ac7c 017c 037c 0464 0419 0019  .k.s.|.|.|.d....
+00010b50: 006b 0272 c074 0764 067c 0117 0064 0717  .k.r.t.d.|...d..
+00010b60: 0083 0101 0064 0053 007c 017c 0464 0519  .....d.S.|.|.d..
+00010b70: 006b 0273 dc7c 017c 037c 0464 0519 0019  .k.s.|.|.|.d....
+00010b80: 006b 0272 e674 0764 0883 0101 006e d27c  .k.r.t.d.....n.|
+00010b90: 017c 0464 0219 006b 0290 0173 067c 017c  .|.d...k...s.|.|
+00010ba0: 037c 0464 0219 0019 006b 0290 0172 1a74  .|.d.....k...r.t
+00010bb0: 0764 067c 0117 0064 0717 0083 0101 0064  .d.|...d.......d
+00010bc0: 0053 007c 017c 0464 0919 006b 0290 0173  .S.|.|.d...k...s
+00010bd0: 3a7c 017c 037c 0464 0919 0019 006b 0290  :|.|.|.d.....k..
+00010be0: 0172 4e74 0764 067c 0117 0064 0717 0083  .rNt.d.|...d....
+00010bf0: 0101 0064 0053 007c 017c 0464 0a19 006b  ...d.S.|.|.d...k
+00010c00: 0290 0173 6e7c 017c 037c 0464 0a19 0019  ...sn|.|.|.d....
+00010c10: 006b 0290 0172 ac64 017c 027c 0264 056b  .k...r.d.|.|.d.k
+00010c20: 053c 007c 0264 046b 027d 0574 08a0 097c  .<.|.d.k.}.t...|
+00010c30: 0564 0364 0085 0219 0064 0ba1 027d 0564  .d.d.....d...}.d
+00010c40: 037c 027c 053c 0064 037c 027c 0264 046b  .|.|.<.d.|.|.d.k
+00010c50: 023c 006e 0c74 0a64 0c7c 0117 0083 0182  .<.n.t.d.|......
+00010c60: 017c 0253 0029 0d4e 7201 0000 0072 d900  .|.S.).Nr....r..
+00010c70: 0000 722e 0000 0072 4700 0000 7246 0000  ..r....rG...rF..
+00010c80: 007a 1563 616e 206e 6f74 2063 6f6e 7665  .z.can not conve
+00010c90: 7274 2074 7970 6520 7a0f 2072 6574 7572  rt type z. retur
+00010ca0: 6e69 6e67 204e 6f6e 657a 1d61 6c72 6561  ning Nonez.alrea
+00010cb0: 6479 2069 6e20 7468 6520 636f 7272 6563  dy in the correc
+00010cc0: 7420 666f 726d 6174 729b 0000 0072 5702  t formatr....rW.
+00010cd0: 0000 467a 246b 6579 2064 6f65 7320 6e6f  ..Fz$key does no
+00010ce0: 7420 6d61 7463 682e 2069 6e76 616c 6964  t match. invalid
+00010cf0: 206b 6579 202d 2d3e 2029 0b72 1b00 0000   key --> ).r....
+00010d00: 721c 0000 0072 c001 0000 7205 0000 005a  r....r....r....Z
+00010d10: 1b6c 6162 656c 5f6e 616d 696e 675f 7368  .label_naming_sh
+00010d20: 6f72 7468 616e 645f 6469 6374 7239 0000  orthand_dictr9..
+00010d30: 0072 9900 0000 724b 0000 0072 1d00 0000  .r....rK...r....
+00010d40: 7223 0000 00da 0a56 616c 7565 4572 726f  r#.....ValueErro
+00010d50: 7229 0672 4200 0000 7221 0200 0072 e500  r).rB...r!...r..
+00010d60: 0000 5a09 6e61 6d65 5f64 6963 7472 9900  ..Z.name_dictr..
+00010d70: 0000 5a14 6f6e 655f 746f 5f74 6865 5f6c  ..Z.one_to_the_l
+00010d80: 6566 745f 696e 6473 7216 0000 0072 1600  eft_indsr....r..
+00010d90: 0000 7217 0000 00da 1d63 6f6e 7665 7274  ..r......convert
+00010da0: 5f6c 6162 656c 735f 6261 636b 5f74 6f5f  _labels_back_to_
+00010db0: 6269 6e61 7279 630b 0000 7338 0000 0000  binaryc...s8....
+00010dc0: 010a 060a 010c 011c 010c 0110 021c 010c  ................
+00010dd0: 0110 021c 0110 0104 011c 010a 0120 0110  ............. ..
+00010de0: 0104 0120 0110 0104 0120 010c 0108 0114  ... ..... ......
+00010df0: 0108 010e 020c 0172 7502 0000 6300 0000  .......ru...c...
+00010e00: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00010e10: 0043 0000 0073 2600 0000 6401 7d00 7400  .C...s&...d.}.t.
+00010e20: a001 7c00 a101 a002 a100 7d01 7403 7c01  ..|.......}.t.|.
+00010e30: 8301 0100 7403 6402 8301 0100 6400 5300  ....t.d.....d.S.
+00010e40: 2903 4e7a 3270 7974 686f 6e33 2022 2f55  ).Nz2python3 "/U
+00010e50: 7365 7273 2f70 6869 6c2f 4472 6f70 626f  sers/phil/Dropbo
+00010e60: 782f 5550 4441 5445 5f57 4841 4343 5f50  x/UPDATE_WHACC_P
+00010e70: 5950 492e 7079 227a 7b70 6c65 6173 6520  YPI.py"z{please 
+00010e80: 7265 6665 7220 746f 2074 6865 206f 7065  refer to the ope
+00010e90: 6e20 7465 726d 696e 616c 2077 696e 646f  n terminal windo
+00010ea0: 7720 666f 7220 6675 7274 6865 7220 6465  w for further de
+00010eb0: 7461 696c 730a 7265 7275 6e20 7574 696c  tails.rerun util
+00010ec0: 732e 646f 776e 6c6f 6164 5f72 6573 6e65  s.download_resne
+00010ed0: 745f 6d6f 6465 6c28 2920 746f 2070 7574  t_model() to put
+00010ee0: 2074 6865 206d 6f64 656c 2066 696c 6520   the model file 
+00010ef0: 6261 636b 2904 725f 0000 00da 0570 6f70  back).r_.....pop
+00010f00: 656e 724d 0100 0072 4b00 0000 2902 7253  enrM...rK...).rS
+00010f10: 0000 0072 9300 0000 7216 0000 0072 1600  ...r....r....r..
+00010f20: 0000 7217 0000 00da 0c75 7064 6174 655f  ..r......update_
+00010f30: 7768 6163 638a 0b00 0073 0c00 0000 0008  whacc....s......
+00010f40: 0401 0e01 0801 0201 02ff 7277 0200 0063  ..........rw...c
+00010f50: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00010f60: 0500 0000 4300 0000 73a4 0000 0074 007c  ....C...s....t.|
+00010f70: 0074 0183 0273 9c7c 0173 1674 0264 0183  .t...s.|.s.t.d..
+00010f80: 0101 0074 037c 0083 0174 046a 056b 0872  ...t.|...t.j.k.r
+00010f90: 2c7c 0067 017d 026e 6c64 0274 0674 037c  ,|.g.}.nld.t.t.|
+00010fa0: 0083 0183 01a0 07a1 006b 0672 4a74 017c  .........k.rJt.|
+00010fb0: 0083 017d 026e 4e74 037c 0083 016a 0874  ...}.nNt.|...j.t
+00010fc0: 046a 096b 0272 8074 0274 037c 0083 0183  .j.k.r.t.t.|....
+00010fd0: 0101 0064 0373 9874 0a64 0474 0674 037c  ...d.s.t.d.t.t.|
+00010fe0: 0083 0183 0117 0083 0182 016e 1874 007c  ...........n.t.|
+00010ff0: 0074 0683 0272 927c 0067 017d 026e 067c  .t...r.|.g.}.n.|
+00011000: 0067 017d 027c 0253 007c 0053 0064 0053  .g.}.|.S.|.S.d.S
+00011010: 0029 054e 7a5e 696e 7075 7420 6973 2073  .).Nz^input is s
+00011020: 7570 706f 7365 6420 746f 2062 6520 6120  upposed to be a 
+00011030: 6c69 7374 2c20 636f 6e76 6572 7469 6e67  list, converting
+00011040: 2069 7420 6275 7420 7573 6572 2073 686f   it but user sho
+00011050: 756c 6420 646f 2074 6869 7320 746f 2073  uld do this to s
+00011060: 7570 7072 6573 7320 7468 6973 2077 6172  uppress this war
+00011070: 6e69 6e67 722e 0200 0046 7a54 7365 6520  ningr....FzTsee 
+00011080: 6d6f 6475 6c65 2077 6861 6363 2e75 7469  module whacc.uti
+00011090: 6c73 2e6d 616b 655f 6c69 7374 2c20 7765  ls.make_list, we
+000110a0: 2068 6176 6520 6e6f 7420 6f66 6669 6369   have not offici
+000110b0: 616c 2070 726f 746f 636f 6c20 666f 7220  al protocol for 
+000110c0: 7468 6973 2069 6e70 7574 2074 7970 6520  this input type 
+000110d0: 290b 720b 0100 0072 3900 0000 724b 0000  ).r....r9...rK..
+000110e0: 0072 1c01 0000 721d 0000 00da 0473 7472  .r....r......str
+000110f0: 5f72 ad00 0000 721d 0100 0072 7601 0000  _r....r....rv...
+00011100: 7277 0100 0072 4e00 0000 2903 7253 0000  rw...rN...).rS..
+00011110: 0072 5600 0000 7245 0200 0072 1600 0000  .rV...rE...r....
+00011120: 7216 0000 0072 1700 0000 7257 0000 0099  r....r....rW....
+00011130: 0b00 0073 2200 0000 0001 0a01 0401 0801  ...s"...........
+00011140: 0e01 0803 1401 0a01 1001 0c01 0a01 06ff  ................
+00011150: 0a02 0a01 0802 0601 0402 7257 0000 00da  ..........rW....
+00011160: 0769 6e64 6963 6573 6303 0000 0000 0000  .indicesc.......
+00011170: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
+00011180: 0073 6e00 0000 7c00 6a00 7c01 6a00 0200  .sn...|.j.|.j...
+00011190: 7d03 7d04 7401 a002 7c04 a101 7d05 7c00  }.}.t...|...}.|.
+000111a0: 7401 a002 7c03 7c04 1800 6401 1700 a101  t...|.|...d.....
+000111b0: 6400 6400 8502 6400 6602 1900 7c05 1700  d.d...d.f...|...
+000111c0: 1900 7c01 6b02 a003 6401 a101 7d06 7c02  ..|.k...d...}.|.
+000111d0: 6402 6b02 725e 7401 a004 7c06 a101 6403  d.k.r^t...|...d.
+000111e0: 1900 5300 7c02 6404 6b02 726a 7c06 5300  ..S.|.d.k.rj|.S.
+000111f0: 6400 5300 2905 4e72 2e00 0000 7279 0200  d.S.).Nr....ry..
+00011200: 0072 0100 0000 7286 0000 0029 0572 3001  .r....r....).r0.
+00011210: 0000 721d 0000 0072 b400 0000 722f 0000  ..r....r....r/..
+00011220: 0072 b900 0000 2907 da03 6172 72da 0373  .r....)...arr..s
+00011230: 6571 da0b 7265 7475 726e 5f74 7970 655a  eq..return_typeZ
+00011240: 024e 615a 044e 7365 715a 0572 5f73 6571  .NaZ.NseqZ.r_seq
+00011250: da01 4d72 1600 0000 7216 0000 0072 1700  ..Mr....r....r..
+00011260: 0000 da15 7365 6172 6368 5f73 6571 7565  ....search_seque
+00011270: 6e63 655f 6e75 6d70 79b0 0b00 0073 0e00  nce_numpy....s..
+00011280: 0000 0001 0e01 0a01 3002 0801 0e01 0801  ........0.......
+00011290: 727e 0200 0063 0300 0000 0000 0000 0000  r~...c..........
+000112a0: 0000 0e00 0000 0900 0000 4300 0000 73aa  ..........C...s.
+000112b0: 0000 0067 007d 0374 007c 0283 0164 0117  ...g.}.t.|...d..
+000112c0: 007d 0474 0174 027c 0083 0183 0144 005d  .}.t.t.|.....D.]
+000112d0: 565c 027d 055c 027d 067d 077c 017c 067c  V\.}.\.}.}.|.|.|
+000112e0: 0785 0219 007d 0874 037c 0864 0264 038d  .....}.t.|.d.d..
+000112f0: 025c 027d 097d 0a74 04a0 0564 0464 0584  .\.}.}.t...d.d..
+00011300: 007c 0944 0083 0174 04a0 0664 017c 047c  .|.D...t...d.|.|
+00011310: 04a1 03a1 025c 027d 0b7d 0c7c 03a0 077c  .....\.}.}.|...|
+00011320: 0ba1 0101 0071 1c74 04a0 087c 03a1 017d  .....q.t...|...}
+00011330: 037c 0374 04a0 087c 02a1 0114 007d 0374  .|.t...|.....}.t
+00011340: 04a0 0974 04a0 0a74 046a 0b7c 0364 0164  ...t...t.j.|.d.d
+00011350: 068d 02a1 01a1 017d 0d7c 0d53 0029 074e  .......}.|.S.).N
+00011360: 722e 0000 0072 0100 0000 2901 72f0 0000  r....r....).r...
+00011370: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00011380: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00011390: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+000113a0: 0453 0072 1600 0000 7248 0000 0072 3100  .S.r....rH...r1.
+000113b0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000113c0: 0072 3400 0000 c10b 0000 7304 0000 0006  .r4.......s.....
+000113d0: 0002 007a 3b66 696e 645f 7472 6961 6c73  ...z;find_trials
+000113e0: 5f77 6974 685f 7375 7370 6963 696f 7573  _with_suspicious
+000113f0: 5f70 7265 6469 6374 696f 6e73 2e3c 6c6f  _predictions.<lo
+00011400: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00011410: 72ff 0000 0029 0c72 3000 0000 7224 0000  r....).r0...r$..
+00011420: 0072 3700 0000 723b 0000 0072 1d00 0000  .r7...r;...r....
+00011430: da09 6869 7374 6f67 7261 6d72 8d00 0000  ..histogramr....
+00011440: 7223 0000 0072 3800 0000 7297 0100 0072  r#...r8...r....r
+00011450: 8a00 0000 da07 6e61 6e6d 6561 6e29 0e72  ......nanmean).r
+00011460: 4100 0000 5a09 7072 6564 5f62 6f6f 6c5a  A...Z.pred_boolZ
+00011470: 0b74 6d70 5f77 6569 6768 7473 5a08 616c  .tmp_weightsZ.al
+00011480: 6c5f 6c65 6e73 da04 6269 6e73 722c 0000  l_lens..binsr,..
+00011490: 0072 bd00 0000 72be 0000 0072 0102 0000  .r....r....r....
+000114a0: 72e5 0000 0072 4200 0000 72bf 0000 0072  r....rB...r....r
+000114b0: 5300 0000 5a1d 736f 7274 6564 5f77 6f72  S...Z.sorted_wor
+000114c0: 7374 5f65 7374 696d 6174 6564 5f74 7269  st_estimated_tri
+000114d0: 616c 7372 1600 0000 7216 0000 0072 1700  alsr....r....r..
+000114e0: 0000 da27 6669 6e64 5f74 7269 616c 735f  ...'find_trials_
+000114f0: 7769 7468 5f73 7573 7069 6369 6f75 735f  with_suspicious_
+00011500: 7072 6564 6963 7469 6f6e 73bb 0b00 0073  predictions....s
+00011510: 1600 0000 0001 0401 0c01 1801 0c01 1001  ................
+00011520: 2401 0c01 0a02 0e01 1a01 7282 0200 0063  $.........r....c
+00011530: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00011540: 0300 0000 4300 0000 7338 0000 0074 006a  ....C...s8...t.j
+00011550: 01a0 027c 00a1 0172 1a74 006a 01a0 037c  ...|...r.t.j...|
+00011560: 00a1 017d 006e 1a74 006a 01a0 047c 00a1  ...}.n.t.j...|..
+00011570: 0172 286e 0c64 0173 3474 0564 0283 0182  .r(n.d.s4t.d....
+00011580: 017c 0053 0029 034e 467a 1c74 6869 7320  .|.S.).NFz.this 
+00011590: 6973 206e 6f74 2061 2070 6174 6820 6f72  is not a path or
+000115a0: 2061 2066 696c 6529 0672 5f00 0000 7261   a file).r_...ra
+000115b0: 0000 0072 a900 0000 72a7 0000 0072 6200  ...r....r....rb.
+000115c0: 0000 724e 0000 0029 01da 0673 7472 5f69  ..rN...)...str_i
+000115d0: 6e72 1600 0000 7216 0000 0072 1700 0000  nr....r....r....
+000115e0: da0b 6173 7365 7274 5f70 6174 68ca 0b00  ..assert_path...
+000115f0: 0073 0c00 0000 0001 0c01 0e01 0c01 0202  .s..............
+00011600: 0c01 7284 0200 0063 0100 0000 0000 0000  ..r....c........
+00011610: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00011620: 734e 0000 0074 007c 0083 017d 0074 01a0  sN...t.|...}.t..
+00011630: 02a1 0064 016b 0272 2074 03a0 047c 00a1  ...d.k.r t...|..
+00011640: 0101 006e 2a74 01a0 02a1 0064 026b 0272  ...n*t.....d.k.r
+00011650: 3c74 05a0 0664 037c 0067 02a1 0101 006e  <t...d.|.g.....n
+00011660: 0e74 05a0 0664 047c 0067 02a1 0101 0064  .t...d.|.g.....d
+00011670: 0053 0029 054e da07 5769 6e64 6f77 73da  .S.).N..Windows.
+00011680: 0644 6172 7769 6e72 ba01 0000 7a08 7864  .Darwinr....z.xd
+00011690: 672d 6f70 656e 2907 7284 0200 00da 0870  g-open).r......p
+000116a0: 6c61 7466 6f72 6dda 0673 7973 7465 6d72  latform..systemr
+000116b0: 5f00 0000 5a09 7374 6172 7466 696c 65da  _...Z.startfile.
+000116c0: 0a73 7562 7072 6f63 6573 73da 0550 6f70  .subprocess..Pop
+000116d0: 656e 726f 0000 0072 1600 0000 7216 0000  enro...r....r...
+000116e0: 0072 1700 0000 da0b 6f70 656e 5f66 6f6c  .r......open_fol
+000116f0: 6465 72d4 0b00 0073 0c00 0000 0001 0801  der....s........
+00011700: 0c01 0c01 0c01 1002 728b 0200 0063 0200  ........r....c..
+00011710: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00011720: 0000 4300 0000 733c 0000 007c 006a 0064  ..C...s<...|.j.d
+00011730: 0119 0064 016b 0272 2274 0174 02a0 037c  ...d.k.r"t.t...|
+00011740: 00a1 017c 0164 028d 027d 026e 1674 0474  ...|.d...}.n.t.t
+00011750: 02a0 037c 00a1 017c 0164 0167 0264 028d  ...|...|.d.g.d..
+00011760: 027d 027c 0253 0029 034e 722e 0000 0029  .}.|.S.).Nr....)
+00011770: 015a 0b6b 6572 6e65 6c5f 7369 7a65 2905  .Z.kernel_size).
+00011780: 7221 0000 0072 0900 0000 721b 0000 0072  r!...r....r....r
+00011790: 1c00 0000 720a 0000 0029 03da 0c70 7265  ....r....)...pre
+000117a0: 645f 626f 6f6c 5f69 6eda 0e6b 6572 6e65  d_bool_in..kerne
+000117b0: 6c5f 7369 7a65 5f69 6eda 0d70 7265 645f  l_size_in..pred_
+000117c0: 626f 6f6c 5f6f 7574 7216 0000 0072 1600  bool_outr....r..
+000117d0: 0000 7217 0000 00da 196d 6564 6669 6c74  ..r......medfilt
+000117e0: 5f63 6f6e 6669 6465 6e63 655f 7363 6f72  _confidence_scor
+000117f0: 6573 de0b 0000 7308 0000 0000 010e 0114  es....s.........
+00011800: 0216 0172 8f02 0000 729c 0000 0063 0200  ...r....r....c..
+00011810: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00011820: 0000 4300 0000 7332 0000 007c 006a 0064  ..C...s2...|.j.d
+00011830: 0119 0064 016b 0272 207c 007c 016b 0464  ...d.k.r |.|.k.d
+00011840: 0114 00a0 01a1 007d 026e 0e74 026a 037c  .......}.n.t.j.|
+00011850: 0064 0164 028d 027d 027c 0253 0029 034e  .d.d...}.|.S.).N
+00011860: 722e 0000 0072 ff00 0000 2904 7221 0000  r....r....).r!..
+00011870: 0072 f900 0000 721d 0000 0072 ef00 0000  .r....r....r....
+00011880: 2903 728c 0200 00da 0974 6872 6573 685f  ).r......thresh_
+00011890: 696e 728e 0200 0072 1600 0000 7216 0000  inr....r....r...
+000118a0: 0072 1700 0000 da19 636f 6e66 6964 656e  .r......confiden
+000118b0: 6365 5f73 636f 7265 5f74 6f5f 636c 6173  ce_score_to_clas
+000118c0: 73e6 0b00 0073 0800 0000 0001 0e01 1202  s....s..........
+000118d0: 0e02 7291 0200 0063 0400 0000 0000 0000  ..r....c........
+000118e0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+000118f0: 733c 0000 0074 007c 007c 0383 027d 0474  s<...t.|.|...}.t
+00011900: 017c 047c 0283 027d 0464 01a0 027c 01a0  .|.|...}.d...|..
+00011910: 0364 02a1 0164 0319 00a0 0364 04a1 01a1  .d...d.....d....
+00011920: 017d 0574 047c 047c 0583 027d 047c 0453  .}.t.|.|...}.|.S
+00011930: 0029 054e 72e6 0100 00da 025f 5f72 4600  .).Nr......__rF.
+00011940: 0000 728b 0100 0029 0572 8f02 0000 7291  ..r....).r....r.
+00011950: 0200 0072 da00 0000 72db 0000 0072 7502  ...r....r....ru.
+00011960: 0000 2906 728c 0200 005a 0b6b 6579 5f6e  ..).r....Z.key_n
+00011970: 616d 655f 696e 7290 0200 0072 8d02 0000  ame_inr....r....
+00011980: 728e 0200 005a 064c 5f6b 6579 5f72 1600  r....Z.L_key_r..
+00011990: 0000 7216 0000 0072 1700 0000 da19 7072  ..r....r......pr
+000119a0: 6f63 6573 735f 636f 6e66 6964 656e 6365  ocess_confidence
+000119b0: 5f73 636f 7265 73ef 0b00 0073 0a00 0000  _scores....s....
+000119c0: 0001 0a01 0a01 1a01 0a01 7293 0200 0063  ..........r....c
+000119d0: 0200 0000 0000 0000 0000 0000 0800 0000  ................
+000119e0: 0800 0000 4300 0000 7380 0000 0074 006a  ....C...s....t.j
+000119f0: 01a0 027c 00a1 017d 0074 037c 0083 0174  ...|...}.t.|...t
+00011a00: 0374 006a 016a 0483 0117 007d 0274 057c  .t.j.j.....}.t.|
+00011a10: 0183 016a 0664 0164 0164 028d 0201 0074  ...j.d.d.d.....t
+00011a20: 00a0 077c 00a1 0144 005d 3e5c 037d 037d  ...|...D.]>\.}.}
+00011a30: 047d 057c 0444 005d 2e7d 0674 006a 01a0  .}.|.D.].}.t.j..
+00011a40: 087c 017c 037c 0264 0085 0219 007c 06a1  .|.|.|.d.....|..
+00011a50: 037d 0774 057c 0783 016a 0664 0164 0164  .}.t.|...j.d.d.d
+00011a60: 028d 0201 0071 4a71 3c64 0053 0072 5f01  .....qJq<d.S.r_.
+00011a70: 0000 2909 725f 0000 0072 6100 0000 da07  ..).r_...ra.....
+00011a80: 6162 7370 6174 6872 3000 0000 7260 0000  abspathr0...r`..
+00011a90: 0072 0e00 0000 7263 0100 0072 1202 0000  .r....rc...r....
+00011aa0: 72da 0000 0029 08da 0373 7263 727a 0000  r....)...srcrz..
+00011ab0: 005a 0a73 7263 5f70 7265 6669 7872 1502  .Z.src_prefixr..
+00011ac0: 0000 7216 0200 0072 1702 0000 72a7 0000  ..r....r....r...
+00011ad0: 00da 0764 6972 7061 7468 7216 0000 0072  ...dirpathr....r
+00011ae0: 1600 0000 7217 0000 0072 9901 0000 f70b  ....r....r......
+00011af0: 0000 730e 0000 0000 010c 0114 0112 0114  ..s.............
+00011b00: 0108 0118 0172 9901 0000 6308 0000 0000  .....r....c.....
+00011b10: 0000 0000 0000 000f 0000 0006 0000 0043  ...............C
+00011b20: 0000 0073 5001 0000 7c00 a000 7401 6a02  ...sP...|...t.j.
+00011b30: a101 7401 6a02 1700 7d00 7c01 a000 7401  ..t.j...}.|...t.
+00011b40: 6a02 a101 7401 6a02 1700 7d01 7403 7c00  j...t.j...}.t.|.
+00011b50: 6401 6402 8d02 7d08 7404 7c08 7c02 7c03  d.d...}.t.|.|.|.
+00011b60: 6403 8d03 7d09 7c05 7264 6404 6405 8400  d...}.|.rdd.d...
+00011b70: 7405 7c09 8301 4400 8301 7d0a 7c07 7260  t.|...D...}.|.r`
+00011b80: 7c09 6406 6602 5300 6406 5300 6700 7d0b  |.d.f.S.d.S.g.}.
+00011b90: 7c09 4400 5d3e 7d0c 7c01 a006 7c0c a007  |.D.]>}.|...|...
+00011ba0: 7c00 a101 a101 7d0d 7401 6a08 a009 7c0c  |.....}.t.j...|.
+00011bb0: a101 72a0 740a 7c0d 8301 6a0b 6407 6407  ..r.t.|...j.d.d.
+00011bc0: 6408 8d02 0100 716c 7c0b a00c 7c0c a101  d.....ql|...|...
+00011bd0: 0100 716c 6700 7d0e 740d 7c0b 7c06 6409  ..qlg.}.t.|.|.d.
+00011be0: 8d02 4400 5d80 7d0c 7c01 a006 7c0c a007  ..D.].}.|...|...
+00011bf0: 7c00 a101 a101 7d0d 7c0e a00c 7c0d a101  |.....}.|...|...
+00011c00: 0100 7c04 73ec 7401 6a08 a00e 7c0d a101  ..|.s.t.j...|...
+00011c10: 9001 732c 7401 6a08 a00e 7c0d a101 9001  ..s,t.j...|.....
+00011c20: 7204 7401 a00f 7c0d a101 0100 740a 7401  r.t...|.....t.t.
+00011c30: 6a08 a010 7c0d a101 8301 6a0b 6407 6407  j...|.....j.d.d.
+00011c40: 6408 8d02 0100 7411 a012 7c0c 7c0d a102  d.....t...|.|...
+00011c50: 0100 71bc 7c04 73bc 7413 640a 7c0d 1700  ..q.|.s.t.d.|...
+00011c60: 8301 0100 71bc 7c07 9001 724c 7c0b 7c0e  ....q.|...rL|.|.
+00011c70: 6602 5300 6406 5300 290b 61ee 0200 000a  f.S.d.S.).a.....
+00011c80: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00011c90: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00011ca0: 2020 2072 6574 7572 6e5f 6c69 7374 5f6f     return_list_o
+00011cb0: 665f 6669 6c65 7320 3a0a 2020 2020 7372  f_files :.    sr
+00011cc0: 6320 3a20 736f 7572 6365 2066 6f6c 6465  c : source folde
+00011cd0: 720a 2020 2020 6473 7420 3a20 6465 7374  r.    dst : dest
+00011ce0: 696e 6174 696f 6e20 666f 6c64 6572 0a20  ination folder. 
+00011cf0: 2020 206b 6565 705f 7374 7269 6e67 7320     keep_strings 
+00011d00: 3a20 7365 6520 7574 696c 732e 6c69 7374  : see utils.list
+00011d10: 6572 5f69 742c 206c 6973 7420 6f66 2073  er_it, list of s
+00011d20: 7472 696e 6773 2074 6f20 6d61 7463 6820  trings to match 
+00011d30: 696e 206f 7264 6572 2074 6f20 636f 7079  in order to copy
+00011d40: 0a20 2020 2072 656d 6f76 655f 7374 7269  .    remove_stri
+00011d50: 6e67 203a 2073 6565 2075 7469 6c73 2e6c  ng : see utils.l
+00011d60: 6973 7465 725f 6974 2c20 6c69 7374 206f  ister_it, list o
+00011d70: 6620 7374 7269 6e67 7320 746f 206d 6174  f strings to mat
+00011d80: 6368 2069 6e20 6f72 6465 7220 746f 206e  ch in order to n
+00011d90: 6f74 2063 6f70 790a 2020 2020 6f76 6572  ot copy.    over
+00011da0: 7772 6974 6520 3a20 7769 6c6c 206f 7665  write : will ove
+00011db0: 7277 7269 7465 2066 696c 6573 2069 6620  rwrite files if 
+00011dc0: 7472 7565 0a20 2020 206a 7573 745f 7072  true.    just_pr
+00011dd0: 696e 745f 7768 6174 5f77 696c 6c5f 6265  int_what_will_be
+00011de0: 5f63 6f70 6965 6420 3a20 6361 6e20 6a75  _copied : can ju
+00011df0: 7374 2070 7269 6e74 2077 6861 7420 7769  st print what wi
+00011e00: 6c6c 2062 6520 636f 7069 6564 2074 6f20  ll be copied to 
+00011e10: 6265 2073 7572 6520 6974 2069 7320 636f  be sure it is co
+00011e20: 7272 6563 740a 2020 2020 6469 7361 626c  rrect.    disabl
+00011e30: 655f 7471 646d 203a 2069 6620 5472 7565  e_tqdm : if True
+00011e40: 2069 7420 7769 6c6c 2070 7265 7665 6e74   it will prevent
+00011e50: 2074 6865 2054 5144 4d20 6c6f 6164 696e   the TQDM loadin
+00011e60: 6720 6261 720a 0a20 2020 2045 7861 6d70  g bar..    Examp
+00011e70: 6c65 730a 2020 2020 5f5f 5f5f 5f5f 5f5f  les.    ________
+00011e80: 0a20 2020 2063 6f70 795f 6669 6c65 5f66  .    copy_file_f
+00011e90: 696c 7465 7228 272f 5573 6572 732f 7068  ilter('/Users/ph
+00011ea0: 696c 2f44 6573 6b74 6f70 2f46 414b 455f  il/Desktop/FAKE_
+00011eb0: 6675 6c6c 5f64 6174 6127 2c20 272f 5573  full_data', '/Us
+00011ec0: 6572 732f 7068 696c 2f44 6573 6b74 6f70  ers/phil/Desktop
+00011ed0: 2f61 6161 6161 6161 6161 6127 2c20 6b65  /aaaaaaaaaa', ke
+00011ee0: 6570 5f73 7472 696e 6773 3d27 2f33 6c61  ep_strings='/3la
+00011ef0: 672f 272c 0a20 2020 2020 2020 2020 2020  g/',.           
+00011f00: 2020 2020 2020 7265 6d6f 7665 5f73 7472        remove_str
+00011f10: 696e 673d 4e6f 6e65 2c20 6f76 6572 7772  ing=None, overwr
+00011f20: 6974 653d 5472 7565 2c20 6a75 7374 5f70  ite=True, just_p
+00011f30: 7269 6e74 5f77 6861 745f 7769 6c6c 5f62  rint_what_will_b
+00011f40: 655f 636f 7069 6564 3d46 616c 7365 290a  e_copied=False).
+00011f50: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00011f60: 2d2d 2d2d 2d2d 2d0a 0a20 2020 20da 012a  -------..    ..*
+00011f70: 2901 7214 0200 0029 0272 d801 0000 72d9  ).r....).r....r.
+00011f80: 0100 0063 0100 0000 0000 0000 0000 0000  ...c............
+00011f90: 0300 0000 0500 0000 5300 0000 7324 0000  ........S...s$..
+00011fa0: 0067 007c 005d 1c5c 027d 017d 0274 0074  .g.|.].\.}.}.t.t
+00011fb0: 017c 0183 0164 0017 007c 0217 0083 0191  .|...d...|......
+00011fc0: 0271 0453 0029 0172 8b01 0000 2902 724b  .q.S.).r....).rK
+00011fd0: 0000 0072 ad00 0000 720a 0200 0072 1600  ...r....r....r..
+00011fe0: 0000 7216 0000 0072 1700 0000 7234 0000  ..r....r....r4..
+00011ff0: 001f 0c00 0073 0400 0000 0600 0600 7a24  .....s........z$
+00012000: 636f 7079 5f66 696c 655f 6669 6c74 6572  copy_file_filter
+00012010: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00012020: 6f6d 703e 4e54 7260 0100 0029 01da 0764  omp>NTr`...)...d
+00012030: 6973 6162 6c65 7a2c 6f76 6572 7772 6974  isablez,overwrit
+00012040: 6520 3d20 4661 6c73 653a 2066 696c 6520  e = False: file 
+00012050: 6578 6973 7473 2c20 736b 6970 7069 6e67  exists, skipping
+00012060: 2d2d 3e20 2914 da06 7273 7472 6970 725f  --> )...rstripr_
+00012070: 0000 0072 6000 0000 7296 0100 0072 da01  ...r`...r....r..
+00012080: 0000 7224 0000 0072 da00 0000 72db 0000  ..r$...r....r...
+00012090: 0072 6100 0000 7262 0000 0072 0e00 0000  .ra...rb...r....
+000120a0: 7263 0100 0072 2300 0000 720b 0000 0072  rc...r#...r....r
+000120b0: a900 0000 7279 0000 0072 a700 0000 7273  ....ry...r....rs
+000120c0: 0000 00da 0863 6f70 7966 696c 6572 4b00  .....copyfilerK.
+000120d0: 0000 290f 7295 0200 0072 7a00 0000 72d8  ..).r....rz...r.
+000120e0: 0100 0072 d901 0000 725c 0000 005a 1e6a  ...r....r\...Z.j
+000120f0: 7573 745f 7072 696e 745f 7768 6174 5f77  ust_print_what_w
+00012100: 696c 6c5f 6265 5f63 6f70 6965 645a 0c64  ill_be_copiedZ.d
+00012110: 6973 6162 6c65 5f74 7164 6d5a 1472 6574  isable_tqdmZ.ret
+00012120: 7572 6e5f 6c69 7374 5f6f 665f 6669 6c65  urn_list_of_file
+00012130: 735a 1261 6c6c 5f66 696c 6573 5f61 6e64  sZ.all_files_and
+00012140: 5f64 6972 735a 0774 6f5f 636f 7079 72e6  _dirsZ.to_copyr.
+00012150: 0100 005a 0874 6f5f 636f 7079 3272 3300  ...Z.to_copy2r3.
+00012160: 0000 72be 0000 005a 0c66 696e 616c 5f63  ..r....Z.final_c
+00012170: 6f70 6965 6472 1600 0000 7216 0000 0072  opiedr....r....r
+00012180: 1700 0000 da10 636f 7079 5f66 696c 655f  ......copy_file_
+00012190: 6669 6c74 6572 010c 0000 7338 0000 0000  filter....s8....
+000121a0: 1712 0112 020c 010e 0204 0112 0104 0108  ................
+000121b0: 0204 0204 0108 0110 010c 0114 020c 0104  ................
+000121c0: 0110 0110 010a 0112 010e 010a 011a 010e  ................
+000121d0: 0104 010e 0106 0172 9b02 0000 7264 0200  .......r....rd..
+000121e0: 0063 0200 0000 0000 0000 0000 0000 0a00  .c..............
+000121f0: 0000 0600 0000 4300 0000 73f8 0000 0067  ......C...s....g
+00012200: 007d 0267 007d 0367 007d 0474 007c 0083  .}.g.}.g.}.t.|..
+00012210: 0144 005d d85c 027d 057d 067c 06a0 0174  .D.].\.}.}.|...t
+00012220: 026a 03a1 017d 0674 026a 04a0 057c 06a1  .j...}.t.j...|..
+00012230: 0172 1474 026a 04a0 067c 06a1 017d 0774  .r.t.j...|...}.t
+00012240: 026a 03a0 077c 06a0 0874 026a 03a1 0164  .j...|...t.j...d
+00012250: 0064 0185 0219 00a1 0174 026a 0317 007c  .d.......t.j...|
+00012260: 0117 0074 026a 0317 007d 0874 097c 0864  ...t.j...}.t.|.d
+00012270: 0283 027d 0964 037c 07a0 0aa1 006b 0672  ...}.d.|.....k.r
+00012280: 9074 0b7c 0964 0364 048d 027d 096e 1864  .t.|.d.d...}.n.d
+00012290: 057c 07a0 0aa1 006b 0672 a874 0b7c 0964  .|.....k.r.t.|.d
+000122a0: 0564 048d 027d 0974 0c7c 0983 0164 066b  .d...}.t.|...d.k
+000122b0: 0272 d87c 02a0 0d7c 06a1 0101 007c 03a0  .r.|...|.....|..
+000122c0: 0d7c 0964 0219 00a1 0101 007c 04a0 0d7c  .|.d.......|...|
+000122d0: 05a1 0101 0071 1474 0e64 077c 0717 0064  .....q.t.d.|...d
+000122e0: 0817 0083 0101 0001 0071 ee71 147c 027c  .........q.q.|.|
+000122f0: 037c 0466 0353 0029 094e 72e9 0100 0072  .|.f.S.).Nr....r
+00012300: 0100 0000 5a05 7472 6169 6e29 0172 d801  ....Z.train).r..
+00012310: 0000 da03 7661 6c72 2e00 0000 7a0a 4669  ....valr....z.Fi
+00012320: 6c65 206e 616d 6520 7a1b 2063 6f75 6c64  le name z. could
+00012330: 206e 6f74 2066 696e 6420 7661 6c69 6420   not find valid 
+00012340: 6d61 7463 6829 0f72 2400 0000 7299 0200  match).r$...r...
+00012350: 0072 5f00 0000 7260 0000 0072 6100 0000  .r_...r`...ra...
+00012360: 72a9 0000 0072 a800 0000 72da 0000 0072  r....r....r....r
+00012370: db00 0000 7229 0100 0072 1d01 0000 72da  ....r)...r....r.
+00012380: 0100 0072 3000 0000 7223 0000 0072 4b00  ...r0...r#...rK.
+00012390: 0000 290a 7219 0200 005a 1561 6c74 5f6c  ..).r....Z.alt_l
+000123a0: 6162 656c 5f66 6f6c 6465 725f 6e61 6d65  abel_folder_name
+000123b0: 5a07 6835 5f69 6d67 735a 0968 355f 6c61  Z.h5_imgsZ.h5_la
+000123c0: 6265 6c73 5a0d 696e 6473 5f6f 665f 6669  belsZ.inds_of_fi
+000123d0: 6c65 7372 2c00 0000 7233 0000 0072 4f01  lesr,...r3...rO.
+000123e0: 0000 5a0e 616c 745f 6c61 6265 6c73 5f64  ..Z.alt_labels_d
+000123f0: 6972 7250 0000 0072 1600 0000 7216 0000  irrP...r....r...
+00012400: 0072 1700 0000 da22 636f 7079 5f61 6c74  .r....."copy_alt
+00012410: 5f6c 6162 656c 735f 6261 7365 645f 6f6e  _labels_based_on
+00012420: 5f64 6972 6563 746f 7279 3b0c 0000 7328  _directory;...s(
+00012430: 0000 0000 0104 0104 0104 0110 010c 010c  ................
+00012440: 010c 012c 010a 010c 010e 010c 010c 010c  ...,............
+00012450: 010a 010e 010c 0210 0106 0172 9d02 0000  ...........r....
+00012460: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00012470: 0006 0000 0043 0000 0073 8000 0000 7400  .....C...s....t.
+00012480: 6401 7401 a002 7c00 a101 8302 0100 7400  d.t...|.......t.
+00012490: 6402 7401 a003 7c00 a101 8302 0100 7400  d.t...|.......t.
+000124a0: 6403 7401 a004 7c00 a101 8302 0100 7400  d.t...|.......t.
+000124b0: 6404 7c00 6a05 8302 0100 7400 6405 7406  d.|.j.....t.d.t.
+000124c0: 7401 a007 7c00 a101 8301 8302 0100 7400  t...|.........t.
+000124d0: 6406 7408 7c00 8301 8302 0100 7a10 7400  d.t.|.......z.t.
+000124e0: 6407 7c00 6a09 8302 0100 5700 6e0c 0100  d.|.j.....W.n...
+000124f0: 0100 0100 5900 6e02 5800 6400 5300 2908  ....Y.n.X.d.S.).
+00012500: 4e7a 040a 6d69 6e72 1301 0000 7287 0000  Nz..minr....r...
+00012510: 0072 2100 0000 7a0d 6c65 6e20 6f66 2075  .r!...z.len of u
+00012520: 6e69 7175 6572 1c01 0000 7a06 4474 7970  niquer....z.Dtyp
+00012530: 6520 290a 724b 0000 0072 1d00 0000 726a  e ).rK...r....rj
+00012540: 0200 0072 1301 0000 7287 0000 0072 2100  ...r....r....r!.
+00012550: 0000 7230 0000 0072 d200 0000 721c 0100  ..r0...r....r...
+00012560: 00da 0564 7479 7065 2901 5a06 696e 5f61  ...dtype).Z.in_a
+00012570: 7272 7216 0000 0072 1600 0000 7217 0000  rrr....r....r...
+00012580: 0072 7501 0000 530c 0000 7314 0000 0000  .ru...S...s.....
+00012590: 0110 0110 0110 010c 0114 010e 0102 0110  ................
+000125a0: 0106 0172 7501 0000 6302 0000 0000 0000  ...ru...c.......
+000125b0: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
+000125c0: 0073 1200 0000 7c01 7400 7c00 6401 6402  .s....|.t.|.d.d.
+000125d0: 6403 8d03 6b06 5300 2904 4e54 4672 4d02  d...k.S.).NTFrM.
+000125e0: 0000 2901 72ab 0000 0029 0272 c200 0000  ..).r....).r....
+000125f0: da06 6b65 795f 696e 7216 0000 0072 1600  ..key_inr....r..
+00012600: 0000 7217 0000 0072 6d01 0000 600c 0000  ..r....rm...`...
+00012610: 7302 0000 0000 0172 6d01 0000 6302 0000  s......rm...c...
+00012620: 0000 0000 0000 0000 0003 0000 0009 0000  ................
+00012630: 0043 0000 0073 2c00 0000 7400 7c00 7c01  .C...s,...t.|.|.
+00012640: 8302 7228 7401 a002 7c00 6401 a102 8f0c  ..r(t...|.d.....
+00012650: 7d02 7c02 7c01 3d00 5700 3500 5100 5200  }.|.|.=.W.5.Q.R.
+00012660: 5800 6400 5300 a902 4e72 a600 0000 a903  X.d.S...Nr......
+00012670: 726d 0100 0072 ae00 0000 72af 0000 0029  rm...r....r....)
+00012680: 0372 c200 0000 729f 0200 0072 c000 0000  .r....r....r....
+00012690: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+000126a0: 4c01 0000 640c 0000 7306 0000 0000 010a  L...d...s.......
+000126b0: 010e 0172 4c01 0000 6303 0000 0000 0000  ...rL...c.......
+000126c0: 0000 0000 0005 0000 0009 0000 0043 0000  .............C..
+000126d0: 0073 4000 0000 7400 7c00 7c01 8302 7d03  .s@...t.|.|...}.
+000126e0: 7401 a002 7c00 6401 a102 8f20 7d04 7c03  t...|.d.... }.|.
+000126f0: 7222 7c04 7c01 3d00 7c02 6400 6b09 7232  r"|.|.=.|.d.k.r2
+00012700: 7c02 7c04 7c01 3c00 5700 3500 5100 5200  |.|.|.<.W.5.Q.R.
+00012710: 5800 6400 5300 72a0 0200 0072 a102 0000  X.d.S.r....r....
+00012720: 2905 72c2 0000 0072 9f02 0000 726f 0200  ).r....r....ro..
+00012730: 005a 0a65 7869 7374 5f74 6573 7472 c000  .Z.exist_testr..
+00012740: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00012750: 0072 2201 0000 6a0c 0000 730c 0000 0000  .r"...j...s.....
+00012760: 010a 010e 0104 0106 0108 0172 2201 0000  ...........r"...
+00012770: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00012780: 0002 0000 0043 0000 0073 0e00 0000 6401  .....C...s....d.
+00012790: 6402 8400 7c00 4400 8301 5300 2903 4e63  d...|.D...S.).Nc
+000127a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000127b0: 0600 0000 5300 0000 7318 0000 0067 007c  ....S...s....g.|
+000127c0: 005d 107d 017c 01a0 0064 0064 01a1 0291  .].}.|...d.d....
+000127d0: 0271 0453 0072 1601 0000 721a 0100 0029  .q.S.r....r....)
+000127e0: 0272 3200 0000 da01 6e72 1600 0000 7216  .r2.....nr....r.
+000127f0: 0000 0072 1700 0000 7234 0000 0074 0c00  ...r....r4...t..
+00012800: 0073 0400 0000 0600 0200 7a32 636f 6e76  .s........z2conv
+00012810: 6572 745f 6c69 7374 5f6f 665f 7374 7269  ert_list_of_stri
+00012820: 6e67 735f 666f 725f 6835 2e3c 6c6f 6361  ngs_for_h5.<loca
+00012830: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7216  ls>.<listcomp>r.
+00012840: 0000 0029 0172 1e01 0000 7216 0000 0072  ...).r....r....r
+00012850: 1600 0000 7217 0000 00da 1e63 6f6e 7665  ....r......conve
+00012860: 7274 5f6c 6973 745f 6f66 5f73 7472 696e  rt_list_of_strin
+00012870: 6773 5f66 6f72 5f68 3573 0c00 0073 0200  gs_for_h5s...s..
+00012880: 0000 0001 72a3 0200 0063 0200 0000 0000  ....r....c......
+00012890: 0000 0000 0000 0200 0000 0300 0000 0300  ................
+000128a0: 0000 7312 0000 0087 0066 0164 0164 0284  ..s......f.d.d..
+000128b0: 087c 0044 0083 0153 0029 037a 5572 6574  .|.D...S.).zUret
+000128c0: 756e 2069 6e6e 6465 7820 6f66 206c 656e  un inndex of len
+000128d0: 6774 6820 6c65 6e28 6172 7231 2920 696e  gth len(arr1) in
+000128e0: 7374 6561 6420 6f66 206e 756d 7079 7320  stead of numpys 
+000128f0: 6c65 6e67 7468 206d 696e 285b 6c65 6e28  length min([len(
+00012900: 6172 7231 292c 206c 656e 2861 7272 3229  arr1), len(arr2)
+00012910: 5d29 6301 0000 0000 0000 0000 0000 0002  ])c.............
+00012920: 0000 0005 0000 0013 0000 0073 2200 0000  ...........s"...
+00012930: 6700 7c00 5d1a 7d01 6400 6401 8400 7400  g.|.].}.d.d...t.
+00012940: 8800 8301 4400 8301 7c01 1900 9102 7104  ....D...|.....q.
+00012950: 5300 2902 6301 0000 0000 0000 0000 0000  S.).c...........
+00012960: 0003 0000 0004 0000 0053 0000 0073 1600  .........S...s..
+00012970: 0000 6900 7c00 5d0e 5c02 7d01 7d02 7c02  ..i.|.].\.}.}.|.
+00012980: 7c01 9302 7104 5300 7216 0000 0072 1600  |...q.S.r....r..
+00012990: 0000 2903 7232 0000 0072 2c00 0000 7204  ..).r2...r,...r.
+000129a0: 0200 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000129b0: 0000 da0a 3c64 6963 7463 6f6d 703e 790c  ....<dictcomp>y.
+000129c0: 0000 7306 0000 0006 0006 0002 007a 2c69  ..s..........z,i
+000129d0: 6e74 6572 7365 6374 5f61 6c6c 2e3c 6c6f  ntersect_all.<lo
+000129e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000129f0: 2e3c 6469 6374 636f 6d70 3e72 0b02 0000  .<dictcomp>r....
+00012a00: 2902 7232 0000 0072 0402 0000 a901 72e4  ).r2...r......r.
+00012a10: 0000 0072 1600 0000 7217 0000 0072 3400  ...r....r....r4.
+00012a20: 0000 790c 0000 7304 0000 0006 0002 007a  ..y...s........z
+00012a30: 2169 6e74 6572 7365 6374 5f61 6c6c 2e3c  !intersect_all.<
+00012a40: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00012a50: 703e 7216 0000 0029 0272 e300 0000 72e4  p>r....).r....r.
+00012a60: 0000 0072 1600 0000 72a5 0200 0072 1700  ...r....r....r..
+00012a70: 0000 da0d 696e 7465 7273 6563 745f 616c  ....intersect_al
+00012a80: 6c77 0c00 0073 0200 0000 0002 72a6 0200  lw...s......r...
+00012a90: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00012aa0: 0000 0300 0000 4300 0000 7320 0000 0074  ......C...s ...t
+00012ab0: 00a0 017c 00a1 016a 0264 011b 007c 016b  ...|...j.d...|.k
+00012ac0: 0473 1c74 0364 0283 0182 0164 0053 0029  .s.t.d.....d.S.)
+00012ad0: 034e 6900 ca9a 3b7a 3773 7061 6365 5f63  .Ni...;z7space_c
+00012ae0: 6865 636b 2066 756e 6374 696f 6e3a 2047  heck function: G
+00012af0: 4220 6c69 6d69 7420 7265 6163 6865 642c  B limit reached,
+00012b00: 2065 6e64 696e 6720 6675 6e63 7469 6f6e   ending function
+00012b10: 2904 7273 0000 00da 0a64 6973 6b5f 7573  ).rs.....disk_us
+00012b20: 6167 65da 0466 7265 6572 4e00 0000 2902  age..freerN...).
+00012b30: 7261 0000 005a 066d 696e 5f67 6272 1600  ra...Z.min_gbr..
+00012b40: 0000 7216 0000 0072 1700 0000 da0b 7370  ..r....r......sp
+00012b50: 6163 655f 6368 6563 6b7c 0c00 0073 1200  ace_check|...s..
+00012b60: 0000 0001 0401 02ff 0401 02ff 0201 02ff  ................
+00012b70: 0601 02ff 72a9 0200 0029 0172 1800 0000  ....r....).r....
+00012b80: 2902 4672 0100 0000 2902 4672 0100 0000  ).Fr....).Fr....
+00012b90: 2902 4672 0100 0000 2902 4672 0100 0000  ).Fr....).Fr....
+00012ba0: 2902 4672 0100 0000 2903 7282 0000 0054  ).Fr....).r....T
+00012bb0: 4e29 054e 4e4e 464e 2901 4e29 014e 2901  N).NNNFN).N).N).
+00012bc0: 4e29 0372 1f01 0000 7220 0100 0072 d400  N).r....r ...r..
+00012bd0: 0000 2902 7228 0100 0072 1f01 0000 2901  ..).r(...r....).
+00012be0: 7228 0100 0029 0172 2e00 0000 2901 729a  r(...).r....).r.
+00012bf0: 0000 0029 014e 2901 725c 0100 0029 054e  ...).N).r\...).N
+00012c00: 5446 726c 0100 0072 2301 0000 2901 727a  TFrl...r#...).rz
+00012c10: 0100 0029 0772 4700 0000 4e54 464e 5454  ...).rG...NTFNTT
+00012c20: 2901 5429 0146 2902 4672 0100 0000 2901  ).T).F).Fr....).
+00012c30: 72d9 0000 0029 0246 5429 014e 2903 72d4  r....).FT).N).r.
+00012c40: 0000 004e 4629 044e 4646 72df 0100 0029  ...NF).NFFr....)
+00012c50: 0454 4646 72df 0100 0029 0454 4646 72df  .TFFr....).TFFr.
+00012c60: 0100 0029 0172 2e00 0000 2901 5429 0172  ...).r....).T).r
+00012c70: d400 0000 2901 4629 0146 2901 4629 0272  ....).F).F).F).r
+00012c80: 3102 0000 7282 0000 0029 0172 0100 0000  1...r....).r....
+00012c90: 2902 7247 0000 0072 0100 0000 2904 7268  ).rG...r....).rh
+00012ca0: 0200 0072 0100 0000 5446 2905 7201 0000  ...r....TF).r...
+00012cb0: 0072 0100 0000 5446 4e29 0146 2901 4629  .r....TFN).F).F)
+00012cc0: 0172 7902 0000 2901 729c 0000 0029 0272  .ry...).r....).r
+00012cd0: 9c00 0000 722e 0000 0029 0672 d400 0000  ....r....).r....
+00012ce0: 4e46 4646 4629 0172 6402 0000 2901 4e29  NFFFF).rd...).N)
+00012cf0: 0172 4700 0000 29a6 5a13 7768 6163 632e  .rG...).Z.whacc.
+00012d00: 6665 6174 7572 655f 6d61 6b65 7272 0200  feature_makerr..
+00012d10: 0000 7203 0000 005a 1277 6861 6363 2e70  ..r....Z.whacc.p
+00012d20: 6f6c 655f 7472 6163 6b65 7272 0400 0000  ole_trackerr....
+00012d30: 72c0 0100 0072 0500 0000 7273 0000 00da  r....r....rs....
+00012d40: 056e 756d 7079 721d 0000 0072 5f00 0000  .numpyr....r_...
+00012d50: da03 7379 7372 b301 0000 5a07 6e61 7473  ..sysr....Z.nats
+00012d60: 6f72 7472 0600 0000 7207 0000 005a 0873  ortr....r....Z.s
+00012d70: 6369 7079 2e69 6fda 0269 6f72 1a02 0000  cipy.io..ior....
+00012d80: 72ae 0000 00da 116d 6174 706c 6f74 6c69  r......matplotli
+00012d90: 622e 7079 706c 6f74 da06 7079 706c 6f74  b.pyplot..pyplot
+00012da0: 7211 0000 005a 0670 616e 6461 7372 9f01  r....Z.pandasr..
+00012db0: 0000 721b 0000 0072 9a01 0000 7208 0000  ..r....r....r...
+00012dc0: 0072 8702 0000 7289 0200 005a 0c73 6369  .r....r....Z.sci
+00012dd0: 7079 2e73 6967 6e61 6c72 0900 0000 720a  py.signalr....r.
+00012de0: 0000 0072 bb01 0000 5a11 7471 646d 2e61  ...r....Z.tqdm.a
+00012df0: 7574 6f6e 6f74 6562 6f6f 6b72 0b00 0000  utonotebookr....
+00012e00: 720d 0000 0072 0c00 0000 727b 0100 0072  r....r....r{...r
+00012e10: 8f00 0000 72c6 0000 00da 0770 6174 686c  ....r......pathl
+00012e20: 6962 720e 0000 00da 0e75 726c 6c69 622e  ibr......urllib.
+00012e30: 7265 7175 6573 7472 7500 0000 da07 7a69  requestru.....zi
+00012e40: 7066 696c 6572 0f00 0000 7210 0000 0072  pfiler....r....r
+00012e50: 2d00 0000 7244 0000 0072 5400 0000 7258  -...rD...rT...rX
+00012e60: 0000 0072 5d00 0000 724c 0000 0072 6c00  ...r]...rL...rl.
+00012e70: 0000 727f 0000 0072 5b00 0000 725a 0000  ..r....r[...rZ..
+00012e80: 0072 5900 0000 7294 0000 0072 c500 0000  .rY...r....r....
+00012e90: 72ce 0000 0072 8e00 0000 72dc 0000 0072  r....r....r....r
+00012ea0: e000 0000 72df 0000 0072 e800 0000 72f1  ....r....r....r.
+00012eb0: 0000 0072 4d00 0000 720a 0100 0072 0c01  ...rM...r....r..
+00012ec0: 0000 7211 0100 0072 0e01 0000 7212 0100  ..r....r....r...
+00012ed0: 0072 1401 0000 72b3 0000 0072 2701 0000  .r....r....r'...
+00012ee0: 722b 0100 0072 2d01 0000 7237 0100 0072  r+...r-...r7...r
+00012ef0: 5201 0000 7254 0100 0072 7400 0000 729e  R...rT...rt...r.
+00012f00: 0000 0072 5b01 0000 72b1 0000 0072 aa00  ...r[...r....r..
+00012f10: 0000 7265 0100 0072 6a01 0000 726b 0100  ..re...rj...rk..
+00012f20: 0072 7301 0000 7279 0100 0072 8301 0000  .rs...ry...r....
+00012f30: 72a2 0100 0072 a701 0000 72a4 0100 0072  r....r....r....r
+00012f40: b501 0000 72b7 0100 0072 9d01 0000 7263  ....r....r....rc
+00012f50: 0000 0072 5e00 0000 72c3 0100 0072 1a00  ...r^...r....r..
+00012f60: 0000 72c4 0100 0072 c901 0000 72ca 0100  ..r....r....r...
+00012f70: 0072 ab00 0000 72d0 0100 00da 066f 626a  .r....r......obj
+00012f80: 6563 7472 da01 0000 72de 0100 0072 7801  ectr....r....rx.
+00012f90: 0000 7200 0200 0072 7401 0000 723b 0000  ..r....rt...r;..
+00012fa0: 0072 2901 0000 7207 0200 0072 cb01 0000  .r)...r....r....
+00012fb0: 7211 0200 0072 1802 0000 7296 0100 0072  r....r....r....r
+00012fc0: 1b02 0000 721c 0200 0072 2002 0000 7229  ....r....r ...r)
+00012fd0: 0200 0072 2c02 0000 7237 0000 0072 3002  ...r,...r7...r0.
+00012fe0: 0000 7235 0200 0072 3b02 0000 723f 0200  ..r5...r;...r?..
+00012ff0: 0072 4602 0000 7249 0200 0072 4c02 0000  .rF...rI...rL...
+00013000: 729c 0100 0072 4f02 0000 7250 0200 0072  r....rO...rP...r
+00013010: 5602 0000 7263 0200 0072 6502 0000 7267  V...rc...re...rg
+00013020: 0200 0072 6d02 0000 726e 0200 0072 7002  ...rm...rn...rp.
+00013030: 0000 724e 0100 0072 7302 0000 7275 0200  ..rN...rs...ru..
+00013040: 0072 7702 0000 7257 0000 0072 7e02 0000  .rw...rW...r~...
+00013050: 7282 0200 0072 8402 0000 728b 0200 0072  r....r....r....r
+00013060: 8f02 0000 7291 0200 0072 9302 0000 7299  ....r....r....r.
+00013070: 0100 0072 9b02 0000 729d 0200 0072 7501  ...r....r....ru.
+00013080: 0000 726d 0100 0072 4c01 0000 7222 0100  ..rm...rL...r"..
+00013090: 0072 a302 0000 72a6 0200 0072 a902 0000  .r....r....r....
+000130a0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000130b0: 1700 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000130c0: 0000 7350 0100 0010 010c 010c 0108 0208  ..sP............
+000130d0: 0108 0108 0108 0110 010c 0108 010c 0108  ................
+000130e0: 0208 0108 010c 0108 0108 0108 0110 0108  ................
+000130f0: 010c 0210 0108 0108 0108 020c 0108 010c  ................
+00013100: 1808 040c 1208 1714 2408 090c 0b08 0d08  ........$.......
+00013110: 0c0c 140c 160c 160c 160c 1d00 0100 0000  ................
+00013120: 0002 ff0a 6508 2508 0608 050c 5308 0408  ....e.%.....S...
+00013130: 0908 090c 4f08 2d08 5408 0408 0708 040c  ....O.-.T.......
+00013140: 0d08 1d0c 0f0c 0c0c 1a0c 370c 2e08 0508  ..........7.....
+00013150: 050c 0b14 160c 0808 0408 0508 0808 0b00  ................
+00013160: 0100 0002 ff0a 1708 190c 0800 0100 0000  ................
+00013170: 0100 0000 0102 fd0a 7f00 7f00 220c 180c  ............"...
+00013180: 7c0c 2c08 0608 0608 0508 0508 0708 0a0c  |.,.............
+00013190: 1508 1608 080c 090c 0c12 4708 290c 480c  ..........G.).H.
+000131a0: 3e0c 5b0c 2a0c 1508 1708 0f08 1208 1b08  >.[.*...........
+000131b0: 130c 2a08 1908 1308 160c 1008 140c 310c  ..*...........1.
+000131c0: 1d0c 4508 2f0c 1e0c 1d08 1608 0f08 2808  ..E./.........(.
+000131d0: 0908 1208 1f08 3308 3608 040c 1408 0b00  ......3.6.......
+000131e0: 0102 ff0a 180c 0d08 0708 2708 0f0c 170c  ..........'.....
+000131f0: 0b14 0f08 0a08 0a08 080c 090c 080c 0a00  ................
+00013200: 0100 0000 0002 ff0e 3a10 180c 0d0c 040c  ........:.......
+00013210: 0610 090c 040c 05                        .......
```

### Comparing `whacc-1.3.8/whacc/analysis.py` & `whacc-1.3.9/whacc/analysis.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/0.5 before batch processing.py` & `whacc-1.3.9/whacc/examples/0.5 before batch processing.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/1_make_h5_example.py` & `whacc-1.3.9/whacc/examples/1_make_h5_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/2_predict_touches_example.py` & `whacc-1.3.9/whacc/examples/2_predict_touches_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/3_make_subset_H5_example.py` & `whacc-1.3.9/whacc/examples/3_make_subset_H5_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/4_augment_H5_example.py` & `whacc-1.3.9/whacc/examples/4_augment_H5_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/5_split_data_for_retrain_example.py` & `whacc-1.3.9/whacc/examples/5_split_data_for_retrain_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/6_retrain_example.py` & `whacc-1.3.9/whacc/examples/6_retrain_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/7_select_TL_trials.py` & `whacc-1.3.9/whacc/examples/7_select_TL_trials.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/8_make_feature_data.py` & `whacc-1.3.9/whacc/examples/8_make_feature_data.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/9_re_train_GBM_EXAMPLE.py` & `whacc-1.3.9/whacc/examples/9_re_train_GBM_EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/CNN_+lightGBM_V5_Testing_GPU_RAM_limits_V2.py` & `whacc-1.3.9/whacc/examples/CNN_+lightGBM_V5_Testing_GPU_RAM_limits_V2.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/SCRATCH5.py` & `whacc-1.3.9/whacc/examples/SCRATCH5.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/TL_10_20_30.py` & `whacc-1.3.9/whacc/examples/TL_10_20_30.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/add_pole_times.py` & `whacc-1.3.9/whacc/examples/add_pole_times.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/best_T1V1t2_model.py` & `whacc-1.3.9/whacc/examples/best_T1V1t2_model.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/colors.py` & `whacc-1.3.9/whacc/examples/colors.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/compare_models_for_feature_selection.py` & `whacc-1.3.9/whacc/examples/compare_models_for_feature_selection.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/convert_h5_to_feature_h5.py` & `whacc-1.3.9/whacc/examples/convert_h5_to_feature_h5.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/copy_temp.py` & `whacc-1.3.9/whacc/examples/copy_temp.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/define_in_range.py` & `whacc-1.3.9/whacc/examples/define_in_range.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/diff_h5_creator.py` & `whacc-1.3.9/whacc/examples/diff_h5_creator.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/error_analysis_example.py` & `whacc-1.3.9/whacc/examples/error_analysis_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/final_CNN_performance_with_final_mathcing_datasets.py` & `whacc-1.3.9/whacc/examples/final_CNN_performance_with_final_mathcing_datasets.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/full_pipeline.py` & `whacc-1.3.9/whacc/examples/full_pipeline.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/full_pipeline_no_transfer_learning.py` & `whacc-1.3.9/whacc/examples/full_pipeline_no_transfer_learning.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/gists.py` & `whacc-1.3.9/whacc/examples/gists.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/h5_tester.py` & `whacc-1.3.9/whacc/examples/h5_tester.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/heat_map_plotter.py` & `whacc-1.3.9/whacc/examples/heat_map_plotter.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/heat_mapper_boost_mods.py` & `whacc-1.3.9/whacc/examples/heat_mapper_boost_mods.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/heatmap_maker.py` & `whacc-1.3.9/whacc/examples/heatmap_maker.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/load_all_predictions_from_all_100_final_models_for_cloud.py` & `whacc-1.3.9/whacc/examples/load_all_predictions_from_all_100_final_models_for_cloud.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/lstm_transfer_learning_lstm_using_subsets_v3.py` & `whacc-1.3.9/whacc/examples/lstm_transfer_learning_lstm_using_subsets_v3.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/make_master_training_H5_example.py` & `whacc-1.3.9/whacc/examples/make_master_training_H5_example.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/make_new_data_and train.py` & `whacc-1.3.9/whacc/examples/make_new_data_and train.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/pack_samsons_data.py` & `whacc-1.3.9/whacc/examples/pack_samsons_data.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/re_pole_down.py` & `whacc-1.3.9/whacc/examples/re_pole_down.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/redo_all_data.py` & `whacc-1.3.9/whacc/examples/redo_all_data.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/run_all_model.py` & `whacc-1.3.9/whacc/examples/run_all_model.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/scratch4.py` & `whacc-1.3.9/whacc/examples/scratch4.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/scratch8.py` & `whacc-1.3.9/whacc/examples/scratch8.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/scratch_3.py` & `whacc-1.3.9/whacc/examples/scratch_3.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/subset_to_altered_for_training.py` & `whacc-1.3.9/whacc/examples/subset_to_altered_for_training.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/temp_TVt1_and_TVt2_model_directories.py` & `whacc-1.3.9/whacc/examples/temp_TVt1_and_TVt2_model_directories.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/test_training_with_worst_trials.py` & `whacc-1.3.9/whacc/examples/test_training_with_worst_trials.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/testing_LSTM_model_defnitions.py` & `whacc-1.3.9/whacc/examples/testing_LSTM_model_defnitions.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/testing_batch_predicting.py` & `whacc-1.3.9/whacc/examples/testing_batch_predicting.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/examples/var_rename_scratch.py` & `whacc-1.3.9/whacc/examples/var_rename_scratch.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/feature_maker.py` & `whacc-1.3.9/whacc/feature_maker.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/feature_maker_temp.py` & `whacc-1.3.9/whacc/feature_maker_temp.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/FIG_2_border_touches_explained.py` & `whacc-1.3.9/whacc/figures/FIG_2_border_touches_explained.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/FIG_2_pie_graph_percentages.py` & `whacc-1.3.9/whacc/figures/FIG_2_pie_graph_percentages.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/FIG_2_pie_graph_percentages_V2.py` & `whacc-1.3.9/whacc/figures/FIG_2_pie_graph_percentages_V2.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/PSTH neuron compare.py` & `whacc-1.3.9/whacc/figures/PSTH neuron compare.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/PSTH_V1.py` & `whacc-1.3.9/whacc/figures/PSTH_V1.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/SHAP_histograms.py` & `whacc-1.3.9/whacc/figures/SHAP_histograms.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/__pycache__/pretty_plots.cpython-38.pyc` & `whacc-1.3.9/whacc/figures/__pycache__/pretty_plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/all agree analysis fig V2.py` & `whacc-1.3.9/whacc/figures/all agree analysis fig V2.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/all agree analysis.py` & `whacc-1.3.9/whacc/figures/all agree analysis.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/error_analysis_explained_critical_errors.py` & `whacc-1.3.9/whacc/figures/error_analysis_explained_critical_errors.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/error_type_analysis.py` & `whacc-1.3.9/whacc/figures/error_type_analysis.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/features_with_video.py` & `whacc-1.3.9/whacc/figures/features_with_video.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/fig_3_model_compare.py` & `whacc-1.3.9/whacc/figures/fig_3_model_compare.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/fig_3_model_compare_V2.py` & `whacc-1.3.9/whacc/figures/fig_3_model_compare_V2.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/get_feature_names.py` & `whacc-1.3.9/whacc/figures/get_feature_names.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/load/load.py` & `whacc-1.3.9/whacc/figures/load/load.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/not_using/simulation_simple.py` & `whacc-1.3.9/whacc/figures/not_using/simulation_simple.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/pretty_plots.py` & `whacc-1.3.9/whacc/figures/pretty_plots.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/what_features_look_like.py` & `whacc-1.3.9/whacc/figures/what_features_look_like.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/figures/whisker_images.py` & `whacc-1.3.9/whacc/figures/whisker_images.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/image_tools.py` & `whacc-1.3.9/whacc/image_tools.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/model_maker.py` & `whacc-1.3.9/whacc/model_maker.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/pole_tracker.py` & `whacc-1.3.9/whacc/pole_tracker.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/retrain_LGBM.py` & `whacc-1.3.9/whacc/retrain_LGBM.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/run_in_terminal_template.py` & `whacc-1.3.9/whacc/run_in_terminal_template.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/subset_h5_generator.py` & `whacc-1.3.9/whacc/subset_h5_generator.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/touch_curation_GUI.py` & `whacc-1.3.9/whacc/touch_curation_GUI.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/transfer_learning.py` & `whacc-1.3.9/whacc/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/utils.py` & `whacc-1.3.9/whacc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     download_inds = _single_to_list_input_checker(download_inds, 3)
 
     download_resnet_model(overwrite[0], download_inds[0])
     download_training_data(overwrite[1], download_inds[1])
     download_extra_LGBM_models(overwrite[2], download_inds[2])
 
 
+
 def load_training_data():
     bd = get_whacc_path() + os.sep + '/whacc_data/training_data'
     if not os.path.isdir(bd):
         print('Auto downloading training data, this will only run once')
         download_training_data()
 
     tvt_x = load_obj(bd + os.sep + 'tvt_x.pkl')
@@ -169,17 +170,40 @@
 
 def download_data_dict():
     d = dict()
     d['resnet_model'] = ['https://www.dropbox.com/sh/knq6la5fcu73zk5/AABQuMmxm4msVbWIddl9x1v3a?dl=1',
                          'https://www.dropbox.com/s/k0398tchgk20lkv/final_resnet50V2_full_model.zip?dl=1']
     d['split_by_trial_2105_data'] = ['https://www.dropbox.com/sh/07uavloxi3ugnjy/AAABU4nsRkJJ4TtkBGxh7zIHa?dl=1']
     d['extra_LGBM_models'] = ['https://www.dropbox.com/sh/l5yuw3r2hqdhrw0/AABSq2L9265cWzAs6AgJOS9Va?dl=1']
+
+    d['example_MP4s'] = ['https://www.dropbox.com/sh/bv5wectlbugacef/AAAuueROhu_rHmMZjdVgGly_a?dl=1']
+
     return d
 
 
+def download_example_mp4s(dst, overwrite=False, link_ind=0):
+    d = download_data_dict()
+    filename = get_whacc_path() + os.sep + '/whacc_data/example_MP4s.zip'
+    if os.path.isdir(dst):
+        if overwrite:
+            shutil.rmtree(dst)
+        else:
+            print('example_MP4s are already downloaded, if you want to overwrite it set overwrite to True')
+            return
+    # make_path(dst)
+    print('downloading example_MP4s...')
+    url = d['example_MP4s'][link_ind]
+    urllib.request.urlretrieve(url, filename)
+    with ZipFile(filename, 'r') as zipObj:
+        print('unzipping file ...')
+        zipObj.extractall(path=dst)
+    print('deleting zip file ...')
+    os.remove(filename)
+    print('Done')
+
 def download_extra_LGBM_models(overwrite_model=False, link_ind=0):
     d = download_data_dict()
     filename = get_whacc_path() + os.sep + '/whacc_data/final_model/extra_LGBM_models.zip'
     dst = filename[:-4]
     if os.path.isdir(dst):
         if overwrite_model:
             shutil.rmtree(dst)
```

### Comparing `whacc-1.3.8/whacc/whacc_data/.DS_Store` & `whacc-1.3.9/whacc/whacc_data/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 000011e0: 5369 6465 6261 7208 0909 0909 5f10 187b  Sidebar....._..{
 000011f0: 7b35 3135 2c20 3239 397d 2c20 7b39 3230  {515, 299}, {920
 00001200: 2c20 3436 347d 7d09 0817 2531 3d49 606d  , 464}}...%1=I`m
 00001210: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 00001220: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00001230: 0000 0000 0000 9a00 0000 0b00 6600 6900  ............f.i.
 00001240: 6e00 6100 6c00 5f00 6d00 6f00 6400 6500  n.a.l._.m.o.d.e.
-00001250: 6c64 7363 6c62 6f6f 6c01 0000 000b 0066  ldsclbool......f
+00001250: 6c64 7363 6c62 6f6f 6c00 0000 000b 0066  ldsclbool......f
 00001260: 0069 006e 0061 006c 005f 006d 006f 0064  .i.n.a.l._.m.o.d
 00001270: 0065 006c 6c73 7643 626c 6f62 0000 0307  .e.llsvCblob....
 00001280: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
 00001290: 0809 0a0b 1956 570a 595f 1012 7669 6577  .....VW.Y_..view
 000012a0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 000012b0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 000012c0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
```

### Comparing `whacc-1.3.8/whacc/whacc_data/feature_data/feature_data_dict.pkl` & `whacc-1.3.9/whacc/whacc_data/feature_data/feature_data_dict.pkl`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/feature_data/start_end_nan_locations.pkl` & `whacc-1.3.9/whacc/whacc_data/feature_data/start_end_nan_locations.pkl`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/final_model/.DS_Store` & `whacc-1.3.9/whacc/whacc_data/final_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/final_model/final_resnet50V2_HEAD/final_CNN_model_head.pkl` & `whacc-1.3.9/whacc/whacc_data/final_model/final_resnet50V2_HEAD/final_CNN_model_head.pkl`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/final_model/light_GBM_model/.DS_Store` & `whacc-1.3.9/whacc/whacc_data/final_model/light_GBM_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/final_model/light_GBM_model/FINAL_WHACC_MODEL_016_model.pkl` & `whacc-1.3.9/whacc/whacc_data/final_model/light_GBM_model/FINAL_WHACC_MODEL_016_model.pkl`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc/whacc_data/template_img.png` & `whacc-1.3.9/whacc/whacc_data/template_img.png`

 * *Files identical despite different names*

### Comparing `whacc-1.3.8/whacc.egg-info/PKG-INFO` & `whacc-1.3.9/whacc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whacc
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automatic and customizable pipeline for creating a CNN + light GBM model to predict whiskers contacting objects
 Home-page: https://github.com/hireslab/whacc
 Author: Phillip Maire
 Author-email: phillip.maire@gmail.com
 License: MIT
 Description: ![](./pictures/whacc-logo-v1.png) <br />
         
@@ -15,27 +15,32 @@
         ## [Walkthrough: Google CoLab](https://colab.research.google.com/drive/1pgdpc0IWkce07Sto6AolQTGoXKCW_mes?authuser=1&pli=1#scrollTo=UAIbs6IlTTfj)  
         
         ![](./pictures/trial_animation.gif) <br />
         *Single example trial lasting 4 seconds. Example video (left) along with whisker traces, decomposed components, and spikes recorded from L5 (right). How do we identify the precise millisecond frame when touch occurs?*
         
         
         ## Flow diagram of WhACC video pre-processing and design implementation
-        ![](./pictures/WhACC figure 1.png) <br />
+        
+        ![](./pictures/WhACC_figure_1.png) <br />
         
         ## Touch frame scoring and variation in human curation
-        ![](./pictures/WhACC figure 2.png) <br />
+        
+        ![](./pictures/WhACC_figure_2.png) <br />
         
         ## Feature engineering and selection
-        ![](./pictures/WhACC figure 3.png) <br />
+        
+        ![](./pictures/WhACC_figure_3.png) <br />
         
         ## Data selection and model performance
-        ![](./pictures/WhACC figure 4.png) <br />
+        
+        ![](./pictures/WhACC_figure_4.png) <br />
         
         ## WhACC shows expert human level performance
-        ![](./pictures/WhACC figure 5.png) <br />
+        
+        ![](./pictures/WhACC_figure_5.png) <br />
         
         
         ## Code contributors:
         WhACC code and software was originally developed by Phillip Maire and Jonathan Cheung in the laboratory of [Samuel Andrew Hires](https://www.hireslab.org/). 
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whacc-1.3.8/whacc.egg-info/SOURCES.txt` & `whacc-1.3.9/whacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

