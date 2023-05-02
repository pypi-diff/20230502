# Comparing `tmp/hdsr_fewspy-1.4.tar.gz` & `tmp/hdsr_fewspy-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.4.tar", last modified: Tue May  2 11:07:43 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.5.tar", last modified: Tue May  2 16:32:30 2023, max compression
```

## Comparing `hdsr_fewspy-1.4.tar` & `hdsr_fewspy-1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    22741 2023-05-02 11:07:45.000000 hdsr_fewspy-1.4/PKG-INFO
--rw-rw-rw-   0        0        0    21865 2023-05-02 11:04:14.000000 hdsr_fewspy-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/
--rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    13952 2023-05-02 10:30:15.000000 hdsr_fewspy-1.4/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-05-02 10:26:47.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     9390 2023-05-02 10:33:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     5781 2023-05-01 14:59:17.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2636 2023-05-01 14:10:38.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.4/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.4/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-05-01 14:59:17.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    12259 2023-05-02 10:21:43.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     7155 2023-05-02 10:02:46.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    22741 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-02 11:07:44.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 14:59:36.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 11:07:43.000000 hdsr_fewspy-1.4/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-02 11:07:45.000000 hdsr_fewspy-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-02 10:12:25.000000 hdsr_fewspy-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    22748 2023-05-02 16:32:31.000000 hdsr_fewspy-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    21872 2023-05-02 16:32:08.000000 hdsr_fewspy-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    13962 2023-05-02 16:24:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6394 2023-05-02 11:50:34.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.5/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.5/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.5/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1815 2023-05-02 16:24:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7674 2023-05-02 16:25:46.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    22748 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-02 16:32:31.000000 hdsr_fewspy-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-02 15:44:24.000000 hdsr_fewspy-1.5/setup.py
```

### Comparing `hdsr_fewspy-1.4/LICENSE.txt` & `hdsr_fewspy-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/PKG-INFO` & `hdsr_fewspy-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.4
+Version: 1.5
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.4.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.5.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -27,14 +27,15 @@
 
 [hkvfewspy]: https://github.com/HKV-products-services/hkvfewspy
 [fewspy]: https://github.com/d2hydro/fewspy
 [MIT]: https://github.com/hdsr-mid/hdsr_fewspy/blob/main/LICENSE.txt
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+[releases]: https://pypi.org/project/hdsr-fewspy/#history
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
 authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
@@ -320,59 +321,57 @@
    GITHUB_PERSONAL_ACCESS_TOKEN=<your_token>
    
 
 ### License 
 [MIT]
 
 ### Releases
-TODO
+[Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
 ### Test Coverage (May 2nd 2023)
 ```
--- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
-
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
+hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
-hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1507    188    88%
+TOTAL                                                              1518    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.4/README.md` & `hdsr_fewspy-1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 [hkvfewspy]: https://github.com/HKV-products-services/hkvfewspy
 [fewspy]: https://github.com/d2hydro/fewspy
 [MIT]: https://github.com/hdsr-mid/hdsr_fewspy/blob/main/LICENSE.txt
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+[releases]: https://pypi.org/project/hdsr-fewspy/#history
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
 authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
@@ -298,59 +299,57 @@
    GITHUB_PERSONAL_ACCESS_TOKEN=<your_token>
    
 
 ### License 
 [MIT]
 
 ### Releases
-TODO
+[Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
 ### Test Coverage (May 2nd 2023)
 ```
--- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
-
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
+hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
-hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1507    188    88%
+TOTAL                                                              1518    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from hdsr_fewspy import api_calls
 from hdsr_fewspy import exceptions
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.choices import TimeZoneChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.constants.pi_settings import pi_settings_production
 from hdsr_fewspy.constants.pi_settings import PiSettings
-from hdsr_fewspy.constants.request_settings import default_request_settings
+from hdsr_fewspy.constants.request_settings import get_default_request_settings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.permissions import Permissions
 from hdsr_fewspy.retry_session import RetryBackoffSession
 from pathlib import Path
 from typing import List
 from typing import Optional
 from typing import Union
@@ -39,15 +39,15 @@
         self,
         pi_settings: PiSettings = pi_settings_production,
         output_directory_root: Union[str, Path] = None,
     ):
         self.permissions = Permissions()
         self.output_dir = self._get_output_dir(output_directory_root=output_directory_root)
         self.pi_settings = self._validate_pi_settings(pi_settings=pi_settings)
-        self.request_settings: RequestSettings = default_request_settings
+        self.request_settings: RequestSettings = get_default_request_settings()
         self.retry_backoff_session = RetryBackoffSession(
             _request_settings=self.request_settings,
             pi_settings=self.pi_settings,
             output_dir=self.output_dir,
         )
         self._ensure_service_is_running()
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
                  'default_request_period': Timedelta('35 days 00:00:00'),
                  'document_format': 'PI_JSON',
                  'document_version': 1.25,
                  'domain': 'localhost',
                  'filter_id': 'INTERNAL-API',
                  'max_request_nr_timestamps': 100000,
                  'max_request_period': Timedelta('728 days 00:00:00'),
-                 'max_request_size_kb': 3000,
                  'max_response_time': Timedelta('0 days 00:00:20'),
                  'min_request_nr_timestamps': 10000,
                  'min_time_between_requests': Timedelta('0 days 00:00:01'),
                  'module_instance_ids': 'WerkFilter',
                  'output_choice': 'json_response_in_memory',
                  'output_dir': None,
                  'port': 8080,
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,20 +125,21 @@
                 date_range_freq=date_range_freq,
                 request_settings=self.request_settings,
                 startdate_request=data_range_start,
                 enddate_request=data_range_end,
             )
             create_new_date_ranges = new_date_range_freq != date_range_freq
             if create_new_date_ranges:
+                self.request_settings.updated_request_period = new_date_range_freq
                 new_date_ranges, new_date_range_freq = DateFrequencyBuilder.create_date_ranges_and_frequency_used(
                     startdate_obj=data_range_start,
                     enddate_obj=pd.Timestamp(self.end_time),
                     frequency=new_date_range_freq,
                 )
-                logger.info(f"Updated request time-window from {date_range_freq} to {new_date_range_freq}")
+                logger.debug(f"Updated request time-window from {date_range_freq} to {new_date_range_freq}")
                 # continue with recursive call with updated (smaller or larger) time-window
                 return self._download_timeseries(
                     date_ranges=new_date_ranges,
                     date_range_freq=new_date_range_freq,
                     request_params=request_params,
                     responses=responses,
                 )
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,24 @@
         ]
 
     def run(self) -> List[Path]:
         all_file_paths = []
         responses = []
         cartesian_parameters_list = self._get_cartesian_parameters_list(parameters=self.initial_fews_parameters)
         for index, request_params in enumerate(cartesian_parameters_list):
+            # eventually continue with request_period of last request (avoiding all freq update iterations)
+            frequency = (
+                self.request_settings.updated_request_period
+                if self.request_settings.updated_request_period
+                else self.request_settings.default_request_period
+            )
             date_ranges, date_range_freq = DateFrequencyBuilder.create_date_ranges_and_frequency_used(
                 startdate_obj=pd.Timestamp(self.start_time),
                 enddate_obj=pd.Timestamp(self.end_time),
-                frequency=self.request_settings.default_request_period,
+                frequency=frequency,
             )
             responses = self._download_timeseries(
                 date_ranges=date_ranges,
                 date_range_freq=date_range_freq,
                 request_params=request_params,
                 responses=responses,
             )
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,22 @@
         return [
             OutputChoices.json_response_in_memory,
             OutputChoices.xml_response_in_memory,
             OutputChoices.pandas_dataframe_in_memory,
         ]
 
     def run(self) -> Union[List[ResponseType], pd.DataFrame]:
+        # eventually continue with request_period of last request (avoiding all freq update iterations)
+        frequency = (
+            self.request_settings.updated_request_period
+            if self.request_settings.updated_request_period
+            else self.request_settings.default_request_period
+        )
         date_ranges, date_range_freq = DateFrequencyBuilder.create_date_ranges_and_frequency_used(
-            startdate_obj=pd.Timestamp(self.start_time),
-            enddate_obj=pd.Timestamp(self.end_time),
-            frequency=self.request_settings.default_request_period,
+            startdate_obj=pd.Timestamp(self.start_time), enddate_obj=pd.Timestamp(self.end_time), frequency=frequency
         )
         responses = self._download_timeseries(
             date_ranges=date_ranges,
             date_range_freq=date_range_freq,
             request_params=self.initial_fews_parameters,
         )
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.5/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.5/hdsr_fewspy/constants/paths.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.5/hdsr_fewspy/constants/pi_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -107,47 +107,56 @@
         "port",
         "service",
         "filter_id",
         "module_instance_ids",
         "time_zone",
     ]
 
-    @classmethod
-    def _read_github(cls, settings_name: str) -> pd.Series:
-        logger.info(f"get_on_the_fly_pi_settings for setttings_name {settings_name}")
+    def __init__(self):
+        self._df_github_settings = None
+
+    @property
+    def df_github_settings(self) -> pd.DataFrame:
+        if self._df_github_settings is not None:
+            return self._df_github_settings
         github_downloader = GithubFileDownloader(
             target_file=github.GITHUB_HDSR_FEWSPY_AUTH_SETTINGS_TARGET_FILE,
             allowed_period_no_updates=github.GITHUB_HDSR_FEWSPY_AUTH_ALLOWED_PERIOD_NO_UPDATES,
             repo_name=github.GITHUB_HDSR_FEWSPY_AUTH_REPO_NAME,
             branch_name=github.GITHUB_HDSR_FEWSPY_AUTH_BRANCH_NAME,
             repo_organisation=github.GITHUB_ORGANISATION,
         )
         df = pd.read_csv(filepath_or_buffer=github_downloader.get_download_url(), sep=";")
-        df_slice = df[df["settings_name"] == settings_name]
+        assert sorted(df.columns) == sorted(self.expected_columns), "code_error"
+        self._df_github_settings = df
+        return self._df_github_settings
+
+    def _read_github(self, settings_name: str) -> pd.Series:
+        logger.info(f"get_on_the_fly_pi_settings for setttings_name '{settings_name}'")
+        df_slice = self.df_github_settings[self.df_github_settings["settings_name"] == settings_name]
         if df_slice.empty:
-            available_setting_names = df["settings_name"].tolist()
-            msg = f"pi settings_name {settings_name} is not in available setting_names {available_setting_names}"
+            available_setting_names = self.df_github_settings["settings_name"].tolist()
+            msg = f"pi settings_name '{settings_name}' is not in available setting_names '{available_setting_names}'"
             raise AssertionError(msg)
         assert len(df_slice) == 1, "code error"
-        assert sorted(df.columns) == sorted(cls.expected_columns), "code_error"
         pd_series = df_slice.iloc[0]
         return pd_series
 
-    @classmethod
-    def get_pi_settings(cls, settings_name: str) -> PiSettings:
-        pd_series = cls._read_github(settings_name=settings_name)
+    def get_pi_settings(self, settings_name: str) -> PiSettings:
+        pd_series = self._read_github(settings_name=settings_name)
         pi_settings = PiSettings(
             settings_name=pd_series["settings_name"],
             document_version=pd_series["document_version"],
             ssl_verify=bool(pd_series["ssl_verify"]),
             domain=pd_series["domain"],
             port=int(pd_series["port"]),
             service=pd_series["service"],
             filter_id=pd_series["filter_id"],
             module_instance_ids=pd_series["module_instance_ids"],
             time_zone=float(pd_series["time_zone"]),
         )
         return pi_settings
 
 
-pi_settings_sa = GithubPiSettings.get_pi_settings(settings_name="standalone")
-pi_settings_production = GithubPiSettings.get_pi_settings(settings_name="production")
+github_pi_settings = GithubPiSettings()
+pi_settings_sa = github_pi_settings.get_pi_settings(settings_name="standalone")
+pi_settings_production = github_pi_settings.get_pi_settings(settings_name="production")
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.5/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.5/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.5/hdsr_fewspy/converters/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
         if self.output_choice == OutputChoices.xml_file_in_download_dir:
             return XmlDownloadDir(request_class=self.request_class, output_dir=self.output_dir)
         elif self.output_choice == OutputChoices.json_file_in_download_dir:
             return JsonDownloadDir(request_class=self.request_class, output_dir=self.output_dir)
         elif self.output_choice == OutputChoices.csv_file_in_download_dir:
             return CsvDownloadDir(request_class=self.request_class, output_dir=self.output_dir)
         else:
-            logger.info(f"memory choice {self.output_choice} must be handled in GetRequest.run() itself")
+            logger.debug(f"memory choice {self.output_choice} must be handled in GetRequest.run() itself")
             return None
 
     def run(self, responses: List[ResponseType], **kwargs):
         # allowed_kwargs = ["file_name_values", "drop_missing_values", "flag_threshold"]
         return self.response_handler.run(responses=responses, **kwargs)
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.5/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.5/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.5/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/exceptions.py` & `hdsr_fewspy-1.5/hdsr_fewspy/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.5/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.5/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.5/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,34 +193,26 @@
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_file_in_download_dir,
     )
     assert len(all_file_paths) == 9
 
     mapper_expected_xmls = request_data.get_expected_xmls()
     for downloaded_file in all_file_paths:
-        try:
-            found = parse(downloaded_file.as_posix())
-            found_header = found.TimeSeries.series.header
-            found_events = found.TimeSeries.series.event
-
-            expected = mapper_expected_xmls[downloaded_file.stem]
-            expected_header = expected.TimeSeries.series.header
-            expected_events = expected.TimeSeries.series.event
-
-            assert found_header.timeStep._attributes["unit"] == expected_header.timeStep._attributes["unit"]
-            assert len(found_events) == len(expected_events)
-            assert found_events[0]._attributes["date"] == expected_events[0]._attributes["date"]
-            assert found_events[-1]._attributes["date"] == expected_events[-1]._attributes["date"]
-        except AttributeError:
-            assert downloaded_file.name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_3.xml"
-            found = parse(downloaded_file.as_posix())
-            expected = mapper_expected_xmls[downloaded_file.stem]
-            for x in (found, expected):
-                assert x.root.doc.response_http_status.cdata == "400"
-                assert x.root.doc.response_text.cdata == "No timeSeries found"
+        found = parse(downloaded_file.as_posix())
+        found_header = found.TimeSeries.series.header
+        found_events = found.TimeSeries.series.event
+
+        expected = mapper_expected_xmls[downloaded_file.stem]
+        expected_header = expected.TimeSeries.series.header
+        expected_events = expected.TimeSeries.series.event
+
+        assert found_header.timeStep._attributes["unit"] == expected_header.timeStep._attributes["unit"]
+        assert len(found_events) == len(expected_events)
+        assert found_events[0]._attributes["date"] == expected_events[0]._attributes["date"]
+        assert found_events[-1]._attributes["date"] == expected_events[-1]._attributes["date"]
 
 
 def test_sa_multi_timeseries_2_ok_csv_download(fixture_api_sa_with_download_dir):
     """OutputChoices.csv_file_in_download_dir"""
     api = fixture_api_sa_with_download_dir
     request_data = fixtures_requests.RequestTimeSeriesMulti2
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,35 +137,41 @@
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
     )
     assert len(responses) == 11
+    assert api.request_settings.default_request_period == pd.Timedelta(days=56)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
 
 
 def test_sa_single_ts_long_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
     )
     assert len(responses) == 11
+    assert api.request_settings.default_request_period == pd.Timedelta(days=56)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
 
 
 def test_sa_single_ts_long_ok_df_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     df_found = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.pandas_dataframe_in_memory,
     )
-    assert len(df_found) == 199251
+    assert len(df_found) == 199255
+    assert api.request_settings.default_request_period == pd.Timedelta(days=56)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.5/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.4
+Version: 1.5
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.4.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.5.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -27,14 +27,15 @@
 
 [hkvfewspy]: https://github.com/HKV-products-services/hkvfewspy
 [fewspy]: https://github.com/d2hydro/fewspy
 [MIT]: https://github.com/hdsr-mid/hdsr_fewspy/blob/main/LICENSE.txt
 [Deltares FEWS PI]: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service
 [issues page]: https://github.com/hdsr-mid/hdsr_fewspy/issues
 [github personal token]: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+[releases]: https://pypi.org/project/hdsr-fewspy/#history
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds client-side authentication, 
 authorisation, and throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
@@ -320,59 +321,57 @@
    GITHUB_PERSONAL_ACCESS_TOKEN=<your_token>
    
 
 ### License 
 [MIT]
 
 ### Releases
-TODO
+[Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
 ### Test Coverage (May 2nd 2023)
 ```
--- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
-
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   99     11    89%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                           108      9    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
-hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
+hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
-hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1507    188    88%
+TOTAL                                                              1518    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.4/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.5/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/pyproject.toml` & `hdsr_fewspy-1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.4/setup.py` & `hdsr_fewspy-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.4"
+version = "1.5"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

