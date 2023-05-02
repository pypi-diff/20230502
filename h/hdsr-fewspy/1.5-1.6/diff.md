# Comparing `tmp/hdsr_fewspy-1.5.tar.gz` & `tmp/hdsr_fewspy-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.5.tar", last modified: Tue May  2 16:32:30 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.6.tar", last modified: Tue May  2 18:39:18 2023, max compression
```

## Comparing `hdsr_fewspy-1.5.tar` & `hdsr_fewspy-1.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    22748 2023-05-02 16:32:31.000000 hdsr_fewspy-1.5/PKG-INFO
--rw-rw-rw-   0        0        0    21872 2023-05-02 16:32:08.000000 hdsr_fewspy-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/
--rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    13962 2023-05-02 16:24:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6394 2023-05-02 11:50:34.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.5/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.5/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.5/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.5/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1815 2023-05-02 16:24:31.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     7674 2023-05-02 16:25:46.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:32:30.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    22748 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 16:32:28.000000 hdsr_fewspy-1.5/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.5/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-02 16:32:31.000000 hdsr_fewspy-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-02 15:44:24.000000 hdsr_fewspy-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    22748 2023-05-02 18:39:19.000000 hdsr_fewspy-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21872 2023-05-02 16:32:08.000000 hdsr_fewspy-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    14082 2023-05-02 18:30:36.000000 hdsr_fewspy-1.6/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6246 2023-05-02 18:32:13.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.6/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.6/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.6/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7674 2023-05-02 16:25:46.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    22748 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 16:32:28.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-02 18:39:19.000000 hdsr_fewspy-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-02 18:38:09.000000 hdsr_fewspy-1.6/setup.py
```

### Comparing `hdsr_fewspy-1.5/LICENSE.txt` & `hdsr_fewspy-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/PKG-INFO` & `hdsr_fewspy-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.5
+Version: 1.6
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.5.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.6.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hdsr_fewspy-1.5/README.md` & `hdsr_fewspy-1.6/README.md`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from hdsr_fewspy import api_calls
 from hdsr_fewspy import exceptions
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.choices import TimeZoneChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
-from hdsr_fewspy.constants.pi_settings import pi_settings_production
+from hdsr_fewspy.constants.pi_settings import github_pi_setting_defaults
 from hdsr_fewspy.constants.pi_settings import PiSettings
 from hdsr_fewspy.constants.request_settings import get_default_request_settings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.permissions import Permissions
 from hdsr_fewspy.retry_session import RetryBackoffSession
 from pathlib import Path
 from typing import List
@@ -33,15 +33,15 @@
 
     The methods corresponding with the FEWS PI-REST requests. For more info on how to work with the FEWS REST Web
     Service, visit the Deltares website: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service.
     """
 
     def __init__(
         self,
-        pi_settings: PiSettings = pi_settings_production,
+        pi_settings: PiSettings = None,
         output_directory_root: Union[str, Path] = None,
     ):
         self.permissions = Permissions()
         self.output_dir = self._get_output_dir(output_directory_root=output_directory_root)
         self.pi_settings = self._validate_pi_settings(pi_settings=pi_settings)
         self.request_settings: RequestSettings = get_default_request_settings()
         self.retry_backoff_session = RetryBackoffSession(
@@ -76,15 +76,17 @@
             f"{self.pi_settings.test_url}"
         )
         if self.pi_settings.domain == "localhost":
             msg += ". Please make sure FEWS SA webservice is running and start embedded tomcat server via F12 key."
             raise exceptions.StandAloneFewsWebServiceNotRunningError(msg)
         raise exceptions.FewsWebServiceNotRunningError(msg)
 
-    def _validate_pi_settings(self, pi_settings: PiSettings) -> PiSettings:
+    def _validate_pi_settings(self, pi_settings: PiSettings = None) -> PiSettings:
+        if not pi_settings:
+            pi_settings = github_pi_setting_defaults.get_pi_settings(settings_name="production")
         if not isinstance(pi_settings, PiSettings):
             raise AssertionError("pi_settings must be a PiSettings, see README.ml example how to create one")
         mapper = {
             # setting: (used, allowed)
             "domain": (pi_settings.domain, self.permissions.allowed_domain),
             "module_instance_id": (pi_settings.module_instance_ids, self.permissions.allowed_module_instance_id),
             "timezone": (pi_settings.time_zone, TimeZoneChoices.get_all()),
```

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.6/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.6/hdsr_fewspy/constants/paths.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.6/hdsr_fewspy/constants/pi_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             raise AssertionError(f"test_url '{self.test_url}' must be valid")
 
     @property
     def all_fields(self) -> Dict:
         return asdict(self)
 
 
-class GithubPiSettings:
+class GithubPiSettingDefaults:
 
     expected_columns = [
         "settings_name",
         "document_version",
         "ssl_verify",
         "domain",
         "port",
@@ -153,10 +153,8 @@
             filter_id=pd_series["filter_id"],
             module_instance_ids=pd_series["module_instance_ids"],
             time_zone=float(pd_series["time_zone"]),
         )
         return pi_settings
 
 
-github_pi_settings = GithubPiSettings()
-pi_settings_sa = github_pi_settings.get_pi_settings(settings_name="standalone")
-pi_settings_production = github_pi_settings.get_pi_settings(settings_name="production")
+github_pi_setting_defaults = GithubPiSettingDefaults()
```

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.6/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.6/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.6/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.6/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.6/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.6/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.6/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/exceptions.py` & `hdsr_fewspy-1.6/hdsr_fewspy/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.6/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.6/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.6/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from hdsr_fewspy.api import Api
-from hdsr_fewspy.constants.pi_settings import pi_settings_sa
+from hdsr_fewspy.constants.pi_settings import github_pi_setting_defaults
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture(scope="function")
 def fixture_api_sa_no_download_dir():
-    api = Api(pi_settings=pi_settings_sa)
-    assert api.pi_settings.base_url == pi_settings_sa.base_url
+    api = Api(pi_settings=github_pi_setting_defaults.get_pi_settings(settings_name="standalone"))
     assert api.pi_settings.ssl_verify == True  # noqa
     assert api.pi_settings.settings_name == "standalone"
     assert api.pi_settings.domain == "localhost"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     assert api.pi_settings.document_version == 1.25
@@ -22,17 +21,19 @@
 
 
 @pytest.fixture(scope="function")
 def fixture_api_sa_with_download_dir(tmpdir_factory):
     output_dir = tmpdir_factory.mktemp("hdsr_fewspy_test_dir")  # tmpdir_factory can do session scope. nice!
     output_dir_path = Path(output_dir)
     assert output_dir_path.is_dir()
-    api = Api(pi_settings=pi_settings_sa, output_directory_root=output_dir_path)
+    api = Api(
+        pi_settings=github_pi_setting_defaults.get_pi_settings(settings_name="standalone"),
+        output_directory_root=output_dir_path,
+    )
     assert isinstance(api.output_dir, Path)
-    assert api.pi_settings.base_url == pi_settings_sa.base_url
     assert api.pi_settings.ssl_verify == True  # noqa
     assert api.pi_settings.settings_name == "standalone"
     assert api.pi_settings.domain == "localhost"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     assert api.pi_settings.document_version == 1.25
```

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.6/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.5
+Version: 1.6
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.5.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.6.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hdsr_fewspy-1.5/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.6/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/pyproject.toml` & `hdsr_fewspy-1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.5/setup.py` & `hdsr_fewspy-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.5"
+version = "1.6"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

