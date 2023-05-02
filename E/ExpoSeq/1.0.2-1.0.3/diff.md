# Comparing `tmp/ExpoSeq-1.0.2.tar.gz` & `tmp/ExpoSeq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.0.2.tar", last modified: Mon Mar 13 10:36:16 2023, max compression
+gzip compressed data, was "ExpoSeq-1.0.3.tar", last modified: Tue May  2 17:28:12 2023, max compression
```

## Comparing `ExpoSeq-1.0.2.tar` & `ExpoSeq-1.0.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.892282 ExpoSeq-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       59 2023-03-08 13:53:44.000000 ExpoSeq-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4086 2023-03-13 10:36:16.892282 ExpoSeq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-03-11 12:17:37.000000 ExpoSeq-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-13 10:36:16.892282 ExpoSeq-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1266 2023-03-13 10:36:04.000000 ExpoSeq-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.704780 ExpoSeq-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.720406 ExpoSeq-1.0.2/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.767312 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-03-11 12:06:04.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      905 2023-03-09 14:58:45.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     1833 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7770 2023-03-13 10:18:22.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10041 2023-03-11 10:14:21.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     5730 2023-03-10 12:50:00.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-03-09 15:09:25.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    18045 2023-03-13 10:34:22.000000 ExpoSeq-1.0.2/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    28170 2023-03-11 12:06:04.000000 ExpoSeq-1.0.2/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.798532 ExpoSeq-1.0.2/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2055 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1660 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-03-10 14:44:08.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3363 2023-03-10 12:31:37.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7663 2023-03-10 14:40:44.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4291 2023-03-10 12:31:37.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3346 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1464 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-03-10 10:47:32.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1058 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2536 2023-03-09 13:38:51.000000 ExpoSeq-1.0.2/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-03-11 11:48:16.000000 ExpoSeq-1.0.2/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0     7139 2023-03-13 09:53:10.000000 ExpoSeq-1.0.2/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.829784 ExpoSeq-1.0.2/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1727 2023-03-10 12:14:15.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-03-08 14:12:47.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-03-11 11:49:10.000000 ExpoSeq-1.0.2/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.876656 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.876656 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-03-09 13:29:06.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      423 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1200 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-03-08 13:17:42.000000 ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-03-13 10:36:16.736032 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4086 2023-03-13 10:36:16.000000 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2023-03-13 10:36:16.000000 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 10:36:16.000000 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2023-03-13 10:36:16.000000 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-13 10:36:16.000000 ExpoSeq-1.0.2/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.750118 ExpoSeq-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-03-08 13:53:44.000000 ExpoSeq-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4086 2023-05-02 17:28:12.750118 ExpoSeq-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-03-11 12:17:37.000000 ExpoSeq-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:28:12.750118 ExpoSeq-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2023-05-02 17:28:06.000000 ExpoSeq-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.699326 ExpoSeq-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.699326 ExpoSeq-1.0.3/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.714951 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-03-11 12:06:04.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-05-01 13:26:21.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     3114 2023-05-01 13:32:58.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7770 2023-03-13 10:18:22.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10041 2023-03-11 10:14:21.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     5730 2023-03-10 12:50:00.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-03-09 15:09:25.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    12682 2023-05-02 17:24:21.000000 ExpoSeq-1.0.3/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    28170 2023-03-11 12:06:04.000000 ExpoSeq-1.0.3/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.734485 ExpoSeq-1.0.3/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2055 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1660 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-03-10 14:44:08.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3363 2023-03-10 12:31:37.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7663 2023-03-10 14:40:44.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4291 2023-03-10 12:31:37.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3346 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1464 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1634 2023-03-10 10:47:32.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1058 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2536 2023-03-09 13:38:51.000000 ExpoSeq-1.0.3/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-03-11 11:48:16.000000 ExpoSeq-1.0.3/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0     7139 2023-03-13 09:53:10.000000 ExpoSeq-1.0.3/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.734485 ExpoSeq-1.0.3/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1727 2023-03-10 12:14:15.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-03-08 14:12:47.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-03-11 11:49:10.000000 ExpoSeq-1.0.3/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.734485 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.750118 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-03-09 13:29:06.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      423 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1200 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-03-08 13:17:42.000000 ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:12.714951 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4086 2023-05-02 17:28:12.000000 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2439 2023-05-02 17:28:12.000000 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:28:12.000000 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-05-02 17:28:12.000000 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 17:28:12.000000 ExpoSeq-1.0.3/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.0.2/LICENSE` & `ExpoSeq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/PKG-INFO` & `ExpoSeq-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.2
+Version: 1.0.3
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: s220672@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.0.2/README.md` & `ExpoSeq-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/setup.py` & `ExpoSeq-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.0.2",
+    version = "1.0.3",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "s220672@dtu.dk",
     license = "MIT",
     package_data={
         "ExpoSeq": ["settings/*.txt"]
     },
     install_requires = [
-                        "numpy>=1.24.1",
+                        "numpy>=1.23.5",
                         "pandas>=1.5.3",
                         "matplotlib>=3.6.3",
                         "scipy>=1.10.0",
                         "seaborn>=0.12.2",
                         "logomaker==0.8",
                         "editdistance==0.6.2",
                         "networkx>=2.6.3",
-                        "PyQt5==5.15.8",
-                        "sgt>=2.0.3",
+                        "PyQt5==5.15.7",
                         "scikit-learn>=1.2.1",
-                        "bio==1.5.3"
+                        "biopython==1.5.3",
+                        "sgt>=2.0.3",
                         ],
     python_requires=">=3.8",
     package_dir = {"": "src"},
     packages = find_packages(where="src"),
 
 )
```

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/load_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from glob import glob
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
-def collectFiles(filetypes = ('.txt', '.fastq_AlignmentReport')):
+def collectFiles(filetypes = ('.txt', ".tsv", '.fastq_AlignmentReport')):
     filenames = []
     try:
         data_folder = filedialog.askdirectory()
     except:
         while True:
             data_folder = input("copy and paste the path to the directory without any / as ending.")
             if path.isdir(os.path.abspath(data_folder)) == True:
```

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.0.3/src/ExpoSeq/augment_data/uploader.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,153 +11,196 @@
 import pkg_resources
 from .trimming import trimming
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
+
+def pull_seq_align_repo():
+    try:
+        print("choose the directory where you store your alignment reports and your sequencing report")
+        filenames_dir = filedialog.askdirectory()
+        filenames = glob(filenames_dir + "//*")
+        for i in filenames:
+            if os.path.isdir(i):
+                if "alignment_reports" in i:
+                    alignment_repos = glob(i)
+                    filenames.extend(alignment_repos)
+    except:
+        filenames_dir = input(
+            "Enter the directory where you store the alignment reports and your sequencing report manually.")
+        filenames_dir = os.path.abspath(filenames_dir)
+        filenames = glob(filenames_dir)
+        for i in filenames:
+            if os.path.isdir(i):
+                if "alignment_reports" in i:
+                    alignment_repos = glob(i)
+                    filenames.extend(alignment_repos)
+    sequencing_report, all_alignment_reports = load_mixed_files(filenames)
+    return sequencing_report, all_alignment_reports
+
+def check_experiment(module_dir):
+    while True:
+        experiment = input("How do you want to call your new experiment?")
+        if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
+            replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
+            if replace in ["Y", "y", "n", "N"]:
+                break
+            else:
+                print("Please enter another name.")
+        else:
+
+            os.mkdir(os.path.join(module_dir,
+                                       "my_experiments",
+                                       experiment))
+            break
+    return experiment
+
+def method_one(experiment, repo_path, module_dir):
+    use_method = input(
+        "Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
+    if use_method == "":
+        method = "milab-human-tcr-dna-multiplex-cdr3"
+    else:
+        method = use_method
+    paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
+    if paired_end.lower() in ["Y", "y"]:
+        paired_end = True
+    else:
+        paired_end = False
+    process_mixcr(experiment,
+                  method=method,
+                  paired_end_sequencing=paired_end)
+
+    with open(repo_path, "rb") as f:
+        sequencing_report = pd.read_table(f, sep=",")
+    try:
+        align_repo_path = os.path.join(module_dir,
+                                       "my_experiemnts",
+                                       experiment,
+                                       "alignment_reports",
+                                       "*")
+        alignment_reports = glob(align_repo_path)
+        all_alignment_reports = load_alignment_reports(alignment_reports)
+    except:
+        all_alignment_reports = pd.DataFrame([])
+        print(
+            "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+    return sequencing_report, all_alignment_reports
+def method_two(module_dir, experiment):
+
+    print("Choose the folder which contains the sequencing_report and the alignment reports.")
+
+    sequencing_report, all_alignment_reports = pull_seq_align_repo()
+
+    while True:
+        if sequencing_report.shape[0] == 0:
+            print(
+                "Something went wrong. Unfortunately you could not collect the data in the sequencing report. Please make sure that you have chosen the right directory and that you have tsv files as output from mixcr in that directory.")
+            sequencing_report, all_alignment_reports = pull_seq_align_repo()
+        else:
+            break
+        #  sys.exit()
+    while True:
+        trim_data = input("Do you need to trim your data? (Y/n)")
+        if trim_data in ["Y", "y", "n", "N"]:
+            break
+        else:
+            print("Please enter a correct value.")
+    if trim_data.lower() in ["Y", "y"]:
+        sequencing_report = trimming(sequencing_report,
+                                     divisible_by=3,  # might be possible that columns are different
+                                     min_count=1,
+                                     new_fraction="cloneFraction")
+    else:
+        pass
+    seq_report_dir = os.path.join(module_dir,
+                                  "my_experiments",
+                                  experiment,
+                                  "sequencing_report.csv")
+    sequencing_report.to_csv(seq_report_dir)
+    unique_experiments = sequencing_report["Experiment"].unique()
+    experiment_dic = {item: item for item in list(unique_experiments)}
+    exp_names_dir = os.path.join(module_dir,
+                                 "my_experiments",
+                                 experiment,
+                                 "experiment_names.pickle")
+    with open(exp_names_dir, "wb") as f:
+        pickle.dump(experiment_dic, f)
+
+    if all_alignment_reports.shape[0] == 0:
+        print(
+            "No Alignment Reports were uploaded. You will continue the analysis without being able to analyze the Alignment Quality.")
+    else:
+        try:
+            all_alignment_reports = check_completeness(all_alignment_reports, sequencing_report)
+        except:
+            pass
+    exp_name_path = os.path.join(module_dir,
+                                 "my_experiments",
+                                 experiment,
+                                 "experiment_names.pickle")
+
+    unique_experiments = sequencing_report["Experiment"].unique()
+    experiment_dic = {item: item for item in list(unique_experiments)}
+
+    with open(exp_name_path, "wb") as f:
+        pickle.dump(experiment_dic, f)
+    return sequencing_report, all_alignment_reports
+
+def method_three():
+    try:
+        print("choose the file where you store your sequencing report")
+        f = filedialog.askopenfilename()
+        sequencing_report = pd.read_table(f, sep=",")
+    except:
+        while True:
+            f = input("give the path to your file which is the sequencing report")
+            f = os.path.abspath(f)
+            if os.path.isfile(f):
+                sequencing_report = pd.read_table(f, sep=",")
+                break
+            else:
+                print("Sorry, but the filepath you entered is invalid.")
+    all_alignment_reports = None
+    return sequencing_report,all_alignment_reports
+
 def upload():
     module_dir = os.path.abspath("")
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     glob_vars = os.path.join(pkg_path,
                              "settings",
                              "global_vars.txt")
     with open(glob_vars, "r") as f:
         data = f.read()
     data = literal_eval(data)
 
     last_experiment = data["last_experiment"]
-    repo_path = os.path.join(module_dir, "my_experiments", "last_experiment", "sequencing_report.txt")
+    repo_path = os.path.join(module_dir,
+                             "my_experiments",
+                             "last_experiment",
+                             "sequencing_report.txt")
 
     if os.path.isfile(repo_path):
         continue_analysis = input("Do you want to continue to analyze with " + last_experiment + "? Y/n")
         if continue_analysis.lower() in ["n", "N"]:
             next_step = input("If you want to upload a new experiment press 1. If you want to choose another experiment press 2")
             if next_step == "1":
-                experiment = input("How do you want to call your new experiment?")
+                experiment = check_experiment(module_dir)
+
                 choose_method = input("If you want to process your data with mixcr press 1. If you want to upload already processed txt files with unique clones, press 2")
                 if choose_method == "1":
-                    use_method = input("Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
-                    if use_method == "":
-                        method = "milab-human-tcr-dna-multiplex-cdr3"
-                    else:
-                        method = use_method
-                    paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
-                    if paired_end.lower() in ["Y", "y"]:
-                        paired_end = True
-                    else:
-                        paired_end = False
-                    process_mixcr(experiment,
-                                    method = method,
-                                    paired_end_sequencing = paired_end)
-
-                    with open(repo_path, "rb") as f:
-                        sequencing_report = pd.read_table(f, sep=",")
-                    try:
-                        align_repo_path = os.path.join(module_dir,
-                                                       "my_experiemnts",
-                                                       experiment,
-                                                       "alignment_reports",
-                                                       "*")
-                        alignment_reports = glob(align_repo_path)
-                        all_alignment_reports = load_alignment_reports(alignment_reports)
-                    except:
-                        all_alignment_reports = pd.DataFrame([])
-                        print("No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+                    sequencing_report, all_alignment_reports = method_one(experiment, repo_path, module_dir)
                 if choose_method == "2":
-                    experiment = input("How do you want to call your experiment?")
-                    print("Choose the folder which contains the sequencing_report and the alignment reports.")
+                    sequencing_report, all_alignment_reports = method_two(module_dir, experiment)
 
-                    try:
-                        try:
-                            print("choose the directory where you store you alignment reports and your sequencing report")
-                            filenames_dir = filedialog.askdirectory()
-                            filenames = glob(filenames_dir)
-                            for i in filenames:
-                                if os.path.isdir(i):
-                                    if "alignment_reports" in i:
-                                        alignment_repos = glob(i)
-                                        filenames.extend(alignment_repos)
-                        except:
-                            filenames_dir = input("Enter the directory where you store the alignment reports and your sequencing report manually.")
-                            filenames_dir = os.path.abspath(filenames_dir)
-                            filenames = glob(filenames_dir)
-                            for i in filenames:
-                                if os.path.isdir(i):
-                                    if "alignment_reports" in i:
-                                        alignment_repos = glob(i)
-                                        filenames.extend(alignment_repos)
-                        sequencing_report, all_alignment_reports = load_mixed_files(filenames)
-                        if sequencing_report.shape[0] == 0:
-                            print("Something went wrong. Unfortunately you could not collect the data in the sequencing report. Please make sure that you have chosen the right directory and that you have tsv files as output from mixcr in that directory.")
-                            sys.exit()
-                        trim_data = input("Do you need to trim your data? (Y/n)")
-                        if trim_data.lower() in ["Y", "y"]:
-                                sequencing_report = trimming(sequencing_report,
-                                                            divisible_by=3,                   # might be possible that columns are different
-                                                            min_count=1,
-                                                            new_fraction="cloneFraction")
-                        else:
-                            pass
-                        seq_report_dir = os.path.join(module_dir,
-                                                      "my_experiments",
-                                                      experiment,
-                                                      "sequencing_report.csv")
-                        sequencing_report.to_csv(seq_report_dir)
-                        unique_experiments = sequencing_report["Experiment"].unique()
-                        experiment_dic = {item: item for item in list(unique_experiments)}
-                        exp_names_dir = os.path.join(module_dir,
-                                                     "my_experiments",
-                                                     experiment,
-                                                     "experiment_names.pickle")
-                        with open(exp_names_dir, "wb") as f:
-                            pickle.dump(experiment_dic, f)
-                    except:
-                        print("The system could not find any files.")
-                        sys.exit()
-                    if all_alignment_reports.shape[0] == 0:
-                        print(
-                            "No Alignment Reports were uploaded. You will continue the analysis without being able to analyze the Alignment Quality.")
-                    else:
-                        try:
-                            all_alignment_reports = check_completeness(all_alignment_reports, sequencing_report)
-                        except:
-                            pass
-                    exp_name_path = os.path.join(module_dir,
-                                                 "my_experiments",
-                                                 experiment,
-                                                 "experiment_names.pickle")
-                    try:
-                        unique_experiments = sequencing_report["Experiment"].unique()
-                        experiment_dic = {item: item for item in list(unique_experiments)}
-
-                        with open(exp_name_path, "wb") as f:
-                            pickle.dump(experiment_dic, f)
-                    except:
-                        col_name = input("Please type in the exact column name which contains the name of the samples")
-                        unique_experiments = sequencing_report[col_name].unique()
-                        experiment_dic = {item: item for item in list(unique_experiments)}
-                        with open(exp_name_path, "wb") as f:
-                            pickle.dump(experiment_dic, f)
 
                 if choose_method == "3":
-                    try:
-                        print("choose the file where you store your sequencing report")
-                        f = filedialog.askopenfilename()
-                        sequencing_report = pd.read_table(f, sep=",")
-                    except:
-                        while True:
-                            f = input("give the path to your file which is the sequencing report")
-                            f = os.path.abspath(f)
-                            if os.path.isfile(f):
-                                sequencing_report = pd.read_table(f, sep=",")
-                                break
-                            else:
-                                print("Sorry, but the filepath you entered is invalid.")
-                    all_alignment_reports = None
+                    sequencing_report, all_alignment_reports = method_three()
 
             if next_step == "2":
                 while True:
                     user_input = input("Enter the name of the experiment you want to analyze")
 
                     user_input = user_input  # Try to convert the input to an integer
                     spec_exp_name_path = os.path.join(module_dir,
@@ -207,101 +250,20 @@
                 all_alignment_reports = load_alignment_reports(alignment_reports)
             except:
                 all_alignment_reports = pd.DataFrame([])
                 print(
                     "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
 
     else:
-        experiment = input("How do you want to call your experiment?")
-        choose_method = input("Welcome to ExpoSeq. If you want to start by processing your fastq files with mixcr press 1. If you want to upload already processed files press 2. If you want to upload a sequencing report press 3.")
 
+        choose_method = input("Welcome to ExpoSeq. If you want to start by processing your fastq files with mixcr press 1. If you want to upload already processed files press 2. If you want to upload a sequencing report press 3.")
+        experiment = check_experiment(module_dir)
         if choose_method == "1":
-            use_method = input(
-                "Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
-            if use_method == "":
-                method = "milab-human-tcr-dna-multiplex-cdr3"
-            else:
-                method = use_method
-            paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
-            if paired_end.lower() in ["Y", "y"]:
-                paired_end = True
-            else:
-                paired_end = False
-            process_mixcr(experiment,
-                          method=method,
-                          paired_end_sequencing=paired_end)
-            seq_report_path = os.path.join(module_dir,
-                                           "my_experiments",
-                                           experiment,
-                                           "sequencing_report.txt")
-            with open(seq_report_path, "rb") as f:
-                sequencing_report = pd.read_table(f, sep=",")
-            try:
-                align_repo_path = os.path.join(module_dir,
-                                               "my_experiments",
-                                               experiment,
-                                               "alignment_reports",
-                                               "*")
-                alignment_reports = glob(align_repo_path)
-                all_alignment_reports = load_alignment_reports(alignment_reports)
-            except:
-                all_alignment_reports = pd.DataFrame([])
-                print(
-                    "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+            sequencing_report, all_alignment_reports = method_one(experiment, repo_path, module_dir)
         else:
             pass
         if choose_method == "2":
-            experiment = input("How do you want to call your experiment")
-            print("Choose the folder which contains the txt files with the Alignment Reports and the Sequencing Reports. Please avoid having other text files in this folder.")
-            filenames = collectFiles()
-            try:
-                sequencing_report, all_alignment_reports = load_mixed_files(filenames)
-             #   trim_data = input("Do you need to trim your data? (Y/n)")
-        #        if trim_data.lower() in ["Y", "y"]:
-         #           sequencing_report = trimming(sequencing_report,
-          #                                       divisible_by=3,                   # might be possible that columns are different
-           #                                      min_count=1,
-            #                                     new_fraction="cloneFraction")
-             #   else:
-              #      pass
-            except:
-                sys.exit()
-            if all_alignment_reports.shape[0] == 0:
-                print(
-                    "No Alignment Reports were uploaded. You will continue the analysis without being able to analyze the Alignment Quality.")
-            else:
-                all_alignment_reports = check_completeness(all_alignment_reports, sequencing_report)
-            exp_name_path = os.path.join(module_dir,
-                                         "my_experiments",
-                                         experiment,
-                                         "experiment_names.pickle")
-            try:
-                unique_experiments = sequencing_report["Experiment"].unique()
-                experiment_dic = {item: item for item in list(unique_experiments)}
-
-                with open(exp_name_path, "wb") as f:
-                    pickle.dump(experiment_dic, f)
-            except:
-                col_name = input("Please type in the exact column name which contains the name of the samples")
-                unique_experiments = sequencing_report[col_name].unique()
-                experiment_dic = {item: item for item in list(unique_experiments)}
-                with open(exp_name_path, "wb") as f:
-                    pickle.dump(experiment_dic, f)
-        else:
-            pass
+            sequencing_report, all_alignment_reports = method_two(module_dir, experiment)
         if choose_method == "3":
-            try:
-                print("choose the file where you store your sequencing report")
-                f = filedialog.askopenfilename()
-                sequencing_report = pd.read_table(f, sep=",")
-            except:
-                while True:
-                    f = input("give the path to your file which is the sequencing report")
-                    f = os.path.abspath(f)
-                    if os.path.isfile(f):
-                        sequencing_report = pd.read_table(f, sep=",")
-                        break
-                    else:
-                        print("Sorry, but the filepath you entered is invalid.")
-            all_alignment_reports = None
+            sequencing_report, all_alignment_reports = method_three()
 
     return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.0.3/src/ExpoSeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.0.3/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/reset.py` & `ExpoSeq-1.0.3/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/run.py` & `ExpoSeq-1.0.3/src/ExpoSeq/run.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.0.3/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.0.3/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.0.3/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.0.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.0.3/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.2
+Version: 1.0.3
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: s220672@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.0.2/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.0.3/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

