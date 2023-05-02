# Comparing `tmp/wetterdienst-0.8.0.tar.gz` & `tmp/wetterdienst-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetterdienst-0.8.0.tar", last modified: Thu Sep 24 22:35:15 2020, max compression
+gzip compressed data, was "wetterdienst-0.9.0.tar", last modified: Fri Oct  9 18:45:43 2020, max compression
```

## Comparing `wetterdienst-0.8.0.tar` & `wetterdienst-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     3333 2020-09-24 22:31:54.126142 wetterdienst-0.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2063 2020-09-24 22:31:54.126142 wetterdienst-0.8.0/DWD_FILE_SERVER_STRUCTURE.md
--rw-r--r--   0        0        0     1123 2020-09-24 22:31:54.126142 wetterdienst-0.8.0/LICENSE.rst
--rw-r--r--   0        0        0     1123 2020-09-24 22:31:54.126142 wetterdienst-0.8.0/LICENSE.rst
--rw-r--r--   0        0        0     5300 2020-09-24 22:31:54.126142 wetterdienst-0.8.0/README.rst
--rw-r--r--   0        0        0     4888 2020-09-24 22:31:54.134142 wetterdienst-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1681 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/__init__.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/__init__.py
--rw-r--r--   0        0        0     1792 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/cache.py
--rw-r--r--   0        0        0    14495 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/functions.py
--rw-r--r--   0        0        0     8630 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/geo_location.py
--rw-r--r--   0        0        0     2005 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/time_handling.py
--rw-r--r--   0        0        0     1246 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/additionals/util.py
--rw-r--r--   0        0        0    13068 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/api.py
--rw-r--r--   0        0        0    15290 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/cli.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/__init__.py
--rw-r--r--   0        0        0      546 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/access_credentials.py
--rw-r--r--   0        0        0     1597 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/column_name_mapping.py
--rw-r--r--   0        0        0      566 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/metadata.py
--rw-r--r--   0        0        0     3877 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/parameter_mapping.py
--rw-r--r--   0        0        0      649 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/constants/time_resolution_mapping.py
--rw-r--r--   0        0        0     9988 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/data_collection.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/data_models/__init__.py
--rw-r--r--   0        0        0     1031 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/data_models/coordinates.py
--rw-r--r--   0        0        0     4861 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/data_storing.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/download/__init__.py
--rw-r--r--   0        0        0     6190 2020-09-24 22:31:54.154142 wetterdienst-0.8.0/wetterdienst/download/download.py
--rw-r--r--   0        0        0      602 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/download/download_services.py
--rw-r--r--   0        0        0      603 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/download/https_handling.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/__init__.py
--rw-r--r--   0        0        0    23346 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/column_names_enumeration.py
--rw-r--r--   0        0        0      265 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/datetime_format_enumeration.py
--rw-r--r--   0        0        0     1024 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/parameter_enumeration.py
--rw-r--r--   0        0        0     1723 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/period_type_enumeration.py
--rw-r--r--   0        0        0      376 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/enumerations/time_resolution_enumeration.py
--rw-r--r--   0        0        0      401 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/exceptions.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/file_path_handling/__init__.py
--rw-r--r--   0        0        0     2744 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/file_path_handling/file_list_creation.py
--rw-r--r--   0        0        0     3597 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/file_path_handling/path_handling.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/indexing/__init__.py
--rw-r--r--   0        0        0     5651 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/indexing/file_index_creation.py
--rw-r--r--   0        0        0    11576 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/indexing/meta_index_creation.py
--rw-r--r--   0        0        0     9344 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/mosmix.py
--rw-r--r--   0        0        0       86 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/pandas/__init__.py
--rw-r--r--   0        0        0     8706 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/pandas/io.py
--rw-r--r--   0        0        0     4924 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/pandas/wd.py
--rw-r--r--   0        0        0     2334 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/parse_metadata.py
--rw-r--r--   0        0        0        0 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/parsing_data/__init__.py
--rw-r--r--   0        0        0     4558 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/parsing_data/parse_data_from_files.py
--rw-r--r--   0        0        0      267 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/run.py
--rw-r--r--   0        0        0     5031 2020-09-24 22:31:54.158142 wetterdienst-0.8.0/wetterdienst/service.py
--rw-r--r--   0        0        0     7853 2020-09-24 22:35:15.210258 wetterdienst-0.8.0/setup.py
--rw-r--r--   0        0        0     9385 2020-09-24 22:35:15.211136 wetterdienst-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4121 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1123 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/LICENSE.rst
+-rw-r--r--   0        0        0     1123 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/LICENSE.rst
+-rw-r--r--   0        0        0     5347 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/README.rst
+-rw-r--r--   0        0        0     5569 2020-10-09 18:40:17.093996 wetterdienst-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      811 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/__init__.py
+-rw-r--r--   0        0        0    15631 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/cli.py
+-rw-r--r--   0        0        0       79 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/__init__.py
+-rw-r--r--   0        0        0     2457 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/index.py
+-rw-r--r--   0        0        0      227 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/__init__.py
+-rw-r--r--   0        0        0     2512 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_map.py
+-rw-r--r--   0        0        0    23344 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_names.py
+-rw-r--r--   0        0        0     7800 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_types.py
+-rw-r--r--   0        0        0      902 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/constants.py
+-rw-r--r--   0        0        0      265 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/datetime.py
+-rw-r--r--   0        0        0     4724 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/parameter.py
+-rw-r--r--   0        0        0     1723 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/period_type.py
+-rw-r--r--   0        0        0      939 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/time_resolution.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/__init__.py
+-rw-r--r--   0        0        0     5566 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/access.py
+-rw-r--r--   0        0        0     3916 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/api.py
+-rw-r--r--   0        0        0     1080 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/network.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/__init__.py
+-rw-r--r--   0        0        0     5539 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/access.py
+-rw-r--r--   0        0        0    18455 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/api.py
+-rw-r--r--   0        0        0     2708 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/fields.py
+-rw-r--r--   0        0        0     3176 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/fileindex.py
+-rw-r--r--   0        0        0    11418 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/metaindex.py
+-rw-r--r--   0        0        0     4328 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/parser.py
+-rw-r--r--   0        0        0    10122 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/stations.py
+-rw-r--r--   0        0        0     3975 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/store.py
+-rw-r--r--   0        0        0     6612 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/pandas.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/__init__.py
+-rw-r--r--   0        0        0    12583 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/access.py
+-rw-r--r--   0        0        0     9914 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/api.py
+-rw-r--r--   0        0        0      989 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/cli.py
+-rw-r--r--   0        0        0     9611 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/index.py
+-rw-r--r--   0        0        0     3451 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/metadata.py
+-rw-r--r--   0        0        0     6742 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/sites.py
+-rw-r--r--   0        0        0     1445 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/util.py
+-rw-r--r--   0        0        0     6004 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/util.py
+-rw-r--r--   0        0        0      362 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/exceptions.py
+-rw-r--r--   0        0        0      259 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/run.py
+-rw-r--r--   0        0        0     5065 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/service.py
+-rw-r--r--   0        0        0       80 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/__init__.py
+-rw-r--r--   0        0        0     1792 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/cache.py
+-rw-r--r--   0        0        0     1246 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/cli.py
+-rw-r--r--   0        0        0      887 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/datetime.py
+-rw-r--r--   0        0        0     1031 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/geo.py
+-rw-r--r--   0        0        0     1218 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/network.py
+-rw-r--r--   0        0        0     8691 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/pandas.py
+-rw-r--r--   0        0        0      371 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/pdf.py
+-rw-r--r--   0        0        0     8082 2020-10-09 18:45:44.075213 wetterdienst-0.9.0/setup.py
+-rw-r--r--   0        0        0     9752 2020-10-09 18:45:44.076029 wetterdienst-0.9.0/PKG-INFO
```

### Comparing `wetterdienst-0.8.0/CHANGELOG.rst` & `wetterdienst-0.9.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 *********
 
 Development
 ===========
 
 ...
 
+0.9.0 (09.10.2020)
+==================
+
+- Large refactoring
+- Make period type in DWDObservationData and cli optional
+- Activate SQL querying again by using DuckDB 0.2.2.dev254. Thanks, @Mytherin!
+- Fix coercion of integers with nans
+- Fix problem with storing IntegerArrays in HDF
+- Rename ``DWDStationRequest`` to ``DWDObservationData``
+- Add ``DWDObservationSites`` API wrapper to acquire station information
+- Move ``discover_climate_observations`` to ``DWDObservationMetadata.discover_parameters``
+- Add PDF-based ``DWDObservationMetadata.describe_fields()``
+- Upgrade Docker images to Python 3.8.6
+- Move intermediate storage of HDF out of data collection
+- Fix bug with date filtering for empty/no station data for a given parameter
+- Radar data: Add non-RADOLAN data acquisition
+
 0.8.0 (25.09.2020)
 ==================
 
 - Add TTL-based persistent caching using dogpile.cache
 - Add ``example/radolan.py`` and adjust documentation
 - Export dataframe to different data sinks like SQLite, DuckDB, InfluxDB and CrateDB
 - Query results with SQL, based on in-memory DuckDB
@@ -43,15 +60,15 @@
 
 - add RADOLAN support
 - change module and function naming in accordance with RADOLAN
 
 0.4.0 (03.08.2020)
 ==================
 
-- extend DWDStationRequest to take multiple parameters as request
+- extend DWDObservationData to take multiple parameters as request
 - add documentation at readthedocs.io
 - [cli] Adjust methods to work with multiple parameters
 
 0.3.0 (26.07.2020)
 ==================
 
 - establish code style black
```

### Comparing `wetterdienst-0.8.0/LICENSE.rst` & `wetterdienst-0.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `wetterdienst-0.8.0/README.rst` & `wetterdienst-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -36,42 +36,45 @@
 
 While our long-term goal is to provide access to multiple weather services,
 we are still stuck with the German Weather Service (DWD). Contributions are
 always welcome!
 
 This program and its repository tries to use modern Python technologies
 all over the place. The library is based on Pandas across the board,
-uses Poetry for package administration and GitHub actions for
+uses Poetry for package administration and GitHub Actions for
 all things CI.
 
 
 Features
 ********
 
 Coverage
 ========
 The library currently covers
 
-- historical weather data from ground stations
-- RADOLAN fitted radar data for areal precipitation
-- MOSMIX statistical optimized scalar forecasts extracted from weather models
+- Weather observation data.
+  Both historical and recent.
+- Radar data.
+  All of composite, radolan, radvor, sites and radolan_cdc.
+- MOSMIX statistical optimized scalar forecasts extracted from weather models.
+  Both MOSMIX-L and MOSMIX-S is supported.
 
 To get better insight on which data we have currently made available, with this library
 take a look at `data coverage`_.
 
 
 Details
 =======
 - Get metadata for a set of Parameter, PeriodType and TimeResolution.
 - Get station(s) nearby a selected location.
 - Store/recover collected data.
 - Command line interface.
 - Run SQL queries on the results.
 - Export results to databases and other data sinks.
-- Public Docker image on ghcr.io.
+- Public Docker image.
 
 
 Setup
 *****
 Run this to make ``wetterdienst`` available in your current environment:
 
 .. code-block:: bash
@@ -80,30 +83,29 @@
 
 Synopsis
 ********
 Get historical data for specific stations, using Python:
 
 .. code-block:: python
 
-    from wetterdienst import DWDStationRequest, Parameter, PeriodType, TimeResolution
+    from wetterdienst import DWDObservationData, Parameter, PeriodType, TimeResolution
 
-    request = DWDStationRequest(
+    observations = DWDObservationData(
         station_ids=[1048,4411],
         parameter=[Parameter.CLIMATE_SUMMARY, Parameter.SOLAR],
         time_resolution=TimeResolution.DAILY,
         start_date="1990-01-01",
         end_date="2020-01-01",
         tidy_data=True,
         humanize_column_names=True,
-        write_file=True,
-        prefer_local=True
     )
 
-    for df in request.collect_data():
-        # analyse the station here
+    # Collect and analyse data here.
+    for df in observations.collect_data():
+        print(df)
 
 Get data for specific stations from the command line:
 
 .. code-block:: bash
 
     # Get list of all stations for daily climate summary data in JSON format
     wetterdienst stations --parameter=kl --resolution=daily --period=recent
```

### Comparing `wetterdienst-0.8.0/pyproject.toml` & `wetterdienst-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "wetterdienst"
-version = "0.8.0"
+version = "0.9.0"
 description = "Open weather data for humans"
 authors = [
     "Benjamin Gutzmann <gutzemann@gmail.com>",
     "Daniel Lassahn <daniel.lassahn@meteointelligence.de>",
     "Andreas Motl <andreas.motl@panodata.org>"
 ]
 license = "MIT"
 readme = "README.rst"
 include = [
     "LICENSE.rst",
     "CHANGELOG.rst",
-    "CODE_OF_CONDUCT.rst",
-    "DWD_FILE_SERVER_STRUCTURE.md"
+    "CODE_OF_CONDUCT.rst"
 ]
 homepage = "https://wetterdienst.readthedocs.io/"
 repository = "https://github.com/earthobservations/wetterdienst"
 keywords = [
     "dwd",
     "deutscher wetterdienst",
     "german weather service",
@@ -77,14 +76,17 @@
 beautifulsoup4 = "^4.9.1"
 requests = "^2.24.0"
 python-dateutil = "^2.8.0"
 "dogpile.cache" = "^1.0.2"
 appdirs = "^1.4.4"
 lxml = "^4.5.2"
 tqdm = "^4.47.0"
+PyPDF2 = "^1.26.0"
+tabulate = "^0.8.7"
+deprecation = "^2.1.0"
 
 # Conditionally installed for backward compatibility with older Python versions
 importlib_metadata              = {version = "1.7.0", python = "<3.8"}
 dataclasses                     = {version = "0.7", python = "^3.6,<3.7"}
 
 # Optional dependencies aka. "extras"
 ipython                         = { version = "^7.10.1", optional = true }
@@ -94,23 +96,27 @@
 
 sphinx                          = { version = "^3.2.1", optional = true }
 sphinx-material                 = { version = "^0.0.30", optional = true }
 sphinx-autodoc-typehints        = { version = "1.11.0", optional = true }
 sphinxcontrib-svg2pdfconverter  = { version = "1.1.0", optional = true }
 tomlkit                         = { version = "0.7.0", optional = true }
 
-duckdb                          = { version = "^0.2.1", optional = true }
+duckdb                          = { version = "^0.2.2.dev254", optional = true }
 influxdb                        = { version = "^5.3.0", optional = true }
 crate                           = { version = "^0.25.0", optional = true, extras = ["sqlalchemy"] }
 mysqlclient                     = { version = "^2.0.1", optional = true }
-psycopg2                        = { version = "^2.8.6", optional = true }
+psycopg2-binary                 = { version = "^2.8.6", optional = true }
 
 fastapi                         = { version = "^0.61.1", optional = true }
 uvicorn                         = { version = "^0.11.8", optional = true }
 
+wradlib                         = { version = "^1.8.0", optional = true }
+pybufrkit                       = { version = "^0.2.17", optional = true }
+
+
 [tool.poetry.extras]
 ipython = ["ipython", "ipython-genutils", "matplotlib"]
 excel = ["openpyxl"]
 docs = [
     "sphinx",
     "sphinx-material",
     "tomlkit",
@@ -121,15 +127,17 @@
 ]
 http = ["fastapi", "uvicorn"]
 sql = ["duckdb"]
 duckdb = ["duckdb"]
 influxdb = ["influxdb"]
 cratedb = ["crate"]
 mysql = ["mysqlclient"]
-postgresql = ["psycopg2"]
+postgresql = ["psycopg2-binary"]
+radar = ["wradlib", "pybufrkit"]
+bufr = ["pybufrkit"]
 
 [tool.poetry.dev-dependencies]
 nox = "^2020.8.22"
 black = "^20.8b1"
 flake8 = "^3.8.3"
 flake8-black = "^0.2.1"
 flake8-bugbear = "^20.1.4"
@@ -139,14 +147,37 @@
 pytest-cov = "^2.10.1"
 pytest-notebook = "^0.6.1"
 pytest-dictsdiff = "^0.5.8"
 nbconvert = ">=5.0, <6.0"
 mock = "^4.0.2"
 surrogate = "^0.1"
 matplotlib = "^3.3.2"
+pybufrkit = "^0.2.17"
+# wradlib = "^1.8.0"
 
 [tool.poetry.scripts]
 wetterdienst = 'wetterdienst.cli:run'
+wddump = 'wetterdienst.dwd.radar.cli:wddump'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
+
+[tool.pytest.ini_options]
+markers = [
+    "remote: Tests accessing the internet.",
+    "slow: Slow tests.",
+    "sql: All tests related to SQL."
+]
+
+[tool.coverage.run]
+branch = true
+source = ["wetterdienst"]
+
+[tool.coverage.report]
+show_missing = true
+fail_under = 0
+omit =[
+    "tests/*",
+    "noxfile.py",
+    "wetterdienst/dwd/radar/cli.py",
+]
```

### Comparing `wetterdienst-0.8.0/wetterdienst/additionals/cache.py` & `wetterdienst-0.9.0/wetterdienst/util/cache.py`

 * *Files identical despite different names*

### Comparing `wetterdienst-0.8.0/wetterdienst/additionals/util.py` & `wetterdienst-0.9.0/wetterdienst/util/cli.py`

 * *Files identical despite different names*

### Comparing `wetterdienst-0.8.0/wetterdienst/api.py` & `wetterdienst-0.9.0/wetterdienst/dwd/radar/access.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,339 +1,357 @@
+import bz2
+import gzip
 import logging
-from io import BytesIO
-from pathlib import Path
-from typing import List, Union, Generator, Optional, Tuple
+import tarfile
+from dataclasses import dataclass
 from datetime import datetime
+from io import BytesIO
+from typing import Optional, Generator
 
 import pandas as pd
-from pandas import Timestamp
-import dateparser
 
-from wetterdienst.data_collection import (
-    collect_climate_observations_data,
-    collect_radolan_data,
+from wetterdienst import TimeResolution, PeriodType
+from wetterdienst.dwd.metadata.constants import ArchiveFormat
+
+from wetterdienst.dwd.network import download_file_from_dwd
+from wetterdienst.dwd.radar.index import (
+    create_fileindex_radolan_cdc,
+    create_fileindex_radar,
 )
-from wetterdienst.enumerations.parameter_enumeration import Parameter
-from wetterdienst.enumerations.period_type_enumeration import PeriodType
-from wetterdienst.enumerations.time_resolution_enumeration import TimeResolution
-from wetterdienst.additionals.functions import (
-    parse_enumeration_from_template,
+from wetterdienst.dwd.radar.util import get_date_from_filename
+from wetterdienst.dwd.radar.metadata import (
+    RadarParameter,
+    RadarDate,
+    RadarDataFormat,
+    RadarDataSubset,
 )
-from wetterdienst.exceptions import InvalidParameterCombination, StartDateEndDateError
-from wetterdienst.constants.metadata import DWD_FOLDER_MAIN
-from wetterdienst.enumerations.column_names_enumeration import DWDMetaColumns
-from wetterdienst.indexing.file_index_creation import (
-    create_file_index_for_radolan,
+from wetterdienst.dwd.radar.sites import RadarSite
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.metadata.datetime import DatetimeFormat
+from wetterdienst.util.cache import (
+    payload_cache_twelve_hours,
+    payload_cache_five_minutes,
 )
 
+
 log = logging.getLogger(__name__)
 
 
-class DWDStationRequest:
+@dataclass
+class RadarResult:
     """
-    The DWDStationRequest class represents a request for station data as provided by the
-    DWD service
+    Result object encapsulating radar data and metadata.
+    Currently, this will relate to exactly one radar data file.
     """
 
-    def __init__(
-        self,
-        station_ids: Union[str, int, List[Union[int, str]]],
-        parameter: Union[str, Parameter, List[Union[str, Parameter]]],
-        time_resolution: Union[str, TimeResolution],
-        period_type: Union[
-            Union[None, str, PeriodType], List[Union[None, str, PeriodType]]
-        ] = None,
-        start_date: Union[None, str, Timestamp] = None,
-        end_date: Union[None, str, Timestamp] = None,
-        prefer_local: bool = False,
-        write_file: bool = False,
-        folder: Union[str, Path] = DWD_FOLDER_MAIN,
-        tidy_data: bool = True,
-        humanize_column_names: bool = False,
-    ) -> None:
+    data: BytesIO
+    timestamp: datetime = None
+    url: str = None
+    filename: str = None
+
+    def __getitem__(self, index):
         """
-        Class with mostly flexible arguments to define a request regarding DWD data.
-        Special handling for period type. If start_date/end_date are given all period
-        types are considered and merged together and the data is filtered for the given
-        dates afterwards.
-
-        :param station_ids: definition of stations by str, int or list of str/int,
-                            will be parsed to list of int
-        :param parameter:           Observation measure
-        :param time_resolution:     Frequency/granularity of measurement interval
-        :param period_type:         Recent or historical files
-        :param start_date:          Replacement for period type to define exact time
-                                    of requested data
-        :param end_date:            Replacement for period type to define exact time
-                                    of requested data
-        :param prefer_local:        Definition if data should rather be taken from a
-                                    local source
-        :param write_file:          Should data be written to a local file
-        :param folder:              Place where file lists (and station data) are stored
-        :param tidy_data:           Reshape DataFrame to a more tidy
-                                    and row-based version of data
-        :param humanize_column_names: Replace column names by more meaningful ones
+        Backward compatibility to address this instance as a tuple.
+
+        Formerly, this returned a tuple of ``(datetime, BytesIO)``.
+
+        :param index:
+        :return:
         """
+        if index == 0:  # pragma: no cover
+            return self.timestamp
+        elif index == 1:
+            return self.data
+        else:  # pragma: no cover
+            raise KeyError(f"Index {index} undefined on RadarResult")
+
+
+def collect_radar_data(
+    parameter: RadarParameter,
+    time_resolution: Optional[TimeResolution] = None,
+    period_type: Optional[PeriodType] = None,
+    site: Optional[RadarSite] = None,
+    format: Optional[RadarDataFormat] = None,
+    subset: Optional[RadarDataSubset] = None,
+    elevation: Optional[int] = None,
+    start_date: Optional[datetime] = None,
+    end_date: Optional[datetime] = None,
+) -> RadarResult:
+    """
+    Collect radar data for given parameters.
 
-        if not (period_type or start_date or end_date):
-            raise ValueError(
-                "Define either a 'time_resolution' or one of or both 'start_date' and "
-                "'end_date' and leave 'time_resolution' empty!"
-            )
+    :param parameter:       The radar moment to request
+    :param site:            Site/station if parameter is one of
+                            RADAR_PARAMETERS_SITES
+    :param format:          Data format (BINARY, BUFR, HDF5)
+    :param subset:          The subset (simple or polarimetric) for HDF5 data.
+    :param start_date:      Start date
+    :param end_date:        End date
+    :param time_resolution: Time resolution for RadarParameter.RADOLAN_CDC,
+                            either daily or hourly or 5 minutes.
+    :param period_type:     Period type for RadarParameter.RADOLAN_CDC
 
-        try:
-            self.station_ids = pd.Series(station_ids).astype(int).tolist()
-        except ValueError:
-            raise ValueError("List of station id's can not be parsed to integers.")
-
-        self.parameter = (
-            pd.Series(parameter)
-            .apply(parse_enumeration_from_template, args=(Parameter,))
-            .tolist()
-        )
+    :return:                ``RadarResult`` item
+    """
+
+    # Find latest file.
+    if start_date == RadarDate.LATEST:
 
-        self.time_resolution = parse_enumeration_from_template(
-            time_resolution, TimeResolution
+        file_index = create_fileindex_radar(
+            parameter=parameter,
+            site=site,
+            format=format,
+            parse_datetime=False,
         )
 
-        # start date and end date required for collect_data in any case
-        self.start_date = None
-        self.end_date = None
-
-        if period_type:
-            # For the case that a period_type is given, parse the period type(s)
-            self.period_type = (
-                pd.Series(period_type)
-                .apply(parse_enumeration_from_template, args=(PeriodType,))
-                .sort_values()
-                .tolist()
-            )
-        else:
-            # working with ranges of data means expecting data to be laying between
-            # periods, thus including all periods
-            self.period_type = [
-                PeriodType.HISTORICAL,
-                PeriodType.RECENT,
-                PeriodType.NOW,
-            ]
+        # Find "-latest-" file.
+        filenames = file_index["FILENAME"].tolist()
+        latest_file = list(filter(lambda x: "-latest-" in x, filenames))[0]
 
-            # If only one date given, make the other one equal
-            if not start_date:
-                start_date = end_date
-
-            if not end_date:
-                end_date = start_date
-
-            self.start_date = Timestamp(dateparser.parse(start_date))
-            self.end_date = Timestamp(dateparser.parse(end_date))
-
-            if not self.start_date <= self.end_date:
-                raise StartDateEndDateError(
-                    "Error: 'start_date' must be smaller or equal to 'end_date'."
-                )
+        # Yield single "RadarResult" item.
+        result = next(_download_generic_data(url=latest_file))
+        yield result
 
-        self.prefer_local = prefer_local
-        self.write_file = write_file
-        self.folder = folder
-        # If more then one parameter requested, automatically tidy data
-        self.tidy_data = len(self.parameter) == 2 or tidy_data
-        self.humanize_column_names = humanize_column_names
-
-    def __eq__(self, other):
-        return [
-            self.station_ids,
-            self.parameter,
-            self.time_resolution,
-            self.period_type,
-            self.start_date,
-            self.end_date,
-        ] == other
-
-    def __str__(self):
-        station_ids_joined = "& ".join(
-            [str(station_id) for station_id in self.station_ids]
-        )
-        return ", ".join(
-            [
-                f"station_ids {station_ids_joined}",
-                "& ".join([parameter.value for parameter in self.parameter]),
-                self.time_resolution.value,
-                "& ".join([period_type.value for period_type in self.period_type]),
-                self.start_date.value,
-                self.end_date.value,
-            ]
-        )
+    else:
 
-    def collect_data(self) -> Generator[pd.DataFrame, None, None]:
-        """
-        Method to collect data for a defined request. The function is build as generator
-        in order to not cloak the memory thus if the user wants the data as one pandas
-        DataFrame the generator has to be casted to a DataFrame manually via
-        pd.concat(list(request.collect_data()).
+        if parameter == RadarParameter.RADOLAN_CDC:
 
-        :return: A generator yielding a pandas.DataFrame per station.
-        """
-        for station_id in self.station_ids:
-            df_station = pd.DataFrame()
+            if period_type:
+                period_types = [period_type]
+            else:
+                period_types = [PeriodType.RECENT, PeriodType.HISTORICAL]
 
-            for parameter in self.parameter:
-                df_parameter_period = pd.DataFrame()
+            results = []
+            for period_type in period_types:
+
+                file_index = create_fileindex_radolan_cdc(
+                    time_resolution=time_resolution, period_type=period_type
+                )
 
-                for period_type in self.period_type:
-                    try:
-                        df_period = collect_climate_observations_data(
-                            station_ids=[station_id],
-                            parameter=parameter,
-                            time_resolution=self.time_resolution,
-                            period_type=period_type,
-                            folder=self.folder,
-                            prefer_local=self.prefer_local,
-                            write_file=self.write_file,
-                            tidy_data=self.tidy_data,
-                            humanize_column_names=self.humanize_column_names,
+                # Filter for dates range if start_date and end_date are defined.
+                if period_type == PeriodType.RECENT:
+                    file_index = file_index[
+                        (file_index[DWDMetaColumns.DATETIME.value] >= start_date)
+                        & (file_index[DWDMetaColumns.DATETIME.value] < end_date)
+                    ]
+
+                # This is for matching historical data, e.g. "RW-200509.tar.gz".
+                else:
+                    file_index = file_index[
+                        (
+                            file_index[DWDMetaColumns.DATETIME.value].dt.year
+                            == start_date.year
                         )
-                    except InvalidParameterCombination:
-                        log.info(
-                            f"Combination for "
-                            f"{parameter.value}/"
-                            f"{self.time_resolution.value}/"
-                            f"{period_type} does not exist and is skipped."
+                        & (
+                            file_index[DWDMetaColumns.DATETIME.value].dt.month
+                            == start_date.month
                         )
+                    ]
 
-                        continue
+                results.append(file_index)
 
-                    # Filter out values which already are in the DataFrame
-                    try:
-                        df_period = df_period[
-                            ~df_period[DWDMetaColumns.DATE.value].isin(
-                                df_parameter_period[DWDMetaColumns.DATE.value]
-                            )
-                        ]
-                    except KeyError:
-                        pass
+            file_index = pd.concat(results)
 
-                    df_parameter_period = df_parameter_period.append(
-                        df_period, ignore_index=True
-                    )
+            if file_index.empty:
+                # TODO: Extend this log message.
+                log.warning(f"No radar file found for {parameter}, {site}, {format}")
+                return
+
+            # Iterate list of files and yield "RadarResult" items.
+            for _, row in file_index.iterrows():
+                url = row[DWDMetaColumns.FILENAME.value]
+                yield download_radolan_data(start_date, url)
 
-                df_station = df_station.append(df_parameter_period, ignore_index=True)
+        else:
+            file_index = create_fileindex_radar(
+                parameter=parameter,
+                site=site,
+                format=format,
+                subset=subset,
+                parse_datetime=True,
+            )
 
-            # Filter for dates range if start_date and end_date are defined
-            if self.start_date:
-                df_station = df_station[
-                    (df_station[DWDMetaColumns.DATE.value] >= self.start_date)
-                    & (df_station[DWDMetaColumns.DATE.value] <= self.end_date)
+            # Filter for dates range if start_date and end_date are defined.
+            file_index = file_index[
+                (file_index[DWDMetaColumns.DATETIME.value] >= start_date)
+                & (file_index[DWDMetaColumns.DATETIME.value] < end_date)
+            ]
+
+            # Filter SWEEP_VOL_VELOCITY_H and SWEEP_VOL_REFLECTIVITY_H by elevation.
+            if elevation is not None:
+                filename = file_index[DWDMetaColumns.FILENAME.value]
+                file_index = file_index[
+                    (filename.str.contains(f"vradh_{elevation:02d}"))
+                    | (filename.str.contains(f"sweep_vol_v_{elevation}"))
+                    | (filename.str.contains(f"dbzh_{elevation:02d}"))
+                    | (filename.str.contains(f"sweep_vol_z_{elevation}"))
                 ]
 
-            # Empty dataframe should be skipped
-            if df_station.empty:
-                continue
+            if file_index.empty:
+                log.warning(f"No radar file found for {parameter}, {site}, {format}")
+                return
+
+            # Iterate list of files and yield "RadarResult" items.
+            for _, row in file_index.iterrows():
+                date_time = row[DWDMetaColumns.DATETIME.value]
+                url = row[DWDMetaColumns.FILENAME.value]
+
+                for result in _download_generic_data(url=url):
+                    if result.timestamp is None:
+                        result.timestamp = date_time
+                    yield result
 
-            yield df_station
 
-    def collect_safe(self):
-        """
-        Collect all data from ``DWDStationRequest``.
-        """
+def should_cache_download(*args, **kwargs) -> bool:  # pragma: no cover
+    """
+    Determine whether this specific result should be cached.
 
-        data = list(self.collect_data())
+    Here, we don't want to cache any files containing "-latest-" in their filenames.
+
+    :param args: Arguments of decorated function.
+    :param kwargs: Keyword arguments of decorated function.
+    :return: When cache should be dimissed, return False. Otherwise, return True.
+    """
+    url = args[0]
+    if "-latest-" in url:
+        return False
+    return True
 
-        if not data:
-            raise ValueError("No data available for given constraints")
 
-        return pd.concat(data)
+@payload_cache_five_minutes.cache_on_arguments(should_cache_fn=should_cache_download)
+def _download_generic_data_cached(url: str) -> BytesIO:
+    return url, download_file_from_dwd(url)
 
 
-class DWDRadolanRequest:
+def _download_generic_data(url: str) -> Generator[RadarResult, None, None]:
     """
-    API for DWD RADOLAN data requests.
+    Download radar data.
+
+    :param url:         The URL to the file on the DWD server
+
+    :return:            The file in binary, either an archive of one file
+                        or an archive of multiple files.
     """
 
-    def __init__(
-        self,
-        time_resolution: Union[str, TimeResolution],
-        date_times: Optional[Union[str, List[Union[str, datetime]]]] = None,
-        start_date: Optional[Union[str, datetime]] = None,
-        end_date: Optional[Union[str, datetime]] = None,
-        prefer_local: bool = False,
-        write_file: bool = False,
-        folder: Union[str, Path] = DWD_FOLDER_MAIN,
-    ) -> None:
-        """
+    _, data = _download_generic_data_cached(url)
 
-        :param time_resolution: Time resolution enumeration, either hourly or daily
-        :param date_times:      List of datetimes for which RADOLAN is requested.
-                                Minutes have o be defined (HOUR:50), otherwise rounded
-                                to 50 minutes as of its provision.
-        :param start_date:      Alternative to datetimes, giving a start and end date
-        :param end_date:        Alternative to datetimes, giving a start and end date
-        :param prefer_local:    RADOLAN should rather be loaded from disk, for
-                                processing purposes
-        :param write_file:      File should be stored on drive
-        :param folder:          Folder where to store RADOLAN data
+    data.seek(0)
 
-        :return:                Nothing for now.
-        """
-        time_resolution = parse_enumeration_from_template(
-            time_resolution, TimeResolution
-        )
+    # RadarParameter.FX_REFLECTIVITY
+    if url.endswith(ArchiveFormat.TAR_BZ2.value):
+        with bz2.BZ2File(data, mode="rb") as archive:
+            with tarfile.open(fileobj=archive) as tar_file:
+                for file in tar_file.getmembers():
+                    yield RadarResult(
+                        data=BytesIO(tar_file.extractfile(file).read()),
+                        timestamp=get_date_from_filename(file.name),
+                        filename=file.name,
+                    )
 
-        if time_resolution not in (TimeResolution.HOURLY, TimeResolution.DAILY):
-            raise ValueError("RADOLAN only supports hourly and daily resolution.")
+    # RadarParameter.WN_REFLECTIVITY, RADAR_PARAMETERS_SWEEPS (BUFR)
+    elif url.endswith(ArchiveFormat.BZ2.value):
+        with bz2.BZ2File(data, mode="rb") as archive:
+            data = BytesIO(archive.read())
+            yield RadarResult(url=url, data=data, timestamp=get_date_from_filename(url))
+
+    # RADAR_PARAMETERS_RADVOR
+    elif url.endswith(ArchiveFormat.GZ.value):
+        with gzip.GzipFile(fileobj=data, mode="rb") as archive:
+            data = BytesIO(archive.read())
+            yield RadarResult(url=url, data=data, timestamp=get_date_from_filename(url))
+
+    else:
+        yield RadarResult(url=url, data=data, timestamp=get_date_from_filename(url))
+
+
+def download_radolan_data(
+    date_time: datetime,
+    url: str,
+) -> RadarResult:
+    """
+    Function used to download RADOLAN_CDC data for a given datetime. The function calls
+    a separate download function that is cached for reuse which is especially used for
+    historical data that comes packaged for multiple time steps within a single archive.
+
+    :param date_time:   The datetime for the requested RADOLAN file.
+                        This is required for the recognition of the returned binary,
+                        which has no obvious name tag.
+
+    :param url:         The URL to the file that has the data
+                        for the requested datetime, either an archive of multiple files
+                        for a datetime in historical time or an archive with one file
+                        for the recent RADOLAN file
 
-        self.time_resolution = time_resolution
+    :return:            ``RadarResult`` item
+    """
+    archive_in_bytes = _download_radolan_data(url)
 
-        if date_times == "latest":
-            file_index_radolan = create_file_index_for_radolan(time_resolution)
+    result = _extract_radolan_data(date_time, archive_in_bytes)
+    result.url = url
 
-            self.date_times = pd.Series(
-                file_index_radolan[DWDMetaColumns.DATETIME.value][-1:]
-            )
-        elif date_times:
-            self.date_times = pd.Series(
-                pd.to_datetime(date_times, infer_datetime_format=True)
-            )
-        else:
-            self.date_times = pd.Series(
-                pd.date_range(
-                    pd.to_datetime(start_date, infer_datetime_format=True),
-                    pd.to_datetime(end_date, infer_datetime_format=True),
-                )
-            )
+    return result
 
-        self.date_times = self.date_times.dt.floor(freq="H") + pd.Timedelta(minutes=50)
 
-        self.date_times = self.date_times.drop_duplicates().sort_values()
+@payload_cache_twelve_hours.cache_on_arguments()
+def _download_radolan_data(remote_radolan_filepath: str) -> BytesIO:
+    """
+    Function (cached) that downloads the RADOLAN_CDC file.
 
-        self.prefer_local = prefer_local
-        self.write_file = write_file
-        self.folder = folder
-
-    def __eq__(self, other):
-        return (
-            self.time_resolution == other.time_resolution
-            and self.date_times.values.tolist() == other.date_times.values.tolist()
-        )
+    Args:
+        remote_radolan_filepath: the file path to the file on the DWD server
 
-    def __str__(self):
-        return ", ".join(
-            [
-                self.time_resolution.value,
-                "& ".join([str(date_time) for date_time in self.date_times]),
-            ]
-        )
+    Returns:
+        the file in binary, either an archive of one file or an archive of multiple
+        files
+    """
+    return download_file_from_dwd(remote_radolan_filepath)
 
-    def collect_data(self) -> Generator[Tuple[datetime, BytesIO], None, None]:
-        """
-        Function used to get the data for the request returned as generator.
 
-        :return: For each datetime, the same datetime and file in bytes
-        """
-        for date_time in self.date_times:
-            _, file_in_bytes = collect_radolan_data(
-                time_resolution=self.time_resolution,
-                date_times=[date_time],
-                write_file=self.write_file,
-                folder=self.folder,
-            )[0]
+def _extract_radolan_data(
+    date_time: datetime, archive_in_bytes: BytesIO
+) -> RadarResult:
+    """
+    Function used to extract RADOLAN_CDC file for the requested datetime
+    from the downloaded archive.
 
-            yield date_time, file_in_bytes
+    Args:
+        date_time: requested datetime of RADOLAN
+        archive_in_bytes: downloaded archive of RADOLAN file
+
+    Returns:
+        the datetime formatted as string and the RADOLAN file for the datetime
+    """
+    # Need string of datetime to check if one of the files in the archive contains
+    # the requested datetime
+    date_time_string = date_time.strftime(DatetimeFormat.ymdhm.value)
+
+    # First try to unpack archive from archive (case for historical data)
+    try:
+        # Have to seek(0) as the archive might be reused
+        archive_in_bytes.seek(0)
+
+        with gzip.GzipFile(fileobj=archive_in_bytes, mode="rb") as gz_file:
+            file_in_archive = BytesIO(gz_file.read())
+
+            with tarfile.open(fileobj=file_in_archive) as tar_file:
+                for file in tar_file.getmembers():
+                    if date_time_string in file.name:
+                        return RadarResult(
+                            data=BytesIO(tar_file.extractfile(file).read()),
+                            timestamp=date_time,
+                            filename=file.name,
+                        )
+
+                raise FileNotFoundError(
+                    f"RADOLAN file for {date_time_string} not found."
+                )  # pragma: no cover
+
+    # Otherwise if there's an error the data is from recent time period and only has to
+    # be unpacked once
+    except tarfile.ReadError:
+        # Seek again for reused purpose
+        archive_in_bytes.seek(0)
+
+        with gzip.GzipFile(fileobj=archive_in_bytes, mode="rb") as gz_file:
+            return RadarResult(
+                data=BytesIO(gz_file.read()), timestamp=date_time, filename=gz_file.name
+            )
```

### Comparing `wetterdienst-0.8.0/wetterdienst/cli.py` & `wetterdienst-0.9.0/wetterdienst/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 # -*- coding: utf-8 -*-
+import json
 import sys
 import logging
 from datetime import datetime, timedelta
 
 from docopt import docopt
 from munch import Munch
 import pandas as pd
 
-from wetterdienst import (
-    __appname__,
-    __version__,
-    metadata_for_climate_observations,
-    get_nearby_stations_by_number,
-    get_nearby_stations_by_distance,
-    discover_climate_observations,
+from wetterdienst import __appname__, __version__
+from wetterdienst.dwd.observations.store import StorageAdapter
+from wetterdienst.util.cli import normalize_options, setup_logging, read_list
+from wetterdienst.dwd.observations.api import (
+    DWDObservationData,
+    DWDObservationSites,
+    DWDObservationMetadata,
 )
-from wetterdienst.additionals.util import normalize_options, setup_logging, read_list
-from wetterdienst.api import DWDStationRequest
-from wetterdienst.enumerations.parameter_enumeration import Parameter
-from wetterdienst.enumerations.period_type_enumeration import PeriodType
-from wetterdienst.enumerations.time_resolution_enumeration import TimeResolution
+from wetterdienst.dwd.metadata import Parameter, TimeResolution, PeriodType
 
 log = logging.getLogger(__name__)
 
 
 def run():
     """
     Usage:
-      wetterdienst stations --parameter=<parameter> --resolution=<resolution> --period=<period> [--station=] [--latitude=] [--longitude=] [--number=] [--distance=] [--persist] [--sql=] [--format=<format>]
-      wetterdienst readings --parameter=<parameter> --resolution=<resolution> --period=<period> --station=<station> [--persist] [--date=<date>] [--sql=] [--format=<format>] [--target=<target>]
-      wetterdienst readings --parameter=<parameter> --resolution=<resolution> --period=<period> --latitude= --longitude= [--number=] [--distance=] [--persist] [--date=<date>] [--sql=] [--format=<format>] [--target=<target>]
+      wetterdienst dwd stations --parameter=<parameter> --resolution=<resolution> --period=<period> [--station=<station>] [--latitude=<latitude>] [--longitude=<longitude>] [--number=<number>] [--distance=<distance>] [--persist] [--sql=<sql>] [--format=<format>]
+      wetterdienst dwd readings --parameter=<parameter> --resolution=<resolution> --station=<station> [--period=<period>] [--persist] [--date=<date>] [--sql=<sql>] [--format=<format>] [--target=<target>]
+      wetterdienst dwd readings --parameter=<parameter> --resolution=<resolution> --latitude=<latitude> --longitude=<longitude> [--period=<period>] [--number=<number>] [--distance=<distance>] [--persist] [--date=<date>] [--sql=<sql>] [--format=<format>] [--target=<target>]
+      wetterdienst dwd about [parameters] [resolutions] [periods]
+      wetterdienst dwd about coverage [--parameter=<parameter>] [--resolution=<resolution>] [--period=<period>]
       wetterdienst service [--listen=<listen>]
-      wetterdienst about [parameters] [resolutions] [periods]
-      wetterdienst about coverage [--parameter=<parameter>] [--resolution=<resolution>] [--period=<period>]
       wetterdienst --version
       wetterdienst (-h | --help)
 
     Options:
       --parameter=<parameter>       Parameter/variable, e.g. "kl", "air_temperature", "precipitation", etc.
       --resolution=<resolution>     Dataset resolution: "annual", "monthly", "daily", "hourly", "minute_10", "minute_1"
       --period=<period>             Dataset period: "historical", "recent", "now"
@@ -56,120 +53,120 @@
       --listen=<listen>             HTTP server listen address. [Default: localhost:7890]
       -h --help                     Show this screen
 
 
     Examples requesting stations:
 
       # Get list of all stations for daily climate summary data in JSON format
-      wetterdienst stations --parameter=kl --resolution=daily --period=recent
+      wetterdienst dwd stations --parameter=kl --resolution=daily --period=recent
 
       # Get list of all stations in CSV format
-      wetterdienst stations --parameter=kl --resolution=daily --period=recent --format=csv
+      wetterdienst dwd stations --parameter=kl --resolution=daily --period=recent --format=csv
 
       # Get list of specific stations
-      wetterdienst stations --resolution=daily --parameter=kl --period=recent --station=1,1048,4411
+      wetterdienst dwd stations --resolution=daily --parameter=kl --period=recent --station=1,1048,4411
 
       # Get list of specific stations in GeoJSON format
-      wetterdienst stations --resolution=daily --parameter=kl --period=recent --station=1,1048,4411 --format=geojson
+      wetterdienst dwd stations --resolution=daily --parameter=kl --period=recent --station=1,1048,4411 --format=geojson
 
     Examples requesting readings:
 
       # Get daily climate summary data for specific stations
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent
 
       # Optionally save/restore to/from disk in order to avoid asking upstream servers each time
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --persist
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --persist
 
       # Limit output to specific date
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --date=2020-05-01
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --date=2020-05-01
 
       # Limit output to specified date range in ISO-8601 time interval format
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --date=2020-05-01/2020-05-05
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --date=2020-05-01/2020-05-05
 
       # The real power horse: Acquire data across historical+recent data sets
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=historical,recent --date=1969-01-01/2020-06-11
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=historical,recent --date=1969-01-01/2020-06-11
 
       # Acquire monthly data for 2020-05
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=monthly --period=recent,historical --date=2020-05
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=monthly --period=recent,historical --date=2020-05
 
       # Acquire monthly data from 2017-01 to 2019-12
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=monthly --period=recent,historical --date=2017-01/2019-12
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=monthly --period=recent,historical --date=2017-01/2019-12
 
       # Acquire annual data for 2019
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=annual --period=recent,historical --date=2019
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=annual --period=recent,historical --date=2019
 
       # Acquire annual data from 2010 to 2020
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=annual --period=recent,historical --date=2010/2020
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=annual --period=recent,historical --date=2010/2020
 
       # Acquire hourly data
-      wetterdienst readings --station=1048,4411 --parameter=air_temperature --resolution=hourly --period=recent --date=2020-06-15T12
+      wetterdienst dwd readings --station=1048,4411 --parameter=air_temperature --resolution=hourly --period=recent --date=2020-06-15T12
 
     Examples using geospatial features:
 
       # Acquire stations and readings by geoposition, request specific number of nearby stations.
-      wetterdienst stations --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --num=5
-      wetterdienst readings --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --num=5 --date=2020-06-30
+      wetterdienst dwd stations --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --num=5
+      wetterdienst dwd readings --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --num=5 --date=2020-06-30
 
       # Acquire stations and readings by geoposition, request stations within specific radius.
-      wetterdienst stations --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --distance=25
-      wetterdienst readings --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --distance=25 --date=2020-06-30
+      wetterdienst dwd stations --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --distance=25
+      wetterdienst dwd readings --resolution=daily --parameter=kl --period=recent --lat=49.9195 --lon=8.9671 --distance=25 --date=2020-06-30
 
     Examples using SQL filtering:
 
       # Find stations by state.
-      wetterdienst stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE state='Sachsen'"
+      wetterdienst dwd stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE state='Sachsen'"
 
       # Find stations by name (LIKE query).
-      wetterdienst stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE lower(station_name) LIKE lower('%dresden%')"
+      wetterdienst dwd stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE lower(station_name) LIKE lower('%dresden%')"
 
       # Find stations by name (regexp query).
-      wetterdienst stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE regexp_matches(lower(station_name), lower('.*dresden.*'))"
+      wetterdienst dwd stations --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE regexp_matches(lower(station_name), lower('.*dresden.*'))"
 
       # Filter measurements: Display daily climate observation readings where the maximum temperature is below two degrees.
-      wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE element='temperature_air_max_200' AND value < 2.0;"
+      wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent --sql="SELECT * FROM data WHERE element='temperature_air_max_200' AND value < 2.0;"
 
     Examples for inquiring metadata:
 
       # Display list of available parameters (air_temperature, precipitation, pressure, ...)
-      wetterdienst about parameters
+      wetterdienst dwd about parameters
 
       # Display list of available resolutions (10_minutes, hourly, daily, ...)
-      wetterdienst about resolutions
+      wetterdienst dwd about resolutions
 
       # Display list of available periods (historical, recent, now)
-      wetterdienst about periods
+      wetterdienst dwd about periods
 
       # Display coverage/correlation between parameters, resolutions and periods.
       # This can answer questions like ...
-      wetterdienst about coverage
+      wetterdienst dwd about coverage
 
       # Tell me all periods and resolutions available for 'air_temperature'.
-      wetterdienst about coverage --parameter=air_temperature
+      wetterdienst dwd about coverage --parameter=air_temperature
 
       # Tell me all parameters available for 'daily' resolution.
-      wetterdienst about coverage --resolution=daily
+      wetterdienst dwd about coverage --resolution=daily
 
     Examples for exporting data to databases:
 
       # Shortcut command for fetching readings from DWD
-      alias fetch="wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent"
+      alias fetch="wetterdienst dwd readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent"
 
       # Store readings to DuckDB
       fetch --target="duckdb://database=dwd.duckdb&table=weather"
 
       # Store readings to InfluxDB
       fetch --target="influxdb://localhost/?database=dwd&table=weather"
 
       # Store readings to CrateDB
       fetch --target="crate://localhost/?database=dwd&table=weather"
 
     Run as HTTP service:
 
-      wetterdienst service
-      wetterdienst service --listen=0.0.0.0:9999
+      wetterdienst dwd service
+      wetterdienst dwd service --listen=0.0.0.0:9999
 
     """
 
     appname = f"{__appname__} {__version__}"
 
     # Read command line options.
     options = normalize_options(docopt(run.__doc__, version=appname))
@@ -200,19 +197,19 @@
     if options.readings and options.format == "geojson":
         raise KeyError("GeoJSON format only available for stations output")
 
     df = None
 
     # Acquire station list.
     if options.stations:
-        df = metadata_for_climate_observations(
+        df = DWDObservationSites(
             parameter=options.parameter,
             time_resolution=options.resolution,
             period_type=options.period,
-        )
+        ).all()
 
         if options.station:
             station_ids = read_list(options.station)
             df = df[df.STATION_ID.isin(station_ids)]
 
         elif options.latitude and options.longitude:
             df = get_nearby(options)
@@ -232,60 +229,61 @@
         elif options.latitude and options.longitude:
             df = get_nearby(options)
             station_ids = df.STATION_ID.unique()
 
         else:
             raise KeyError("Either --station or --lat, --lon required")
 
+        storage = StorageAdapter(persist=options.persist)
+
         # Funnel all parameters to the workhorse.
-        request = DWDStationRequest(
+        observations = DWDObservationData(
             station_ids=station_ids,
             parameter=read_list(options.parameter),
             time_resolution=options.resolution,
             period_type=read_list(options.period),
-            write_file=options.persist,
-            prefer_local=options.persist,
+            storage=storage,
             humanize_column_names=True,
             tidy_data=True,
         )
 
         # Collect data and merge together.
         try:
-            df = request.collect_safe()
+            df = observations.collect_safe()
 
         except ValueError as ex:
             log.error(ex)
             sys.exit(1)
 
     # Sanity checks.
     if df is None:
         log.error("No data available")
         sys.exit(1)
 
     # Filter readings by datetime expression.
     if options.readings and options.date:
-        df = df.wd.filter_by_date(options.date, request.time_resolution)
+        df = df.dwd.filter_by_date(options.date, observations.time_resolution)
 
     # Make column names lowercase.
-    df = df.wd.lower()
+    df = df.dwd.lower()
 
     # Apply filtering by SQL.
     if options.sql:
         log.info(f"Filtering with SQL: {options.sql}")
         df = df.io.sql(options.sql)
 
     # Emit to data sink, e.g. write to database.
     if options.target:
         log.info(f"Writing data to target {options.target}")
         df.io.export(options.target)
         return
 
     # Render to output format.
     try:
-        output = df.wd.format(options.format)
+        output = df.dwd.format(options.format)
     except KeyError as ex:
         log.error(
             f'{ex}. Output format must be one of "json", "geojson", "csv", "excel".'
         )
         sys.exit(1)
 
     print(output)
@@ -308,39 +306,43 @@
 
     # Obtain DWIM date range for station liveness.
     # TODO: Obtain from user.
     #   However, some dates will not work and Pandas will croak with:
     #   KeyError: "None of [Int64Index([0, 0, 0, 0, 0], dtype='int64')] are in the [index]"
     # See also https://github.com/earthobservations/wetterdienst/pull/145#discussion_r487698588.
 
-    days500 = datetime.now() + timedelta(days=-500)
-    now = datetime.now() + timedelta(days=-2)
+    days500 = datetime.utcnow() + timedelta(days=-500)
+    now = datetime.utcnow() + timedelta(days=-2)
 
     minimal_date = datetime(days500.year, days500.month, days500.day)
     maximal_date = datetime(now.year, now.month, now.day)
 
     nearby_baseline_args = dict(
-        latitude=float(options.latitude),
-        longitude=float(options.longitude),
-        minimal_available_date=minimal_date,
-        maximal_available_date=maximal_date,
         parameter=options.parameter,
         time_resolution=options.resolution,
         period_type=options.period,
+        start_date=minimal_date,
+        end_date=maximal_date,
     )
 
     if options.latitude and options.longitude:
         if options.number:
-            nearby_stations = get_nearby_stations_by_number(
+            nearby_stations = DWDObservationSites(
                 **nearby_baseline_args,
+            ).nearby_number(
+                latitude=float(options.latitude),
+                longitude=float(options.longitude),
                 num_stations_nearby=int(options.number),
             )
         elif options.distance:
-            nearby_stations = get_nearby_stations_by_distance(
+            nearby_stations = DWDObservationSites(
                 **nearby_baseline_args,
+            ).nearby_radius(
+                latitude=float(options.latitude),
+                longitude=float(options.longitude),
                 max_distance_in_km=int(options.distance),
             )
 
         return nearby_stations
 
     return pd.DataFrame()
 
@@ -368,19 +370,23 @@
     elif options.resolutions:
         output(TimeResolution)
 
     elif options.periods:
         output(PeriodType)
 
     elif options.coverage:
-        print(
-            discover_climate_observations(
+        output = json.dumps(
+            DWDObservationMetadata(
                 time_resolution=options.resolution,
                 parameter=read_list(options.parameter),
                 period_type=read_list(options.period),
-            )
+            ).discover_parameters(),
+            indent=4,
         )
+        print(output)
 
     else:
-        log.error('Please invoke "wetterdienst about" with one of these subcommands:')
+        log.error(
+            'Please invoke "wetterdienst dwd about" with one of these subcommands:'
+        )
         output(["parameters", "resolutions", "periods", "coverage"])
         sys.exit(1)
```

### Comparing `wetterdienst-0.8.0/wetterdienst/data_models/coordinates.py` & `wetterdienst-0.9.0/wetterdienst/util/geo.py`

 * *Files identical despite different names*

### Comparing `wetterdienst-0.8.0/wetterdienst/data_storing.py` & `wetterdienst-0.9.0/wetterdienst/dwd/observations/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,120 @@
-""" Data storing/restoring methods"""
+""" function to read data from dwd server """
+import logging
+from typing import List, Tuple, Union
 from io import BytesIO
-from pathlib import Path
-from typing import Union, Tuple
-from datetime import datetime
-
 import pandas as pd
 
-from wetterdienst.enumerations.parameter_enumeration import Parameter
-from wetterdienst.enumerations.period_type_enumeration import PeriodType
-from wetterdienst.enumerations.time_resolution_enumeration import TimeResolution
-from wetterdienst.file_path_handling.path_handling import (
-    build_local_filepath_for_station_data,
-    build_local_filepath_for_radolan,
+from wetterdienst.dwd.metadata.column_map import GERMAN_TO_ENGLISH_COLUMNS_MAPPING
+from wetterdienst.dwd.metadata.constants import NA_STRING, STATION_DATA_SEP
+from wetterdienst.dwd.metadata.column_names import (
+    DWDOrigMetaColumns,
+    DWDMetaColumns,
+    DWDOrigDataColumns,
 )
+from wetterdienst.dwd.metadata.parameter import Parameter
+from wetterdienst import TimeResolution
+
+log = logging.getLogger(__name__)
 
 
-def store_climate_observations(
-    station_data: pd.DataFrame,
-    station_id: int,
+def parse_climate_observations_data(
+    filenames_and_files: List[Tuple[str, BytesIO]],
     parameter: Parameter,
-    time_resolution: TimeResolution,
-    period_type: PeriodType,
-    folder: Union[str, Path],
-) -> None:
+    time_resolution: Union[TimeResolution, str],
+) -> pd.DataFrame:
     """
-    Function to store data in a local file hdf file. The function takes a pandas
-    DataFrame plus additionally the request parameters to identify data within the
-    hdf file and another folder argument for the place where the file is stored.
-
-    :param station_data:            The pandas DataFrame with the obtained data
-    :param station_id:              The station id of the station to store
-    :param parameter:               Observation measure
-    :param time_resolution:         Frequency/granularity of measurement interval
-    :param period_type:             Recent or historical files
-    :param folder:                  The folder where the hdf is stored
-
-    :return:                        Nothing, only prints information if data was
-                                    not stored.
+    This function is used to read the station data from given bytes object.
+    The filename is required to defined if and where an error happened.
+    Args:
+        filenames_and_files: list of tuples of a filename and its local stored file
+        that should be read
+        parameter: enumeration of parameter used to correctly parse the date field
+        time_resolution: enumeration of time resolution used to correctly parse the
+        date field
+    Returns:
+        pandas.DataFrame with requested data, for different station ids the data is
+        still put into one DataFrame
     """
-    # Make sure that there is data that can be stored
-    if station_data.empty:
-        return
 
-    request_string = _build_local_store_key(
-        station_id, parameter, time_resolution, period_type
-    )
+    time_resolution = TimeResolution(time_resolution)
 
-    local_filepath = build_local_filepath_for_station_data(folder)
+    data = [
+        _parse_climate_observations_data(filename_and_file, parameter, time_resolution)
+        for filename_and_file in filenames_and_files
+    ]
 
-    local_filepath.parent.mkdir(parents=True, exist_ok=True)
+    data = pd.concat(data).reset_index(drop=True)
 
-    station_data.to_hdf(path_or_buf=local_filepath, key=request_string)
+    return data
 
 
-def restore_climate_observations(
-    station_id: int,
+def _parse_climate_observations_data(
+    filename_and_file: Tuple[str, BytesIO],
     parameter: Parameter,
     time_resolution: TimeResolution,
-    period_type: PeriodType,
-    folder: Union[str, Path],
 ) -> pd.DataFrame:
     """
-    Function to restore data from a local hdf file based on the place (folder) where
-    the file is stored and parameters that define the request in particular.
-
-    :param station_id:              Station id of which data should be restored
-    :param parameter:               Observation measure
-    :param time_resolution:         Frequency/granularity of measurement interval
-    :param period_type:             Recent or historical files
-    :param folder:                  The folder where the hdf is stored
-
-    :return:                        All the data.
+    A wrapping function that only handles data for one station id. The files passed to
+    it are thus related to this id. This is important for storing the data locally as
+    the DataFrame that is stored should obviously only handle one station at a time.
+    Args:
+        filename_and_file: the files belonging to one station
+        time_resolution: enumeration of time resolution used to correctly parse the
+        date field
+    Returns:
+        pandas.DataFrame with data from that station, acn be empty if no data is
+        provided or local file is not found or has no data in it
     """
-    request_string = _build_local_store_key(
-        station_id, parameter, time_resolution, period_type
-    )
-
-    local_filepath = build_local_filepath_for_station_data(folder)
+    filename, file = filename_and_file
 
     try:
-        # typing required as pandas.read_hdf returns an object by typing
-        station_data = pd.read_hdf(path_or_buf=local_filepath, key=request_string)
-    except (FileNotFoundError, KeyError):
+        data = pd.read_csv(
+            filepath_or_buffer=BytesIO(
+                file.read().replace(b" ", b"")
+            ),  # prevent leading/trailing whitespace
+            sep=STATION_DATA_SEP,
+            dtype="str",
+            na_values=NA_STRING,
+        )
+    except pd.errors.ParserError:
+        log.warning(
+            f"The file representing {filename} could not be parsed and is skipped."
+        )
+        return pd.DataFrame()
+    except ValueError:
+        log.warning(f"The file representing {filename} is None and is skipped.")
         return pd.DataFrame()
 
-    # Cast to pandas DataFrame
-    station_data = pd.DataFrame(station_data)
-
-    return station_data
-
-
-def _build_local_store_key(
-    station_id: Union[str, int],
-    parameter: Parameter,
-    time_resolution: TimeResolution,
-    period_type: PeriodType,
-) -> str:
-    """
-    Function that builds a request string from defined parameters including a single
-    station id
-
-    :param station_id:              Station id of data
-    :param parameter:               Observation measure
-    :param time_resolution:         Frequency/granularity of measurement interval
-    :param period_type:             Recent or historical files
-
-    :return: A string building a key that is used to identify the request
-    """
-    request_string = (
-        f"{parameter.value}/{time_resolution.value}/"
-        f"{period_type.value}/station_id_{int(station_id)}"
-    )
-
-    return request_string
-
-
-def store_radolan_data(
-    date_time_and_file: Tuple[datetime, BytesIO],
-    time_resolution: TimeResolution,
-    folder: Union[str, Path],
-) -> None:
-
-    date_time, file = date_time_and_file
-
-    filepath = build_local_filepath_for_radolan(date_time, folder, time_resolution)
-
-    filepath.parent.mkdir(parents=True, exist_ok=True)
-
-    with filepath.open("wb") as f:
-        f.write(file.read())
+    # Column names contain spaces, so strip them away.
+    data = data.rename(columns=str.strip)
 
-    # When the file has been written, reset seek pointer.
-    file.seek(0)
+    # Make column names uppercase.
+    data = data.rename(columns=str.upper)
 
+    # End of record (EOR) has no value, so drop it right away.
+    data = data.drop(columns=DWDMetaColumns.EOR.value, errors="ignore")
 
-def restore_radolan_data(
-    date_time: datetime, time_resolution: TimeResolution, folder: Union[str, Path]
-) -> BytesIO:
-    filepath = build_local_filepath_for_radolan(date_time, folder, time_resolution)
+    # Special handling for hourly solar data, as it has more date columns
+    if time_resolution == TimeResolution.HOURLY and parameter == Parameter.SOLAR:
+        # Rename date column correctly to end of interval, as it has additional minute
+        # information. Also rename column with true local time to english one
+        data = data.rename(
+            columns={
+                "MESS_DATUM_WOZ": DWDOrigDataColumns.HOURLY.SOLAR.TRUE_LOCAL_TIME.value,
+            }
+        )
+
+        # Duplicate the date column to end of interval column
+        data[DWDOrigDataColumns.HOURLY.SOLAR.END_OF_INTERVAL.value] = data[
+            DWDOrigMetaColumns.DATE.value
+        ]
+
+        # Fix real date column by cutting of minutes
+        data[DWDOrigMetaColumns.DATE.value] = data[DWDOrigMetaColumns.DATE.value].str[
+            :-3
+        ]
 
-    with filepath.open("rb") as f:
-        file_in_bytes = BytesIO(f.read())
+    # Assign meaningful column names (baseline).
+    data = data.rename(columns=GERMAN_TO_ENGLISH_COLUMNS_MAPPING)
 
-    return file_in_bytes
+    return data
```

### Comparing `wetterdienst-0.8.0/wetterdienst/enumerations/column_names_enumeration.py` & `wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from enum import Enum
 
 
+# https://stackoverflow.com/questions/33727217/subscriptable-objects-in-class
+class _GetAttrMeta(type):
+    def __getitem__(cls, x):
+        return getattr(cls, x)
+
+
 class DWDOrigMetaColumns(Enum):
     """ Original meta column names from DWD data """
 
     STATION_ID = "STATIONS_ID"
     DATE = "MESS_DATUM"
     FROM_DATE = "VON_DATUM"
     TO_DATE = "BIS_DATUM"
@@ -45,20 +51,14 @@
     # Columns used for RADOLAN
     PERIOD_TYPE = "PERIOD_TYPE"
     DATETIME = "DATETIME"
     # Column for distance used by get_nearby_stations_...
     DISTANCE_TO_LOCATION = "DISTANCE_TO_LOCATION"
 
 
-# https://stackoverflow.com/questions/33727217/subscriptable-objects-in-class
-class _GetAttrMeta(type):
-    def __getitem__(cls, x):
-        return getattr(cls, x)
-
-
 class _DWDDataColumnBase(metaclass=_GetAttrMeta):
     pass
 
 
 class DWDOrigDataColumns(_DWDDataColumnBase):
     """
     Original data column names from DWD data
@@ -75,15 +75,15 @@
             QN = "QN"
             RS_01 = "RS_01"
             RTH_01 = "RTH_01"
             RWH_01 = "RWH_01"
             RS_IND_01 = "RS_IND_01"  # int
 
     # 10_minutes
-    class MINUTES_10(_DWDDataColumnBase):  # noqa
+    class MINUTE_10(_DWDDataColumnBase):  # noqa
         # air_temperature
         class TEMPERATURE_AIR(Enum):  # noqa
             QN = "QN"
             PP_10 = "PP_10"
             TT_10 = "TT_10"
             TM5_10 = "TM5_10"
             RF_10 = "RF_10"
@@ -431,15 +431,15 @@
             QN = "QUALITY"
             RS_01 = "PRECIPITATION_HEIGHT"
             RTH_01 = "PRECIPITATION_HEIGHT_DROPLET"
             RWH_01 = "PRECIPITATION_HEIGHT_ROCKER"
             RS_IND_01 = "PRECIPITATION_FORM"  # int
 
     # 10_minutes
-    class MINUTES_10(_DWDDataColumnBase):  # noqa
+    class MINUTE_10(_DWDDataColumnBase):  # noqa
         # air_temperature
         class TEMPERATURE_AIR(Enum):  # noqa
             QN = "QUALITY"
             PP_10 = "PRESSURE_AIR_STATION_HEIGHT"
             TT_10 = "TEMPERATURE_AIR_200"
             TM5_10 = "TEMPERATURE_AIR_005"
             RF_10 = "HUMIDITY"
```

### Comparing `wetterdienst-0.8.0/wetterdienst/enumerations/period_type_enumeration.py` & `wetterdienst-0.9.0/wetterdienst/dwd/metadata/period_type.py`

 * *Files identical despite different names*

### Comparing `wetterdienst-0.8.0/wetterdienst/file_path_handling/file_list_creation.py` & `wetterdienst-0.9.0/wetterdienst/dwd/index.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,71 @@
-""" file list creation for requested files """
-from typing import Union, List
-from datetime import datetime
-
-from wetterdienst.enumerations.column_names_enumeration import DWDMetaColumns
-from wetterdienst.enumerations.parameter_enumeration import Parameter
-from wetterdienst.enumerations.period_type_enumeration import PeriodType
-from wetterdienst.enumerations.time_resolution_enumeration import TimeResolution
-from wetterdienst.indexing.file_index_creation import (
-    create_file_index_for_climate_observations,
-    create_file_index_for_radolan,
+from functools import reduce
+from urllib.parse import urljoin
+
+import pandas as pd
+
+from wetterdienst import Parameter, TimeResolution, PeriodType
+from wetterdienst.dwd.metadata.constants import DWDCDCBase, DWD_SERVER, DWD_CDC_PATH
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.util.cache import (
+    fileindex_cache_five_minutes,
+    fileindex_cache_one_hour,
 )
+from wetterdienst.util.network import list_remote_files
 
 
-def create_file_list_for_climate_observations(
-    station_ids: List[int],
-    parameter: Union[Parameter, str],
-    time_resolution: Union[TimeResolution, str],
-    period_type: Union[PeriodType, str],
-) -> List[str]:
+def _create_file_index_for_dwd_server(
+    parameter: Parameter,
+    time_resolution: TimeResolution,
+    period_type: PeriodType,
+    cdc_base: DWDCDCBase,
+) -> pd.DataFrame:
     """
-    Function for selecting datafiles (links to archives) for given
-    station_ids, parameter, time_resolution and period_type under consideration of a
-    created list of files that are
-    available online.
+    Function to create a file index of the DWD station data, which usually is shipped as
+    zipped/archived data. The file index is created for an individual set of parameters.
     Args:
-        station_ids: ids for the weather station to ask for data
-        parameter: observation measure
-        time_resolution: frequency/granularity of measurement interval
-        period_type: recent or historical files
+        parameter: parameter of Parameter enumeration
+        time_resolution: time resolution of TimeResolution enumeration
+        period_type: period type of PeriodType enumeration
+        cdc_base: base path e.g. climate_observations/germany
     Returns:
-        List of path's to file
+        file index in a pandas.DataFrame with sets of parameters and station id
     """
+    parameter_path = build_path_to_parameter(parameter, time_resolution, period_type)
+
+    url = reduce(urljoin, [DWD_SERVER, DWD_CDC_PATH, cdc_base.value, parameter_path])
 
-    parameter = Parameter(parameter)
-    time_resolution = TimeResolution(time_resolution)
-    period_type = PeriodType(period_type)
+    files_server = list_remote_files(url, recursive=True)
 
-    file_index = create_file_index_for_climate_observations(
-        parameter, time_resolution, period_type
+    files_server = pd.DataFrame(
+        files_server, columns=[DWDMetaColumns.FILENAME.value], dtype="str"
     )
 
-    file_index = file_index[
-        file_index[DWDMetaColumns.STATION_ID.value].isin(station_ids)
-    ]
+    return files_server
+
 
-    return file_index[DWDMetaColumns.FILENAME.value].values.tolist()
+def reset_file_index_cache() -> None:
+    """ Function to reset the cached file index for all kinds of parameters """
+    fileindex_cache_five_minutes.invalidate()
+    fileindex_cache_one_hour.invalidate()
 
 
-def create_filepath_for_radolan(
-    date_time: datetime, time_resolution: TimeResolution
+def build_path_to_parameter(
+    parameter: Parameter, time_resolution: TimeResolution, period_type: PeriodType
 ) -> str:
     """
-    Function used to create a relative filepath for a requested datetime depending on
-    the file index for the relevant time resolution.
-
+    Function to build a indexing file path
     Args:
-        date_time: datetime for requested RADOLAN file
-        time_resolution: time resolution enumeration of the request
+        parameter: observation measure
+        time_resolution: frequency/granularity of measurement interval
+        period_type: recent or historical files
 
     Returns:
-        a string, either empty if non found or with the relative path to the file
+        indexing file path relative to climate observations path
     """
-    file_index = create_file_index_for_radolan(time_resolution)
-
-    if date_time in file_index[DWDMetaColumns.DATETIME.value].tolist():
-        file_index = file_index[file_index[DWDMetaColumns.DATETIME.value] == date_time]
-    else:
-        file_index = file_index[
-            (file_index[DWDMetaColumns.DATETIME.value].dt.year == date_time.year)
-            & (file_index[DWDMetaColumns.DATETIME.value].dt.month == date_time.month)
-        ]
-
-    if file_index.empty:
-        return ""
+    if parameter == Parameter.SOLAR and time_resolution in (
+        TimeResolution.HOURLY,
+        TimeResolution.DAILY,
+    ):
+        return f"{time_resolution.value}/{parameter.value}/"
 
-    return f"{file_index[DWDMetaColumns.FILENAME.value].item()}"
+    return f"{time_resolution.value}/{parameter.value}/{period_type.value}/"
```

### Comparing `wetterdienst-0.8.0/wetterdienst/indexing/meta_index_creation.py` & `wetterdienst-0.9.0/wetterdienst/dwd/observations/metaindex.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,39 +6,35 @@
 from concurrent.futures import ThreadPoolExecutor
 import datetime as dt
 from urllib.parse import urljoin
 
 import pandas as pd
 from requests.exceptions import InvalidURL
 
-from wetterdienst.additionals.cache import metaindex_cache
-from wetterdienst.constants.access_credentials import (
+from wetterdienst.util.cache import metaindex_cache
+from wetterdienst.dwd.metadata.constants import (
     DWDCDCBase,
     DWD_SERVER,
     DWD_CDC_PATH,
+    STATION_ID_REGEX,
+    NA_STRING,
+    STATION_DATA_SEP,
 )
-from wetterdienst.constants.column_name_mapping import (
+from wetterdienst.dwd.metadata.column_map import (
     GERMAN_TO_ENGLISH_COLUMNS_MAPPING,
     METADATA_DTYPE_MAPPING,
 )
-from wetterdienst.constants.metadata import (
-    STATION_ID_REGEX,
-    STATION_DATA_SEP,
-    NA_STRING,
-)
-from wetterdienst.download.download_services import download_file_from_dwd
-from wetterdienst.enumerations.column_names_enumeration import DWDMetaColumns
-from wetterdienst.enumerations.parameter_enumeration import Parameter
-from wetterdienst.enumerations.period_type_enumeration import PeriodType
-from wetterdienst.enumerations.time_resolution_enumeration import TimeResolution
+from wetterdienst.dwd.network import download_file_from_dwd
+from wetterdienst.dwd.index import build_path_to_parameter
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.metadata.parameter import Parameter
+from wetterdienst.dwd.metadata.period_type import PeriodType
+from wetterdienst import TimeResolution
 from wetterdienst.exceptions import MetaFileNotFound
-from wetterdienst.file_path_handling.path_handling import (
-    build_path_to_parameter,
-    list_remote_files,
-)
+from wetterdienst.util.network import list_remote_files
 
 METADATA_COLUMNS = [
     DWDMetaColumns.STATION_ID.value,
     DWDMetaColumns.FROM_DATE.value,
     DWDMetaColumns.TO_DATE.value,
     DWDMetaColumns.STATION_HEIGHT.value,
     DWDMetaColumns.LATITUDE.value,
```

### Comparing `wetterdienst-0.8.0/wetterdienst/pandas/io.py` & `wetterdienst-0.9.0/wetterdienst/util/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 acquired through the core machinery.
 
 Extending pandas
 ================
 - https://pandas.pydata.org/pandas-docs/stable/development/extending.html
 """
 import logging
-from urllib.parse import urlparse, parse_qs
 import pandas as pd
+from urllib.parse import urlparse, parse_qs
 
 
 log = logging.getLogger(__name__)
 
 
 @pd.api.extensions.register_dataframe_accessor("io")
 class IoAccessor:
@@ -40,33 +40,33 @@
         """
         import duckdb
 
         df = duckdb.query(self.df, "data", sql).df()
         self.df = df
         return df
 
-    def format(self, format: str) -> str:
+    def format(self, fmt: str) -> str:
         """
         Format/render Pandas DataFrame to given output format.
 
-        :param format: One of json, geojson, csv, excel.
+        :param fmt: One of json, geojson, csv, excel.
         :return: Rendered payload.
         """
 
         # Output as JSON.
-        if format == "json":
+        if fmt == "json":
             output = self.df.to_json(orient="records", date_format="iso", indent=4)
 
         # Output as CSV.
-        elif format == "csv":
+        elif fmt == "csv":
             output = self.df.to_csv(index=False, date_format="%Y-%m-%dT%H-%M-%S")
 
         # Output as XLSX.
         # FIXME: Make --format=excel write to a designated file.
-        elif format == "excel":
+        elif fmt == "excel":
             # TODO: Obtain output file name from command line.
             output_filename = "output.xlsx"
             log.info(f"Writing {output_filename}")
             self.df.to_excel(output_filename, index=False)
             output = None
 
         else:
```

### Comparing `wetterdienst-0.8.0/wetterdienst/pandas/wd.py` & `wetterdienst-0.9.0/wetterdienst/dwd/pandas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 # Extending pandas
 # https://pandas.pydata.org/pandas-docs/stable/development/extending.html
 import json
 
 import pandas as pd
 
-from wetterdienst import TimeResolution
-from wetterdienst.additionals.time_handling import parse_datetime, mktimerange
-from wetterdienst.enumerations.column_names_enumeration import DWDMetaColumns
+from wetterdienst.dwd.metadata import TimeResolution
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.util import parse_datetime, mktimerange
+
+
+POSSIBLE_ID_VARS = (
+    DWDMetaColumns.STATION_ID.value,
+    DWDMetaColumns.DATE.value,
+    DWDMetaColumns.FROM_DATE.value,
+    DWDMetaColumns.TO_DATE.value,
+)
+
+POSSIBLE_DATE_VARS = (
+    DWDMetaColumns.DATE.value,
+    DWDMetaColumns.FROM_DATE.value,
+    DWDMetaColumns.TO_DATE.value,
+)
 
 
-@pd.api.extensions.register_dataframe_accessor("wd")
-class WetterdienstAccessor:
+@pd.api.extensions.register_dataframe_accessor("dwd")
+class PandasDwdExtension:
     def __init__(self, pandas_obj):
         self.df = pandas_obj
 
-    def lower(self):
+    def lower(self) -> pd.DataFrame:
         """
         Make Pandas DataFrame column names and parameters lowercase.
 
         :return: Mungled DataFrame
         """
         df = self.df.rename(columns=str.lower)
 
@@ -82,28 +96,28 @@
                 )
             else:
                 expression = date == self.df[DWDMetaColumns.DATE.value]
             df = self.df[expression]
 
         return df
 
-    def format(self, format: str) -> str:
+    def format(self, fmt: str) -> str:
         """
         Format/render Pandas DataFrame to given output format.
 
-        :param format: One of json, geojson, csv, excel.
+        :param fmt: One of json, geojson, csv, excel.
         :return: Rendered payload.
         """
 
         # Output as GeoJSON.
-        if format == "geojson":
-            output = json.dumps(self.df.wd.to_geojson(), indent=4)
+        if fmt == "geojson":
+            output = json.dumps(self.df.dwd.to_geojson(), indent=4)
 
         else:
-            output = self.df.io.format(format=format)
+            output = self.df.io.format(fmt=fmt)
 
         return output
 
     def to_geojson(self) -> dict:
         """
         Convert DWD station information into GeoJSON format.
 
@@ -143,7 +157,49 @@
                 }
             )
 
         return {
             "type": "FeatureCollection",
             "features": features,
         }
+
+    def tidy_up_data(self) -> pd.DataFrame:
+        """
+        Function to create a tidy DataFrame by reshaping it, putting quality in a
+        separate column, so that for each timestamp there is a tuple of parameter, value
+        and quality.
+
+        :return:            The tidied DataFrame
+        """
+        id_vars = []
+        date_vars = []
+
+        # Add id columns based on metadata columns
+        for column in POSSIBLE_ID_VARS:
+            if column in self.df:
+                id_vars.append(column)
+                if column in POSSIBLE_DATE_VARS:
+                    date_vars.append(column)
+
+        # Extract quality
+        # Set empty quality for first columns until first QN column
+        quality = pd.Series(dtype=pd.Int64Dtype())
+        column_quality = pd.Series(dtype=pd.Int64Dtype())
+
+        for column in self.df:
+            # If is quality column, overwrite current "column quality"
+            if column.startswith("QN"):
+                column_quality = self.df.pop(column)
+            else:
+                quality = quality.append(column_quality)
+
+        df_tidy = self.df.melt(
+            id_vars=id_vars,
+            var_name=DWDMetaColumns.ELEMENT.value,
+            value_name=DWDMetaColumns.VALUE.value,
+        )
+
+        df_tidy[DWDMetaColumns.QUALITY.value] = quality.reset_index(drop=True).astype(
+            pd.Int64Dtype()
+        )
+
+        return df_tidy
```

### Comparing `wetterdienst-0.8.0/wetterdienst/service.py` & `wetterdienst-0.9.0/wetterdienst/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
 
 from fastapi import FastAPI, Query, HTTPException
 from fastapi.responses import HTMLResponse, PlainTextResponse
 
-from wetterdienst import __appname__, __version__
-from wetterdienst import PeriodType, Parameter, TimeResolution
-from wetterdienst import metadata_for_climate_observations, DWDStationRequest
-from wetterdienst.additionals.functions import parse_enumeration_from_template
-from wetterdienst.additionals.util import read_list
+from wetterdienst import (
+    __appname__,
+    __version__,
+    TimeResolution,
+)
+from wetterdienst import PeriodType, Parameter
+from wetterdienst import DWDObservationData
+from wetterdienst.dwd.observations.api import DWDObservationSites
+from wetterdienst.dwd.util import parse_enumeration_from_template
+from wetterdienst.util.cli import read_list
 
 app = FastAPI(debug=False)
 
 log = logging.getLogger(__name__)
 
 dwd_source = "https://opendata.dwd.de/climate_environment/CDC/"
 dwd_copyright = "© Deutscher Wetterdienst (DWD), Climate Data Center (CDC)"
@@ -71,22 +76,22 @@
 ):
 
     parameter = parse_enumeration_from_template(parameter, Parameter)
     resolution = parse_enumeration_from_template(resolution, TimeResolution)
     period = parse_enumeration_from_template(period, PeriodType)
 
     # Data acquisition.
-    df = metadata_for_climate_observations(
+    df = DWDObservationSites(
         parameter=parameter,
         time_resolution=resolution,
         period_type=period,
-    )
+    ).all()
 
     # Postprocessing.
-    df = df.wd.lower()
+    df = df.dwd.lower()
 
     if sql is not None:
         df = df.io.sql(sql)
 
     return make_json_response(df.io.to_dict())
 
 
@@ -127,30 +132,30 @@
 
     station_ids = map(int, read_list(station))
     parameter = parse_enumeration_from_template(parameter, Parameter)
     resolution = parse_enumeration_from_template(resolution, TimeResolution)
     period = parse_enumeration_from_template(period, PeriodType)
 
     # Data acquisition.
-    request = DWDStationRequest(
+    observations = DWDObservationData(
         station_ids=station_ids,
         parameter=parameter,
         time_resolution=resolution,
         period_type=period,
         tidy_data=True,
         humanize_column_names=True,
     )
 
     # Postprocessing.
-    df = request.collect_safe()
+    df = observations.collect_safe()
 
     if date is not None:
-        df = df.wd.filter_by_date(date, resolution)
+        df = df.dwd.filter_by_date(date, resolution)
 
-    df = df.wd.lower()
+    df = df.dwd.lower()
 
     if sql is not None:
         df = df.io.sql(sql)
 
     data = json.loads(df.to_json(orient="records", date_format="iso"))
     return make_json_response(data)
```

### Comparing `wetterdienst-0.8.0/setup.py` & `wetterdienst-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['wetterdienst',
- 'wetterdienst.additionals',
- 'wetterdienst.constants',
- 'wetterdienst.data_models',
- 'wetterdienst.download',
- 'wetterdienst.enumerations',
- 'wetterdienst.file_path_handling',
- 'wetterdienst.indexing',
- 'wetterdienst.pandas',
- 'wetterdienst.parsing_data']
+ 'wetterdienst.dwd',
+ 'wetterdienst.dwd.metadata',
+ 'wetterdienst.dwd.mosmix',
+ 'wetterdienst.dwd.observations',
+ 'wetterdienst.dwd.radar',
+ 'wetterdienst.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['appdirs>=1.4.4,<2.0.0',
+['PyPDF2>=1.26.0,<2.0.0',
+ 'appdirs>=1.4.4,<2.0.0',
  'beautifulsoup4>=4.9.1,<5.0.0',
  'cachetools>=4.1.1,<5.0.0',
  'dateparser>=0.7.6,<0.8.0',
+ 'deprecation>=2.1.0,<3.0.0',
  'docopt>=0.6.2,<0.7.0',
  'dogpile.cache>=1.0.2,<2.0.0',
  'fire>=0.3.1,<0.4.0',
  'h5py>=2.10.0,<3.0.0',
  'lxml>=4.5.2,<5.0.0',
  'munch>=2.5.0,<3.0.0',
  'numpy>=1.19.2,<2.0.0',
  'pandas>=1.1.2,<2.0.0',
  'python-dateutil>=2.8.0,<3.0.0',
  'requests>=2.24.0,<3.0.0',
  'scipy>=1.5.2,<2.0.0',
  'tables>=3.6.1,<4.0.0',
+ 'tabulate>=0.8.7,<0.9.0',
  'tqdm>=4.47.0,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata==1.7.0'],
  ':python_version >= "3.6" and python_version < "3.7"': ['dataclasses==0.7'],
+ 'bufr': ['pybufrkit>=0.2.17,<0.3.0'],
  'cratedb': ['crate[sqlalchemy]>=0.25.0,<0.26.0'],
  'docs': ['ipython>=7.10.1,<8.0.0',
           'matplotlib>=3.3.2,<4.0.0',
           'sphinx>=3.2.1,<4.0.0',
           'sphinx-material>=0.0.30,<0.0.31',
           'sphinx-autodoc-typehints==1.11.0',
           'sphinxcontrib-svg2pdfconverter==1.1.0',
           'tomlkit==0.7.0'],
- 'duckdb': ['duckdb>=0.2.1,<0.3.0'],
+ 'duckdb': ['duckdb>=0.2.2.dev254,<0.3.0'],
  'excel': ['openpyxl>=3.0.5,<4.0.0'],
  'http': ['fastapi>=0.61.1,<0.62.0', 'uvicorn>=0.11.8,<0.12.0'],
  'influxdb': ['influxdb>=5.3.0,<6.0.0'],
  'ipython': ['ipython>=7.10.1,<8.0.0',
              'ipython-genutils>=0.2.0,<0.3.0',
              'matplotlib>=3.3.2,<4.0.0'],
  'mysql': ['mysqlclient>=2.0.1,<3.0.0'],
- 'postgresql': ['psycopg2>=2.8.6,<3.0.0'],
- 'sql': ['duckdb>=0.2.1,<0.3.0']}
+ 'postgresql': ['psycopg2-binary>=2.8.6,<3.0.0'],
+ 'radar': ['wradlib>=1.8.0,<2.0.0', 'pybufrkit>=0.2.17,<0.3.0'],
+ 'sql': ['duckdb>=0.2.2.dev254,<0.3.0']}
 
 entry_points = \
-{'console_scripts': ['wetterdienst = wetterdienst.cli:run']}
+{'console_scripts': ['wddump = wetterdienst.dwd.radar.cli:wddump',
+                     'wetterdienst = wetterdienst.cli:run']}
 
 setup_kwargs = {
     'name': 'wetterdienst',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Open weather data for humans',
-    'long_description': '###########################################\nWetterdienst - Open weather data for humans\n###########################################\n\n.. image:: https://github.com/earthobservations/wetterdienst/workflows/Tests/badge.svg\n   :target: https://github.com/earthobservations/wetterdienst/actions?workflow=Tests\n.. image:: https://codecov.io/gh/earthobservations/wetterdienst/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/earthobservations/wetterdienst\n.. image:: https://readthedocs.org/projects/wetterdienst/badge/?version=latest\n   :target: https://wetterdienst.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/pypi/pyversions/wetterdienst.svg\n   :target: https://pypi.python.org/pypi/wetterdienst/\n.. image:: https://img.shields.io/pypi/v/wetterdienst.svg\n   :target: https://pypi.org/project/wetterdienst/\n.. image:: https://img.shields.io/pypi/status/wetterdienst.svg\n   :target: https://pypi.python.org/pypi/wetterdienst/\n.. image:: https://pepy.tech/badge/wetterdienst/month\n   :target: https://pepy.tech/project/wetterdienst/month\n.. image:: https://img.shields.io/github/license/earthobservations/wetterdienst\n   :target: https://github.com/earthobservations/wetterdienst/blob/master/LICENSE.rst\n.. image:: https://zenodo.org/badge/160953150.svg\n   :target: https://zenodo.org/badge/latestdoi/160953150\n\n\nIntroduction\n************\nWelcome to Wetterdienst, your friendly weather service library for Python.\n\nWe are a group of like-minded people trying to make access to weather data in\nPython feel like a warm summer breeze, similar to other projects like\nrdwd_ for the R language, which originally drew our interest in this project.\n\nWhile our long-term goal is to provide access to multiple weather services,\nwe are still stuck with the German Weather Service (DWD). Contributions are\nalways welcome!\n\nThis program and its repository tries to use modern Python technologies\nall over the place. The library is based on Pandas across the board,\nuses Poetry for package administration and GitHub actions for\nall things CI.\n\n\nFeatures\n********\n\nCoverage\n========\nThe library currently covers\n\n- historical weather data from ground stations\n- RADOLAN fitted radar data for areal precipitation\n- MOSMIX statistical optimized scalar forecasts extracted from weather models\n\nTo get better insight on which data we have currently made available, with this library\ntake a look at `data coverage`_.\n\n\nDetails\n=======\n- Get metadata for a set of Parameter, PeriodType and TimeResolution.\n- Get station(s) nearby a selected location.\n- Store/recover collected data.\n- Command line interface.\n- Run SQL queries on the results.\n- Export results to databases and other data sinks.\n- Public Docker image on ghcr.io.\n\n\nSetup\n*****\nRun this to make ``wetterdienst`` available in your current environment:\n\n.. code-block:: bash\n\n    pip install wetterdienst\n\nSynopsis\n********\nGet historical data for specific stations, using Python:\n\n.. code-block:: python\n\n    from wetterdienst import DWDStationRequest, Parameter, PeriodType, TimeResolution\n\n    request = DWDStationRequest(\n        station_ids=[1048,4411],\n        parameter=[Parameter.CLIMATE_SUMMARY, Parameter.SOLAR],\n        time_resolution=TimeResolution.DAILY,\n        start_date="1990-01-01",\n        end_date="2020-01-01",\n        tidy_data=True,\n        humanize_column_names=True,\n        write_file=True,\n        prefer_local=True\n    )\n\n    for df in request.collect_data():\n        # analyse the station here\n\nGet data for specific stations from the command line:\n\n.. code-block:: bash\n\n    # Get list of all stations for daily climate summary data in JSON format\n    wetterdienst stations --parameter=kl --resolution=daily --period=recent\n\n    # Get daily climate summary data for specific stations\n    wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent\n\n\nDocumentation\n*************\nWe strongly recommend reading the full documentation, which will be updated continuously\nas we make progress with this library:\n\n- https://wetterdienst.readthedocs.io/\n\nFor the whole functionality, check out the `Wetterdienst API`_ section of our\ndocumentation, which will be constantly updated. To stay up to date with the\ndevelopment, take a look at the changelog_. Also, don\'t miss out our examples_.\n\n\nData license\n************\nAlthough the data is specified as being open, the DWD asks you to reference them as\ncopyright owner. Please take a look at the `Open Data Strategy at the DWD`_ and the\n`Official Copyright`_ statements before using the data.\n\n\n.. _rdwd: https://github.com/brry/rdwd\n.. _Wetterdienst API: https://wetterdienst.readthedocs.io/en/latest/pages/api.html\n.. _data coverage: https://wetterdienst.readthedocs.io/en/latest/pages/data_coverage.html\n.. _changelog: https://wetterdienst.readthedocs.io/en/latest/pages/changelog.html\n.. _examples: https://github.com/earthobservations/wetterdienst/tree/master/example\n.. _Open Data Strategy at the DWD: https://www.dwd.de/EN/ourservices/opendata/opendata.html\n.. _Official Copyright: https://www.dwd.de/EN/service/copyright/copyright_artikel.html?nn=495490&lsbId=627548\n',
+    'long_description': '###########################################\nWetterdienst - Open weather data for humans\n###########################################\n\n.. image:: https://github.com/earthobservations/wetterdienst/workflows/Tests/badge.svg\n   :target: https://github.com/earthobservations/wetterdienst/actions?workflow=Tests\n.. image:: https://codecov.io/gh/earthobservations/wetterdienst/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/earthobservations/wetterdienst\n.. image:: https://readthedocs.org/projects/wetterdienst/badge/?version=latest\n   :target: https://wetterdienst.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/pypi/pyversions/wetterdienst.svg\n   :target: https://pypi.python.org/pypi/wetterdienst/\n.. image:: https://img.shields.io/pypi/v/wetterdienst.svg\n   :target: https://pypi.org/project/wetterdienst/\n.. image:: https://img.shields.io/pypi/status/wetterdienst.svg\n   :target: https://pypi.python.org/pypi/wetterdienst/\n.. image:: https://pepy.tech/badge/wetterdienst/month\n   :target: https://pepy.tech/project/wetterdienst/month\n.. image:: https://img.shields.io/github/license/earthobservations/wetterdienst\n   :target: https://github.com/earthobservations/wetterdienst/blob/master/LICENSE.rst\n.. image:: https://zenodo.org/badge/160953150.svg\n   :target: https://zenodo.org/badge/latestdoi/160953150\n\n\nIntroduction\n************\nWelcome to Wetterdienst, your friendly weather service library for Python.\n\nWe are a group of like-minded people trying to make access to weather data in\nPython feel like a warm summer breeze, similar to other projects like\nrdwd_ for the R language, which originally drew our interest in this project.\n\nWhile our long-term goal is to provide access to multiple weather services,\nwe are still stuck with the German Weather Service (DWD). Contributions are\nalways welcome!\n\nThis program and its repository tries to use modern Python technologies\nall over the place. The library is based on Pandas across the board,\nuses Poetry for package administration and GitHub Actions for\nall things CI.\n\n\nFeatures\n********\n\nCoverage\n========\nThe library currently covers\n\n- Weather observation data.\n  Both historical and recent.\n- Radar data.\n  All of composite, radolan, radvor, sites and radolan_cdc.\n- MOSMIX statistical optimized scalar forecasts extracted from weather models.\n  Both MOSMIX-L and MOSMIX-S is supported.\n\nTo get better insight on which data we have currently made available, with this library\ntake a look at `data coverage`_.\n\n\nDetails\n=======\n- Get metadata for a set of Parameter, PeriodType and TimeResolution.\n- Get station(s) nearby a selected location.\n- Store/recover collected data.\n- Command line interface.\n- Run SQL queries on the results.\n- Export results to databases and other data sinks.\n- Public Docker image.\n\n\nSetup\n*****\nRun this to make ``wetterdienst`` available in your current environment:\n\n.. code-block:: bash\n\n    pip install wetterdienst\n\nSynopsis\n********\nGet historical data for specific stations, using Python:\n\n.. code-block:: python\n\n    from wetterdienst import DWDObservationData, Parameter, PeriodType, TimeResolution\n\n    observations = DWDObservationData(\n        station_ids=[1048,4411],\n        parameter=[Parameter.CLIMATE_SUMMARY, Parameter.SOLAR],\n        time_resolution=TimeResolution.DAILY,\n        start_date="1990-01-01",\n        end_date="2020-01-01",\n        tidy_data=True,\n        humanize_column_names=True,\n    )\n\n    # Collect and analyse data here.\n    for df in observations.collect_data():\n        print(df)\n\nGet data for specific stations from the command line:\n\n.. code-block:: bash\n\n    # Get list of all stations for daily climate summary data in JSON format\n    wetterdienst stations --parameter=kl --resolution=daily --period=recent\n\n    # Get daily climate summary data for specific stations\n    wetterdienst readings --station=1048,4411 --parameter=kl --resolution=daily --period=recent\n\n\nDocumentation\n*************\nWe strongly recommend reading the full documentation, which will be updated continuously\nas we make progress with this library:\n\n- https://wetterdienst.readthedocs.io/\n\nFor the whole functionality, check out the `Wetterdienst API`_ section of our\ndocumentation, which will be constantly updated. To stay up to date with the\ndevelopment, take a look at the changelog_. Also, don\'t miss out our examples_.\n\n\nData license\n************\nAlthough the data is specified as being open, the DWD asks you to reference them as\ncopyright owner. Please take a look at the `Open Data Strategy at the DWD`_ and the\n`Official Copyright`_ statements before using the data.\n\n\n.. _rdwd: https://github.com/brry/rdwd\n.. _Wetterdienst API: https://wetterdienst.readthedocs.io/en/latest/pages/api.html\n.. _data coverage: https://wetterdienst.readthedocs.io/en/latest/pages/data_coverage.html\n.. _changelog: https://wetterdienst.readthedocs.io/en/latest/pages/changelog.html\n.. _examples: https://github.com/earthobservations/wetterdienst/tree/master/example\n.. _Open Data Strategy at the DWD: https://www.dwd.de/EN/ourservices/opendata/opendata.html\n.. _Official Copyright: https://www.dwd.de/EN/service/copyright/copyright_artikel.html?nn=495490&lsbId=627548\n',
     'author': 'Benjamin Gutzmann',
     'author_email': 'gutzemann@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://wetterdienst.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wetterdienst-0.8.0/PKG-INFO` & `wetterdienst-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wetterdienst
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open weather data for humans
 Home-page: https://wetterdienst.readthedocs.io/
 License: MIT
 Keywords: dwd,deutscher wetterdienst,german weather service,weather,weather-data,open-data,observations,historical-data,forecasts,radar
 Author: Benjamin Gutzmann
 Author-email: gutzemann@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
@@ -34,59 +34,66 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
+Provides-Extra: bufr
 Provides-Extra: cratedb
 Provides-Extra: docs
 Provides-Extra: duckdb
 Provides-Extra: excel
 Provides-Extra: http
 Provides-Extra: influxdb
 Provides-Extra: ipython
 Provides-Extra: mysql
 Provides-Extra: postgresql
+Provides-Extra: radar
 Provides-Extra: sql
+Requires-Dist: PyPDF2 (>=1.26.0,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: cachetools (>=4.1.1,<5.0.0)
 Requires-Dist: crate[sqlalchemy] (>=0.25.0,<0.26.0); extra == "cratedb"
 Requires-Dist: dataclasses (==0.7); python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: dateparser (>=0.7.6,<0.8.0)
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: dogpile.cache (>=1.0.2,<2.0.0)
-Requires-Dist: duckdb (>=0.2.1,<0.3.0); extra == "sql" or extra == "duckdb"
+Requires-Dist: duckdb (>=0.2.2.dev254,<0.3.0); extra == "sql" or extra == "duckdb"
 Requires-Dist: fastapi (>=0.61.1,<0.62.0); extra == "http"
 Requires-Dist: fire (>=0.3.1,<0.4.0)
 Requires-Dist: h5py (>=2.10.0,<3.0.0)
 Requires-Dist: importlib_metadata (==1.7.0); python_version < "3.8"
 Requires-Dist: influxdb (>=5.3.0,<6.0.0); extra == "influxdb"
 Requires-Dist: ipython (>=7.10.1,<8.0.0); extra == "ipython" or extra == "docs"
 Requires-Dist: ipython-genutils (>=0.2.0,<0.3.0); extra == "ipython"
 Requires-Dist: lxml (>=4.5.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.3.2,<4.0.0); extra == "ipython" or extra == "docs"
 Requires-Dist: munch (>=2.5.0,<3.0.0)
 Requires-Dist: mysqlclient (>=2.0.1,<3.0.0); extra == "mysql"
 Requires-Dist: numpy (>=1.19.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.5,<4.0.0); extra == "excel"
 Requires-Dist: pandas (>=1.1.2,<2.0.0)
-Requires-Dist: psycopg2 (>=2.8.6,<3.0.0); extra == "postgresql"
+Requires-Dist: psycopg2-binary (>=2.8.6,<3.0.0); extra == "postgresql"
+Requires-Dist: pybufrkit (>=0.2.17,<0.3.0); extra == "radar" or extra == "bufr"
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: scipy (>=1.5.2,<2.0.0)
 Requires-Dist: sphinx (>=3.2.1,<4.0.0); extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints (==1.11.0); extra == "docs"
 Requires-Dist: sphinx-material (>=0.0.30,<0.0.31); extra == "docs"
 Requires-Dist: sphinxcontrib-svg2pdfconverter (==1.1.0); extra == "docs"
 Requires-Dist: tables (>=3.6.1,<4.0.0)
+Requires-Dist: tabulate (>=0.8.7,<0.9.0)
 Requires-Dist: tomlkit (==0.7.0); extra == "docs"
 Requires-Dist: tqdm (>=4.47.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.11.8,<0.12.0); extra == "http"
+Requires-Dist: wradlib (>=1.8.0,<2.0.0); extra == "radar"
 Project-URL: Repository, https://github.com/earthobservations/wetterdienst
 Description-Content-Type: text/x-rst
 
 ###########################################
 Wetterdienst - Open weather data for humans
 ###########################################
 
@@ -124,42 +131,45 @@
 
 While our long-term goal is to provide access to multiple weather services,
 we are still stuck with the German Weather Service (DWD). Contributions are
 always welcome!
 
 This program and its repository tries to use modern Python technologies
 all over the place. The library is based on Pandas across the board,
-uses Poetry for package administration and GitHub actions for
+uses Poetry for package administration and GitHub Actions for
 all things CI.
 
 
 Features
 ********
 
 Coverage
 ========
 The library currently covers
 
-- historical weather data from ground stations
-- RADOLAN fitted radar data for areal precipitation
-- MOSMIX statistical optimized scalar forecasts extracted from weather models
+- Weather observation data.
+  Both historical and recent.
+- Radar data.
+  All of composite, radolan, radvor, sites and radolan_cdc.
+- MOSMIX statistical optimized scalar forecasts extracted from weather models.
+  Both MOSMIX-L and MOSMIX-S is supported.
 
 To get better insight on which data we have currently made available, with this library
 take a look at `data coverage`_.
 
 
 Details
 =======
 - Get metadata for a set of Parameter, PeriodType and TimeResolution.
 - Get station(s) nearby a selected location.
 - Store/recover collected data.
 - Command line interface.
 - Run SQL queries on the results.
 - Export results to databases and other data sinks.
-- Public Docker image on ghcr.io.
+- Public Docker image.
 
 
 Setup
 *****
 Run this to make ``wetterdienst`` available in your current environment:
 
 .. code-block:: bash
@@ -168,30 +178,29 @@
 
 Synopsis
 ********
 Get historical data for specific stations, using Python:
 
 .. code-block:: python
 
-    from wetterdienst import DWDStationRequest, Parameter, PeriodType, TimeResolution
+    from wetterdienst import DWDObservationData, Parameter, PeriodType, TimeResolution
 
-    request = DWDStationRequest(
+    observations = DWDObservationData(
         station_ids=[1048,4411],
         parameter=[Parameter.CLIMATE_SUMMARY, Parameter.SOLAR],
         time_resolution=TimeResolution.DAILY,
         start_date="1990-01-01",
         end_date="2020-01-01",
         tidy_data=True,
         humanize_column_names=True,
-        write_file=True,
-        prefer_local=True
     )
 
-    for df in request.collect_data():
-        # analyse the station here
+    # Collect and analyse data here.
+    for df in observations.collect_data():
+        print(df)
 
 Get data for specific stations from the command line:
 
 .. code-block:: bash
 
     # Get list of all stations for daily climate summary data in JSON format
     wetterdienst stations --parameter=kl --resolution=daily --period=recent
```

