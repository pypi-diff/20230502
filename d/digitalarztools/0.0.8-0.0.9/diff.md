# Comparing `tmp/digitalarztools-0.0.8.tar.gz` & `tmp/digitalarztools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/digitalarztools-0.0.8.tar", last modified: Fri Apr 14 15:06:47 2023, max compression
+gzip compressed data, was "dist/digitalarztools-0.0.9.tar", last modified: Sat Apr 15 00:59:19 2023, max compression
```

## Comparing `digitalarztools-0.0.8.tar` & `digitalarztools-0.0.9.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.749206 digitalarztools-0.0.8/
--rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-14 15:06:47.748707 digitalarztools-0.0.8/PKG-INFO
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.658429 digitalarztools-0.0.8/digitalarztools/
--rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.0.8/digitalarztools/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.662592 digitalarztools-0.0.8/digitalarztools/io/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.0.8/digitalarztools/io/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7106 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/io/file_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      606 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/io/url_io.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.664300 digitalarztools-0.0.8/digitalarztools/operations/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/operations/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1433 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/operations/transformation.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.668883 digitalarztools-0.0.8/digitalarztools/pipelines/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5517 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/alos_palser.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.671071 digitalarztools-0.0.8/digitalarztools/pipelines/config/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/config/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4188 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/config/data_centers.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.673344 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3059 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15085 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/m2m.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.674604 digitalarztools-0.0.8/digitalarztools/pipelines/gee/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.675372 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.681417 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1582 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/auth.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/feature_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_api.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1092 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_map.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8600 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6061 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4608 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/region.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/grace.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      307 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/landsat.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.686826 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2898 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/chirp.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    13082 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/geos.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    24728 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/merra.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/variables_info.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.692979 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3621 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    12834 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/soil_contents.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4915 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_fc.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3705 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_res.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7294 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_sat2.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4037 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/srtm.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.704686 digitalarztools-0.0.8/digitalarztools/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-03 12:45:02.000000 digitalarztools-0.0.8/digitalarztools/raster/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.727369 digitalarztools-0.0.8/digitalarztools/raster/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/biomass_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/clear_sky_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/constants.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/dem_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/emissivity_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/et_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/leaf_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/meteo_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/resistance_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/roughness_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_moisture.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/solar_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/temperature_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/unstable.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/vegitation_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/water_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3427 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/band_process.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5726 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/cog_raster.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.731834 digitalarztools-0.0.8/digitalarztools/raster/datasets/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    40684 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_modis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_probav_viirs.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    14536 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/gdal_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2508 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/gdal_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8494 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/hdf_reader.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2022-10-08 11:45:28.000000 digitalarztools-0.0.8/digitalarztools/raster/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.732954 digitalarztools-0.0.8/digitalarztools/raster/opencv/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/raster/opencv/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/opencv/segmentation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2118 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_extraction.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9789 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_process.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    34443 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_raster.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.735591 digitalarztools-0.0.8/digitalarztools/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.737219 digitalarztools-0.0.8/digitalarztools/test/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/raster/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/raster/test_functionalities.py
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/test_config.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.742603 digitalarztools-0.0.8/digitalarztools/utils/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/utils/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/utils/date_utils.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/utils/logger.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5487 2023-04-14 08:02:54.000000 digitalarztools-0.0.8/digitalarztools/utils/s3_utils.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/utils/waitbar_console.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.743865 digitalarztools-0.0.8/digitalarztools/vector/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 10:28:22.000000 digitalarztools-0.0.8/digitalarztools/vector/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8757 2023-03-02 22:15:56.000000 digitalarztools-0.0.8/digitalarztools/vector/gpd_vector.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.660757 digitalarztools-0.0.8/digitalarztools.egg-info/
--rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/PKG-INFO
--rw-r--r--   0 atherashraf   (501) staff       (20)     3898 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/SOURCES.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/dependency_links.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/top_level.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-04-14 15:06:47.749336 digitalarztools-0.0.8/setup.cfg
--rw-r--r--   0 atherashraf   (501) staff       (20)     1449 2023-04-14 08:03:38.000000 digitalarztools-0.0.8/setup.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.747069 digitalarztools-0.0.8/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.0.8/test/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.0.8/test/test_config.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      783 2022-12-04 11:47:04.000000 digitalarztools-0.0.8/test/test_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      309 2022-12-04 11:11:10.000000 digitalarztools-0.0.8/test/test_vector_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.574210 digitalarztools-0.0.9/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-15 00:59:19.573950 digitalarztools-0.0.9/PKG-INFO
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.531837 digitalarztools-0.0.9/digitalarztools/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.0.9/digitalarztools/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.534451 digitalarztools-0.0.9/digitalarztools/io/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.0.9/digitalarztools/io/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7106 2023-04-14 08:01:50.000000 digitalarztools-0.0.9/digitalarztools/io/file_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      606 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/io/url_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.534952 digitalarztools-0.0.9/digitalarztools/operations/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/operations/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1433 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/operations/transformation.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.537172 digitalarztools-0.0.9/digitalarztools/pipelines/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5517 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/alos_palser.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.538335 digitalarztools-0.0.9/digitalarztools/pipelines/config/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/config/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4188 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/config/data_centers.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.540372 digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3059 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15085 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/m2m.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.541399 digitalarztools-0.0.9/digitalarztools/pipelines/gee/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.542702 digitalarztools-0.0.9/digitalarztools/pipelines/gee/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/analysis/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.547059 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1582 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/auth.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/feature_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/gee_api.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1092 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/gee_map.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8600 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/image.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6061 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/image_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4608 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/region.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/grace.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      307 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/landsat.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.550826 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2898 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/chirp.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    13082 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/geos.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    24728 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/merra.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/nasa/variables_info.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.553378 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3621 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    12834 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/soil_contents.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4915 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_fc.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3705 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_res.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7294 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_sat2.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4037 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/pipelines/srtm.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.557810 digitalarztools-0.0.9/digitalarztools/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-03 12:45:02.000000 digitalarztools-0.0.9/digitalarztools/raster/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.565818 digitalarztools-0.0.9/digitalarztools/raster/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/biomass_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/clear_sky_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/constants.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/dem_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/emissivity_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/et_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/leaf_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/meteo_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/resistance_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/roughness_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/soil_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/soil_moisture.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/solar_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/temperature_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/unstable.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/vegitation_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/analysis/water_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3427 2023-04-14 08:01:50.000000 digitalarztools-0.0.9/digitalarztools/raster/band_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5534 2023-04-15 00:49:56.000000 digitalarztools-0.0.9/digitalarztools/raster/cog_raster.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.567541 digitalarztools-0.0.9/digitalarztools/raster/datasets/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/datasets/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    40684 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/datasets/rio_landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/datasets/rio_modis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/datasets/rio_probav_viirs.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14536 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/gdal_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2508 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/gdal_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8494 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/hdf_reader.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2022-10-08 11:45:28.000000 digitalarztools-0.0.9/digitalarztools/raster/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.568639 digitalarztools-0.0.9/digitalarztools/raster/opencv/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/raster/opencv/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/opencv/segmentation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2118 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/raster/rio_extraction.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9789 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/raster/rio_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    34443 2023-04-14 08:01:50.000000 digitalarztools-0.0.9/digitalarztools/raster/rio_raster.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.569816 digitalarztools-0.0.9/digitalarztools/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/test/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.570383 digitalarztools-0.0.9/digitalarztools/test/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/test/raster/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/test/raster/test_functionalities.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/test/test_config.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.572088 digitalarztools-0.0.9/digitalarztools/utils/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.9/digitalarztools/utils/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.0.9/digitalarztools/utils/date_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/utils/logger.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5487 2023-04-14 08:02:54.000000 digitalarztools-0.0.9/digitalarztools/utils/s3_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.0.9/digitalarztools/utils/waitbar_console.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.572565 digitalarztools-0.0.9/digitalarztools/vector/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 10:28:22.000000 digitalarztools-0.0.9/digitalarztools/vector/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8757 2023-03-02 22:15:56.000000 digitalarztools-0.0.9/digitalarztools/vector/gpd_vector.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.533447 digitalarztools-0.0.9/digitalarztools.egg-info/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-15 00:59:19.000000 digitalarztools-0.0.9/digitalarztools.egg-info/PKG-INFO
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3936 2023-04-15 00:59:19.000000 digitalarztools-0.0.9/digitalarztools.egg-info/SOURCES.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-04-15 00:59:19.000000 digitalarztools-0.0.9/digitalarztools.egg-info/dependency_links.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1194 2023-04-15 00:59:19.000000 digitalarztools-0.0.9/digitalarztools.egg-info/requires.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-04-15 00:59:19.000000 digitalarztools-0.0.9/digitalarztools.egg-info/top_level.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-04-15 00:59:19.574296 digitalarztools-0.0.9/setup.cfg
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1495 2023-04-15 00:59:17.000000 digitalarztools-0.0.9/setup.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-15 00:59:19.573616 digitalarztools-0.0.9/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.0.9/test/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.0.9/test/test_config.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      783 2022-12-04 11:47:04.000000 digitalarztools-0.0.9/test/test_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      309 2022-12-04 11:11:10.000000 digitalarztools-0.0.9/test/test_vector_io.py
```

### Comparing `digitalarztools-0.0.8/PKG-INFO` & `digitalarztools-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.0.8/digitalarztools/io/file_io.py` & `digitalarztools-0.0.9/digitalarztools/io/file_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/io/url_io.py` & `digitalarztools-0.0.9/digitalarztools/io/url_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/operations/transformation.py` & `digitalarztools-0.0.9/digitalarztools/operations/transformation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/alos_palser.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/alos_palser.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/config/data_centers.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/config/data_centers.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/landsat.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/m2m.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/earth_explorer/m2m.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/indices.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/analysis/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/auth.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/auth.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/feature_collection.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/feature_collection.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_api.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/gee_api.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_map.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/gee_map.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/image.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image_collection.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/image_collection.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/region.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/gee/core/region.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/chirp.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/nasa/chirp.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/geos.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/nasa/geos.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/merra.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/nasa/merra.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/variables_info.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/nasa/variables_info.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/n_van_genuchten.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/soil_contents.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/soil_contents.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_fc.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_fc.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_res.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_res.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_sat2.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/soil_grids/theta_sat2.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/pipelines/srtm.py` & `digitalarztools-0.0.9/digitalarztools/pipelines/srtm.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/biomass_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/biomass_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/clear_sky_radiation.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/constants.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/constants.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/dem_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/dem_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/emissivity_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/emissivity_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/et_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/et_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/leaf_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/leaf_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/meteo_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/meteo_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/resistance_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/resistance_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/roughness_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/roughness_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/soil_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_moisture.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/solar_radiation.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/temperature_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/temperature_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/unstable.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/unstable.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/vegitation_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/vegitation_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/analysis/water_analysis.py` & `digitalarztools-0.0.9/digitalarztools/raster/analysis/water_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/band_process.py` & `digitalarztools-0.0.9/digitalarztools/raster/band_process.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/cog_raster.py` & `digitalarztools-0.0.9/digitalarztools/raster/cog_raster.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from PIL import Image
 from rasterio.session import AWSSession
 
 from rio_tiler.io import COGReader
 from rio_tiler.colormap import cmap
 from rio_tiler.models import ImageData
 
-from api.utils import CommonUtils
+from digitalarztools.io.file_io import FileIO
 from digitalarztools.raster.rio_raster import RioRaster
-from da_utils.raster.s3 import S3Utils
-from digitalarz.settings import MEDIA_ROOT
 from rio_cogeo import cog_profiles, cog_translate
 
 
 class COGRaster:
     cog: COGReader
     file_path: str
 
@@ -60,19 +58,17 @@
         return RioRaster(self.cog.dataset)
 
     @classmethod
     def create_cog(cls, src_rio_raster: RioRaster, des_path: str,
                    profile: str = "deflate",
                    profile_options: dict = {},
                    **options):
-        CommonUtils.make_dirs(des_path)
+        FileIO.mkdirs(des_path)
         with src_rio_raster.get_dataset() as src:
             """Convert image to COG."""
-            # Format creation option (see gdalwarp `-co` option)
-            # profile = 'DEFLATE'  # ycbcr
             output_profile = cog_profiles.get(profile)
             output_profile.update(dict(BIGTIFF="IF_SAFER"))
             output_profile.update(profile_options)
 
             # Dataset Open option (see gdalwarp `-oo` option)
             config = dict(
                 GDAL_NUM_THREADS="ALL_CPUS",
@@ -140,16 +136,16 @@
         # blank_image[:, :, 3] = 0
         return self.create_image(blank_image)
 
     @staticmethod
     def create_image(np_array, format="PNG", f_name=None, is_data_file=False):
         img = Image.fromarray(np_array)
         if f_name and is_data_file:
-            fp = os.path.join(MEDIA_ROOT, f_name)
-            CommonUtils.make_dirs(fp)
+            fp = os.path.join('media/temp', f_name)
+            FileIO.mkdirs(fp)
             # img.save(fp, format)
 
         buffer = BytesIO()
         img.save(buffer, format=format)  # Enregistre l'image dans le buffer
         # return "data:image/PNG;base64," + base64.b64encode(buffer.getvalue()).decode()
         return buffer  # .getvalue()
```

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_landsat.py` & `digitalarztools-0.0.9/digitalarztools/raster/datasets/rio_landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_probav_viirs.py` & `digitalarztools-0.0.9/digitalarztools/raster/datasets/rio_probav_viirs.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/gdal_raster.py` & `digitalarztools-0.0.9/digitalarztools/raster/gdal_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/gdal_raster_io.py` & `digitalarztools-0.0.9/digitalarztools/raster/gdal_raster_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/hdf_reader.py` & `digitalarztools-0.0.9/digitalarztools/raster/hdf_reader.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/indices.py` & `digitalarztools-0.0.9/digitalarztools/raster/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/opencv/segmentation.py` & `digitalarztools-0.0.9/digitalarztools/raster/opencv/segmentation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/rio_extraction.py` & `digitalarztools-0.0.9/digitalarztools/raster/rio_extraction.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/rio_process.py` & `digitalarztools-0.0.9/digitalarztools/raster/rio_process.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/raster/rio_raster.py` & `digitalarztools-0.0.9/digitalarztools/raster/rio_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/test/raster/test_functionalities.py` & `digitalarztools-0.0.9/digitalarztools/test/raster/test_functionalities.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/utils/date_utils.py` & `digitalarztools-0.0.9/digitalarztools/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/utils/logger.py` & `digitalarztools-0.0.9/digitalarztools/utils/logger.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/utils/s3_utils.py` & `digitalarztools-0.0.9/digitalarztools/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/utils/waitbar_console.py` & `digitalarztools-0.0.9/digitalarztools/utils/waitbar_console.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools/vector/gpd_vector.py` & `digitalarztools-0.0.9/digitalarztools/vector/gpd_vector.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.8/digitalarztools.egg-info/PKG-INFO` & `digitalarztools-0.0.9/digitalarztools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.0.8/digitalarztools.egg-info/SOURCES.txt` & `digitalarztools-0.0.9/digitalarztools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 digitalarztools/__init__.py
 digitalarztools.egg-info/PKG-INFO
 digitalarztools.egg-info/SOURCES.txt
 digitalarztools.egg-info/dependency_links.txt
+digitalarztools.egg-info/requires.txt
 digitalarztools.egg-info/top_level.txt
 digitalarztools/io/__init__.py
 digitalarztools/io/file_io.py
 digitalarztools/io/url_io.py
 digitalarztools/operations/__init__.py
 digitalarztools/operations/transformation.py
 digitalarztools/pipelines/__init__.py
```

### Comparing `digitalarztools-0.0.8/setup.py` & `digitalarztools-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 pip install twine 
 python setup.py sdist bdist_wheel
 twine upload dist/* 
 """
 import os
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
-requirement_path = lib_folder + '/digitalarztools/requirements.txt'
+requirement_path = os.path.join(lib_folder, 'requirements.txt') #lib_folder + '/digitalarztools/requirements.txt'
 install_requires = []  # Here we'll get: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Digital Arz tools for applications'
 LONG_DESCRIPTION = 'Package provides tool for developing digitalarz application using rasterio, gdal, geopandas, and pandas'
 
 # Setting up
 setuptools.setup(
     name="digitalarztools",
     version=VERSION,
```

### Comparing `digitalarztools-0.0.8/test/test_raster_io.py` & `digitalarztools-0.0.9/test/test_raster_io.py`

 * *Files identical despite different names*

