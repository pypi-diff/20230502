# Comparing `tmp/simplyfire-0.4.2.tar.gz` & `tmp/simplyfire-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplyfire-0.4.2.tar", last modified: Wed Mar 30 06:26:30 2022, max compression
+gzip compressed data, was "simplyfire-0.5.1.tar", last modified: Mon May  1 23:29:11 2023, max compression
```

## Comparing `simplyfire-0.4.2.tar` & `simplyfire-0.5.1.tar`

### file list

```diff
@@ -1,103 +1,93 @@
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.365979 simplyfire-0.4.2/
--rw-rw-rw-   0        0        0    33092 2022-03-30 05:43:27.000000 simplyfire-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       66 2022-03-30 05:43:27.000000 simplyfire-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1960 2022-03-30 06:26:30.365979 simplyfire-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2022-03-30 06:15:49.000000 simplyfire-0.4.2/README.md
--rw-rw-rw-   0        0        0      108 2022-03-30 05:43:27.000000 simplyfire-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0      170 2022-03-30 06:26:30.369979 simplyfire-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2550 2022-03-30 06:25:58.000000 simplyfire-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.228099 simplyfire-0.4.2/simplyfire/
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/__init__.py
--rw-rw-rw-   0        0        0     2236 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/__main__.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.261106 simplyfire-0.4.2/simplyfire/__pycache__/
--rw-rw-rw-   0        0        0      163 2022-03-30 05:49:01.000000 simplyfire-0.4.2/simplyfire/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    10931 2022-03-30 05:49:01.000000 simplyfire-0.4.2/simplyfire/__pycache__/app.cpython-310.pyc
--rw-rw-rw-   0        0        0    15816 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/app.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.267108 simplyfire-0.4.2/simplyfire/backend/
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/backend/__init__.py
--rw-rw-rw-   0        0        0    15680 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/backend/interface.py
--rw-rw-rw-   0        0        0    22133 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/backend/interpreter.py
--rw-rw-rw-   0        0        0     4163 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/backend/plugin_manager.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.284728 simplyfire-0.4.2/simplyfire/img/
--rw-rw-rw-   0        0        0      239 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/arrow.png
--rw-rw-rw-   0        0        0   123774 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/loading.gif
--rw-rw-rw-   0        0        0   108307 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/logo.ico
--rw-rw-rw-   0        0        0   106769 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/logo_bw.ico
--rw-rw-rw-   0        0        0      255 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/pan_up.png
--rw-rw-rw-   0        0        0      553 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/x_zoom_in.png
--rw-rw-rw-   0        0        0      482 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/x_zoom_out.png
--rw-rw-rw-   0        0        0      528 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/y_zoom_in.png
--rw-rw-rw-   0        0        0      506 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/y_zoom_out.png
--rw-rw-rw-   0        0        0      597 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/img/zoom_in_y.png
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.299146 simplyfire-0.4.2/simplyfire/layout/
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/__init__.py
--rw-rw-rw-   0        0        0    28853 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/batch_popup.py
--rw-rw-rw-   0        0        0    12580 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/graph_panel.py
--rw-rw-rw-   0        0        0     4461 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/log_display.py
--rw-rw-rw-   0        0        0     8567 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/menubar.py
--rw-rw-rw-   0        0        0     5979 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/plugin_tab.py
--rw-rw-rw-   0        0        0     2635 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/results_display.py
--rw-rw-rw-   0        0        0    12488 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/setting_tab.py
--rw-rw-rw-   0        0        0    16174 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/layout/trace_display.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.208825 simplyfire-0.4.2/simplyfire/plugins/
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.302147 simplyfire-0.4.2/simplyfire/plugins/comparison_plot/
--rw-rw-rw-   0        0        0    15742 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/comparison_plot/comparison_GUI.py
--rw-rw-rw-   0        0        0      200 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/comparison_plot/plugin.yaml
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.307148 simplyfire-0.4.2/simplyfire/plugins/evoked_basic/
--rw-rw-rw-   0        0        0    15452 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/evoked_basic/evoked_GUI.py
--rw-rw-rw-   0        0        0     2721 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/evoked_basic/evoked_analysis.py
--rw-rw-rw-   0        0        0      232 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/evoked_basic/plugin.yaml
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.312149 simplyfire-0.4.2/simplyfire/plugins/mini_analysis/
--rw-rw-rw-   0        0        0    88598 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/mini_analysis/mini_GUI.py
--rw-rw-rw-   0        0        0    62039 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/mini_analysis/mini_analysis.py
--rw-rw-rw-   0        0        0      236 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/mini_analysis/plugin.yaml
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.314149 simplyfire-0.4.2/simplyfire/plugins/navigation/
--rw-rw-rw-   0        0        0     8946 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/navigation/navigation.py
--rw-rw-rw-   0        0        0      172 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/navigation/plugin.yaml
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.319151 simplyfire-0.4.2/simplyfire/plugins/process_recording/
--rw-rw-rw-   0        0        0      254 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/process_recording/plugin.yaml
--rw-rw-rw-   0        0        0    20425 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/process_recording/process_GUI.py
--rw-rw-rw-   0        0        0     5410 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/process_recording/process_recording.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.322155 simplyfire-0.4.2/simplyfire/plugins/style/
--rw-rw-rw-   0        0        0      199 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/style/plugin.yaml
--rw-rw-rw-   0        0        0     5451 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/style/style_tab.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.325152 simplyfire-0.4.2/simplyfire/plugins/sweeps/
--rw-rw-rw-   0        0        0      201 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/sweeps/plugin.yaml
--rw-rw-rw-   0        0        0    14881 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/plugins/sweeps/sweeps_GUI.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.330153 simplyfire-0.4.2/simplyfire/setting/
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.333154 simplyfire-0.4.2/simplyfire/setting/__pycache__/
--rw-rw-rw-   0        0        0      171 2022-03-30 05:49:01.000000 simplyfire-0.4.2/simplyfire/setting/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3986 2022-03-30 05:49:01.000000 simplyfire-0.4.2/simplyfire/setting/__pycache__/config.cpython-310.pyc
--rw-rw-rw-   0        0        0     6453 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/setting/config.py
--rw-rw-rw-   0        0        0     3493 2022-03-30 06:26:01.000000 simplyfire-0.4.2/simplyfire/setting/default_config.yaml
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.336155 simplyfire-0.4.2/simplyfire/temp/
--rw-rw-rw-   0        0        0      218 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/temp/README.md
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/temp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.358977 simplyfire-0.4.2/simplyfire/utils/
--rw-rw-rw-   0        0        0        0 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.363978 simplyfire-0.4.2/simplyfire/utils/__pycache__/
--rw-rw-rw-   0        0        0      169 2022-03-30 05:49:50.000000 simplyfire-0.4.2/simplyfire/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    21766 2022-03-30 05:49:50.000000 simplyfire-0.4.2/simplyfire/utils/__pycache__/custom_widgets.cpython-310.pyc
--rw-rw-rw-   0        0        0     3031 2022-03-30 05:49:50.000000 simplyfire-0.4.2/simplyfire/utils/__pycache__/validation.cpython-310.pyc
--rw-rw-rw-   0        0        0     6411 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/abfWriter.py
--rw-rw-rw-   0        0        0     6620 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/calculate.py
--rw-rw-rw-   0        0        0    23659 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/custom_widgets.py
--rw-rw-rw-   0        0        0     3311 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/formatting.py
--rw-rw-rw-   0        0        0     2932 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/plugin_GUI.py
--rw-rw-rw-   0        0        0     8664 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/plugin_controller.py
--rw-rw-rw-   0        0        0     7778 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/plugin_form.py
--rw-rw-rw-   0        0        0     1900 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/plugin_popup.py
--rw-rw-rw-   0        0        0     8023 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/plugin_table.py
--rw-rw-rw-   0        0        0    18140 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/recording.py
--rw-rw-rw-   0        0        0    11690 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/scrollable_option_frame.py
--rw-rw-rw-   0        0        0     2651 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/threader.py
--rw-rw-rw-   0        0        0     3932 2022-03-30 05:43:27.000000 simplyfire-0.4.2/simplyfire/utils/validation.py
-drwxrwxrwx   0        0        0        0 2022-03-30 06:26:30.258105 simplyfire-0.4.2/simplyfire.egg-info/
--rw-rw-rw-   0        0        0     1960 2022-03-30 06:26:29.000000 simplyfire-0.4.2/simplyfire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2830 2022-03-30 06:26:30.000000 simplyfire-0.4.2/simplyfire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-30 06:26:29.000000 simplyfire-0.4.2/simplyfire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-03-30 06:26:29.000000 simplyfire-0.4.2/simplyfire.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-03-30 05:48:59.000000 simplyfire-0.4.2/simplyfire.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2022-03-30 06:26:30.000000 simplyfire-0.4.2/simplyfire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-30 06:26:30.000000 simplyfire-0.4.2/simplyfire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.767148 simplyfire-0.5.1/
+-rw-rw-rw-   0        0        0    33092 2023-05-01 23:06:43.000000 simplyfire-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       66 2023-05-01 23:06:43.000000 simplyfire-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1947 2023-05-01 23:29:11.767148 simplyfire-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-05-01 23:06:43.000000 simplyfire-0.5.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-01 23:06:43.000000 simplyfire-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      170 2023-05-01 23:29:11.768199 simplyfire-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2564 2023-05-01 23:27:17.000000 simplyfire-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.558971 simplyfire-0.5.1/simplyfire/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/__main__.py
+-rw-rw-rw-   0        0        0    15816 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/app.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.582279 simplyfire-0.5.1/simplyfire/backend/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/__init__.py
+-rw-rw-rw-   0        0        0    16487 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/interface.py
+-rw-rw-rw-   0        0        0    22220 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/interpreter.py
+-rw-rw-rw-   0        0        0     4163 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/plugin_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.597229 simplyfire-0.5.1/simplyfire/img/
+-rw-rw-rw-   0        0        0      239 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/arrow.png
+-rw-rw-rw-   0        0        0   123774 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/loading.gif
+-rw-rw-rw-   0        0        0   108307 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/logo.ico
+-rw-rw-rw-   0        0        0   106769 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/logo_bw.ico
+-rw-rw-rw-   0        0        0      255 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/pan_up.png
+-rw-rw-rw-   0        0        0      553 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/x_zoom_in.png
+-rw-rw-rw-   0        0        0      482 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/x_zoom_out.png
+-rw-rw-rw-   0        0        0      528 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/y_zoom_in.png
+-rw-rw-rw-   0        0        0      506 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/y_zoom_out.png
+-rw-rw-rw-   0        0        0      597 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/zoom_in_y.png
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.630742 simplyfire-0.5.1/simplyfire/layout/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/__init__.py
+-rw-rw-rw-   0        0        0    28853 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/batch_popup.py
+-rw-rw-rw-   0        0        0    12580 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/graph_panel.py
+-rw-rw-rw-   0        0        0     4461 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/log_display.py
+-rw-rw-rw-   0        0        0     8569 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/menubar.py
+-rw-rw-rw-   0        0        0     5979 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/plugin_tab.py
+-rw-rw-rw-   0        0        0     2635 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/results_display.py
+-rw-rw-rw-   0        0        0    12488 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/setting_tab.py
+-rw-rw-rw-   0        0        0    16937 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/trace_display.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.537614 simplyfire-0.5.1/simplyfire/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.640733 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/
+-rw-rw-rw-   0        0        0    15742 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/comparison_GUI.py
+-rw-rw-rw-   0        0        0      200 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.649784 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/
+-rw-rw-rw-   0        0        0    15452 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_GUI.py
+-rw-rw-rw-   0        0        0     2721 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_analysis.py
+-rw-rw-rw-   0        0        0      232 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.660456 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/
+-rw-rw-rw-   0        0        0    89249 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_GUI.py
+-rw-rw-rw-   0        0        0    61353 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_analysis.py
+-rw-rw-rw-   0        0        0      236 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.666001 simplyfire-0.5.1/simplyfire/plugins/navigation/
+-rw-rw-rw-   0        0        0     8946 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/navigation/navigation.py
+-rw-rw-rw-   0        0        0      172 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/navigation/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.673936 simplyfire-0.5.1/simplyfire/plugins/process_recording/
+-rw-rw-rw-   0        0        0      254 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/plugin.yaml
+-rw-rw-rw-   0        0        0    20784 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/process_GUI.py
+-rw-rw-rw-   0        0        0     5259 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/process_recording.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.679919 simplyfire-0.5.1/simplyfire/plugins/style/
+-rw-rw-rw-   0        0        0      199 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/style/plugin.yaml
+-rw-rw-rw-   0        0        0     5451 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/style/style_tab.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.685856 simplyfire-0.5.1/simplyfire/plugins/sweeps/
+-rw-rw-rw-   0        0        0      201 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/sweeps/plugin.yaml
+-rw-rw-rw-   0        0        0    14881 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/sweeps/sweeps_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.700600 simplyfire-0.5.1/simplyfire/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/__init__.py
+-rw-rw-rw-   0        0        0     6453 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/config.py
+-rw-rw-rw-   0        0        0     3517 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/default_config.yaml
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.702678 simplyfire-0.5.1/simplyfire/temp/
+-rw-rw-rw-   0        0        0      218 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/temp/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/temp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.763200 simplyfire-0.5.1/simplyfire/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/__init__.py
+-rw-rw-rw-   0        0        0     6411 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/abfWriter.py
+-rw-rw-rw-   0        0        0     6620 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/calculate.py
+-rw-rw-rw-   0        0        0    23659 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/custom_widgets.py
+-rw-rw-rw-   0        0        0     3311 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/formatting.py
+-rw-rw-rw-   0        0        0     2932 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_GUI.py
+-rw-rw-rw-   0        0        0     8664 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_controller.py
+-rw-rw-rw-   0        0        0     7778 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_form.py
+-rw-rw-rw-   0        0        0     1900 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_popup.py
+-rw-rw-rw-   0        0        0     8023 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_table.py
+-rw-rw-rw-   0        0        0    19411 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/recording.py
+-rw-rw-rw-   0        0        0    11690 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/scrollable_option_frame.py
+-rw-rw-rw-   0        0        0     2651 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/threader.py
+-rw-rw-rw-   0        0        0     3932 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/validation.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.568961 simplyfire-0.5.1/simplyfire.egg-info/
+-rw-rw-rw-   0        0        0     1947 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2459 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 23:21:50.000000 simplyfire-0.5.1/simplyfire.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/top_level.txt
```

### Comparing `simplyfire-0.4.2/LICENSE` & `simplyfire-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/PKG-INFO` & `simplyfire-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.4.2
+Version: 0.5.1
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
-Author: Megumi Mori
+Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimplyFire
 A customizable analysis package for electrophysiologists
 
-Read the full manual [here](https://simplyfire-beta.readthedocs.io/).
+Read the full manual [here](https://simplyfire.readthedocs.io/).
 
 ## .exe Installation
 
-Download the software zip file from the recent [release](https://github.com/megumi-mori/SimplyFire-beta/releases).
+Download the software zip file from the recent [release](https://github.com/HaghighiLabBuck/SimplyFire/releases).
 You only need to download the zip file.
 
 Extract the contents of the zip file, and locate SimplyFire.exe to run the software.
 
 ## Python Installation
 If you have Python, you can install and run SimplyFire as a Python module. 
 
@@ -54,8 +53,7 @@
 Tools are provided to easily create custom plugins. 
 
 Pull-requests for fixes and additions are welcome! 
 Details on the development workflow will be available in the future. 
 
 ## License
 SimplyFire is released under the GPLv3 or later license. 
-
```

### Comparing `simplyfire-0.4.2/README.md` & `simplyfire-0.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SimplyFire
 A customizable analysis package for electrophysiologists
 
-Read the full manual [here](https://simplyfire-beta.readthedocs.io/).
+Read the full manual [here](https://simplyfire.readthedocs.io/).
 
 ## .exe Installation
 
-Download the software zip file from the recent [release](https://github.com/megumi-mori/SimplyFire-beta/releases).
+Download the software zip file from the recent [release](https://github.com/HaghighiLabBuck/SimplyFire/releases).
 You only need to download the zip file.
 
 Extract the contents of the zip file, and locate SimplyFire.exe to run the software.
 
 ## Python Installation
 If you have Python, you can install and run SimplyFire as a Python module. 
 
@@ -35,8 +35,8 @@
 SimplyFire has been written to make electrophysiology analysis straightforward, automatable, and customizable.
 Tools are provided to easily create custom plugins. 
 
 Pull-requests for fixes and additions are welcome! 
 Details on the development workflow will be available in the future. 
 
 ## License
-SimplyFire is released under the GPLv3 or later license. 
+SimplyFire is released under the GPLv3 or later license.
```

### Comparing `simplyfire-0.4.2/setup.py` & `simplyfire-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 """
 from setuptools import setup, find_packages
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='simplyfire',
-    version='0.4.2',
-    author='Megumi Mori',
+    version='0.5.1',
+    author='Megumi Mori, Andrew Rosko',
     description='Customizable electrophysiology analysis software',
     long_description=readme,
     long_description_content_type='text/markdown',
     url="https://simplyfire.readthedocs.io/",
     pakage_dir={'simplyfire':'simplyfire'},
     packages = find_packages(),
     entry_points={
```

### Comparing `simplyfire-0.4.2/simplyfire/__main__.py` & `simplyfire-0.5.1/simplyfire/__main__.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/app.py` & `simplyfire-0.5.1/simplyfire/app.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/backend/interface.py` & `simplyfire-0.5.1/simplyfire/backend/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 
 import pandas as pd
 import os
 # This module is the workhorse of the GUI
 # Use this module to connect analysis functions to the GUI
 from simplyfire.utils import abfWriter
 from simplyfire.utils.recording import Recording
+from psutil import Process
 
 mini_df = pd.DataFrame()
 current_channel = 0
 
+
 ##########################
 # Undo controls
 ##########################
 def get_temp_num():
     global temp_num
     try:
         temp_num += 1
@@ -324,41 +326,54 @@
     app.trace_display.ax.tick_params(axis='x', which='major')#, labelsize=int(float(app.inputs['font_size'].get())))
     app.root.event_generate('<<Plotted>>')
     app.root.event_generate('<<PlotDone>>')
     app.trace_display.draw_ani()
 
 
 def plot_continuous(recording, draw=False, sweep_name_suffix='Sweep', relim=True, **kwargs):
-    global current_channel
+    global current_channel, plot_mode
+    plot_mode = 'continuous'
     app.trace_display.plot_trace(recording.get_xs(mode='continuous', channel=current_channel),
                              recording.get_ys(mode='continuous', channel=current_channel),
                              draw=draw,
                              relim=relim,
                              name=f'{sweep_name_suffix}_0',
                              **kwargs)
     if draw:
         app.trace_display.draw_ani()
 
 
 def plot_overlay(recording, draw=False, sweep_name_suffix='Sweep', relim=True, **kwargs):
+    global plot_mode
+    plot_mode = 'overlay'
     for i in range(recording.sweep_count):
         app.pb['value'] = (i+1)/recording.sweep_count*100
         app.pb.update()
         xs = recording.get_xs(mode='overlay', sweep=i, channel=current_channel)
         ys = recording.get_ys(mode='overlay', sweep=i, channel=current_channel)
         app.trace_display.plot_trace(xs, ys,
                                  draw=False,
-                                 relim=(i == recording.sweep_count-1 and relim),  #relim for the final sweep
+                                 relim=(i == 0 and relim), # Relim for first sweep
+                                 ##relim=(i == recording.sweep_count-1 and relim),  #relim for the final sweep
                                  name = f"{sweep_name_suffix}_{i}",
                                  **kwargs)
     if draw:
         app.trace_display.draw_ani()
         app.trace_display.draw_ani()
     app.pb['value'] = 0
     app.pb.update()
+    
+def update_trace(trace_name,new_xlim):
+    if plot_mode == 'overlay':
+        new_xs = recordings[0].get_xs(mode='overlay', sweep=int(trace_name[-1]), channel=current_channel,xlim=new_xlim)
+        new_ys = recordings[0].get_ys(mode='overlay', sweep=int(trace_name[-1]), channel=current_channel,xlim=new_xlim)
+    elif plot_mode == 'continuous':
+        new_xs = recordings[0].get_xs(mode='continuous', sweep=None, channel=current_channel,xlim=new_xlim)
+        new_ys = recordings[0].get_ys(mode='continuous', sweep=None, channel=current_channel,xlim=new_xlim)
+    return new_xs,new_ys
 
 ######################################
 # Handling GUI placements
 ######################################
 
 # def select_left(e=None):
 #     """
```

### Comparing `simplyfire-0.4.2/simplyfire/backend/interpreter.py` & `simplyfire-0.5.1/simplyfire/backend/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,22 +167,24 @@
     app.trace_display.canvas.mpl_connect('pick_event', plot_event_pick)
     app.trace_display.canvas.mpl_connect('button_press_event', plot_mouse_press)
     app.trace_display.canvas.mpl_connect('motion_notify_event', plot_mouse_move)
     app.trace_display.canvas.mpl_connect('button_release_event', plot_mouse_release)
     app.trace_display.canvas.mpl_connect('scroll_event', plot_mouse_scroll)
     global scroll_axis
     scroll_axis = 'x'
-    def zoom_axis_press(event=None):
+    def zoom_axis_y(event=None):
         global scroll_axis
         scroll_axis = 'y'
-    def zoom_axis_release(event=None):
+    def zoom_axis_x(event=None):
         global scroll_axis
         scroll_axis = 'x'
-    for key in get_keys('zoom_axis'):
-        bind_key_dp(key, zoom_axis_press, zoom_axis_release)
+    for key in get_keys('set_zoom_axis_x'):
+        bind_key_dp(key, press_function=zoom_axis_x)
+    for key in get_keys('set_zoom_axis_y'):
+        bind_key_dp(key, press_function=zoom_axis_y)
 
 
     app.root.bind('<Alt-o>', lambda e: app.menubar.ask_open_recording())
 
     #######################################
     # Global Keys
     #######################################
```

### Comparing `simplyfire-0.4.2/simplyfire/backend/plugin_manager.py` & `simplyfire-0.5.1/simplyfire/backend/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/loading.gif` & `simplyfire-0.5.1/simplyfire/img/loading.gif`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/logo.ico` & `simplyfire-0.5.1/simplyfire/img/logo.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/logo_bw.ico` & `simplyfire-0.5.1/simplyfire/img/logo_bw.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/x_zoom_in.png` & `simplyfire-0.5.1/simplyfire/img/x_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/y_zoom_in.png` & `simplyfire-0.5.1/simplyfire/img/y_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/img/zoom_in_y.png` & `simplyfire-0.5.1/simplyfire/img/zoom_in_y.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/batch_popup.py` & `simplyfire-0.5.1/simplyfire/layout/batch_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/graph_panel.py` & `simplyfire-0.5.1/simplyfire/layout/graph_panel.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/log_display.py` & `simplyfire-0.5.1/simplyfire/layout/log_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/menubar.py` & `simplyfire-0.5.1/simplyfire/layout/menubar.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     inputs['trace_mode'].set('continuous')
     app.log_display.log('change to continuous mode')
     # switch to continuous mode tab
     # interface.config_cp_tab('continuous', state='normal')
 
     try:
         # interface.plot_continuous(interface.recordings[0], fix_axis=True)
-        interface.plot(fix_y=True, fix_x=True, relim=True)
+        interface.plot(fix_y=True, fix_x=False, relim=True)
     except:
         pass
     # if inputs['analysis_mode'].get() == 'mini':
     #     interface.config_cp_tab('mini', state='normal')
     #     interface.config_data_tab('mini', state='normal')
     # interface.config_cp_tab('adjust', state='normal')
     prev_trace_mode = 'continuous'
@@ -193,15 +193,15 @@
     #     interface.add_undo([
     #         lambda d=False: set_view_compare(d)
     #     ])
     inputs['trace_mode'].set('overlay')
     app.log_display.log('change to overlay mode')
     # interface.config_cp_tab('overlay', state='normal')
     try:
-        interface.plot(fix_x=True, fix_y=True, relim=True)
+        interface.plot(fix_x=False, fix_y=True, relim=True)
     except:
         pass
     prev_trace_mode = 'overlay'
     app.root.event_generate('<<ChangedToOverlayView>>')
     pass
 
 def undo_disable():
```

### Comparing `simplyfire-0.4.2/simplyfire/layout/plugin_tab.py` & `simplyfire-0.5.1/simplyfire/layout/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/results_display.py` & `simplyfire-0.5.1/simplyfire/layout/results_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/setting_tab.py` & `simplyfire-0.5.1/simplyfire/layout/setting_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/layout/trace_display.py` & `simplyfire-0.5.1/simplyfire/layout/trace_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.patches import Rectangle
 from matplotlib.animation import FuncAnimation
 from simplyfire import app
 import gc
 from simplyfire.utils import calculate
+from simplyfire.backend import interface
 
 sweeps = {}
 
 event_pick = False
 
 highlighted_sweep = []
 
@@ -125,15 +126,15 @@
 
     if new_lim[0] < default_xlim[0]:
         delta = default_xlim[0] - new_lim[0]
         new_lim = (new_lim[0] + delta, new_lim[1] + delta)
     elif new_lim[1] > default_xlim[1]:
         delta = new_lim[1] - default_xlim[1]
         new_lim = (new_lim[0] - delta, new_lim[1] - delta)
-    ax.set_xlim(new_lim)
+    update_x_limits_data(new_lim)
 
     global fig
     global ani
     draw_ani()
     # ani._start()
     update_x_scrollbar(new_lim)
     scroll_y_by(0)
@@ -167,15 +168,15 @@
     xlim = ax.get_xlim()
     if xlim[1] == default_xlim[1] and xlim[0] == default_xlim[0]:
         app.graph_panel.x_scrollbar.set(50)
         return None
     start = (default_xlim[1] - default_xlim[0] - (xlim[1] - xlim[0])) * float(num) / 100 + default_xlim[0]
     end = start + xlim[1] - xlim[0]
 
-    ax.set_xlim((start, end))
+    update_x_limits_data((start, end))
     global fig
     global ani
     draw_ani()
     # ani._start()
     scroll_y_by(0)
 
 
@@ -218,15 +219,15 @@
         adjust = max(0, default_xlim[0] - new_xlim_left)
         new_xlim_right += adjust
         adjust = min(0, default_xlim[1] - new_xlim_right)
         new_xlim_left += adjust
 
         new_xlim_left = max(default_xlim[0], new_xlim_left)
         new_xlim_right = min(default_xlim[1], new_xlim_right)
-        ax.set_xlim(new_xlim_left, new_xlim_right)
+        update_x_limits_data((new_xlim_left, new_xlim_right))
         update_x_scrollbar((new_xlim_left, new_xlim_right))
         new_xlim = (new_xlim_left, new_xlim_right)
 
     if ylim[0] > y or ylim[1] < y:
         ylim_width = ylim[1] - ylim[0]
         new_ylim_bottom = y - ylim_width / 2
         new_ylim_top = y + ylim_width / 2
@@ -256,15 +257,15 @@
         new_xlim_right = min(max(xlim[1], x2 + padx), default_xlim[1])
 
     pady = (y2 - y1) * pad
 
     new_ylim_bottom = min(ylim[0], y1 - pady)
     new_ylim_top = max(ylim[1], y2 + pady)
 
-    ax.set_xlim(new_xlim_left, new_xlim_right)
+    update_x_limits_data((new_xlim_left, new_xlim_right))
     update_x_scrollbar((new_xlim_left, new_xlim_right))
     ax.set_ylim(new_ylim_bottom, new_ylim_top)
     update_y_scrollbar(xlim=(new_xlim_left, new_xlim_right), ylim=(new_ylim_bottom, new_ylim_top))
 
     # canvas.draw()
     draw_ani()
 
@@ -288,15 +289,15 @@
     if new_lim[0] < default_xlim[0]:
         width = new_lim[1] - new_lim[0]
         new_lim = (default_xlim[0], min(new_lim[0] + width, default_xlim[1]))
     elif new_lim[1] > default_xlim[1]:
         width = new_lim[1] - new_lim[0]
         new_lim = (max(new_lim[1] - width, default_xlim[0]), default_xlim[1])
 
-    ax.set_xlim(new_lim)
+    update_x_limits_data(new_lim)
     global fig
     global ani
     # ani = FuncAnimation(
     #     fig,
     #     anim_func,
     #     frames=1,
     #     interval = int(1),
@@ -395,45 +396,62 @@
 
 def plot_trace(xs, ys, draw=True, relim=True, idx=0, color=None, width=None, name="", relim_axis='both'):
     global sweeps
     global trace_color
     global trace_width
     if not width:
         width=trace_width
+    if relim:
+        ax.autoscale(enable=False, axis='both')
+        ax.relim(visible_only=True)
+        # canvas.draw()
+        draw_ani()
+        if relim_axis == 'x' or relim_axis == 'both':
+            minX = min(xs)
+            maxX = max(xs)
+            global default_xlim
+            if len(xs) > 100000:
+                ax.set_xlim(minX,xs[99999])
+            else:
+                ax.set_xlim(minX,maxX)
+            default_xlim = (minX,maxX)
+        if relim_axis == 'y' or relim_axis == 'both':
+            ax.autoscale(enable=True, axis='y', tight=True)
+            global default_ylim
+            default_ylim = ax.get_ylim()    
+    	
     if name == "":
         name = f'Sweep_{len(sweeps)}'
+    	
+    xlims = ax.get_xlim()
+    ## Check to see if bounds of trace should be clipped
+    if xlims[0] > xs[0] or xlims[1] < xs[-1]:
+        xs,ys = interface.update_trace(name,xlims)
     if sweeps.get(name, None):
         sweeps.get(name).set_xdata(xs)
         sweeps.get(name).set_ydata(ys)
     else:
         if not color:
             # color = app.widgets['style_trace_line_color'].get()
             color = trace_color
         sweeps[name], = ax.plot(xs, ys,
                                               linewidth=width,
                                               c=color,
                                               animated=False)  # pickradius=int(app.widgets['style_event_pick_offset'].get())
-    if relim:
-        ax.autoscale(enable=False, axis='both')
-        ax.autoscale(enable=True, axis=relim_axis, tight=True)
-        ax.relim(visible_only=True)
-        # canvas.draw()
-        draw_ani()
-        if relim_axis == 'x' or relim_axis == 'both':
-            global default_xlim
-            default_xlim = ax.get_xlim()
-        if relim_axis == 'y' or relim_axis =='both':
-            global default_ylim
-            default_ylim = ax.get_ylim()
-
-
     if draw:
         # canvas.draw()
         # refresh()
         draw_ani()
+		
+def update_x_limits_data(new_lims):
+    for name, sweep in sweeps.items():
+        new_x,new_y = interface.update_trace(name,new_lims)
+        sweep.set_xdata(new_x)
+        sweep.set_ydata(new_y)
+    ax.set_xlim(new_lims)
 
 def hide_sweep(idx, draw=False):
     try:
         sweeps['sweep_{}'.format(idx)].set_linestyle('None')
         # del sweeps['sweep_{}'.format(idx)]
     except:
         pass
@@ -465,27 +483,28 @@
     if update_default:
         global default_xlim
         default_xlim = ax.get_xlim()
         global default_ylim
         default_ylim = ax.get_ylim()
 
 def update_default_lim(x=True, y=True, fix_x=False, fix_y=False):
+    print('update_default_lim')
     xlim = ax.get_xlim()
     ylim = ax.get_ylim()
     ax.autoscale(enable=True, axis='both', tight=True)
     ax.relim(visible_only=True)
     draw_ani()
     if x:
         global default_xlim
         default_xlim = ax.get_xlim()
     if y:
         global default_ylim
         default_ylim = ax.get_ylim()
     if fix_x:
-        ax.set_xlim(xlim)
+        update_x_limits_data(xlim)
     if fix_y:
         ax.set_ylim(ylim)
 
 get_axis_limits = lambda axis: getattr(ax, 'get_{}lim'.format(axis))()
 
 def adjust_default_ylim(adjust):
     global default_ylim
@@ -495,15 +514,15 @@
 def set_axis_limit(axis, lim, draw=True):
     if axis == 'x':
         l = [float(e) if e != 'auto' else default_xlim[i] for i, e in enumerate(lim)]
         if l[0] < default_xlim[0] or l[0] > default_xlim[1]:
             l[0] = default_xlim[0]
         if l[1] < default_xlim[0] or l[1] > default_xlim[1]:
             l[1] = default_xlim[1]
-        ax.set_xlim(l)
+        update_x_limits_data(l)
     if axis == 'y':
         l = [float(e) if e != 'auto' else default_ylim[i] for i, e in enumerate(lim)]
         ax.set_ylim(l)
     # canvas.draw()
     if draw:
         draw_ani()
```

### Comparing `simplyfire-0.4.2/simplyfire/plugins/comparison_plot/comparison_GUI.py` & `simplyfire-0.5.1/simplyfire/plugins/comparison_plot/comparison_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/plugins/evoked_basic/evoked_GUI.py` & `simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/plugins/evoked_basic/evoked_analysis.py` & `simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_analysis.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/plugins/mini_analysis/mini_GUI.py` & `simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,37 +561,34 @@
 def _find_mini_all_thread(undo=True):
     """
     Used to call the find-all algorithm from the mini_analysis module.
     Use this inside of a thread
     """
     global mini_df
     params = get_params()
-    try:
-        xs = app.trace_display.sweeps['Sweep_0'].get_xdata()
-        ys = app.trace_display.sweeps['Sweep_0'].get_ydata()
-    except:  # no traces yet
-        return
-    df = mini_analysis.find_mini_auto(xlim=None, xs=xs, ys=ys, x_sigdig=app.interface.recordings[0].x_sigdig,
+    df = mini_analysis.find_mini_auto(xlim=None, xs=None, ys=None, x_sigdig=app.interface.recordings[0].x_sigdig,
                                          sampling_rate=app.interface.recordings[0].sampling_rate,
                                          channel=app.interface.current_channel,
+                                         recording = app.interface.recordings[0],
                                          reference_df=mini_df, y_unit=app.interface.recordings[0].y_unit,
                                          x_unit=app.interface.recordings[0].x_unit, progress_bar=app.pb, **params)
     mini_df = pd.concat([mini_df, df])
     global saved
     undo_stack = []
     if df.shape[0] > 0:
         # if int(app.widgets['config_undo_stack'].get()) > 0:
         #     add_undo([
         #         lambda iid=df['t'].values, u=False: delete_event(iid, undo=u),
         #         lambda msg='Undo mini search': detector_tab.log(msg)
         #     ])
         update_event_markers(draw=True)
         datapanel.append(df, undo=False)
         saved = False  # track change
-        if undo and app.interface.is_accepting_undo():
+##        if undo and app.interface.is_accepting_undo():
+        if False:
             undo_stack.append(
                 lambda s=df[df.channel == app.interface.current_channel]['t']: delete_selection(s, undo=False)
             )
     undo_stack.append(lambda msg=f'Undo find mini all. Delete {df.shape[0]} minis':controller.log(msg))
     controller.add_undo(undo_stack)
 
     app.clear_progress_bar()
@@ -1138,82 +1135,82 @@
     if not x or not y:
         return
     popup.ax.plot((x, x), (y, baseline),
                   linewidth=app.trace_display.trace_width,
                   c='black',
                   alpha=0.9)
 
-def popup_plot_base_extrapolate(xs, end, data):
+def popup_plot_base_extrapolate(xs, idx_offset, end, data):
     """
     Plot the baseline on the popup guide, as extrapolation from the decay of the previous peak
     """
     global popup_tracker
     popup_tracker = True
 
-    xs = xs[int(data['prev_peak_idx']):end]
+    xs = xs[int(data['prev_peak_idx'])-idx_offset:end]
     A = data['prev_decay_A']
     decay = data['prev_decay_const'] / 1000
     baseline = data['prev_baseline']
     direction = data['direction']
     prev_direction = data['prev_mini_direction']
     popup.ax.plot(xs, mini_analysis.single_exponent(xs - xs[0], A, decay) * prev_direction + baseline,
                   linewidth=app.trace_display.trace_width,
                   c='black',
                   alpha=0.9,
                   label='Prev decay'
                   )
 
-def popup_plot_base_range(xs, ys, data):
+def popup_plot_base_range(xs, ys, idx_offset, data):
     """
     Plot info on the popup guide.
     Marks the datapoints that were referenced to estimate the baseline
     """
-    popup.ax.plot(xs[int(data['base_idx_L']): int(data['base_idx_R'])],
-                  ys[int(data['base_idx_L']): int(data['base_idx_R'])],
+    popup.ax.plot(xs[int(data['base_idx_L'])-idx_offset: int(data['base_idx_R'])-idx_offset],
+                  ys[int(data['base_idx_L'])-idx_offset: int(data['base_idx_R'])-idx_offset],
                   linewidth=app.trace_display.trace_width * 3,
                   c='pink',
                   alpha=0.9,
                   label='Baseline sample')
 
-def popup_plot_base_simple(xs, end, data):
+def popup_plot_base_simple(xs, idx_offset, end, data):
     """
     Plot info on the popup guide.
     Creates a horizontal line marking the baseline value.
     """
-    x1 = xs[int(data['start_idx'])]
+    x1 = xs[int(data['start_idx'])-idx_offset]
     x2 = xs[end]
     baseline = data['baseline']
     popup.ax.plot([x1, x2], [baseline, baseline],
                   linewidth=app.trace_display.trace_width,
                   c='black',
                   alpha=0.9)
 
-def popup_plot_decay_fit(xs, end, data):
+def popup_plot_decay_fit(xs, idx_offset, end, data):
     """
     Plot info on the popup guide
     Plot a single-exponential decay
     """
-    xs = xs[int(data['peak_idx']):end]
+    xs = xs[int(data['peak_idx'])-idx_offset:end]
     A = data['decay_A']
     tau = data['decay_const'] / 1000
     decay_base = data['decay_baseline']  # support for constant
     baseline = data['baseline']
     direction = data['direction']
     guide_markers['decay_fit'], = popup.ax.plot(xs,
                   mini_analysis.single_exponent_constant(xs - xs[0], A, tau, decay_base) * direction + baseline,
                   linewidth=app.trace_display.trace_width,
                   c=decay_color,
                   label='Decay fit')
 
-def popup_plot_decay_extrapolate(xs, end, data):
+def popup_plot_decay_extrapolate(xs, idx_offset, end, data):
     """
     Plot info on the popup guide
     Plot the single-exponential decay offset by the decay of the previous mini of the compound mini
     """
-    xs = xs[int(data['peak_idx']):end]
+    xs = xs[int(data['peak_idx'])-idx_offset:end]
     A = data['decay_A']
     tau = data['decay_const'] / 1000
     decay_base = data['decay_baseline']  # support for constant
     baseline = data['baseline']
     direction = data['direction']
 
     ys = mini_analysis.single_exponent_constant(xs - xs[0], A, tau, decay_base) * direction
@@ -1262,36 +1259,39 @@
     global popup_peak
     popup_peak, = popup.ax.plot(x, y, marker='o', c=peak_color,
                              markersize=peak_size,
                              linestyle='None',
                              label='Peak')
     guide_markers['peak'] = popup_peak
 
-def popup_plot_recording(xs, ys, data):
-    start_lim_idx = int(max(data.get('start_idx', 0) - data.get('lag', 0) - data.get('delta_x', 0), 0))
-    xlim_idx_L = data.get('xlim_idx_L')
+def popup_plot_recording(xs, ys, idx_offset, data):
+    start_lim_idx = int(max(data.get('start_idx', 0) - data.get('lag', 0) - data.get('delta_x', 0) - idx_offset, 0))
+    xlim_idx_L = data.get('xlim_idx_L') - idx_offset
     if xlim_idx_L is None:
         xlim_idx_L = np.inf
     start_idx = int(min(start_lim_idx, xlim_idx_L))
     if data['compound']:
-        start_idx = int(min(start_idx, int(data['prev_peak_idx'])))
+        start_idx = int(min(start_idx, int(data['prev_peak_idx'])-idx_offset))
 
-    end_lim_idx = int(min(data.get('peak_idx', 0) + data.get('decay_max_points', 0), len(xs) - 1))
-    xlim_idx_R = data.get('xlim_idx_R')
+    end_lim_idx = int(min(data.get('peak_idx', 0) + data.get('decay_max_points', 0) - idx_offset, len(xs) - 1))
+    xlim_idx_R = data.get('xlim_idx_R') - idx_offset
     if xlim_idx_R is None:
         xlim_idx_R = 0
     end_idx = int(max(end_lim_idx, xlim_idx_R))
+    
+    print(start_idx)
+    print(end_idx)
 
     popup.ax.plot(xs[start_idx:end_idx],
                  ys[start_idx:end_idx],
                  linewidth=app.trace_display.trace_width,
                  color=app.trace_display.trace_color,
                  )
     popup.ax.set_xlim((xs[start_lim_idx], xs[end_lim_idx]))
-    popup_plot_start(xs[int(data['start_idx'])], ys[int(data['start_idx'])])
+    popup_plot_start(xs[int(data['start_idx'])-idx_offset], ys[int(data['start_idx']-idx_offset)])
     return start_idx, end_idx
 
 def popup_plot_start(x, y):
     guide_markers['start'], = popup.ax.plot(x, y, marker='x', c=start_color,
                  markersize=start_size,
                  label='Event start')
 
@@ -1304,82 +1304,86 @@
     datapanel.datatable.table.selection_set([str(popup_data['t'])])
     datapanel.delete_selected()
 
 def popup_report(xs:np.ndarray, ys:np.ndarray, data:dict):
     """
     Call this function to plot the results to the popup guide
     """
+    ##Note that all indices in "data" are relative to the start of the recording!
     popup_clear()
     global popup_data
     popup_data = data
+    print(xs)
     if data['failure']:
         popup.msg_label.insert(text=str(data.get('failure'))+'\n')
     else:
         popup.msg_label.insert(text='Success!' + '\n')
+    idx_offset = int(xs[0]*app.interface.recordings[0].sampling_rate) # the position of the left plotted data point in the trace display, within the full recording
+    print(idx_offset)
     try:
-        start, end = popup_plot_recording(xs, ys, data)  # start coordinate and the plot
+        start, end = popup_plot_recording(xs, ys, idx_offset, data)  # start coordinate and the plot, returned indices are corrected for scrolled window
     except Exception as e:
-        # print(e)
+        print(e)
         pass
     try:
         popup.msg_label.insert(f'Peak: {data["peak_coord_x"]:.3f}, {data["peak_coord_y"]:.3f}\n')
         popup_plot_peak(data['peak_coord_x'], data['peak_coord_y'])
         popup_plot_amplitude(data['peak_coord_x'], data['peak_coord_y'], data['baseline'])
     except KeyError:
         pass
     try:
         if data['base_idx_L'] is not None and not data['compound']:
-            popup_plot_base_range(xs, ys, data)
+            popup_plot_base_range(xs, ys, idx_offset, data)
     except:
         pass
 
     try:
         popup.msg_label.insert(f'Baseline: {data["baseline"]:.3f} {data["baseline_unit"]}\n')
         if data['compound']:
             popup.msg_label.insert(f'Baseline extrapolated from preceding mini\n')
         else:
             left_idx = data.get('base_idx_L', None)
             right_idx = data.get('base_idx_R', None)
             if left_idx and right_idx:
                 popup.msg_label.insert(
-                    f'Baseline calculated by averaging: {xs[int(left_idx)]:.3f}-{xs[int(right_idx)]:.3f}\n')
+                    f'Baseline calculated by averaging: {xs[int(left_idx)-idx_offset]:.3f}-{xs[int(right_idx)-idx_offset]:.3f}\n')
             else:
-                popup.msg_label.inesrt(f'Baseline calculated by averaging data points.\n')
+                popup.msg_label.insert(f'Baseline calculated by averaging data points.\n')
     except:
         pass
 
     try:
         popup.msg_label.insert(f"Amplitude: {data['amp']:.3f} {data['amp_unit']}\n")
     except:
         pass
     try:
         popup.msg_label.insert(f"Rise: {data['rise_const']:.3f} {data['rise_unit']}\n")
     except:
         pass
 
     try:
         if not data['compound']:
-            popup_plot_base_simple(xs, end, data)
+            popup_plot_base_simple(xs, idx_offset, end, data)
         else:
-            popup_plot_base_extrapolate(xs, end, data)
+            popup_plot_base_extrapolate(xs, idx_offset, end, data)
     except:
         pass
 
     try:
         popup.msg_label.insert(f'Decay: {data["decay_const"]:.3f} {data["decay_unit"]}\n')
         if data['min_drr'] > 0 or data['max_drr'] is not np.inf:
             popup.msg_label.insert(f'Decay:rise ratio: {data["decay_const"] / data["rise_const"]:.3f}\n')
     except:
         pass
 
     try:
         if not data['compound']:
-            popup_plot_decay_fit(xs, end, data)
+            popup_plot_decay_fit(xs, idx_offset, end, data)
         else:
-            popup_plot_decay_extrapolate(xs, end, data)
+            popup_plot_decay_extrapolate(xs, idx_offset, end, data)
     except:
         pass
 
     try:
         popup_plot_decay_point(data)
     except:
         pass
```

### Comparing `simplyfire-0.4.2/simplyfire/plugins/mini_analysis/mini_analysis.py` & `simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 """
 import numpy as np
 import pandas as pd
 from simplyfire.utils import calculate
 from scipy import optimize
 from datetime import datetime
 
-
 def filter_mini(mini_df: pd.DataFrame = None,
                 xlim=None,
                 min_amp: float = 0.0,
                 max_amp: float = np.inf,
                 min_rise: float = 0.0,
                 max_rise: float = np.inf,
                 min_decay: float = 0.0,
@@ -166,17 +165,17 @@
     show_time = False
     global stop
     stop = False
     if xs is None or ys is None:
         if recording is None:
             return None  # cannot analyze
     if xs is None:
-        xs = recording.get_x_matrix(mode='continuous', channels=[channel], sweeps=sweeps, xlim=xlim).flatten()
+        xs = recording.get_xs(mode='continuous', channel=channel, xlim=xlim)
     if ys is None:
-        ys = recording.get_y_matrix(mode='continuous', channels=[channel], sweeps=sweeps, xlim=xlim).flatten()
+        ys = recording.get_ys(mode='continuous', channel=channel, xlim=xlim)
     else:
         ys = ys.copy()  # make a copy to edit
     try:
         xlim_idx = (
             calculate.search_index(xlim[0], xs, sampling_rate), calculate.search_index(xlim[1], xs, sampling_rate))
     except:
         xlim_idx = (0, len(xs))
@@ -224,26 +223,27 @@
                 direction=direction,
                 reference_df=reference_df,
                 prev_peak=prev_peak,
                 **kwargs
             )
             if mini['success']:
                 mini['xlim_idx_L'] = start_idx
-                mini['xlim_idx_R'] = end_idx
+                mini['xlim_coord_L'] = xs[start_idx]
+                mini['xlim_idx_R'] = min(len(xs)-1,end_idx)
+                mini['xlim_coord_R'] = xs[min(len(xs)-1,end_idx)]
                 hits.append(mini)
                 prev_peak = mini
             else:
                 if mini['failure'] == 'Mini was previously found':
                     # make sure the failure code matches here
                     prev_peak = mini
 
             # print(f'end of analysis, mini was: {mini}')
             # print(f'end of analysis, prev_peak is set to: {prev_peak}')
         start_idx += stride
-        # start_idx += stride
         end_idx = min(start_idx + kernel, xlim_idx[1])
         try:
             # if start_idx > increment:
             #     progress_bar['value'] = progress_bar['value'] + 5
             #     progress_bar.update()
             #     progress_bar.after(5, None)
             #     increment += increment
@@ -375,15 +375,15 @@
 
     if peak_idx < start + FUDGE:  # the local extremum is at the left end of the search window
         return find_peak_recursive(xs, ys, start + FUDGE, end, direction)
     if peak_idx > end - FUDGE:  # the local extremum is at the right end of the search window
         return find_peak_recursive(xs, ys, start, end - FUDGE, direction)
     return peak_idx
 
-
+##@njit
 def find_mini_start(peak_idx: int,
                     ys: np.ndarray,
                     lag: int = 100,
                     delta_x: int = 400,
                     direction: int = 1) -> tuple:
     """
     Calculates estimated baseline value and the index of start of a mini event
@@ -570,27 +570,22 @@
         if prev_mini_direction is None:
             prev_mini_direction = direction
         y_data = ys - prev_mini_baseline
         y_data = y_data - single_exponent_constant((xs * 1000 - prev_mini_t_ms), prev_mini_A, prev_mini_decay,
                                                    prev_mini_decay_baseline) * prev_mini_direction
         y_data = y_data * direction
 
-        # y_data = ys * direction + single_exponent_constant((xs * 1000 - prev_mini_t_ms), prev_mini_A,
-        #                                                    prev_mini_decay,
-        #                                                    prev_mini_decay_baseline) * prev_mini_direction - prev_mini_baseline * direction
     else:
         y_data = (ys - baseline) * direction
-    left_idx = np.where(y_data[:peak_idx] <= (amp * 0.5) * direction)
-    if len(left_idx[0]):
-        left_idx = left_idx[0][-1]
-    else:
+    left_idx = np.argmax(y_data[:peak_idx] >= (amp * 0.5) * direction)
+    if left_idx == -1:
         left_idx = None
-    right_idx = np.where(y_data[peak_idx:] <= (amp * 0.5) * direction)
-    if len(right_idx[0]):
-        right_idx = right_idx[0][0] + peak_idx
+    right_idx = np.argmax(y_data[peak_idx:] <= (amp * 0.5) * direction)
+    if right_idx > -1:
+        right_idx += peak_idx
     else:
         right_idx = None
     return left_idx, right_idx  # pick the shortest length
 
 
 def fit_mini_decay(xs: np.ndarray,
                    ys: np.ndarray,
@@ -624,18 +619,14 @@
     x_data = (xs - xs[0]) * 1000
     # print(x_data)
 
     if prev_mini_t is not None:  # compound mini
         prev_mini_t_ms = prev_mini_t * 1000
         if prev_mini_direction is None:
             prev_mini_direction = direction
-        # y_data = ys * direction + single_exponent_constant((xs * 1000 - prev_mini_t_ms), prev_mini_A, prev_mini_decay,
-        #                                                    prev_mini_decay_baseline) * prev_mini_direction - prev_mini_baseline * direction
-        # y_data = ys - single_exponent_constant((xs*1000 - prev_mini_t_ms), prev_mini_A, prev_mini_decay, prev_mini_decay_baseline) * prev_mini_direction
-        # y_data = (y_data - prev_mini_baseline) * direction
 
         y_data = ys - prev_mini_baseline
         y_data = y_data - single_exponent_constant((xs * 1000 - prev_mini_t_ms), prev_mini_A, prev_mini_decay,
                                                    prev_mini_decay_baseline) * prev_mini_direction
         y_data = y_data * direction
 
     else:
@@ -710,43 +701,37 @@
     # fit
     results = optimize.curve_fit(single_exponent,
                                  x_data,
                                  y_data,
                                  sigma=y_weight,
                                  absolute_sigma=True,
                                  maxfev=15000)
-    # print(results[0])
     a = results[0][0]
     t = results[0][1]
-    # d = results[0][2]
-    # print((a, t, d))
     decay_constant_idx = calculate.search_index(t, x_data, sampling_rate) + start_idx  # offset to start_idx
 
     return a, t, decay_constant_idx
 
 def calculate_mini_10_90_rise(xs:np.ndarray,
                               ys:np.ndarray,
                               baseline:float,
                               amp:float,
                               start_idx:int,
                               peak_idx:int,
                               direction:int=1,
                               sampling_rate:int=None):
-    low_idx = np.where((ys[start_idx:peak_idx]-baseline)*direction>amp*direction*0.1)[0][0] # take first spot
-    high_idx = np.where((ys[start_idx:peak_idx+1]-baseline)*direction>amp*direction*0.9)[0][0] # take first spot #peak_idx inclusive
+    low_idx = np.argmax((ys[start_idx:peak_idx+1]-baseline)*direction > amp*direction*0.1)
+    high_idx = np.argmax((ys[start_idx:peak_idx+1]-baseline)*direction > amp*direction*0.1)
 
     if sampling_rate:
         return (high_idx-low_idx)*1/sampling_rate*1000
     else:
         return (xs[high_idx] - xs[low_idx]) *1000
 
 
-
-
-
 def analyze_candidate_mini(xs,
                            ys,
                            peak_idx=None,
                            peak_t=None,
                            x_sigdig=None,
                            sampling_rate=None,
                            channel=0,
@@ -791,14 +776,15 @@
                            #################################
                            offset=0,
                            y_unit='mV',
                            x_unit='s',
                            ##################################
                            prev_peak_idx=None,
                            prev_peak=None,
+                           manual_radius = 0,
                            **kwargs
                            ):
     """
         peak_idx: int - Index within the xs data corresponding to a peak.
         peak_t: float - if provided, takes precedence over peak_idx
         x_sigdig: significant digits in x
         sampling_rate: sampling rate of xs in Hz
@@ -826,15 +812,14 @@
         reference_df: pd.DataFrame to compare the results against previously found minis
         reanalyze: bool indicating whether the candidate mini is already in mini_df
             Set to True if reanalyzing a previously found mini.
             If set to False, previously found minis will be ignored.
 
     """
     # print(f'start of analysis, prev peak passed is: {prev_peak}')
-
     show_time = False
     # perform conversions
     if sampling_rate == 'auto':
         sampling_rate = 1 / np.mean(xs[1:5] - xs[0:4])
     # convert lag_ms to lag
     if lag_ms is not None:
         lag = int(lag_ms / 1000 * sampling_rate)
@@ -851,29 +836,31 @@
     min_peak2peak = min_peak2peak_ms / 1000 * sampling_rate
     if prev_peak:  # had the prev peak provided as dict
         try:
             prev_peak_idx = prev_peak['peak_idx']
         except:
             print('prev peak is None')
             prev_peak = None
-    elif prev_peak_idx:  # had index provided but not the dict
+    elif prev_peak_idx:  # had index provided but not the dict  
         try:
             prev_peak_candidate = reference_df.loc[(reference_df['peak_idx'] == prev_peak_idx) &
                                                    (reference_df['channel'] == channel)]
             if prev_peak_candidate.shape[0] > 0:
                 prev_peak = prev_peak_candidate.squeeze().to_dict()
+
         except:
             prev_peak = None
     # initiate mini data dict
     mini = {'direction': direction, 'lag': lag, 'delta_x': delta_x, 'channel': channel, 'min_amp': min_amp,
             'max_amp': max_amp,
             'min_rise': min_rise, 'max_rise': max_rise, 'min_hw': min_hw, 'max_hw': max_hw, 'min_decay': min_decay,
             'min_s2n': min_s2n, 'max_s2n': max_s2n, 'min_drr': min_drr, 'max_drr': max_drr,
             'max_decay': max_decay, 'decay_max_points': decay_max_points, 'decay_max_interval': decay_max_interval,
-            'datetime': datetime.now().strftime('%m-%d-%y %H:%M:%S'), 'failure': None, 'success': True,
+            'datetime': datetime.now().strftime('%m-%d-%y %H:%M:%S'), 
+            'failure': None, 'success': True,
             't': xs[peak_idx], 'peak_idx': peak_idx + offset, 'compound': False,
             'baseline_unit': y_unit}
     max_compound_interval_idx = max_compound_interval * sampling_rate / 1000
     if x_unit in ['s', 'sec', 'second', 'seconds']:
         mini['decay_unit'] = mini['rise_unit'] = mini['halfwidth_unit'] = 'ms'
     else:
         mini['decay_unit'] = mini['rise_unit'] = mini['halfwidth_unit'] = x_unit + 'E-3'
@@ -889,15 +876,15 @@
             if mini['t'] in reference_df[
                 (reference_df['channel'] == channel)].t.values:  # check if t exists in the channel
                 mini = reference_df.loc[(reference_df['t'] == mini['t']) &
                                         (reference_df['channel'] == channel)].squeeze().to_dict()
                 mini['success'] = False
                 mini['failure'] = 'Mini was previously found'
                 return mini
-        except Exception as e:  # if df is empty, will throw an error
+        except:  # if df is empty, will throw an error
             pass
 
     # store peak coordinate
     mini['peak_coord_x'] = xs[peak_idx]
     mini['peak_coord_y'] = ys[peak_idx]
 
     baseline_idx, mini['baseline'] = find_mini_start(peak_idx=peak_idx,
@@ -912,20 +899,23 @@
         mini['failure'] = 'Baseline could not be found'
         return mini
     if delta_x is None or delta_x == 0:
         base_idx = (baseline_idx - lag, baseline_idx)
     else:
         base_idx = (int(peak_idx - delta_x - lag / 2), int(peak_idx - delta_x + lag / 2))
     mini['base_idx_L'] = base_idx[0] + offset
+    mini['base_coord_L'] = xs[base_idx[0] + offset]
     mini['base_idx_R'] = base_idx[1] + offset
+    mini['base_coord_R'] = xs[base_idx[1] + offset]
     ####### search baseline #######
     # find baseline/start of event
     mini['start_idx'] = baseline_idx + offset
 
     if reference_df is not None or prev_peak is not None:
+##    if False:  
         # find the peak of the previous mini
         # peak x-value must be stored in the column 't'
         # check that the channels are the same
         try:
             prev_peak_candidate_idx = reference_df.loc[(reference_df['channel'] == channel) & (
                     reference_df['t'] < mini['t'])].peak_idx
             prev_peak_candidate_idx = max(prev_peak_candidate_idx)
@@ -1004,24 +994,26 @@
                         baseline_idx = baseline_idx_min
                     mini['start_idx'] = baseline_idx + offset
                     # extrapolate baseline at peak from previous decay
                     mini['baseline'] = single_exponent((xs[peak_idx] - xs[prev_peak_idx_offset]) * 1000,
                                                        mini['prev_decay_A'],
                                                        mini['prev_decay_const']) * mini['prev_mini_direction'] + mini[
                                            'prev_baseline']  # get the extrapolated baseline value
-
+##    print("Before amplitude check: " + str(mini['success']))
     mini['amp'] = (mini['peak_coord_y'] - mini['baseline'])  # signed
     # store coordinate for start of mini (where the plot meets the baseline)
     mini['start_coord_x'] = xs[baseline_idx]
     mini['start_coord_y'] = ys[baseline_idx]
 
     if min_amp and (mini['amp'] * direction) < min_amp:
         mini['success'] = False
         mini['failure'] = 'Min amp not met'
         return mini
+		
+##    print("After amplitude check: " + str(mini['success']))
 
     if max_amp and mini['amp'] * direction > max_amp:
         mini['success'] = False
         mini['failure'] = 'Max amp exceeded'
         return mini
 
     ####### calculate stdev ########
@@ -1135,18 +1127,18 @@
                 direction=direction,
                 baseline=mini['baseline'],
             )
     elif decay_algorithm == '% amplitude':
         # mimics Mini Analysis
         mini['decay_A'] = mini['amp'] * direction
         mini['decay_baseline'] = 0
-        decay_idx = np.where((ys[int(peak_idx): int(min(peak_idx + decay_max_points, len(ys)))] - mini[
+        decay_idx = np.argmax((ys[int(peak_idx): int(min(peak_idx + decay_max_points, len(ys)))] - mini[
             'baseline']) * direction < decay_p_amp * mini['amp'] * direction / 100)
-        if len(decay_idx[0]) > 0:
-            mini['decay_const'] = decay_idx[0][0] / sampling_rate * 1000
+        if decay_idx > 0:
+            mini['decay_const'] = decay_idx / sampling_rate * 1000
         else:
             mini['failure'] = 'Decay constant could not be calculated'
             mini['success'] = False
             return mini
     elif decay_algorithm == 'None':
         mini['decay_A'] = None
         mini['decay_const'] = None
```

### Comparing `simplyfire-0.4.2/simplyfire/plugins/navigation/navigation.py` & `simplyfire-0.5.1/simplyfire/plugins/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/plugins/process_recording/process_GUI.py` & `simplyfire-0.5.1/simplyfire/plugins/process_recording/process_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 baseline_range_right= 1
 baseline_fixed = 0
 sweep_target = 'All sweeps'
 channel_target = '1'
 baseline_mode = 'Mean of all targets'
 filter_algorithm = 'Lowpass'
 average_show_result = '1'
+filter_undoable = '1'
 width = 11
 pole = 8
 Hz = 1000
 filter_Lowpass_algorithm = 'Boxcar'
 filter_Highpass_algorithm = 'Not yet supported'
 
 #### modify the PluginForm class ####
@@ -271,25 +272,28 @@
         # account for more recordings being open (consider only the main file open)
         if app.inputs['trace_mode'].get() == 'continuous' and 0 in target_sweeps:
             target_sweeps = range(app.interface.recordings[0].sweep_count)
         elif app.inputs['trace_mode'].get() == 'overlay':
             # account for more recordings being open (consider only the main file open)
             target_sweeps = [i for i in target_sweeps if i < app.interface.recordings[0].sweep_count]
 
-    if app.interface.is_accepting_undo():
-        temp_filename = app.interface.get_temp_filename()
-        app.interface.recordings[0].save_y_data(filename=temp_filename,
-                                                channels=target_channels,
-                                                sweeps=target_sweeps)
-        controller.add_undo([
-            lambda f=temp_filename, c=target_channels, s=target_sweeps: app.interface.recordings[0].load_y_data(f,c,s),
-            lambda c=False:app.interface.plot(clear=c, relim=False, fix_x=True, fix_y=True),
-            lambda f=temp_filename:app.interface.delete_temp_file(f),
-            lambda msg='Undo filter': controller.log(msg)
-        ])
+    if(form.inputs['filter_undoable'].get() == '1'):			
+        if app.interface.is_accepting_undo():
+            temp_filename = app.interface.get_temp_filename()
+            app.interface.recordings[0].save_y_data(filename=temp_filename,
+                                                    channels=target_channels,
+                                                    sweeps=target_sweeps)
+            controller.add_undo([
+                lambda f=temp_filename, c=target_channels, s=target_sweeps: app.interface.recordings[0].load_y_data(f,c,s),
+                lambda c=False:app.interface.plot(clear=c, relim=False, fix_x=True, fix_y=True),
+                lambda f=temp_filename:app.interface.delete_temp_file(f),
+                lambda msg='Undo filter': controller.log(msg)
+            ])
+    else:
+        app.interface.clear_undo()
     filter_choice = form.inputs['filter_algorithm'].get()
     filter_algorithm = form.inputs[f'filter_{filter_choice}_algorithm'].get()
     params = {}
     for key in filter_param_set[filter_algorithm]:
         params[key] = form.inputs[key].get()
 
     # deal with undo later
@@ -399,14 +403,23 @@
 )
 form.insert_separator()
 form.insert_title(
     text='Filtering',
     separator=False
 )
 
+form.insert_label_checkbox(
+    name='filter_undoable',
+    text='Allow undo for filtering',
+    onvalue='1',
+    offvalue='',
+    separator=False,
+    default=filter_undoable
+)
+
 form.insert_label_optionmenu(
     name='filter_algorithm',
     text="Select low or high pass:",
     options=filter_choices,
     separator=False,
     command=form.apply_parameters,
     default=filter_algorithm
```

### Comparing `simplyfire-0.4.2/simplyfire/plugins/process_recording/process_recording.py` & `simplyfire-0.5.1/simplyfire/plugins/process_recording/process_recording.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,49 +57,45 @@
     result = recording.get_y_matrix(mode=plot_mode, channels=channels, sweeps=sweeps) + shift
     recording.replace_y_data(mode=plot_mode, channels=channels, sweeps=sweeps, new_data=result)
 
 
 def filter_Boxcar(recording:Recording,
                   params:dict=None,
                   channels:list=None,
-                  sweeps:list=None,
                   ):
     assert type(recording) == Recording, f'data passed must be of type {Recording}'
     width = int(params['width'])
     kernel = np.ones(width)/width
     if not channels:
         channels = range(recording.channel_count)
-    if not sweeps:
-        sweeps = range(recording.sweep_count)
     for c in channels:
-        ys = recording.get_y_matrix(mode='continuous', channels=[c], sweeps=sweeps)
+        ys = recording.get_y_matrix(mode='continuous', channels=[c], sweeps=None)
         filtered = np.convolve(ys.flatten(), kernel, mode='same')
         filtered = np.reshape(filtered, (1,1,len(filtered)))
         filtered[:, :, :int(width/2)] = ys[:,:,:int(width/2)] # prevent 0-ing of the edges
         filtered[:, :, -int(width/2):] = ys[:,:,-int(width/2):] # prevent 0-ing of the edges
-        recording.replace_y_data(mode='continuous', channels=[c], sweeps=sweeps, new_data=filtered)
+        recording.replace_y_data(mode='continuous', channels=[c], sweeps=None, new_data=filtered)
 
     return recording
 
 def filter_Bessel(recording:Recording,
                   params:dict=None,
-                  channels:list=None,
-                  sweeps:list=None):
+                  channels:list=None):
     assert type(recording) == Recording, f'data passed must be of type {Recording}'
     pole = int(params['pole'])
     Hz = int(params['Hz'])
     Wn = 2*np.pi*Hz
     b,a = signal.bessel(pole, Wn, btype='low', analog=True, output='ba')
     for c in channels:
         # https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.lsim.html
-        ys = recording.get_y_matrix(mode='continuous', channels=[c], sweeps=sweeps).flatten()
-        xs = recording.get_x_matrix(mode='continuous', channels=[c], sweeps=sweeps).flatten()
+        ys = recording.get_y_matrix(mode='continuous', channels=[c], sweeps=None).flatten()
+        xs = recording.get_x_matrix(mode='continuous', channels=[c], sweeps=None).flatten()
         tout, filtered, xout = signal.lsim((b,a), U=ys, T=xs)
         filtered = np.reshape(filtered, (1, 1, len(filtered)))
-        recording.replace_y_data(mode='continuous', channels=[c], sweeps=sweeps, new_data=filtered)
+        recording.replace_y_data(mode='continuous', channels=[c], sweeps=None, new_data=filtered)
 
     pass
 
 
 # implement Boxel 8pole 1000Hz!
 
 def average_sweeps(recording:Recording,
```

### Comparing `simplyfire-0.4.2/simplyfire/plugins/style/style_tab.py` & `simplyfire-0.5.1/simplyfire/plugins/style/style_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/plugins/sweeps/sweeps_GUI.py` & `simplyfire-0.5.1/simplyfire/plugins/sweeps/sweeps_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/setting/config.py` & `simplyfire-0.5.1/simplyfire/setting/config.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/setting/default_config.yaml` & `simplyfire-0.5.1/simplyfire/setting/default_config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -153,13 +153,15 @@
 
   key_find_all:
     - '<F4>'
 
   key_find_in_window:
     - '<F5>'
 
-  key_zoom_axis:
-    - '<Control_L>'
-    - '<Control_R>'
+  key_set_zoom_axis_x:
+    - '<Key-x>'
+
+  key_set_zoom_axis_y:
+    - '<Key-y>'
 
   key_show_all:
     - '<Key-Home>'
```

### Comparing `simplyfire-0.4.2/simplyfire/utils/abfWriter.py` & `simplyfire-0.5.1/simplyfire/utils/abfWriter.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/calculate.py` & `simplyfire-0.5.1/simplyfire/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/custom_widgets.py` & `simplyfire-0.5.1/simplyfire/utils/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/formatting.py` & `simplyfire-0.5.1/simplyfire/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/plugin_GUI.py` & `simplyfire-0.5.1/simplyfire/utils/plugin_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/plugin_controller.py` & `simplyfire-0.5.1/simplyfire/utils/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/plugin_form.py` & `simplyfire-0.5.1/simplyfire/utils/plugin_form.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/plugin_popup.py` & `simplyfire-0.5.1/simplyfire/utils/plugin_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/plugin_table.py` & `simplyfire-0.5.1/simplyfire/utils/plugin_table.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/recording.py` & `simplyfire-0.5.1/simplyfire/utils/recording.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 """
 import numpy as np
 import os
 from pyabf import abf
 from simplyfire.utils import abfWriter
 from simplyfire.setting import config
 from math import ceil
+from psutil import Process
 
 class Recording():
     def __init__(self, filepath):
         self.filepath = filepath
         # initialize metadata
         self.channel = 0
         self.added_sweep_count = 0
@@ -69,18 +70,16 @@
         self.x_label = data.sweepLabelX  # in the form of Label (Units)
 
         # y_value metadata
         self.sweep_count = data.sweepCount
         self.original_sweep_count = self.sweep_count
         self.sweep_points = data.sweepPointCount
 
-        # extract y and x values and store as 3D numpy array (channel, sweep, datapoint)
+        # extract y values and store as 3D numpy array (channel, sweep, datapoint)
         self.y_data = np.reshape(data.data, (self.channel_count, self.sweep_count, self.sweep_points))
-        self.x_data = np.repeat(np.reshape(data.sweepX, (1, 1, self.sweep_points)), self.sweep_count, axis=1)
-        self.x_data = np.repeat(self.x_data, self.channel_count, axis=0)
 
     def read_csv(self, filename):
         """
         only supports single channel data
         """
         self.channel_count = 1
         self.sweep_count = 0
@@ -124,18 +123,14 @@
                         ys = [float(i) for i in l.split(',')]
                         if self.sweep_points == 0:
                             self.sweep_points = len(ys)
                         self.y_data = np.reshape(np.array(ys),
                                                  (1, 1, self.sweep_points))
             if self.sweep_count == 0:
                 self.sweep_count = self.y_data.shape[1]
-            sweepX = np.arange(self.sweep_points)/self.sampling_rate
-            self.x_data = np.repeat(np.reshape(np.array(sweepX), (1, 1, self.sweep_points)),
-                                    self.sweep_count,
-                                    axis=1)
 
     def save(self, filename, channels=None, suffix=0, handle_error=False):
         if channels is None:
             channels = [i for i in range(self.channel_count)]
         if suffix > 0:
             fname = f'{filename.split(".")[0]}({suffix}).{filename.split(".")[1]}'
         else:
@@ -221,91 +216,107 @@
                 result[c, sweeps, :] = new_data[i]
             return result
 
 
     def get_y_matrix(self, mode='continuous', sweeps=None, channels=None, xlim=None):
         """
         returns a slice of the y_data
-        mode: string
-            'continuous', 'overlay'
+        mode: 'continuous' or 'overlay'
         channels: list of int - if None, defaults to all channels
         sweeps: list of int - If None, defaults to all sweeps
         xlim: float tuple [left, right] - If None, defaults to all data points in each sweep
         """
         if channels == None:
             channels = range(self.channel_count)
         elif type(channels) == int:
             channels = [channels]
         if sweeps == None:
             sweeps = [i for i in range(self.sweep_count)]
         elif type(sweeps) == int:
             sweeps = [sweeps]
+        print(channels)
+        print(sweeps)
+        print(self.y_data.shape)
+                           
         if mode == 'continuous':
             if xlim:
                 return np.reshape(self.y_data[channels][:, sweeps, :],
                                   (len(channels), 1, len(sweeps) * self.sweep_points))[
                        :, :, max(0, int(xlim[0] / self.x_interval)):min(self.sweep_count * self.sweep_points,
                                                                         ceil(xlim[1] / self.x_interval) + 1)]
             else:
                 return np.reshape(self.y_data[channels][:, sweeps, :],
-                                  (len(channels), 1, len(sweeps) * self.sweep_points))[
-                       :, :, :]
+                                  (len(channels), 1, len(sweeps) * self.sweep_points))
         if mode == 'overlay':
             if xlim:
-                return self.y_data[channels][:, sweeps,
+                print('xlim overlay')
+                return self.y_data[channels][:, sweeps, :][:,:,
                        max(0, int(xlim[0] / self.x_interval)):min(self.sweep_count * self.sweep_points,
                                                                   ceil(xlim[1] / self.x_interval) + 1)]
-            return self.y_data[channels][:, sweeps]
+            else:
+                print('no xlim overlay')
+                return_val = self.y_data[channels][:, sweeps, :]
+                print(return_val.shape)
+                return self.y_data[channels][:, sweeps, :]
 
     def get_x_matrix(self, mode='continuous', sweeps=None, channels=None, xlim=None):
         """
         returns a slice of the x_data
-        mode: string
-            'continuous', 'overlay'
         channels: list of int - if None, defaults to all channels
         sweeps: list of int - only used for the 'overlay' plot_mode. If None, defaults to all sweeps
         xlim: float tuple [left, right] - If None, defaults to all data points in each sweep
         """
-        if sweeps is None:
-            sweeps = range(self.sweep_count)
+
         if channels == None:
             channels = range(self.channel_count)
+            
         if mode == 'continuous':
-            mult = np.arange(0, len(sweeps))
-            mult = np.reshape(mult, (1, len(sweeps), 1))
-            offset = mult * (self.sweep_points * self.x_interval)
-            x_matrix = np.reshape(self.x_data[channels][:, sweeps] + offset,
-                                  (len(channels), 1, len(sweeps) * self.sweep_points))
             if xlim:
                 start_idx = max(0, int(xlim[0] / self.x_interval))
                 end_idx = min(self.sweep_count * self.sweep_points, ceil(xlim[1] / self.x_interval) + 1)
-                return x_matrix[:, :, start_idx:end_idx]
-            return x_matrix
-        if mode == 'overlay':
+                return np.linspace(self.x_interval*start_idx,self.x_interval*end_idx,end_idx-start_idx+1)
+            elif sweeps is None:
+                return np.linspace(0,(self.sweep_count*self.sweep_points-1)*self.x_interval,self.sweep_count*self.sweep_points)
+            else:
+                mult = np.reshape(sweeps, (1, len(sweeps), 1))
+                offset = mult * (self.sweep_points * self.x_interval)
+                one_row = np.linspace(0,(self.sweep_points-1)*self.x_interval,self.sweep_points)
+                return np.repeat(one_row,len(sweeps)*len(channels)) + offset
+        elif mode == 'overlay':
             if xlim:
                 start_idx = max(0, int(xlim[0] / self.x_interval))
                 end_idx = min(self.sweep_count * self.sweep_points, ceil(xlim[1] / self.x_interval) + 1)
-                return self.x_data[channels][:, sweeps][:, :, start_idx, end_idx]
-            return self.x_data[channels][:, sweeps]
+                one_row = np.linspace(self.x_interval*start_idx,self.x_interval*end_idx,end_idx-start_idx+1)
+            else:
+                one_row = np.linspace(0,(self.sweep_points-1)*self.x_interval,self.sweep_points)
+            return np.broadcast_to(one_row,(len(sweeps)*len(channels),)+one_row.shape)
 
     def get_xs(self, mode='continuous', sweep=None, channel=None, xlim=None):
         """
         returns a 1D numpy array representing the x-values in the recording.
         Use this function to get x-values for plotting
         mode: string
             continuous, concatenate, or None
         sweep: int
         channel: int if None, defaults to current channel
         xlim: float tuple - [left, right] If None, defaults to all x-values
         """
-        if not channel:
-            channel = self.channel
-        if mode == 'continuous':
-            return self.get_x_matrix(mode='continuous', channels=[channel], xlim=xlim).flatten()
-        return self.get_x_matrix(mode='overlay', sweeps=[sweep], channels=[channel], xlim=xlim).flatten()
+        if mode == 'continuous':                             
+            if xlim:
+                start_idx = max(0, int(xlim[0] / self.x_interval))
+                end_idx = min(self.sweep_count * self.sweep_points -1, ceil(xlim[1] / self.x_interval))
+                return np.linspace(self.x_interval*start_idx,self.x_interval*end_idx,end_idx-start_idx+1)
+            return np.linspace(0,(self.sweep_count*self.sweep_points-1)*self.x_interval,self.sweep_count*self.sweep_points)
+        if mode == 'overlay':
+            if xlim:
+                start_idx = max(0, int(xlim[0] / self.x_interval))
+                end_idx = min(self.sweep_points-1, ceil(xlim[1] / self.x_interval))
+                return np.linspace(self.x_interval*start_idx,self.x_interval*end_idx,end_idx-start_idx+1)
+            return np.linspace(0,(self.sweep_points-1)*self.x_interval,self.sweep_points)
+            return return_val
 
     def get_ys(self, mode='continuous', sweep=None, channel=None, xlim=None):
         """
         returns a 1D numpy array representing the y-values of the recording.
         Use this functions to get y-values for plotting
         mode: string
             'continuous', 'overlay', or None
@@ -314,16 +325,30 @@
         channel: int
             if empty, the current channel in the object is used
         xlim: float tuple - [left, right] If None, defaults to all x-values
         """
         if channel == None:
             channel = self.channel
         if mode == 'continuous':
-            return self.get_y_matrix(mode='continuous', channels=[channel], xlim=xlim).flatten()
-        return self.get_y_matrix(mode=mode, channels=[channel], sweeps=[sweep], xlim=xlim).flatten()
+            if xlim:
+                ##print('xlim continuous')
+                return self.y_data[channel,:,:].ravel()[
+                       max(0, int(xlim[0] / self.x_interval)):min(self.sweep_count * self.sweep_points,
+                                                                        ceil(xlim[1] / self.x_interval) + 1)]
+            else:
+                ##print('no xlim continuous')			
+                return self.y_data[channel,:,:].ravel()	
+        if mode == 'overlay':
+            if xlim:
+                ##print('xlim overlay')
+                return self.y_data[channel, sweep,
+                       max(0, int(xlim[0] / self.x_interval)):min(self.sweep_points,
+                                                                  ceil(xlim[1] / self.x_interval) + 1)]
+            ##print('no xlim overlay')
+            return self.y_data[channel, sweep]
 
     def save_y_data(self, filename, channels=None, sweeps=None):
         """
         saves y_data of specified channels and sweeps in a temporary file
 
         filename: str name of the file
         channels: list of int, defaults to all channels if None
@@ -369,18 +394,16 @@
             temp_data = np.full((self.channel_count, 1, self.sweep_points), dtype=np.float, fill_value=fill)
             assert new_data.shape[
                        -1] == self.sweep_points, 'dimension mismatch - the sweep length does not match the existing data'
             new_data_reshape = np.reshape(new_data, (len(channels), 1, self.sweep_points))
             temp_data[channels] = new_data_reshape
             self.y_data = np.append(self.y_data, temp_data, axis=1)
 
-        self.x_data = np.append(self.x_data, self.x_data[:, -new_data.shape[1]:, :], axis=1)
         self.sweep_count += 1
         self.added_sweep_count += 1
 
     def delete_last_sweep(self):
         if self.sweep_count == self.original_sweep_count:
             return None  # cannot delete original data
         self.y_data = self.y_data[:, :-1, :]
-        self.x_data = self.x_data[:, :-1, :]
         self.sweep_count -= 1
         self.added_sweep_count -= 1
```

### Comparing `simplyfire-0.4.2/simplyfire/utils/scrollable_option_frame.py` & `simplyfire-0.5.1/simplyfire/utils/scrollable_option_frame.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/threader.py` & `simplyfire-0.5.1/simplyfire/utils/threader.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire/utils/validation.py` & `simplyfire-0.5.1/simplyfire/utils/validation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.4.2/simplyfire.egg-info/PKG-INFO` & `simplyfire-0.5.1/simplyfire.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.4.2
+Version: 0.5.1
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
-Author: Megumi Mori
+Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimplyFire
 A customizable analysis package for electrophysiologists
 
-Read the full manual [here](https://simplyfire-beta.readthedocs.io/).
+Read the full manual [here](https://simplyfire.readthedocs.io/).
 
 ## .exe Installation
 
-Download the software zip file from the recent [release](https://github.com/megumi-mori/SimplyFire-beta/releases).
+Download the software zip file from the recent [release](https://github.com/HaghighiLabBuck/SimplyFire/releases).
 You only need to download the zip file.
 
 Extract the contents of the zip file, and locate SimplyFire.exe to run the software.
 
 ## Python Installation
 If you have Python, you can install and run SimplyFire as a Python module. 
 
@@ -54,8 +53,7 @@
 Tools are provided to easily create custom plugins. 
 
 Pull-requests for fixes and additions are welcome! 
 Details on the development workflow will be available in the future. 
 
 ## License
 SimplyFire is released under the GPLv3 or later license. 
-
```

### Comparing `simplyfire-0.4.2/simplyfire.egg-info/SOURCES.txt` & `simplyfire-0.5.1/simplyfire.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 simplyfire.egg-info/PKG-INFO
 simplyfire.egg-info/SOURCES.txt
 simplyfire.egg-info/dependency_links.txt
 simplyfire.egg-info/entry_points.txt
 simplyfire.egg-info/not-zip-safe
 simplyfire.egg-info/requires.txt
 simplyfire.egg-info/top_level.txt
-simplyfire/__pycache__/__init__.cpython-310.pyc
-simplyfire/__pycache__/app.cpython-310.pyc
 simplyfire/backend/__init__.py
 simplyfire/backend/interface.py
 simplyfire/backend/interpreter.py
 simplyfire/backend/plugin_manager.py
 simplyfire/img/arrow.png
 simplyfire/img/loading.gif
 simplyfire/img/logo.ico
@@ -55,16 +53,14 @@
 simplyfire/plugins/style/plugin.yaml
 simplyfire/plugins/style/style_tab.py
 simplyfire/plugins/sweeps/plugin.yaml
 simplyfire/plugins/sweeps/sweeps_GUI.py
 simplyfire/setting/__init__.py
 simplyfire/setting/config.py
 simplyfire/setting/default_config.yaml
-simplyfire/setting/__pycache__/__init__.cpython-310.pyc
-simplyfire/setting/__pycache__/config.cpython-310.pyc
 simplyfire/temp/README.md
 simplyfire/temp/__init__.py
 simplyfire/utils/__init__.py
 simplyfire/utils/abfWriter.py
 simplyfire/utils/calculate.py
 simplyfire/utils/custom_widgets.py
 simplyfire/utils/formatting.py
@@ -72,11 +68,8 @@
 simplyfire/utils/plugin_controller.py
 simplyfire/utils/plugin_form.py
 simplyfire/utils/plugin_popup.py
 simplyfire/utils/plugin_table.py
 simplyfire/utils/recording.py
 simplyfire/utils/scrollable_option_frame.py
 simplyfire/utils/threader.py
-simplyfire/utils/validation.py
-simplyfire/utils/__pycache__/__init__.cpython-310.pyc
-simplyfire/utils/__pycache__/custom_widgets.cpython-310.pyc
-simplyfire/utils/__pycache__/validation.cpython-310.pyc
+simplyfire/utils/validation.py
```

