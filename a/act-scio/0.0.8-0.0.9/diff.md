# Comparing `tmp/act-scio-0.0.8.tar.gz` & `tmp/act-scio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/act-scio-0.0.8.tar", last modified: Mon Aug 24 10:14:56 2020, max compression
+gzip compressed data, was "dist/act-scio-0.0.9.tar", last modified: Mon Aug 24 11:44:46 2020, max compression
```

## Comparing `act-scio-0.0.8.tar` & `act-scio-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,64 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/scio/
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    10451 2020-08-20 16:29:13.000000 act-scio-0.0.8/act/scio/upload.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1554 2020-08-24 07:39:27.000000 act-scio-0.0.8/act/scio/es.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      199 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/nltk_download.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5455 2020-08-24 10:14:50.000000 act-scio-0.0.8/act/scio/tika_engine.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3440 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugin.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/scio/plugins/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4336 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/locations.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      818 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/tools_pattern.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      521 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/pos_tag.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2352 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/sectors.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    13798 2020-08-20 19:59:52.000000 act-scio-0.0.8/act/scio/plugins/indicators.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1141 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/threatactor_pattern.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       65 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/plugins/__init__.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8005 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/vocabulary.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3809 2020-08-24 10:14:50.000000 act-scio-0.0.8/act/scio/config.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/scio/etc/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      856 2020-08-24 07:39:27.000000 act-scio-0.0.8/act/scio/etc/scio.ini
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8417 2020-08-20 16:29:13.000000 act-scio-0.0.8/act/scio/etc/secstoplist.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1642 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/etc/feeds.txt
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/scio/feeds/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1178 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/upload.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3778 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/cache.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3257 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/feeds.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4477 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/extract.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     6058 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/download.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3430 2020-08-20 16:29:13.000000 act-scio-0.0.8/act/scio/feeds/conf.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3326 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/feeds/analyze.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/feeds/__init__.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act/scio/vendor/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)  5912447 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/vendor/cities15000.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    65351 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/vendor/ISO-3166-countries-with-regional-codes.json
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    28565 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/vendor/countryInfo.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5915 2020-08-24 10:14:50.000000 act-scio-0.0.8/act/scio/api.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4186 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/alias.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5302 2020-08-24 10:14:50.000000 act-scio-0.0.8/act/scio/analyze.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3642 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/scio_config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2534 2020-08-14 08:11:45.000000 act-scio-0.0.8/act/scio/logsetup.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       65 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5090 2020-07-01 08:06:42.000000 act-scio-0.0.8/act/scio/aliasregex.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1188 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3878 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-08-03 06:54:01.000000 act-scio-0.0.8/act_scio.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/namespace_packages.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      179 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      293 2020-08-24 10:14:56.000000 act-scio-0.0.8/act_scio.egg-info/entry_points.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2020-08-24 10:14:56.000000 act-scio-0.0.8/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2568 2020-07-01 08:06:42.000000 act-scio-0.0.8/README.md
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3878 2020-08-24 10:14:56.000000 act-scio-0.0.8/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2185 2020-08-24 10:14:50.000000 act-scio-0.0.8/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    10451 2020-08-20 16:29:13.000000 act-scio-0.0.9/act/scio/upload.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1554 2020-08-24 07:39:27.000000 act-scio-0.0.9/act/scio/es.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      199 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/nltk_download.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5455 2020-08-24 10:14:50.000000 act-scio-0.0.9/act/scio/tika_engine.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3440 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugin.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/plugins/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4336 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/locations.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      818 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/tools_pattern.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      521 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/pos_tag.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2352 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/sectors.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    13798 2020-08-20 19:59:52.000000 act-scio-0.0.9/act/scio/plugins/indicators.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1141 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/threatactor_pattern.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       65 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/plugins/__init__.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8005 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/vocabulary.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3809 2020-08-24 10:14:50.000000 act-scio-0.0.9/act/scio/config.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/etc/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      856 2020-08-24 07:39:27.000000 act-scio-0.0.9/act/scio/etc/scio.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8417 2020-08-20 16:29:13.000000 act-scio-0.0.9/act/scio/etc/secstoplist.txt
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/etc/plugins/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1645 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/sectors.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      193 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/locations.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1722 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/tools.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5823 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/ta_aliases.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      268 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/threatactor_pattern.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       87 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/sectors.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       81 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/tools_pattern.ini
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    21101 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/plugins/country_aliases.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1642 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/etc/feeds.txt
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/feeds/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1178 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/upload.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3778 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/cache.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     3257 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/feeds.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4477 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/extract.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     6058 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/download.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3430 2020-08-20 16:29:13.000000 act-scio-0.0.9/act/scio/feeds/conf.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3326 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/feeds/analyze.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/feeds/__init__.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act/scio/vendor/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)  5912447 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/vendor/cities15000.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    65351 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/vendor/ISO-3166-countries-with-regional-codes.json
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    28565 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/vendor/countryInfo.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     5915 2020-08-24 10:14:50.000000 act-scio-0.0.9/act/scio/api.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4186 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/alias.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5302 2020-08-24 10:14:50.000000 act-scio-0.0.9/act/scio/analyze.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3642 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/scio_config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     2534 2020-08-14 08:11:45.000000 act-scio-0.0.9/act/scio/logsetup.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       65 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     5090 2020-07-01 08:06:42.000000 act-scio-0.0.9/act/scio/aliasregex.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2020-08-24 11:44:46.000000 act-scio-0.0.9/act_scio.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1481 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3878 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-08-03 06:54:01.000000 act-scio-0.0.9/act_scio.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/namespace_packages.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      179 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      293 2020-08-24 11:44:45.000000 act-scio-0.0.9/act_scio.egg-info/entry_points.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2020-08-24 11:44:46.000000 act-scio-0.0.9/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2568 2020-07-01 08:06:42.000000 act-scio-0.0.9/README.md
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     3878 2020-08-24 11:44:46.000000 act-scio-0.0.9/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2202 2020-08-24 11:44:40.000000 act-scio-0.0.9/setup.py
```

### Comparing `act-scio-0.0.8/act/scio/upload.py` & `act-scio-0.0.9/act/scio/upload.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/es.py` & `act-scio-0.0.9/act/scio/es.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/tika_engine.py` & `act-scio-0.0.9/act/scio/tika_engine.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugin.py` & `act-scio-0.0.9/act/scio/plugin.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/locations.py` & `act-scio-0.0.9/act/scio/plugins/locations.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/tools_pattern.py` & `act-scio-0.0.9/act/scio/plugins/tools_pattern.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/pos_tag.py` & `act-scio-0.0.9/act/scio/plugins/pos_tag.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/sectors.py` & `act-scio-0.0.9/act/scio/plugins/sectors.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/indicators.py` & `act-scio-0.0.9/act/scio/plugins/indicators.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/plugins/threatactor_pattern.py` & `act-scio-0.0.9/act/scio/plugins/threatactor_pattern.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/vocabulary.py` & `act-scio-0.0.9/act/scio/vocabulary.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/config.py` & `act-scio-0.0.9/act/scio/config.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/etc/scio.ini` & `act-scio-0.0.9/act/scio/etc/scio.ini`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/etc/secstoplist.txt` & `act-scio-0.0.9/act/scio/etc/secstoplist.txt`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/etc/feeds.txt` & `act-scio-0.0.9/act/scio/etc/feeds.txt`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/upload.py` & `act-scio-0.0.9/act/scio/feeds/upload.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/cache.py` & `act-scio-0.0.9/act/scio/feeds/cache.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/feeds.py` & `act-scio-0.0.9/act/scio/feeds/feeds.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/extract.py` & `act-scio-0.0.9/act/scio/feeds/extract.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/download.py` & `act-scio-0.0.9/act/scio/feeds/download.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/conf.py` & `act-scio-0.0.9/act/scio/feeds/conf.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/feeds/analyze.py` & `act-scio-0.0.9/act/scio/feeds/analyze.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/vendor/cities15000.txt` & `act-scio-0.0.9/act/scio/vendor/cities15000.txt`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/vendor/ISO-3166-countries-with-regional-codes.json` & `act-scio-0.0.9/act/scio/vendor/ISO-3166-countries-with-regional-codes.json`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/vendor/countryInfo.txt` & `act-scio-0.0.9/act/scio/vendor/countryInfo.txt`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/api.py` & `act-scio-0.0.9/act/scio/api.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/alias.py` & `act-scio-0.0.9/act/scio/alias.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/analyze.py` & `act-scio-0.0.9/act/scio/analyze.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/scio_config.py` & `act-scio-0.0.9/act/scio/scio_config.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/logsetup.py` & `act-scio-0.0.9/act/scio/logsetup.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act/scio/aliasregex.py` & `act-scio-0.0.9/act/scio/aliasregex.py`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/act_scio.egg-info/SOURCES.txt` & `act-scio-0.0.9/act_scio.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 act/scio/scio_config.py
 act/scio/tika_engine.py
 act/scio/upload.py
 act/scio/vocabulary.py
 act/scio/etc/feeds.txt
 act/scio/etc/scio.ini
 act/scio/etc/secstoplist.txt
+act/scio/etc/plugins/country_aliases.cfg
+act/scio/etc/plugins/locations.ini
+act/scio/etc/plugins/sectors.cfg
+act/scio/etc/plugins/sectors.ini
+act/scio/etc/plugins/ta_aliases.cfg
+act/scio/etc/plugins/threatactor_pattern.ini
+act/scio/etc/plugins/tools.cfg
+act/scio/etc/plugins/tools_pattern.ini
 act/scio/feeds/__init__.py
 act/scio/feeds/analyze.py
 act/scio/feeds/cache.py
 act/scio/feeds/conf.py
 act/scio/feeds/download.py
 act/scio/feeds/extract.py
 act/scio/feeds/feeds.py
```

### Comparing `act-scio-0.0.8/act_scio.egg-info/PKG-INFO` & `act-scio-0.0.9/act_scio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-scio
-Version: 0.0.8
+Version: 0.0.9
 Summary: ACT SCIO
 Home-page: https://github.com/mnemonic-no/act-scio2
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: MIT
 Description: # act-scio2
         Scio v2 is a reimplementation of [Scio](https://github.com/mnemonic-no/act-scio) in Python3.
```

### Comparing `act-scio-0.0.8/README.md` & `act-scio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `act-scio-0.0.8/PKG-INFO` & `act-scio-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-scio
-Version: 0.0.8
+Version: 0.0.9
 Summary: ACT SCIO
 Home-page: https://github.com/mnemonic-no/act-scio2
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: MIT
 Description: # act-scio2
         Scio v2 is a reimplementation of [Scio](https://github.com/mnemonic-no/act-scio) in Python3.
```

### Comparing `act-scio-0.0.8/setup.py` & `act-scio-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), "rb") as f:
     long_description = f.read().decode('utf-8')
 
 setup(
     name="act-scio",
-    version="0.0.8",
+    version="0.0.9",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="ACT SCIO",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
@@ -29,15 +29,15 @@
             'scio-tika-server = act.scio.tika_engine:main',
             'scio-nltk-download= act.scio.nltk_download:main',
             'scio-upload = act.scio.upload:main',
         ]
     },
 
     # Include ini-file(s) from act/workers/etc
-    package_data={'act.scio': ['etc/*', 'vendor/*']},
+    package_data={'act.scio': ['etc/*', 'etc/plugins/*', 'vendor/*']},
     packages=["act.scio", "act.scio.plugins", "act.scio.feeds"],
 
     # https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages
     # __init__.py under all packages under in the act namespace must contain exactly string:
     # __path__ = __import__('pkgutil').extend_path(__path__, __name__)
     namespace_packages=['act'],
     url="https://github.com/mnemonic-no/act-scio2",
```

