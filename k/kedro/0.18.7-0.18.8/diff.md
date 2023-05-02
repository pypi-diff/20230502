# Comparing `tmp/kedro-0.18.7.tar.gz` & `tmp/kedro-0.18.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kedro-0.18.7.tar", last modified: Wed Mar 22 16:11:21 2023, max compression
+gzip compressed data, was "/home/circleci/project/dist/.tmp-eup6eyn_/kedro-0.18.8.tar", last modified: Tue May  2 12:17:02 2023, max compression
```

## Comparing `kedro-0.18.7.tar` & `kedro-0.18.8.tar`

### file list

```diff
@@ -1,252 +1,250 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-03-22 16:07:43.000000 kedro-0.18.7/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-03-22 16:07:43.000000 kedro-0.18.7/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12921 2023-03-22 16:11:21.000000 kedro-0.18.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10639 2023-03-22 16:07:43.000000 kedro-0.18.7/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/dependency/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-03-22 16:07:43.000000 kedro-0.18.7/dependency/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      274 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/abstract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8975 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5309 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13557 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/omegaconf_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10667 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/config/templated_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/api/api_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/biosequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/biosequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5543 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/dask/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/dask/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8298 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/email/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/email/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8066 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/email/message_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/geopandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/geopandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6467 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/holoviews/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/holoviews/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5210 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/json/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/json/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6157 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/json/json_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/matplotlib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/matplotlib/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8926 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/networkx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/networkx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/networkx/gml_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5929 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/networkx/graphml_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5967 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/networkx/json_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/pandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7270 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/csv_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10403 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/excel_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7287 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/feather_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11787 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/gbq_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/generic_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7953 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/hdf_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7139 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8950 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/parquet_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18006 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/sql_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6622 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/pickle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pickle/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10690 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/pillow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pillow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5635 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/pillow/image_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/plotly/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/plotly/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6713 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/plotly/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6101 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/redis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      215 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/redis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/redis/redis_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/spark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/spark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3945 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/spark/deltatable_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15687 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/spark/spark_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9174 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7063 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/spark/spark_jdbc_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/svmlight/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/svmlight/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/tensorflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/tensorflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7536 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/text/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/text/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5314 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/text/text_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/tracking/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      359 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/tracking/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/tracking/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2593 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12182 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/video/video_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/datasets/yaml/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/yaml/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6062 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/extensions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/extensions/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      806 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/extensions/ipython.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/extras/logging/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/logging/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2508 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/extras/logging/color_logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5713 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/catalog.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7309 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/cli.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/cli/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/hooks/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/hooks/markers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/hooks/specs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10525 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/jupyter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30240 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/micropkg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11144 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15085 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1630 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20841 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/starters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16744 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/cli/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/context/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/context/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12703 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/context/context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3706 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/hooks/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/hooks/markers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/hooks/specs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/project/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15249 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/project/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/project/default_logging.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/framework/session/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/session/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16256 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/session/session.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1379 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/session/shelvestore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/session/store.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6546 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/framework/startup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4151 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/cached_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27254 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21693 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/data_catalog.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/lambda_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4140 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/memory_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23213 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/io/partitioned_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/ipython/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5615 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/ipython/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1735 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/ipython/logo-32x32.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/ipython/logo-64x64.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/ipython/logo-svg.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/pipeline/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11659 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/pipeline/modular_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23319 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/pipeline/node.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34035 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/pipeline/pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/runner/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/runner/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14084 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/runner/parallel_runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16528 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/runner/runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/runner/sequential_runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5974 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/runner/thread_runner.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/cookiecutter.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/{{ cookiecutter.pipeline_name }}.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/cookiecutter.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/prompts.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3965 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      901 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6849 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      459 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/logs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/logs/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      423 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      925 2023-03-22 16:07:43.000000 kedro-0.18.7/kedro/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12921 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8073 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-22 16:11:17.000000 kedro-0.18.7/kedro.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4140 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-22 16:11:21.000000 kedro-0.18.7/kedro.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2878 2023-03-22 16:07:43.000000 kedro-0.18.7/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-03-22 16:11:21.000000 kedro-0.18.7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6701 2023-03-22 16:07:43.000000 kedro-0.18.7/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1978 2023-03-22 16:07:43.000000 kedro-0.18.7/test_requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-22 16:11:21.000000 kedro-0.18.7/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2023-03-22 16:07:43.000000 kedro-0.18.7/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-02 12:12:54.000000 kedro-0.18.8/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-05-02 12:12:54.000000 kedro-0.18.8/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-02 12:17:02.000000 kedro-0.18.8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10671 2023-05-02 12:12:54.000000 kedro-0.18.8/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/dependency/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-05-02 12:12:54.000000 kedro-0.18.8/dependency/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      274 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/abstract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5332 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13573 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/omegaconf_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10683 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/templated_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/api/api_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5543 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/dask/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/dask/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8298 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/email/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/email/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8066 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/email/message_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6467 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5210 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/json/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/json/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6157 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/json/json_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8926 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/networkx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/gml_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5929 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5967 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/json_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7270 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/csv_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10403 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/excel_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7287 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/feather_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11787 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/generic_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7953 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7139 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18006 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/sql_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6622 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pickle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pickle/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10690 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pillow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pillow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5635 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pillow/image_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/plotly/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6713 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6101 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/redis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      215 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/redis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/redis/redis_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3945 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15687 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9174 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7063 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_jdbc_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7536 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/text/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/text/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/text/text_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/tracking/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      359 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2593 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12182 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/video/video_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/yaml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/yaml/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6062 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/extensions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      806 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/extensions/ipython.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/logging/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/logging/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2508 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/logging/color_logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5713 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/catalog.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7309 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/cli/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/markers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/specs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10525 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/jupyter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/micropkg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11144 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15085 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1630 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20841 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/starters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16744 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/context/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12666 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/context/context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3706 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/markers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/specs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/project/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15378 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/project/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/project/default_logging.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/session/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16362 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/session.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/shelvestore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/store.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6546 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/startup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4151 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/cached_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27408 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21689 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/data_catalog.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/lambda_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4140 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/memory_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23205 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/partitioned_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/ipython/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5615 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1735 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-32x32.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-64x64.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-svg.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11661 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/modular_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23303 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/node.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33957 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/runner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14068 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/parallel_runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16528 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/sequential_runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/thread_runner.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/cookiecutter.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/{{ cookiecutter.pipeline_name }}.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/cookiecutter.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/prompts.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3965 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6849 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      459 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      423 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      925 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8006 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 12:16:50.000000 kedro-0.18.8/kedro.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4738 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4050 2023-05-02 12:12:54.000000 kedro-0.18.8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-02 12:17:02.000000 kedro-0.18.8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5772 2023-05-02 12:12:54.000000 kedro-0.18.8/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1978 2023-05-02 12:12:54.000000 kedro-0.18.8/test_requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2023-05-02 12:12:54.000000 kedro-0.18.8/tests/test_utils.py
```

### Comparing `kedro-0.18.7/LICENSE.md` & `kedro-0.18.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/PKG-INFO` & `kedro-0.18.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.18.7
+Version: 0.18.8
 Summary: Kedro helps you build production-ready data and analytics pipelines
-Home-page: https://github.com/kedro-org/kedro
 Author: Kedro
 License: Apache Software License (Apache 2.0)
+Project-URL: Homepage, https://kedro.org
+Project-URL: Source, https://github.com/kedro-org/kedro
+Project-URL: Documentation, https://docs.kedro.org
+Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
 Provides-Extra: docs
 Provides-Extra: geopandas
 Provides-Extra: matplotlib
@@ -135,15 +138,15 @@
  - To enhance **team collaboration** when different team members have varied exposure to software engineering concepts
  - To increase efficiency, because applied concepts like modularity and separation of concerns inspire the creation of
   **reusable analytics code**
 
 
 ## The humans behind Kedro
 
-The [Kedro product team](https://docs.kedro.org/en/stable/faq/faq.html#who-maintains-kedro) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
+The [Kedro product team](https://docs.kedro.org/en/stable/contribution/technical_steering_committee.html#kedro-maintainers) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
 
 
 ## Can I contribute?
 
 Yes! Want to help build Kedro? Check out our [guide to contributing to Kedro](https://github.com/kedro-org/kedro/blob/main/CONTRIBUTING.md).
```

### Comparing `kedro-0.18.7/README.md` & `kedro-0.18.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
  - To enhance **team collaboration** when different team members have varied exposure to software engineering concepts
  - To increase efficiency, because applied concepts like modularity and separation of concerns inspire the creation of
   **reusable analytics code**
 
 
 ## The humans behind Kedro
 
-The [Kedro product team](https://docs.kedro.org/en/stable/faq/faq.html#who-maintains-kedro) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
+The [Kedro product team](https://docs.kedro.org/en/stable/contribution/technical_steering_committee.html#kedro-maintainers) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
 
 
 ## Can I contribute?
 
 Yes! Want to help build Kedro? Check out our [guide to contributing to Kedro](https://github.com/kedro-org/kedro/blob/main/CONTRIBUTING.md).
```

### Comparing `kedro-0.18.7/dependency/requirements.txt` & `kedro-0.18.8/dependency/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 anyconfig~=0.10.0
 attrs>=21.3
 cachetools~=5.3
 click<9.0
 cookiecutter>=2.1.1, <3.0
 dynaconf>=3.1.2, <4.0
-fsspec>=2021.4, <=2023.1.0; python_version == '3.7'
-fsspec>=2023.1, <2023.4; python_version >= '3.8'
+fsspec>=2021.4, <2024.1  # Upper bound set arbitrarily, to be reassessed in early 2024
 gitpython~=3.0
 importlib-metadata>=3.6; python_version >= '3.8'
 importlib_metadata>=3.6, <5.0; python_version < '3.8'  # The "selectable" entry points were introduced in `importlib_metadata` 3.6 and Python 3.10. Bandit on Python 3.7 relies on a library with `importlib_metadata` < 5.0
 importlib_resources>=1.3  # The `files()` API was introduced in `importlib_resources` 1.3 and Python 3.9.
 jmespath>=0.9.5, <1.0
-more_itertools~=9.1
+more_itertools~=9.0
 omegaconf~=2.3
-pip-tools~=6.12
+pip-tools~=6.5
 pluggy~=1.0.0
 PyYAML>=4.2, <7.0
-rich~=13.3
-rope~=1.7.0  # subject to LGPLv3 license
+rich>=12.0, <14.0
+rope>=0.21, <2.0  # subject to LGPLv3 license
 setuptools>=65.5.1
 toml~=0.10
-toposort~=1.10  # Needs to be at least 1.5 to be able to raise CircularDependencyError
+toposort~=1.5  # Needs to be at least 1.5 to be able to raise CircularDependencyError
```

### Comparing `kedro-0.18.7/kedro/config/__init__.py` & `kedro-0.18.8/kedro/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/config/abstract_config.py` & `kedro-0.18.8/kedro/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/config/common.py` & `kedro-0.18.8/kedro/config/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from glob import iglob
 from pathlib import Path
 from typing import AbstractSet, Any, Dict, Iterable, List, Set
 from warnings import warn
 
 from yaml.parser import ParserError
 
-from kedro.config import BadConfigException, MissingConfigException
+from kedro.config.abstract_config import BadConfigException, MissingConfigException
 
 SUPPORTED_EXTENSIONS = [
     ".yml",
     ".yaml",
     ".json",
     ".ini",
     ".pickle",
@@ -60,16 +60,16 @@
 
     if not patterns:
         raise ValueError(
             "'patterns' must contain at least one glob "
             "pattern to match config filenames against."
         )
 
-    config = {}  # type: Dict[str, Any]
-    processed_files = set()  # type: Set[Path]
+    config: Dict[str, Any] = {}
+    processed_files: Set[Path] = set()
 
     for conf_path in conf_paths:
         if not Path(conf_path).is_dir():
             raise ValueError(
                 f"Given configuration path either does not exist "
                 f"or is not a valid directory: {conf_path}"
             )
@@ -169,15 +169,15 @@
 
     Returns:
         Resulting configuration dictionary.
 
     """
 
     aggregate_config = {}
-    seen_file_to_keys = {}  # type: Dict[Path, AbstractSet[str]]
+    seen_file_to_keys: Dict[Path, AbstractSet[str]] = {}
 
     for config_filepath in config_filepaths:
         single_config = _load_config_file(
             config_filepath, ac_template=ac_template, ac_context=ac_context
         )
         _check_duplicate_keys(seen_file_to_keys, config_filepath, single_config)
         seen_file_to_keys[config_filepath] = single_config.keys()
@@ -203,15 +203,15 @@
         config_files -= seen_files
 
     return sorted(config_files)
 
 
 def _remove_duplicates(items: Iterable[str]):
     """Remove duplicates while preserving the order."""
-    unique_items = []  # type: List[str]
+    unique_items: List[str] = []
     for item in items:
         if item not in unique_items:
             unique_items.append(item)
         else:
             warn(
                 f"Duplicate environment detected! "
                 f"Skipping re-loading from configuration path: {item}"
```

### Comparing `kedro-0.18.7/kedro/config/config.py` & `kedro-0.18.8/kedro/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module provides ``kedro.config`` with the functionality to load one
 or more configuration files from specified paths.
 """
 from pathlib import Path
 from typing import Any, Dict, Iterable, List
 
-from kedro.config import AbstractConfigLoader
+from kedro.config.abstract_config import AbstractConfigLoader
 from kedro.config.common import _get_config_from_patterns, _remove_duplicates
 
 
 class ConfigLoader(AbstractConfigLoader):
     """Recursively scan directories (config paths) contained in ``conf_source`` for
     configuration files with a ``yaml``, ``yml``, ``json``, ``ini``,
     ``pickle``, ``xml`` or ``properties`` extension, load them,
@@ -82,15 +82,15 @@
             runtime_params: Extra parameters passed to a Kedro run.
             config_patterns: Regex patterns that specify the naming convention for configuration
                 files so they can be loaded. Can be customised by supplying config_patterns as
                 in `CONFIG_LOADER_ARGS` in `settings.py`.
             base_env: Name of the base environment. Defaults to `"base"`.
                 This is used in the `conf_paths` property method to construct
                 the configuration paths.
-            default_run_env: Name of the base environment. Defaults to `"local"`.
+            default_run_env: Name of the default run environment. Defaults to `"local"`.
                 This is used in the `conf_paths` property method to construct
                 the configuration paths. Can be overriden by supplying the `env` argument.
         """
         self.base_env = base_env
         self.default_run_env = default_run_env
 
         self.config_patterns = {
```

### Comparing `kedro-0.18.7/kedro/config/omegaconf_config.py` & `kedro-0.18.8/kedro/config/omegaconf_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import fsspec
 from omegaconf import OmegaConf
 from omegaconf.resolvers import oc
 from yaml.parser import ParserError
 from yaml.scanner import ScannerError
 
-from kedro.config import AbstractConfigLoader, MissingConfigException
+from kedro.config.abstract_config import AbstractConfigLoader, MissingConfigException
 
 _config_logger = logging.getLogger(__name__)
 
 
 class OmegaConfigLoader(AbstractConfigLoader):
     """Recursively scan directories (config paths) contained in ``conf_source`` for
     configuration files with a ``yaml``, ``yml`` or ``json`` extension, load and merge
```

### Comparing `kedro-0.18.7/kedro/config/templated_config.py` & `kedro-0.18.8/kedro/config/templated_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional
 
 import jmespath
 
-from kedro.config import AbstractConfigLoader
+from kedro.config.abstract_config import AbstractConfigLoader
 from kedro.config.common import _get_config_from_patterns, _remove_duplicates
 
 IDENTIFIER_PATTERN = re.compile(
     r"""\$\{
     (?P<path>[A-Za-z0-9_\.]+)  # identifier
     (?:\|(?P<default>[^}]*))?  # optional default value
     \}""",
```

### Comparing `kedro-0.18.7/kedro/extras/datasets/api/api_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/api/api_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/biosequence/biosequence_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/biosequence/biosequence_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/dask/parquet_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/email/message_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/email/message_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/geopandas/geojson_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/holoviews/holoviews_writer.py` & `kedro-0.18.8/kedro/extras/datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/json/json_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/matplotlib/matplotlib_writer.py` & `kedro-0.18.8/kedro/extras/datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/networkx/gml_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/networkx/graphml_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/networkx/json_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/__init__.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/csv_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/excel_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/feather_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/gbq_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/gbq_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/generic_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/hdf_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/hdf_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/json_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/parquet_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/sql_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pandas/xml_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pickle/pickle_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pickle/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/pillow/image_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/plotly/json_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/plotly/plotly_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/redis/redis_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/redis/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/spark/deltatable_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/spark/spark_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/spark/spark_hive_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/spark/spark_jdbc_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/svmlight/svmlight_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/text/text_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/tracking/json_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/tracking/metrics_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/video/video_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/datasets/yaml/yaml_dataset.py` & `kedro-0.18.8/kedro/extras/datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/extensions/ipython.py` & `kedro-0.18.8/kedro/extras/extensions/ipython.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/extras/logging/color_logger.py` & `kedro-0.18.8/kedro/extras/logging/color_logger.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/catalog.py` & `kedro-0.18.8/kedro/framework/cli/catalog.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/cli.py` & `kedro-0.18.8/kedro/framework/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/hooks/manager.py` & `kedro-0.18.8/kedro/framework/cli/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/hooks/specs.py` & `kedro-0.18.8/kedro/framework/cli/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/jupyter.py` & `kedro-0.18.8/kedro/framework/cli/jupyter.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/micropkg.py` & `kedro-0.18.8/kedro/framework/cli/micropkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,15 +476,15 @@
     if refactored_package_source.is_dir():
         _sync_dirs(refactored_package_source, package_dest)
 
 
 def _find_config_files(
     source_config_dir: Path, glob_patterns: List[str]
 ) -> List[Tuple[Path, str]]:
-    config_files = []  # type: List[Tuple[Path, str]]
+    config_files: List[Tuple[Path, str]] = []
 
     if source_config_dir.is_dir():
         config_files = [
             (path, path.parent.relative_to(source_config_dir).as_posix())
             for glob_pattern in glob_patterns
             for path in source_config_dir.glob(glob_pattern)
             if path.is_file()
```

### Comparing `kedro-0.18.7/kedro/framework/cli/pipeline.py` & `kedro-0.18.8/kedro/framework/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/project.py` & `kedro-0.18.8/kedro/framework/cli/project.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/registry.py` & `kedro-0.18.8/kedro/framework/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/starters.py` & `kedro-0.18.8/kedro/framework/cli/starters.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/cli/utils.py` & `kedro-0.18.8/kedro/framework/cli/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/context/context.py` & `kedro-0.18.8/kedro/framework/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 def _is_relative_path(path_string: str) -> bool:
     """Checks whether a path string is a relative path.
 
     Example:
     ::
         >>> _is_relative_path("data/01_raw") == True
-        >>> _is_relative_path("logs/info.log") == True
+        >>> _is_relative_path("info.log") == True
         >>> _is_relative_path("/tmp/data/01_raw") == False
-        >>> _is_relative_path(r"C:\\logs\\info.log") == False
-        >>> _is_relative_path(r"\\logs\\'info.log") == False
-        >>> _is_relative_path("c:/logs/info.log") == False
-        >>> _is_relative_path("s3://logs/info.log") == False
+        >>> _is_relative_path(r"C:\\info.log") == False
+        >>> _is_relative_path(r"\\'info.log") == False
+        >>> _is_relative_path("c:/info.log") == False
+        >>> _is_relative_path("s3://info.log") == False
 
     Args:
         path_string: The path string to check.
     Returns:
         Whether the string is a relative path.
     """
     # os.path.splitdrive does not reliably work on non-Windows systems
@@ -63,21 +63,21 @@
     Example:
     ::
         >>> conf = _convert_paths_to_absolute_posix(
         >>>     project_path=Path("/path/to/my/project"),
         >>>     conf_dictionary={
         >>>         "handlers": {
         >>>             "info_file_handler": {
-        >>>                 "filename": "logs/info.log"
+        >>>                 "filename": "info.log"
         >>>             }
         >>>         }
         >>>     }
         >>> )
         >>> print(conf['handlers']['info_file_handler']['filename'])
-        "/path/to/my/project/logs/info.log"
+        "/path/to/my/project/info.log"
 
     Args:
         project_path: The root directory to prepend to relative path to make absolute path.
         conf_dictionary: The configuration containing paths to expand.
     Returns:
         A dictionary containing only absolute paths.
     Raises:
```

### Comparing `kedro-0.18.7/kedro/framework/hooks/manager.py` & `kedro-0.18.8/kedro/framework/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/hooks/specs.py` & `kedro-0.18.8/kedro/framework/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/project/__init__.py` & `kedro-0.18.8/kedro/framework/project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,14 @@
     )
     _CONFIG_LOADER_ARGS = Validator("CONFIG_LOADER_ARGS", default={})
     _DATA_CATALOG_CLASS = _IsSubclassValidator(
         "DATA_CATALOG_CLASS", default=_get_default_class("kedro.io.DataCatalog")
     )
 
     def __init__(self, *args, **kwargs):
-
         kwargs.update(
             validators=[
                 self._CONF_SOURCE,
                 self._HOOKS,
                 self._CONTEXT_CLASS,
                 self._SESSION_STORE_CLASS,
                 self._SESSION_STORE_ARGS,
@@ -129,14 +128,15 @@
         super().__init__(*args, **kwargs)
 
 
 def _load_data_wrapper(func):
     """Wrap a method in _ProjectPipelines so that data is loaded on first access.
     Taking inspiration from dynaconf.utils.functional.new_method_proxy
     """
+
     # pylint: disable=protected-access
     def inner(self, *args, **kwargs):
         self._load_data()
         return func(self._content, *args, **kwargs)
 
     return inner
 
@@ -208,20 +208,21 @@
     __repr__ = _load_data_wrapper(repr)
     __str__ = _load_data_wrapper(str)
 
 
 class _ProjectLogging(UserDict):
     # pylint: disable=super-init-not-called
     def __init__(self):
-        """Initialise project logging with default configuration. Also enable
-        rich tracebacks."""
-        default_logging = (Path(__file__).parent / "default_logging.yml").read_text(
-            encoding="utf-8"
+        """Initialise project logging. The path to logging configuration is given in
+        environment variable KEDRO_LOGGING_CONFIG (defaults to default_logging.yml)."""
+        path = os.environ.get(
+            "KEDRO_LOGGING_CONFIG", Path(__file__).parent / "default_logging.yml"
         )
-        self.configure(yaml.safe_load(default_logging))
+        logging_config = Path(path).read_text(encoding="utf-8")
+        self.configure(yaml.safe_load(logging_config))
         logging.captureWarnings(True)
 
         # We suppress click here to hide tracebacks related to it conversely,
         # kedro is not suppressed to show its tracebacks for easier debugging.
         # sys.executable is used to get the kedro executable path to hide the
         # top level traceback.
         # Rich traceback handling does not work on databricks. Hopefully this will be
```

### Comparing `kedro-0.18.7/kedro/framework/session/session.py` & `kedro-0.18.8/kedro/framework/session/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module implements Kedro session responsible for project lifecycle."""
 import getpass
 import logging
 import logging.config
 import os
 import subprocess
+import sys
 import traceback
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, Optional, Union
 
 import click
 from omegaconf import OmegaConf, omegaconf
@@ -33,36 +34,38 @@
     project_path = str(project_path)
     try:
         res = subprocess.check_output(
             ["git", "rev-parse", "--short", "HEAD"],
             cwd=project_path,
             stderr=subprocess.STDOUT,
         )
-        git_data = {"commit_sha": res.decode().strip()}  # type: Dict[str, Any]
+        git_data: Dict[str, Any] = {"commit_sha": res.decode().strip()}
         git_status_res = subprocess.check_output(
             ["git", "status", "--short"],
             cwd=project_path,
             stderr=subprocess.STDOUT,
         )
         git_data["dirty"] = bool(git_status_res.decode().strip())
 
     # `subprocess.check_output()` raises `NotADirectoryError` on Windows
-    except (subprocess.CalledProcessError, FileNotFoundError, NotADirectoryError):
-        logging.getLogger(__name__).debug("Unable to git describe %s", project_path)
+    except Exception:  # pylint: disable=broad-except
+        logger = logging.getLogger(__name__)
+        logger.debug("Unable to git describe %s", project_path)
+        logger.debug(traceback.format_exc())
         return {}
 
     return {"git": git_data}
 
 
 def _jsonify_cli_context(ctx: click.core.Context) -> Dict[str, Any]:
     return {
         "args": ctx.args,
         "params": ctx.params,
         "command_name": ctx.command.name,
-        "command_path": ctx.command_path,
+        "command_path": " ".join(["kedro"] + sys.argv[1:]),
     }
 
 
 class KedroSessionError(Exception):
     """``KedroSessionError`` raised by ``KedroSession``
     in the case that multiple runs are attempted in one session.
     """
@@ -160,15 +163,14 @@
 
         # have to explicitly type session_data otherwise mypy will complain
         # possibly related to this: https://github.com/python/mypy/issues/1430
         session_data: Dict[str, Any] = {
             "package_name": session._package_name,
             "project_path": session._project_path,
             "session_id": session.session_id,
-            **_describe_git(session._project_path),
         }
 
         ctx = click.get_current_context(silent=True)
         if ctx:
             session_data["cli"] = _jsonify_cli_context(ctx)
 
         env = env or os.getenv("KEDRO_ENV")
@@ -183,16 +185,19 @@
         except Exception as exc:  # pylint: disable=broad-except
             logging.getLogger(__name__).debug(
                 "Unable to get username. Full exception: %s", exc
             )
 
         session._store.update(session_data)
 
-        # we need a ConfigLoader registered in order to be able to set up logging
+        # We need ConfigLoader and env to setup logging correctly
         session._setup_logging()
+        session_data.update(**_describe_git(session._project_path))
+        session._store.update(session_data)
+
         return session
 
     def _get_logging_config(self) -> Dict[str, Any]:
         logging_config = self._get_config_loader()["logging"]
         if isinstance(logging_config, omegaconf.DictConfig):
             logging_config = OmegaConf.to_container(logging_config)
         # turn relative paths in logging config into absolute path
```

### Comparing `kedro-0.18.7/kedro/framework/session/shelvestore.py` & `kedro-0.18.8/kedro/framework/session/shelvestore.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     @property
     def _location(self) -> Path:
         return Path(self._path).expanduser().resolve() / self._session_id / "store"
 
     def read(self) -> Dict[str, Any]:
         """Read the data from disk using `shelve` package."""
-        data = {}  # type: Dict[str, Any]
+        data: Dict[str, Any] = {}
         try:
             with shelve.open(str(self._location), flag="r") as _sh:  # nosec
                 data = dict(_sh)
         except dbm.error:
             pass
         return data
```

### Comparing `kedro-0.18.7/kedro/framework/session/store.py` & `kedro-0.18.8/kedro/framework/session/store.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/framework/startup.py` & `kedro-0.18.8/kedro/framework/startup.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/io/__init__.py` & `kedro-0.18.8/kedro/io/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """``kedro.io`` provides functionality to read and write to a
-number of data sets. At core of the library is ``AbstractDataSet``
-which allows implementation of various ``AbstractDataSet``s.
+number of data sets. At core of the library is the ``AbstractDataSet`` class.
 """
 
 from .cached_dataset import CachedDataSet
 from .core import (
     AbstractDataSet,
     AbstractVersionedDataSet,
     DataSetAlreadyExistsError,
```

### Comparing `kedro-0.18.7/kedro/io/cached_dataset.py` & `kedro-0.18.8/kedro/io/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/io/core.py` & `kedro-0.18.8/kedro/io/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,17 @@
 _CONSISTENCY_WARNING = (
     "Save version '{}' did not match load version '{}' for {}. This is strongly "
     "discouraged due to inconsistencies it may cause between 'save' and "
     "'load' operations. Please refrain from setting exact load version for "
     "intermediate data sets where possible to avoid this warning."
 )
 
+# `kedro_datasets` is probed before `kedro.extras.datasets`,
+# hence the DeprecationWarning will not be shown
+# if the dataset is available in the former
 _DEFAULT_PACKAGES = ["kedro.io.", "kedro_datasets.", "kedro.extras.datasets.", ""]
 
 
 def parse_dataset_definition(
     config: Dict[str, Any], load_version: str = None, save_version: str = None
 ) -> Tuple[Type[AbstractDataSet], Dict[str, Any]]:
     """Parse and instantiate a dataset class using the configuration provided.
```

### Comparing `kedro-0.18.7/kedro/io/data_catalog.py` & `kedro-0.18.8/kedro/io/data_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
         Args:
             data_sets: A dictionary of data set names and data set instances.
             feed_dict: A feed dict with data to be added in memory.
             layers: A dictionary of data set layers. It maps a layer name
                 to a set of data set names, according to the
                 data engineering convention. For more details, see
-                https://kedro.readthedocs.io/en/stable/faq/faq.html#what-is-data-engineering-convention
+                https://docs.kedro.org/en/stable/resources/glossary.html#layers-data-engineering-convention
 
         Example:
         ::
 
             >>> from kedro.extras.datasets.pandas import CSVDataSet
             >>>
             >>> cars = CSVDataSet(filepath="cars.csv",
@@ -263,15 +263,15 @@
         missing_keys = load_versions.keys() - catalog.keys()
         if missing_keys:
             raise DataSetNotFoundError(
                 f"'load_versions' keys [{', '.join(sorted(missing_keys))}] "
                 f"are not found in the catalog."
             )
 
-        layers = defaultdict(set)  # type: Dict[str, Set[str]]
+        layers: Dict[str, Set[str]] = defaultdict(set)
         for ds_name, ds_config in catalog.items():
             ds_layer = ds_config.pop("layer", None)
             if ds_layer is not None:
                 layers[ds_layer].add(ds_name)
 
             ds_config = _resolve_credentials(ds_config, credentials)
             data_sets[ds_name] = AbstractDataSet.from_config(
```

### Comparing `kedro-0.18.7/kedro/io/lambda_dataset.py` & `kedro-0.18.8/kedro/io/lambda_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/io/memory_dataset.py` & `kedro-0.18.8/kedro/io/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/io/partitioned_dataset.py` & `kedro-0.18.8/kedro/io/partitioned_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         super().__init__()
 
         self._path = path
         self._filename_suffix = filename_suffix
         self._overwrite = overwrite
         self._protocol = infer_storage_options(self._path)["protocol"]
-        self._partition_cache = Cache(maxsize=1)  # type: Cache
+        self._partition_cache: Cache = Cache(maxsize=1)
 
         dataset = dataset if isinstance(dataset, dict) else {"type": dataset}
         self._dataset_type, self._dataset_config = parse_dataset_definition(dataset)
         if VERSION_KEY in self._dataset_config:
             raise DataSetError(
                 f"'{self.__class__.__name__}' does not support versioning of the "
                 f"underlying dataset. Please remove '{VERSIONED_FLAG_KEY}' flag from "
```

### Comparing `kedro-0.18.7/kedro/ipython/__init__.py` & `kedro-0.18.8/kedro/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/ipython/logo-32x32.png` & `kedro-0.18.8/kedro/ipython/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/ipython/logo-64x64.png` & `kedro-0.18.8/kedro/ipython/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/ipython/logo-svg.svg` & `kedro-0.18.8/kedro/ipython/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/pipeline/modular_pipeline.py` & `kedro-0.18.8/kedro/pipeline/modular_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     *,
     inputs: Union[str, Set[str], Dict[str, str]] = None,
     outputs: Union[str, Set[str], Dict[str, str]] = None,
     parameters: Union[str, Set[str], Dict[str, str]] = None,
     tags: Union[str, Iterable[str]] = None,
     namespace: str = None,
 ) -> Pipeline:
-    """Create a ``Pipeline`` from a collection of nodes and/or ``Pipeline``s.
+    r"""Create a ``Pipeline`` from a collection of nodes and/or ``Pipeline``\s.
 
     Args:
         pipe: The nodes the ``Pipeline`` will be made of. If you
             provide pipelines among the list of nodes, those pipelines will
             be expanded and all their nodes will become part of this
             new pipeline.
         inputs: A name or collection of input names to be exposed as connection points
```

### Comparing `kedro-0.18.7/kedro/pipeline/node.py` & `kedro-0.18.8/kedro/pipeline/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,16 +494,16 @@
                 f"{common_in_out}"
             )
 
     @staticmethod
     def _process_inputs_for_bind(inputs: Union[None, str, List[str], Dict[str, str]]):
         # Safeguard that we do not mutate list inputs
         inputs = copy.copy(inputs)
-        args = []  # type: List[str]
-        kwargs = {}  # type: Dict[str, str]
+        args: List[str] = []
+        kwargs: Dict[str, str] = {}
         if isinstance(inputs, str):
             args = [inputs]
         elif isinstance(inputs, list):
             args = inputs
         elif isinstance(inputs, dict):
             kwargs = inputs
         return args, kwargs
```

### Comparing `kedro-0.18.7/kedro/pipeline/pipeline.py` & `kedro-0.18.8/kedro/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,21 +146,21 @@
         nodes = [n.tag(_tags) for n in nodes]
 
         self._nodes_by_name = {node.name: node for node in nodes}
         _validate_unique_outputs(nodes)
         _validate_unique_confirms(nodes)
 
         # input -> nodes with input
-        self._nodes_by_input = defaultdict(set)  # type: Dict[str, Set[Node]]
+        self._nodes_by_input: Dict[str, Set[Node]] = defaultdict(set)
         for node in nodes:
             for input_ in node.inputs:
                 self._nodes_by_input[_strip_transcoding(input_)].add(node)
 
         # output -> node with output
-        self._nodes_by_output = {}  # type: Dict[str, Node]
+        self._nodes_by_output: Dict[str, Node] = {}
         for node in nodes:
             for output in node.outputs:
                 self._nodes_by_output[_strip_transcoding(output)] = node
 
         self._nodes = nodes
         self._topo_sorted_nodes = _topologically_sorted(self.node_dependencies)
 
@@ -325,17 +325,15 @@
         """All dependencies of nodes where the first Node has a direct dependency on
         the second Node.
 
         Returns:
             Dictionary where keys are nodes and values are sets made up of
             their parent nodes. Independent nodes have this as empty sets.
         """
-        dependencies = {
-            node: set() for node in self._nodes
-        }  # type: Dict[Node, Set[Node]]
+        dependencies: Dict[Node, Set[Node]] = {node: set() for node in self._nodes}
         for parent in self._nodes:
             for output in parent.outputs:
                 for child in self._nodes_by_input[_strip_transcoding(output)]:
                     dependencies[child].add(parent)
 
         return dependencies
 
@@ -535,15 +533,15 @@
             A new ``Pipeline`` object, containing a subset of the
                 nodes of the current one such that only nodes depending
                 directly or transitively on the provided inputs are being
                 copied.
 
         """
         starting = set(inputs)
-        result = set()  # type: Set[Node]
+        result: Set[Node] = set()
         next_nodes = self._get_nodes_with_inputs_transcode_compatible(starting)
 
         while next_nodes:
             result |= next_nodes
             outputs = set(chain.from_iterable(node.outputs for node in next_nodes))
             starting = outputs
 
@@ -600,15 +598,15 @@
         Returns:
             A new ``Pipeline`` object, containing a subset of the nodes of the
             current one such that only nodes which are directly or transitively
             required to produce the provided outputs are being copied.
 
         """
         starting = set(outputs)
-        result = set()  # type: Set[Node]
+        result: Set[Node] = set()
         next_nodes = self._get_nodes_with_outputs_transcode_compatible(starting)
 
         while next_nodes:
             result |= next_nodes
             inputs = set(chain.from_iterable(node.inputs for node in next_nodes))
             starting = inputs
 
@@ -799,16 +797,16 @@
             "pipeline": transformed,
         }
 
         return json.dumps(pipeline_versioned)
 
 
 def _validate_duplicate_nodes(nodes_or_pipes: Iterable[Union[Node, Pipeline]]):
-    seen_nodes = set()  # type: Set[str]
-    duplicates = defaultdict(set)  # type: Dict[Union[Pipeline, None], Set[str]]
+    seen_nodes: Set[str] = set()
+    duplicates: Dict[Union[Pipeline, None], Set[str]] = defaultdict(set)
 
     def _check_node(node_: Node, pipeline_: Pipeline = None):
         name = node_.name
         if name in seen_nodes:
             duplicates[pipeline_].add(name)
         else:
             seen_nodes.add(name)
```

### Comparing `kedro-0.18.7/kedro/runner/parallel_runner.py` & `kedro-0.18.8/kedro/runner/parallel_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from collections import Counter
 from concurrent.futures import FIRST_COMPLETED, ProcessPoolExecutor, wait
 from itertools import chain
 from multiprocessing.managers import BaseProxy, SyncManager  # type: ignore
 from multiprocessing.reduction import ForkingPickler
 from pickle import PicklingError
-from typing import Any, Dict, Iterable, Set  # noqa
+from typing import Any, Dict, Iterable, Set
 
 from pluggy import PluginManager
 
 from kedro.framework.hooks.manager import (
     _create_hook_manager,
     _register_hooks,
     _register_hooks_setuptools,
@@ -286,15 +286,15 @@
         nodes = pipeline.nodes
         self._validate_catalog(catalog, pipeline)
         self._validate_nodes(nodes)
 
         load_counts = Counter(chain.from_iterable(n.inputs for n in nodes))
         node_dependencies = pipeline.node_dependencies
         todo_nodes = set(node_dependencies.keys())
-        done_nodes = set()  # type: Set[Node]
+        done_nodes: Set[Node] = set()
         futures = set()
         done = None
         max_workers = self._get_required_workers_count(pipeline)
 
         from kedro.framework.project import LOGGING, PACKAGE_NAME
 
         with ProcessPoolExecutor(max_workers=max_workers) as pool:
```

### Comparing `kedro-0.18.7/kedro/runner/runner.py` & `kedro-0.18.8/kedro/runner/runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/runner/sequential_runner.py` & `kedro-0.18.8/kedro/runner/sequential_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/runner/thread_runner.py` & `kedro-0.18.8/kedro/runner/thread_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 be used to run the ``Pipeline`` in parallel groups formed by toposort
 using threads.
 """
 import warnings
 from collections import Counter
 from concurrent.futures import FIRST_COMPLETED, ThreadPoolExecutor, wait
 from itertools import chain
-from typing import Set  # noqa
+from typing import Set
 
 from pluggy import PluginManager
 
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline
-from kedro.pipeline.node import Node  # noqa
+from kedro.pipeline.node import Node
 from kedro.runner.runner import AbstractRunner, run_node
 
 
 class ThreadRunner(AbstractRunner):
     """``ThreadRunner`` is an ``AbstractRunner`` implementation. It can
     be used to run the ``Pipeline`` in parallel groups formed by toposort
     using threads.
@@ -99,15 +99,15 @@
             Exception: in case of any downstream node failure.
 
         """
         nodes = pipeline.nodes
         load_counts = Counter(chain.from_iterable(n.inputs for n in nodes))
         node_dependencies = pipeline.node_dependencies
         todo_nodes = set(node_dependencies.keys())
-        done_nodes = set()  # type: Set[Node]
+        done_nodes: Set[Node] = set()
         futures = set()
         done = None
         max_workers = self._get_required_workers_count(pipeline)
 
         with ThreadPoolExecutor(max_workers=max_workers) as pool:
             while True:
                 ready = {n for n in todo_nodes if node_dependencies[n] <= done_nodes}
```

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,15 @@
     formatter: simple
     stream: ext://sys.stdout
 
   info_file_handler:
     class: logging.handlers.RotatingFileHandler
     level: INFO
     formatter: simple
-    filename: logs/info.log
-    maxBytes: 10485760 # 10MB
-    backupCount: 20
-    encoding: utf8
-    delay: True
-
-  error_file_handler:
-    class: logging.handlers.RotatingFileHandler
-    level: ERROR
-    formatter: simple
-    filename: logs/errors.log
+    filename: info.log
     maxBytes: 10485760 # 10MB
     backupCount: 20
     encoding: utf8
     delay: True
 
   rich:
     class: rich.logging.RichHandler
@@ -40,8 +30,8 @@
   kedro:
     level: INFO
 
   {{ cookiecutter.python_package }}:
     level: INFO
 
 root:
-  handlers: [rich, info_file_handler, error_file_handler]
+  handlers: [rich, info_file_handler]
```

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro/utils.py` & `kedro-0.18.8/kedro/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/kedro.egg-info/PKG-INFO` & `kedro-0.18.8/kedro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.18.7
+Version: 0.18.8
 Summary: Kedro helps you build production-ready data and analytics pipelines
-Home-page: https://github.com/kedro-org/kedro
 Author: Kedro
 License: Apache Software License (Apache 2.0)
+Project-URL: Homepage, https://kedro.org
+Project-URL: Source, https://github.com/kedro-org/kedro
+Project-URL: Documentation, https://docs.kedro.org
+Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: biosequence
 Provides-Extra: dask
 Provides-Extra: docs
 Provides-Extra: geopandas
 Provides-Extra: matplotlib
@@ -135,15 +138,15 @@
  - To enhance **team collaboration** when different team members have varied exposure to software engineering concepts
  - To increase efficiency, because applied concepts like modularity and separation of concerns inspire the creation of
   **reusable analytics code**
 
 
 ## The humans behind Kedro
 
-The [Kedro product team](https://docs.kedro.org/en/stable/faq/faq.html#who-maintains-kedro) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
+The [Kedro product team](https://docs.kedro.org/en/stable/contribution/technical_steering_committee.html#kedro-maintainers) and a number of [open source contributors from across the world](https://github.com/kedro-org/kedro/releases) maintain Kedro.
 
 
 ## Can I contribute?
 
 Yes! Want to help build Kedro? Check out our [guide to contributing to Kedro](https://github.com/kedro-org/kedro/blob/main/CONTRIBUTING.md).
```

### Comparing `kedro-0.18.7/kedro.egg-info/SOURCES.txt` & `kedro-0.18.8/kedro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,14 @@
 kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
 kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
-kedro/templates/project/{{ cookiecutter.repo_name }}/logs/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
 kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
```

### Comparing `kedro-0.18.7/kedro.egg-info/requires.txt` & `kedro-0.18.8/kedro.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 anyconfig~=0.10.0
 attrs>=21.3
 cachetools~=5.3
 click<9.0
 cookiecutter<3.0,>=2.1.1
 dynaconf<4.0,>=3.1.2
+fsspec<2024.1,>=2021.4
 gitpython~=3.0
 importlib_resources>=1.3
 jmespath<1.0,>=0.9.5
-more_itertools~=9.1
+more_itertools~=9.0
 omegaconf~=2.3
-pip-tools~=6.12
+pip-tools~=6.5
 pluggy~=1.0.0
 PyYAML<7.0,>=4.2
-rich~=13.3
-rope~=1.7.0
+rich<14.0,>=12.0
+rope<2.0,>=0.21
 setuptools>=65.5.1
 toml~=0.10
-toposort~=1.10
+toposort~=1.5
 
 [:python_version < "3.8"]
 importlib_metadata<5.0,>=3.6
 
-[:python_version == "3.7"]
-fsspec<=2023.1.0,>=2021.4
-
 [:python_version >= "3.8"]
-fsspec<2023.4,>=2023.1
 importlib-metadata>=3.6
 
 [all]
 Jinja2<3.1.0
 Pillow~=9.0
 PyYAML<7.0,>=4.2
 SQLAlchemy~=1.2
@@ -38,44 +35,50 @@
 dask[complete]~=2021.10
 delta-spark<3.0,>=1.0
 docutils==0.16
 geopandas<1.0,>=0.6.0
 hdfs<3.0,>=2.5.8
 holoviews~=1.13.0
 ipykernel<7.0,>=5.3
+kedro-datasets[api,biosequence,dask,geopandas,holoviews,matplotlib,networkx,pandas,pillow,plotly,polars,redis,spark,svmlight,video,yaml]==1.1.1
 lxml~=4.6
 matplotlib<4.0,>=3.0.3
-myst-parser~=0.17.2
-nbsphinx==0.8.1
-nbstripout~=0.4
+myst-parser~=1.0.0
 networkx~=2.4
 opencv-python~=4.5.5.64
 openpyxl<4.0,>=3.0.6
 pandas-gbq<0.18.0,>=0.12.0
 pandas~=1.3
 plotly<6.0,>=4.8.0
 pyarrow<7.0,>=1.0
 pyproj~=3.0
 pyspark<4.0,>=2.2
 redis~=4.1
 requests~=2.20
 s3fs<0.5,>=0.3.0
 scikit-learn~=1.0.2
 scipy~=1.7.3
-sphinx-autodoc-typehints==1.11.1
+sphinx-autodoc-typehints==1.20.2
+sphinx-notfound-page
 sphinx_copybutton==0.3.1
-sphinx_rtd_theme==1.1.1
+sphinx_rtd_theme==1.2.0
 sphinxcontrib-mermaid~=0.7.1
-sphinx~=3.4.3
+sphinx~=5.3.0
 tensorflow~=2.0
 triad<1.0,>=0.6.7
 
+[all:platform_system != "Darwin" or platform_machine != "arm64"]
+kedro-datasets[tensorflow]==1.1.1
+
 [all:platform_system != "Windows"]
 tables~=3.6
 
+[all:platform_system == "Darwin" and platform_machine == "arm64"]
+tensorflow-macos~=2.0
+
 [all:platform_system == "Windows"]
 tables~=3.6.0
 
 [api]
 requests~=2.20
 
 [api.APIDataSet]
@@ -93,24 +96,30 @@
 
 [dask.ParquetDataSet]
 dask[complete]~=2021.10
 triad<1.0,>=0.6.7
 
 [docs]
 docutils==0.16
-sphinx~=3.4.3
-sphinx_rtd_theme==1.1.1
-nbsphinx==0.8.1
-nbstripout~=0.4
-sphinx-autodoc-typehints==1.11.1
+sphinx~=5.3.0
+sphinx_rtd_theme==1.2.0
+sphinx-autodoc-typehints==1.20.2
 sphinx_copybutton==0.3.1
+sphinx-notfound-page
 ipykernel<7.0,>=5.3
 sphinxcontrib-mermaid~=0.7.1
-myst-parser~=0.17.2
+myst-parser~=1.0.0
 Jinja2<3.1.0
+kedro-datasets[api,biosequence,dask,geopandas,holoviews,matplotlib,networkx,pandas,pillow,plotly,polars,redis,spark,svmlight,video,yaml]==1.1.1
+
+[docs:platform_system != "Darwin" or platform_machine != "arm64"]
+kedro-datasets[tensorflow]==1.1.1
+
+[docs:platform_system == "Darwin" and platform_machine == "arm64"]
+tensorflow-macos~=2.0
 
 [geopandas]
 geopandas<1.0,>=0.6.0
 pyproj~=3.0
 
 [geopandas.GeoJSONDataSet]
 geopandas<1.0,>=0.6.0
```

### Comparing `kedro-0.18.7/pyproject.toml` & `kedro-0.18.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 # PEP-518 https://peps.python.org/pep-0518/
 [build-system]
 # Minimum requirements for the build system to execute.
-requires = ["setuptools>=65.5.1", "wheel"]  # PEP 518 specifications.
+requires = ["setuptools>=65.5.1"]  # PEP 518 specifications
+
+[project]
+name = "kedro"
+authors = [
+    {name = "Kedro"}
+]
+description = "Kedro helps you build production-ready data and analytics pipelines"
+requires-python = ">=3.7, <3.11"
+keywords = [
+    "pipelines",
+    "machine learning",
+    "data pipelines",
+    "data science",
+    "data engineering",
+]
+license = {text = "Apache Software License (Apache 2.0)"}
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+]
+dynamic = ["readme", "version", "dependencies", "optional-dependencies"]
+
+[project.urls]
+Homepage = "https://kedro.org"
+Source = "https://github.com/kedro-org/kedro"
+Documentation = "https://docs.kedro.org"
+Tracker = "https://github.com/kedro-org/kedro/issues"
+
+[project.scripts]
+kedro = "kedro.framework.cli:main"
+
+[tool.setuptools]
+zip-safe = false
+
+[tool.setuptools.packages.find]
+include = ["kedro*"]
+
+[tool.setuptools.dynamic]
+readme = {file = "README.md", content-type = "text/markdown"}
+version = {attr = "kedro.__version__"}
+dependencies = {file = "dependency/requirements.txt"}
 
 [tool.black]
 exclude = "/templates/|^features/steps/test_starter"
 
 [tool.isort]
 profile = "black"
```

### Comparing `kedro-0.18.7/setup.py` & `kedro-0.18.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,27 @@
-import re
 from codecs import open
 from glob import glob
 from itertools import chain
 from os import path
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
 name = "kedro"
 here = path.abspath(path.dirname(__file__))
 
 # at least 1.3 to be able to use XMLDataSet and pandas integration with fsspec
 PANDAS = "pandas~=1.3"
 SPARK = "pyspark>=2.2, <4.0"
 HDFS = "hdfs>=2.5.8, <3.0"
 S3FS = "s3fs>=0.3.0, <0.5"
 
-# get package version
-with open(path.join(here, name, "__init__.py"), encoding="utf-8") as f:
-    result = re.search(r'__version__ = ["\']([^"\']+)', f.read())
-
-    if not result:
-        raise ValueError("Can't find the version in kedro/__init__.py")
-
-    version = result.group(1)
-
 # get the dependencies and installs
 with open("dependency/requirements.txt", encoding="utf-8") as f:
     requires = [x.strip() for x in f if x.strip()]
 
-# get test dependencies and installs
-with open("test_requirements.txt", encoding="utf-8") as f:
-    test_requires = [x.strip() for x in f if x.strip() and not x.startswith("-r")]
-
-
-# Get the long description from the README file
-with open(path.join(here, "README.md"), encoding="utf-8") as f:
-    readme = f.read()
-
 template_files = []
 for pattern in ["**/*", "**/.*", "**/.*/**", "**/.*/.**"]:
     template_files.extend(
         [
             name.replace("kedro/", "", 1)
             for name in glob("kedro/templates/" + pattern, recursive=True)
         ]
@@ -105,25 +86,33 @@
 yaml_require = {"yaml.YAMLDataSet": [PANDAS, "PyYAML>=4.2, <7.0"]}
 
 extras_require = {
     "api": _collect_requirements(api_require),
     "biosequence": _collect_requirements(biosequence_require),
     "dask": _collect_requirements(dask_require),
     "docs": [
+        # docutils>=0.17 changed the HTML
+        # see https://github.com/readthedocs/sphinx_rtd_theme/issues/1115
         "docutils==0.16",
-        "sphinx~=3.4.3",
-        "sphinx_rtd_theme==1.1.1",
-        "nbsphinx==0.8.1",
-        "nbstripout~=0.4",
-        "sphinx-autodoc-typehints==1.11.1",
+        "sphinx~=5.3.0",
+        "sphinx_rtd_theme==1.2.0",
+        # Regression on sphinx-autodoc-typehints 1.21
+        # that creates some problematic docstrings
+        "sphinx-autodoc-typehints==1.20.2",
         "sphinx_copybutton==0.3.1",
+        "sphinx-notfound-page",
         "ipykernel>=5.3, <7.0",
         "sphinxcontrib-mermaid~=0.7.1",
-        "myst-parser~=0.17.2",
+        "myst-parser~=1.0.0",
         "Jinja2<3.1.0",
+        # https://github.com/kedro-org/kedro-plugins/issues/141
+        # https://github.com/kedro-org/kedro-plugins/issues/143
+        "kedro-datasets[api,biosequence,dask,geopandas,matplotlib,holoviews,networkx,pandas,pillow,polars,video,plotly,redis,spark,svmlight,yaml]==1.1.1",
+        "kedro-datasets[tensorflow]==1.1.1; platform_system != 'Darwin' or platform_machine != 'arm64'",
+        "tensorflow-macos~=2.0; platform_system == 'Darwin' and platform_machine == 'arm64'",
     ],
     "geopandas": _collect_requirements(geopandas_require),
     "matplotlib": _collect_requirements(matplotlib_require),
     "holoviews": _collect_requirements(holoviews_require),
     "networkx": _collect_requirements(networkx_require),
     "pandas": _collect_requirements(pandas_require),
     "pickle": _collect_requirements(pickle_require),
@@ -152,35 +141,12 @@
     **tensorflow_required,
     **yaml_require,
 }
 
 extras_require["all"] = _collect_requirements(extras_require)
 
 setup(
-    name=name,
-    version=version,
-    description="Kedro helps you build production-ready data and analytics pipelines",
-    license="Apache Software License (Apache 2.0)",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    url="https://github.com/kedro-org/kedro",
-    python_requires=">=3.7, <3.11",
-    packages=find_packages(exclude=["docs*", "tests*", "tools*", "features*"]),
-    include_package_data=True,
-    tests_require=test_requires,
-    install_requires=requires,
-    author="Kedro",
-    entry_points={"console_scripts": ["kedro = kedro.framework.cli:main"]},
     package_data={
         name: ["py.typed", "test_requirements.txt"] + template_files
     },
-    zip_safe=False,
-    keywords="pipelines, machine learning, data pipelines, data science, data engineering",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-    ],
     extras_require=extras_require,
 )
```

### Comparing `kedro-0.18.7/test_requirements.txt` & `kedro-0.18.8/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `kedro-0.18.7/tests/test_utils.py` & `kedro-0.18.8/tests/test_utils.py`

 * *Files identical despite different names*

