# Comparing `tmp/hdsr_fewspy-1.3.tar.gz` & `tmp/hdsr_fewspy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.3.tar", last modified: Mon May  1 14:59:36 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.4.tar", last modified: Tue May  2 11:07:43 2023, max compression
```

## Comparing `hdsr_fewspy-1.3.tar` & `hdsr_fewspy-1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    22740 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/PKG-INFO
--rw-rw-rw-   0        0        0    21864 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/
--rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    13821 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     8329 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     5781 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2636 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4332 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    13380 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     6655 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    22740 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    22741 2023-05-02 11:07:45.000000 hdsr_fewspy-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21865 2023-05-02 11:04:14.000000 hdsr_fewspy-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    13952 2023-05-02 10:30:15.000000 hdsr_fewspy-1.4/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-05-02 10:26:47.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9390 2023-05-02 10:33:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     5781 2023-05-01 14:59:17.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2636 2023-05-01 14:10:38.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.4/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.4/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-05-01 14:59:17.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    12259 2023-05-02 10:21:43.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7155 2023-05-02 10:02:46.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    22741 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 14:59:36.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-02 11:07:45.000000 hdsr_fewspy-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-02 10:12:25.000000 hdsr_fewspy-1.4/setup.py
```

### Comparing `hdsr_fewspy-1.3/LICENSE.txt` & `hdsr_fewspy-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/PKG-INFO` & `hdsr_fewspy-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.3
+Version: 1.4
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.3.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.4.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -31,16 +31,16 @@
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
-two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
-throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
+two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
+authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
 Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
@@ -50,17 +50,17 @@
 ------------------------------|--------------------|--------
 get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
 get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
 get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
 get_qualifiers                | 4, 6               | Returns 1 object (xml response or dataframe)
 get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
 get_samples                   | TODO               | Not implemented yet
-get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
-get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
@@ -325,54 +325,54 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 1st 2023)
+### Test Coverage (May 2nd 2023)
 ```
 -- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
 
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   98     10    90%
+hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
 hdsr_fewspy\constants\request_settings.py                            11      0   100%
-hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
-hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1497    183    88%
+TOTAL                                                              1507    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.3/README.md` & `hdsr_fewspy-1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
-two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
-throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
+two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
+authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
 Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
@@ -28,17 +28,17 @@
 ------------------------------|--------------------|--------
 get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
 get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
 get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
 get_qualifiers                | 4, 6               | Returns 1 object (xml response or dataframe)
 get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
 get_samples                   | TODO               | Not implemented yet
-get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
-get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
@@ -303,54 +303,54 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 1st 2023)
+### Test Coverage (May 2nd 2023)
 ```
 -- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
 
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   98     10    90%
+hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
 hdsr_fewspy\constants\request_settings.py                            11      0   100%
-hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
-hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1497    183    88%
+TOTAL                                                              1507    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from hdsr_fewspy import api_calls
 from hdsr_fewspy import exceptions
+from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.choices import TimeZoneChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.constants.pi_settings import pi_settings_production
 from hdsr_fewspy.constants.pi_settings import PiSettings
 from hdsr_fewspy.constants.request_settings import default_request_settings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.permissions import Permissions
@@ -14,15 +15,14 @@
 from typing import Optional
 from typing import Union
 
 import geopandas as gpd
 import logging
 import os
 import pandas as pd
-import requests
 import urllib3  # noqa
 
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 logger = logging.getLogger(__name__)
@@ -63,15 +63,15 @@
         assert is_dir_writable, f"output_directory_root {output_directory_root} must be writable"
         # create subdir
         output_dir = output_directory_root / f"hdsr_fewspy_{datetime.now().strftime('%Y%m%d_%H%M%S')}"
         return output_dir
 
     def _ensure_service_is_running(self) -> None:
         # check endpoint with smallest response (=timezonid)
-        response = requests.get(url=f"{self.pi_settings.base_url}timezoneid/", verify=self.pi_settings.ssl_verify)
+        response = self.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
         if response.ok:
             logger.info("PiWebService is running")
             return
         msg = (
             f"Piwebservice is not running, err={response.text}. Ensure that you can visit the test page "
             f"{self.pi_settings.test_url}"
         )
@@ -88,19 +88,20 @@
             "domain": (pi_settings.domain, self.permissions.allowed_domain),
             "module_instance_id": (pi_settings.module_instance_ids, self.permissions.allowed_module_instance_id),
             "timezone": (pi_settings.time_zone, TimeZoneChoices.get_all()),
             "filter_id": (pi_settings.filter_id, self.permissions.allowed_filter_id),
             "service": (pi_settings.service, self.permissions.allowed_service),
         }
         for setting, value in mapper.items():
-            used, allowed = value
-            assert isinstance(allowed, list), f"code error, {allowed} must be a list"
-            if used in allowed:
+            used_value, allowed_values = value
+            assert isinstance(allowed_values, list), f"code error, allowed_values {allowed_values} must be a list"
+            if used_value in allowed_values:
                 continue
-            raise exceptions.PiSettingsError(f"{setting} has {used} which is not in allowed {allowed}")
+            msg = f"setting='{setting}' used_value='{used_value}' is not in allowed_values='{allowed_values}'"
+            raise exceptions.PiSettingsError(msg)
 
         return pi_settings
 
     def get_parameters(self, output_choice: str) -> Union[ResponseType, pd.DataFrame]:
         """Get FEWS parameters as a pandas DataFrame."""
         # show_attributes does not make a difference in response (both for Pi_JSON and PI_XML)
         api_call = api_calls.GetParameters(
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from hdsr_fewspy.constants.choices import ApiParameters
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.constants.pi_settings import PiSettings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.converters.manager import ResponseManager
-from hdsr_fewspy.converters.utils import datetime_to_fews_str
+from hdsr_fewspy.converters.utils import datetime_to_fews_date_str
 from hdsr_fewspy.converters.utils import snake_to_camel_case
 from hdsr_fewspy.retry_session import RetryBackoffSession
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
@@ -140,15 +140,15 @@
         """Prepare Python API dictionary for FEWS API request.
 
         Arg:
             - do_filter (bool): filters out all parameters not in allowed_request_args."""
 
         def _convert_kv(k: str, v) -> Tuple[str, Any]:
             if k in ApiParameters.non_pi_settings_keys_datetime():
-                v = datetime_to_fews_str(v)
+                v = datetime_to_fews_date_str(v)
             k = snake_to_camel_case(k)
             return k, v
 
         # non pi settings
         filtered = self.allowed_request_args if do_filter else ApiParameters.non_pi_settings_keys()
         params_non_pi = [_convert_kv(k, v) for k, v in parameters.items() if k in filtered]
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod
 from datetime import datetime
+from hdsr_fewspy import exceptions
 from hdsr_fewspy.api_calls.base import GetRequest
 from hdsr_fewspy.constants.choices import ApiParameters
 from hdsr_fewspy.constants.choices import PiRestDocumentFormatChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
-from hdsr_fewspy.converters.utils import datetime_to_fews_str
+from hdsr_fewspy.converters.utils import datetime_to_fews_date_str
 from hdsr_fewspy.converters.xml_to_python_obj import parse
 from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
@@ -17,14 +18,19 @@
 import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 
 class GetTimeSeriesBase(GetRequest):
+
+    response_text_no_ts_found = "No timeSeries found"
+    response_text_location_not_found = "Some of the location ids do not exist"
+    response_text_parameter_not_found = "Some of the parameters do not exists"
+
     def __init__(
         self,
         start_time: datetime,
         end_time: datetime,
         location_ids: Union[List[str], str],
         parameter_ids: Union[List[str], str],
         qualifier_ids: Union[List[str], str] = None,
@@ -102,17 +108,21 @@
         Before each download of actual timeseries we first check nr_timestamps_in_response (a small request with
         showHeaders=True, and showStatistics=True). If that number if outside a certain bandwith, then we update
         (smaller or larger windows) parameters 'startTime' and 'endTime' again.
         """
         responses = responses if responses else []
         for request_index, (data_range_start, data_range_end) in enumerate(date_ranges):
             # update start and end in request params
-            request_params["startTime"] = datetime_to_fews_str(data_range_start)
-            request_params["endTime"] = datetime_to_fews_str(data_range_end)
-            nr_timestamps_in_response = self._get_nr_timestamps(request_params=request_params)
+            request_params["startTime"] = datetime_to_fews_date_str(data_range_start)
+            request_params["endTime"] = datetime_to_fews_date_str(data_range_end)
+            try:
+                nr_timestamps_in_response = self._get_nr_timestamps(request_params=request_params)
+            except (exceptions.LocationIdsDoesNotExistErr, exceptions.ParameterIdsDoesNotExistErr) as err:
+                logger.warning(err)
+                return []
             logger.debug(f"nr_timestamps_in_response={nr_timestamps_in_response}")
             new_date_range_freq = DateFrequencyBuilder.optional_change_date_range_freq(
                 nr_timestamps=nr_timestamps_in_response,
                 date_range_freq=date_range_freq,
                 request_settings=self.request_settings,
                 startdate_request=data_range_start,
                 enddate_request=data_range_end,
@@ -142,47 +152,57 @@
                 request_params["onlyHeaders"] = False
                 request_params["showStatistics"] = False
                 response = self.retry_backoff_session.get(
                     url=self.url, params=request_params, verify=self.pi_settings.ssl_verify
                 )
                 if response.status_code != 200:
                     logger.error(f"FEWS Server responds {response.text}")
-                responses.append(response)
+                else:
+                    responses.append(response)
         return responses
 
     def _get_statistics(self, request_params: Dict) -> ResponseType:
         request_params["onlyHeaders"] = True
         request_params["showStatistics"] = True
         response = self.retry_backoff_session.get(
             url=self.url, params=request_params, verify=self.pi_settings.ssl_verify
         )
         return response
 
     def _get_nr_timestamps(self, request_params: Dict) -> int:
         assert "moduleInstanceIds" in request_params, "code error"
         response = self._get_statistics(request_params=request_params)
+        msg = f"status_code={response.status_code}, err={response.text}, request_params={request_params}"
         if not response.ok:
-            if response.text == "No timeSeries found":
-                return 0
-            raise AssertionError(f"response not okay, status_code={response.status_code}, err={response.text}")
+            return self.__get_nr_timestamps_invalid_response(response=response, msg=msg)
         if self.pi_settings.document_format == PiRestDocumentFormatChoices.json:
             timeseries = response.json().get("timeSeries", None)
             if not timeseries:
                 return 0
             nr_timeseries = len(timeseries)
             if nr_timeseries == 1:
                 nr_timestamps = int(timeseries[0]["header"]["valueCount"])
                 return nr_timestamps
-            raise AssertionError(f"code error: found {nr_timeseries} timeseries in _get_nr_timestamps. Expected 0 or 1")
+            msg = f"code error: found {nr_timeseries} timeseries in _get_nr_timestamps. Expected 0 or 1, {msg}"
+            raise AssertionError(msg)
         elif self.pi_settings.document_format == PiRestDocumentFormatChoices.xml:
             xml_python_obj = parse(response.text)
             try:
                 nr_timestamps = int(xml_python_obj.TimeSeries.series.header.valueCount.cdata)
                 return nr_timestamps
             except Exception as err:
-                raise AssertionError(f"could not get nr_timestamps from xml_python_obj, err={err}")
+                raise AssertionError(f"could not get nr_timestamps from xml_python_obj, err={err}, {msg}")
         else:
-            raise NotImplementedError("only xml and json are available")
+            raise NotImplementedError(f"invalid document_format {self.pi_settings.document_format}")
+
+    def __get_nr_timestamps_invalid_response(self, response: ResponseType, msg: str):
+        if self.response_text_no_ts_found in response.text:
+            return 0
+        if self.response_text_location_not_found in response.text:
+            raise exceptions.LocationIdsDoesNotExistErr(msg)
+        elif self.response_text_parameter_not_found in response.text:
+            raise exceptions.ParameterIdsDoesNotExistErr(msg)
+        raise AssertionError(f"(unknown non-200 response, {msg}")
 
     @abstractmethod
     def run(self, *args, **kwargs):
         raise NotImplementedError
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.4/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.4/hdsr_fewspy/constants/paths.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.4/hdsr_fewspy/constants/pi_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.4/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.4/hdsr_fewspy/converters/download.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
 from pathlib import Path
-from typing import Dict
 from typing import List
 
 import json
 import logging
 import requests
-import xml.etree.cElementTree as ET  # TODO: from xml.etree import ElementTree
 
 
 logger = logging.getLogger(__name__)
 
 
 class DownloadBase:
     def __init__(self, request_class: str, output_dir: Path):
@@ -62,51 +60,38 @@
             self.output_dir.mkdir(parents=True, exist_ok=True)
 
     def run(self, responses: List[requests.models.Response], file_name_values: List[str], **kwargs):
         raise NotImplementedError
 
 
 class XmlDownloadDir(DownloadBase):
-    @staticmethod
-    def create_custom_xml_tree(data: Dict):
-        root = ET.Element("root")
-        doc = ET.SubElement(root, "doc")
-        for key, value in data.items():
-            ET.SubElement(doc, key, name=key).text = str(value)
-        tree = ET.ElementTree(root)
-        return tree
-
     def run(self, responses: List[ResponseType], file_name_values: List[str], **kwargs) -> List[Path]:
         """Create for every response a separate .xml file.
         All responses are for a unique location_parameter_qualifier combi in get_time_series_multi."""
         file_name_base = self._get_base_file_name(request_class=self.request_class, file_name_values=file_name_values)
         file_paths_created = []
         for index, response in enumerate(responses):
+            assert response.status_code == 200, "code error"
             file_path = self.output_dir / f"{file_name_base}_{index}.xml"
             logger.info(f"writing response to new file {file_path}")
             self._ensure_output_dir_exists(file_path=file_path)
-            if response.status_code != 200:
-                response_in_xml = self.create_custom_xml_tree(
-                    data={"response_http_status": response.status_code, "response_text": response.text}
-                )
-                response_in_xml.write(file_or_filename=file_path.as_posix(), encoding="utf-8")
-            else:
-                with open(file=file_path.as_posix(), mode="w", encoding="utf-8") as xml_file:
-                    xml_file.write(response.text)
+            with open(file=file_path.as_posix(), mode="w", encoding="utf-8") as xml_file:
+                xml_file.write(response.text)
             file_paths_created.append(file_path)
         return file_paths_created
 
 
 class JsonDownloadDir(DownloadBase):
     def run(self, responses: List[ResponseType], file_name_values: List[str], **kwargs) -> List[Path]:
         """Create for every response a separate .json file.
         All responses are for a unique location_parameter_qualifier combi in get_time_series_multi."""
         file_name_base = self._get_base_file_name(request_class=self.request_class, file_name_values=file_name_values)
         file_paths_created = []
         for index, response in enumerate(responses):
+            assert response.status_code == 200, "code error"
             file_path = self.output_dir / f"{file_name_base}_{index}.json"
             logger.info(f"writing response to new file {file_path}")
             self._ensure_output_dir_exists(file_path=file_path)
             with open(file=file_path.as_posix(), mode="w", encoding="utf-8") as json_file:
                 # indent=None results in half the file size compared to indent=4
                 json.dump(obj=response.json(), fp=json_file, ensure_ascii=False, indent=None)
             file_paths_created.append(file_path)
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.4/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.4/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.4/hdsr_fewspy/converters/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         datetime: Converted datetime object (in example datetime.datetime(2022, 5, 1, 0, 0))
     """
     time = data.get("time", "00:00:00")
     date_time = datetime.fromisoformat(f'{data["date"]}T{time}')
     return date_time
 
 
-def datetime_to_fews_str(date_time: datetime) -> str:
+def datetime_to_fews_date_str(date_time: datetime) -> str:
     """Convert a FEWS PI datetime to datetime str e.g. 2022-05-01T00:00:00Z."""
     try:
         fews_str = date_time.strftime(TimeZoneChoices.date_string_format())
         return fews_str
     except Exception:
         msg = f"Could not convert datetime {date_time} to str using format {TimeZoneChoices.date_string_format()}"
         raise AssertionError(msg)
@@ -81,9 +81,9 @@
             epsg_code += 100
         crs = f"epsg:{epsg_code}"
     elif geo_datum.lower().startswith("epsg"):
         crs = geo_datum.lower()
     elif geo_datum in GEODATUM_MAPPING.keys():
         crs = GEODATUM_MAPPING[geo_datum]
     else:
-        crs = None
+        crs = ""
     return crs
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.4/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.4/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.4/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.4/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.4/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,37 +53,49 @@
         csv_paths = dict()
         for file_path in file_paths:
             df = pd.read_csv(filepath_or_buffer=file_path.as_posix(), sep=",")
             csv_paths[file_path.stem] = df
         return csv_paths
 
 
-class RequestTimeSeriesSingle1(RequestTimeSeriesBase):
+class RequestTimeSeriesSingleShort(RequestTimeSeriesBase):
     """Single as we use 1 location_ids and 1 parameter_ids."""
 
     # OW433001 H.G.O loopt van 29 sep 2011 tm 17 jan 2023 (filters: WIS/Werkfilter, WIS/Metingenfilter, HDSR/CAW)
     location_ids = "OW433001"
     parameter_ids = "H.G.0"
     start_time = datetime(2012, 1, 1)
     end_time = datetime(2012, 1, 2)
 
     @classmethod
     def file_dir_expected_files(cls) -> Path:
         return TEST_INPUT_DIR / "RequestTimeSeriesSingle1"
 
 
-class RequestTimeSeriesSingle2(RequestTimeSeriesBase):
-    """Single as we use 1 location_ids and 1 parameter_ids."""
+class RequestTimeSeriesSingleLong(RequestTimeSeriesBase):
+    """Long timeseries"""
 
     # OW433001 H.G.O loopt van 29 sep 2011 tm 17 jan 2023 (filters: WIS/Werkfilter, WIS/Metingenfilter, HDSR/CAW)
     location_ids = "OW433001"
     parameter_ids = "H.G.0"
     start_time = datetime(2012, 1, 1)
-    # end_time = datetime(2012, 6, 1)  # 11227 df rows?? get many timestamp
-    end_time = datetime(2016, 1, 1)  # 9157 df rows ??
+    end_time = datetime(2016, 1, 1)
+
+    @classmethod
+    def file_dir_expected_files(cls) -> Path:
+        return Path("not used in test")
+
+
+class RequestTimeSeriesSingleNaN(RequestTimeSeriesBase):
+    """Location does not exists"""
+
+    location_ids = "OW1234"
+    parameter_ids = "H.G.O"
+    start_time = datetime(year=2022, month=11, day=1)
+    end_time = datetime(year=2022, month=11, day=3)
 
     @classmethod
     def file_dir_expected_files(cls) -> Path:
         return Path("not used in test")
 
 
 class RequestTimeSeriesMulti1(RequestTimeSeriesBase):
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files 8% similar despite different names*

```diff
@@ -189,25 +189,15 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_file_in_download_dir,
     )
-    assert len(all_file_paths) == 10
-    assert all_file_paths[0].name == "gettimeseriesmulti_kw215712_qby_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[1].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[2].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_1.xml"
-    assert all_file_paths[3].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[4].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_1.xml"
-    assert all_file_paths[5].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_2.xml"
-    assert all_file_paths[6].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[7].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_1.xml"
-    assert all_file_paths[8].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_2.xml"
-    assert all_file_paths[9].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_3.xml"
+    assert len(all_file_paths) == 9
 
     mapper_expected_xmls = request_data.get_expected_xmls()
     for downloaded_file in all_file_paths:
         try:
             found = parse(downloaded_file.as_posix())
             found_header = found.TimeSeries.series.header
             found_events = found.TimeSeries.series.event
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,43 +9,57 @@
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
 fixture_api_sa_with_download_dir = fixture_api_sa_with_download_dir
 
 
-def test_sa_single_timeseries_1_wrong(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_wrong(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
 
     request_data = fixtures_requests.RequestTimeSeriesMulti1
     # multiple location_ids is not possible
     with pytest.raises(AssertionError):
         api.get_time_series_single(
             location_id=request_data.location_ids,
             parameter_id=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.json_response_in_memory,
         )
 
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
     # output_choice xml_file_in_download_dir is not possible
     with pytest.raises(AssertionError):
         api.get_time_series_single(
             location_id=request_data.location_ids,
             parameter_id=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.xml_file_in_download_dir,
         )
 
 
-def test_sa_single_timeseries_1_ok_json_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_nan(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleLong
+
+    responses = api.get_time_series_single(
+        location_id="OW123456789",  # location does not exist
+        parameter_id=request_data.parameter_ids,
+        start_time=request_data.start_time,
+        end_time=request_data.end_time,
+        output_choice=OutputChoices.xml_response_in_memory,
+    )
+    assert not responses
+
+
+def test_sa_single_ts_short_ok_json_memory(fixture_api_sa_no_download_dir):
+    api = fixture_api_sa_no_download_dir
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
@@ -56,17 +70,17 @@
     for response_found, expected_json_key in zip(responses, mapper_jsons_expected.keys()):
         assert response_found.status_code == 200
         json_found = response_found.json()
         json_expected = mapper_jsons_expected[expected_json_key]
         assert json_found == json_expected
 
 
-def test_sa_single_timeseries_1_ok_xml_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_short_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
@@ -89,17 +103,17 @@
 
         assert found_unit == expected_unit == "nonequidistant"
         assert len(found_events) == len(expected_events) == 102
         assert found_events[0]._attributes["date"] == expected_events[0]._attributes["date"] == "2012-01-01"
         assert found_events[-1]._attributes["date"] == expected_events[-1]._attributes["date"] == "2012-01-02"
 
 
-def test_sa_single_timeseries_1_ok_df_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_short_ok_df_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
 
     df_found = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.pandas_dataframe_in_memory,
@@ -111,45 +125,45 @@
     df_expected.set_index("datetime", inplace=True)
 
     df_found.set_index(pd.to_datetime(df_found.index), inplace=True)
     df_expected.set_index(pd.to_datetime(df_expected.index), inplace=True)
     pd.testing.assert_frame_equal(left=df_found, right=df_expected, check_index_type=False)
 
 
-def test_sa_single_timeseries_2_ok_json_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_long_ok_json_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle2
+    request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
     )
     assert len(responses) == 11
 
 
-def test_sa_single_timeseries_2_ok_xml_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_long_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle2
+    request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
     )
     assert len(responses) == 11
 
 
-def test_sa_single_timeseries_2_ok_df_memory(fixture_api_sa_no_download_dir):
+def test_sa_single_ts_long_ok_df_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle2
+    request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     df_found = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.pandas_dataframe_in_memory,
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,44 +19,44 @@
             location_id=request_data.location_ids,
             parameter_id=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.json_response_in_memory,
         )
 
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
     # output_choice xml_file_in_download_dir is not possible
     with pytest.raises(AssertionError):
         api.get_time_series_statistics(
             location_id=request_data.location_ids,
             parameter_id=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.xml_file_in_download_dir,
         )
 
 
 def test_sa_timeseries_stats_2_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle2
+    request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     response = api.get_time_series_statistics(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
     )
 
     assert response.status_code == 200
 
 
 def test_sa_timeseries_stats_1_ok_json_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
-    request_data = fixtures_requests.RequestTimeSeriesSingle1
+    request_data = fixtures_requests.RequestTimeSeriesSingleShort
 
     response = api.get_time_series_statistics(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.4/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.3
+Version: 1.4
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.3.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.4.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -31,16 +31,16 @@
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
-two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
-throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
+two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
+authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
 Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
@@ -50,17 +50,17 @@
 ------------------------------|--------------------|--------
 get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
 get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
 get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
 get_qualifiers                | 4, 6               | Returns 1 object (xml response or dataframe)
 get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
 get_samples                   | TODO               | Not implemented yet
-get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
-get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
@@ -325,54 +325,54 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 1st 2023)
+### Test Coverage (May 2nd 2023)
 ```
 -- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
 
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   98     10    90%
+hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
 hdsr_fewspy\constants\request_settings.py                            11      0   100%
-hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
-hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1497    183    88%
+TOTAL                                                              1507    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.3/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.4/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/pyproject.toml` & `hdsr_fewspy-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.3/setup.py` & `hdsr_fewspy-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.3"
+version = "1.4"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

