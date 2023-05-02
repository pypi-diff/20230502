# Comparing `tmp/fastf1-2.3.3.tar.gz` & `tmp/fastf1-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-2.3.3.tar", last modified: Sat Apr 29 11:23:21 2023, max compression
+gzip compressed data, was "fastf1-3.0.0.tar", last modified: Tue May  2 20:43:31 2023, max compression
```

## Comparing `fastf1-2.3.3.tar` & `fastf1-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 11:23:10.000000 fastf1-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 11:23:10.000000 fastf1-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-29 11:23:21.499235 fastf1-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-29 11:23:10.000000 fastf1-2.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70728 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   118447 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/ergast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30500 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 11:23:10.000000 fastf1-2.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 11:23:21.499235 fastf1-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 11:23:10.000000 fastf1-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 20:43:19.000000 fastf1-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 20:43:19.000000 fastf1-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-02 20:43:31.091595 fastf1-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 20:43:19.000000 fastf1-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132755 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-02 20:43:31.000000 fastf1-3.0.0/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 20:43:19.000000 fastf1-3.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-02 20:43:31.091595 fastf1-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 20:43:19.000000 fastf1-3.0.0/setup.py
```

### Comparing `fastf1-2.3.3/LICENSE` & `fastf1-3.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 theOehrly
+Copyright (c) 2023 Philipp Schäfer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastf1-2.3.3/fastf1/__init__.py` & `fastf1-3.0.0/fastf1/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,66 +18,87 @@
     fastf1.get_testing_session
     fastf1.get_event
     fastf1.get_events_remaining
     fastf1.get_testing_session
     fastf1.get_event_schedule
 
 
-Caching
--------
+.. _requests-and-caching:
 
-Caching should almost always be enabled to speed up the runtime of your
-scripts and to prevent exceeding the rate limit of api servers.
-FastF1 will print an annoyingly obnoxious warning message if you do not
-enable caching.
-
-The following class-level functions are used to setup, enable and
-(temporarily) disable caching.
-
-.. autosummary::
-    fastf1.Cache.enable_cache
-    fastf1.Cache.clear_cache
-    fastf1.Cache.disabled
-    fastf1.Cache.set_disabled
-    fastf1.Cache.set_enabled
+Requests and Caching
+--------------------
+
+.. automodule::
+    fastf1.req
+
+.. currentmodule:: fastf1
 
 
 General Functions - API Reference
 ---------------------------------
 
-Events API
-..........
+Event and Session API
+.....................
 
 .. autofunction:: get_session
 .. autofunction:: get_testing_session
 .. autofunction:: get_event
 .. autofunction:: get_events_remaining
 .. autofunction:: get_testing_event
 .. autofunction:: get_event_schedule
 
 Cache API
 .........
 
 .. autoclass:: Cache
-    :members: enable_cache, clear_cache, disabled, set_disabled, set_enabled
+    :members: enable_cache, clear_cache, disabled, set_disabled, set_enabled,
+        offline_mode
     :autosummary:
 
+
+Configure Logging Verbosity
+...........................
+
+All parts of FastF1 generally log at the log level 'INFO'.
+The reason for this is that many data loading processes take multiple
+seconds to complete. Logging is used to give progress information here as well
+as for showing warnings and non-terminal errors.
+
+The logging level for FastF1 can be easily customized::
+
+    import fastf1
+
+    fastf1.set_log_level('WARNING')
+
+    # ... your code  here ... #
+
+The available levels are (in order of increasing severity): DEBUG, INFO,
+WARNING, ERROR and CRITICAL.
+
+.. autofunction:: set_log_level
+
+For more information see :ref:`logging`.
+
 """
+from typing import Dict
+
 from fastf1.events import (get_session,  # noqa: F401
                            get_testing_session,
                            get_event,
                            get_events_remaining,
                            get_testing_event,
                            get_event_schedule)
 
-from fastf1.api import Cache  # noqa: F401
+from fastf1.logger import set_log_level  # noqa: F401
+
+from fastf1.req import Cache, RateLimitExceededError   # noqa: F401
 from fastf1.version import __version__   # noqa: F401
 
 
-_DRIVER_TEAM_MAPPING = {
+_DRIVER_TEAM_MAPPING: Dict[str, Dict[str, str]] = {
     # only necessary when loading live timing data that does not include
     # the driver and team listing and no data is available on ergast yet
     '23': {'Abbreviation': 'ALB', 'FirstName': 'Alexander',
            'LastName': 'Albon', 'TeamName': 'Williams'},
     '14': {'Abbreviation': 'ALO', 'FirstName': 'Fernando',
            'LastName': 'Alonso', 'TeamName': 'Alpine F1 Team'},
     '77': {'Abbreviation': 'BOT', 'FirstName': 'Valtteri',
```

### Comparing `fastf1-2.3.3/fastf1/api.py` & `fastf1-3.0.0/fastf1/_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,397 +1,58 @@
-"""
-Api Functions - :mod:`fastf1.api`
-=================================
-
-.. note:: The functions listed here are primarily for internal use within
-    FastF1. While you can use these functions directly, it is usually
-    better to use the functionality provided by the data objects
-    in :mod:`fastf1.core` instead.
-
-A collection of functions to interface with the F1 web api.
-
-.. autosummary::
-   :nosignatures:
-
-   timing_data
-   timing_app_data
-   car_data
-   position_data
-   track_status_data
-   session_status_data
-   race_control_messages
-   driver_info
-   weather_data
-   fetch_page
-   parse
-
-"""
 import base64
 import datetime
-import functools
 import json
-import logging
-import os
-import pickle
 import zlib
+from typing import Dict
 
 import numpy as np
 import pandas as pd
-import requests
-import requests_cache
 
+from fastf1.logger import get_logger, soft_exceptions
+from fastf1.req import Cache
 from fastf1.utils import recursive_dict_get, to_timedelta, to_datetime
 
+_logger = get_logger('api')
 
 base_url = 'https://livetiming.formula1.com'
 
-headers = {
-  'Host': 'livetiming.formula1.com',
-  'Connection': 'close',
-  'TE': 'identity',
-  'User-Agent': 'BestHTTP',
-  'Accept-Encoding': 'gzip, identity',
+headers: Dict[str, str] = {
+    'Host': 'livetiming.formula1.com',
+    'Connection': 'close',
+    'TE': 'identity',
+    'User-Agent': 'BestHTTP',
+    'Accept-Encoding': 'gzip, identity',
 }
 
-pages = {
-  'session_data': 'SessionData.json',  # track + session status + lap count
-  'session_info': 'SessionInfo.json',  # more rnd
-  'archive_status': 'ArchiveStatus.json',  # rnd=1880327548
-  'heartbeat': 'Heartbeat.jsonStream',  # Probably time synchronization?
-  'audio_streams': 'AudioStreams.jsonStream',  # Link to audio commentary
-  'driver_list': 'DriverList.jsonStream',  # Driver info and line story
-  'extrapolated_clock': 'ExtrapolatedClock.jsonStream',  # Boolean
-  'race_control_messages': 'RaceControlMessages.json',  # Flags etc
-  'session_status': 'SessionStatus.jsonStream',  # Start and finish times
-  'team_radio': 'TeamRadio.jsonStream',  # Links to team radios
-  'timing_app_data': 'TimingAppData.jsonStream',  # Tyres and laps (juicy)
-  'timing_stats': 'TimingStats.jsonStream',  # 'Best times/speed' useless
-  'track_status': 'TrackStatus.jsonStream',  # SC, VSC and Yellow
-  'weather_data': 'WeatherData.jsonStream',  # Temp, wind and rain
-  'position': 'Position.z.jsonStream',  # Coordinates, not GPS? (.z)
-  'car_data': 'CarData.z.jsonStream',  # Telemetry channels (.z)
-  'content_streams': 'ContentStreams.jsonStream',  # Lap by lap feeds
-  'timing_data': 'TimingData.jsonStream',  # Gap to car ahead
-  'lap_count': 'LapCount.jsonStream',  # Lap counter
-  'championship_prediction': 'ChampionshipPrediction.jsonStream'  # Points
+pages: Dict[str, str] = {
+    'session_data': 'SessionData.json',  # track + session status + lap count
+    'session_info': 'SessionInfo.json',  # more rnd
+    'archive_status': 'ArchiveStatus.json',  # rnd=1880327548
+    'heartbeat': 'Heartbeat.jsonStream',  # Probably time synchronization?
+    'audio_streams': 'AudioStreams.jsonStream',  # Link to audio commentary
+    'driver_list': 'DriverList.jsonStream',  # Driver info and line story
+    'extrapolated_clock': 'ExtrapolatedClock.jsonStream',  # Boolean
+    'race_control_messages': 'RaceControlMessages.jsonStream',  # Flags etc
+    'session_status': 'SessionStatus.jsonStream',  # Start and finish times
+    'team_radio': 'TeamRadio.jsonStream',  # Links to team radios
+    'timing_app_data': 'TimingAppData.jsonStream',  # Tyres and laps (juicy)
+    'timing_stats': 'TimingStats.jsonStream',  # 'Best times/speed' useless
+    'track_status': 'TrackStatus.jsonStream',  # SC, VSC and Yellow
+    'weather_data': 'WeatherData.jsonStream',  # Temp, wind and rain
+    'position': 'Position.z.jsonStream',  # Coordinates, not GPS? (.z)
+    'car_data': 'CarData.z.jsonStream',  # Telemetry channels (.z)
+    'content_streams': 'ContentStreams.jsonStream',  # Lap by lap feeds
+    'timing_data': 'TimingData.jsonStream',  # Gap to car ahead
+    'lap_count': 'LapCount.jsonStream',  # Lap counter
+    'championship_prediction': 'ChampionshipPrediction.jsonStream',  # Points
+    'index': 'Index.json'
 }
 """Known API requests"""
 
 
-class Cache:
-    """Pickle and requests based API cache.
-
-    The parsed API data will be saved as a pickled object.
-    Raw GET requests are cached in a sqlite db using the 'requests-cache'
-    module.
-
-    Caching should almost always be enabled to speed up the runtime of your
-    scripts and to prevent exceeding the rate limit of api servers.
-    FastF1 will print an annoyingly obnoxious warning message if you do not
-    enable caching.
-
-    The cache has two "stages".
-
-        - Stage 1: Caching of raw GET requests. This works for all requests.
-          Cache control is employed to refresh the cached data periodically.
-        - Stage 2: Caching of the parsed data. This saves a lot of time when
-          running your scripts,  as parsing of the data is computationally
-          expensive. Stage 2 caching is only used for some api functions.
-
-    Most commonly, you will enable caching right at the beginning of your script:
-
-        >>> import fastf1
-        >>> fastf1.Cache.enable_cache('path/to/cache')  # doctest: +SKIP
-        # change cache directory to an exisitng empty directory on your machine
-        >>> session = fastf1.get_session(2021, 5, 'Q')
-        >>> # ...
-
-    Note that you should always enable caching except for very rare
-    circumstances which are usually limited to doing core developement
-    on FastF1.
-    """
-    _CACHE_DIR = ''
-    # version of the api parser code (unrelated to release version number)
-    _API_CORE_VERSION = 7
-    _IGNORE_VERSION = False
-    _FORCE_RENEW = False
-
-    _requests_session = None
-    _has_been_warned = False  # flag to ensure that warning about disabled cache is logged once only
-    _tmp_disabled = False
-
-    @classmethod
-    def enable_cache(cls, cache_dir, ignore_version=False, force_renew=False, use_requests_cache=True):
-        """Enables the API cache.
-
-        Args:
-            cache_dir (str): Path to the directory which should be used to store cached data. Path needs to exist.
-            ignore_version (bool): Ignore if cached data was create with a different version of the API parser
-                (not recommended: this can cause crashes or unrecognized errors as incompatible data may be loaded)
-            force_renew (bool): Ignore existing cached data. Download data and update the cache instead.
-            use_requests_cache (bool): Do caching of the raw GET and POST requests.
-        """
-        # Allow users to use paths such as ~user or ~/
-        cache_dir = os.path.expanduser(cache_dir)
-
-        if not os.path.exists(cache_dir):
-            raise NotADirectoryError("Cache directory does not exist! Please check for typos or create it first.")
-        cls._CACHE_DIR = cache_dir
-        cls._IGNORE_VERSION = ignore_version
-        cls._FORCE_RENEW = force_renew
-        if use_requests_cache:
-            cls._requests_session = requests_cache.CachedSession(
-                cache_name=os.path.join(cache_dir, 'fastf1_http_cache'),
-                backend='sqlite',
-                allowable_methods=('GET', 'POST'),
-                expire_after=datetime.timedelta(hours=12),
-                cache_control=True,
-                stale_if_error=True
-            )
-            if force_renew:
-                cls._requests_session.cache.clear()
-
-    @classmethod
-    def requests_get(cls, *args, **kwargs):
-        """Wraps `requests.Session().get()` with caching if enabled.
-
-        All GET requests that require caching should be performed through this
-        wrapper. Caching will be done if the module-wide cache has been
-        enabled. Else, `requests.Session().get()` will be called without any
-        caching.
-        """
-        cls._show_not_enabled_warning()
-        if (cls._requests_session is None) or cls._tmp_disabled:
-            return requests.get(*args, **kwargs)
-        return cls._requests_session.get(*args, **kwargs)
-
-    @classmethod
-    def requests_post(cls, *args, **kwargs):
-        """Wraps `requests.Session().post()` with caching if enabled.
-
-        All POST requests that require caching should be performed through this
-        wrapper. Caching will be done if the module-wide cache has been
-        enabled. Else, `requests.Session().get()` will be called without any
-        caching.
-        """
-        cls._show_not_enabled_warning()
-        if (cls._requests_session is None) or cls._tmp_disabled:
-            return requests.post(*args, **kwargs)
-        return cls._requests_session.post(*args, **kwargs)
-
-    @classmethod
-    def clear_cache(cls, cache_dir, deep=False):
-        """Clear all cached data.
-
-        This deletes all cache files in the provided cache directory.
-        Optionally, the requests cache is cleared too.
-
-        Can be called without enabling the cache first.
-
-        Deleting specific events or sessions is not supported but can be done manually (stage 2 cache).
-        The cached data is structured by year, event and session. The structure is more or less self-explanatory.
-        To delete specific events or sessions delete the corresponding folder within the cache directory.
-        Deleting specific requests from the requests cache (stage 1) is not possible. To delete the requests cache only,
-        delete the sqlite file in the root of the cache directory.
-
-        Args:
-            cache_dir (str): Path to the directory which is used to store cached data.
-            deep (bool): Clear the requests cache (stage 1) too.
-        """
-        if not os.path.exists(cache_dir):
-            raise NotADirectoryError("Cache directory does not exist!")
-
-        for dirpath, dirnames, filenames in os.walk(cache_dir):
-            for filename in filenames:
-                if filename.endswith('.ff1pkl'):
-                    os.remove(os.path.join(dirpath, filename))
-
-        if deep:
-            if not hasattr(requests.Session(), 'cache'):
-                cls._install_requests_cache(cache_dir)
-            requests_cache.clear()
-
-    @classmethod
-    def api_request_wrapper(cls, func):
-        """Wrapper function for adding stage 2 caching to api functions.
-
-        Args:
-            func: function to be wrapped
-
-        Returns:
-            The wrapped function
-        """
-        @functools.wraps(func)
-        def _cached_api_request(api_path, response=None, livedata=None):
-            if cls._CACHE_DIR and not cls._tmp_disabled:
-                # caching is enabled
-                func_name = str(func.__name__)
-                cache_file_path = cls._get_cache_file_path(api_path, func_name)
-
-                if os.path.isfile(cache_file_path):
-                    # file exists already, try to load it
-                    try:
-                        cached = pickle.load(open(cache_file_path, 'rb'))
-                    except:  # noqa: E722 (bare except)
-                        # don't like the bare exception clause but who knows
-                        # which dependency will raise which internal exception
-                        # after it was updated
-                        cached = None
-
-                    if cached is not None and cls._data_ok_for_use(cached):
-                        # cached data is ok for use, return it
-                        logging.info(f"Using cached data for {func_name}")
-                        return cached['data']
-
-                    else:
-                        # cached data needs to be downloaded again and updated
-                        logging.info(f"Updating cache for {func_name}...")
-                        data = func(
-                            api_path, response=response, livedata=livedata
-                        )
-
-                        if data is not None:
-                            cls._write_cache(data, cache_file_path)
-                            logging.info("Cache updated!")
-                            return data
-
-                        logging.critical(
-                            "A cache update is required but the data failed "
-                            "to download. Cannot continue!\nYou may force to "
-                            "ignore a cache version mismatch by using the "
-                            "`ignore_version=True` keyword when enabling the "
-                            "cache (not recommended)."
-                        )
-                        exit()
-
-                else:  # cached data does not yet exist for this api request
-                    logging.info(f"No cached data found for {func_name}. "
-                                 f"Loading data...")
-                    data = func(
-                        api_path, response=response, livedata=livedata
-                    )
-                    if data is not None:
-                        cls._write_cache(data, cache_file_path)
-                        logging.info("Data has been written to cache!")
-                        return data
-
-                    logging.critical("Failed to load data!")
-                    exit()
-
-            else:  # cache was not enabled
-                if not cls._tmp_disabled:
-                    cls._show_not_enabled_warning()
-                return func(api_path, response=response, livedata=livedata)
-
-        return _cached_api_request
-
-    @classmethod
-    def _get_cache_file_path(cls, api_path, name):
-        # extend the cache dir path using the api path and a file name
-        # leading '/static/' is dropped form api path
-        cache_dir_path = os.path.join(cls._CACHE_DIR, api_path[8:])
-        if not os.path.exists(cache_dir_path):
-            # create subfolders if they don't yet exist
-            os.makedirs(cache_dir_path)
-
-        file_name = name + '.ff1pkl'
-        cache_file_path = os.path.join(cache_dir_path, file_name)
-        return cache_file_path
-
-    @classmethod
-    def _data_ok_for_use(cls, cached):
-        # check if cached data is ok or needs to be downloaded again
-        if cls._FORCE_RENEW:
-            return False
-        elif cls._IGNORE_VERSION:
-            return True
-        elif cached['version'] == cls._API_CORE_VERSION:
-            return True
-        return False
-
-    @classmethod
-    def _write_cache(cls, data, cache_file_path, **kwargs):
-        new_cached = dict(
-            **{'version': cls._API_CORE_VERSION, 'data': data},
-            **kwargs
-        )
-        with open(cache_file_path, 'wb') as cache_file_obj:
-            pickle.dump(new_cached, cache_file_obj)
-
-    @classmethod
-    def _show_not_enabled_warning(cls):
-        if not cls._CACHE_DIR and not cls._has_been_warned:
-            # warn only once and only if cache is not enabled
-            logging.warning(
-                "\n\nNO CACHE! Api caching has not been enabled! \n\t"
-                "It is highly recommended to enable this feature for much "
-                "faster data loading!\n\t"
-                "Use `fastf1.Cache.enable_cache('path/to/cache/')`\n")
-
-            cls._has_been_warned = True
-
-    @classmethod
-    def disabled(cls):
-        """Returns a context manager object that creates a context within
-        which the cache is temporarily disabled.
-
-        Example::
-
-            with Cache.disabled():
-                # no caching takes place here
-                ...
-
-        .. note::
-            The context manager is not multithreading-safe
-        """
-        return _NoCacheContext()
-
-    @classmethod
-    def set_disabled(cls):
-        """Disable the cache while keeping the configuration intact.
-
-        This disables stage 1 and stage 2 caching!
-
-        You can enable the cache at any time using :func:`set_enabled`
-
-        .. note:: You may prefer to use :func:`disabled` to get a context
-            manager object and disable the cache only within a specific
-            context.
-
-        .. note::
-            This function is not multithreading-safe
-        """
-        cls._tmp_disabled = True
-
-    @classmethod
-    def set_enabled(cls):
-        """Enable the cache after it has been disabled with
-        :func:`set_disabled`.
-
-        .. warning::
-            To enable the cache it needs to be configured properly. You need
-            to call :func`enable_cache` once to enable the cache initially.
-            :func:`set_enabled` and :func:`set_disabled` only serve to
-            (temporarily) disable the cache for specific parts of code that
-            should be run without caching.
-
-        .. note::
-            This function is not multithreading-safe
-        """
-        cls._tmp_disabled = False
-
-
-class _NoCacheContext:
-    def __enter__(self):
-        Cache.set_disabled()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        Cache.set_enabled()
-
-
 def make_path(wname, wdate, sname, sdate):
     """Create the api path base string to append on livetiming.formula1.com for api
     requests.
 
     The api path base string changes for every session only.
 
     Args:
@@ -419,15 +80,20 @@
 
 EMPTY_STREAM = {'Time': pd.NaT, 'Driver': str(), 'Position': np.NaN,
                 'GapToLeader': np.NaN, 'IntervalToPositionAhead': np.NaN}
 
 
 @Cache.api_request_wrapper
 def timing_data(path, response=None, livedata=None):
-    """Fetch and parse timing data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse timing data.
 
     Timing data is a mixed stream of information. At a given time a packet of data may indicate position, lap time,
     speed trap, sector times and so on.
 
     While most of this data can be mapped lap by lap giving a readable and usable data structure (-> laps_data),
     other entries like position and time gaps are provided on a more frequent time base. Those values are separated
     and returned as a separate object (-> stream_data).
@@ -487,22 +153,22 @@
     # possible optional sanity checks (TODO, maybe):
     #   - inlap has to be followed by outlap
     #   - pit stops may never be negative (missing outlap)
     #   - speed traps against telemetry (especially in Q FastLap - Slow Lap)
     if livedata is not None and livedata.has('TimingData'):
         response = livedata.get('TimingData')
     elif response is None:  # no previous response provided
-        logging.info("Fetching timing data...")
+        _logger.info("Fetching timing data...")
         response = fetch_page(path, 'timing_data')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
-    logging.info("Parsing timing data...")
+    _logger.info("Parsing timing data...")
 
     # split up response per driver for easier iteration and processing later
     resp_per_driver = dict()
     for entry in response:
         if (len(entry) < 2) or 'Lines' not in entry[1]:
             continue
         for drv in entry[1]['Lines']:
@@ -515,28 +181,113 @@
     laps_data = {key: list() for key, val in EMPTY_LAPS.items()}
     stream_data = {key: list() for key, val in EMPTY_STREAM.items()}
 
     for drv in resp_per_driver.keys():
         drv_laps_data = _laps_data_driver(resp_per_driver[drv], EMPTY_LAPS, drv)
         drv_stream_data = _stream_data_driver(resp_per_driver[drv], EMPTY_STREAM, drv)
 
+        if (drv_laps_data is None) or (drv_stream_data is None):
+            continue
+
         for key in EMPTY_LAPS.keys():
             laps_data[key].extend(drv_laps_data[key])
 
         for key in EMPTY_STREAM.keys():
             stream_data[key].extend(drv_stream_data[key])
 
     laps_data = pd.DataFrame(laps_data)
     stream_data = pd.DataFrame(stream_data)
 
+    _align_laps(laps_data, stream_data)
+
+    # pandas doesn't correctly infer bool dtype columns, set type explicitly
+    laps_data[['IsPersonalBest']] = laps_data[['IsPersonalBest']].astype(bool)
+
     return laps_data, stream_data
 
 
+@soft_exceptions("lap alignment",
+                 "Failed to align laps between drivers!",
+                 logger=_logger)
+def _align_laps(laps_data, stream_data):
+    # align lap start and end times between drivers based on Gap to leader
+    if not pd.isnull(stream_data['GapToLeader']).all():
+        expected_gap = dict()
+        delta = dict()
+        leader = None
+        max_delta = None
+
+        # try to align on the first lap where useable data is available
+        # ideally, this is the end of the first lap
+        offset = -1  # start at -1 so that value it is zero on first iteration
+
+        while leader is None:
+            offset += 1
+            # find the leader after the first useable lap and get the expected
+            # gaps to the leader for all other drivers
+            for drv in laps_data['Driver'].unique():
+                try:
+                    gap_str = _get_gap_str_for_drv(drv, offset, laps_data,
+                                                   stream_data)
+                    if 'LAP' in gap_str:
+                        leader = drv
+                    else:
+                        expected_gap[drv] = to_timedelta(gap_str)
+                except IndexError:
+                    expected_gap[drv] = None
+
+        # find the greatest delta between actual gap and currently calculated
+        # gap
+        leader_time \
+            = laps_data[laps_data['Driver'] == leader].iloc[offset]['Time']
+
+        for drv in expected_gap.keys():
+            if expected_gap[drv] is None:
+                delta[drv] = None
+                continue
+
+            other_time \
+                = laps_data[laps_data['Driver'] == drv].iloc[offset]['Time']
+            is_gap = other_time - leader_time
+            delta[drv] = expected_gap[drv] - is_gap
+            if (max_delta is None) or (delta[drv] > max_delta):
+                max_delta = delta[drv]
+
+        # Subtract the maximum delta from all leader timestamps.
+        # It is impossible that the data was received too early, which in turn
+        # means that it must have been received too late if the delta is
+        # greater than zero
+        if max_delta > datetime.timedelta(0):
+            max_delta = datetime.timedelta(0)
+        laps_data.loc[laps_data['Driver'] == leader, 'Time'] -= max_delta
+
+        # Subtract the delta between actual gap and currently calculated gap
+        # from each drivers timestamps to align them. Correct for the max
+        # delta shift of the timestamps of the leader.
+        for drv in delta.keys():
+            if delta[drv] is None:
+                continue
+            laps_data.loc[laps_data['Driver'] == drv, 'Time'] \
+                -= (max_delta - delta[drv])
+
+
+def _get_gap_str_for_drv(drv, idx, laps_data, stream_data):
+    first_time = laps_data[laps_data['Driver'] == drv].iloc[idx]['Time']
+    ref_idx = (stream_data[stream_data['Driver'] == drv]['Time']
+               - first_time).abs().idxmin()
+    gap_str = stream_data.loc[ref_idx]['GapToLeader']
+    return gap_str
+
+
 def _laps_data_driver(driver_raw, empty_vals, drv):
     """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
     Data is on a per-lap basis.
 
     Boolean flag 'PitOut' is not evaluated. Meaning is unknown and flag is only sometimes present when a car leaves
     the pits.
 
     Params:
         driver_raw (list): raw api response for this driver only [(Timestamp, data), (...), ...]
@@ -564,16 +315,18 @@
 
     for time, resp in driver_raw:
         # the first three ifs are just edge case handling for the rare sessions were the data goes back in time
         if in_past and 'NumberOfLaps' in resp and resp['NumberOfLaps'] == api_lapcnt:
             in_past = False  # we're back in the present
 
         if 'NumberOfLaps' in resp and ((prev_lapcnt := resp['NumberOfLaps']) < api_lapcnt):
-            logging.warning(f"Driver {drv: >2}: Ignoring late data for a previously processed lap."
-                            f"The data may contain errors (previous: {prev_lapcnt}; current {lapcnt})")
+            _logger.warning(f"Driver {drv: >2}: Ignoring late data for a "
+                            f"previously processed lap.The data may contain "
+                            f"errors (previous: {prev_lapcnt}; "
+                            f"current {lapcnt})")
             in_past = True
             continue
 
         if in_past:  # still in the past, just continue and ignore everything
             continue
 
         if ('InPit' in resp) and (resp['InPit'] is False):
@@ -593,15 +346,15 @@
     # now, do the main pass where all the other data is actually filled in
     # same counters and flags as before, reset them
     lapcnt = 0  # we're keeping two separate lap counts because sometimes the api has a non existent lap too much...
     api_lapcnt = 0  # ...at the beginning; we can correct that though;
     # api_lapcnt does not count backwards even if the source data does
     in_past = False  # flag for when the data went back in time
 
-    personal_best_lap_time = None
+    personal_best_lap_times = list()
 
     pitstops = -1  # start with -1 because first is out lap, needs to be zero after that
 
     # iterate through the data; new lap triggers next row in data
     for time, resp in driver_raw:
         # the first three ifs are just edge case handling for the rare sessions were the data goes back in time
         if in_past and 'NumberOfLaps' in resp and resp['NumberOfLaps'] == api_lapcnt:
@@ -656,38 +409,40 @@
 
         if 'InPit' in resp:
             # 'InPit': True is received once when entering pits, False is received once when leaving
             if resp['InPit'] is True:
                 if pitstops >= 0:
                     drv_data['PitInTime'][lapcnt] = to_timedelta(time)
             elif ((('NumberOfLaps' in resp) and resp['NumberOfLaps'] > api_lapcnt)
-                  or (drv_data['Time'][lapcnt] - to_timedelta(time)) < pd.Timedelta(5, 's')):
-                # same response line as beginning of next lap or beginning of next lap less than 5 seconds away
-                drv_data['PitOutTime'][lapcnt+1] = to_timedelta(time)  # add to next lap
+                  or (drv_data['Time'][lapcnt] - to_timedelta(time))
+                  < pd.Timedelta(5, 's')):
+                # same response line as beginning of next lap
+                # or beginning of next lap less than 5 seconds away
+                drv_data['PitOutTime'][lapcnt + 1] = to_timedelta(time)  # add to next lap
                 pitstops += 1
             else:
                 drv_data['PitOutTime'][lapcnt] = to_timedelta(time)  # add to current lap
                 pitstops += 1
 
         if val := recursive_dict_get(resp, 'BestLapTime', 'Value'):
-            personal_best_lap_time = to_timedelta(val)
+            personal_best_lap_times.append(to_timedelta(val))
 
         # new lap; create next row
         if 'NumberOfLaps' in resp and resp['NumberOfLaps'] > api_lapcnt:
             api_lapcnt += 1
             # make sure the car actually drove out of the pits already; it can't be a new lap if it didn't
             if pitstops >= 0:
                 drv_data['Time'][lapcnt] = to_timedelta(time)
                 drv_data['NumberOfLaps'][lapcnt] = lapcnt + 1  # don't use F1's lap count; ours is better
                 drv_data['NumberOfPitStops'][lapcnt] = pitstops
                 drv_data['Driver'][lapcnt] = drv
                 lapcnt += 1
 
     if lapcnt == 0:  # no data at all for this driver
-        return drv_data
+        return None
 
     # done reading the data, do postprocessing
 
     def data_in_lap(lap_n):
         relevant = ('Sector1Time', 'Sector2Time', 'Sector3Time', 'SpeedI1', 'SpeedI2',
                     'SpeedFL', 'SpeedST', 'LapTime')
         for col in relevant:
@@ -698,38 +453,72 @@
     # 'NumberOfLaps' always introduces a new lap (can be a previous one) but sometimes there is one more lap at the end
     # in this case the data will be added as usual above, lap count and pit stops are added here and the 'Time' is
     # calculated below from sector times
     if data_in_lap(lapcnt):
         drv_data['NumberOfLaps'][lapcnt] = lapcnt + 1
         drv_data['NumberOfPitStops'][lapcnt] = pitstops
         drv_data['Driver'][lapcnt] = drv
-    else:  # if there was no more data after the last lap count increase, delete the last empty record
+    else:  # if there was no more data after the last lap count increase,
+        # delete the last empty record
         for key in drv_data.keys():
             drv_data[key] = drv_data[key][:-1]
-    if not data_in_lap(0):  # remove first lap if there's no data; "pseudo outlap" that didn't exist
+    if not data_in_lap(0):  # remove first lap if there's no data;
+        # "pseudo outlap" that didn't exist
         for key in drv_data.keys():
             drv_data[key] = drv_data[key][1:]
-        drv_data['NumberOfLaps'] = list(map(lambda n: n-1, drv_data['NumberOfLaps']))  # reduce each lap count by one
+        drv_data['NumberOfLaps'] = list(map(lambda n: n - 1, drv_data['NumberOfLaps']))  # reduce each lap count by one
 
     if not drv_data['Time']:
         # ensure that there is still data left after potentially removing a lap
         return drv_data
 
-    # check for incorrect lap times and remove them
-    # fixes GH#167 among others
     for i in range(len(drv_data['Time'])):
         sector_sum = datetime.timedelta(0)
+        na_sectors = list()  # list of keys for missing sector times
         for key in ('Sector1Time', 'Sector2Time', 'Sector3Time'):
             st = drv_data[key][i]
             if pd.isna(st):
+                na_sectors.append(key)
                 continue
             sector_sum += st
+
+        # check for incorrect lap times and remove them
+        # fixes GH#167 among others
         if sector_sum > drv_data['LapTime'][i]:
             drv_data['LapTime'][i] = pd.NaT
-            integrity_errors.append(i+1)
+            integrity_errors.append(i + 1)
+
+        if i == 0:
+            # only do following corrections for 2nd lap and onwards
+            continue
+
+        # The API only sends and update if a state changes, therefore, if two
+        # lap times or sector times are exactly equal, the second value will
+        # be missing. Missing sector times and lap times are calculated here
+        # based on the available values for a lap (max one may be missing). If
+        # the calculated value matches the previous value, it will be set.
+
+        # lap time is missing
+        if (not na_sectors) and pd.isna(drv_data['LapTime'][i]) \
+                and (drv_data['LapTime'][i - 1] == sector_sum):
+
+            drv_data['LapTime'][i] = sector_sum
+
+        # one sector time is missing
+        elif (len(na_sectors) == 1) and not pd.isna(drv_data['LapTime'][i]):
+            # create a list with the two keys for available sector times
+            ref_sec = ['Sector1Time', 'Sector2Time', 'Sector3Time']
+            ref_sec.remove(na_sectors[0])
+
+            if (sec1 := (drv_data['LapTime'][i]
+                         - drv_data[ref_sec[0]][i]
+                         - drv_data[ref_sec[1]][i])) \
+                    == drv_data[na_sectors[0]][i - 1]:
+
+                drv_data[na_sectors[0]][i] = sec1
 
     # lap time sync; check which sector time was triggered with the lowest latency
     # Sector3SessionTime == end of lap
     # Sector2SessionTime + Sector3Time == end of lap
     # Sector1SessionTime + Sector2Time + Sector3Time == end of lap
     # all of these three have slightly different times; take earliest one -> most exact because can't trigger too early
     for i in range(len(drv_data['Time'])):
@@ -743,16 +532,16 @@
             if pd.isnull(sector_time):
                 break  # need to stop here because else the sector sum will be incorrect
 
             sector_sum += sector_time
             new_time = session_time + sector_sum
             if not pd.isnull(new_time) and (new_time < min_time or pd.isnull(min_time)):
                 min_time = new_time
-        if i > 0 and min_time < drv_data['Time'][i-1]:
-            integrity_errors.append(i+1)  # not be possible if sector times and lap time are correct
+        if i > 0 and min_time < drv_data['Time'][i - 1]:
+            integrity_errors.append(i + 1)  # not be possible if sector times and lap time are correct
             continue
 
         drv_data['Time'][i] = min_time
 
     # last lap needs to be removed if it does not have a 'Time' and it could not be calculated (likely an inlap)
     if pd.isnull(drv_data['Time'][-1]):
         if not pd.isnull(drv_data['PitInTime'][-1]):
@@ -762,54 +551,91 @@
                 drv_data[key] = drv_data[key][:-1]
 
     if not drv_data['Time']:
         # ensure that there is still data left after potentially removing a lap
         return drv_data
 
     # more lap sync, this time check which lap triggered with the lowest latency
-    for i in range(len(drv_data['Time'])-1, 0, -1):
-        if (new_time := drv_data['Time'][i] - drv_data['LapTime'][i]) < drv_data['Time'][i-1]:
-            if i > 1 and new_time < drv_data['Time'][i-2]:
-                integrity_errors.append(i+1)  # not be possible if sector times and lap time are correct
+    for i in range(len(drv_data['Time']) - 1, 0, -1):
+        if (new_time := drv_data['Time'][i] - drv_data['LapTime'][i]) < \
+                drv_data['Time'][i - 1]:
+            if i > 1 and new_time < drv_data['Time'][i - 2]:
+                integrity_errors.append(i + 1)  # not be possible if sector times and lap time are correct
             else:
-                drv_data['Time'][i-1] = new_time
+                drv_data['Time'][i - 1] = new_time
 
     # need to go both directions once to make everything match up; also recalculate sector times
-    for i in range(len(drv_data['Time'])-1):
-        if any(pd.isnull(tst) for tst in (drv_data['Time'][i], drv_data['LapTime'][i+1], drv_data['Sector1Time'][i+1],
-                                          drv_data['Sector2Time'][i+1], drv_data['Sector3Time'][i+1])):
+    for i in range(len(drv_data['Time']) - 1):
+        if any(pd.isnull(tst) for tst in (
+                drv_data['Time'][i], drv_data['LapTime'][i + 1],
+                drv_data['Sector1Time'][i + 1],
+                drv_data['Sector2Time'][i + 1],
+                drv_data['Sector3Time'][i + 1])):
             continue  # lap not usable, missing critical values
 
-        if (new_time := drv_data['Time'][i] + drv_data['LapTime'][i+1]) < drv_data['Time'][i+1]:
+        if (new_time := drv_data['Time'][i] + drv_data['LapTime'][i+1]) \
+                < drv_data['Time'][i+1]:
             drv_data['Time'][i+1] = new_time
-        if (new_s1_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1]) < drv_data['Sector1SessionTime'][i+1]:
+        if (new_s1_time := drv_data['Time'][i]
+                + drv_data['Sector1Time'][i+1]) \
+                < drv_data['Sector1SessionTime'][i+1]:
             drv_data['Sector1SessionTime'][i+1] = new_s1_time
-        if (new_s2_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1] + drv_data['Sector2Time'][i+1]) < \
-                drv_data['Sector2SessionTime'][i+1]:
+        if (new_s2_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1]
+                + drv_data['Sector2Time'][i+1]) \
+                < drv_data['Sector2SessionTime'][i+1]:
             drv_data['Sector2SessionTime'][i+1] = new_s2_time
-        if (new_s3_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1] + drv_data['Sector2Time'][i+1] +
-                drv_data['Sector3Time'][i+1]) < drv_data['Sector3SessionTime'][i+1]:
+        if (new_s3_time := drv_data['Time'][i] + drv_data['Sector1Time'][i+1]
+                + drv_data['Sector2Time'][i+1]
+                + drv_data['Sector3Time'][i+1]) \
+                < drv_data['Sector3SessionTime'][i+1]:
             drv_data['Sector3SessionTime'][i+1] = new_s3_time
 
-    for i, time in enumerate(drv_data['LapTime']):
-        if time == personal_best_lap_time:
-            drv_data['IsPersonalBest'][i] = True
-            break
+    # iterate over list of personal lap times set 'IsPersonalBest'
+    # when a lap is deleted, the API resends the previous personal best.
+    # Therefore, by iterating in reverse, if any lap is encountered that is
+    # quicker than already processed personal best lap times, it must have
+    # been deleted.
+    _corrected_personal_best_lap_times = list()
+    # list is only used for backreference within the loop
+    for pb_lap_time in reversed(personal_best_lap_times):
+        if _corrected_personal_best_lap_times:
+            if pb_lap_time in _corrected_personal_best_lap_times:
+                continue
+            elif pb_lap_time < min(_corrected_personal_best_lap_times):
+                continue
+
+        _corrected_personal_best_lap_times.append(pb_lap_time)
+
+        # find the index of the corresponding lap by comparing with the lap
+        # times and set 'IsPersonalBest' to True for that lap
+        try:
+            pb_idx = drv_data['LapTime'].index(pb_lap_time)
+        except ValueError:
+            # one example case where this error occurs, are wildly of personal
+            # best times (>2 min lap time) that are sometimes present and
+            # which have no corresponding lap time
+            pass
+        else:
+            drv_data['IsPersonalBest'][pb_idx] = True
 
     if integrity_errors:
-        logging.warning(
+        _logger.warning(
             f"Driver {drv: >2}: Encountered {len(integrity_errors)} timing "
             f"integrity error(s) near lap(s): {integrity_errors}.\n"
             f"This might be a bug and should be reported.")
 
     return drv_data
 
 
 def _stream_data_driver(driver_raw, empty_vals, drv):
     """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
     Data is on a timestamp basis.
 
     Params:
         driver_raw (list): raw api response for this driver only [(Timestamp, data), (...), ...]
         empty_vals (dict): dictionary of column names and empty column values
         drv (str): driver identifier
 
@@ -849,15 +675,20 @@
         drv_data[key] = drv_data[key][:-1]  # remove very last row again
 
     return drv_data
 
 
 @Cache.api_request_wrapper
 def timing_app_data(path, response=None, livedata=None):
-    """Fetch and parse 'timing app data'.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse 'timing app data'.
 
     Timing app data provides the following data channels per sample:
        - LapNumber (float or nan): Current lap number
        - Driver (str): Driver number
        - LapTime (pandas.Timedelta or None): Lap time of last lap
        - Stint (int): Counter for the number of driven stints
        - TotalLaps (float or nan): Total number of laps driven on this set of tires (includes laps driven in
@@ -885,15 +716,15 @@
 
     Raises:
         SessionNotAvailableError: in case the F1 livetiming api returns no data
     """
     if livedata is not None and livedata.has('TimingAppData'):
         response = livedata.get('TimingAppData')
     elif response is None:  # no previous response provided
-        logging.info("Fetching timing app data...")
+        _logger.info("Fetching timing app data...")
         response = fetch_page(path, 'timing_app_data')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -920,26 +751,36 @@
                             elif key == 'New':
                                 val = True if val == 'true' else False
                             data[key].append(val)
                         else:
                             data[key].append(None)
                     for key in stint:
                         if key not in data:
-                            logging.debug(f"Found unknown key in timing app data: {key}")
+                            _logger.debug(f"Found unknown key in timing app "
+                                          f"data: {key}")
 
                     data['Time'][-1] = time
                     data['Driver'][-1] = driver_number
                     data['Stint'][-1] = stint_number
 
-    return pd.DataFrame(data)
+    df = pd.DataFrame(data)
+    # pandas doesn't correctly infer bool dtype columns, set type explicitly
+    df[['New', 'TyresNotChanged']] \
+        = df[['New', 'TyresNotChanged']].astype(bool)
+    return df
 
 
 @Cache.api_request_wrapper
 def car_data(path, response=None, livedata=None):
-    """Fetch and parse car data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse car data.
 
     Car data provides the following data channels per sample:
         - Time (pandas.Timedelta): session timestamp (time only); inaccurate, has duplicate values; use Date instead
         - Date (pandas.Timestamp): timestamp for this sample as Date + Time; more or less exact
         - Speed (int): Km/h
         - RPM (int)
         - Gear (int): [called 'nGear' in the data!]
@@ -978,23 +819,23 @@
     # data recorded from live timing has a slightly different structure
     is_livedata = False  # flag to indicate live timing data
 
     if livedata is not None and livedata.has('CarData.z'):
         response = livedata.get('CarData.z')
         is_livedata = True
     elif response is None:
-        logging.info("Fetching car data...")
+        _logger.info("Fetching car data...")
         response = fetch_page(path, 'car_data')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
-    logging.info("Parsing car data...")
+    _logger.info("Parsing car data...")
 
     channels = {'0': 'RPM', '2': 'Speed', '3': 'nGear', '4': 'Throttle', '5': 'Brake', '45': 'DRS'}
     num_channels = ['RPM', 'Speed', 'nGear', 'Throttle', 'DRS']
     bool_channels = ['Brake']
     columns = ['Time', 'Date', 'RPM', 'Speed', 'nGear', 'Throttle', 'Brake', 'DRS', 'Source']
     ts_length = 12  # length of timestamp: len('00:00:00:000')
 
@@ -1019,26 +860,27 @@
                     if driver not in data:
                         data[driver] = {col: list() for col in columns}
 
                     data[driver]['Time'].append(time)
                     data[driver]['Date'].append(date)
 
                     for n in channels:
-                        val = recursive_dict_get(entry, 'Cars', driver, 'Channels', n)
-                        if not val:
+                        try:
+                            val = entry['Cars'][driver]['Channels'][n]
+                        except (KeyError, IndexError):
                             val = 0
                         data[driver][channels[n]].append(int(val))
 
         except Exception:
             # too risky to specify an exception: unexpected invalid data!
             decode_error_count += 1
             continue
 
     if decode_error_count > 0:
-        logging.warning(f"Car data: failed to decode {decode_error_count} "
+        _logger.warning(f"Car data: failed to decode {decode_error_count} "
                         f"messages ({len(response)} messages total)")
 
     # create one dataframe per driver and check for the longest dataframe
     most_complete_ref = None
     for driver in data:
         # add source reference for each sample
         data[driver]['Source'] = ['car', ] * len(data[driver]['Date'])
@@ -1052,46 +894,50 @@
         # and no postprocessing is necessary
         if len(data[driver]['Date']) < len(most_complete_ref):
             # there is missing data for this driver
             # extend the Date column and fill up missing telemetry values with
             # zero, except Time which is left as NaT and will be calculated
             # correctly based on Session.t0_date anyways when creating Telemetry
             # instances in Session.load_telemetry
-            index_df = pd.DataFrame(data={'Date': most_complete_ref})
-            data[driver] = data[driver]\
-                .merge(index_df, how='outer')\
-                .sort_values(by='Date')\
+            data[driver] = data[driver] \
+                .merge(most_complete_ref, how='outer') \
+                .sort_values(by='Date') \
                 .reset_index(drop=True)
 
-            logging.warning(f"Driver {driver: >2}: Car data is incomplete!")
+            _logger.warning(f"Driver {driver: >2}: Car data is incomplete!")
 
         # ensure that brake data is 'boolean-compatible' in case that this is
         # ever changed
         _unique_brake_values = data[driver].loc[:, 'Brake'].unique()
         if ((_unique_brake_values > 0) & (_unique_brake_values < 100)).any():
-            logging.warning(f"Driver {driver: >2}: Raw brake data contains "
+            _logger.warning(f"Driver {driver: >2}: Raw brake data contains "
                             f"non-boolean values!")
 
         # convert to correct datatypes
-        data[driver].loc[:, num_channels] = data[driver] \
-            .loc[:, num_channels]\
-            .fillna(value=0, inplace=False)\
+        data[driver][num_channels] = \
+            data[driver].loc[:, num_channels] \
+            .fillna(value=0, inplace=False) \
             .astype('int64')
 
-        data[driver].loc[:, bool_channels] = data[driver] \
-            .loc[:, bool_channels]\
-            .fillna(value=False, inplace=False)\
+        data[driver][bool_channels] = \
+            data[driver].loc[:, bool_channels] \
+            .fillna(value=False, inplace=False) \
             .astype('bool')
 
     return data
 
 
 @Cache.api_request_wrapper
 def position_data(path, response=None, livedata=None):
-    """Fetch and parse position data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse position data.
 
     Position data provides the following data channels per sample:
         - Time (pandas.Timedelta): session timestamp (time only); inaccurate, has duplicate values; use Date instead
         - Date (pandas.Timestamp): timestamp for this sample as Date + Time; more or less exact
         - Status (str): 'OnTrack' or 'OffTrack'
         - X, Y, Z (int): Position coordinates; starting from 2020 the coordinates are given in 1/10 meter
         - Source (str): Indicates the source of a sample; 'pos' for all values here
@@ -1115,23 +961,23 @@
     # data recorded from live timing has a slightly different structure
     is_livedata = False  # flag to indicate live timing data
 
     if livedata is not None and livedata.has('Position.z'):
         response = livedata.get('Position.z')
         is_livedata = True
     elif response is None:
-        logging.info("Fetching position data...")
+        _logger.info("Fetching position data...")
         response = fetch_page(path, 'position')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
-    logging.info("Parsing position data...")
+    _logger.info("Parsing position data...")
 
     if not response:
         return {}
 
     ts_length = 12  # length of timestamp: len('00:00:00:000')
     columns = ['Time', 'Date', 'Status', 'X', 'Y', 'Z', 'Source']
 
@@ -1158,28 +1004,32 @@
 
                     data[driver]['Time'].append(time)
                     data[driver]['Date'].append(date)
 
                     for coord in ['X', 'Y', 'Z']:
                         data[driver][coord].append(recursive_dict_get(sample, 'Entries', driver, coord))
 
-                    status = recursive_dict_get(sample, 'Entries', driver, 'Status')
+                    try:
+                        status = sample['Entries'][driver]['Status']
+                    except KeyError:
+                        status = None
                     if str(status).isdigit():
                         # Fallback on older api status mapping and convert
                         status = 'OffTrack' if int(status) else 'OnTrack'
                     data[driver]['Status'].append(status)
 
         except Exception:
             # too risky to specify an exception: unexpected invalid data!
             decode_error_count += 1
             continue
 
     if decode_error_count > 0:
-        logging.warning(f"Position data: failed to decode {decode_error_count} "
-                        f"messages ({len(response)} messages total)")
+        _logger.warning(
+            f"Position data: failed to decode {decode_error_count} "
+            f"messages ({len(response)} messages total)")
 
     # create one dataframe per driver and check for the longest dataframe
     most_complete_ref = None
     for driver in data:
         data[driver]['Source'] = ['pos', ] * len(data[driver]['Date'])  # add source reference for each sample
         data[driver] = pd.DataFrame(data[driver])  # convert dict to dataframe
         # check length of dataframe; sometimes there can be missing data
@@ -1191,31 +1041,37 @@
         if len(data[driver]['Date']) < len(most_complete_ref):
             # there is missing data for this driver
             # extend the Date column and fill up missing telemetry values with
             # zero, except Time which is left as NaT and will be calculated
             # correctly based on Session.t0_date anyways when creating Telemetry
             # instances in Session.load_telemetry
             # and except Status which should be 'OffTrack' for missing data
-            index_df = pd.DataFrame(data={'Date': most_complete_ref})
-            data[driver] = data[driver]\
-                .merge(index_df, how='outer')\
-                .sort_values(by='Date')\
+            data[driver] = data[driver] \
+                .merge(most_complete_ref, how='outer') \
+                .sort_values(by='Date') \
                 .reset_index(drop=True)
             data[driver]['Status'].fillna(value='OffTrack', inplace=True)
-            data[driver].loc[:, ['X', 'Y', 'Z']] = data[driver]\
-                .loc[:, ['X', 'Y', 'Z']].fillna(value=0, inplace=False)
+            data[driver].loc[:, ['X', 'Y', 'Z']] = \
+                data[driver].loc[:, ['X', 'Y', 'Z']]\
+                .fillna(value=0, inplace=False)
 
-            logging.warning(f"Driver {driver: >2}: Position data is incomplete!")
+            _logger.warning(f"Driver {driver: >2}: Position data is "
+                            f"incomplete!")
 
     return data
 
 
 @Cache.api_request_wrapper
 def track_status_data(path, response=None, livedata=None):
-    """Fetch and parse track status data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse track status data.
 
     Track status contains information on yellow/red/green flags, safety car and virtual safety car. It provides the
     following data channels per sample:
 
         - Time (datetime.timedelta): session timestamp (time only)
         - Status (str): contains track status changes as numeric values (described below)
         - Message (str): contains the same information as status but in easily understandable
@@ -1243,18 +1099,18 @@
         A dictionary containing one key for each data channel and a list of values per key.
 
     Raises:
         SessionNotAvailableError: in case the F1 livetiming api returns no data
     """
     if livedata is not None and livedata.has('TrackStatus'):
         # does not need any further processing
-        logging.info("Loading track status data")
+        _logger.info("Loading track status data")
         return livedata.get('TrackStatus')
     elif response is None:
-        logging.info("Fetching track status data...")
+        _logger.info("Fetching track status data...")
         response = fetch_page(path, 'track_status')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -1271,15 +1127,20 @@
         data['Message'].append(row.get('Message', ''))
 
     return data
 
 
 @Cache.api_request_wrapper
 def session_status_data(path, response=None, livedata=None):
-    """Fetch and parse session status data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse session status data.
 
     Session status contains information on when a session was started and when it ended (amongst others). It
     provides the following data channels per sample:
 
         - Time (datetime.timedelta): session timestamp (time only)
         - Status (str): status messages
 
@@ -1294,18 +1155,18 @@
         A dictionary containing one key for each data channel and a list of values per key.
 
     Raises:
         SessionNotAvailableError: in case the F1 livetiming api returns no data
     """
     if livedata is not None and livedata.has('SessionStatus'):
         # does not need any further processing
-        logging.info("Loading session status data")
+        _logger.info("Loading session status data")
         return livedata.get('SessionStatus')
     elif response is None:
-        logging.info("Fetching session status data...")
+        _logger.info("Fetching session status data...")
         response = fetch_page(path, 'session_status')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -1322,15 +1183,20 @@
         data['Status'].append(row['Status'])
 
     return data
 
 
 @Cache.api_request_wrapper
 def race_control_messages(path, response=None, livedata=None):
-    """Fetch and parse race control messages.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse race control messages.
 
     Race control messages are sent by race control to all teams to notify of
     decisions and statuses of the session.
 
     Every message has the following attributes:
 
         - Utc: Message timestamp
@@ -1359,18 +1225,18 @@
         values per key.
 
     Raises:
         SessionNotAvailableError: in case the F1 livetiming api returns no data
     """
     if livedata is not None and livedata.has('RaceControlMessages'):
         # does not need any further processing
-        logging.info("Loading race control messages")
+        _logger.info("Loading race control messages")
         return livedata.get('RaceControlMessages')
     elif response is None:
-        logging.info("Fetching race control messages...")
+        _logger.info("Fetching race control messages...")
         response = fetch_page(path, 'race_control_messages')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -1378,30 +1244,103 @@
         'Time': [], 'Category': [], 'Message': [], 'Status': [],
         'Flag': [], 'Scope': [], 'Sector': [], 'RacingNumber': []
     }
     data_keys = ('Category', 'Message', 'Status', 'Flag', 'Scope', 'Sector',
                  'RacingNumber')
     converters = (str, str, str, str, str, int, str)
 
-    for entry in response['Messages']:
-        data['Time'].append(to_datetime(entry['Utc']))
+    for line in response:
+        messages = line[1]['Messages']
+        if isinstance(messages, dict):
+            messages = list(messages.values())
+        for entry in messages:
+            data['Time'].append(to_datetime(entry['Utc']))
+
+            for key, conv in zip(data_keys, converters):
+                try:
+                    data[key].append(conv(entry[key]))
+                except (KeyError, ValueError):
+                    # type conversion failed or key is missing
+                    data[key].append(None)
+
+    return data
+
+
+@Cache.api_request_wrapper
+def lap_count(path, response=None, livedata=None):
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse lap count data.
+
+    It provides the following data channels per sample:
+        - Time: session timestamp (time only)
+        - TotalLaps (int): Intended number of total laps
+        - CurrentLap (int): Current race lap
+
+    A value can have both 'TotalLaps' and 'CurrentLap' or only one of them.
+
+    A new value is sent every time a lap is completed or
+    the intended number of laps changes.
+
+    Args:
+        path (str): api path base string (usually ``Session.api_path``)
+        response: Response as returned by :func:`fetch_page` can be passed if
+            it was downloaded already.
+        livedata: An instance of
+            :class:`fastf1.livetiming.data.LiveTimingData` to use as a source
+            instead of the api
+
+    Returns:
+        A dictionary containing one key for each data channel and a list of
+        values per key.
+
+    Raises:
+        SessionNotAvailableError: in case the F1 livetiming api returns no data
+    """
+    if livedata is not None and livedata.has('LapCount'):
+        # does not need any further processing
+        _logger.info("Loading lap count data")
+        response = livedata.get('LapCount')
+    elif response is None:
+        _logger.info("Fetching lap count data...")
+        response = fetch_page(path, 'lap_count')
+        if response is None:  # no response received
+            raise SessionNotAvailableError(
+                "No data for this session! If this session only finished "
+                "recently, please try again in a few minutes."
+            )
+
+    data = {'Time': [], 'TotalLaps': [], 'CurrentLap': []}
+    data_keys = ('TotalLaps', 'CurrentLap')
+    converters = (int, int)
+
+    for entry in response:
+        data['Time'].append(to_timedelta(entry[0]))
 
         for key, conv in zip(data_keys, converters):
             try:
-                data[key].append(conv(entry[key]))
+                data[key].append(conv(entry[1][key]))
             except (KeyError, ValueError):
                 # type conversion failed or key is missing
                 data[key].append(None)
 
     return data
 
 
 @Cache.api_request_wrapper
 def driver_info(path, response=None, livedata=None):
-    """Fetch driver information.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch driver information.
 
     Driver information contains the following information about each driver:
 
         `['RacingNumber', 'BroadcastName', 'FullName', 'Tla', 'Line',
         'TeamName', 'TeamColour', 'FirstName', 'LastName', 'Reference',
         'HeadshotUrl']`
 
@@ -1417,18 +1356,18 @@
         with the drivers racing number as key
 
     Raises:
         SessionNotAvailableError: in case the F1 livetiming api returns no data
     """
     if livedata is not None and livedata.has('DriverList'):
         # does not need any further processing
-        logging.info("Loading driver list")
+        _logger.info("Loading driver list")
         response = livedata.get('DriverList')
     elif response is None:
-        logging.info("Fetching driver list...")
+        _logger.info("Fetching driver list...")
         response = fetch_page(path, 'driver_list')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -1477,26 +1416,31 @@
         if 'RacingNumber' not in list(drv_info.values())[0]:
             return dict()
         return drv_info
 
 
 @Cache.api_request_wrapper
 def weather_data(path, response=None, livedata=None):
-    """Fetch and parse weather data.
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch and parse weather data.
 
     Weather data provides the following data channels per sample:
 
         - Time (datetime.timedelta): session timestamp (time only)
         - AirTemp (float): Air temperature [°C]
         - Humidity (float): Relative humidity [%]
         - Pressure (float): Air pressure [mbar]
         - Rainfall (bool): Shows if there is rainfall
         - TrackTemp (float): Track temperature [°C]
         - WindDirection (int): Wind direction [°] (0°-359°)
-        - WindSpeed (float): Wind speed [km/h]
+        - WindSpeed (float): Wind speed [m/s]
 
     Weather data is updated once per minute.
 
     Args:
         path (str): api path base string (usually ``Session.api_path``)
         response: Response as returned by :func:`fetch_page` can
             be passed if it was downloaded already.
@@ -1510,18 +1454,18 @@
 
     Raises:
         SessionNotAvailableError: in case the F1 live timing api
             returns no data
     """
     if livedata is not None and livedata.has('WeatherData'):
         # does not need any further processing
-        logging.info("Loading weather data")
+        _logger.info("Loading weather data")
         response = livedata.get('WeatherData')
     elif response is None:
-        logging.info("Fetching weather data...")
+        _logger.info("Fetching weather data...")
         response = fetch_page(path, 'weather_data')
         if response is None:  # no response received
             raise SessionNotAvailableError(
                 "No data for this session! If this session only finished "
                 "recently, please try again in a few minutes."
             )
 
@@ -1550,16 +1494,35 @@
             except (KeyError, ValueError):
                 # type conversion failed or key is missing
                 data[key].append(conv(0))
 
     return data
 
 
+@Cache.api_request_wrapper
+def season_schedule(path, response=None):
+    if response is None:
+        _logger.info("Fetching season schedule...")
+        response = fetch_page(path, 'index')
+        if response is None:  # no response received
+            raise SessionNotAvailableError(
+                "No data for this session! If this session only finished "
+                "recently, please try again in a few minutes."
+            )
+
+    return response['Meetings']
+
+
 def fetch_page(path, name):
-    """Fetch data from the formula1 livetiming web api, given url base path and page name. An attempt
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Fetch data from the formula1 livetiming web api, given url base path and page name. An attempt
     to parse json or decode known messages is made.
 
     Args:
         path (str): api path base string (usually ``Session.api_path``)
         name (str): page name (see :attr:`pages` for all known pages)
 
     Returns:
@@ -1587,26 +1550,31 @@
                 for e in records:
                     try:
                         ret.append([e[:tl], parse(e[tl:], zipped=is_z)])
                     except json.JSONDecodeError:
                         decode_error_count += 1
                         continue
                 if decode_error_count > 0:
-                    logging.warning(f"Failed to decode {decode_error_count}"
+                    _logger.warning(f"Failed to decode {decode_error_count}"
                                     f" messages ({len(records)} messages "
                                     f"total)")
                 return ret
         else:
             return parse(raw, is_z)
     else:
         return None
 
 
 def parse(text, zipped=False):
-    """Parse json and jsonStream as returned by livetiming.formula1.com
+    """
+    .. warning::
+        :mod:`fastf1.api` will be considered private in future releases and
+        potentially be removed or changed.
+
+    Parse json and jsonStream as returned by livetiming.formula1.com
 
     This function can only pass one data entry at a time, not a whole response.
     Timestamps and data need to be separated before and only the data must be passed as a string to be parsed.
 
     Args:
         text (str): The string which should be parsed
         zipped (bool): Whether or not the text is compressed. This is the case for '.z' data (e.g. position data=)
@@ -1619,16 +1587,17 @@
     if text[0] == '{':
         return json.loads(text)
     if text[0] == '"':
         text = text.strip('"')
     if zipped:
         text = zlib.decompress(base64.b64decode(text), -zlib.MAX_WBITS)
         return parse(text.decode('utf-8-sig'))
-    logging.warning("Couldn't parse text")
+    _logger.warning("Couldn't parse text")
     return text
 
 
 class SessionNotAvailableError(Exception):
     """Raised if an api request returned no data for the requested session.
     A likely cause is that the session does not exist because it was cancelled."""
+
     def __init__(self, *args):
         super().__init__(*args)
```

### Comparing `fastf1-2.3.3/fastf1/core.py` & `fastf1-3.0.0/fastf1/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,111 +9,69 @@
 ------------
 
 All data is provided through the following data objects:
 
     .. autosummary::
        :nosignatures:
 
-       Weekend
        Session
        Laps
        Lap
        Telemetry
        SessionResults
        DriverResult
 
 
 The :class:`Session` object is mainly used as an entry point for loading
 timing data and telemetry data. The :class:`Session` can create a
 :class:`Laps` object which contains all timing, track and session status
 data for a whole session.
 
-Usually you will be using :func:`get_session` to get a :class:`Session`
+Usually you will be using :func:`fastf1.get_session` to get a :class:`Session`
 object.
 
 The :class:`Laps` object holds detailed information about multiples laps.
 
 The :class:`Lap` object holds the same information as :class:`Laps` but only
 for one single lap. When selecting a single lap from a :class:`Laps` object,
 an object of type :class:`Lap` will be returned.
 
 Apart from only providing data, the :class:`Laps`, :class:`Lap` and
 :class:`Telemetry` objects implement various methods for selecting and
 analyzing specific parts of the data.
-
-
-Functions
----------
-
-.. autosummary::
-   :nosignatures:
-
-    get_session
-    get_round
-
 """
 import collections
+import re
 from functools import cached_property
-import logging
 import warnings
+import typing
+from typing import Optional, List, Iterable, Union, Tuple, Any
 
 import numpy as np
 import pandas as pd
 
 import fastf1
-from fastf1 import api, ergast
-from fastf1.utils import recursive_dict_get, to_timedelta
-
-logging.basicConfig(level=logging.INFO, style='{',
-                    format="{module: <8} {levelname: >10} \t{message}")
-
-
-D_LOOKUP = [[44, 'HAM', 'Mercedes'], [77, 'BOT', 'Mercedes'],
-            [55, 'SAI', 'Ferrari'], [16, 'LEC', 'Ferrari'],
-            [33, 'VER', 'Red Bull'], [11, 'PER', 'Red Bull'],
-            [3, 'RIC', 'McLaren'], [4, 'NOR', 'McLaren'],
-            [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
-            [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
-            [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
-            [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
-            [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
-            [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
-
-
-def get_session(*args, **kwargs):
-    """
-    .. deprecated:: 2.2
-        replaced by :func:`fastf1.get_session`
-    """
-    # TODO remove
-    warnings.warn("`fastf1.core.get_session` has been deprecated and will be"
-                  "removed in a future version.\n"
-                  "Use `fastf1.get_session` instead.", FutureWarning)
-    from fastf1 import events
-    return events.get_session(*args, **kwargs)
-
-
-def get_round(year, match):
-    """
-    .. deprecated:: 2.2
-        will be removed without replacement;
-        Use :func:`fastf1.get_event` instead to get an
-        :class:`~fastf1.events.Event` object which provides
-        information including the round number for the event.
-    """
-    # TODO remove
-    warnings.warn("_func:`fastf1.core.get_round` has been deprecated and will "
-                  "be removed without replacement in a future version.\n"
-                  "Use :func:`fastf1.get_event` instead to get an "
-                  ":class:`~fastf1.events.Event` object which provides "
-                  "information including the round number for the event.",
-                  FutureWarning)
-    from fastf1 import events
-    event = events.get_event(year, match)
-    return event.RoundNumber
+from fastf1 import _api as api
+from fastf1 import ergast
+from fastf1.logger import get_logger, soft_exceptions
+from fastf1.utils import to_timedelta
+
+_logger = get_logger(__name__)
+
+D_LOOKUP: List[List] = \
+    [[44, 'HAM', 'Mercedes'], [77, 'BOT', 'Mercedes'],
+     [55, 'SAI', 'Ferrari'], [16, 'LEC', 'Ferrari'],
+     [33, 'VER', 'Red Bull'], [11, 'PER', 'Red Bull'],
+     [3, 'RIC', 'McLaren'], [4, 'NOR', 'McLaren'],
+     [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
+     [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
+     [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
+     [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
+     [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
+     [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
 
 
 class Telemetry(pd.DataFrame):
     """Multi-channel time series telemetry data
 
     The object can contain multiple telemetry channels. Multiple telemetry
     objects with different channels can be merged on time. Each telemetry
@@ -217,26 +175,28 @@
         'DifferentialDistance': {'type': 'continuous', 'missing': 'quadratic'},
         'DriverAhead': {'type': 'discrete'},
         'DistanceToDriverAhead': {'type': 'continuous', 'missing': 'linear'}
     }
     """Known telemetry channels which are supported by default"""
 
     _metadata = ['session', 'driver']
+    _internal_names = pd.DataFrame._internal_names + ['base_class_view']
+    _internal_names_set = set(_internal_names)
 
     def __init__(self, *args, session=None, driver=None,
                  drop_unknown_channels=False, **kwargs):
         super().__init__(*args, **kwargs)
-        self.session = session
+        self.session: Optional[Session] = session
         self.driver = driver
 
         if drop_unknown_channels:
             unknown = set(self.columns).difference(self._CHANNELS.keys())
             super().drop(columns=unknown, inplace=True)
             if unknown:
-                logging.warning(
+                _logger.warning(
                     f"The following unknown telemetry channels have "
                     f"been dropped when creating a Telemetry object: "
                     f"{unknown} (driver: {self.driver})"
                 )
 
     @property
     def _constructor(self):
@@ -272,24 +232,21 @@
         for var in self._metadata:
             meta[var] = getattr(self, var)
         ret = super().merge(*args, **kwargs)
         for var, val in meta.items():
             setattr(ret, var, val)
         return ret
 
-    def slice_by_mask(self, mask, pad=0, pad_side='both'):
+    def slice_by_mask(self, mask, pad=0, pad_side='both') -> "Telemetry":
         """Slice self using a boolean array as a mask.
 
         Args:
             mask (array-like): Array of boolean values with the same length as self
             pad (int): Number of samples used for padding the sliced data
             pad_side (str): Where to pad the data; possible options: 'both', 'before', 'after'
-
-        Returns:
-            :class:`Telemetry`
         """
         if pad:
             if pad_side in ('both', 'before'):
                 i_left_pad = max(0, np.min(np.where(mask)) - pad)
             else:
                 i_left_pad = np.min(np.where(mask))
 
@@ -299,32 +256,36 @@
                 i_right_pad = np.max(np.where(mask))
             mask[i_left_pad: i_right_pad + 1] = True
 
         data_slice = self.loc[mask].copy()
 
         return data_slice
 
-    def slice_by_lap(self, ref_laps, pad=0, pad_side='both', interpolate_edges=False):
+    def slice_by_lap(
+            self,
+            ref_laps: Union["Lap", "Laps"],
+            pad: int = 0,
+            pad_side: str = 'both',
+            interpolate_edges: bool = False
+    ):
         """Slice self to only include data from the provided lap or laps.
 
         .. note:: Self needs to contain a 'SessionTime' column.
 
         .. note:: When slicing with an instance of :class:`Laps` as a reference, the data will be sliced by first and
             last lap. Missing laps in between will not be considered and data for these will still be included in
             the sliced result.
 
         Args:
-            ref_laps (Lap or Laps): The lap/laps by which to slice self
-            pad (int): Number of samples used for padding the sliced data
-            pad_side (str): Where to pad the data; possible options: 'both', 'before', 'after
-            interpolate_edges (bool): Add an interpolated sample at the beginning and end to exactly
-                match the provided time window.
-
-        Returns:
-            :class:`Telemetry`
+            ref_laps: The lap/laps by which to slice self
+            pad: Number of samples used for padding the sliced data
+            pad_side: Where to pad the data; possible options:
+                'both', 'before', 'after
+            interpolate_edges: Add an interpolated sample at the beginning
+                and end to exactly match the provided time window.
         """
         if isinstance(ref_laps, Laps) and len(ref_laps) > 1:
             if 'DriverNumber' not in ref_laps.columns:
                 ValueError("Laps is missing 'DriverNumber'. Cannot return telemetry for unknown driver.")
             if not len(ref_laps['DriverNumber'].unique()) <= 1:
                 raise ValueError("Cannot create telemetry for multiple drivers at once!")
 
@@ -340,51 +301,63 @@
             start_time = ref_laps['LapStartTime']
 
         else:
             raise TypeError("Attribute 'ref_laps' needs to be an instance of `Lap` or `Laps`")
 
         return self.slice_by_time(start_time, end_time, pad, pad_side, interpolate_edges)
 
-    def slice_by_time(self, start_time, end_time, pad=0, pad_side='both', interpolate_edges=False):
+    def slice_by_time(
+            self,
+            start_time,
+            end_time,
+            pad: int = 0,
+            pad_side: str = 'both',
+            interpolate_edges: bool = False
+    ) -> "Telemetry":
         """Slice self to only include data in a specific time frame.
 
         .. note:: Self needs to contain a 'SessionTime' column. Slicing by time use the 'SessionTime' as its reference.
 
         Args:
             start_time (Timedelta): Start of the section
             end_time (Timedelta): End of the section
-            pad (int): Number of samples used for padding the sliced data
-            pad_side (str): Where to pad the data; possible options: 'both', 'before', 'after
-            interpolate_edges (bool): Add an interpolated sample at the beginning and end to exactly
-                match the provided time window.
+            pad: Number of samples used for padding the sliced data
+            pad_side: Where to pad the data; possible options:
+                'both', 'before', 'after
+            interpolate_edges: Add an interpolated sample at the beginning
+                and end to exactly match the provided time window.
 
         Returns:
             :class:`Telemetry`
         """
         if interpolate_edges:
             edges = Telemetry({'SessionTime': (start_time, end_time),
                                'Date': (start_time + self.session.t0_date, end_time + self.session.t0_date)},
-                              session=self.session)
+                              session=self.session).__finalize__(self)
             d = self.merge_channels(edges)
 
         else:
             d = self.copy()  # TODO no copy?
 
         sel = ((d['SessionTime'] <= end_time) & (d['SessionTime'] >= start_time))
         if np.any(sel):
             data_slice = d.slice_by_mask(sel, pad, pad_side)
 
             if 'Time' in data_slice.columns:
                 # shift time to 0 so laps can overlap
                 data_slice.loc[:, 'Time'] = data_slice['SessionTime'] - start_time
 
             return data_slice
-        return Telemetry()
+        return Telemetry().__finalize__(self)
 
-    def merge_channels(self, other, frequency=None):
+    def merge_channels(
+            self,
+            other: Union["Telemetry", pd.DataFrame],
+            frequency: Union[int, str] = None
+    ):
         """Merge telemetry objects containing different telemetry channels.
 
         The two objects don't need to have a common time base. The data will be merged, optionally resampled and
         missing values will be interpolated.
 
         :attr:`Telemetry.TELEMETRY_FREQUENCY` determines if and how the data is resampled. This can be overridden using
         the `frequency` keyword fo this method.
@@ -410,20 +383,17 @@
         .. note :: Unknown telemetry channels will be merged but missing values will not be interpolated. This can
             either be done manually or a custom telemetry channel can be added using :meth:`register_new_channel`.
 
         .. note :: Do not resample data multiple times. Always resample based on the original data
             to preserve accuracy
 
         Args:
-            other (:class:`Telemetry` or :class:`pandas.DataFrame`): Object to be merged with self
-            frequency (str or int): Optional frequency to overwrite global preset. (Either string 'original' or integer
-                for a frequency in Hz)
-
-        Returns:
-            :class:`Telemetry`
+            other: Object to be merged with self
+            frequency: Optional frequency to overwrite global preset.
+                (Either string 'original' or integer for a frequency in Hz)
         """
         # merge the data and interpolate missing; 'Date' needs to be the index
         data = self.set_index('Date')
         other = other.set_index('Date')
 
         # save dtypes before merging so they can be restored after merging
         # necessary for example because merging produces NaN values which would cause an int column to become float
@@ -489,33 +459,39 @@
 
                 resampled_columns[ch] = res
 
             res_source = merged.loc[:, 'Source'].resample(frq, origin=ref_date).asfreq().fillna(value='interpolation')
             resampled_columns['Source'] = res_source
 
             # join resampled columns and make 'Date' a column again
-            merged = Telemetry(resampled_columns)\
-                .__finalize__(self)\
-                .reset_index()\
+            merged = Telemetry(resampled_columns) \
+                .__finalize__(self) \
+                .reset_index() \
                 .rename(columns={'index': 'Date'})
 
             # recalculate the time columns
             merged['SessionTime'] = merged['Date'] - self.session.t0_date
             merged['Time'] = merged['SessionTime'] - merged['SessionTime'].iloc[0]
 
         # restore data types from before merging
         for col in dtype_map.keys():
             try:
-                merged.loc[:, col] = merged.loc[:, col].astype(dtype_map[col])
+                merged[col] = merged.loc[:, col].astype(dtype_map[col])
             except ValueError:
-                logging.warning(f"Failed to preserve data type for column '{col}' while merging telemetry.")
+                _logger.warning(f"Failed to preserve data type for column "
+                                f"'{col}' while merging telemetry.")
 
         return merged
 
-    def resample_channels(self, rule=None, new_date_ref=None, **kwargs):
+    def resample_channels(
+            self,
+            rule: Optional[str] = None,
+            new_date_ref: Optional[pd.Series] = None,
+            **kwargs: Optional[Any]
+    ):
         """Resample telemetry data.
 
         Convenience method for frequency conversion and resampling. Up and down sampling of data is supported.
         'Date' and 'SessionTime' need to exist in the data. 'Date' is used as the main time reference.
 
         There are two ways to use this method:
 
@@ -524,26 +500,26 @@
               reference. See the pandas method to see which options are available.
 
             - using the 'new_date_ref' keyword a :class:`pandas.Series` containing new values for date
               (dtype :class:`pandas.Timestamp`) can be provided. The existing data will be resampled onto this new
               time reference.
 
         Args:
-            rule (optional, str): Resampling rule for :meth:`pandas.Series.resample`
-            new_date_ref (optional, pandas.Series): New custom Series of reference dates
-            **kwargs (optional, any): Only in combination with 'rule'; additional parameters for
-                :meth:`pandas.Series.resample`
+            rule: Resampling rule for :meth:`pandas.Series.resample`
+            new_date_ref: New custom Series of reference dates
+            **kwargs: Only in combination with 'rule'; additional parameters
+                for :meth:`pandas.Series.resample`
         """
         if rule is not None and new_date_ref is not None:
             raise ValueError("You can only specify one of 'rule' or 'new_index'")
         if rule is None and new_date_ref is None:
             raise ValueError("You need to specify either 'rule' or 'new_index'")
 
         if new_date_ref is None:
-            st = pd.Series(index=pd.DatetimeIndex(self['Date']), dtype=int)\
+            st = pd.Series(index=pd.DatetimeIndex(self['Date']), dtype=int) \
                 .resample(rule, **kwargs).asfreq()
             new_date_ref = pd.Series(st.index)
 
         new_tel = Telemetry(columns=self.columns).__finalize__(self)
         new_tel.loc[:, 'Date'] = new_date_ref
 
         combined_tel = self.merge_channels(
@@ -595,26 +571,31 @@
         elif isinstance(ret.index, pd.DatetimeIndex):
             ret['SessionTime'] = ret.index - self.session.t0_date  # assume index is Date
         ret['Time'] = ret['SessionTime'] - ret['SessionTime'].iloc[0]
 
         return ret
 
     @classmethod
-    def register_new_channel(cls, name, signal_type, interpolation_method=None):
+    def register_new_channel(
+            cls,
+            name: str,
+            signal_type: str,
+            interpolation_method: Optional[str] = None
+    ):
         """Register a custom telemetry channel.
 
         Registered telemetry channels are automatically interpolated when merging or resampling data.
 
         Args:
-            name (str): Telemetry channel/column name
-            signal_type (str): One of three possible signal types:
+            name: Telemetry channel/column name
+            signal_type: One of three possible signal types:
                 - 'continuous': Speed, RPM, Distance, ...
                 - 'discrete': DRS, nGear, status values, ...
                 - 'excluded': Data channel will be ignored during resampling
-            interpolation_method (optional, str): The interpolation method
+            interpolation_method: The interpolation method
                 which should be used. Can only be specified and is required
                 in combination with ``signal_type='continuous'``. See
                 :meth:`pandas.Series.interpolate` for possible interpolation
                 methods.
         """
         if signal_type not in ('discrete', 'continuous', 'excluded'):
             raise ValueError(f"Unknown signal type {signal_type}.")
@@ -627,77 +608,83 @@
         """Return the first index at which the 'Time' value is not zero or NA/NaT"""
         # find first row where time is not zero; usually this is the first row but sometimes.....
         i_arr = np.where((self['Time'] != pd.Timedelta(0)) & ~pd.isna(self['Time']))[0]
         if i_arr.size != 0:
             return np.min(i_arr)
         return None
 
-    def add_differential_distance(self, drop_existing=True):
+    def add_differential_distance(
+            self,
+            drop_existing: bool = True
+    ) -> "Telemetry":
         """Add column 'DifferentialDistance' to self.
 
         This column contains the distance driven between subsequent samples.
 
         Calls :meth:`calculate_differential_distance` and joins the result
         with self.
 
         Args:
-            drop_existing (bool): Drop and recalculate column if it already exists
+            drop_existing: Drop and recalculate column if it already exists
         Returns:
-            :class:`Telemetry`: self joined with new column or self if column exists and `drop_existing` is False.
+            self joined with new column or self if column exists
+            and `drop_existing` is False.
         """
         if ('DifferentialDistance' in self.columns) and not drop_existing:
             return self
 
         new_dif_dist = pd.DataFrame(
             {'DifferentialDistance': self.calculate_differential_distance()}
         )
         if 'DifferentialDistance' in self.columns:
             return self.drop(labels='DifferentialDistance', axis=1) \
                 .join(new_dif_dist, how='outer')
 
         return self.join(new_dif_dist, how='outer')
 
-    def add_distance(self, drop_existing=True):
+    def add_distance(self, drop_existing: bool = True) -> "Telemetry":
         """Add column 'Distance' to self.
 
         This column contains the distance driven since the first sample of self in meters.
 
         The data is produced by integrating the differential distance between subsequent laps.
         You should not apply this function to telemetry of many laps simultaneously to reduce integration error.
         Instead apply it only to single laps or few laps at a time!
 
         Calls :meth:`integrate_distance` and joins the result with self.
 
         Args:
-            drop_existing (bool): Drop and recalculate column if it already exists
+            drop_existing: Drop and recalculate column if it already exists
         Returns:
-            :class:`Telemetry`: self joined with new column or self if column exists and `drop_existing` is False.
+            self joined with new column or self if column exists
+            and `drop_existing` is False.
         """
         if ('Distance' in self.columns) and not drop_existing:
             return self
 
         new_dist = pd.DataFrame({'Distance': self.integrate_distance()})
         if 'Distance' in self.columns:
             return self.drop(labels='Distance', axis=1).join(new_dist, how='outer')
 
         return self.join(new_dist, how='outer')
 
-    def add_relative_distance(self, drop_existing=True):
+    def add_relative_distance(self, drop_existing: bool = True) -> "Telemetry":
         """Add column 'RelativeDistance' to self.
 
         This column contains the distance driven since the first sample as
         a floating point number where ``0.0`` is the first sample of self
         and ``1.0`` is the last sample.
 
         This is calculated the same way as 'Distance' (see: :meth:`add_distance`). The same warnings apply.
 
         Args:
-            drop_existing (bool): Drop and recalculate column if it already exists
+            drop_existing: Drop and recalculate column if it already exists
         Returns:
-            :class:`Telemetry`: self joined with new column or self if column exists and `drop_existing` is False.
+            self joined with new column or self if column exists
+            and `drop_existing` is False.
         """
         if 'RelativeDistance' in self.columns:
             if drop_existing:
                 d = self.drop(labels='RelativeDistance', axis=1)
             else:
                 return self
         else:
@@ -706,15 +693,64 @@
         if 'Distance' in d.columns:
             rel_dist = d.loc[:, 'Distance'] / d.loc[:, 'Distance'].iloc[-1]
         else:
             dist = d.integrate_distance()
             rel_dist = dist / dist.iloc[-1]
         return d.join(pd.DataFrame({'RelativeDistance': rel_dist}), how='outer')
 
-    def add_driver_ahead(self, drop_existing=True):
+    def add_track_status(self, drop_existing=True):
+        """Add column 'TrackStatus' to self.
+
+        This column contains the Track Status for each event as a number.
+
+        See :func:`fastf1.api.track_status_data` for more information.
+
+        Args:
+            drop_existing (bool): Drop and recalculate column if it already
+                exists.
+        Returns:
+            :class:`Telemetry`: self joined with new column or self if column
+                exists and `drop_existing` is False.
+        """
+        if 'TrackStatus' in self.columns:
+            if drop_existing:
+                d = self.drop(labels='TrackStatus', axis=1)
+            else:
+                return self
+        else:
+            d = self
+
+        ts = []
+        statuses = d.session.track_status['Status']
+        events = d.session.t0_date + d.session.track_status['Time']
+
+        # |--- event K ---|--- N telemetry samples ---|--- event K + 1 ---|
+        #                           ^
+        #                   all samples have the same
+        #                 track status because of event K
+        #
+        # For each track status event, calculate the in between events of the
+        # telemetry, up until the next track status event. For each of the in
+        # between events add the corresponding track status to an array. At
+        # last, create the new column 'TrackStatus' with the array of track
+        # statuses.
+        for index in range(events.shape[0] - 1):
+            curr_e = events[index]
+            next_e = events[index+1]
+
+            dd_shape = d[(d['Date'] < next_e) & (d['Date'] >= curr_e)].shape[0]
+            ts.extend([statuses[index]] * dd_shape)
+
+        dd_shape = d[(d['Date'] > events.iloc[-1])].shape[0]
+        ts.extend([statuses.iloc[-1]] * dd_shape)
+
+        d['TrackStatus'] = ts
+        return d
+
+    def add_driver_ahead(self, drop_existing: bool = True) -> "Telemetry":
         """Add column 'DriverAhead' and 'DistanceToDriverAhead' to self.
 
         DriverAhead: Driver number of the driver ahead as string
         DistanceToDriverAhead: Distance to next car ahead in meters
 
         .. note:: Cars in the pit lane are currently not excluded from the data. They will show up when overtaken on
             pit straight even if they're not technically in front of the car. A fix for this is TBD with other
@@ -725,17 +761,18 @@
         should be merged afterwards.
         If you absolutely need to apply it to a whole session, use the legacy implementation. Note that data of
         the legacy implementation will be considerably less smooth. (see :mod:`fastf1.legacy`)
 
         Calls :meth:`calculate_driver_ahead` and joins the result with self.
 
         Args:
-            drop_existing (bool): Drop and recalculate column if it already exists
+            drop_existing: Drop and recalculate column if it already exists
         Returns:
-            :class:`Telemetry`: self joined with new column or self if column exists and `drop_existing` is False.
+            self joined with new column or self if column exists
+            and `drop_existing` is False.
         """
         if 'DriverAhead' in self.columns and 'DistanceToDriverAhead' in self.columns:
             if drop_existing:
                 d = self.drop(labels='DriverAhead', axis=1) \
                     .drop(labels='DistanceToDriverAhead', axis=1)
             else:
                 return self
@@ -765,21 +802,18 @@
         # indices need to match as .join works index-on-index
         dtd['_SelfIndex'] = d.index
         dtd.set_index('_SelfIndex', drop=True, inplace=True)
 
         return d.join(dtd.loc[:, ('DriverAhead', 'DistanceToDriverAhead')],
                       how='outer')
 
-    def calculate_differential_distance(self):
+    def calculate_differential_distance(self) -> pd.Series:
         """Calculate the distance between subsequent samples of self.
 
         Distance is in meters
-
-        Returns:
-            :class:`pandas.Series`
         """
         if not all([col in self.columns for col in ('Speed', 'Time')]):
             raise ValueError("Telemetry does not contain required channels 'Time' and 'Speed'.")
         if self.size != 0:
             dt = self['Time'].dt.total_seconds().diff()
             dt.iloc[0] = self['Time'].iloc[0].total_seconds()
             ds = self['Speed'] / 3.6 * dt
@@ -798,26 +832,26 @@
         """
         ds = self.calculate_differential_distance()
         if not ds.empty:
             return ds.cumsum()
         else:
             return pd.Series()
 
-    def calculate_driver_ahead(self, return_reference=False):
+    def calculate_driver_ahead(self, return_reference: bool = False):
         """Calculate driver ahead and distance to driver ahead.
 
         Driver ahead: Driver number of the driver ahead as string
         Distance to driver ahead: Distance to the car ahead in meters
 
         .. note:: This gives a smoother/cleaner result than the legacy implementation but WILL introduce
             integration error when used over long distances (more than one or two laps may sometimes be considered
             a long distance). If in doubt, do sanity checks (against the legacy version or in another way).
 
         Args:
-            return_reference (bool): Additionally return the reference
+            return_reference: Additionally return the reference
                 telemetry data slice that is used to calculate the new data.
 
         Returns:
             driver ahead (numpy.array), distance to driver ahead (numpy.array),
             [reference telemetry (optional, :class:`Telemetry`)]
         """
         t_start = self['SessionTime'].iloc[0]
@@ -877,15 +911,15 @@
                         (drv_laps['LapNumber'] >= (lap_n_before - pad_before))
                         & (drv_laps['LapNumber'] <= lap_n_after + pad_after)
                     ]
                 except IndexError:
                     break
 
                 if (pad_before >= 1) or (pad_after >= 1):
-                    logging.warning(f"Car number {drv} cannot be located "
+                    _logger.warning(f"Car number {drv} cannot be located "
                                     f"on track while calculating the distance"
                                     f"between cars.")
                     break
 
                 if relevant_laps.empty:
                     break
 
@@ -899,15 +933,15 @@
                 break
 
             if (relevant_laps is None) or relevant_laps.empty:
                 continue
 
             # first slice by lap and calculate distance, so that distance is zero at finish line
             drv_tel = self.session.car_data[drv] \
-                          .slice_by_lap(relevant_laps)
+                .slice_by_lap(relevant_laps)
 
             if drv_tel.empty:
                 continue
 
             drv_tel = drv_tel.add_distance()
 
             # now slice again by time to only get the relevant time frame
@@ -950,133 +984,128 @@
 
         if return_reference:
             return drv_ahead, dist_to_drv_ahead, own_ref_tel
 
         return drv_ahead, dist_to_drv_ahead
 
 
-class Weekend:
-    """
-    .. deprecated:: 2.2
-        Use :class:`fastf1.events.Event` instead
-    """
-    def __new__(cls, year, gp):
-        warnings.warn("`fastf1.core.Weekend` has been deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `fastf1.events.Event` instead.", FutureWarning)
-        from fastf1 import events
-        return events.get_event(year, gp)
-
-
 class Session:
     """Object for accessing session specific data.
 
     The session class will usually be your starting point. This object will
     have various information about the session.
 
     .. note:: Most of the data is only available after calling
         :func:`Session.load`
     """
 
     def __init__(self, event, session_name, f1_api_support=False):
-        # TODO: load drivers immediately
-        # TODO: load driver list for older seasons through ergast
         self.event = event
         """:class:`~fastf1.events.Event`: Reference to the associated event
         object."""
         self.name = session_name
         """str: Name of this session, for example 'Qualifying', 'Race', 'FP1', ..."""
         self.f1_api_support = f1_api_support
         """bool: The official F1 API supports this event and lap timing data and
         telemetry data are available."""
-        self.date = self.event.get_session_date(session_name)
+        self.date = self.event.get_session_date(session_name, utc=True)
         """pandas.Datetime: Date at which this session took place."""
         self.api_path = api.make_path(
             self.event['EventName'],
             self.event['EventDate'].strftime('%Y-%m-%d'),
             self.name, self.date.strftime('%Y-%m-%d')
         )
         """str: API base path for this session"""
 
-        self._session_status = dict()
-        self._race_control_messages = dict()
+        self._ergast = ergast.Ergast()
+
+        self._session_status: pd.DataFrame
+        self._race_control_messages: pd.DataFrame
 
+        self._track_status: pd.DataFrame
+
+        self._total_laps: Optional[int]
         self._laps: Laps
-        self._t0_date: pd.Timestamp
 
-        self._session_start_time: pd.Timedelta
+        self._t0_date: Optional[pd.Timestamp]
+        self._session_start_time: Optional[pd.Timedelta]
 
         self._car_data: dict
         self._pos_data: dict
 
         self._weather_data: pd.DataFrame
         self._results: SessionResults
 
+    def __repr__(self):
+        return (f"{self.event.year} Season Round {self.event.RoundNumber}: "
+                f"{self.event.EventName} - {self.name}")
+
     def _get_property_warn_not_loaded(self, name):
-        d = getattr(self, name, None)
-        if d is None:
+        if not hasattr(self, name):
             raise DataNotLoadedError("The data you are trying to access has not "
                                      "been loaded yet. See `Session.load`")
-        return d
-
-    @property
-    def weekend(self):
-        """Deprecated: use :attr:`Session.event` instead"""
-        warnings.warn("The property `Session.weekend` has been renamed to "
-                      "`Session.event`.\n The old property will be removed in"
-                      "a future version.", FutureWarning)
-        return self.event
+        return getattr(self, name, None)
 
     @property
     def drivers(self):
         """:class:`list`: List of all drivers that took part in this
         session; contains driver numbers as string.
 
         Data is available after calling `Session.load`
         """
         return list(self.results['DriverNumber'].unique())
 
     @property
-    def results(self):
+    def results(self) -> "SessionResults":
         """:class:`SessionResults`: Session result with driver information.
 
         Data is available after calling `Session.load`
         """
         return self._get_property_warn_not_loaded('_results')
 
     @property
-    def laps(self):
+    def laps(self) -> "Laps":
         """:class:`Laps`: All laps from all drivers driven in this session.
 
         Data is available after calling `Session.load` with ``laps=True``
         """
         return self._get_property_warn_not_loaded('_laps')
 
     @property
+    def total_laps(self) -> int:
+        """:class:`int`: Originally scheduled number of laps for race-like
+        sessions such as Race and Sprint. It takes None as a default value
+        for other types of sessions or if data is unavailable
+
+        Data is available after calling `Session.load` with ``laps=True``
+        """
+        return self._get_property_warn_not_loaded('_total_laps')
+
+    @property
     def weather_data(self):
         """Dataframe containing weather data for this session as received
         from the api. See :func:`fastf1.api.weather_data` for available data
         channels. Each data channel is one row of the dataframe.
 
         Data is available after calling `Session.load` with ``weather=True``
         """
         return self._get_property_warn_not_loaded('_weather_data')
 
     @property
-    def car_data(self):
+    def car_data(self) -> "Telemetry":
         """Dictionary of car telemetry (Speed, RPM, etc.) as received from
         the api by car number (where car number is a string and the telemetry
         is an instance of :class:`Telemetry`)
 
         Data is available after calling `Session.load` with ``telemetry=True``
         """
         return self._get_property_warn_not_loaded('_car_data')
 
     @property
-    def pos_data(self):
+    def pos_data(self) -> "Telemetry":
         """Dictionary of car position data as received from the api by car
         number (where car number is a string and the telemetry
         is an instance of :class:`Telemetry`)
 
         Data is available after calling `Session.load` with ``telemetry=True``
         """
         return self._get_property_warn_not_loaded('_pos_data')
@@ -1087,24 +1116,33 @@
         :func:`fastf1.api.session_status_data`
 
         Data is available after calling `Session.load` with ``laps=True``
         """
         return self._get_property_warn_not_loaded('_session_status')
 
     @property
+    def track_status(self):
+        """:class:`pandas.Dataframe`: Track status data as returned by
+        :func:`fastf1.api.track_status_data`
+
+        Data is available after calling `Session.load` with ``laps=True``
+        """
+        return self._get_property_warn_not_loaded('_track_status')
+
+    @property
     def race_control_messages(self):
         """:class:`pandas.Dataframe`: Race Control messages as returned by
         :func:`fastf1.api.race_control_messages`
 
         Data is available after calling `Session.load` with ``messages=True``
         """
         return self._get_property_warn_not_loaded('_race_control_messages')
 
     @property
-    def session_start_time(self):
+    def session_start_time(self) -> pd.Timedelta:
         """:class:`pandas.Timedelta`: Session time at which the session was
         started according to the session status data. This is not the
         time at which the session is scheduled to be started!
 
         Data is available after calling `Session.load` with ``laps=True``
         """
         return self._get_property_warn_not_loaded('_session_start_time')
@@ -1122,17 +1160,20 @@
              livedata=None):
         """Load session data from the supported APIs.
 
         This method allows to flexibly load some or all data that FastF1 can
         give you access to. Without specifying any further options, all data
         is loaded by default.
 
-        Downloading and parsing of the data takes a considerable amount of
-        time. Therefore, it is highly recommended to enable caching so that
-        most of the data processing needs to be done only once.
+        Usually, it is recommended to load all available data because
+        internally FastF1 partially mixes data from multiple endpoints and
+        data sources to correct for errors or to add more information. These
+        features are optional and may not work when some data is unavailable.
+        In these cases, FastF1 will return the data to the best of its
+        abilities.
 
         .. note:: **Lap data: drivers crashing and retiring**
 
             *During a session:*
             An additional last lap is added for a driver if the last timed
             lap of a driver is not an inlap and the session is aborted next.
             The `Time` for when this lap was "set" will be set to the time at
@@ -1159,167 +1200,126 @@
             telemetry (bool): Load telemetry data.
             weather (bool): Load weather data.
             messages (bool): Load race control messages for the session
             livedata (:class:`fastf1.livetiming.data.LiveTimingData`, optional):
                 instead of requesting the data from the api, locally saved
                 livetiming data can be used as a data source
         """
-        logging.info(f"Loading data for "
+        _logger.info(f"Loading data for "
                      f"{self.event['EventName']} - {self.name}"
                      f" [v{fastf1.__version__}]")
 
         self._load_drivers_results(livedata=livedata)
 
         if self.f1_api_support:
             if laps:
-                try:
-                    self._load_laps_data(livedata)
-                except Exception as exc:
-                    logging.warning("Failed to load lap data!")
-                    logging.debug("Lap data failure traceback:", exc_info=exc)
+                self._load_session_status_data(livedata=livedata)
+                self._load_total_lap_count(livedata=livedata)
+                self._load_track_status_data(livedata=livedata)
+                self._load_laps_data(livedata=livedata)
+                self._add_first_lap_time_from_ergast()
 
             if telemetry:
-                try:
-                    self._load_telemetry(livedata=livedata)
-                except Exception as exc:
-                    logging.warning("Failed to load telemetry data!")
-                    logging.debug("Telemetry data failure traceback:", exc_info=exc)
+                self._load_telemetry(livedata=livedata)
 
             if weather:
-                try:
-                    self._load_weather_data(livedata=livedata)
-                except Exception as exc:
-                    logging.warning("Failed to load weather data!")
-                    logging.debug("Weather data failure traceback:", exc_info=exc)
+                self._load_weather_data(livedata=livedata)
 
             if messages:
-                try:
-                    self._load_race_control_messages(livedata=livedata)
-                except Exception as exc:
-                    logging.warning("Failed to load Race Control message "
-                                    "data!")
-                    logging.debug("RC message data failure traceback:",
-                                  exc_info=exc)
+                self._load_race_control_messages(livedata=livedata)
 
         else:
             if any((laps, telemetry, weather, messages)):
-                logging.warning(
+                _logger.warning(
                     "Cannot load laps, telemetry, weather, and message data "
                     "because the relevant API is not supported for this "
                     "session."
                 )
 
-        logging.info(f"Finished loading data for {len(self.drivers)} "
-                     f"drivers: {self.drivers}")
+        self._fix_missing_laps_retired_on_track()
+        self._set_laps_deleted_from_rcm()
 
-    def load_laps(self, with_telemetry=False, livedata=None):
-        """
-        .. deprecated:: 2.2
-            use :func:`Session.load` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("`Session.load_laps` is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Session.load` instead.", FutureWarning)
-        self.load(telemetry=with_telemetry, livedata=livedata)
-        return self.laps
-
-    def load_telemetry(self, livedata=None):
-        """
-        .. deprecated:: 2.2
-            use :func:`Session.load` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("`Session.load_laps` is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Session.load` instead.", FutureWarning)
-        self._load_telemetry(livedata=livedata)
+        _logger.info(f"Finished loading data for {len(self.drivers)} "
+                     f"drivers: {self.drivers}")
 
-    def _load_laps_data(self, livedata):
+    @soft_exceptions("lap timing data", "Failed to load timing data!", _logger)
+    def _load_laps_data(self, livedata=None):
         data, _ = api.timing_data(self.api_path, livedata=livedata)
         app_data = api.timing_app_data(self.api_path, livedata=livedata)
-        logging.info("Processing timing data...")
+        _logger.info("Processing timing data...")
         # Matching data and app_data. Not super straightforward
         # Sometimes a car may enter the pit without changing tyres, so
         # new compound is associated with the help of logging time.
         data.drop(columns=['NumberOfPitStops'], inplace=True)
         useful = app_data[['Driver', 'Time', 'Compound', 'StartLaps', 'New',
                            'Stint']]
         useful = useful[~useful['Compound'].isnull()]
-        # check when a session was started; for a race this indicates the
-        # start of the race
-        session_status = api.session_status_data(self.api_path,
-                                                 livedata=livedata)
-        for i in range(len(session_status['Status'])):
-            if session_status['Status'][i] == 'Started':
-                self._session_start_time = session_status['Time'][i]
-                break
-        self._session_status = pd.DataFrame(session_status)
-        df = None
-
-        track_status = api.track_status_data(self.api_path, livedata=livedata)
 
         drivers = self.drivers
         if not drivers:
             # no driver list, generate from lap data
-            drivers = set(data['Driver'].unique())\
+            drivers = set(data['Driver'].unique()) \
                 .intersection(set(useful['Driver'].unique()))
 
             _nums_df = pd.DataFrame({'DriverNumber': list(drivers)},
                                     index=list(drivers))
             _info_df = pd.DataFrame(fastf1._DRIVER_TEAM_MAPPING).T
 
             self._results = SessionResults(_nums_df.join(_info_df),
                                            force_default_cols=True)
 
-            logging.warning("Generating minimal driver "
+            _logger.warning("Generating minimal driver "
                             "list from timing data.")
 
+        df = None
         for i, driver in enumerate(drivers):
             d1 = data[data['Driver'] == driver]
             d2 = useful[useful['Driver'] == driver]
-            # TODO: replace number of pitstops with stint?
             if d2.shape[0] != len(d2['Stint'].unique()):
                 # tyre info includes correction messages that need to be
                 # applied before continuing
                 d2 = self.__fix_tyre_info(d2)
-            only_one_lap = False
 
+            is_generated = False
             if not len(d1):
                 if ((self.name in ('Race', 'Sprint', 'Sprint Qualifying'))
                         and len(d2)):
                     # add data for drivers who crashed on the very first lap
                     # as a downside, this potentially adds a nonexistent lap
                     # for drivers who could not start the race
-                    only_one_lap = True
+                    is_generated = True
                     result = d1.copy()
                     result['Driver'] = [driver, ]
                     result['NumberOfLaps'] = 0
                     result['Time'] = data['Time'].min()
                     result['IsPersonalBest'] = False
                     result['Compound'] = d2['Compound'].iloc[0]
                     result['TyreLife'] = d2['StartLaps'].iloc[0]
                     result['Stint'] = 0
                     result['New'] = d2['New'].iloc[0]
                 else:
-                    logging.warning(f"No lap data for driver {driver}")
+                    _logger.warning(f"No lap data for driver {driver}")
                     continue  # no data for this driver; skip
 
             elif not len(d2):
                 result = d1.copy()
                 result['Compound'] = str()
                 result['TyreLife'] = np.nan
                 result['Stint'] = 0
                 result['New'] = False
-                logging.warning(f"No tyre data for driver {driver}")
+                _logger.warning(f"No tyre data for driver {driver}")
 
             else:
-                result = pd.merge_asof(d1, d2, on='Time', by='Driver')\
+                result = pd.merge_asof(d1, d2, on='Time', by='Driver') \
                     .rename(columns={'StartLaps': 'TyreLife'})
 
+            # add flag that indicates if the data for this lap was generated
+            # by FastF1
+            result['FastF1Generated'] = is_generated
+
             # calculate lap start time by setting it to the 'Time' of the
             # previous lap
             laps_start_time = list(result['Time'])[:-1]
             if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
                 # assumption that the first lap started when the session was
                 # started can only be made for the race
                 laps_start_time.insert(0, self.session_start_time)
@@ -1367,111 +1367,342 @@
             result.loc[mask, 'LapStartTime'] = result.loc[mask, 'PitOutTime']
 
             # create total laps counter for each tyre used
             for npit in result['Stint'].unique():
                 sel = result['Stint'] == npit
                 result.loc[sel, 'TyreLife'] += np.arange(0, sel.sum()) + 1
 
-            # check if there is another lap during which the session was aborted
-            # but which is not in the data
-            # if yes, add as much data as possible for it
-            # set the time of abort as lap end time given that there is no
-            # accurate time available
-            # this block of code has no tests; testing would require to mock
-            # the data as the actual data may be updated on the server after
-            # some time and the problem no longer occurs
-            if pd.isna(result['PitInTime'].iloc[-1]) and not only_one_lap:
-                if not pd.isna(result['Time'].iloc[-1]):
-                    next_statuses = self.session_status[
-                        self.session_status['Time'] > result['Time'].iloc[-1]
-                        ]
-                else:
-                    next_statuses = self.session_status[
-                        self.session_status['Time']
-                        > result['LapStartTime'].iloc[-1]
-                        ]
-
-                aborted = False
-                if not next_statuses.empty:
-                    next_status = next_statuses.iloc[0]
-                    aborted = (next_status['Status'] == 'Aborted')
-
-                if aborted:
-                    new_last = pd.DataFrame({
-                        'LapStartTime': [result['Time'].iloc[-1]],
-                        'Time': [next_status['Time']],
-                        'Driver': [result['Driver'].iloc[-1]],
-                        'NumberOfLaps': [result['NumberOfLaps'].iloc[-1] + 1],
-                        'Stint': [result['Stint'].iloc[-1]],
-                        # 'IsPersonalBest': False,
-                        'Compound': [result['Compound'].iloc[-1]],
-                        'TyreLife': [result['TyreLife'].iloc[-1] + 1],
-                        'New': [result['New'].iloc[-1]],
-                    })
-                    if not only_one_lap:
-                        result = result.append(new_last).reset_index(drop=True)
-                    else:
-                        result = new_last
-
             df = pd.concat([df, result], sort=False)
+
         if df is None:
             raise NoLapDataError
+
         laps = df.reset_index(drop=True)  # noqa: F821
+
+        # rename some columns
         laps.rename(columns={'Driver': 'DriverNumber',
                              'NumberOfLaps': 'LapNumber',
                              'New': 'FreshTyre'}, inplace=True)
+
         laps['Stint'] += 1  # counting stints from 1
+
+        # add team names and driver names based on driver number
         t_map = {r['DriverNumber']: r['TeamName']
                  for _, r in self.results.iterrows()}
         laps['Team'] = laps['DriverNumber'].map(t_map)
         d_map = {r['DriverNumber']: r['Abbreviation']
                  for _, r in self.results.iterrows()}
         laps['Driver'] = laps['DriverNumber'].map(d_map)
 
-        # add track status data
+        # add Position based on lap timing
+        laps['Position'] = np.NaN  # create empty column
+        if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
+            for lap_n in laps['LapNumber'].unique():
+                # get each drivers lap for the current lap number, sorted by
+                # the time when each lap was set
+                laps_eq_n = laps.loc[
+                    laps['LapNumber'] == lap_n, ('Time', 'Position')
+                ].reset_index(drop=True).sort_values(by='Time')
+
+                # number positions and restore previous order by index
+                laps_eq_n['Position'] = range(1, len(laps_eq_n) + 1)
+                laps.loc[laps['LapNumber'] == lap_n, 'Position'] \
+                    = laps_eq_n.sort_index()['Position'].to_list()
+
+        self._add_track_status_to_laps(laps)
+
+        self._laps = Laps(laps, session=self, force_default_cols=True)
+        self._check_lap_accuracy()
+
+    def _fix_missing_laps_retired_on_track(self):
+        # generate a last lap entry with assumed end time for cars that
+        # retired on track
+
+        if not hasattr(self, '_laps'):
+            return
+
+        any_new = False
+        for drv in self.laps['DriverNumber'].unique():
+            drv_laps = self._laps[self.laps['DriverNumber'] == drv]
+
+            if (len(drv_laps) == 1) and drv_laps['FastF1Generated'].iloc[0]:
+                # there is only one lap which was added by FastF1, don't
+                # generate a followup lap based on that
+                continue
+
+            # try to get a valid last timestamp for the last lap
+            ref_time = drv_laps['Time'].iloc[-1]
+            if pd.isna(ref_time):
+                ref_time = drv_laps['LapStartTime'].iloc[-1]
+            # split session status at reference timestamp
+            # if ref_time is still NaT, next/prev_statuses will be empty
+            # after comparison
+            next_statuses = self.session_status[
+                self.session_status['Time'] > ref_time
+                ]
+            prev_statuses = self.session_status[
+                self.session_status['Time'] <= ref_time
+                ]
+
+            if ((not prev_statuses.empty)
+                    and (prev_statuses['Status'] == 'Finished').any()):
+                # driver finished session correctly, nothing to do
+                continue
+
+            if (next_statuses.empty
+                    or (not (next_statuses['Status'] == 'Finished').any())):
+                # there are no next statuses or no status message indicates
+                # that the session finished after the current timestamp
+                # -> the data is inconclusive
+                continue
+
+            if not pd.isna(drv_laps['PitInTime'].iloc[-1]):
+                # last lap was an inlap
+                continue
+
+            if ((total_laps := getattr(self, '_total_laps', None)) is not None
+                    and (drv_laps.shape[0] >= total_laps)):
+                # driver has already completed full race distance
+                # can happen because rc message timestamp is slightly off
+                continue
+
+            if ((len(drv_laps) >= 2)
+                    and (not pd.isna(drv_laps['PitInTime'].iloc[-2]))
+                    and pd.isna(drv_laps['PitOutTime'].iloc[-1])):
+                # last lap was an inlap and a new lap was started in the pit
+                # lane but the car did not leave the pits again (happens if
+                # box comes after timing line in pits)
+                continue
+
+            next_status = next_statuses.iloc[0]
+
+            if next_status['Status'] == 'Aborted':
+                # the session was aborted, use the time when the session was
+                # aborted as the end time of the lap
+                assumed_end_time = next_status['Time']
+
+            else:
+                assumed_end_time = pd.NaT
+                if drv in (car_data := getattr(self, '_car_data', {})):
+                    # when car_data is available, get the first time at which
+                    # the car's speed becomes zero after the reference time and
+                    # add 5 seconds of margin
+                    try:
+                        next_zero_speed_time = car_data[drv].loc[
+                            ((car_data[drv]['SessionTime'] > ref_time)
+                             & (car_data[drv]['Speed'] == 0.0))
+                        ].iloc[0]['SessionTime']
+                    except (IndexError, KeyError):
+                        pass
+                    else:
+                        assumed_end_time = next_zero_speed_time
+
+                if pd.isna(assumed_end_time):
+                    # still no valid timestamp extracted
+                    # fallback: use an assumed lap time of 150 seconds;
+                    # this should cover all situations but most of the time
+                    # it will be much too long
+                    assumed_end_time = ref_time + pd.Timedelta(150, 'sec')
+
+            new_last = pd.DataFrame({
+                'LapStartTime': [drv_laps['Time'].iloc[-1]],
+                'Time': [assumed_end_time],
+                'Driver': [drv_laps['Driver'].iloc[-1]],
+                'DriverNumber': [drv_laps['DriverNumber'].iloc[-1]],
+                'Team': [drv_laps['Team'].iloc[-1]],
+                'LapNumber': [drv_laps['LapNumber'].iloc[-1] + 1],
+                'Stint': [drv_laps['Stint'].iloc[-1]],
+                'Compound': [drv_laps['Compound'].iloc[-1]],
+                'TyreLife': [drv_laps['TyreLife'].iloc[-1] + 1],
+                'FreshTyre': [drv_laps['FreshTyre'].iloc[-1]],
+                'Position': [np.NaN],
+                'FastF1Generated': [True],
+                'IsAccurate': [False]
+            })
+
+            # add generated laps at the end and fix sorting at the end
+            self._laps = pd.concat([self._laps, new_last])
+            any_new = True
+
+        if any_new:
+            # re-sort and re-index to restore correct order of the laps
+            self._laps = self._laps \
+                .sort_values(by=['DriverNumber', 'LapNumber']) \
+                .reset_index(drop=True)
+
+    def _set_laps_deleted_from_rcm(self):
+        # parse race control messages to find deleted lap times and
+        # set the 'Deleted' flag in self._laps
+
+        if ((not hasattr(self, '_laps'))
+                or (not hasattr(self, '_race_control_messages'))):
+            return
+
+        # set all to False, then selectively set to True if actually deleted
+        self._laps['Deleted'] = False
+
+        msg_pattern = re.compile(
+            r"CAR (\d{1,2}) .* TIME (\d:\d\d\.\d\d\d) DELETED - (.*)"
+        )
+        timestamp_pattern = re.compile(r"\d\d:\d\d:\d\d")
+
+        for _, row in self._race_control_messages.iterrows():
+            match = msg_pattern.match(row['Message'])
+            if match:
+                drv = match[1]
+                deleted_time = to_timedelta(match[2])
+                # remove timestamp from reasons because confusingly it is given
+                # as local time at the track
+                reason = timestamp_pattern.sub("", match[3])
+                self._laps.loc[
+                    (self._laps['DriverNumber'] == drv)
+                    & (self._laps['LapTime'] == deleted_time),
+                    ('Deleted', 'IsPersonalBest', 'DeletedReason')
+                ] = (True, False, reason)
+
+    def _add_track_status_to_laps(self, laps):
+        # add track status information to each lap
+
+        track_status = getattr(self, '_track_status')
+        if track_status is None:
+            return
+
+        # first set all laps to green flag as a starting point
         laps['TrackStatus'] = '1'
 
         def applicator(new_status, current_status):
             if current_status == '1':
                 return new_status
             elif new_status not in current_status:
                 return current_status + new_status
             else:
                 return current_status
 
         if len(track_status['Time']) > 0:
             t = track_status['Time'][0]
             status = track_status['Status'][0]
-            for next_t, next_status in zip(track_status['Time'][1:], track_status['Status'][1:]):
+            for next_t, next_status in zip(track_status['Time'][1:],
+                                           track_status['Status'][1:]):
                 if status != '1':
-                    # status change partially in lap partially outside
-                    sel = (((next_t >= laps['LapStartTime']) & (laps['LapStartTime'] >= t)) |
-                           ((t <= laps['Time']) & (laps['Time'] <= next_t)))
-                    laps.loc[sel, 'TrackStatus'] = laps.loc[sel, 'TrackStatus'].apply(
-                        lambda curr: applicator(status, curr)
+                    # status change partially in lap and partially outside
+                    sel = (((next_t >= laps['LapStartTime'])
+                            & (laps['LapStartTime'] >= t))
+                           | ((t <= laps['Time']) & (laps['Time'] <= next_t)))
+
+                    laps.loc[sel, 'TrackStatus'] \
+                        = laps.loc[sel, 'TrackStatus'].apply(
+                            lambda curr: applicator(status, curr)
                     )
 
-                    # status change two times in one lap (e.g. short yellow flag)
-                    sel = ((laps['LapStartTime'] <= t) & (laps['Time'] >= next_t))
-                    laps.loc[sel, 'TrackStatus'] = laps.loc[sel, 'TrackStatus'].apply(
-                        lambda curr: applicator(status, curr)
+                    # status change two times in one lap (short yellow flag)
+                    sel = ((laps['LapStartTime'] <= t)
+                           & (laps['Time'] >= next_t))
+
+                    laps.loc[sel, 'TrackStatus'] \
+                        = laps.loc[sel, 'TrackStatus'].apply(
+                            lambda curr: applicator(status, curr)
                     )
 
                 t = next_t
                 status = next_status
 
             sel = laps['LapStartTime'] >= t
             laps.loc[sel, 'TrackStatus'] = laps.loc[sel, 'TrackStatus'].apply(
                 lambda curr: applicator(status, curr)
             )
 
+    @soft_exceptions("first lap time",
+                     "Failed to add first lap time from Ergast!",
+                     _logger)
+    def _add_first_lap_time_from_ergast(self):
+        # The f1 api does not provide a value for the first lap time.
+        # For races, lap times are also available on Ergast -> add the
+        # first lap time from there
+
+        if not self.name == 'Race':
+            return
+
+        # load lap times for first lap from Ergast and add driver number
+        # based on driver id from results
+        response = self._ergast.get_lap_times(
+            self.event.year, self.event.RoundNumber, lap_number=1
+        )
+        if response.description.empty:
+            _logger.warning("Cannot load lap times for first lap from Ergast. "
+                            "Timing data is not available for this session.")
+            return  # no data returned
+
+        first_lap_times = response.content[0].set_index('driverId')
+
+        drv_num_ref = self.results \
+                          .loc[:, ('DriverNumber', 'DriverId')] \
+                          .set_index('DriverId')
+        first_lap_times = first_lap_times.join(drv_num_ref)
+
+        # set the first lap time for each driver individually
+        # (.merge, .update, ... not easily usable because not shared index)
+        failed_drvs = list()
+        for _, row in first_lap_times.iterrows():
+            drv = row['DriverNumber']
+            try:
+                self._laps.loc[
+                    (self._laps['LapNumber'] == 1)
+                    & (self._laps['DriverNumber'] == drv),
+                    'LapTime'
+                ] = row['time']
+            except Exception as exc:
+                _logger.debug(f"Failed to add first lap time for "
+                              f"driver '{drv}'", exc_info=exc)
+                failed_drvs.append(drv)
+
+        if failed_drvs:
+            _logger.warning(f"Failed to add first lap time from Ergast for "
+                            f"drivers: {failed_drvs}")
+
+    @soft_exceptions("track status data", "Failed to load track status data!",
+                     _logger)
+    def _load_track_status_data(self, livedata=None):
+        track_status = api.track_status_data(self.api_path, livedata=livedata)
+        self._track_status = pd.DataFrame(track_status)
+        if not self._track_status.size:
+            _logger.warning("Could not load any valid session status "
+                            "information!")
+
+    @soft_exceptions("total lap count", "Failed to load total lap count!",
+                     _logger)
+    def _load_total_lap_count(self, livedata=None):
+        # Get the number of originally scheduled laps
+        # Lap count data only exists for race-like sessions.
+        if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
+            try:
+                lap_count = api.lap_count(self.api_path, livedata=livedata)
+                # A race-like session can have multiple intended total laps,
+                # the first one being the original schedule
+                self._total_laps = lap_count['TotalLaps'][0]
+            except IndexError:
+                self._total_laps = None
+                _logger.warning("No lap count data for this session.")
         else:
-            logging.warning("Could not load any valid session status information!")
-        self._laps = Laps(laps, session=self)
-        self._check_lap_accuracy()
+            self._total_laps = None
+
+    @soft_exceptions("session status data",
+                     "Failed to load session status data!", _logger)
+    def _load_session_status_data(self, livedata=None):
+        # check when a session was started; for a race this indicates the
+        # start of the race
+        session_status = api.session_status_data(self.api_path,
+                                                 livedata=livedata)
+        for i in range(len(session_status['Status'])):
+            if session_status['Status'][i] == 'Started':
+                self._session_start_time = session_status['Time'][i]
+                break
+        else:
+            _logger.warning("Failed to determine `Session.session_start_time`")
+            self._session_start_time = None
+        self._session_status = pd.DataFrame(session_status)
 
     def __fix_tyre_info(self, df):
         # Sometimes later corrections of tyre info are sent through the api.
         # These updates only set values that need to be changed and all other
         # values are none-like. Therefore, if correction updates exist, for
         # each stint the first received information is taken and then
         # iteratively updated with non-NA values from all updates for this
@@ -1485,15 +1716,15 @@
                 # iterate over all messages (rows) that were received for this
                 # stint
                 if pd.isna(corrected.loc[i]).all():
                     # first message: set as a whole (performance)
                     corrected.loc[i] = row
                     continue
 
-                for key, value in row.iteritems():
+                for key, value in row.items():
                     # correction: update existing values only if new value
                     # is non-na
                     if pd.isna(value):
                         continue
                     if (key == 'Time') and not pd.isna(corrected.loc[i, key]):
                         # always keep first time stamp instead of corrected
                         # corresponds to pit stop time
@@ -1506,23 +1737,23 @@
 
         return corrected
 
     def _check_lap_accuracy(self):
         """Accuracy validation; simples yes/no validation
         Currently only relies on provided information which can't catch all problems"""
         # TODO: check for outliers in lap start position
-        # self.laps['IsAccurate'] = False  # default should be not accurate
         for drv in self.drivers:
             is_accurate = list()
             prev_lap = None
             integrity_errors = 0
             for _, lap in self.laps[self.laps['DriverNumber'] == drv].iterrows():
                 # require existence, non-existence and specific values for some variables
                 check_1 = (pd.isnull(lap['PitInTime'])
                            & pd.isnull(lap['PitOutTime'])
+                           & (not lap['FastF1Generated'])
                            & (lap['TrackStatus'] in ('1', '2'))  # slightly paranoid, allow only green and yellow flag
                            & (not pd.isnull(lap['LapTime']))
                            & (not pd.isnull(lap['Sector1Time']))
                            & (not pd.isnull(lap['Sector2Time']))
                            & (not pd.isnull(lap['Sector3Time'])))
 
                 if check_1:  # only do check 2 if all necessary values for this check are even available
@@ -1544,168 +1775,201 @@
 
                 result = check_1 and check_2 and check_3
                 is_accurate.append(result)
                 prev_lap = lap
 
             if len(is_accurate) > 0:
                 self._laps.loc[self.laps['DriverNumber'] == drv, 'IsAccurate'] = is_accurate
+            else:
+                _logger.warning("Failed to perform lap accuracy check - all "
+                                "laps marked as inaccurate.")
+                self.laps['IsAccurate'] = False  # default should be inaccurate
+
+            # necessary to explicitly cast to bool
+            self._laps[['IsAccurate']] \
+                = self._laps[['IsAccurate']].astype(bool)
 
             if integrity_errors > 0:
-                logging.warning(f"Driver {drv: >2}: Lap timing integrity check failed for {integrity_errors} lap(s)")
+                _logger.warning(
+                    f"Driver {drv: >2}: Lap timing integrity check "
+                    f"failed for {integrity_errors} lap(s)")
 
+    @soft_exceptions("results", "Failed to load results data!", _logger)
     def _load_drivers_results(self, *, livedata=None):
         # get list of drivers
         driver_info = None
         if self.f1_api_support:
             # load driver info from f1 api
             driver_info = self._drivers_from_f1_api(livedata=livedata)
 
         if not driver_info:
             if not self.event.is_testing():
                 # load driver info and results from ergast
                 # (season 2017 and older or fallback from f1 api)
                 driver_info = self._drivers_results_from_ergast(
                     load_drivers=True, load_results=True
                 )
-                self._results = SessionResults(
-                    driver_info, index=driver_info['DriverNumber'],
-                    force_default_cols=True
-                )
+                if driver_info is not None:
+                    self._results = SessionResults(
+                        driver_info, force_default_cols=True
+                    )
+                    self._results.index = driver_info['DriverNumber']
             else:
-                logging.warning("Failed to load driver list and "
+                _logger.warning("Failed to load driver list and "
                                 "session results!")
                 self._results = SessionResults(force_default_cols=True)
 
         else:
             # extend existing driver info (f1 api) with results from ergast
             drivers = pd.DataFrame(driver_info,
                                    index=driver_info['DriverNumber'])
             if not self.event.is_testing():
                 r = self._drivers_results_from_ergast(load_results=True)
             else:
                 r = None
 
-            if r:
+            if r is not None:
                 # join driver info and session results
-                results = pd.DataFrame(r).set_index('DriverNumber')
-                self._results = SessionResults(drivers.join(results),
-                                               force_default_cols=True)
+                results = r.set_index('DriverNumber')
+                self._results = SessionResults(
+                    drivers.join(results, how='outer'), force_default_cols=True
+                )
+                self._results['DriverNumber'] = self._results.index
             else:
                 # return driver info without session results
                 self._results = SessionResults(drivers,
                                                force_default_cols=True)
 
         if (dupl_mask := self._results.index.duplicated()).any():
             dupl_drv = list(self._results.index[dupl_mask])
-            logging.warning("Session results contain duplicate entries for "
+            _logger.warning(f"Session results contain duplicate entries for "
                             f"driver(s) {dupl_drv}")
 
         if 'Position' in self._results:
             self._results = self._results.sort_values('Position')
 
     def _drivers_from_f1_api(self, *, livedata=None):
         try:
             f1di = api.driver_info(self.api_path, livedata=livedata)
         except Exception as exc:
-            logging.warning("Failed to load extended driver information!")
-            logging.debug("Exception while loading driver list", exc_info=exc)
+            _logger.warning("Failed to load extended driver information!")
+            _logger.debug("Exception while loading driver list", exc_info=exc)
             driver_info = {}
         else:
             driver_info = collections.defaultdict(list)
             for key1, key2 in {
                 'RacingNumber': 'DriverNumber',
                 'BroadcastName': 'BroadcastName',
                 'Tla': 'Abbreviation', 'TeamName': 'TeamName',
                 'TeamColour': 'TeamColor', 'FirstName': 'FirstName',
-                'LastName': 'LastName'
+                'LastName': 'LastName', 'HeadshotUrl': 'HeadshotUrl',
+                'CountryCode': 'CountryCode'
             }.items():
                 for entry in f1di.values():
                     driver_info[key2].append(entry.get(key1))
             if 'FirstName' in driver_info and 'LastName' in driver_info:
                 for first, last in zip(driver_info['FirstName'],
                                        driver_info['LastName']):
                     driver_info['FullName'].append(f"{first} {last}")
         return driver_info
 
-    def _drivers_results_from_ergast(self, *, load_drivers=False,
-                                     load_results=False):
+    def _drivers_results_from_ergast(
+            self, *, load_drivers=False, load_results=False
+    ) -> Optional[pd.DataFrame]:
         if self.name in ('Qualifying', 'Sprint Qualifying', 'Sprint', 'Race'):
             session_name = self.name
         else:
             # this is a practice session, use drivers from race session but
             # don't load results
             session_name = 'Race'
             load_results = False
 
-        d = collections.defaultdict(list)
-        try:
-            data = ergast.fetch_results(
-                self.event.year, self.event['RoundNumber'], session_name
-            )
-        except Exception as exc:
-            logging.warning("Failed to load data from Ergast API! "
-                            "(This is expected for recent sessions)")
-            logging.debug("Ergast failure traceback:", exc_info=exc)
-            return d
-
-        time0 = None
-        for r in data:
-            d['DriverNumber'].append(r.get('number'))
-            if load_drivers:
-                d['Abbreviation'].append(
-                    recursive_dict_get(r, 'Driver', 'code',
-                                       default_none=True))
-                first_name = recursive_dict_get(r, 'Driver', 'givenName',
-                                                default_none=True)
-                last_name = recursive_dict_get(r, 'Driver', 'familyName',
-                                               default_none=True)
-                d['FirstName'].append(first_name)
-                d['LastName'].append(last_name)
-                d['FullName'].append(f"{first_name} {last_name}")
-                d['TeamName'].append(
-                    recursive_dict_get(r, 'Constructor', 'name',
-                                       default_none=True))
-            if load_results:
-                d['Position'].append(r.get('position'))
-                d['GridPosition'].append(r.get('grid'))
-                d['Q1'].append(to_timedelta(r.get('Q1')))
-                d['Q2'].append(to_timedelta(r.get('Q2')))
-                d['Q3'].append(to_timedelta(r.get('Q3')))
-                if time0 is None:
-                    ts = recursive_dict_get(r, 'Time', 'time',
-                                            default_none=True)
-                    if ts:
-                        time0 = to_timedelta(ts)
-                    else:
-                        time0 = pd.NaT
-                    d['Time'].append(time0)
-                else:
-                    ts = recursive_dict_get(r, 'Time', 'time',
-                                            default_none=True)
-                    if ts:
-                        dt = to_timedelta(ts)
-                    else:
-                        dt = pd.NaT
-                    d['Time'].append(time0 + dt)
-                d['Status'].append(r.get('status'))
-                d['Points'].append(r.get('points'))
+        @soft_exceptions("ergast result data",
+                         "Failed to load result data from Ergast! (This is "
+                         "expected for recent sessions)",
+                         _logger)
+        def _get_data():
+            if session_name == 'Race':
+                return self._ergast.get_race_results(
+                    self.event.year, self.event.RoundNumber
+                ).content[0]
+            elif session_name == 'Qualifying':
+                return self._ergast.get_qualifying_results(
+                    self.event.year, self.event.RoundNumber
+                ).content[0]
+            else:
+                return self._ergast.get_sprint_results(
+                    self.event.year, self.event.RoundNumber
+                ).content[0]
+
+        data = _get_data()
+
+        if data is None:
+            return None
+
+        rename_return = {
+            'number': 'DriverNumber',
+            'driverId': 'DriverId',
+            'constructorId': 'TeamId'
+        }
+
+        if load_drivers:
+            rename_return.update({
+                'driverCode': 'Abbreviation',
+                'givenName': 'FirstName',
+                'familyName': 'LastName',
+                'constructorName': 'TeamName',
+            })
+
+        if load_results:
+            rename_return.update({
+                'position': 'Position',
+            })
+
+            if session_name in ('Sprint Qualifying', 'Sprint', 'Race'):
+                rename_return.update({
+                    'positionText': 'ClassifiedPosition',
+                    'grid': 'GridPosition',
+                    'status': 'Status',
+                    'points': 'Points',
+                    'totalRaceTime': 'Time'
+                })
+
+            if session_name == 'Qualifying':
+                rename_return.update({
+                    'Q1': 'Q1',
+                    'Q2': 'Q2',
+                    'Q3': 'Q3',
+                })
+
+        d = data.loc[:, list(rename_return.keys())] \
+            .rename(columns=rename_return) \
+            .astype({'DriverNumber': 'str'})
+
+        if load_drivers:
+            d['FullName'] = d['FirstName'] + " " + d['LastName']
 
         return d
 
+    @soft_exceptions("weather data", "Failed to load weather data!", _logger)
     def _load_weather_data(self, livedata=None):
         weather_data = api.weather_data(self.api_path, livedata=livedata)
         weather_df = pd.DataFrame(weather_data)
         self._weather_data = weather_df
 
+    @soft_exceptions("race control messages",
+                     "Failed to load race control messages!", _logger)
     def _load_race_control_messages(self, livedata=None):
         race_control_messages = api.race_control_messages(self.api_path,
                                                           livedata=livedata)
         race_control_df = pd.DataFrame(race_control_messages)
         self._race_control_messages = race_control_df
 
+    @soft_exceptions("telemetry data", "Failed to load telemetry data!",
+                     _logger)
     def _load_telemetry(self, livedata=None):
         """Load telemetry data from the API.
 
         This method can only be called after :meth:`load_laps` has been
         called. You will usually just want to call :meth:`load_laps` with
         the optional ``with_telemetry=True`` argument instead of calling this
         method separately. The result will be the same.
@@ -1755,26 +2019,28 @@
             drv_pos['Time'] = drv_pos['Date'] - self.t0_date
             drv_car['SessionTime'] = drv_car['Time']
             drv_pos['SessionTime'] = drv_pos['Time']
 
             self._car_data[drv] = drv_car
             self._pos_data[drv] = drv_pos
 
-        self._laps['LapStartDate'] = self._laps['LapStartTime'] + self.t0_date
+        if hasattr(self, '_laps'):
+            self._laps['LapStartDate'] \
+                = self._laps['LapStartTime'] + self.t0_date
 
-    def get_driver(self, identifier):
+    def get_driver(self, identifier) -> "DriverResult":
         """
         Get a driver object which contains additional information about a driver.
 
         Args:
             identifier (str): driver's three letter identifier (for
                 example 'VER') or driver number as string
 
         Returns:
-            instance of :class:`Driver`
+            instance of :class:`DriverResult`
         """
         mask = ((self.results['Abbreviation'] == identifier)
                 | (self.results['DriverNumber'] == identifier))
         if not mask.any():
             raise ValueError(f"Invalid driver identifier '{identifier}'")
         return self.results[mask].iloc[0]
 
@@ -1797,15 +2063,19 @@
 
         for data in (car_data, pos_data):
             for drv in data.keys():
                 new_offset = max(data[drv]['Date'] - data[drv]['Time'])
                 if date_offset is None or new_offset > date_offset:
                     date_offset = new_offset
 
-        self._t0_date = date_offset.round('ms')
+        if date_offset is None:
+            self._t0_date = None
+            _logger.warning("Failed to determine `Session.t0_date`!")
+        else:
+            self._t0_date = date_offset.round('ms')
 
 
 class Laps(pd.DataFrame):
     """Object for accessing lap (timing) data of multiple laps.
 
     Args:
         *args (any): passed through to :class:`pandas.DataFrame` super class
@@ -1840,16 +2110,16 @@
         - **Time** (pandas.Timedelta): Session time when the lap time was
           set (end of lap)
         - **Driver** (string): Three letter driver identifier
         - **DriverNumber** (str): Driver number
         - **LapTime** (pandas.Timedelta): Recorded lap time.
           Officially deleted lap times will *not* be deleted here.
           Deleting laps is currently not supported.
-        - **LapNumber** (int): Recorded lap number
-        - **Stint** (int): Stint number
+        - **LapNumber** (float): Recorded lap number
+        - **Stint** (float): Stint number
         - **PitOutTime** (pandas.Timedelta): Session time when car exited
           the pit
         - **PitInTime** (pandas.Timedelta): Session time when car entered
           the pit
         - **Sector1Time** (pandas.Timedelta): Sector 1 recorded time
         - **Sector2Time** (pandas.Timedelta): Sector 2 recorded time
         - **Sector3Time** (pandas.Timedelta): Sector 3 recorded time
@@ -1862,16 +2132,16 @@
         - **SpeedI1** (float): Speedtrap sector 1 [km/h]
         - **SpeedI2** (float): Speedtrap sector 2 [km/h]
         - **SpeedFL** (float): Speedtrap at finish line [km/h]
         - **SpeedST** (float): Speedtrap on longest straight (Not sure) [km/h]
         - **IsPersonalBest** (bool): Flag that indicates whether this lap is
           the official personal best lap of a driver. If any lap of a driver
           is quicker than their respective personal best lap, this means that
-          the quicker lap is invalid and not counted. This can happen it the
-          track limits were execeeded, for example.
+          the quicker lap is invalid and not counted. For example, this can
+          happen if the track limits were exceeded.
         - **Compound** (str): Tyres event specific compound name: SOFT, MEDIUM,
           HARD, INTERMEDIATE, WET (the actual underlying compounds C1 to C5 are
           not differentiated).
         - **TyreLife** (float): Laps driven on this tire (includes laps in
           other sessions for used sets of tires)
         - **FreshTyre** (bool): Tyre had TyreLife=0 at stint start, i.e.
           was a new tire
@@ -1882,14 +2152,27 @@
           the lap
         - **TrackStatus** (str): A string that contains track status numbers
           for all track status that occurred
           during this lap. The meaning of the track status numbers is
           explained in :func:`fastf1.api.track_status_data`.
           For filtering laps by track status, you may want to use
           :func:`Laps.pick_track_status`.
+        - **Position** (float): Position of the driver at the end of each lap.
+          This value is NaN for FP1, FP2, FP3 and Qualifying as well as for
+          crash laps.
+        - **Deleted** (Optional[bool]): Indicates that a lap was deleted by
+          the stewards, for example because of a track limits violation.
+          This data is only available when race control messages are loaded.
+        - **DeletedReason** (str): Gives the reason for a lap time deletion.
+          This data is only available when race control messages are loaded.
+        - **FastF1Generated** (bool): Indicates that this lap was added by
+          FastF1. Such a lap will generally have very limited information
+          available and information is partly interpolated or based on
+          reasonable assumptions. Cases were this is used are, for example,
+          when a partial last lap is added for drivers that retired on track.
         - **IsAccurate** (bool): Indicates that the lap start and end time are
           synced correctly with other laps. Do not confuse this with the
           accuracy of the lap time or sector times. They are always considered
           to be accurate if they exist!
           If this value is True, the lap has passed as basic accuracy check
           for timing data. This does not guarantee accuracy but laps marked
           as inaccurate need to be handled with caution. They might contain
@@ -1906,45 +2189,116 @@
             - has a value for lap time and all sector times
             - the sum of the sector times matches the lap time
               (If this were to ever occur, it would also be logged separately
               as a data integrity error. You usually don't need to worry about
               this.)
     """
 
+    _COL_TYPES = {
+        'Time': 'timedelta64[ns]',
+        'Driver': str,
+        'DriverNumber': str,
+        'LapTime': 'timedelta64[ns]',
+        'LapNumber': 'float64',
+        'Stint': 'float64',
+        'PitOutTime': 'timedelta64[ns]',
+        'PitInTime': 'timedelta64[ns]',
+        'Sector1Time': 'timedelta64[ns]',
+        'Sector2Time': 'timedelta64[ns]',
+        'Sector3Time': 'timedelta64[ns]',
+        'Sector1SessionTime': 'timedelta64[ns]',
+        'Sector2SessionTime': 'timedelta64[ns]',
+        'Sector3SessionTime': 'timedelta64[ns]',
+        'SpeedI1': 'float64',
+        'SpeedI2': 'float64',
+        'SpeedFL': 'float64',
+        'SpeedST': 'float64',
+        'IsPersonalBest': bool,
+        'Compound': str,
+        'TyreLife': 'float64',
+        'FreshTyre': bool,
+        'Team': str,
+        'LapStartTime': 'timedelta64[ns]',
+        'LapStartDate': 'datetime64[ns]',
+        'TrackStatus': str,
+        'Position': 'float64',  # need to support NaN
+        'Deleted': Optional[bool],
+        'DeletedReason': str,
+        'FastF1Generated': bool,
+        'IsAccurate': bool
+    }
+
     _metadata = ['session']
+    _internal_names = pd.DataFrame._internal_names \
+        + ['base_class_view', 'telemetry']
+    _internal_names_set = set(_internal_names)
 
     QUICKLAP_THRESHOLD = 1.07
     """Used to determine 'quick' laps. Defaults to the 107% rule."""
 
-    def __init__(self, *args, session=None, **kwargs):
+    def __init__(self,
+                 *args,
+                 session: Optional[Session] = None,
+                 force_default_cols: bool = False,
+                 **kwargs):
+
+        if force_default_cols:
+            kwargs['columns'] = list(self._COL_TYPES.keys())
+
         super().__init__(*args, **kwargs)
+
+        if force_default_cols:
+            # apply column specific dtypes
+            for col, _type in self._COL_TYPES.items():
+                if col not in self.columns:
+                    continue
+                convert = True
+                if self[col].isna().all():
+                    if isinstance(_type, str):
+                        self[col] = pd.Series(dtype=_type)
+                    elif type(None) in typing.get_args(_type):
+                        # column is optional, cannot force dtype, set to None
+                        self[col] = None
+                        convert = False
+                    else:
+                        self[col] = _type()
+
+                if convert:
+                    self[col] = self[col].astype(_type)
+
         self.session = session
 
     @property
     def _constructor(self):
         def _new(*args, **kwargs):
             return Laps(*args, **kwargs).__finalize__(self)
 
         return _new
 
     @property
     def _constructor_sliced(self):
         def _new(*args, **kwargs):
+            name = kwargs.get('name')
+            if name and (name in self.columns):
+                # vertical slice
+                return pd.Series(*args, **kwargs).__finalize__(self)
+
+            # horizontal slice
             return Lap(*args, **kwargs).__finalize__(self)
 
         return _new
 
     @property
     def base_class_view(self):
         """For a nicer debugging experience; can now view as
         dataframe in various IDEs"""
         return pd.DataFrame(self)
 
     @cached_property
-    def telemetry(self):
+    def telemetry(self) -> Telemetry:
         """Telemetry data for all laps in `self`
 
         This is a cached (!) property for :meth:`get_telemetry`. It will return the same value as `get_telemetry`
         but cache the result so that the involved processing is only done once.
 
         This is mainly provided for convenience and backwards compatibility.
 
@@ -1952,15 +2306,15 @@
 
         .. note:: Telemetry can only be returned if `self` contains laps of one driver only.
 
         Returns:
             instance of :class:`Telemetry`"""
         return self.get_telemetry()
 
-    def get_telemetry(self):
+    def get_telemetry(self) -> Telemetry:
         """Telemetry data for all laps in `self`
 
         Telemetry data is the result of merging the returned data from :meth:`get_car_data` and :meth:`get_pos_data`.
         This means that telemetry data at least partially contains interpolated values! Telemetry data additionally
         already has computed channels added (e.g. Distance).
 
         This method is provided for convenience and compatibility reasons. But using it does usually not produce
@@ -1974,26 +2328,27 @@
 
         Returns:
             instance of :class:`Telemetry`
         """
         pos_data = self.get_pos_data(pad=1, pad_side='both')
         car_data = self.get_car_data(pad=1, pad_side='both')
 
-        # calculate driver ahead from from data without padding to
+        # calculate driver ahead from data without padding to
         # prevent out of bounds errors
-        drv_ahead = car_data.iloc[1:-1].add_driver_ahead() \
+        drv_ahead = car_data.iloc[1:-1] \
+            .add_driver_ahead() \
             .loc[:, ('DriverAhead', 'DistanceToDriverAhead',
                      'Date', 'Time', 'SessionTime')]
 
         car_data = car_data.add_distance().add_relative_distance()
         car_data = car_data.merge_channels(drv_ahead)
         merged = pos_data.merge_channels(car_data)
         return merged.slice_by_lap(self, interpolate_edges=True)
 
-    def get_car_data(self, **kwargs):
+    def get_car_data(self, **kwargs) -> Telemetry:
         """Car data for all laps in `self`
 
         Slices the car data in :attr:`Session.car_data` using this set of laps and returns the result.
 
         The data returned by this method does not contain computed telemetry channels. The can be added by calling the
         appropriate `add_*()` method on the returned telemetry object..
 
@@ -2010,15 +2365,15 @@
             raise ValueError("Cannot slice telemetry because self contains no driver number!")
         if len(drv_num) > 1:
             raise ValueError("Cannot slice telemetry because self contains Laps of multiple drivers!")
         drv_num = drv_num[0]
         car_data = self.session.car_data[drv_num].slice_by_lap(self, **kwargs).reset_index(drop=True)
         return car_data
 
-    def get_pos_data(self, **kwargs):
+    def get_pos_data(self, **kwargs) -> Telemetry:
         """Pos data for all laps in `self`
 
         Slices the position data in :attr:`Session.pos_data` using this set of laps and returns the result.
 
         .. note:: Position data can only be returned if `self` contains laps of one driver only.
 
         Args:
@@ -2032,15 +2387,15 @@
             raise ValueError("Cannot slice telemetry because self contains no driver number!")
         if len(drv_num) > 1:
             raise ValueError("Cannot slice telemetry because self contains Laps of multiple drivers!")
         drv_num = drv_num[0]
         pos_data = self.session.pos_data[drv_num].slice_by_lap(self, **kwargs).reset_index(drop=True)
         return pos_data
 
-    def get_weather_data(self):
+    def get_weather_data(self) -> pd.DataFrame:
         """Return weather data for each lap in self.
 
         Weather data is updated once per minute. This means that there are
         usually one or two data points per lap. This function will always
         return only one data point per lap:
 
            - The first value within the duration of a lap
@@ -2090,36 +2445,50 @@
             >>> laps = session.laps
             >>> laps = laps.reset_index(drop=True)
             >>> weather_data = weather_data.reset_index(drop=True)
 
             # exclude the 'Time' column from weather data when joining
             >>> joined = pd.concat([laps, weather_data.loc[:, ~(weather_data.columns == 'Time')]], axis=1)
             >>> print(joined)
-                                  Time DriverNumber  ... WindDirection  WindSpeed
-            0   0 days 00:21:01.358000           16  ...           212        2.0
-            1   0 days 00:22:21.775000           16  ...           207        2.7
-            2   0 days 00:24:03.991000           16  ...           210        2.3
-            3   0 days 00:25:24.117000           16  ...           207        3.2
-            4   0 days 00:27:09.461000           16  ...           238        1.8
-            ..                     ...          ...  ...           ...        ...
-            270 0 days 00:36:38.150000           88  ...           192        0.9
-            271 0 days 00:38:37.508000           88  ...           213        0.9
-            272 0 days 00:33:27.227000           33  ...           183        1.3
-            273 0 days 00:35:05.865000           33  ...           272        0.8
-            274 0 days 00:36:47.787000           33  ...           339        1.1
+                                  Time Driver  ... WindDirection WindSpeed
+            0   0 days 00:21:01.358000    LEC  ...           212       2.0
+            1   0 days 00:22:21.775000    LEC  ...           207       2.7
+            2   0 days 00:24:03.991000    LEC  ...           210       2.3
+            3   0 days 00:25:24.117000    LEC  ...           207       3.2
+            4   0 days 00:27:09.461000    LEC  ...           238       1.8
+            ..                     ...    ...  ...           ...       ...
+            270 0 days 00:36:38.150000    KUB  ...           192       0.9
+            271 0 days 00:38:37.508000    KUB  ...           213       0.9
+            272 0 days 00:33:27.227000    VER  ...           183       1.3
+            273 0 days 00:35:05.865000    VER  ...           272       0.8
+            274 0 days 00:36:47.787000    VER  ...           339       1.1
             <BLANKLINE>
-            [275 rows x 33 columns]
+            [275 rows x 38 columns]
         """
         wd = [lap.get_weather_data() for _, lap in self.iterrows()]
         if wd:
             return pd.concat(wd, axis=1).T
         else:
             return pd.DataFrame(columns=self.session.weather_data.columns)
 
-    def pick_driver(self, identifier):
+    def pick_lap(self, lap_number: int) -> "Laps":
+        """Return all laps of a specific LapNumber in self based on LapNumber
+
+            lap_1 = ff1.pick_lap(1)
+            lap_25 = ff1.pick_lap(25)
+
+        Args:
+            lap_number (int): Lap number
+
+        Returns:
+            instance of :class:`Laps`
+        """
+        return self[self['LapNumber'] == lap_number]
+
+    def pick_driver(self, identifier: Union[int, str]) -> "Laps":
         """Return all laps of a specific driver in self based on the driver's
         three letters identifier or based on the driver number ::
 
             perez_laps = ff1.pick_driver('PER')
             bottas_laps = ff1.pick_driver(77)
             kimi_laps = ff1.pick_driver('RAI')
 
@@ -2131,15 +2500,15 @@
         """
         identifier = str(identifier)
         if identifier.isdigit():
             return self[self['DriverNumber'] == identifier]
         else:
             return self[self['Driver'] == identifier]
 
-    def pick_drivers(self, identifiers):
+    def pick_drivers(self, identifiers: Iterable[Union[int, str]]) -> "Laps":
         """Return all laps of the specified drivers in self based on the
         drivers' three letters identifier or based on the driver number. This
         is the same as :meth:`Laps.pick_driver` but for multiple drivers
         at once. ::
 
             some_drivers_laps = ff1.pick_drivers([5, 'BOT', 7])
 
@@ -2151,15 +2520,15 @@
         """
         names = [n for n in identifiers if not str(n).isdigit()]
         numbers = [str(n) for n in identifiers if str(n).isdigit()]
         drv, num = self['Driver'], self['DriverNumber']
 
         return self[(drv.isin(names) | num.isin(numbers))]
 
-    def pick_team(self, name):
+    def pick_team(self, name: str) -> "Laps":
         """Return all laps of a specific team in self based on the
         team's name ::
 
             mercedes = ff1.pick_team('Mercedes')
             alfa_romeo = ff1.pick_team('Alfa Romeo')
 
         Have a look to :attr:`fastf1.plotting.TEAM_COLORS` for a quick reference on team names.
@@ -2168,30 +2537,30 @@
             name (str): Team name
 
         Returns:
             instance of :class:`Laps`
         """
         return self[self['Team'] == name]
 
-    def pick_teams(self, names):
+    def pick_teams(self, names: Iterable[str]) -> "Laps":
         """Return all laps of the specified teams in self based on the teams'
         name. This is the same as :meth:`Laps.pick_team` but for multiple
         teams at once. ::
 
             some_drivers_laps = ff1.pick_teams(['Mercedes', 'Williams'])
 
         Args:
             names (iterable): Multiple team names
 
         Returns:
             instance of :class:`Laps`
         """
         return self[self['Team'].isin(names)]
 
-    def pick_fastest(self, only_by_time=False):
+    def pick_fastest(self, only_by_time: bool = False) -> "Lap":
         """Return the lap with the fastest lap time.
 
         This method will by default return the quickest lap out of self, that
         is also marked as personal best lap of a driver.
 
         If the quickest lap by lap time is not marked as personal best, this
         means that it was not counted. This can be the case for example, if
@@ -2214,24 +2583,24 @@
         if only_by_time:
             laps = self  # all laps
         else:
             # select only laps marked as personal fastest
             laps = self.loc[self['IsPersonalBest'] == True]  # noqa: E712 comparison with True
 
         if not laps.size:
-            return Lap(index=self.columns)
+            return Lap(index=self.columns, dtype=object).__finalize__(self)
 
         lap = laps.loc[laps['LapTime'].idxmin()]
         if isinstance(lap, pd.DataFrame):
             # More laps, same time
             lap = lap.iloc[0]  # take first clocked
 
         return lap
 
-    def pick_quicklaps(self, threshold=None):
+    def pick_quicklaps(self, threshold: Optional[float] = None) -> "Laps":
         """Return all laps with `LapTime` faster than a certain limit. By
         default the threshold is 107% of the best `LapTime` of all laps
         in self.
 
         Args:
             threshold (optional, float): custom threshold coefficent
                 (e.g. 1.05 for 105%)
@@ -2241,26 +2610,26 @@
         """
         if threshold is None:
             threshold = Laps.QUICKLAP_THRESHOLD
         time_threshold = self['LapTime'].min() * threshold
 
         return self[self['LapTime'] < time_threshold]
 
-    def pick_tyre(self, compound):
+    def pick_tyre(self, compound: str) -> "Laps":
         """Return all laps in self which were done on a specific compound.
 
         Args:
             compound (string): may be "SOFT", "MEDIUM", "HARD", "INTERMEDIATE" or "WET"
 
         Returns:
             instance of :class:`Laps`
         """
         return self[self['Compound'] == compound]
 
-    def pick_track_status(self, status, how='equals'):
+    def pick_track_status(self, status: str, how: str = 'equals') -> "Laps":
         """Return all laps set under a specific track status.
 
         Args:
             status (str): The track status as a string, e.g. '1'
             how (str): one of 'equals'/'contains'
                 For example, if how='equals', status='2' will only match '2'.
                 If how='contains', status='2' will also match '267' and similar
@@ -2270,32 +2639,77 @@
         if how == 'equals':
             return self[self['TrackStatus'] == status]
         elif how == 'contains':
             return self[self['TrackStatus'].str.contains(status, regex=False)]
         else:
             raise ValueError(f"Invalid value '{how}' for kwarg 'how'")
 
-    def pick_wo_box(self):
+    def pick_wo_box(self) -> "Laps":
         """Return all laps which are NOT in laps or out laps.
 
         Returns:
             instance of :class:`Laps`
         """
         return self[pd.isnull(self['PitInTime']) & pd.isnull(self['PitOutTime'])]
 
-    def pick_accurate(self):
+    def pick_accurate(self) -> "Laps":
         """Return all laps which pass the accuracy validation check
         (lap['IsAccurate'] is True).
 
         Returns:
             instance of :class:`Laps`
         """
         return self[self['IsAccurate']]
 
-    def iterlaps(self, require=()):
+    def split_qualifying_sessions(self) -> List[Optional["Laps"]]:
+        """Splits a lap object into individual laps objects for each
+        qualifying session.
+
+        This method only works for qualifying sessions and requires that
+        session status data is loaded.
+
+        Example::
+
+            q1, q2, q3 = laps.split_qualifying_sessions()
+
+        Returns: Three :class:`Laps` objects, one for Q1, Q2 and Q3
+            each. If any of these sessions was cancelled, ``None`` will be
+            returned instead of :class:`Laps`.
+        """
+        if self.session.name != "Qualifying":
+            raise ValueError("Session is not a qualifying session!")
+        elif self.session.session_status is None:
+            raise ValueError("Session status data is unavailable!")
+
+        # get the timestamps for 'Started' from the session status data
+        # note that after a red flag, a session is 'Started' as well.
+        # Therefore, it is necessary to check for red flags and ignore
+        # the first 'Started' entry after a red flag.
+        split_times = list()
+        session_suspended = False
+        for _, row in self.session.session_status.iterrows():
+            if row['Status'] == 'Started':
+                if not session_suspended:
+                    split_times.append(row['Time'])
+                else:
+                    session_suspended = False
+            elif row['Status'] == 'Aborted':
+                session_suspended = True
+
+        # at the very last timestamp, to get an end for the last interval
+        split_times.append(self.session.session_status['Time'].iloc[-1])
+
+        laps = [None, None, None]
+        for i in range(len(split_times) - 1):
+            laps[i] = self[(self['Time'] > split_times[i])
+                           & (self['Time'] < split_times[i + 1])]
+        return laps
+
+    def iterlaps(self, require: Optional[Iterable] = None) \
+            -> Iterable[Tuple[int, "Lap"]]:
         """Iterator for iterating over all laps in self.
 
         This method wraps :meth:`pandas.DataFrame.iterrows`.
         It additionally provides the `require` keyword argument.
 
         Args:
              require (optional, iterable): Require is a list of column/telemetry channel names. All names listed in
@@ -2319,41 +2733,43 @@
 class Lap(pd.Series):
     """Object for accessing lap (timing) data of a single lap.
 
     This class wraps :class:`pandas.Series`. It provides extra functionality for accessing a lap's associated
     telemetry data.
     """
     _metadata = ['session']
+    _internal_names = pd.Series._internal_names + ['telemetry']
+    _internal_names_set = set(_internal_names)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         def _new(*args, **kwargs):
             return Lap(*args, **kwargs).__finalize__(self)
 
         return _new
 
     @cached_property
-    def telemetry(self):
+    def telemetry(self) -> Telemetry:
         """Telemetry data for this lap
 
         This is a cached (!) property for :meth:`get_telemetry`. It will return the same value as `get_telemetry`
         but cache the result so that the involved processing is only done once.
 
         This is mainly provided for convenience and backwards compatibility.
 
         See :meth:`get_telemetry` for more information.
 
         Returns:
             instance of :class:`Telemetry`"""
         return self.get_telemetry()
 
-    def get_telemetry(self):
+    def get_telemetry(self) -> Telemetry:
         """Telemetry data for this lap
 
         Telemetry data is the result of merging the returned data from :meth:`get_car_data` and :meth:`get_pos_data`.
         This means that telemetry data at least partially contains interpolated values! Telemetry data additionally
         already has computed channels added (e.g. Distance).
 
         This method is provided for convenience and compatibility reasons. But using it does usually not produce
@@ -2367,24 +2783,25 @@
             instance of :class:`Telemetry`
         """
         pos_data = self.get_pos_data(pad=1, pad_side='both')
         car_data = self.get_car_data(pad=1, pad_side='both')
 
         # calculate driver ahead from from data without padding to
         # prevent out of bounds errors
-        drv_ahead = car_data.iloc[1:-1].add_driver_ahead() \
+        drv_ahead = car_data.iloc[1:-1] \
+            .add_driver_ahead() \
             .loc[:, ('DriverAhead', 'DistanceToDriverAhead',
                      'Date', 'Time', 'SessionTime')]
 
         car_data = car_data.add_distance().add_relative_distance()
         car_data = car_data.merge_channels(drv_ahead)
         merged = pos_data.merge_channels(car_data)
         return merged.slice_by_lap(self, interpolate_edges=True)
 
-    def get_car_data(self, **kwargs):
+    def get_car_data(self, **kwargs) -> Telemetry:
         """Car data for this lap
 
         Slices the car data in :attr:`Session.car_data` using this lap and returns the result.
 
         The data returned by this method does not contain computed telemetry channels. The can be added by calling the
         appropriate `add_*()` method on the returned telemetry object.
 
@@ -2393,29 +2810,29 @@
 
         Returns:
             instance of :class:`Telemetry`
         """
         car_data = self.session.car_data[self['DriverNumber']].slice_by_lap(self, **kwargs).reset_index(drop=True)
         return car_data
 
-    def get_pos_data(self, **kwargs):
+    def get_pos_data(self, **kwargs) -> Telemetry:
         """Pos data for all laps in `self`
 
         Slices the position data in :attr:`Session.pos_data` using this lap and returns the result.
 
         Args:
             **kwargs: Keyword arguments are passed to :meth:`Telemetry.slice_by_lap`
 
         Returns:
             instance of :class:`Telemetry`
         """
         pos_data = self.session.pos_data[self['DriverNumber']].slice_by_lap(self, **kwargs).reset_index(drop=True)
         return pos_data
 
-    def get_weather_data(self):
+    def get_weather_data(self) -> pd.Series:
         """Return weather data for this lap.
 
         Weather data is updated once per minute. This means that there are
         usually one or two data points per lap. This function will always
         return only one data point:
 
             - The first value within the duration of a lap
@@ -2449,16 +2866,16 @@
             Rainfall                          False
             TrackTemp                          37.8
             WindDirection                       166
             WindSpeed                           0.8
             Name: 70, dtype: object
         """
         # get first value within the duration of the lap
-        mask = ((self.session.weather_data['Time'] >= self['LapStartTime']) &
-                (self.session.weather_data['Time'] <= self['Time']))
+        mask = ((self.session.weather_data['Time'] >= self['LapStartTime'])
+                & (self.session.weather_data['Time'] <= self['Time']))
         samples = self.session.weather_data[mask]
         if not samples.empty:
             return samples.iloc[0]
 
         # fallback: get last value before the lap ended
         mask = self.session.weather_data['Time'] <= self['Time']
         samples = self.session.weather_data[mask]
@@ -2492,29 +2909,48 @@
 
         - ``FullName`` | :class:`str` |
           The drivers full name (e.g. "Pierre Gasly")
 
         - ``Abbreviation`` | :class:`str` |
           The drivers three letter abbreviation (e.g. "GAS")
 
+        - ``DriverId`` | :class:`str` |
+          ``driverId`` that is used by the Ergast API
+
         - ``TeamName`` | :class:`str` |
           The team name (short version without title sponsors)
 
         - ``TeamColor`` | :class:`str` |
           The color commonly associated with this team (hex value)
 
+        - ``TeamId`` | :class:`str` |
+          ``constructorId`` that is used by the Ergast API
+
         - ``FirstName`` | :class:`str` |
           The drivers first name
 
         - ``LastName`` | :class:`str` |
           The drivers last name
 
+        - ``HeadshotUrl`` | :class:`str` |
+          The URL to the driver's headshot
+
+        - ``CountryCode`` | :class:`str` |
+          The driver's country code (e.g. "FRA")
+
         - ``Position`` | :class:`float` |
           The drivers finishing position (values only given if session is
-          'Race', 'Qualifying' or 'Sprint Qualifying')
+          'Race', 'Qualifying' or 'Sprint Qualifying').
+
+        - ``ClassifiedPosition`` | :class:`str` |
+          The official classification result for each driver.
+          This is either an integer value if the driver is
+          officially classified or one of "R" (retired), "D" (disqualified),
+          "E" (excluded), "W" (withdrawn), "F" (failed to qualify) or
+          "N" (not classified).
 
         - ``GridPosition`` | :class:`float` |
           The drivers starting position (values only given if session is
           'Race' or 'Sprint Qualifying')
 
         - ``Q1`` | :class:`pd.Timedelta` |
           The drivers best Q1 time (values only given if session is
@@ -2535,15 +2971,15 @@
 
         - ``Status`` | :class:`str` |
           A status message to indicate if and how the driver finished the race
           or to indicate the cause of a DNF. Possible values include but are
           not limited to 'Finished', '+ 1 Lap', 'Crash', 'Gearbox', ...
           (values only given if session is 'Race' or 'Sprint Qualifying')
 
-        - ``Status`` | :class:`float` |
+        - ``Points`` | :class:`float` |
           The number of points received by each driver for their finishing
           result.
 
     By default, the session results are indexed by driver number and sorted by
     finishing position.
 
     .. note:: This class is usually not instantiated directly. You should
@@ -2560,61 +2996,74 @@
     .. versionadded:: 2.2
     """
 
     _COL_TYPES = {
         'DriverNumber': str,
         'BroadcastName': str,
         'Abbreviation': str,
+        'DriverId': str,
         'TeamName': str,
         'TeamColor': str,
+        'TeamId': str,
         'FirstName': str,
         'LastName': str,
         'FullName': str,
-        'Position': float,
-        'GridPosition': float,
+        'HeadshotUrl': str,
+        'CountryCode': str,
+        'Position': 'float64',
+        'ClassifiedPosition': str,
+        'GridPosition': 'float64',
         'Q1': 'timedelta64[ns]',
         'Q2': 'timedelta64[ns]',
         'Q3': 'timedelta64[ns]',
         'Time': 'timedelta64[ns]',
         'Status': str,
-        'Points': float
+        'Points': 'float64'
     }
 
-    _internal_names = ['base_class_view']
+    _internal_names = pd.DataFrame._internal_names + ['base_class_view']
+    _internal_names_set = set(_internal_names)
 
-    def __init__(self, *args, force_default_cols=False, **kwargs):
+    def __init__(self, *args, force_default_cols: bool = False, **kwargs):
         if force_default_cols:
             kwargs['columns'] = list(self._COL_TYPES.keys())
         super().__init__(*args, **kwargs)
 
         # apply column specific dtypes
-        for col, _type in self._COL_TYPES.items():
-            if col not in self.columns:
-                continue
-            if self[col].isna().all():
-                if _type == 'timedelta64[ns]':
-                    self[col] = pd.Series(dtype='timedelta64[ns]')
-                else:
-                    self[col] = _type()
+        if force_default_cols:
+            for col, _type in self._COL_TYPES.items():
+                if col not in self.columns:
+                    continue
+                if self[col].isna().all():
+                    if isinstance(_type, str):
+                        self[col] = pd.Series(dtype=_type)
+                    else:
+                        self[col] = _type()
 
-            self[col] = self[col].astype(_type)
+                self[col] = self[col].astype(_type)
 
     def __repr__(self):
         return self.base_class_view.__repr__()
 
     @property
     def _constructor(self):
         def _new(*args, **kwargs):
             return SessionResults(*args, **kwargs).__finalize__(self)
 
         return _new
 
     @property
     def _constructor_sliced(self):
         def _new(*args, **kwargs):
+            name = kwargs.get('name')
+            if name and (name in self.columns):
+                # vertical slice
+                return pd.Series(*args, **kwargs).__finalize__(self)
+
+            # horizontal slice
             return DriverResult(*args, **kwargs).__finalize__(self)
 
         return _new
 
     @property
     def base_class_view(self):
         """For a nicer debugging experience; can view DataFrame through
@@ -2637,122 +3086,32 @@
     Args:
         *args: passed on to :class:`pandas.Series` superclass
         **kwargs: passed on to :class:`pandas.Series` superclass
 
     .. versionadded:: 2.2
     """
 
+    _internal_names = pd.DataFrame._internal_names + ['dnf']
+    _internal_names_set = set(_internal_names)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._getattr_override = True  # TODO: remove in v2.3
 
     @property
     def _constructor(self):
         def _new(*args, **kwargs):
             return DriverResult(*args, **kwargs).__finalize__(self)
 
         return _new
 
-    def __getattribute__(self, name):
-        # TODO: remove in v2.3
-        if name == 'name' and getattr(self, '_getattr_override', False):
-            if 'FirstName' in self:
-                warnings.warn(
-                    "The `Driver.name` property is deprecated and will be"
-                    "removed in a future version.\n"
-                    "Use `Driver['FirstName']` or `Driver.FirstName` instead.",
-                    FutureWarning
-                )
-                # name may be accessed by pandas internals to, when data
-                # does not exist yet
-                return self['FirstName']
-
-        return super().__getattribute__(name)
-
-    def __repr__(self):
-        # don't show .name deprecation message when .name is accessed internally
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore',
-                                    message=r".*property is deprecated.*")
-            return super().__repr__()
-
     @property
-    def dnf(self):
+    def dnf(self) -> bool:
         """True if driver did not finish"""
         return not (self.Status[3:6] == 'Lap' or self.Status == 'Finished')
 
-    @property
-    def grid(self):
-        """Grid position
-
-        .. deprecated:: 2.2
-            Use ``Driver['GridPosition']`` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("The `Driver.grid` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Driver['GridPosition']` or `Driver.GridPosition` "
-                      "instead.", FutureWarning)
-        return self['GridPosition']
-
-    @property
-    def position(self):
-        """Finishing position
-
-        .. deprecated:: 2.2
-            Use ``Driver['Position']`` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("The `Driver.position` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Driver['Position']` or `Driver.Position` "
-                      "instead.", FutureWarning)
-        return self['Position']
-
-    @property
-    def familyname(self):
-        """Driver family name
-
-        .. deprecated:: 2.2
-            Use ``Driver['LastName']`` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("The `Driver.position` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Driver['LastName']` or `Driver.LastName` "
-                      "instead.", FutureWarning)
-        return self['LastName']
-
-    @property
-    def team(self):
-        """Team name
-
-        .. deprecated:: 2.2
-            Use ``Driver['TeamName']`` instead
-        """
-        # TODO: remove in v2.3
-        warnings.warn("The `Driver.team` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Driver['TeamName']` or `Driver.TeamName` "
-                      "instead.", FutureWarning)
-        return self['TeamName']
-
-
-class Driver:
-    """
-    .. deprecated:: 2.2
-        Use :class:`fastf1.core.DriverResult` instead
-    """
-    def __new__(cls, *args, **kwargs):
-        warnings.warn("`fastf1.core.Driver` has been deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `fastf1.core.DriverResult` instead.",
-                      FutureWarning)
-        return DriverResult()
-
 
 class DataNotLoadedError(Exception):
     """Raised if an attempt is made to access data that has not been loaded
     yet."""
     pass
```

### Comparing `fastf1-2.3.3/fastf1/ergast.py` & `fastf1-3.0.0/fastf1/ergast/legacy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 import warnings
 
-from fastf1.api import Cache
-from fastf1.version import __version__
-
-base_url = 'https://ergast.com/api/f1'
-_headers = {'User-Agent': f'FastF1/{__version__}'}
+from fastf1.req import Cache
+from fastf1.ergast.interface import BASE_URL as base_url
+from fastf1.ergast.interface import HEADERS as _headers
 
 
 def fetch_results(year, gp, session):
     """session can be 'Qualifying' or 'Race'
     mainly to port on upper level libraries
     """
     if session == 'Race':
@@ -28,35 +26,14 @@
 def fetch_season(year):
     url = f"{base_url}/{year}.json"
     return _parse_ergast(_parse_json_response(
         Cache.requests_get(url, headers=_headers))
     )
 
 
-def fetch_weekend(year, gp):
-    warnings.warn(
-        "`fetch_weekend()` is deprecated and will be"
-        "removed without a direct replacement in a "
-        "future version.",
-        FutureWarning
-    )
-    url = f"{base_url}/{year}/{gp}.json"
-    data = _parse_ergast(_parse_json_response(
-        Cache.requests_get(url, headers=_headers)
-    ))[0]
-    url = ("https://www.mapcoordinates.net/admin/component/edit/"
-           + "Vpc_MapCoordinates_Advanced_GoogleMapCoords_Component/"
-           + "Component/json-get-elevation")
-    loc = data['Circuit']['Location']
-    body = {'longitude': loc['long'], 'latitude': loc['lat']}
-    res = _parse_json_response(Cache.requests_post(url, data=body))
-    data['Circuit']['Location']['alt'] = res['elevation']
-    return data
-
-
 def fetch_day(year, gp, day):
     """day can be 'qualifying' or 'results'
     """
     url = f"{base_url}/{year}/{gp}/{day}.json"
     return _parse_json_response(Cache.requests_get(url, headers=_headers))
```

### Comparing `fastf1-2.3.3/fastf1/events.py` & `fastf1-3.0.0/fastf1/events.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,22 +41,30 @@
     Usually, this is the same as the date of the last session.
 
   - ``EventFormat`` | :class:`str` |
     The format of the event. One of 'conventional', 'sprint', 'testing'.
 
   - ``Session*`` | :class:`str` |
     The name of the session. One of 'Practice 1', 'Practice 2', 'Practice 3',
-    'Qualifying', 'Sprint Qualifying', 'Sprint Shootout' or 'Race'.
+    'Qualifying', 'Sprint', 'Sprint Shootout' or 'Race'.
     Testing sessions are considered practice.
     ``*`` denotes the number of
     the session (1, 2, 3, 4, 5).
 
-  - ``Session*Date`` | :class:`datetime` |
+  - ``Session*Date`` | :class:`pd.Timestamp` |
     The date and time at which the session is scheduled to start or was
-    scheduled to start.
+    scheduled to start as timezone-aware local timestamp.
+    (Timezone information is not available when the ``'ergast'`` backend
+    is used.)
+    ``*`` denotes the number of the session (1, 2, 3, 4, 5).
+
+  - ``Session*DateUtc`` | :class:`pd.Timestamp` |
+    The date and time at which the session is scheduled to start or was
+    scheduled to start as non-timezone-aware UTC timestamp.
+    (UTC timestamps are not available when the ``'ergast'`` backend is used.)
     ``*`` denotes the number of the session (1, 2, 3, 4, 5).
 
   - ``F1ApiSupport`` | :class:`bool` |
     Denotes whether this session is supported by the official F1 API.
     Lap timing data and telemetry data can only be loaded if this is true.
 
 
@@ -96,26 +104,24 @@
 Session identifiers
 -------------------
 
 Multiple event (schedule) related functions and methods make use of a session
 identifier to differentiate between the various sessions of one event.
 This identifier can currently be one of the following:
 
-    - session name abbreviation: ``'FP1', 'FP2', 'FP3', 'Q', 'S',
-      'SQ', 'SS', 'R'``
+    - session name abbreviation: ``'FP1', 'FP2', 'FP3', 'Q', 'S', 'SS', R'``
     - full session name: ``'Practice 1', 'Practice 2',
-      'Practice 3', 'Sprint Qualifying', 'Sprint', 'Sprint Shootout',
-      'Qualifying', 'Race'``;
-      provided names will be normalized, so that the name is case-insensitive
+      'Practice 3', 'Sprint', 'Sprint Shootout', 'Qualifying', 'Race'``;
+      provided names will be normalized, so that the name is
+      case-insensitive
     - number of the session: ``1, 2, 3, 4, 5``
 
-Note that 'Sprint' is called 'Sprint Qualifying' only in the 2021 season.
-The event name will silently be corrected if you use 'Sprint'/'S' for the 2021
-season or 'Sprint Qualifying'/'SQ' for the subsequent seasons.
-
+Note that 'Sprint Qualifying' is now always called 'Sprint'.
+The event name will silently be corrected if you use 'Sprint Qualifying'/'SQ'
+instead of 'Sprint'/'S'.
 
 Functions for accessing schedule data
 -------------------------------------
 
 The functions for accessing event schedule data are documented in
 :ref:`GeneralFunctions`.
 
@@ -149,34 +155,39 @@
     :undoc-members:
     :show-inheritance:
     :autosummary:
 
 """  # noqa: W605 invalid escape sequence (escaped space)
 import collections
 import datetime
-import logging
+import json
 import warnings
+from typing import Literal, Union, Optional
 
 import dateutil.parser
 
 with warnings.catch_warnings():
     warnings.filterwarnings(
         'ignore', message="Using slow pure-python SequenceMatcher"
     )
     # suppress that warning, it's confusing at best here, we don't need fast
     # sequence matching and the installation (on windows) requires some effort
     from thefuzz import fuzz
 
 import pandas as pd
 
-from fastf1.api import Cache
+import fastf1._api
 from fastf1.core import Session
 import fastf1.ergast
-from fastf1.utils import recursive_dict_get
+from fastf1.logger import get_logger, soft_exceptions
+from fastf1.req import Cache
+from fastf1.utils import recursive_dict_get, to_datetime, to_timedelta
+
 
+_logger = get_logger(__name__)
 
 _SESSION_TYPE_ABBREVIATIONS = {
     'R': 'Race',
     'Q': 'Qualifying',
     'S': 'Sprint',
     'SQ': 'Sprint Qualifying',
     'SS': 'Sprint Shootout',
@@ -185,38 +196,30 @@
     'FP3': 'Practice 3'
 }
 
 _SCHEDULE_BASE_URL = "https://raw.githubusercontent.com/" \
                      "theOehrly/f1schedule/master/"
 
 
-def get_session(year, gp, identifier=None, *, force_ergast=False, event=None):
+def get_session(
+        year: int,
+        gp: Union[str, int],
+        identifier: Optional[Union[int, str]] = None,
+        *,
+        backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
+        force_ergast: bool = False,
+) -> Session:
     """Create a :class:`~fastf1.core.Session` object based on year, event name
     and session identifier.
 
     .. note:: This function will return a :class:`~fastf1.core.Session`
         object, but it will not load any session specific data like lap timing,
         telemetry, ... yet. For this, you will need to call
         :func:`~fastf1.core.Session.load` on the returned object.
 
-    .. deprecated:: 2.2
-        Creating :class:`~fastf1.events.Event` objects (previously
-        :class:`fastf1.core.Weekend`) by not specifying an ``identifier`` has
-        been deprecated. Use :func:`get_event` instead.
-
-    .. deprecated:: 2.2
-        The argument ``event`` has been replaced with ``identifier`` to adhere
-        to new naming conventions.
-
-    .. deprecated:: 2.2
-        Testing sessions can no longer be created by specifying
-        ``gp='testing'``. Use :func:`get_testing_session` instead. There is
-        **no grace period** for this change. This will stop working immediately
-        with the release of v2.2!
-
     To get a testing session, use :func:`get_testing_session`.
 
     Examples:
 
         Get the second free practice of the first race of 2021 by its session
         name abbreviation::
 
@@ -228,213 +231,438 @@
             >>> get_session(2020, 'Austria', 'Qualifying')
 
         Get the 3rd session if the 5th Grand Prix in 2021::
 
             >>> get_session(2021, 5, 3)
 
     Args:
-        year (int): Championship year
-        gp (number or string): Name as str or round number as int. If gp is
+        year: Championship year
+
+        gp: Name as str or round number as int. If gp is
             a string, a fuzzy match will be performed on all events and the
             closest match will be selected.
             Fuzzy matching uses country, location, name and officialName of
             each event as reference.
 
             Some examples that will be correctly interpreted: 'bahrain',
             'australia', 'abudabi', 'monza'.
 
             See :func:`get_event_by_name` for some further remarks on the
             fuzzy matching.
 
-        identifier (str or int): see :ref:`SessionIdentifier`
+        identifier: see :ref:`SessionIdentifier`
 
-        force_ergast (bool): Always use data from the ergast database to
-            create the event schedule
+        backend: select a specific backend as data source, options:
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
 
-        event: deprecated; use identifier instead
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+              for which no timing data is available are not listed
+              (supports 2018 to now)
 
-    Returns:
-        :class:`~fastf1.core.Session`:
-    """
-    if identifier and event:
-        raise ValueError("The arguments 'identifier' and 'event' are "
-                         "mutually exclusive!")
-
-    if gp == 'testing':
-        raise DeprecationWarning('Accessing test sessions through '
-                                 '`get_session` has been deprecated!\nUse '
-                                 '`get_testing_session` instead.')
-
-    if event is not None:
-        warnings.warn("The keyword argument 'event' has been deprecated and "
-                      "will be removed in a future version.\n"
-                      "Use 'identifier' instead.", FutureWarning)
-        identifier = event
-
-    event = get_event(year, gp, force_ergast=force_ergast)
-
-    if identifier is None:
-        warnings.warn("Getting `Event` objects (previously `Session`) through "
-                      "`get_session` has been deprecated.\n"
-                      "Use `fastf1.get_event` instead.", FutureWarning)
-        return event  # TODO: remove in v2.3
+            - ``'ergast'``: uses data from Ergast, no local times are
+              available, no information about availability of f1 timing data is
+              available (supports 1950 to now)
 
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            the other backends are used as a fallback in case the default
+            is not available.
+
+            For seasons older than 2018 ``'ergast'`` is always used.
+
+        force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
+            from the ergast database to create the event schedule
+    """
+    event = get_event(year, gp, force_ergast=force_ergast, backend=backend)
     return event.get_session(identifier)
 
 
-def get_testing_session(year, test_number, session_number):
+def get_testing_session(
+        year: int,
+        test_number: int,
+        session_number: int,
+        *,
+        backend: Optional[Literal['fastf1', 'f1timing']] = None
+) -> Session:
     """Create a :class:`~fastf1.core.Session` object for testing sessions
     based on year, test  event number and session number.
 
     Args:
-        year (int): Championship year
-        test_number (int): Number of the testing event (usually at most two)
-        session_number (int): Number of the session withing a specific testing
+        year: Championship year
+
+        test_number: Number of the testing event (usually at most two)
+
+        session_number: Number of the session within a specific testing
             event. Each testing event usually has three sessions.
 
-    Returns:
-        :class:`~fastf1.core.Session`
+        backend: select a specific backend as data source, options:
+
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
+
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+                for which no timing data is available are not listed
+                (supports 2018 to now)
+
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            ``f1timing`` is used as a fallback in case the default
+            is not available.
 
     .. versionadded:: 2.2
     """
-    event = get_testing_event(year, test_number)
+    event = get_testing_event(year, test_number, backend=backend)
     return event.get_session(session_number)
 
 
-def get_event(year, gp, *, force_ergast=False):
+def get_event(
+        year: int,
+        gp: Union[int, str],
+        *,
+        backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
+        force_ergast: bool = False,
+        strict_search: bool = False
+) -> "Event":
     """Create an :class:`~fastf1.events.Event` object for a specific
     season and gp.
 
     To get a testing event, use :func:`get_testing_event`.
 
     Args:
-        year (int): Championship year
-        gp (int or str): Name as str or round number as int. If gp is
+        year: Championship year
+
+        gp: Name as str or round number as int. If gp is
             a string, a fuzzy match will be performed on all events and the
             closest match will be selected.
             Fuzzy matching uses country, location, name and officialName of
             each event as reference.
             Note that the round number cannot be used to get a testing event,
             as all testing event are round 0!
-        force_ergast (bool): Always use data from the ergast database to
-            create the event schedule
 
-    Returns:
-        :class:`~fastf1.events.Event`
+        backend: select a specific backend as data source, options:
+
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
+
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+              for which no timing data is available are not listed
+              (supports 2018 to now)
+
+            - ``'ergast'``: uses data from Ergast, no local times are
+              available, no information about availability of f1 timing data is
+              available (supports 1950 to now)
+
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            the other backends are used as a fallback in case the default
+            is not available.
+
+            For seasons older than 2018 ``'ergast'`` is always used.
+
+        force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
+            from the ergast database to create the event schedule
+
+        strict_search: Match precisely the query, or default to
+            fuzzy search. If no event is found with
+            ``strict_search=True``, the function will return None
 
     .. versionadded:: 2.2
     """
     schedule = get_event_schedule(year=year, include_testing=False,
-                                  force_ergast=force_ergast)
+                                  force_ergast=force_ergast,
+                                  backend=backend)
 
     if type(gp) is str:
-        event = schedule.get_event_by_name(gp)
+        event = schedule.get_event_by_name(gp, strict_search=strict_search)
     else:
         event = schedule.get_event_by_round(gp)
 
     return event
 
 
-def get_testing_event(year, test_number):
+def get_testing_event(
+        year: int,
+        test_number: int,
+        *,
+        backend: Optional[Literal['fastf1', 'f1timing']] = None
+) -> "Event":
     """Create a :class:`fastf1.events.Event` object for testing sessions
     based on year and test event number.
 
     Args:
-        year (int): Championship year
-        test_number (int): Number of the testing event (usually at most two)
-
-    Returns:
-        :class:`~fastf1.events.Event`
+        year: Championship year
+        test_number: Number of the testing event (usually at most two)
+        backend: select a specific backend as data source, options:
+
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
+
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+              for which no timing data is available are not listed
+              (supports 2018 to now)
+
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            ``f1timing`` is used as a fallback in case the default
+            is not available.
 
     .. versionadded:: 2.2
     """
-    schedule = get_event_schedule(year=year)
+    if backend == 'ergast':
+        raise ValueError("The 'ergast' backend does not support "
+                         "testing events!")
+    schedule = get_event_schedule(year=year, backend=backend)
     schedule = schedule[schedule.is_testing()]
 
     try:
         assert test_number >= 1
-        return schedule.iloc[test_number-1]
+        return schedule.iloc[test_number - 1]
     except (IndexError, AssertionError):
         raise ValueError(f"Test event number {test_number} does not exist")
 
 
-def get_event_schedule(year, *, include_testing=True, force_ergast=False):
+def get_event_schedule(
+        year: int,
+        *,
+        include_testing: bool = True,
+        backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
+        force_ergast: bool = False
+) -> "EventSchedule":
     """Create an :class:`~fastf1.events.EventSchedule` object for a specific
     season.
 
     Args:
-        year (int): Championship year
-        include_testing (bool): Include or exclude testing sessions from the
+        year: Championship year
+
+        include_testing: Include or exclude testing sessions from the
             event schedule.
-        force_ergast (bool): Always use data from the ergast database to
-            create the event schedule
 
-    Returns:
-        :class:`~fastf1.events.EventSchedule`
+        backend: select a specific backend as data source, options:
+
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
+
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+              for which no timing data is available are not listed
+              (supports 2018 to now)
+
+            - ``'ergast'``: uses data from Ergast, no local times are
+              available, no information about availability of f1 timing data is
+              available (supports 1950 to now)
+
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            the other backends are used as a fallback in case the default
+            is not available.
+
+            For seasons older than 2018 ``'ergast'`` is always used.
+
+        force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
+            from the ergast database to create the event schedule
 
     .. versionadded:: 2.2
+
     """
-    if ((year not in range(2018, datetime.datetime.now().year+1))
-            or force_ergast):
-        schedule = _get_schedule_from_ergast(year)
+    if force_ergast:
+        warnings.warn("Option ``force_ergast`` has been deprecated, use"
+                      "``backend='ergast'`` instead")
+        backend = 'ergast'
+
+    _backends_named_order = {
+        'fastf1': _get_schedule_ff1,
+        'f1timing': _get_schedule_from_f1_timing,
+        'ergast': _get_schedule_from_ergast
+    }
+
+    if backend is not None:
+        _backends = [_backends_named_order[backend]]
+    elif year < 2018:
+        _backends = [_backends_named_order['ergast']]
     else:
-        try:
-            schedule = _get_schedule(year)
-        except Exception as exc:
-            logging.error(f"Failed to access primary schedule backend. "
-                          f"Falling back to Ergast! Reason: {exc})")
-            schedule = _get_schedule_from_ergast(year)
+        _backends = list(_backends_named_order.values())
+
+    schedule = None
+    for func in _backends:
+        schedule = func(year)
+        if schedule is not None:
+            break
+
+    if schedule is None:  # raise Error if fallback failed as well
+        raise ValueError("Failed to load any schedule data.")
 
     if not include_testing:
         schedule = schedule[~schedule.is_testing()]
     return schedule
 
 
 def get_events_remaining(
-        dt=None, *, include_testing=True, force_ergast=False) \
-        -> 'EventSchedule':
+        dt: Optional[datetime.datetime] = None,
+        *,
+        include_testing: bool = True,
+        backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
+        force_ergast: bool = False
+) -> 'EventSchedule':
     """Create an :class:`~fastf1.events.EventSchedule` object for remaining season.
 
     Args:
-        dt (datetime): Optional DateTime to get events after.
-        include_testing (bool): Include or exclude testing sessions from the
+        dt: Optional DateTime to get events after.
+
+        include_testing: Include or exclude testing sessions from the
             event schedule.
-        force_ergast (bool): Always use data from the ergast database to
-            create the event schedule
 
-    Returns:
-        :class:`~fastf1.events.EventSchedule`
+        backend: select a specific backend as data source, options:
+
+            - ``'fastf1'``: FastF1's own backend, full support for 2018 to now
+
+            - ``'f1timing'``: uses data from the F1 live timing API, sessions
+              for which no timing data is available are not listed
+              (supports 2018 to now)
+
+            - ``'ergast'``: uses data from Ergast, no local times are
+              available, no information about availability of f1 timing data is
+              available (supports 1950 to now)
+
+            When no backend is specified, ``'fastf1'`` is used as a default and
+            the other backends are used as a fallback in case the default
+            is not available.
+
+            For seasons older than 2018 ``'ergast'`` is always used.
+
+        force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
+            from the ergast database to create the event schedule
 
     .. versionadded:: 2.3
     """
     if dt is None:
         dt = datetime.datetime.now()
 
     events = get_event_schedule(
-        dt.year, include_testing=include_testing, force_ergast=force_ergast)
+        dt.year, include_testing=include_testing,
+        force_ergast=force_ergast, backend=backend
+    )
     result = events.loc[events["EventDate"] >= dt]
     return result
 
 
-def _get_schedule(year):
+@soft_exceptions("FastF1 schedule",
+                 "Failed to load schedule from FastF1 backend!",
+                 _logger)
+def _get_schedule_ff1(year):
     response = Cache.requests_get(
         _SCHEDULE_BASE_URL + f"schedule_{year}.json"
     )
-    df = pd.read_json(response.text)
 
+    data = dict()
+    json_data = json.loads(response.text)
+    for key in json_data.keys():
+        data[key] = list(json_data[key].values())
+
+    # convert gmt offset to timedelta
+    gmt_offset = list()
+    for go in data.pop('gmt_offset'):
+        if go is None:
+            gmt_offset.append(datetime.timedelta(0))
+        else:
+            # hh:mm -> hh:mm:00 before to_timedelta
+            gmt_offset.append(to_timedelta(f"{go}:00"))
+
+    length = len(gmt_offset)
+
+    # create additional columns for UTC timestamps
+    for n in range(5):
+        data[f'session{n+1}_date_Utc'] = [None, ] * length
+
+    # convert and set all timestamps
+    for i in range(length):
+        data['event_date'][i] = to_datetime(data['event_date'][i]) \
+            .replace(hour=0, minute=0, second=0)
+
+        for j in range(5):
+            date = to_datetime(data[f'session{j+1}_date'][i])
+            if date is None:
+                date_utc = None
+            else:
+                # create tz-aware local time
+                date = date.replace(tzinfo=datetime.timezone(gmt_offset[i]))
+
+                # create non-tz-aware utc time
+                date_utc = date.astimezone(datetime.timezone.utc) \
+                    .replace(tzinfo=None)
+
+            data[f'session{j+1}_date'][i] = pd.Timestamp(date)
+            data[f'session{j+1}_date_Utc'][i] = pd.Timestamp(date_utc)
+
+    str().capitalize()
+
+    df = pd.DataFrame(data)
     # change column names from snake_case to UpperCamelCase
     col_renames = {col: ''.join([s.capitalize() for s in col.split('_')])
                    for col in df.columns}
     df = df.rename(columns=col_renames)
 
     schedule = EventSchedule(df, year=year, force_default_cols=True)
     return schedule
 
 
-def _get_schedule_from_ergast(year):
+@soft_exceptions("F1 API schedule",
+                 "Failed to load schedule from F1 API backend!",
+                 _logger)
+def _get_schedule_from_f1_timing(year):
+    # create an event schedule using data from the F1 API
+    response = fastf1._api.season_schedule(f'/static/{year}/')
+    data = collections.defaultdict(list)
+
+    for event in response:
+        data['Country'].append(event['Country']['Name'])
+        data['Location'].append(event['Location'])
+        data['EventName'].append(event['Name'])
+        data['OfficialEventName'].append(event['OfficialName'])
+
+        n_events = min(len(event['Sessions']), 5)
+        # number of events, usually 3 for testing, 5 for race weekends
+        # in special cases there are additional unrelated events
+
+        if (n_events >= 4) and ('Sprint' in event['Sessions'][3]['Name']):
+            if event['Sessions'][3]['Name'] == 'Sprint Qualifying':
+                # fix for 2021 where Sprint was called Sprint Qualifying
+                event['Sessions'][3]['Name'] = 'Sprint'
+            data['EventFormat'].append('sprint')
+            data['RoundNumber'].append(event['Number'])
+        elif 'test' in event['Name'].lower():
+            data['EventFormat'].append('testing')
+            data['RoundNumber'].append(0)
+        else:
+            data['EventFormat'].append('conventional')
+            data['RoundNumber'].append(event['Number'])
+
+        data['F1ApiSupport'].append(True)
+
+        for i in range(0, 5):
+            # parse the up to five sessions for each event
+            try:
+                session = event['Sessions'][i]
+            except IndexError:
+                data[f'Session{i+1}'].append(None)
+                data[f'Session{i+1}Date'].append(None)
+                data[f'Session{i+1}DateUtc'].append(None)
+            else:
+                data[f'Session{i+1}'].append(session['Name'])
+                # save timestamp as tz-aware local time and non-tz-aware utc
+                date = to_datetime(session['StartDate'])
+                gmt_offset = to_timedelta(session['GmtOffset'])
+                date = date.replace(tzinfo=datetime.timezone(gmt_offset))
+                date_utc = date.astimezone(datetime.timezone.utc) \
+                    .replace(tzinfo=None)
+                data[f'Session{i+1}Date'].append(pd.Timestamp(date))
+                data[f'Session{i+1}DateUtc'].append(pd.Timestamp(date_utc))
+
+        # set the event date to the date of the last session
+        ev_date = data[f'Session{n_events}DateUtc'][-1]
+        ev_date = ev_date.replace(hour=0, minute=0, second=0)
+        data['EventDate'].append(ev_date)
+
+    schedule = EventSchedule(data, year=year, force_default_cols=True)
+    return schedule
+
+
+@soft_exceptions("Ergast API Schedule",
+                 "Failed to load schedule from Ergast API backend!",
+                 _logger)
+def _get_schedule_from_ergast(year) -> "EventSchedule":
     # create an event schedule using data from the ergast database
     season = fastf1.ergast.fetch_season(year)
     data = collections.defaultdict(list)
     for rnd in season:
         data['RoundNumber'].append(int(rnd.get('round')))
         data['Country'].append(
             recursive_dict_get(rnd, 'Circuit', 'Location', 'country')
@@ -450,38 +678,45 @@
                 f"{rnd.get('date', '')}T{rnd.get('time', '')}",
             ).tz_localize(None)
         except dateutil.parser.ParserError:
             date = pd.NaT
         data['EventDate'].append(date)
 
         if 'Sprint' in rnd:
-            sprint_name = 'Sprint Qualifying' if year == 2021 else 'Sprint'
             data['EventFormat'].append("sprint")
             data['Session1'].append('Practice 1')
-            data['Session1Date'].append(date.floor('D') - pd.Timedelta(days=2))
+            data['Session1DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=2))
             data['Session2'].append('Qualifying')
-            data['Session2Date'].append(date.floor('D') - pd.Timedelta(days=2))
+            data['Session2DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=2))
             data['Session3'].append('Practice 2')
-            data['Session3Date'].append(date.floor('D') - pd.Timedelta(days=1))
-            data['Session4'].append(sprint_name)
-            data['Session4Date'].append(date.floor('D') - pd.Timedelta(days=1))
+            data['Session3DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=1))
+            data['Session4'].append('Sprint')
+            data['Session4DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=1))
             data['Session5'].append('Race')
-            data['Session5Date'].append(date)
+            data['Session5DateUtc'].append(date)
         else:
             data['EventFormat'].append("conventional")
             data['Session1'].append('Practice 1')
-            data['Session1Date'].append(date.floor('D') - pd.Timedelta(days=2))
+            data['Session1DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=2))
             data['Session2'].append('Practice 2')
-            data['Session2Date'].append(date.floor('D') - pd.Timedelta(days=2))
+            data['Session2DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=2))
             data['Session3'].append('Practice 3')
-            data['Session3Date'].append(date.floor('D') - pd.Timedelta(days=1))
+            data['Session3DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=1))
             data['Session4'].append('Qualifying')
-            data['Session4Date'].append(date.floor('D') - pd.Timedelta(days=1))
+            data['Session4DateUtc'].append(
+                date.floor('D') - pd.Timedelta(days=1))
             data['Session5'].append('Race')
-            data['Session5Date'].append(date)
+            data['Session5DateUtc'].append(date)
 
         data['F1ApiSupport'].append(True if year >= 2018 else False)
         # simplified; this is only true most of the time
 
     df = pd.DataFrame(data)
     schedule = EventSchedule(df, year=year, force_default_cols=True)
     return schedule
@@ -510,43 +745,52 @@
         'Country': str,
         'Location': str,
         'OfficialEventName': str,
         'EventDate': 'datetime64[ns]',
         'EventName': str,
         'EventFormat': str,
         'Session1': str,
-        'Session1Date': 'datetime64[ns]',
+        'Session1Date': object,  # tz-aware datetime.datetime
+        'Session1DateUtc': 'datetime64[ns]',
         'Session2': str,
-        'Session2Date': 'datetime64[ns]',
+        'Session2Date': object,
+        'Session2DateUtc': 'datetime64[ns]',
         'Session3': str,
-        'Session3Date': 'datetime64[ns]',
+        'Session3Date': object,
+        'Session3DateUtc': 'datetime64[ns]',
         'Session4': str,
-        'Session4Date': 'datetime64[ns]',
+        'Session4Date': object,
+        'Session4DateUtc': 'datetime64[ns]',
         'Session5': str,
-        'Session5Date': 'datetime64[ns]',
+        'Session5Date': object,
+        'Session5DateUtc': 'datetime64[ns]',
         'F1ApiSupport': bool
     }
 
     _metadata = ['year']
 
-    _internal_names = ['base_class_view']
+    _internal_names = pd.DataFrame._internal_names + ['base_class_view']
+    _internal_names_set = set(_internal_names)
 
-    def __init__(self, *args, year=0, force_default_cols=False, **kwargs):
+    def __init__(self, *args, year: int = 0,
+                 force_default_cols: bool = False, **kwargs):
         if force_default_cols:
             kwargs['columns'] = list(self._COL_TYPES)
         super().__init__(*args, **kwargs)
         self.year = year
 
         # apply column specific dtypes
         for col, _type in self._COL_TYPES.items():
             if col not in self.columns:
                 continue
             if self[col].isna().all():
                 if _type == 'datetime64[ns]':
                     self[col] = pd.NaT
+                elif _type == object:
+                    self[col] = None
                 else:
                     self[col] = _type()
             self[col] = self[col].astype(_type)
 
     def __repr__(self):
         return self.base_class_view.__repr__()
 
@@ -571,53 +815,44 @@
         return pd.DataFrame(self)
 
     def is_testing(self):
         """Return `True` or `False`, depending on whether each event is a
         testing event."""
         return pd.Series(self['EventFormat'] == 'testing')
 
-    def get_event_by_round(self, round):
+    def get_event_by_round(self, round: int) -> "Event":
         """Get an :class:`Event` by its round number.
 
         Args:
-            round (int): The round number
-        Returns:
-            :class:`Event`
+            round: The round number
         Raises:
             ValueError: The round does not exist in the event schedule
         """
         if round == 0:
             raise ValueError("Cannot get testing event by round number!")
         mask = self['RoundNumber'] == round
         if not mask.any():
             raise ValueError(f"Invalid round: {round}")
         return self[mask].iloc[0]
 
-    def get_event_by_name(self, name):
-        """Get an :class:`Event` by its name.
+    def _strict_event_search(self, name: str):
+        """
+        Match Event Name exactly, ignoring case.
+        """
 
-        A fuzzy match is performed to find the event that best matches the
-        given name. Fuzzy matching is performed using the country, location,
-        name and officialName of each event. This is not guaranteed to return
-        the correct result. You should therefore always check if the function
-        actually returns the event you had wanted.
+        query = name.lower()
+        for i, event in self.iterrows():
+            if 'EventName' in event:
+                if event['EventName'].lower() == query:
+                    return self.loc[i]
+        else:
+            return None
 
-        .. warning:: You should avoid adding common words to ``name`` to avoid
-            false string matches.
-            For example, you should rather use "Belgium" instead of "Belgian
-            Grand Prix" as ``name``.
+    def _fuzzy_event_search(self, name: str) -> "Event":
 
-        Args:
-            name (str): The name of the event. For example,
-                ``.get_event_by_name("british")`` and
-                ``.get_event_by_name("silverstone")`` will both return the
-                event for the British Grand Prix.
-        Returns:
-            :class:`Event`
-        """
         def _matcher_strings(ev):
             strings = list()
             if 'Location' in ev:
                 strings.append(ev['Location'])
             if 'Country' in ev:
                 strings.append(ev['Country'])
             if 'EventName' in ev:
@@ -637,14 +872,54 @@
                  for val in _matcher_strings(event)]
             )
             if ratio > max_ratio:
                 max_ratio = ratio
                 index = i
         return self.loc[index]
 
+    def get_event_by_name(
+            self,
+            name: str,
+            *,
+            strict_search: bool = False
+    ) -> "Event":
+        """Get an :class:`Event` by its name.
+
+        A fuzzy match is performed to find the event that best matches the
+        given name. Fuzzy matching is performed using the country, location,
+        name and officialName of each event. This is not guaranteed to return
+        the correct result. You should therefore always check if the function
+        actually returns the event you had wanted.
+        To gurantee the function returns the event queried, toggle
+        strict_search, which will only return an event if its event name
+        matches (non case sensitive) the query string.
+
+        .. warning:: You should avoid adding common words to ``name`` to avoid
+            false string matches.
+            For example, you should rather use "Belgium" instead of "Belgian
+            Grand Prix" as ``name``.
+
+        Args:
+            name: The name of the event. For example,
+                ``.get_event_by_name("british")`` and
+                ``.get_event_by_name("silverstone")`` will both return the
+                event for the British Grand Prix.
+            strict_search: Search only for exact query matches
+                instead of using fuzzy search. For example,
+                ``.get_event_by_name("British Grand Prix", strict_search=True)`` # noqa: E501
+                will return the event for the British Grand Prix, whereas
+                ``.get_event_by_name("British", strict_search=True)``
+                will return ``None``
+        """
+
+        if strict_search:
+            return self._strict_event_search(name)
+        else:
+            return self._fuzzy_event_search(name)
+
 
 class Event(pd.Series):
     """This class represents a single event (race weekend or testing event).
 
     Each event consists of one or multiple sessions, depending on the type
     of event and depending on the event format.
 
@@ -652,105 +927,46 @@
     :func:`get_event` or similar to get a specific event.
 
     Args:
           year (int): Championship year
     """
     _metadata = ['year']
 
-    _internal_names = ['date', 'gp']
-
-    def __init__(self, *args, year=None, **kwargs):
+    def __init__(self, *args, year: int = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.year = year
-        self._getattr_override = True  # TODO: remove in v2.3
 
     @property
     def _constructor(self):
         def _new(*args, **kwargs):
             return Event(*args, **kwargs).__finalize__(self)
 
         return _new
 
-    def __getattribute__(self, name):
-        # TODO: remove in v2.3
-        if name == 'name' and getattr(self, '_getattr_override', False):
-            if 'EventName' in self:
-                warnings.warn(
-                    "The `Weekend.name` property is deprecated and will be"
-                    "removed in a future version.\n"
-                    "Use `Event['EventName']` or `Event.EventName` instead.",
-                    FutureWarning
-                )
-                # name may be accessed by pandas internals to, when data
-                # does not exist yet
-                return self['EventName']
-
-        return super().__getattribute__(name)
-
-    def __repr__(self):
-        # don't show .name deprecation message when .name is accessed internally
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore',
-                                    message=r".*property is deprecated.*")
-            return super().__repr__()
-
-    @property
-    def date(self):
-        """Event race date (YYYY-MM-DD)
-
-        This wraps ``self['EventDate'].strftime('%Y-%m-%d')``
-
-        .. deprecated:: 2.2
-            use :attr:`Event.EventDate` or :attr:`Event['EventDate']` and
-            use :func:`datetime.datetime.strftime` to format the desired
-            string representation of the datetime object
-        """
-        warnings.warn("The `Weekend.date` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Event['EventDate']` or `Event.EventDate` instead.",
-                      FutureWarning)
-        return self['EventDate'].strftime('%Y-%m-%d')
-
-    @property
-    def gp(self):
-        """Event round number
-
-        .. deprecated:: 2.2
-            use :attr:`Event.eventNumber` or :attr:`Event['eventNumber']`
-        """
-        warnings.warn("The `Weekend.gp` property is deprecated and will be"
-                      "removed in a future version.\n"
-                      "Use `Event['RoundNumber']` or `Event.RoundNumber` "
-                      "instead.", FutureWarning)
-        return self['RoundNumber']
-
-    def is_testing(self):
+    def is_testing(self) -> bool:
         """Return `True` or `False`, depending on whether this event is a
         testing event."""
         return self['EventFormat'] == 'testing'
 
-    def get_session_name(self, identifier):
+    def get_session_name(self, identifier) -> str:
         """Return the full session name of a specific session from this event.
 
         Examples:
 
             >>> import fastf1
             >>> event = fastf1.get_event(2021, 1)
             >>> event.get_session_name(3)
             'Practice 3'
             >>> event.get_session_name('Q')
             'Qualifying'
             >>> event.get_session_name('praCtice 1')
             'Practice 1'
 
         Args:
-            identifier (str or int): see :ref:`SessionIdentifier`
-
-        Returns:
-            :class:`str`
+            identifier: see :ref:`SessionIdentifier`
 
         Raises:
             ValueError: No matching session or invalid identifier
         """
         try:
             num = float(identifier)
         except ValueError:
@@ -782,50 +998,48 @@
                 raise ValueError(f"Invalid session type '{num}'")
             if not session_name:
                 raise ValueError(f"Session number {num} does not "
                                  f"exist for this event")
 
         return session_name
 
-    def get_session_date(self, identifier):
+    def get_session_date(self, identifier: Union[str, int], utc=False) \
+            -> pd.Timestamp:
         """Return the date and time (if available) at which a specific session
         of this event is or was held.
 
         Args:
-            identifier (str or int): see :ref:`SessionIdentifier`
-
-        Returns:
-            :class:`datetime.datetime`
+            identifier: see :ref:`SessionIdentifier`
+            utc: return a non-timezone-aware UTC timestamp
 
         Raises:
             ValueError: No matching session or invalid identifier
         """
         session_name = self.get_session_name(identifier)
         relevant_columns = self.loc[['Session1', 'Session2', 'Session3',
                                      'Session4', 'Session5']]
         mask = (relevant_columns == session_name)
         if not mask.any():
             raise ValueError(f"Session type '{identifier}' does not exist "
                              f"for this event")
         else:
             _name = mask.idxmax()
+            date_utc = self[f"{_name}DateUtc"]
             date = self[f"{_name}Date"]
-            if pd.isnull(date):
-                raise ValueError(f"Session type '{identifier}' does not "
-                                 f"exist for this event")
+            if (not utc) and pd.isnull(date) and (not pd.isnull(date_utc)):
+                raise ValueError("Local timestamp is not available")
+            if utc:
+                return date_utc
             return date
 
-    def get_session(self, identifier):
+    def get_session(self, identifier: Union[int, str]) -> "Session":
         """Return a session from this event.
 
         Args:
-            identifier (str or int): see :ref:`SessionIdentifier`
-
-        Returns:
-            :class:`Session` instance
+            identifier: see :ref:`SessionIdentifier`
 
         Raises:
             ValueError: No matching session or invalid identifier
         """
         try:
             num = float(identifier)
         except ValueError:
@@ -844,43 +1058,29 @@
             if not session_name:
                 raise ValueError(f"Session number {num} does not "
                                  f"exist for this event")
 
         return Session(event=self, session_name=session_name,
                        f1_api_support=self.F1ApiSupport)
 
-    def get_race(self):
-        """Return the race session.
-
-        Returns:
-            :class:`Session` instance
-        """
+    def get_race(self) -> "Session":
+        """Return the race session."""
         return self.get_session('Race')
 
-    def get_qualifying(self):
-        """Return the qualifying session.
-
-        Returns:
-            :class:`Session` instance
-        """
+    def get_qualifying(self) -> "Session":
+        """Return the qualifying session."""
         return self.get_session('Qualifying')
 
-    def get_sprint(self):
-        """Return the sprint session.
-
-        Returns:
-            :class:`Session` instance
-        """
+    def get_sprint(self) -> "Session":
+        """Return the sprint session."""
         return self.get_session('Sprint')
 
     def get_sprint_shootout(self) -> "Session":
         """Return the sprint shootout session."""
         return self.get_session('Sprint Shootout')
 
     def get_practice(self, number: int) -> "Session":
         """Return the specified practice session.
         Args:
             number: 1, 2 or 3 - Free practice session number
-        Returns:
-            :class:`Session` instance
         """
         return self.get_session(f'Practice {number}')
```

### Comparing `fastf1-2.3.3/fastf1/legacy.py` & `fastf1-3.0.0/fastf1/legacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """
-Legacy Functionality - :mod:`fastf1.legacy`
-===========================================
-
 This module contains the legacy implementation for calculating distance to driver ahead.
 
 :func:`inject_driver_ahead` adds 'DriverAhead' and 'DistanceToDriverAhead' to the position data for all laps of all
 drivers. This functionality has been replaced with :func:`fastf1.core.Telemetry.add_driver_ahead`.
 The new implementation provides smoother and more accurate results. Additionally, it can be applied to arbitrary slices
 of data. But it suffers from integration error when used over multiple laps. The legacy implementation has no
 integration error issues.
@@ -22,15 +19,14 @@
     import fastf1
     import fastf1.plotting
     import fastf1.legacy
     import numpy as np
     import matplotlib.pyplot as plt
 
     fastf1.plotting.setup_mpl()
-    # fastf1.Cache.enable_cache("path/to/cache")
 
     session = fastf1.get_session(2020, 'Italy', 'R')
     session.load()
 
     DRIVER = 'VER'  # which driver; need to specify number and abbreviation
     DRIVER_NUMBER = '33'
     LAP_N = 10  # which lap number to plot
@@ -53,16 +49,19 @@
     plt.legend()
     plt.show()
 """
 
 import numpy as np
 import pandas as pd
 import scipy.spatial
-import logging
 
+from fastf1.logger import get_logger
+
+
+_logger = get_logger(__name__)
 
 REFERENCE_LAP_RESOLUTION = 0.667
 """A distance in meters which indicates the resolution of the reference
 lap. This reference is used to project car positions and calculate
 things like distance between cars.
 """
 
@@ -165,15 +164,16 @@
         stream_length = len(session.pos_data[drivers_list[0]])
         dmap = np.empty((stream_length, len(drivers_list)), dtype=int)
 
         fast_query = {'workers': 2, 'distance_upper_bound': 500}
         # fast_query < Increases speed
         for index, drv in enumerate(drivers_list):
             if drv not in session.pos_data.keys():
-                logging.warning(f"Driver {drv: >2}: No position data. (_make_trajectory)")
+                _logger.warning(f"Driver {drv: >2}: No position data. "
+                                f"(_make_trajectory)")
                 continue
             trajectory = session.pos_data[drv][['X', 'Y', 'Z']].values
             projection_index = track_tree.query(trajectory, **fast_query)[1]
             # When tree cannot solve super far points means there is some
             # pit shit shutdown. We can replace these index with 0
             projection_index[projection_index == len(reference_s)] = 0
             dmap[:, index] = fix_suzuka(projection_index.copy(), reference_s)
```

### Comparing `fastf1-2.3.3/fastf1/livetiming/__init__.py` & `fastf1-3.0.0/fastf1/livetiming/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,16 @@
 2. Load this data into FastF1 after the session has finished
 
 .. code-block::
 
     import fastf1
     from fastf1.livetiming.data import LiveTimingData
 
-    fastf1.Cache.enable_cache('cache_directory')
-
     livedata = LiveTimingData('saved_data.txt')
-    session = fastf1.get_session(2021, 'testing', 1)
+    session = fastf1.get_testing_session(2021, 1, 1)
     session.load(livedata=livedata)
 
 optionally you can load live timing data from two or more files
 
 .. code-block::
 
     livedata = LiveTimingData('saved_data_1.txt', 'saved_data_2.txt')
@@ -59,26 +57,30 @@
 
 - You should not mix recorded live timing data and data requested from the api
   after a session. The data will likely not be synchronized correctly.
 
 - You should use the cache with saved live timing data too. This will speed up
   loading of the data considerably after the first run.
 
-- You need to used different cache directories if you want to cache
+- You need to use different cache directories if you want to cache
   saved live timing data and api data **for the same session**!
   The cache cannot tell the data sources apart. If cached data from one source
   already exists it will not be reloaded automatically from a different source.
+  See :class:`fastf1.req.Cache` for details on how to configure a custom
+  cache directory. One simple way is to add the following line to your code::
+
+    fastf1.Cache.enable_cache('path/to/cache/directory')
 
 - You need to force a cache update if you modify the :class:`LiveTimingData`
   (e.g. by adding a second file). The cache cannot tell that the input source
   was modified and will still use the old cached data.
 
   You can force-refresh the cache::
 
-    fastf1.Cache.enable_cache('cache_directory', force_renew=True)
+    fastf1.Cache.enable_cache('path/to/cache/directory', force_renew=True)
 
   You only need to use ``forece_renew=True`` once after modifying the
   input data.
 
 - The SignalR Client seems to get disconnected after 2 hours of recording. It looks
   like the connection is terminated by the server. You need to manually start a
   second recording before the first one disconnects if you want to have no gap in
```

### Comparing `fastf1-2.3.3/fastf1/livetiming/__main__.py` & `fastf1-3.0.0/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.3/fastf1/livetiming/client.py` & `fastf1-3.0.0/fastf1/livetiming/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 import concurrent.futures
 import json
 import logging
 import requests
-import sys
 import time
 
-from signalr_aio import Connection
+from fastf1.signalr_aio import Connection
 
 import fastf1
 
 
 def messages_from_raw(r):
     """Extract data messages from raw recorded SignalR data.
 
@@ -71,20 +70,14 @@
             console. If you wish to customize logging, you can pass an
             instance of :class:`logging.Logger` (see: :mod:`logging`).
     """
     _connection_url = 'https://livetiming.formula1.com/signalr'
 
     def __init__(self, filename, filemode='w', debug=False,
                  timeout=60, logger=None):
-        if (ver := sys.version_info) >= (3, 10):
-            raise RuntimeError(
-                f"The live timing client does only support Python 3.8 and "
-                f"3.9 but you are using version "
-                f"{'.'.join(str(d) for d in ver[:3])}"
-            )
 
         self.headers = {'User-agent': 'BestHTTP',
                         'Accept-Encoding': 'gzip, identity',
                         'Connection': 'keep-alive, Upgrade'}
 
         self.topics = ["Heartbeat", "CarData.z", "Position.z",
                        "ExtrapolatedClock", "TopThree", "RcmSeries",
```

### Comparing `fastf1-2.3.3/fastf1/livetiming/data.py` & `fastf1-3.0.0/fastf1/livetiming/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Data object for livetiming data
 """
 
 from datetime import timedelta
 import json
 import hashlib
-import logging
 
+from fastf1.logger import get_logger
 from fastf1.utils import to_datetime, recursive_dict_get
 
 
+_logger = get_logger(__name__)
+
+
 _track_status_mapping = {
     'AllClear': '1',
     'Yellow': '2',
     'SCDeployed': '4',
     'Red': '5',
     'VSCDeployed': '6',
     'VSCEnding': '7'
@@ -70,15 +73,15 @@
         """
         Read all files, parse the data and store it by category.
 
         Should usually not be called manually. This is called
         automatically the first time :meth:`get`, :meth:`has`
         or :meth:`list_categories` are called.
         """
-        logging.info("Reading live timing data from recording. "
+        _logger.info("Reading live timing data from recording. "
                      "This may take a bit.")
         for fname in self.files:
             self._load_single_file(fname)
         self._files_read = True
 
     def _load_single_file(self, fname):
         # read one file, parse its content and add it to the already loaded
@@ -106,23 +109,22 @@
             if lhash in self._line_hashes:
                 return
             self._line_hashes.append(lhash)
 
         # load the three parts of each data element
         elem = self._fix_json(elem)
         try:
-            cat, msg, dt = json.loads(elem)
+            cat, msg, dt_str = json.loads(elem)
         except (json.JSONDecodeError, ValueError):
             self.errorcount += 1
             return
 
         # convert string to datetime
-        try:
-            dt = to_datetime(dt)
-        except (ValueError, TypeError):
+        dt = to_datetime(dt_str)
+        if dt is None:
             self.errorcount += 1
             return
 
         # if no start date could be determined beforehand, simply use the
         # first timestamp as we need to have some date as start date;
         # convert timestamp to timedelta (SessionTime) base on start date
         if self._start_date is None:
@@ -204,48 +206,48 @@
         # skim content to find 'Started' session status without actually
         # decoding each line to save time
         for elem in data:
             if 'SessionStatus' in elem and 'Started' in elem:
                 break
         else:
             # didn't find 'Started'
-            logging.error("Error while trying to set correct "
+            _logger.error("Error while trying to set correct "
                           "session start date!")
             return
 
         # decode matching line
         elem = self._fix_json(elem)
         try:
             cat, msg, dt = json.loads(elem)
         except (json.JSONDecodeError, ValueError):
-            logging.error("Error while trying to set correct "
+            _logger.error("Error while trying to set correct "
                           "session start date!")
             return
 
         # find correct entry in series
         try:
             for entry in msg['StatusSeries']:
                 status = recursive_dict_get(entry, 'SessionStatus')
                 if status == 'Started':
                     try:
                         self._start_date = to_datetime(entry['Utc'])
                     except (KeyError, ValueError, TypeError):
                         self.errorcount += 1
-                        logging.error("Error while trying to set correct "
+                        _logger.error("Error while trying to set correct "
                                       "session start date!")
                         return
         except AttributeError:
             for entry in msg['StatusSeries'].values():
                 status = entry.get('SessionStatus', None)
                 if status == 'Started':
                     try:
                         self._start_date = to_datetime(entry['Utc'])
                     except (KeyError, ValueError, TypeError):
                         self.errorcount += 1
-                        logging.error("Error while trying to set correct "
+                        _logger.error("Error while trying to set correct "
                                       "session start date!")
                         return
 
     def get(self, name):
         """
         Return data for category name.
```

### Comparing `fastf1-2.3.3/fastf1/plotting.py` & `fastf1-3.0.0/fastf1/plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """
-Plotting - :mod:`fastf1.plotting`
-=================================
-
 Helper functions for creating data plots.
 
 :mod:`fastf1.plotting` provides optional functionality with the intention of making
 it easy to create nice plots.
 
 This module offers mainly two things:
     - team names and colors
@@ -20,15 +17,15 @@
 If you don't want to use matplotlib, you can still use the team names
 and colors which are provided below.
 
 
 .. note:: Plotting related functionality is likely to change in a future
     release.
 """
-from typing import Dict
+from typing import Dict, List
 
 import pandas as pd
 import numpy as np
 import warnings
 
 try:
     import matplotlib
@@ -41,24 +38,26 @@
     import timple
 except ImportError:
     warnings.warn("Failed to import optional dependency 'timple'!"
                   "Plotting of timedelta values will be restricted!",
                   UserWarning)
 
 import warnings
+
 with warnings.catch_warnings():
     warnings.filterwarnings('ignore', message="Using slow pure-python SequenceMatcher")
     # suppress that warning, it's confusing at best here, we don't need fast sequence matching
     # and the installation (on windows) some effort
     from thefuzz import fuzz
 
 
 class __TeamColorsWarnDict(dict):
     """Implements userwarning on KeyError in :any:`TEAM_COLORS` after
     changing team names."""
+
     def get(self, key, default=None):
         value = super().get(key, default)
         if value is None:
             self.warn_change()
         return value
 
     def __getitem__(self, item):
@@ -81,81 +80,93 @@
 TEAM_COLORS = __TeamColorsWarnDict({
     'mercedes': '#00d2be', 'ferrari': '#dc0000',
     'red bull': '#0600ef', 'mclaren': '#ff8700',
     'alpine': '#0090ff', 'aston martin': '#006f62',
     'alfa romeo': '#900000', 'alphatauri': '#2b4562',
     'haas': '#ffffff', 'williams': '#005aff'
 })
-"""Mapping of team colors (hex color code) to team names.
+"""Mapping of team names to team colors (hex color codes).
 (current season only)"""
 
-
-TEAM_TRANSLATE = {'MER': 'mercedes', 'FER': 'ferrari',
-                  'RBR': 'red bull', 'MCL': 'mclaren',
-                  'APN': 'alpine', 'AMR': 'aston martin',
-                  'ARR': 'alfa romeo', 'APT': 'alphatauri',
-                  'HAA': 'haas', 'WIL': 'williams'}
+TEAM_TRANSLATE: Dict[str, str] = {
+    'MER': 'mercedes', 'FER': 'ferrari',
+    'RBR': 'red bull', 'MCL': 'mclaren',
+    'APN': 'alpine', 'AMR': 'aston martin',
+    'ARR': 'alfa romeo', 'APT': 'alphatauri',
+    'HAA': 'haas', 'WIL': 'williams'}
 """Mapping of team names to theirs respective abbreviations."""
 
-DRIVER_COLORS = {
-        "valtteri bottas": "#900000",
-        "zhou guanyu": "#500000",
+DRIVER_COLORS: Dict[str, str] = {
+    "valtteri bottas": "#900000",
+    "zhou guanyu": "#500000",
 
-        "nyck de vries": "#2b4562",
-        "yuki tsunoda": "#356cac",
+    "nyck de vries": "#2b4562",
+    "yuki tsunoda": "#356cac",
 
-        "pierre gasly": "#0090ff",
-        "esteban ocon": "#70c2ff",
+    "pierre gasly": "#0090ff",
+    "esteban ocon": "#70c2ff",
 
-        "fernando alonso": "#006f62",
-        "lance stroll": "#25a617",
-        "felipe drugovich": "#2f9b90",
+    "fernando alonso": "#006f62",
+    "lance stroll": "#25a617",
+    "felipe drugovich": "#2f9b90",
 
-        "charles leclerc": "#dc0000",
-        "carlos sainz": "#ff8181",
+    "charles leclerc": "#dc0000",
+    "carlos sainz": "#ff8181",
 
-        "kevin magnussen": "#ffffff",
-        "nico hulkenburg": "#cacaca",
+    "kevin magnussen": "#ffffff",
+    "nico hulkenberg": "#cacaca",
 
-        "oscar piastri": "#ff8700",
-        "lando norris": "#eeb370",
+    "oscar piastri": "#ff8700",
+    "lando norris": "#eeb370",
 
-        "lewis hamilton": "#00d2be",
-        "george russell": "#24ffff",
+    "lewis hamilton": "#00d2be",
+    "george russell": "#24ffff",
 
-        "max verstappen": "#0600ef",
-        "sergio perez": "#716de2",
+    "max verstappen": "#0600ef",
+    "sergio perez": "#716de2",
 
-        "alexander albon": "#005aff",
-        "logan sargeant": "#012564",
+    "alexander albon": "#005aff",
+    "logan sargeant": "#012564",
 }
-"""Mapping of driver colors (hex color code) to driver names.
+"""Mapping of driver names to driver colors (hex color codes).
 (current season only)"""
 
 DRIVER_TRANSLATE: Dict[str, str] = {
     'LEC': 'charles leclerc', 'SAI': 'carlos sainz',
     'VER': 'max verstappen', 'PER': 'sergio perez',
     'PIA': 'oscar piastri', 'NOR': 'lando norris',
     'GAS': 'pierre gasly', 'OCO': 'esteban ocon',
     'BOT': 'valtteri bottas', 'ZHO': 'zhou guanyu',
     'DEV': 'nyck de vries', 'TSU': 'yuki tsunoda',
-    'MAG': 'kevin magnussen', 'HUL': 'nico hulkenburg',
+    'MAG': 'kevin magnussen', 'HUL': 'nico hulkenberg',
     'ALO': 'fernando alonso', 'STR': 'lance stroll', 'DRU': 'felipe drugovich',
     'HAM': 'lewis hamilton', 'RUS': 'george russell',
     'ALB': 'alexander albon', 'SAR': 'logan sargeant'}
 """Mapping of driver names to theirs respective abbreviations."""
 
-COLOR_PALETTE = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
-                 '#FFB86C', '#FF5555', '#F1FA8C']
+COMPOUND_COLORS: Dict[str, str] = {
+    "SOFT": "da291c",
+    "MEDIUM": "ffd12e",
+    "HARD": "f0f0ec",
+    "INTERMEDIATE": "43b02a",
+    "WET": "0067ad",
+    "UNKNOWN": "00ffff",
+}
+"""Mapping of tyre compound names to compound colors (hex color codes).
+(current season only)"""
+
+COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
+                            '#FFB86C', '#FF5555', '#F1FA8C']
 """The default color palette for matplotlib plot lines in fastf1's color
 scheme."""
 
 
-def setup_mpl(mpl_timedelta_support=True, color_scheme='fastf1',
-              misc_mpl_mods=True):
+def setup_mpl(
+        mpl_timedelta_support: bool = True, color_scheme: str = 'fastf1',
+        misc_mpl_mods: bool = True):
     """Setup matplotlib for use with fastf1.
 
     This is optional but, at least partly, highly recommended.
 
     Parameters:
         mpl_timedelta_support (bool):
             Matplotlib itself offers very limited functionality for plotting
@@ -184,15 +195,15 @@
         _enable_timple()
     if color_scheme == 'fastf1':
         _enable_fastf1_color_scheme()
     if misc_mpl_mods:
         _enable_misc_mpl_mods()
 
 
-def driver_color(identifier):
+def driver_color(identifier: str) -> str:
     """Get a driver's color from a driver name or abbreviation.
 
     This function will try to find a matching driver for any identifier string
     that is passed to it. This involves case insensitive matching and partial
     string matching.
 
     If you want exact string matching, you should use the
@@ -242,24 +253,25 @@
 
         # do fuzzy string matching
         key_ratios = list()
         for existing_key in DRIVER_COLORS.keys():
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
-        if (key_ratios[0][0] < 35) or (key_ratios[0][0]/key_ratios[1][0] < 1.2):
+        if ((key_ratios[0][0] < 35)
+                or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
         return DRIVER_COLORS[best_matched_key]
 
 
-def team_color(identifier):
+def team_color(identifier: str) -> str:
     """Get a team's color from a team name or abbreviation.
 
     This function will try to find a matching team for any identifier string
     that is passed to it. This involves case insensitive matching and partial
     string matching.
 
     If you want exact string matching, you should use the
@@ -315,15 +327,16 @@
 
         # do fuzzy string matching
         key_ratios = list()
         for existing_key in TEAM_COLORS.keys():
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
-        if (key_ratios[0][0] < 35) or (key_ratios[0][0]/key_ratios[1][0] < 1.2):
+        if ((key_ratios[0][0] < 35)
+                or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
         return TEAM_COLORS[best_matched_key]
 
@@ -381,14 +394,15 @@
                 for key in kwargs:
                     if isinstance(kwargs[key], (pd.core.series.Series)):
                         kwargs[key] = kwargs[key].to_numpy()
                     if isinstance(kwargs[key], (list, np.ndarray)):
                         kwargs[key] = [kwargs[key][i] for i in _ids]
                 kwargs.pop('sort', None)
             return bar(*args, **kwargs)
+
         return _bar_sorted_decorator
 
     plt.bar = _bar_sorted(plt.bar)
     plt.barh = _bar_sorted(plt.barh)
     matplotlib.axes.Axes.bar = _bar_sorted(matplotlib.axes.Axes.bar)
     matplotlib.axes.Axes.barh = _bar_sorted(matplotlib.axes.Axes.barh)
```

### Comparing `fastf1-2.3.3/fastf1/utils.py` & `fastf1-3.0.0/fastf1/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-"""
-Utils module - :mod:`fastf1.utils`
-==================================
-"""
-import warnings
+"""This is a collection of various functions."""
+import datetime
 from functools import reduce
+from typing import Dict, Tuple, Optional
+import warnings
 
 import numpy as np
-from datetime import datetime, timedelta
+import pandas as pd
+
+from fastf1.logger import get_logger
 
 
-def delta_time(reference_lap, compare_lap):
-    # TODO move somewhere else
+_logger = get_logger(__name__)
+
+
+def delta_time(reference_lap: pd.Series, compare_lap: pd.Series) -> Tuple:
     """Calculates the delta time of a given lap, along the 'Distance' axis
     of the reference lap.
 
+    .. deprecated:: 3.0.0
+
+    .. warning:: This function should no longer be considered as a stable part
+        of the API. Due to the reasons given below, this function will be
+        modified or removed at a future point.
+
     .. warning:: This is a nice gimmick but not actually very accurate which
         is an inherent problem from the way this is calculated currently (There
         may not be a better way though). In comparison with the sector times and the
         differences that can be calculated from these, there are notable differences!
         You should always verify the result against sector time differences or find a
         different way for verification.
 
@@ -65,14 +74,19 @@
           - :class:`Telemetry` for the reference lap
           - :class:`Telemetry` for the comparison lap
 
           Use the return telemetry for plotting to make sure you have
           telemetry data that was created with the same interpolation and
           resampling options!
     """
+    warnings.warn("`utils.delta_time` is considered deprecated and will"
+                  "be modified or removed in a future release because it has"
+                  "a tendency to give inaccurate results.",
+                  FutureWarning)
+
     ref = reference_lap.get_car_data(interpolate_edges=True).add_distance()
     comp = compare_lap.get_car_data(interpolate_edges=True).add_distance()
 
     def mini_pro(stream):
         # Ensure that all samples are interpolated
         dstream_start = stream[1] - stream[0]
         dstream_end = stream[-1] - stream[-2]
@@ -83,26 +97,26 @@
     lap_time = np.interp(ref['Distance'], ldistance, ltime)
 
     delta = lap_time - ref['Time'].dt.total_seconds()
 
     return delta, ref, comp
 
 
-def recursive_dict_get(d, *keys, default_none=False):
+def recursive_dict_get(d: Dict, *keys: str, default_none: bool = False):
     """Recursive dict get. Can take an arbitrary number of keys and returns an empty
     dict if any key does not exist.
     https://stackoverflow.com/a/28225747"""
     ret = reduce(lambda c, k: c.get(k, {}), keys, d)
     if default_none and ret == {}:
         return None
     else:
         return ret
 
 
-def to_timedelta(x):
+def to_timedelta(x: str) -> Optional[datetime.timedelta]:
     """Fast timedelta object creation from a time string
 
     Permissible string formats:
 
         For example: `13:24:46.320215` with:
 
             - optional hours and minutes
@@ -136,28 +150,32 @@
                 if len(msus) < 6:
                     msus = msus + '0' * (6 - len(msus))
                 elif len(msus) > 6:
                     msus = msus[0:6]
             else:
                 msus = 0
 
-            return timedelta(hours=int(hours), minutes=int(minutes),
-                             seconds=int(seconds), microseconds=int(msus))
-        except Exception as exc:
-            warnings.warn(
-                "In a future version, `to_timedelta` will return NaT instead "
-                "of raising an exception if a value cannot be parsed.",
-                FutureWarning
+            return datetime.timedelta(
+                hours=int(hours), minutes=int(minutes),
+                seconds=int(seconds), microseconds=int(msus)
             )
-            raise exc
-    elif isinstance(x, timedelta):
+
+        except Exception as exc:
+            _logger.debug(f"Failed to parse timedelta string '{x}'",
+                          exc_info=exc)
+            return None
+
+    elif isinstance(x, datetime.timedelta):
         return x
 
+    else:
+        return None
+
 
-def to_datetime(x):
+def to_datetime(x) -> Optional[datetime.datetime]:
     """Fast datetime object creation from a date string.
 
     Permissible string formats:
 
         For example '2020-12-13T13:27:15.320000Z' with:
 
             - optional milliseconds and microseconds with
@@ -179,24 +197,28 @@
         try:
             date, time = x.strip('Z').split('T')
             year, month, day = date.split('-')
             hours, minutes, seconds = time.split(':')
             if '.' in seconds:
                 seconds, msus = seconds.split('.')
                 if len(msus) < 6:
-                    msus = msus+'0'*(6-len(msus))
+                    msus = msus + '0' * (6 - len(msus))
                 elif len(msus) > 6:
                     msus = msus[0:6]
             else:
                 msus = 0
 
-            return datetime(int(year), int(month), int(day), int(hours),
-                            int(minutes), int(seconds), int(msus))
-        except Exception as exc:
-            warnings.warn(
-                "In a future version, `to_datetime` will return NaT instead "
-                "of raising an exception if a value cannot be parsed.",
-                FutureWarning
+            return datetime.datetime(
+                int(year), int(month), int(day), int(hours),
+                int(minutes), int(seconds), int(msus)
             )
-            raise exc
-    elif isinstance(x, datetime):
+
+        except Exception as exc:
+            _logger.debug(f"Failed to parse datetime string '{x}'",
+                          exc_info=exc)
+            return None
+
+    elif isinstance(x, datetime.datetime):
         return x
+
+    else:
+        return None
```

### Comparing `fastf1-2.3.3/setup.cfg` & `fastf1-3.0.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -9,32 +9,38 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
 zip_safe = False
 packages = 
 	fastf1
+	fastf1.ergast
 	fastf1.livetiming
+	fastf1.signalr_aio
 python_requires = >= 3.8
 install_requires = 
-	requests
 	requests-cache>=0.8.0
-	pandas>=1.1.0,<2.0.0
-	numpy>=1.17.3
-	scipy
+	pandas>=1.2.4
+	numpy>=1.20.3
+	scipy>=1.6.3
 	thefuzz
-	matplotlib>=3.3.3
+	matplotlib>=3.4.2
+	python-dateutil
 	timple>=0.1.2
-	signalr-client-aio
+	requests>=2.28.0
+	websockets>=8.1
 
 [build_sphinx]
 project = Fast F1
 source-dir = ./docs
 build-dir = ./docs/_build
 
 [flake8]
 max-line-length = 120
+extend-ignore = W503
+extend-select = W504
+exclude = fastf1/signalr_aio
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

