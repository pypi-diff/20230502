# Comparing `tmp/Simba-UW-tf-dev-1.58.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.58.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.3.tar", last modified: Mon May  1 12:55:01 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.4.tar", last modified: Mon May  1 23:52:58 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.58.3.tar` & `Simba-UW-tf-dev-1.58.4.tar`

### file list

```diff
@@ -1,477 +1,478 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:49.000000 Simba-UW-tf-dev-1.58.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9311 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15058 2023-04-30 14:52:21.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5064 2023-04-29 19:45:45.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12964 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5996 2023-04-28 23:45:44.000000 Simba-UW-tf-dev-1.58.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12639 2023-04-30 13:53:26.000000 Simba-UW-tf-dev-1.58.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10867 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13243 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/ui/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)    33818 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20642 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3419 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9955 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41575 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    36868 2023-05-01 00:37:11.000000 Simba-UW-tf-dev-1.58.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2335 2023-04-28 17:41:31.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    40521 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    14760 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    22224 2023-04-29 19:18:55.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60505 2023-04-30 15:39:23.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6161 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55308 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16894 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7588 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12048 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    17740 2023-04-29 19:49:25.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15283 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11588 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    19886 2023-04-30 16:53:25.000000 Simba-UW-tf-dev-1.58.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    33751 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14068 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.3/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8347 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9092 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10173 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8563 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12304 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    16589 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15891 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-04-30 15:51:37.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5754 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12242 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11210 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15137 2023-04-30 15:05:27.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9888 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2023-04-30 14:48:28.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13133 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8979 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8267 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6329 2023-04-28 18:51:08.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7407 2023-04-28 19:12:39.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12856 2023-05-01 12:53:36.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4821 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16794 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9551 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18464 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.3/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6503 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19691 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_csv_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6450 2023-04-30 20:37:02.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    24450 2023-05-01 11:05:08.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    41580 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65162 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18198 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-01 12:55:00.000000 Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.3/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-01 12:54:43.000000 Simba-UW-tf-dev-1.58.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-01 12:55:01.000000 Simba-UW-tf-dev-1.58.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:49.000000 Simba-UW-tf-dev-1.58.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9311 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15058 2023-04-30 14:52:21.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5064 2023-04-29 19:45:45.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12964 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5996 2023-04-28 23:45:44.000000 Simba-UW-tf-dev-1.58.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10867 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13243 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/ui/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)    33818 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    20642 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3419 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9955 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41575 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    36868 2023-05-01 00:37:11.000000 Simba-UW-tf-dev-1.58.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2335 2023-04-28 17:41:31.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    40521 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    22224 2023-04-29 19:18:55.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60505 2023-04-30 15:39:23.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6161 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.4/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16894 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12198 2023-05-01 19:31:25.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11588 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    19886 2023-04-30 16:53:25.000000 Simba-UW-tf-dev-1.58.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    33751 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14068 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.4/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8347 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9092 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10173 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8563 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12304 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    16589 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15891 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-04-30 15:51:37.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5754 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12242 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11210 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15137 2023-04-30 15:05:27.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9888 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2023-04-30 14:48:28.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13133 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8979 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8267 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6329 2023-04-28 18:51:08.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7407 2023-04-28 19:12:39.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12822 2023-05-01 13:08:33.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4821 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16794 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9551 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18624 2023-05-01 20:34:07.000000 Simba-UW-tf-dev-1.58.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.4/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6503 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19691 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/sleap_csv_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    41580 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65306 2023-05-01 20:29:10.000000 Simba-UW-tf-dev-1.58.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18244 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-01 23:52:57.000000 Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.4/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-01 23:52:54.000000 Simba-UW-tf-dev-1.58.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-01 23:52:58.000000 Simba-UW-tf-dev-1.58.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.58.3/PKG-INFO` & `Simba-UW-tf-dev-1.58.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.3
+Version: 1.58.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/create_project_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,20 @@
 
 class ProjectCreatorPopUp(PopUpMixin):
     """
     Creates tkinter GUI pop-up window accepting user-input for generating SimBA project.
     """
 
     def __init__(self):
-        PopUpMixin.__init__(self, title="PROJECT CONFIGURATION", size=(750, 750))
+
+        self.main_frm = Toplevel()
+        self.main_frm.minsize(750, 750)
+        self.main_frm.wm_title("PROJECT CONFIGURATION")
+        self.main_frm.columnconfigure(0, weight=1)
+        self.main_frm.rowconfigure(0, weight=1)
         parent_tab = ttk.Notebook(hxtScrollbar(self.main_frm))
         self.btn_icons = get_icons_paths()
         for k in self.btn_icons.keys():
             self.btn_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname(__file__), self.btn_icons[k]['icon_path'])))
         self.create_project_tab = ttk.Frame(parent_tab)
         self.import_videos_tab = ttk.Frame(parent_tab)
         self.import_data_tab = ttk.Frame(parent_tab)
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/setting_menu.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.58.4/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.58.4/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.58.4/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.58.4/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.58.4/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.58.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.58.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.58.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/pose_importer_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 from datetime import datetime
 import cv2
 from numba import jit, prange
 import numpy as np
 from copy import deepcopy
 from collections import defaultdict
 import itertools
+import scipy.io as sio
+import h5py
+
 
 import pandas as pd
 
-from simba.utils.errors import NoDataError, NoFilesFoundError, IntegerError, InvalidInputError
+from simba.utils.errors import NoDataError, NoFilesFoundError, IntegerError, InvalidInputError, CountError
 from simba.utils.read_write import get_fn_ext
 
 class PoseImporterMixin(object):
     def __init__(self):
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         pass
 
@@ -229,28 +232,77 @@
             click_n, click_n1 = click_key_combination[0], click_key_combination[1]
             animal_1, animal_2 = self.animal_order[click_n]['animal_name'], self.animal_order[click_n1]['animal_name']
             if animal_1 == animal_2:
                 raise InvalidInputError(msg=f'The animal most proximal to click number {str(click_n)} is animal named {animal_1}. The animal most proximal to click number {str(click_n1)} is also animal {animal_2}.'
                       'Please indicate which animal is which using a video frame where the animals are clearly separated')
 
 
+    def intertwine_probability_cols(self,
+                                    data: pd.DataFrame) -> pd.DataFrame:
+        results = pd.DataFrame()
+        for animal_name, animal_bps in self.animal_bp_dict.items():
+            x_cols, y_cols, p_cols = animal_bps['X_bps'], animal_bps['Y_bps'], animal_bps['P_bps']
+            for x_col, y_col, p_col in zip(x_cols, y_cols, p_cols):
+                df = data[[x_col, y_col, p_col]]
+                results = pd.concat([results, df], axis=1)
+        return results
+
+
     @staticmethod
     @jit(nopython=True)
     def transpose_multi_animal_table(data: np.array, idx: np.array, animal_cnt: int) -> np.array:
         results = np.full((np.max(idx[:, 1]), data.shape[1]*animal_cnt), 0.0)
         for i in prange(np.max(idx[:, 1])):
             for j in prange(animal_cnt):
                 data_idx = np.argwhere((idx[:, 0] == j) & (idx[:, 1] == i)).flatten()
                 if len(data_idx) == 1:
                     animal_frm_data = data[data_idx[0]]
                 else:
                     animal_frm_data = np.full((data.shape[1]), 0.0)
                 results[i][j*animal_frm_data.shape[0]:j*animal_frm_data.shape[0]+animal_frm_data.shape[0]] = animal_frm_data
         return results
 
+    def read_apt_trk_file(self,
+                          file_path: str):
+        print('Reading data using scipy.io...')
+        try:
+            trk_coordinates = sio.loadmat(file_path)['pTrk']
+            track_cnt = trk_coordinates.shape[3]
+            data = [trk_coordinates[..., i] for i in range(track_cnt)]
+
+        except NotImplementedError:
+            print('Failed to read data using scipy.io. Reading data using h5py...')
+            with h5py.File(file_path, 'r') as trk_dict:
+                trk_list = list(trk_dict['pTrk'])
+                t_second = np.array(trk_list)
+                if len(t_second.shape) > 3:
+                    t_third = np.swapaxes(t_second, 0, 3)
+                    trk_coordinates = np.swapaxes(t_third, 1, 2)
+                    track_cnt = trk_coordinates.shape[3]
+                    data = [trk_coordinates[..., i] for i in range(track_cnt)]
+                else:
+                    data = np.swapaxes(t_second, 0, 2)
+                    track_cnt = 1
+        if track_cnt != self.animal_cnt:
+            raise CountError(msg=f'There are {str(track_cnt)} tracks in the .trk file {file_path}. But your SimBA project expects {str(self.animal_cnt)} tracks.')
+
+        if self.animal_cnt != 1:
+            animal_df_lst = []
+            for animal in data:
+                m, n, r = animal.shape
+                out_arr = np.column_stack((np.repeat(np.arange(m), n), animal.reshape(m * n, -1)))
+                animal_df_lst.append(pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True))
+                self.data_df = pd.concat(animal_df_lst, axis=1).fillna(0).astype(np.int)
+        else:
+            m, n, r = data.shape
+            out_arr = np.column_stack((np.repeat(np.arange(m), n), data.reshape(m * n, -1)))
+            self.data_df = pd.DataFrame(out_arr).T.iloc[1:].reset_index(drop=True).astype(np.int)
+
+        p_cols = pd.DataFrame(1, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
+        return pd.concat([self.data_df, p_cols], axis=1) #.sort_index(axis=1)
 
 
 
 
     # def import_log(self):
     #     self.import_log = pd.DataFrame(columns=['VIDEO', 'IMPORT_TIME', 'IMPORT_SOURCE', 'INTERPOLATION_SETTING', 'SMOOTHING_SETTING'])
     #
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.58.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.58.4/simba/mixins/train_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
 
-from simba.utils.enums import ConfigKey, Dtypes, MetaKeys
+from simba.utils.enums import ConfigKey, Dtypes, MetaKeys, Defaults
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
 from simba.utils.data import detect_bouts, create_color_palette
 from simba.utils.read_write import find_core_cnt, get_memory_usage_of_df, read_config_entry, read_df, get_fn_ext
 from simba.utils.checks import (check_int,
                                 check_str,
                                 check_if_dir_exists,
                                 check_float)
@@ -780,16 +780,17 @@
                       ["Max features", model_dict[MetaKeys.RF_MAX_FEATURES.value]],
                       ["Under sampling setting", model_dict[ConfigKey.UNDERSAMPLE_SETTING.value]],
                       ["Under sampling ratio", model_dict[ConfigKey.UNDERSAMPLE_RATIO.value]],
                       ["Over sampling setting", model_dict[ConfigKey.OVERSAMPLE_SETTING.value]],
                       ["Over sampling ratio", model_dict[ConfigKey.OVERSAMPLE_RATIO.value]],
                       ["criterion", model_dict[MetaKeys.CRITERION.value]],
                       ["Min sample leaf", model_dict[MetaKeys.MIN_LEAF.value]]]
-        headers = ["Setting", "value"]
-        print(tabulate(table_view, headers, tablefmt="grid"))
+        table = tabulate(table_view, ["Setting", "value"], tablefmt="grid")
+        print(f'{table} {Defaults.STR_SPLIT_DELIMITER.value}TABLE')
+
 
     def create_meta_data_csv_training_one_model(self,
                                                 meta_data_lst: list,
                                                 clf_name: str,
                                                 save_dir: str):
         """
         Helper to save single model meta data (hyperparameters, sampling settings etc.) into SimBA
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def __init__(self,
                  config_path: str,
                  pre_window: int,
                  post_window: int,
                  cue_light_names: list,
                  clf_list: list):
 
-        ConfigReader.__init__(config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
         self.pre_window, self.post_window = pre_window, post_window
         self.cue_light_names = cue_light_names
         self.clf_list = clf_list
         self.project_path = read_config_entry(self.config, 'General settings', 'project_path', data_type='folder_path')
         self.cue_light_data_dir = os.path.join(self.project_path, 'csv', 'cue_lights')
         self.machine_results_dir = os.path.join(self.project_path, 'csv', 'machine_results')
         self.no_animals = read_config_entry(self.config, 'General settings', 'animal_no', 'int')
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import time
 import platform
 from simba.utils.read_write import read_df, write_df, get_fn_ext, find_video_of_file, get_video_meta_data, find_core_cnt
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.errors import NoFilesFoundError, CountError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
+from simba.utils.warnings import NoDataFoundWarning
 
 
 
 
 def get_intensity_scores_in_rois(frm_list: list=None,
                                  video_path: str = None,
                                  rectangles_df: pd.DataFrame = None,
@@ -85,15 +86,15 @@
 
     def __init__(self,
                  config_path: str,
                  in_dir: str,
                  cue_light_names: list):
 
 
-        ConfigReader.__init__(config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
 
         if len(cue_light_names) == 0:
             raise CountError(msg='SIMBA ERROR: Please select one or more cue lights')
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
         self.out_dir = os.path.join(self.project_path, 'csv', 'cue_lights')
@@ -158,18 +159,21 @@
             video_settings, pix_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
             self.video_recs = self.rectangles_df.loc[(self.rectangles_df['Video'] == self.video_name) & (self.rectangles_df['Name'].isin(self.cue_light_names))]
             self.video_circs = self.circles_df.loc[(self.circles_df['Video'] == self.video_name)  & (self.circles_df['Name'].isin(self.cue_light_names))]
             self.video_polys = self.polygon_df.loc[(self.polygon_df['Video'] == self.video_name) & (self.polygon_df['Name'].isin(self.cue_light_names))]
             self.shape_names = list(itertools.chain(self.rectangles_df['Name'].unique(), self.circles_df['Name'].unique(),self.polygon_df['Name'].unique()))
             self.video_path = find_video_of_file(self.video_dir, self.video_name)
             self.video_meta_data = get_video_meta_data(self.video_path)
+            if len(self.video_recs) + len(self.video_circs) + len(self.video_polys) == 0:
+                NoDataFoundWarning(msg=f'No roi data found for video {self.video_name}. Skipping analysis of {self.video_name}...')
+                continue
+
+
 
-            #self.frm_lst = list(range(0, len(self.data_df), 1))
             self.frm_lst = list(range(0, self.video_meta_data['frame_count'], 1))
-            #self.frame_chunks = np.array_split(self.frm_lst, len(self.data_df) / self.fps)
             self.frame_chunks = np.array_split(self.frm_lst, int(self.video_meta_data['frame_count'] / self.fps))
             imgs_peer_loop = len(self.frame_chunks[0])
             self.intensity_results = {}
 
             with multiprocessing.pool.Pool(self.cpu_cnt_to_use, maxtasksperchild=self.maxtasksperchild) as pool:
                 functools.partial(get_intensity_scores_in_rois, b=self.video_recs, c=self.circles_df, d=self.video_polys)
                 constants = functools.partial(get_intensity_scores_in_rois,
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from simba.utils.checks import check_float, check_int
 from simba.utils.read_write import get_fn_ext, find_video_of_file, get_all_clf_names, read_config_entry
 from simba.cue_light_tools.cue_light_analyzer import CueLightAnalyzer
 from simba.cue_light_tools.cue_light_visualizer import CueLightVisualizer
 from simba.cue_light_tools.cue_light_clf_statistics import CueLightClfAnalyzer
 from simba.cue_light_tools.cue_light_movement_statistics import CueLightMovementAnalyzer
 from simba.utils.errors import NoFilesFoundError, CountError, NoROIDataError, NoChoosenClassifierError
-from simba.ui.tkinter_functions import hxtScrollbar, CreateLabelFrameWithIcon
+from simba.ui.tkinter_functions import CreateLabelFrameWithIcon
 from simba.utils.enums import Keys, Links
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.pop_up_mixin import PopUpMixin
 import webbrowser
 
 
-class CueLightAnalyzerMenu(ConfigReader):
+class CueLightAnalyzerMenu(ConfigReader, PopUpMixin):
     """
     Class for lunching cue light analysis GUI in SimBA.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
@@ -42,32 +43,29 @@
 
     def __init__(self,
                  config_path: str):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.data_dir = os.path.join(self.project_path, 'csv', 'outlier_corrected_movement_location')
         self.cue_light_data_folder = os.path.join(self.project_path, 'csv', 'cue_lights')
-        self.__read_roi_dfs()
+        self.read_roi_data()
         if len(self.shape_names) == 0:
             raise CountError(msg='SIMBA ERROR: Cue light analysis require ROI definitions. Please define ROIs before doing cue light analysis')
-        self.cue_light_main_frame = Toplevel()
-        self.cue_light_main_frame.minsize(750, 300)
-        self.cue_light_main_frame.wm_title("SIMBA CUE LIGHT ANALYZER")
-        self.cue_light_main_frame.lift()
+        PopUpMixin.__init__(self, size=(750, 300), title="SIMBA CUE LIGHT ANALYZER")
         self.lights_dict = {}
 
-        self.cue_light_settings_frm = CreateLabelFrameWithIcon(parent=self.cue_light_main_frame, header='DEFINE CUE LIGHTS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.CUE_LIGHTS.value)
+        self.cue_light_settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='DEFINE CUE LIGHTS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.CUE_LIGHTS.value)
         self.choose_lights_cnt_lbl = Label(self.cue_light_settings_frm, text='# Cue lights', width=10, anchor=W)
         self.choose_lights_cnt_var = IntVar()
         self.choose_lights_cnt_var.set(1)
         self.choose_lights_cnt_dropdown = OptionMenu(self.cue_light_settings_frm, self.choose_lights_cnt_var, *list(range(1, len(self.shape_names) + 1)), command=self.__create_cue_light_menus)
         self.cue_light_settings_frm.grid(row=0, sticky=NW)
         self.choose_lights_cnt_lbl.grid(row=0, column=0, sticky=W)
         self.choose_lights_cnt_dropdown.grid(row=0, column=1, sticky=W)
-        self.analyze_data_frm = LabelFrame(self.cue_light_main_frame, text='ANALYZE', font=('Helvetica', 15, 'bold'), pady=5, padx=15)
+        self.analyze_data_frm = LabelFrame(self.main_frm, text='ANALYZE', font=('Helvetica', 15, 'bold'), pady=5, padx=15)
         self.analyze_cue_light_data_btn = Button(self.analyze_data_frm, text='Analyze cue light data', command=lambda: self.__analyze_cue_light_data())
         self.visualize_cue_light_data_btn = Button(self.analyze_data_frm, text='Visualize cue light data', command=lambda: self.__visualize_cue_light_data())
         self.video_var = BooleanVar()
         self.frames_var = BooleanVar()
         self.video_check = Checkbutton(self.analyze_data_frm, text='Create videos', variable=self.video_var)
         self.frames_check = Checkbutton(self.analyze_data_frm, text='Create frames', variable=self.frames_var)
         self.analyze_movements_btn = Button(self.analyze_data_frm, text='Analyze cue light movement', command=lambda: self.__inititate_animal_movement_menu())
@@ -75,17 +73,17 @@
         self.analyze_data_frm.grid(row=0, column=1, sticky=NW)
         self.analyze_cue_light_data_btn.grid(row=0, column=0, sticky=W)
         self.visualize_cue_light_data_btn.grid(row=1, column=0, sticky=W)
         self.video_check.grid(row=1, column=1, sticky=W)
         self.frames_check.grid(row=1, column=2, sticky=W)
         self.analyze_movements_btn.grid(row=2, column=0, sticky=W)
         self.analyze_clf_btn.grid(row=3, column=0, sticky=W)
-        lbl_info_1 = Label(self.cue_light_main_frame, text='NOTE: Cue light analysis require ROI definitions')
-        lbl_info_2 = Label(self.cue_light_main_frame, text='[Click here to learn about cue light analysis]', cursor='hand2', fg='blue')
-        lbl_info_2.bind('<Button-1>', lambda e: webbrowser.open_new('https://github.com/sgoldenlab/simba/blob/master/docs/FSTTC.md'))
+        lbl_info_1 = Label(self.main_frm, text='NOTE: Cue light analysis require ROI definitions')
+        lbl_info_2 = Label(self.main_frm, text='[Click here to learn about cue light analysis]', cursor='hand2', fg='blue')
+        lbl_info_2.bind('<Button-1>', lambda e: webbrowser.open_new('https://github.com/sgoldenlab/simba/blob/master/docs/cue_light_tutorial.md'))
         lbl_info_1.grid(row=5, column=0, sticky=W)
         lbl_info_2.grid(row=6, column=0, sticky=W)
 
         mainloop()
 
     def __get_cue_light_names(self):
         self.light_lst = []
@@ -104,24 +102,14 @@
             self.lights_dict[light_cnt]['label'] = Label(self.cue_light_settings_frm, text='Cue light {}'.format(str(light_cnt+1)), width=10, anchor=W)
             self.lights_dict[light_cnt]['light_chosen'] = StringVar()
             self.lights_dict[light_cnt]['light_chosen'].set(self.shape_names[light_cnt])
             self.lights_dict[light_cnt]['dropdown'] = OptionMenu(self.cue_light_settings_frm, self.lights_dict[light_cnt]['light_chosen'], *self.shape_names, command=None)
             self.lights_dict[light_cnt]['label'].grid(row=current_row, column=0, sticky=W)
             self.lights_dict[light_cnt]['dropdown'].grid(row=current_row, column=1, sticky=W)
 
-    def __read_roi_dfs(self):
-        if not os.path.isfile(os.path.join(self.logs_path, 'measures', 'ROI_definitions.h5')):
-            raise NoROIDataError(msg='No ROI definitions were found in your SimBA project. Please draw some ROIs before analyzing your ROI data')
-        else:
-            self.roi_h5_path = os.path.join(self.logs_path, 'measures', 'ROI_definitions.h5')
-            self.rectangles_df = pd.read_hdf(self.roi_h5_path, key='rectangles')
-            self.circles_df = pd.read_hdf(self.roi_h5_path, key='circleDf')
-            self.polygon_df = pd.read_hdf(self.roi_h5_path, key='polygons')
-            self.shape_names = list(itertools.chain(self.rectangles_df['Name'].unique(), self.circles_df['Name'].unique(), self.polygon_df['Name'].unique()))
-
     def __analyze_cue_light_data(self):
         self.__get_cue_light_names()
         cue_light_analyzer = CueLightAnalyzer(config_path=self.config_path, in_dir=self.data_dir, cue_light_names=self.light_lst)
         cue_light_analyzer.analyze_files()
 
     def __visualize_cue_light_data(self):
         self.cue_light_data_files = glob.glob(self.cue_light_data_folder + '/*' + self.file_type)
@@ -153,24 +141,22 @@
                                                      command=self.__create_animal_bp_menues)
         self.animal_cnt_frm.grid(row=0, column=0, sticky=W)
         self.choose_animal_cnt_lbl.grid(row=0, column=0, sticky=W)
         self.choose_animal_cnt_dropdown.grid(row=0, column=1)
 
     def __create_animal_bp_menues(self, no_animals):
         self.animal_dict = {}
-        self.bp_names = self.get_body_part_names()[0]
-        self.bp_names = [x[0:-2] for x in self.bp_names]
         current_row = 0
         for animal_cnt in range(no_animals):
             self.animal_dict[animal_cnt] = {}
             current_row = 1 + animal_cnt
             self.animal_dict[animal_cnt]['label'] = Label(self.animal_cnt_frm, text='Animal {} body-part:'.format(str(animal_cnt+1)), width=17, anchor=W)
             self.animal_dict[animal_cnt]['bp_chosen'] = StringVar()
-            self.animal_dict[animal_cnt]['bp_chosen'].set(self.bp_names[animal_cnt])
-            self.animal_dict[animal_cnt]['dropdown'] = OptionMenu(self.animal_cnt_frm, self.animal_dict[animal_cnt]['bp_chosen'], *self.bp_names, command=None)
+            self.animal_dict[animal_cnt]['bp_chosen'].set(self.body_parts_lst[animal_cnt])
+            self.animal_dict[animal_cnt]['dropdown'] = OptionMenu(self.animal_cnt_frm, self.animal_dict[animal_cnt]['bp_chosen'], self.body_parts_lst, command=None)
             self.animal_dict[animal_cnt]['label'].grid(row=current_row, column=0, sticky=W)
             self.animal_dict[animal_cnt]['dropdown'].grid(row=current_row, column=1, sticky=W)
 
         self.pre_window_var = IntVar()
         self.pre_window_var.set(0)
         self.pre_window_lbl = Label(self.animal_cnt_frm, text='Pre-cue window (ms)', width=17, anchor=W)
         self.pre_window_entry = Entry(self.animal_cnt_frm, width=6, textvariable=self.pre_window_var)
@@ -187,15 +173,15 @@
         self.threshold_var.set(0.00)
         self.threshold_entry = Entry(self.animal_cnt_frm, width=6, textvariable=self.threshold_var)
         self.threshold_lbl.grid(row=current_row+3, column=0, sticky=W)
         self.threshold_entry.grid(row=current_row + 3, column=1, sticky=W)
         self.roi_var = BooleanVar()
         self.roi_check = Checkbutton(self.animal_cnt_frm, text='Analyze ROI data', variable=self.roi_var)
         self.roi_check.grid(row=current_row+4, column=0, sticky=W)
-        self.analyze_movement_btn = Button(self.animal_cnt_frm, text='Analyze movement data', command=lambda: self.__start_movement_analysis())
+        self.analyze_movement_btn = Button(self.animal_cnt_frm, text='Analyze movement data', command=lambda: self.start_movement_analysis())
         self.analyze_movement_btn.grid(row=current_row+5, column=0, sticky=W)
 
     def start_movement_analysis(self):
         self.__get_cue_light_names()
         if len(self.light_lst) == 0:
             raise CountError(msg='Zero user-specified cue lights. Please specify cue lights before analyzing movements')
         if not self.config.has_section('Cue light analysis'):
@@ -275,13 +261,13 @@
                                                          post_window=self.post_window_var_clf.get(),
                                                          clf_list=clf_lst,
                                                          cue_light_names=self.light_lst)
             clf_cue_light_analyzer.analyze_clf()
             clf_cue_light_analyzer.organize_results()
             clf_cue_light_analyzer.save_data()
 
-# test = CueLightAnalyzerMenu(config_path=r'/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini')
-# test.cue_light_main_frame.mainloop()
+# test = CueLightAnalyzerMenu(config_path=r'/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
+# test.main_frm.mainloop()
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def __init__(self,
                  config_path: str,
                  cue_light_names: list,
                  video_path: str,
                  frame_setting: bool,
                  video_setting: bool):
 
-        ConfigReader.__init__(config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
 
         if (not frame_setting) and (not video_setting):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choose to select either videos, frames, or both frames and videos.')
         self.video_setting, self.frame_setting = video_setting, frame_setting
         self.in_dir = os.path.join(self.project_path, 'csv', 'cue_lights')
         self.cue_light_names, self.video_path = cue_light_names, video_path
         _, self.video_name, _ = get_fn_ext(video_path)
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.58.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                  config_path: str,
                  pre_window: int,
                  post_window: int,
                  cue_light_names: list,
                  threshold: float,
                  roi_setting: bool):
 
-        ConfigReader.__init__(config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
         self.cue_light_names = cue_light_names
         self.roi_setting = roi_setting
         self.p_threshold = threshold
         self.pre_window, self.post_window = pre_window, post_window
         self.in_dir = os.path.join(self.project_path, 'csv', 'cue_lights')
         self.files_found = glob.glob(self.in_dir + '/*.' + self.file_type)
         self.bp_dict, self.bp_columns = defaultdict(list), []
@@ -75,17 +75,19 @@
         print('Analyzing {} files...'.format(str(len(self.files_found))))
 
         if roi_setting:
             self.roi_analyzer = ROIAnalyzer(ini_path=self.config_path,
                                             data_path=os.path.join(self.project_path, 'csv', 'outlier_corrected_movement_location'),
                                             calculate_distances=False)
             self.roi_analyzer.run()
-            self.entries_exits_df = pd.concat(self.roi_analyzer.entry_exit_df_lst, axis=0)
-            self.entries_exits_df = self.entries_exits_df[~self.entries_exits_df['Shape'].isin(self.cue_light_names)]
-            self.entries_exits_df['inside_lst'] = self.entries_exits_df.apply(lambda x: list(range(int(x['Entry_times']), int(x['Exit_times'] + 1))), axis=1)
+            #self.entries_exits_df = pd.DataFrame.from_dict(self.roi_analyzer.detailed_df, orient='index')
+            print(self.roi_analyzer.detailed_df)
+            self.entries_exits_df = self.roi_analyzer.detailed_df[~self.roi_analyzer.detailed_df['SHAPE'].isin(self.cue_light_names)]
+            if len(self.entries_exits_df) > 0:
+                self.entries_exits_df['inside_lst'] = self.entries_exits_df.apply(lambda x: list(range(int(x['ENTRY FRAMES']), int(x['EXIT FRAMES'] + 1))), axis=1)
 
     def __euclidean_distance(self, bp_1_x_vals, bp_2_x_vals, bp_1_y_vals, bp_2_y_vals, px_per_mm):
         series = (np.sqrt((bp_1_x_vals - bp_2_x_vals) ** 2 + (bp_1_y_vals - bp_2_y_vals) ** 2)) / px_per_mm
         return series
 
     def calculate_whole_session_movement(self):
         """
@@ -139,17 +141,17 @@
                        self.results[self.video_name][animal_name][cue_light][state_name]['Distance (cm)'] = round((df.sum() / 10), 4)
                        velocity_lst = []
                        for sliced_df in np.array_split(df, self.fps): velocity_lst.append(sliced_df.sum())
                        self.results[self.video_name][animal_name][cue_light][state_name]['Velocity (cm/s)'] = round((mean(velocity_lst) / 10), 4)
                 if self.roi_setting:
                     self.roi_results[self.video_name] = {}
                     self.roi_results[self.video_name][animal_name] = {}
-                    for roi_name in self.entries_exits_df['Shape'].unique():
+                    for roi_name in self.entries_exits_df['SHAPE'].unique():
                         self.roi_results[self.video_name][animal_name][roi_name] = {}
-                        inside_roi_frms = self.entries_exits_df['inside_lst'][self.entries_exits_df['Shape'] == roi_name]
+                        inside_roi_frms = self.entries_exits_df['inside_lst'][self.entries_exits_df['SHAPE'] == roi_name]
                         inside_roi_frms = [i for s in inside_roi_frms for i in s]
                         for cue_light in self.cue_light_names:
                             self.roi_results[self.video_name][animal_name][roi_name][cue_light] = {}
                             self.overlap_light = list(set(inside_roi_frms).intersection(self.light_on_dict[cue_light]['light_on_frames']))
                             self.overlap_pre_window_frames = list(set(inside_roi_frms).intersection(self.light_on_dict[cue_light]['pre_window_frames']))
                             self.overlap_post_window_frames = list(set(inside_roi_frms).intersection(self.light_on_dict[cue_light]['post_window_frames']))
                             for state_name, lst in zip(['pre-cue', 'cue', 'post-cue'],
@@ -199,8 +201,20 @@
         self.results_df = self.results_df.sort_values('Video').reset_index(drop=True)
         self.results_df.to_csv(save_results_path)
         stdout_success(msg='Cue light movement statistics saved in project_folder/logs directory.')
         if self.roi_setting:
             save_roi_results_path = os.path.join(self.logs_path, 'Cue_lights_roi_statistics_{}.csv'.format(self.datetime))
             self.results_roi_df = self.results_roi_df.sort_values('Video').reset_index(drop=True)
             self.results_roi_df.to_csv(save_roi_results_path)
-            stdout_success(msg='Cue light ROI statistics saved in project_folder/logs directory.')
+            stdout_success(msg='Cue light ROI statistics saved in project_folder/logs directory.')
+
+# test = CueLightMovementAnalyzer(config_path=r'/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
+#                                 pre_window=100, post_window=100, cue_light_names=['Rectangl_1'], threshold=0.0, roi_setting=True)
+#
+#
+    # def __init__(self,
+    #              config_path: str,
+    #              pre_window: int,
+    #              post_window: int,
+    #              cue_light_names: list,
+    #              threshold: float,
+    #              roi_setting: bool):
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.58.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.58.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.58.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.58.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.58.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/fsttc_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
         """
         Method to save forward spike-time tiling coefficients (FSTTC) to disk within the `project_folder/logs` directory.
 
         Returns
         -------
         None
         """
-        print(self.results_dict)
         self.out_df = pd.DataFrame(columns=['VIDEO', 'FIRST BEHAVIOR', 'SECOND BEHAVIOR', 'FSTTC'])
         for video_name, video_data in self.results_dict.items():
             for first_behavior, first_behavior_data in video_data.items():
                 for second_behavior, fsttc in first_behavior_data.items():
                     self.out_df.loc[len(self.out_df)] = [video_name, first_behavior, second_behavior, fsttc]
         file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
         self.out_df.to_csv(file_save_path)
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.58.4/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.58.4/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.58.4/simba/model/grid_search_rf.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,10 +214,14 @@
 # test = TrainMultipleModelsFromMeta(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.run()
 
 # file_paths = glob.glob('/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/targets_inserted' + '/*.csv')
 # df = read_all_files_in_folder_mp(file_paths=file_paths, file_type='csv')
 # check_dataset_integrity(df=df)
 
+#
+# test = GridSearchRandomForestClassifier(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
+# test.run()
+
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.58.4/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.58.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/madlc_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/misc/madlc_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from simba.utils.errors import BodypartColumnNotFoundError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import write_df, get_video_meta_data, find_all_videos_in_project
 
 from simba.utils.enums import Formats
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
 
-class MADLC_Importer(ConfigReader, PoseImporterMixin):
+class MADLCImporterH5(ConfigReader, PoseImporterMixin):
     """
     Class for importing multi-animal deeplabcut (maDLC) pose-estimation data (in H5 format)
     into a SimBA project in parquet or CSV format.
 
     Parameters
     ----------
     config_path: str
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/misc/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_slp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,453 +1,422 @@
-__author__ = "Simon Nilsson"
-
-import itertools
-import os, glob
-import numpy as np
-import h5py
-import json
-from collections import defaultdict
-import pandas as pd
-import cv2
-import random
-
-
-from simba.mixins.config_reader import ConfigReader
-from simba.mixins.pose_importer_mixin import PoseImporterMixin
-from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
-
-from simba.utils.read_write import get_fn_ext, find_video_of_file, get_video_meta_data, read_df, write_df, find_all_videos_in_project
-from simba.utils.checks import check_if_filepath_list_is_empty
-from simba.utils.data import create_color_palettes
-from simba.utils.enums import Paths, ConfigKey, Methods
-
-
-class SLEAPImporterSLP(ConfigReader, PoseImporterMixin):
-    """
-    Class for importing SLEAP pose-estimation data into a SimBA project.
-
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
-    data_folder: str
-        Path to folder containing SLEAP data in `.slp` format.
-    actor_IDs: list
-        Animal names.
-    interpolation_settings: str
-        String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
-        'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
-        'Body-parts: Quadratic'.
-    smoothing_settings: dict
-        Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
-        'Parameters': {'Time_window': '200'}})
-
-    Example
-    ----------
-    >>> slp_importer = ImportSLEAP(project_path="MyConfigPath", data_folder=r'MySLPDataFolder', actor_IDs=['Mouse_1', 'Mouse_2'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-    >>> slp_importer.initate_import_slp()
-    >>> slp_importer.visualize_sleap()
-    >>> slp_importer.perform_interpolation()
-    >>> slp_importer.perform_smothing()
-    """
-
-
-    def __init__(self,
-                 project_path: str,
-                 data_folder: str,
-                 id_lst: list,
-                 interpolation_settings: str,
-                 smoothing_settings: dict):
-
-        ConfigReader.__init__(self, config_path=project_path)
-        PoseImporterMixin.__init__(self)
-        self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
-        self.data_folder, self.id_lst = data_folder, id_lst
-        self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
-        self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
-        self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.slp'])
-        self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
-        print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
-
-    def __h5_to_dict(self, name, obj):
-        attr = list(obj.attrs.items())
-        if name == 'metadata':
-            jsonList = (attr[1][1])
-            jsonList = jsonList.decode('utf-8')
-            final_dictionary = json.loads(jsonList)
-            final_dictionary = dict(final_dictionary)
-            return final_dictionary
-
-    def run(self):
-        self.analysis_dict = defaultdict(list)
-        self.save_paths_lst = []
-        for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
-            print(f'Analysing {video_name}...')
-            in_h5 = h5py.File(video_data['DATA'], 'r')
-            self.sleap_dict = in_h5.visititems(self.__h5_to_dict)
-            self.video_info = get_video_meta_data(video_path=video_data['VIDEO'])
-            #self.save_path = os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}')
-            self.analysis_dict['bp_names'] = []
-            self.analysis_dict['ordered_ids'] = []
-            self.analysis_dict['ordered_bps'] = []
-            self.analysis_dict['xy_headers'] = []
-            self.analysis_dict['xyp_headers'] = []
-            self.analysis_dict['animals_in_each_frame'] = []
-            for bp in self.sleap_dict['nodes']:
-                self.analysis_dict['bp_names'].append(bp['name'])
-            for orderVar in self.sleap_dict['skeletons'][0]['nodes']:
-                self.analysis_dict['ordered_ids'].append((orderVar['id']))
-            for index in self.analysis_dict['ordered_ids']:
-                self.analysis_dict['ordered_bps'].append(self.analysis_dict['bp_names'][index])
-
-            with h5py.File(video_data['DATA'], 'r') as file:
-                self.analysis_dict['frames'] = file['frames'][:]
-                self.analysis_dict['instances'] = file['instances'][:]
-                self.analysis_dict['predicted_points'] = np.reshape(file['pred_points'][:], (file['pred_points'][:].size, 1))
-            self.analysis_dict['no_frames'] = len(self.analysis_dict['frames'])
-
-            for c in itertools.product(self.id_lst, self.analysis_dict['ordered_bps']):
-                x, y, p = str('{}_{}_x'.format(c[0], c[1])), str('{}_{}_y'.format(c[0], c[1])), (str('{}_{}_p'.format(c[0], c[1])))
-                self.analysis_dict['xy_headers'].extend((x, y))
-                self.analysis_dict['xyp_headers'].extend((x, y, p))
-    #
-            self.data_df = pd.DataFrame(columns=self.analysis_dict['xyp_headers'])
-            frames_lst = [l.tolist() for l in self.analysis_dict['frames']]
-            self.analysis_dict['animals_in_each_frame'] = [x[4] - x[3] for x in frames_lst]
-            self.__create_tracks()
-
-
-    def __create_tracks(self):
-        start_frame = 0
-        for frame_cnt, frame in enumerate(range(self.analysis_dict['no_frames'])):
-            frame_idx = self.analysis_dict['frames'][frame_cnt][2]
-            self.frame_dict = {}
-            print('Restructuring SLEAP frame: {}/{}, Video: {} ({}/{})'.format(str(frame_cnt), str(self.analysis_dict['no_frames']), str(self.video_name), str(self.video_counter + 1), str(len(self.files_found))))
-            self.cnt_animals_frm = self.analysis_dict['animals_in_each_frame'][frame]
-            if self.cnt_animals_frm == 0:
-                self.frame_dict[0] = [0] * len(self.analysis_dict['xyp_headers'])
-                end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
-
-            else:
-                end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
-                start_animal, end_animal = 0, len(self.analysis_dict['ordered_bps'])
-                frame_arr = self.analysis_dict['predicted_points'][start_frame:end_frame]
-                for instance_counter, animal in enumerate(range(self.cnt_animals_frm)):
-                    currRow = []
-                    animal_arr = frame_arr[start_animal:end_animal]
-                    track_id = self.analysis_dict['instances'][instance_counter][4]
-                    for bp in animal_arr:
-                        currRow.extend((bp[0][0], bp[0][1], bp[0][4]))
-                    self.frame_dict[track_id] = currRow
-                    start_animal += len(self.analysis_dict['ordered_bps'])
-                    end_animal += len(self.analysis_dict['ordered_bps'])
-
-            if self.animal_cnt > 1:
-                self.__check_that_all_animals_exist_in_frame()
-            frame_lst = [item for sublist in list(self.frame_dict.values()) for item in sublist]
-            start_frame = end_frame
-            try:
-                self.data_df.loc[frame_idx] = frame_lst
-            except ValueError:
-                break
-
-        self.data_df.fillna(0, inplace=True)
-        self.__fill_missing_indexes()
-        self.data_df.sort_index(inplace=True)
-        self.check_multi_animal_status()
-        if self.animal_cnt < 2:
-            self.multi_animal_status = False
-        color_lst = create_color_palettes(self.animal_cnt, len(self.analysis_dict['ordered_bps']))
-        self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animals_no, self.x_cols, self.x_cols, [], color_lst)
-        self.__update_bp_headers_file()
-        self.__save_multi_index_header_df(df=self.data_df, filetype=self.file_type, savepath=self.save_path)
-        print('Re-organized {} for SimBA analysis...'.format(os.path.basename(self.save_path)))
-
-    #
-    #
-    #
-    #
-    # def visualize_sleap(self):
-    #     self.frame_number = 0
-    #     for file_path in self.save_paths_lst:
-    #         self.data_df = read_df(file_path, self.file_type)
-    #         self.data_df.columns = self.bp_headers
-    #         _, video_name, _ = get_fn_ext(file_path)
-    #         video_path = find_video_of_file(self.video_folder, video_name)
-    #         self.cap = cv2.VideoCapture(video_path)
-    #         self.cap.set(1, self.frame_number)
-    #         if not self.cap.isOpened():
-    #             raise Exception('Can\'t open video file ' + video_path)
-    #         self.video_meta_data = get_video_meta_data(video_path)
-    #         mySpaceScale, myRadius, myResolution, myFontScale = 40, 10, 1500, 1.2
-    #         maxResDimension = max(self.video_meta_data['width'], self.video_meta_data['height'])
-    #         self.circle_scale = int(myRadius / (myResolution / maxResDimension))
-    #         self.font_scale = float(myFontScale / (myResolution / maxResDimension))
-    #         self.spacing_scale = int(mySpaceScale / (myResolution / maxResDimension))
-    #         self.__show_clean_window()
-    #
-    # def __update_config(self):
-    #     self.config.set("General settings", "animal_no", str(self.animals_no))
-    #     with open(self.project_path, "w+") as f:
-    #         self.config.write(f)
-    #     f.close()
-    #
-    # def __h5_to_dict(self, name, obj):
-    #     attr = list(obj.attrs.items())
-    #     if name == 'metadata':
-    #         jsonList = (attr[1][1])
-    #         jsonList = jsonList.decode('utf-8')
-    #         final_dictionary = json.loads(jsonList)
-    #         final_dictionary = dict(final_dictionary)
-    #         return final_dictionary
-    #
-    # def __get_video_frame_cnt(self):
-    #     cap = cv2.VideoCapture(self.video_path)
-    #     self.video_frame_cnt_opencv = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    #
-    # def __fill_missing_indexes(self):
-    #     missing_indexes = list(set(list(range(0, self.video_frame_cnt_opencv))) - set(list(self.data_df.index)))
-    #     missing_df = pd.DataFrame(0, index=missing_indexes, columns=self.analysis_dict['xyp_headers'])
-    #     self.data_df = pd.concat([self.data_df, missing_df], axis=0)
-    #
-    # def __save_multi_index_header_df(self, df=None, filetype=None, savepath=None):
-    #     if filetype == 'csv':
-    #         df.to_csv(savepath)
-    #     if filetype == 'parquet':
-    #         table = pa.Table.from_pandas(df)
-    #         pq.write_table(table, savepath)
-    #     self.save_paths_lst.append(savepath)
-    #
-    # def __update_bp_headers_file(self):
-    #     self.new_headers = []
-    #     if len(list(self.animal_bp_dict.keys())) > 1:
-    #         for cnt, animal in enumerate(self.animal_bp_dict.keys()):
-    #             for bp in self.analysis_dict['ordered_bps']:
-    #                 self.new_headers.append('{}_{}_{}'.format(animal, bp, str(cnt + 1)))
-    #     else:
-    #         for cnt, animal in enumerate(self.animal_bp_dict.keys()):
-    #             for bp in self.analysis_dict['ordered_bps']:
-    #                 self.new_headers.append('{}_{}'.format(bp, str(cnt + 1)))
-    #     new_bp_df = pd.DataFrame(self.new_headers)
-    #     new_bp_df.to_csv(self.bp_names_csv_path, index=False, header=False)
-    #
-    #
-    # def __check_that_all_animals_exist_in_frame(self):
-    #     existing_animals = list(self.frame_dict.keys())
-    #     missing_animals = [x for x in range(self.animals_no) if x not in existing_animals]
-    #     for missing_animal in missing_animals:
-    #         self.frame_dict[missing_animal] = [0] * ((len(self.analysis_dict['ordered_bps']))) * 3
-    #
-    # def __create_tracks(self):
-    #     start_frame = 0
-    #     for frame_cnt, frame in enumerate(range(self.analysis_dict['no_frames'])):
-    #         frame_idx = self.analysis_dict['frames'][frame_cnt][2]
-    #         self.frame_dict = {}
-    #         print('Restructuring SLEAP frame: {}/{}, Video: {} ({}/{})'.format(str(frame_cnt), str(self.analysis_dict['no_frames']), str(self.video_name), str(self.video_counter + 1), str(len(self.files_found))))
-    #         self.cnt_animals_frm = self.analysis_dict['animals_in_each_frame'][frame]
-    #         if self.cnt_animals_frm == 0:
-    #             self.frame_dict[0] = [0] * len(self.analysis_dict['xyp_headers'])
-    #             end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
-    #
-    #         else:
-    #             end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
-    #             start_animal, end_animal = 0, len(self.analysis_dict['ordered_bps'])
-    #             frame_arr = self.analysis_dict['predicted_points'][start_frame:end_frame]
-    #             for instance_counter, animal in enumerate(range(self.cnt_animals_frm)):
-    #                 currRow = []
-    #                 animal_arr = frame_arr[start_animal:end_animal]
-    #                 track_id = self.analysis_dict['instances'][instance_counter][4]
-    #                 for bp in animal_arr:
-    #                     currRow.extend((bp[0][0], bp[0][1], bp[0][4]))
-    #                 self.frame_dict[track_id] = currRow
-    #                 start_animal += len(self.analysis_dict['ordered_bps'])
-    #                 end_animal += len(self.analysis_dict['ordered_bps'])
-    #
-    #         if self.animals_no > 1:
-    #             self.__check_that_all_animals_exist_in_frame()
-    #         frame_lst = [item for sublist in list(self.frame_dict.values()) for item in sublist]
-    #         start_frame = end_frame
-    #         try:
-    #             self.data_df.loc[frame_idx] = frame_lst
-    #         except ValueError:
-    #             break
-    #
-    #     self.data_df.fillna(0, inplace=True)
-    #     self.__fill_missing_indexes()
-    #     self.data_df.sort_index(inplace=True)
-    #     self.check_multi_animal_status()
-    #     if self.animals_no < 2:
-    #         self.multi_animal_status = False
-    #     color_lst = create_color_palettes(self.animals_no, len(self.analysis_dict['ordered_bps']))
-    #     self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animals_no, self.x_cols, self.x_cols, [], color_lst)
-    #     self.__update_bp_headers_file()
-    #     self.__save_multi_index_header_df(df=self.data_df, filetype=self.file_type, savepath=self.save_path)
-    #     print('Re-organized {} for SimBA analysis...'.format(os.path.basename(self.save_path)))
-    #
-    # def __create_first_side_img(self):
-    #     self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
-    #     cv2.putText(self.side_img, 'Current video: ' + self.video_name, (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
-    #     cv2.putText(self.side_img, 'Can you assign identities based on the displayed frame ?', (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale,(255, 255, 255), 2)
-    #     cv2.putText(self.side_img, 'Press "x" to display new - random - frame', (10, int(self.spacing_scale * (self.add_spacer * 3))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
-    #     cv2.putText(self.side_img, 'Press "c" to continue to start assigning identities using this frame', (10, int(self.spacing_scale * (self.add_spacer * 4))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 255), 2)
-    #
-    # def __update_frame(self):
-    #     new_frame_option_lst = list(range(0, self.video_meta_data['frame_count']))
-    #     new_frame_option_lst.remove(self.frame_number)
-    #     self.frame_number = random.choice(new_frame_option_lst)
-    #     self.cap.set(1, self.frame_number)
-    #     self.__show_clean_window()
-    #
-    # def __get_x_y_loc(self, event, x, y, flags, param):
-    #     if event == 1:
-    #         self.click_loc = (x,y)
-    #         self.ID_cords[self.animal_cnt] = {}
-    #         self.ID_cords[self.animal_cnt]['cord'] = self.click_loc
-    #         self.ID_cords[self.animal_cnt]['name'] = self.current_animal
-    #         self.clicked = True
-    #         for id in self.ID_cords.keys():
-    #             cv2.putText(self.frame, self.ID_cords[id]['name'], self.ID_cords[id]['cord'], cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 0), 2)
-    #             self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
-    #             cv2.imshow('Define animal IDs', self.concat_img)
-    #
-    # def __create_third_side_img(self):
-    #     self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
-    #     cv2.putText(self.side_img, 'Current video: ' + self.video_name, (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
-    #     cv2.putText(self.side_img, 'Are you happy with your assigned identities ?', (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
-    #     cv2.putText(self.side_img, 'Press "c" to continue (to finish, or proceed to the next video)', (10, int(self.spacing_scale * (self.add_spacer * 3))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
-    #     cv2.putText(self.side_img, 'Press "x" to re-start assigning identities', (10, int(self.spacing_scale * (self.add_spacer * 4))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 255), 2)
-    #
-    # def __assign_individuals(self):
-    #     self.ID_cords = {}
-    #     for animal_cnt, animal in enumerate(self.animal_bp_dict.keys()):
-    #         self.current_animal = animal
-    #         self.animal_cnt = animal_cnt
-    #         self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
-    #         cv2.putText(self.side_img, 'Double left mouse click on:', (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
-    #         cv2.putText(self.side_img, animal, (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
-    #         self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
-    #         cv2.imshow('Define animal IDs', self.concat_img)
-    #         while animal_cnt not in self.ID_cords.keys():
-    #             cv2.setMouseCallback('Define animal IDs', self.__get_x_y_loc)
-    #             cv2.waitKey(20)
-    #
-    # def __show_clean_window(self):
-    #     cv2.namedWindow('Define animal IDs', cv2.WINDOW_NORMAL)
-    #     ret, self.frame = self.cap.read()
-    #     for animal in self.animal_bp_dict.keys():
-    #         for cnt, bp in enumerate(zip(self.animal_bp_dict[animal]['X_bps'], self.animal_bp_dict[animal]['Y_bps'])):
-    #             bp_cord = (int(self.data_df.at[self.frame_number, bp[0]]), int(self.data_df.at[self.frame_number, bp[1]]))
-    #             cv2.circle(self.frame, bp_cord, self.circle_scale, self.animal_bp_dict[animal]['colors'][cnt], -1, lineType=cv2.LINE_AA)
-    #     self.__create_first_side_img()
-    #     self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
-    #     cv2.imshow('Define animal IDs', self.concat_img)
-    #     keyboard_choice = False
-    #     while not keyboard_choice:
-    #         k = cv2.waitKey(10)
-    #         if k == ord('x'):
-    #             self.__update_frame()
-    #         elif k == ord('c'):
-    #             self.__assign_individuals()
-    #             keyboard_choice = True
-    #
-    #     self.__create_third_side_img()
-    #     self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
-    #     cv2.imshow('Define animal IDs', self.concat_img)
-    #     keyboard_choice = False
-    #     while not keyboard_choice:
-    #         k = cv2.waitKey(50)
-    #         if k == ord('x'):
-    #             self.__update_frame()
-    #         elif k == ord('c'):
-    #             cv2.waitKey(0)
-    #             cv2.destroyAllWindows()
-    #             self.__sort_df()
-    #             keyboard_choice = True
-    #
-    # def __insert_multiindex_header(self):
-    #     multi_index_columns = []
-    #     for column in range(len(self.data_df.columns)):
-    #         multi_index_columns.append(tuple(('SLEAP_multi', 'SLEAP_multi', self.data_df.columns[column])))
-    #     self.data_df.columns = pd.MultiIndex.from_tuples(multi_index_columns, names=['scorer', 'bodypart', 'coords'])
-    #
-    # def __sort_df(self):
-    #     header_order = []
-    #     for animal_id in self.ID_cords:
-    #        d = self.animal_bp_dict[self.ID_cords[animal_id]['name']]
-    #        p_cols = [x.replace(x[-1],'p') for x in d['X_bps']]
-    #        header_order.extend((list(itertools.chain.from_iterable(zip(d['X_bps'],d['Y_bps'], p_cols)))))
-    #     self.data_df = self.data_df[header_order]
-    #
-    # def save_df(self):
-    #     """
-    #     Method to save data created in SLEAP import GUI. Data is saved in the ``project_folder/csv/input_csv``
-    #     directory in the SimBA project.
-    #
-    #     Returns
-    #     -------
-    #     None
-    #
-    #     """
-    #
-    #     self.__insert_multiindex_header()
-    #     self.__save_multi_index_header_df(self.data_df,self.file_format,self.save_path)
-    #
-    # def perform_interpolation(self):
-    #     """
-    #     Method to save perform interpolation of imported SLEAP data.
-    #
-    #     Returns
-    #     -------
-    #     None
-    #
-    #     """
-    #
-    #     if self.interpolation_settings != 'None':
-    #         print('Interpolating missing values in video {} (Method: {})...'.format(self.video_name, self.interpolation_settings))
-    #         _ = Interpolate(input_path=self.save_path, config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
-    #
-    # def perform_smothing(self):
-    #     """
-    #     Method to save perform smoothing of imported SLEAP data.
-    #
-    #     Returns
-    #     -------
-    #     None
-    #     """
-    #
-    #     if (self.smoothing_settings['Method'] == Methods.GAUSSIAN.value) or (self.smoothing_settings['Method'] == Methods.SAVITZKY_GOLAY.value):
-    #         print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
-    #         Smooth(config_path=self.config_path,
-    #                input_path=self.save_path,
-    #                time_window=int(self.smoothing_settings['Parameters']['Time_window']),
-    #                smoothing_method=self.smoothing_settings['Method'],
-    #                initial_import_multi_index=True)
-
-
-test = SLEAPImporterSLP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini",
-                   data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/data',
-                   id_lst=['Simon', 'Nastacia', 'JJ', 'Sam', 'Liana'],
-                   interpolation_settings="Body-parts: Nearest",
-                   smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
-test.run()
-# if test.animals_no > 1:
-#     test.visualize_sleap()
-# test.save_df()
-# test.perform_interpolation()
-# test.perform_smothing()
-# print('All SLEAP imports complete.')
-
-
-# test = ImportSLEAP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_cody/project_folder/project_config.ini",
-#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_cody/import_data',
-#                    actor_IDs=['Animal_1', 'Animal_2'],
-#                    interpolation_settings="Body-parts: Nearest",
-#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
-# test.initate_import_slp()
-# if test.animals_no > 1:
-#     test.visualize_sleap()
-# test.save_df()
-# test.perform_interpolation()
-# test.perform_smothing()
-# print('All SLEAP imports complete.')
-
-
+__author__ = "Simon Nilsson"
+
+import itertools
+import os, glob
+import numpy as np
+import h5py
+import json
+from collections import defaultdict
+import pandas as pd
+import cv2
+import random
+
+
+from simba.mixins.config_reader import ConfigReader
+from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
+from simba.utils.read_write import get_fn_ext, find_video_of_file, get_video_meta_data, read_df, write_df
+from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.data import create_color_palettes
+from simba.utils.enums import Paths, ConfigKey, Methods
+
+
+
+class SLEAPImporterSLP(ConfigReader):
+    """
+    Class for importing SLEAP pose-estimation data into a SimBA project.
+
+    Parameters
+    ----------
+    config_path: str
+        path to SimBA project config file in Configparser format
+    data_folder: str
+        Path to folder containing SLEAP data in `.slp` format.
+    actor_IDs: list
+        Animal names.
+    interpolation_settings: str
+        String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+        'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
+        'Body-parts: Quadratic'.
+    smoothing_settings: dict
+        Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+        'Parameters': {'Time_window': '200'}})
+
+    Example
+    ----------
+    >>> slp_importer = ImportSLEAP(project_path="MyConfigPath", data_folder=r'MySLPDataFolder', actor_IDs=['Mouse_1', 'Mouse_2'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+    >>> slp_importer.initate_import_slp()
+    >>> slp_importer.visualize_sleap()
+    >>> slp_importer.perform_interpolation()
+    >>> slp_importer.perform_smothing()
+    """
+
+
+    def __init__(self,
+                 project_path: str,
+                 data_folder: str,
+                 actor_IDs: list,
+                 interpolation_settings: str,
+                 smoothing_settings: dict):
+
+        ConfigReader.__init__(self, config_path=project_path)
+        self.interpolation_settings = interpolation_settings
+        self.smoothing_settings = smoothing_settings
+        self.actors_IDs = actor_IDs
+        self.video_folder = os.path.join(self.project_path, 'videos')
+        self.files_found = glob.glob(data_folder + '/*.slp')
+        check_if_filepath_list_is_empty(filepaths=self.files_found,
+                                        error_msg='SIMBA ERROR: Zero .slp files found in {} directory'.format(data_folder))
+        self.save_folder = os.path.join(self.project_path, Paths.INPUT_CSV.value)
+        self.animals_no = len(self.actors_IDs)
+        self.add_spacer = 2
+        self.bp_names_csv_path = os.path.join(self.project_path, Paths.BP_NAMES.value)
+        self.pose_settings = self.config.get(ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.POSE_SETTING.value)
+        if self.pose_settings is Methods.USER_DEFINED.value:
+            self.__update_config()
+
+        print('Converting .SLP file(s) into SimBA dataframes...')
+
+    def visualize_sleap(self):
+        self.frame_number = 0
+        for file_path in self.save_paths_lst:
+            self.data_df = read_df(file_path, self.file_type)
+            self.data_df.columns = self.bp_headers
+            _, video_name, _ = get_fn_ext(file_path)
+            video_path = find_video_of_file(self.video_folder, video_name)
+            self.cap = cv2.VideoCapture(video_path)
+            self.cap.set(1, self.frame_number)
+            if not self.cap.isOpened():
+                raise Exception('Can\'t open video file ' + video_path)
+            self.video_meta_data = get_video_meta_data(video_path)
+            mySpaceScale, myRadius, myResolution, myFontScale = 40, 10, 1500, 1.2
+            maxResDimension = max(self.video_meta_data['width'], self.video_meta_data['height'])
+            self.circle_scale = int(myRadius / (myResolution / maxResDimension))
+            self.font_scale = float(myFontScale / (myResolution / maxResDimension))
+            self.spacing_scale = int(mySpaceScale / (myResolution / maxResDimension))
+            self.__show_clean_window()
+
+    def __update_config(self):
+        self.config.set("General settings", "animal_no", str(self.animals_no))
+        with open(self.project_path, "w+") as f:
+            self.config.write(f)
+        f.close()
+
+    def __h5_to_dict(self, name, obj):
+        attr = list(obj.attrs.items())
+        if name == 'metadata':
+            jsonList = (attr[1][1])
+            jsonList = jsonList.decode('utf-8')
+            final_dictionary = json.loads(jsonList)
+            final_dictionary = dict(final_dictionary)
+            return final_dictionary
+
+    def __get_provenance(self):
+        try:
+            video_path = os.path.basename(self.sleap_dict['provenance']['video.path'])
+            _, video_name, _ = get_fn_ext(video_path)
+        except KeyError:
+            _, video_name, _ = get_fn_ext(self.file_path)
+
+        return find_video_of_file(self.video_folder, video_name)
+
+    def __get_video_frame_cnt(self):
+        cap = cv2.VideoCapture(self.video_path)
+        self.video_frame_cnt_opencv = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+
+    def __fill_missing_indexes(self):
+        missing_indexes = list(set(list(range(0, self.video_frame_cnt_opencv))) - set(list(self.data_df.index)))
+        missing_df = pd.DataFrame(0, index=missing_indexes, columns=self.analysis_dict['xyp_headers'])
+        self.data_df = pd.concat([self.data_df, missing_df], axis=0)
+
+    def __save_multi_index_header_df(self, df=None, filetype=None, savepath=None):
+        if filetype == 'csv':
+            df.to_csv(savepath)
+        if filetype == 'parquet':
+            table = pa.Table.from_pandas(df)
+            pq.write_table(table, savepath)
+        self.save_paths_lst.append(savepath)
+
+    def __update_bp_headers_file(self):
+        self.new_headers = []
+        if len(list(self.animal_bp_dict.keys())) > 1:
+            for cnt, animal in enumerate(self.animal_bp_dict.keys()):
+                for bp in self.analysis_dict['ordered_bps']:
+                    self.new_headers.append('{}_{}_{}'.format(animal, bp, str(cnt + 1)))
+        else:
+            for cnt, animal in enumerate(self.animal_bp_dict.keys()):
+                for bp in self.analysis_dict['ordered_bps']:
+                    self.new_headers.append('{}_{}'.format(bp, str(cnt + 1)))
+        new_bp_df = pd.DataFrame(self.new_headers)
+        new_bp_df.to_csv(self.bp_names_csv_path, index=False, header=False)
+
+    def initate_import_slp(self):
+        """
+        Method to initiate SLEAP import GUI.
+
+        Returns
+        -------
+        Attribute: dict
+            analysis_dict
+
+        """
+        self.analysis_dict = defaultdict(list)
+        self.save_paths_lst = []
+        for vdn_cnt, file_path in enumerate(self.files_found):
+            print('Analysing {}{}'.format(os.path.basename(file_path), '...'))
+            self.file_path = file_path
+            in_h5 = h5py.File(file_path, 'r')
+            self.video_counter = vdn_cnt
+            self.sleap_dict = in_h5.visititems(self.__h5_to_dict)
+            self.video_path = self.__get_provenance()
+            self.video_dir, self.video_name, self.video_ext = get_fn_ext(self.video_path)
+            self.save_path = os.path.join(self.save_folder, self.video_name + '.{}'.format(self.file_type))
+            self.__get_video_frame_cnt()
+            self.analysis_dict['bp_names'] = []
+            self.analysis_dict['ordered_ids'] = []
+            self.analysis_dict['ordered_bps'] = []
+            self.analysis_dict['xy_headers'] = []
+            self.analysis_dict['xyp_headers'] = []
+            self.analysis_dict['animals_in_each_frame'] = []
+            for bp in self.sleap_dict['nodes']:
+                self.analysis_dict['bp_names'].append(bp['name'])
+            for orderVar in self.sleap_dict['skeletons'][0]['nodes']:
+                self.analysis_dict['ordered_ids'].append((orderVar['id']))
+            for index in self.analysis_dict['ordered_ids']:
+                self.analysis_dict['ordered_bps'].append(self.analysis_dict['bp_names'][index])
+
+            with h5py.File(file_path, 'r') as file:
+                self.analysis_dict['frames'] = file['frames'][:]
+                self.analysis_dict['instances'] = file['instances'][:]
+                self.analysis_dict['predicted_points'] = np.reshape(file['pred_points'][:], (file['pred_points'][:].size, 1))
+
+            self.analysis_dict['no_frames'] = len(self.analysis_dict['frames'])
+            for c in itertools.product(self.actors_IDs, self.analysis_dict['ordered_bps']):
+                x, y, p = str('{}_{}_x'.format(c[0], c[1])), str('{}_{}_y'.format(c[0], c[1])), (str('{}_{}_p'.format(c[0], c[1])))
+                self.analysis_dict['xy_headers'].extend((x, y))
+                self.analysis_dict['xyp_headers'].extend((x, y, p))
+
+            self.data_df = pd.DataFrame(columns=self.analysis_dict['xyp_headers'])
+            frames_lst = [l.tolist() for l in self.analysis_dict['frames']]
+            self.analysis_dict['animals_in_each_frame'] = [x[4] - x[3] for x in frames_lst]
+            self.__create_tracks()
+
+
+    def __check_that_all_animals_exist_in_frame(self):
+        existing_animals = list(self.frame_dict.keys())
+        missing_animals = [x for x in range(self.animals_no) if x not in existing_animals]
+        for missing_animal in missing_animals:
+            self.frame_dict[missing_animal] = [0] * ((len(self.analysis_dict['ordered_bps']))) * 3
+
+    def __create_tracks(self):
+        start_frame = 0
+        for frame_cnt, frame in enumerate(range(self.analysis_dict['no_frames'])):
+            frame_idx = self.analysis_dict['frames'][frame_cnt][2]
+            self.frame_dict = {}
+            print('Restructuring SLEAP frame: {}/{}, Video: {} ({}/{})'.format(str(frame_cnt), str(self.analysis_dict['no_frames']), str(self.video_name), str(self.video_counter + 1), str(len(self.files_found))))
+            self.cnt_animals_frm = self.analysis_dict['animals_in_each_frame'][frame]
+            if self.cnt_animals_frm == 0:
+                self.frame_dict[0] = [0] * len(self.analysis_dict['xyp_headers'])
+                end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
+
+            else:
+                end_frame = start_frame + (len(self.analysis_dict['ordered_bps']) * self.cnt_animals_frm)
+                start_animal, end_animal = 0, len(self.analysis_dict['ordered_bps'])
+                frame_arr = self.analysis_dict['predicted_points'][start_frame:end_frame]
+                for instance_counter, animal in enumerate(range(self.cnt_animals_frm)):
+                    currRow = []
+                    animal_arr = frame_arr[start_animal:end_animal]
+                    track_id = self.analysis_dict['instances'][instance_counter][4]
+                    for bp in animal_arr:
+                        currRow.extend((bp[0][0], bp[0][1], bp[0][4]))
+                    self.frame_dict[track_id] = currRow
+                    start_animal += len(self.analysis_dict['ordered_bps'])
+                    end_animal += len(self.analysis_dict['ordered_bps'])
+
+            if self.animals_no > 1:
+                self.__check_that_all_animals_exist_in_frame()
+            frame_lst = [item for sublist in list(self.frame_dict.values()) for item in sublist]
+            start_frame = end_frame
+            try:
+                self.data_df.loc[frame_idx] = frame_lst
+            except ValueError:
+                break
+
+        self.data_df.fillna(0, inplace=True)
+        self.__fill_missing_indexes()
+        self.data_df.sort_index(inplace=True)
+        self.check_multi_animal_status()
+        if self.animals_no < 2:
+            self.multi_animal_status = False
+        color_lst = create_color_palettes(self.animals_no, len(self.analysis_dict['ordered_bps']))
+        self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animals_no, self.x_cols, self.x_cols, [], color_lst)
+        self.__update_bp_headers_file()
+        self.__save_multi_index_header_df(df=self.data_df, filetype=self.file_type, savepath=self.save_path)
+        print('Re-organized {} for SimBA analysis...'.format(os.path.basename(self.save_path)))
+
+    def __create_first_side_img(self):
+        self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
+        cv2.putText(self.side_img, 'Current video: ' + self.video_name, (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
+        cv2.putText(self.side_img, 'Can you assign identities based on the displayed frame ?', (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale,(255, 255, 255), 2)
+        cv2.putText(self.side_img, 'Press "x" to display new - random - frame', (10, int(self.spacing_scale * (self.add_spacer * 3))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
+        cv2.putText(self.side_img, 'Press "c" to continue to start assigning identities using this frame', (10, int(self.spacing_scale * (self.add_spacer * 4))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 255), 2)
+
+    def __update_frame(self):
+        new_frame_option_lst = list(range(0, self.video_meta_data['frame_count']))
+        new_frame_option_lst.remove(self.frame_number)
+        self.frame_number = random.choice(new_frame_option_lst)
+        self.cap.set(1, self.frame_number)
+        self.__show_clean_window()
+
+    def __get_x_y_loc(self, event, x, y, flags, param):
+        if event == 1:
+            self.click_loc = (x,y)
+            self.ID_cords[self.animal_cnt] = {}
+            self.ID_cords[self.animal_cnt]['cord'] = self.click_loc
+            self.ID_cords[self.animal_cnt]['name'] = self.current_animal
+            self.clicked = True
+            for id in self.ID_cords.keys():
+                cv2.putText(self.frame, self.ID_cords[id]['name'], self.ID_cords[id]['cord'], cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 0), 2)
+                self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
+                cv2.imshow('Define animal IDs', self.concat_img)
+
+    def __create_third_side_img(self):
+        self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
+        cv2.putText(self.side_img, 'Current video: ' + self.video_name, (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
+        cv2.putText(self.side_img, 'Are you happy with your assigned identities ?', (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
+        cv2.putText(self.side_img, 'Press "c" to continue (to finish, or proceed to the next video)', (10, int(self.spacing_scale * (self.add_spacer * 3))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
+        cv2.putText(self.side_img, 'Press "x" to re-start assigning identities', (10, int(self.spacing_scale * (self.add_spacer * 4))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (0, 255, 255), 2)
+
+    def __assign_individuals(self):
+        self.ID_cords = {}
+        for animal_cnt, animal in enumerate(self.animal_bp_dict.keys()):
+            self.current_animal = animal
+            self.animal_cnt = animal_cnt
+            self.side_img = np.ones((int(self.video_meta_data['height'] / 1.5), self.video_meta_data['width'], 3))
+            cv2.putText(self.side_img, 'Double left mouse click on:', (10, int(self.spacing_scale)), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 255), 2)
+            cv2.putText(self.side_img, animal, (10, int(self.spacing_scale * (self.add_spacer * 2))), cv2.FONT_HERSHEY_SIMPLEX, self.font_scale, (255, 255, 0), 2)
+            self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
+            cv2.imshow('Define animal IDs', self.concat_img)
+            while animal_cnt not in self.ID_cords.keys():
+                cv2.setMouseCallback('Define animal IDs', self.__get_x_y_loc)
+                cv2.waitKey(20)
+
+    def __show_clean_window(self):
+        cv2.namedWindow('Define animal IDs', cv2.WINDOW_NORMAL)
+        ret, self.frame = self.cap.read()
+        for animal in self.animal_bp_dict.keys():
+            for cnt, bp in enumerate(zip(self.animal_bp_dict[animal]['X_bps'], self.animal_bp_dict[animal]['Y_bps'])):
+                bp_cord = (int(self.data_df.at[self.frame_number, bp[0]]), int(self.data_df.at[self.frame_number, bp[1]]))
+                cv2.circle(self.frame, bp_cord, self.circle_scale, self.animal_bp_dict[animal]['colors'][cnt], -1, lineType=cv2.LINE_AA)
+        self.__create_first_side_img()
+        self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
+        cv2.imshow('Define animal IDs', self.concat_img)
+        keyboard_choice = False
+        while not keyboard_choice:
+            k = cv2.waitKey(10)
+            if k == ord('x'):
+                self.__update_frame()
+            elif k == ord('c'):
+                self.__assign_individuals()
+                keyboard_choice = True
+
+        self.__create_third_side_img()
+        self.concat_img = np.uint8(np.concatenate((self.frame, self.side_img), axis=0))
+        cv2.imshow('Define animal IDs', self.concat_img)
+        keyboard_choice = False
+        while not keyboard_choice:
+            k = cv2.waitKey(50)
+            if k == ord('x'):
+                self.__update_frame()
+            elif k == ord('c'):
+                cv2.waitKey(0)
+                cv2.destroyAllWindows()
+                self.__sort_df()
+                keyboard_choice = True
+
+    def __insert_multiindex_header(self):
+        multi_index_columns = []
+        for column in range(len(self.data_df.columns)):
+            multi_index_columns.append(tuple(('SLEAP_multi', 'SLEAP_multi', self.data_df.columns[column])))
+        self.data_df.columns = pd.MultiIndex.from_tuples(multi_index_columns, names=['scorer', 'bodypart', 'coords'])
+
+    def __sort_df(self):
+        header_order = []
+        for animal_id in self.ID_cords:
+           d = self.animal_bp_dict[self.ID_cords[animal_id]['name']]
+           p_cols = [x.replace(x[-1],'p') for x in d['X_bps']]
+           header_order.extend((list(itertools.chain.from_iterable(zip(d['X_bps'],d['Y_bps'], p_cols)))))
+        self.data_df = self.data_df[header_order]
+
+    def save_df(self):
+        """
+        Method to save data created in SLEAP import GUI. Data is saved in the ``project_folder/csv/input_csv``
+        directory in the SimBA project.
+
+        Returns
+        -------
+        None
+
+        """
+
+        self.__insert_multiindex_header()
+        self.__save_multi_index_header_df(self.data_df,self.file_format,self.save_path)
+
+    def perform_interpolation(self):
+        """
+        Method to save perform interpolation of imported SLEAP data.
+
+        Returns
+        -------
+        None
+
+        """
+
+        if self.interpolation_settings != 'None':
+            print('Interpolating missing values in video {} (Method: {})...'.format(self.video_name, self.interpolation_settings))
+            _ = Interpolate(input_path=self.save_path, config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
+
+    def perform_smothing(self):
+        """
+        Method to save perform smoothing of imported SLEAP data.
+
+        Returns
+        -------
+        None
+        """
+
+        if (self.smoothing_settings['Method'] == Methods.GAUSSIAN.value) or (self.smoothing_settings['Method'] == Methods.SAVITZKY_GOLAY.value):
+            print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
+            Smooth(config_path=self.config_path,
+                   input_path=self.save_path,
+                   time_window=int(self.smoothing_settings['Parameters']['Time_window']),
+                   smoothing_method=self.smoothing_settings['Method'],
+                   initial_import_multi_index=True)
+
+
+# test = SLEAPImporterSLP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini",
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/data',
+#                    actor_IDs=['Simon', 'Nastacia', 'JJ', 'Sam', 'Liana'],
+#                    interpolation_settings="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
+# test.initate_import_slp()
+# if test.animals_no > 1:
+#     test.visualize_sleap()
+# test.save_df()
+# test.perform_interpolation()
+# test.perform_smothing()
+# print('All SLEAP imports complete.')
+
+
+# test = ImportSLEAP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_cody/project_folder/project_config.ini",
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_cody/import_data',
+#                    actor_IDs=['Animal_1', 'Animal_2'],
+#                    interpolation_settings="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
+# test.initate_import_slp()
+# if test.animals_no > 1:
+#     test.visualize_sleap()
+# test.save_df()
+# test.perform_interpolation()
+# test.perform_smothing()
+# print('All SLEAP imports complete.')
+
+
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.58.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.58.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.58.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.58.4/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,14 +823,15 @@
         if currentPlatform == OS.MAC.value:
             self.txt.bind("<Button-2>", self.show_right_click_pop_up)
         self.txt.tag_configure(TagNames.GREETING.value, justify='center', foreground='blue', font=("Rockwell", 16, 'bold'))
         self.txt.tag_configure(TagNames.ERROR.value, justify='left', foreground='red', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.STANDARD.value, justify='left', foreground='black', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.COMPLETE.value, justify='left', foreground='darkgreen', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.WARNING.value, justify='left', foreground='darkorange', font=Formats.TKINTER_FONT.value)
+        self.txt.tag_configure('TABLE', foreground='darkorange', font=('Consolas', 10), wrap='none', borderwidth=0)
         self.txt.insert(INSERT, Defaults.WELCOME_MSG.value + emojis['relaxed'] + '\n' * 2)
         self.txt.tag_add(TagNames.GREETING.value, "1.0", "3.25")
         y_sb.pack(side=RIGHT, fill=Y)
         self.txt.pack(expand=True, fill='both')
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
@@ -879,15 +880,15 @@
 
     def write(self, s: str):
         tag_name = TagNames.STANDARD.value
         try:
             s, tag_name = s.split(Defaults.STR_SPLIT_DELIMITER.value, 2)
         except ValueError:
             pass
-        if tag_name != TagNames.STANDARD.value:
+        if (tag_name != TagNames.STANDARD.value) and (tag_name != 'TABLE'):
             s = s + ' ' + self.emojis[tag_name]
         self.text_space.config(state=NORMAL)
         self.text_space.insert("end", s, (tag_name))
         self.text_space.update()
         self.text_space.see("end")
         self.text_space.config(state=DISABLED)
```

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.58.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.58.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.58.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.58.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.58.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.58.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.58.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.58.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.58.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.58.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.3
+Version: 1.58.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,15 @@
 simba/pose_importers/dlc_multi_animal_importer.py
 simba/pose_importers/import_mars.py
 simba/pose_importers/read_DANNCE_mat.py
 simba/pose_importers/sleap_importer_csv.py
 simba/pose_importers/sleap_importer_h5.py
 simba/pose_importers/sleap_importer_slp.py
 simba/pose_importers/trk_importer.py
+simba/pose_importers/misc/apt_trk_importer.py
 simba/pose_importers/misc/madlc_importer.py
 simba/pose_importers/misc/sleap_csv_importer.py
 simba/pose_importers/misc/sleap_h5_importer.py
 simba/pose_importers/misc/sleap_slp_importer.py
 simba/pose_processors/pose_reset.py
 simba/pose_processors/remove_keypoints.py
 simba/pose_processors/reorganize_keypoint.py
```

### Comparing `Simba-UW-tf-dev-1.58.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.58.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/LICENSE.md` & `Simba-UW-tf-dev-1.58.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/README.md` & `Simba-UW-tf-dev-1.58.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.3/setup.py` & `Simba-UW-tf-dev-1.58.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.58.3",
+    version="1.58.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

