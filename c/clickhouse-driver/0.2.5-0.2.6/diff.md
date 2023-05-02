# Comparing `tmp/clickhouse-driver-0.2.5.tar.gz` & `tmp/clickhouse-driver-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-driver-0.2.5.tar", last modified: Sun Nov 27 19:19:59 2022, max compression
+gzip compressed data, was "clickhouse-driver-0.2.6.tar", last modified: Tue May  2 12:54:16 2023, max compression
```

## Comparing `clickhouse-driver-0.2.5.tar` & `clickhouse-driver-0.2.6.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.945161 clickhouse-driver-0.2.5/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1143 2017-05-22 18:29:36.000000 clickhouse-driver-0.2.5/LICENSE
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       42 2020-12-18 20:37:43.000000 clickhouse-driver-0.2.5/MANIFEST.in
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6931 2022-11-27 19:19:59.945161 clickhouse-driver-0.2.5/PKG-INFO
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4014 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/README.rst
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.913160 clickhouse-driver-0.2.5/clickhouse_driver/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      158 2022-11-27 15:11:31.000000 clickhouse-driver-0.2.5/clickhouse_driver/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6215 2022-06-06 17:01:14.000000 clickhouse-driver-0.2.5/clickhouse_driver/block.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      712 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/blockstreamprofileinfo.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   469939 2022-11-05 20:07:45.000000 clickhouse-driver-0.2.5/clickhouse_driver/bufferedreader.c
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     8811 2021-11-24 20:28:39.000000 clickhouse-driver-0.2.5/clickhouse_driver/bufferedreader.pyx
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   437728 2022-11-05 20:07:45.000000 clickhouse-driver-0.2.5/clickhouse_driver/bufferedwriter.c
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4325 2021-11-16 20:15:46.000000 clickhouse-driver-0.2.5/clickhouse_driver/bufferedwriter.pyx
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    30231 2022-11-27 15:11:31.000000 clickhouse-driver-0.2.5/clickhouse_driver/client.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4242 2022-03-16 21:38:38.000000 clickhouse-driver-0.2.5/clickhouse_driver/clientinfo.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.933161 clickhouse-driver-0.2.5/clickhouse_driver/columns/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5084 2022-11-05 20:09:34.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/arraycolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4510 2022-07-28 09:44:13.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      127 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/boolcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1931 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/datecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6691 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/datetimecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3450 2022-03-04 14:51:53.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/decimalcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3219 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/enumcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      163 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/exceptions.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      925 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/floatcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3519 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/intcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      600 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/intervalcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4095 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/ipcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   275236 2022-11-05 20:07:45.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/largeint.c
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6078 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/largeint.pyx
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4042 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/lowcardinalitycolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1964 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/mapcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      619 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/nestedcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      259 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/nothingcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      169 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/nullablecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      331 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/nullcolumn.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.937161 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1410 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      140 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/boolcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      482 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/datecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4610 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/datetimecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      599 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/floatcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      792 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/intcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3332 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/lowcardinalitycolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2126 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/service.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2439 2022-01-20 12:49:04.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/stringcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1233 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/tuplecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5863 2022-07-28 09:44:13.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/service.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      235 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/simpleaggregatefunctioncolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2059 2021-10-25 08:30:30.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/stringcolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1149 2022-07-28 09:44:13.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/tuplecolumn.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1395 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/util.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1823 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/columns/uuidcolumn.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.937161 clickhouse-driver-0.2.5/clickhouse_driver/compression/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      714 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/compression/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2434 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/compression/base.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      631 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/compression/lz4.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      195 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/compression/lz4hc.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      531 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/compression/zstd.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    24589 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.5/clickhouse_driver/connection.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      909 2022-04-22 22:02:15.000000 clickhouse-driver-0.2.5/clickhouse_driver/context.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.941161 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1759 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3032 2022-02-21 08:04:44.000000 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/connection.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    10517 2022-02-20 16:12:45.000000 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/cursor.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      440 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/errors.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2129 2022-02-21 08:04:44.000000 clickhouse-driver-0.2.5/clickhouse_driver/dbapi/extras.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1469 2022-07-28 09:44:13.000000 clickhouse-driver-0.2.5/clickhouse_driver/defines.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    14343 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/errors.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      888 2022-03-13 16:02:39.000000 clickhouse-driver-0.2.5/clickhouse_driver/log.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.941161 clickhouse-driver-0.2.5/clickhouse_driver/numpy/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/numpy/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      180 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/numpy/block.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      704 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/numpy/helpers.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3563 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/numpy/result.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1622 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/opentelemetry.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1039 2021-09-03 20:53:17.000000 clickhouse-driver-0.2.5/clickhouse_driver/progress.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2561 2022-03-16 21:38:38.000000 clickhouse-driver-0.2.5/clickhouse_driver/protocol.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      186 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/queryprocessingstage.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1322 2021-08-05 18:35:40.000000 clickhouse-driver-0.2.5/clickhouse_driver/reader.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      717 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/readhelpers.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4098 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/result.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.941161 clickhouse-driver-0.2.5/clickhouse_driver/settings/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/settings/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    16613 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/settings/available.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1108 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/settings/types.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1064 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/settings/writer.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.941161 clickhouse-driver-0.2.5/clickhouse_driver/streams/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/streams/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2865 2021-11-20 12:36:39.000000 clickhouse-driver-0.2.5/clickhouse_driver/streams/compressed.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2728 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/streams/native.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.945161 clickhouse-driver-0.2.5/clickhouse_driver/util/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.5/clickhouse_driver/util/__init__.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      695 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.5/clickhouse_driver/util/compat.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1453 2022-05-04 21:43:19.000000 clickhouse-driver-0.2.5/clickhouse_driver/util/escape.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1448 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/util/helpers.py
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   171545 2022-11-05 20:07:45.000000 clickhouse-driver-0.2.5/clickhouse_driver/varint.c
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1743 2021-11-16 20:15:46.000000 clickhouse-driver-0.2.5/clickhouse_driver/varint.pyx
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1286 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.5/clickhouse_driver/writer.py
-drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2022-11-27 19:19:59.917160 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6931 2022-11-27 19:19:59.000000 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/PKG-INFO
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3541 2022-11-27 19:19:59.000000 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        1 2022-11-27 19:19:59.000000 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      218 2022-11-27 19:19:59.000000 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/requires.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       18 2022-11-27 19:19:59.000000 clickhouse-driver-0.2.5/clickhouse_driver.egg-info/top_level.txt
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      257 2022-11-27 19:19:59.945161 clickhouse-driver-0.2.5/setup.cfg
--rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3871 2022-11-27 15:11:31.000000 clickhouse-driver-0.2.5/setup.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.445365 clickhouse-driver-0.2.6/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1143 2017-05-22 18:29:36.000000 clickhouse-driver-0.2.6/LICENSE
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       42 2020-12-18 20:37:43.000000 clickhouse-driver-0.2.6/MANIFEST.in
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6881 2023-05-02 12:54:16.445365 clickhouse-driver-0.2.6/PKG-INFO
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4014 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/README.rst
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.401365 clickhouse-driver-0.2.6/clickhouse_driver/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      158 2023-03-12 09:18:32.000000 clickhouse-driver-0.2.6/clickhouse_driver/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6311 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/block.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      712 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/blockstreamprofileinfo.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   469939 2023-02-27 16:39:58.000000 clickhouse-driver-0.2.6/clickhouse_driver/bufferedreader.c
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     8811 2023-02-27 16:39:58.000000 clickhouse-driver-0.2.6/clickhouse_driver/bufferedreader.pyx
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   437728 2023-02-27 16:39:58.000000 clickhouse-driver-0.2.6/clickhouse_driver/bufferedwriter.c
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4325 2023-02-27 16:39:58.000000 clickhouse-driver-0.2.6/clickhouse_driver/bufferedwriter.pyx
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    31798 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/client.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4260 2023-04-26 22:06:22.000000 clickhouse-driver-0.2.6/clickhouse_driver/clientinfo.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.425365 clickhouse-driver-0.2.6/clickhouse_driver/columns/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     5322 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/arraycolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6504 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      127 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/boolcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1931 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/datecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6691 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/datetimecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3450 2022-03-04 14:51:53.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/decimalcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3219 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/enumcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      163 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/exceptions.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      925 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/floatcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3519 2023-04-20 17:21:09.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/intcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      600 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/intervalcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4095 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/ipcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1175 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/jsoncolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   275236 2022-11-05 20:07:45.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/largeint.c
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6078 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/largeint.pyx
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4920 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/lowcardinalitycolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2084 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/mapcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      303 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/nestedcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      259 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/nothingcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      169 2019-07-18 11:24:49.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/nullablecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      331 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/nullcolumn.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.433365 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1410 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      140 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/boolcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      482 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/datecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4777 2023-04-09 22:36:03.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/datetimecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      599 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/floatcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      792 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/intcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3368 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/lowcardinalitycolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2126 2022-10-27 09:10:03.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/service.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2439 2022-01-20 12:49:04.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/stringcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1233 2023-04-19 17:30:43.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/tuplecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6181 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/service.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      235 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/simpleaggregatefunctioncolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2059 2021-10-25 08:30:30.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/stringcolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2040 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/tuplecolumn.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1395 2022-06-13 15:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/util.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1823 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/columns/uuidcolumn.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.437365 clickhouse-driver-0.2.6/clickhouse_driver/compression/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      714 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/compression/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2434 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/compression/base.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      631 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/compression/lz4.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      195 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/compression/lz4hc.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      531 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/compression/zstd.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    27679 2023-05-02 10:35:45.000000 clickhouse-driver-0.2.6/clickhouse_driver/connection.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      909 2022-04-22 22:02:15.000000 clickhouse-driver-0.2.6/clickhouse_driver/context.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.437365 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1759 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3032 2022-02-21 08:04:44.000000 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/connection.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    10517 2022-02-20 16:12:45.000000 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/cursor.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      440 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/errors.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2129 2022-02-21 08:04:44.000000 clickhouse-driver-0.2.6/clickhouse_driver/dbapi/extras.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1704 2023-04-26 22:06:22.000000 clickhouse-driver-0.2.6/clickhouse_driver/defines.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    14343 2022-02-07 11:02:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/errors.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      888 2022-03-13 16:02:39.000000 clickhouse-driver-0.2.6/clickhouse_driver/log.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.441365 clickhouse-driver-0.2.6/clickhouse_driver/numpy/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/numpy/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      180 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/numpy/block.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      704 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/numpy/helpers.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3563 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/numpy/result.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1622 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/opentelemetry.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1045 2023-05-02 10:35:45.000000 clickhouse-driver-0.2.6/clickhouse_driver/progress.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2561 2022-03-16 21:38:38.000000 clickhouse-driver-0.2.6/clickhouse_driver/protocol.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      186 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/queryprocessingstage.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1322 2023-03-12 22:42:40.000000 clickhouse-driver-0.2.6/clickhouse_driver/reader.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      717 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/readhelpers.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     4098 2023-04-10 17:10:03.000000 clickhouse-driver-0.2.6/clickhouse_driver/result.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.441365 clickhouse-driver-0.2.6/clickhouse_driver/settings/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/settings/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)    16613 2021-01-06 14:31:54.000000 clickhouse-driver-0.2.6/clickhouse_driver/settings/available.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1108 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/settings/types.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1099 2023-04-26 22:06:22.000000 clickhouse-driver-0.2.6/clickhouse_driver/settings/writer.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.445365 clickhouse-driver-0.2.6/clickhouse_driver/streams/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/streams/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2865 2021-11-20 12:36:39.000000 clickhouse-driver-0.2.6/clickhouse_driver/streams/compressed.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3316 2023-05-02 10:35:45.000000 clickhouse-driver-0.2.6/clickhouse_driver/streams/native.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.445365 clickhouse-driver-0.2.6/clickhouse_driver/util/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        0 2019-01-07 18:24:36.000000 clickhouse-driver-0.2.6/clickhouse_driver/util/__init__.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      876 2023-04-28 20:09:59.000000 clickhouse-driver-0.2.6/clickhouse_driver/util/compat.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     2256 2023-04-26 22:06:22.000000 clickhouse-driver-0.2.6/clickhouse_driver/util/escape.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1448 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/util/helpers.py
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)   171545 2023-04-19 17:20:52.000000 clickhouse-driver-0.2.6/clickhouse_driver/varint.c
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1743 2023-04-16 18:11:35.000000 clickhouse-driver-0.2.6/clickhouse_driver/varint.pyx
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     1286 2021-09-28 21:41:41.000000 clickhouse-driver-0.2.6/clickhouse_driver/writer.py
+drwxrwxr-x   0 klebedev  (1000) klebedev  (1000)        0 2023-05-02 12:54:16.405365 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     6881 2023-05-02 12:54:16.000000 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3581 2023-05-02 12:54:16.000000 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)        1 2023-05-02 12:54:16.000000 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      218 2023-05-02 12:54:16.000000 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/requires.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)       18 2023-05-02 12:54:16.000000 clickhouse-driver-0.2.6/clickhouse_driver.egg-info/top_level.txt
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)      257 2023-05-02 12:54:16.445365 clickhouse-driver-0.2.6/setup.cfg
+-rw-rw-r--   0 klebedev  (1000) klebedev  (1000)     3822 2023-04-26 21:00:23.000000 clickhouse-driver-0.2.6/setup.py
```

### Comparing `clickhouse-driver-0.2.5/LICENSE` & `clickhouse-driver-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/PKG-INFO` & `clickhouse-driver-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-driver
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python driver with native interface for ClickHouse
 Home-page: https://github.com/mymarilyn/clickhouse-driver
 Author: Konstantin Lebedev
 Author-email: kostyan.lebedev@gmail.com
 License: MIT
 Project-URL: Documentation, https://clickhouse-driver.readthedocs.io
 Project-URL: Changes, https://github.com/mymarilyn/clickhouse-driver/blob/master/CHANGELOG.md
@@ -170,24 +170,23 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: lz4
 Provides-Extra: zstd
 Provides-Extra: numpy
```

### Comparing `clickhouse-driver-0.2.5/README.rst` & `clickhouse-driver-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/block.py` & `clickhouse-driver-0.2.6/clickhouse_driver/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from .columns.util import get_inner_spec, get_inner_columns_with_types
 from .reader import read_varint, read_binary_uint8, read_binary_int32
 from .varint import write_varint
 from .writer import write_binary_uint8, write_binary_int32
-from .columns import nestedcolumn
 
 
 class BlockInfo(object):
     is_overflows = False
     bucket_num = -1
 
     def write(self, buf):
@@ -168,15 +168,16 @@
         columns_with_types,
         check_row_type,
     ):
         columns_with_cwt = []
         for name, type_ in columns_with_types:
             cwt = None
             if type_.startswith('Nested'):
-                cwt = nestedcolumn.get_columns_with_types(type_)
+                inner_spec = get_inner_spec('Nested', type_)
+                cwt = get_inner_columns_with_types(inner_spec)
             columns_with_cwt.append((name, cwt))
 
         for i, row in enumerate(data):
             if check_row_type:
                 check_row_type(row)
 
             new_data = []
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/blockstreamprofileinfo.py` & `clickhouse-driver-0.2.6/clickhouse_driver/blockstreamprofileinfo.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/bufferedreader.c` & `clickhouse-driver-0.2.6/clickhouse_driver/bufferedreader.c`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/bufferedreader.pyx` & `clickhouse-driver-0.2.6/clickhouse_driver/bufferedreader.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/bufferedwriter.c` & `clickhouse-driver-0.2.6/clickhouse_driver/bufferedwriter.c`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/bufferedwriter.pyx` & `clickhouse-driver-0.2.6/clickhouse_driver/bufferedwriter.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/client.py` & `clickhouse-driver-0.2.6/clickhouse_driver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,25 +53,32 @@
         * ``input_format_null_as_default`` -- Initialize null fields with
                            default values if data type of this field is not
                            nullable. Does not work for NumPy. Default: False.
                            New in version *0.2.4*.
         * ``round_robin`` -- If ``alt_hosts`` are provided the query will be
                            executed on host picked with round-robin algorithm.
                            New in version *0.2.5*.
+        * ``namedtuple_as_json`` -- Controls named tuple and nested types
+                           deserialization. To interpret these column alongside
+                           with ``allow_experimental_object_type=1`` as Python
+                           tuple set ``namedtuple_as_json`` to ``False``.
+                           Default: True.
+                           New in version *0.2.6*.
     """
 
     available_client_settings = (
         'insert_block_size',  # TODO: rename to max_insert_block_size
         'strings_as_bytes',
         'strings_encoding',
         'use_numpy',
         'opentelemetry_traceparent',
         'opentelemetry_tracestate',
         'quota_key',
-        'input_format_null_as_default'
+        'input_format_null_as_default',
+        'namedtuple_as_json'
     )
 
     def __init__(self, *args, **kwargs):
         self.settings = (kwargs.pop('settings', None) or {}).copy()
 
         self.client_settings = {
             'insert_block_size': int(self.settings.pop(
@@ -93,14 +100,17 @@
                 'opentelemetry_tracestate', ''
             ),
             'quota_key': self.settings.pop(
                 'quota_key', ''
             ),
             'input_format_null_as_default': self.settings.pop(
                 'input_format_null_as_default', False
+            ),
+            'namedtuple_as_json': self.settings.pop(
+                'namedtuple_as_json', True
             )
         }
 
         if self.client_settings['use_numpy']:
             try:
                 from .numpy.result import (
                     NumpyIterQueryResult, NumpyProgressQueryResult,
@@ -121,21 +131,27 @@
 
         if round_robin and 'alt_hosts' in kwargs:
             alt_hosts = kwargs.pop('alt_hosts')
             for host in alt_hosts.split(','):
                 url = urlparse('clickhouse://' + host)
 
                 connection_kwargs = kwargs.copy()
-                if len(args) > 2:
-                    # port as positional argument
+                num_args = len(args)
+                if num_args >= 2:
+                    # host and port as positional arguments
                     connection_args = (url.hostname, url.port) + args[2:]
-                else:
-                    # port as keyword argument
+                elif num_args >= 1:
+                    # host as positional and port as keyword argument
                     connection_args = (url.hostname, ) + args[1:]
                     connection_kwargs['port'] = url.port
+                else:
+                    # host and port as keyword arguments
+                    connection_args = tuple()
+                    connection_kwargs['host'] = url.hostname
+                    connection_kwargs['port'] = url.port
 
                 connection = Connection(*connection_args, **connection_kwargs)
                 self.connections.append(connection)
 
         self.connection = self.get_connection()
         self.reset_last_query()
         super(Client, self).__init__()
@@ -434,44 +450,49 @@
                 external_tables=external_tables,
                 query_id=query_id, types_check=types_check
             )
             return chunks(rv, chunk_size) if chunk_size > 1 else rv
 
     def query_dataframe(
             self, query, params=None, external_tables=None, query_id=None,
-            settings=None):
+            settings=None, replace_nonwords=True):
         """
         *New in version 0.2.0.*
 
         Queries DataFrame with specified SELECT query.
 
         :param query: query that will be send to server.
         :param params: substitution parameters.
                        Defaults to ``None`` (no parameters  or data).
         :param external_tables: external tables to send.
                                 Defaults to ``None`` (no external tables).
         :param query_id: the query identifier. If no query id specified
                          ClickHouse server will generate it.
         :param settings: dictionary of query settings.
                          Defaults to ``None`` (no additional settings).
+        :param replace_nonwords: boolean to replace non-words in column names
+                                 to underscores. Defaults to ``True``.
         :return: pandas DataFrame.
         """
 
         try:
             import pandas as pd
         except ImportError:
             raise RuntimeError('Extras for NumPy must be installed')
 
         data, columns = self.execute(
             query, columnar=True, with_column_types=True, params=params,
             external_tables=external_tables, query_id=query_id,
             settings=settings
         )
 
-        columns = [re.sub(r'\W', '_', name) for name, type_ in columns]
+        columns = [name for name, type_ in columns]
+        if replace_nonwords:
+            columns = [re.sub(r'\W', '_', x) for x in columns]
+
         return pd.DataFrame(
             {col: d for d, col in zip(data, columns)}, columns=columns
         )
 
     def insert_dataframe(
             self, query, dataframe, external_tables=None, query_id=None,
             settings=None):
@@ -525,31 +546,30 @@
             types_check=False, columnar=False):
 
         if params is not None:
             query = self.substitute_params(
                 query, params, self.connection.context
             )
 
-        self.connection.send_query(query, query_id=query_id)
+        self.connection.send_query(query, query_id=query_id, params=params)
         self.connection.send_external_tables(external_tables,
                                              types_check=types_check)
         return self.receive_result(with_column_types=with_column_types,
                                    progress=True, columnar=columnar)
 
     def process_ordinary_query(
             self, query, params=None, with_column_types=False,
             external_tables=None, query_id=None,
             types_check=False, columnar=False):
 
         if params is not None:
             query = self.substitute_params(
                 query, params, self.connection.context
             )
-
-        self.connection.send_query(query, query_id=query_id)
+        self.connection.send_query(query, query_id=query_id, params=params)
         self.connection.send_external_tables(external_tables,
                                              types_check=types_check)
         return self.receive_result(with_column_types=with_column_types,
                                    columnar=columnar)
 
     def iter_process_ordinary_query(
             self, query, params=None, with_column_types=False,
@@ -557,15 +577,15 @@
             types_check=False):
 
         if params is not None:
             query = self.substitute_params(
                 query, params, self.connection.context
             )
 
-        self.connection.send_query(query, query_id=query_id)
+        self.connection.send_query(query, query_id=query_id, params=params)
         self.connection.send_external_tables(external_tables,
                                              types_check=types_check)
         return self.iter_receive_result(with_column_types=with_column_types)
 
     def process_insert_query(self, query_without_data, data,
                              external_tables=None, query_id=None,
                              types_check=False, columnar=False):
@@ -769,14 +789,25 @@
 
             elif name == 'compress_block_size':
                 kwargs[name] = int(value)
 
             elif name == 'settings_is_important':
                 kwargs[name] = asbool(value)
 
+            elif name == 'tcp_keepalive':
+                try:
+                    kwargs[name] = asbool(value)
+                except ValueError:
+                    parts = value.split(',')
+                    kwargs[name] = (
+                        float(parts[0]), float(parts[1]), int(parts[2])
+                    )
+            elif name == 'client_revision':
+                kwargs[name] = int(value)
+
             # ssl
             elif name == 'verify':
                 kwargs[name] = asbool(value)
             elif name == 'ssl_version':
                 kwargs[name] = getattr(ssl, value)
             elif name in ['ca_certs', 'ciphers', 'keyfile', 'certfile',
                           'server_hostname']:
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/clientinfo.py` & `clickhouse-driver-0.2.6/clickhouse_driver/clientinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,30 @@
         # Query that was initiated by another query for distributed query
         # execution.
         SECONDARY_QUERY = 2
 
     client_version_major = defines.CLIENT_VERSION_MAJOR
     client_version_minor = defines.CLIENT_VERSION_MINOR
     client_version_patch = defines.CLIENT_VERSION_PATCH
-    client_revision = defines.CLIENT_REVISION
     interface = Interface.TCP
 
     initial_user = ''
     initial_query_id = ''
     initial_address = '0.0.0.0:0'
 
-    def __init__(self, client_name, context):
+    def __init__(self, client_name, context, client_revision):
         self.query_kind = ClientInfo.QueryKind.NO_QUERY
 
         try:
             self.os_user = getpass.getuser()
         except KeyError:
             self.os_user = ''
         self.client_hostname = socket.gethostname()
         self.client_name = client_name
+        self.client_revision = client_revision
 
         self.client_trace_context = OpenTelemetryTraceContext(
             context.client_settings['opentelemetry_traceparent'],
             context.client_settings['opentelemetry_tracestate']
         )
 
         self.quota_key = context.client_settings['quota_key']
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/arraycolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/arraycolumn.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,34 +24,39 @@
     3) size of array 2 plus size of all array before in depth=1: 2 + 2 = 4
 
     After sizes info comes flatten data: 3 -> 4 -> 5 -> 6
     """
     py_types = (list, tuple)
 
     def __init__(self, nested_column, **kwargs):
-        self.size_column = UInt64Column()
+        self.init_kwargs = kwargs
+        self.size_column = UInt64Column(**kwargs)
         self.nested_column = nested_column
         self._write_depth_0_size = True
         super(ArrayColumn, self).__init__(**kwargs)
         self.null_value = []
 
     def write_data(self, data, buf):
         # Column of Array(T) is stored in "compact" format and passed to server
         # wrapped into another Array without size of wrapper array.
-        self.nested_column = ArrayColumn(self.nested_column)
+        self.nested_column = ArrayColumn(
+            self.nested_column, **self.init_kwargs
+        )
         self.nested_column.nullable = self.nullable
         self.nullable = False
         self._write_depth_0_size = False
         self._write(data, buf)
 
-    def read_data(self, rows, buf):
-        self.nested_column = ArrayColumn(self.nested_column)
+    def read_data(self, n_rows, buf):
+        self.nested_column = ArrayColumn(
+            self.nested_column, **self.init_kwargs
+        )
         self.nested_column.nullable = self.nullable
         self.nullable = False
-        return self._read(rows, buf)[0]
+        return self._read(n_rows, buf)[0]
 
     def _write_sizes(self, value, buf):
         nulls_map = []
 
         column = self
         sizes = [len(value)] if self._write_depth_0_size else []
 
@@ -102,17 +107,21 @@
     def _write(self, value, buf):
         value = self.prepare_items(value)
         self._write_sizes(value, buf)
         self._write_nulls_data(value, buf)
         self._write_data(value, buf)
 
     def read_state_prefix(self, buf):
-        return self.nested_column.read_state_prefix(buf)
+        super(ArrayColumn, self).read_state_prefix(buf)
+
+        self.nested_column.read_state_prefix(buf)
 
     def write_state_prefix(self, buf):
+        super(ArrayColumn, self).write_state_prefix(buf)
+
         self.nested_column.write_state_prefix(buf)
 
     def _read(self, size, buf):
         slices_series = [[0, size]]
         nested_column = self.nested_column
 
         cur_level_slice_size = size
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/base.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,90 @@
 from struct import Struct, error as struct_error
 
 from . import exceptions
+from ..varint import read_varint
+
+
+class CommonSerialization(object):
+    def __init__(self, column):
+        self.column = column
+        super(CommonSerialization, self).__init__()
+
+    def read_sparse(self, n_items, buf):
+        return n_items
+
+    def apply_sparse(self, items):
+        return items
+
+
+class SparseSerialization(CommonSerialization):
+
+    def __init__(self, *args, **kwargs):
+        self.sparse_indexes = []
+        self.items_total = None
+        super(SparseSerialization, self).__init__(*args, **kwargs)
+
+    def read_sparse(self, n_items, buf):
+        sparse_indexes = []
+        items_total = 0
+        non_default_items = 0
+
+        END_OF_GRANULE_FLAG = 1 << 62
+        end_of_granule = False
+
+        while not end_of_granule:
+            group_size = read_varint(buf)
+            end_of_granule = group_size & END_OF_GRANULE_FLAG
+            group_size &= ~END_OF_GRANULE_FLAG
+
+            items_total += group_size + 1
+            if not end_of_granule:
+                non_default_items += 1
+                sparse_indexes.append(items_total)
+
+        self.sparse_indexes = sparse_indexes
+        self.items_total = items_total
+
+        return non_default_items
+
+    def apply_sparse(self, items):
+        default = self.column.null_value
+        if self.column.after_read_items:
+            default = self.column.after_read_items([default])[0]
+
+        rv = [default] * (self.items_total - 1)
+        for item_number, i in enumerate(self.sparse_indexes):
+            rv[i - 1] = items[item_number]
+
+        return rv
 
 
 class Column(object):
     ch_type = None
     py_types = None
 
     check_item = None
     after_read_items = None
     before_write_items = None
 
     types_check_enabled = False
 
     null_value = 0
 
-    def __init__(self, types_check=False, **kwargs):
+    def __init__(self, types_check=False, has_custom_serialization=False,
+                 **kwargs):
         self.nullable = False
         self.types_check_enabled = types_check
+        self.has_custom_serialization = has_custom_serialization
+        self.serialization = CommonSerialization(self)
         self.input_null_as_default = False
-        if 'context' in kwargs:
-            settings = kwargs['context'].client_settings
-            self.input_null_as_default = settings \
-                .get('input_format_null_as_default', False)
+
+        self.context = kwargs['context']
+        self.input_null_as_default = self.context.client_settings \
+            .get('input_format_null_as_default', False)
 
         super(Column, self).__init__()
 
     def make_null_struct(self, n_items):
         return Struct('<{}B'.format(n_items))
 
     def _read_nulls_map(self, n_items, buf):
@@ -90,20 +148,23 @@
         prepared = self.prepare_items(items)
         self.write_items(prepared, buf)
 
     def write_items(self, items, buf):
         raise NotImplementedError
 
     def read_data(self, n_items, buf):
+        n_items = self.serialization.read_sparse(n_items, buf)
+
         if self.nullable:
             nulls_map = self._read_nulls_map(n_items, buf)
         else:
             nulls_map = None
 
-        return self._read_data(n_items, buf, nulls_map=nulls_map)
+        items = self._read_data(n_items, buf, nulls_map=nulls_map)
+        return self.serialization.apply_sparse(items)
 
     def _read_data(self, n_items, buf, nulls_map=None):
         items = self.read_items(n_items, buf)
 
         if self.after_read_items:
             return self.after_read_items(items, nulls_map)
         elif nulls_map is not None:
@@ -113,15 +174,18 @@
             )
         return items
 
     def read_items(self, n_items, buf):
         raise NotImplementedError
 
     def read_state_prefix(self, buf):
-        pass
+        if self.has_custom_serialization:
+            use_custom_serialization = read_varint(buf)
+            if use_custom_serialization:
+                self.serialization = SparseSerialization(self)
 
     def write_state_prefix(self, buf):
         pass
 
 
 class FormatColumn(Column):
     """
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/datecolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/datecolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/datetimecolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/datetimecolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/decimalcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/decimalcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/enumcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/enumcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/floatcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/floatcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/intcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/intcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/intervalcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/intervalcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/ipcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/ipcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/largeint.c` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/largeint.c`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/largeint.pyx` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/largeint.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/lowcardinalitycolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/lowcardinalitycolumn.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,33 +31,40 @@
     # Need to update dictionary.
     # It means that previous granule has different dictionary.
     need_update_dictionary = 1 << 10
 
     serialization_type = has_additional_keys_bit | need_update_dictionary
 
     def __init__(self, nested_column, **kwargs):
+        self.init_kwargs = kwargs
         self.nested_column = nested_column
         super(LowCardinalityColumn, self).__init__(**kwargs)
 
     def read_state_prefix(self, buf):
-        return read_binary_uint64(buf)
+        super(LowCardinalityColumn, self).read_state_prefix(buf)
+
+        read_binary_uint64(buf)
 
     def write_state_prefix(self, buf):
+        super(LowCardinalityColumn, self).write_state_prefix(buf)
+
         # KeysSerializationVersion. See ClickHouse docs.
         write_binary_int64(1, buf)
 
     def _write_data(self, items, buf):
         index, keys = [], []
         key_by_index_element = {}
+        nested_is_nullable = False
 
         if self.nested_column.nullable:
             # First element represents NULL if column is nullable.
             index.append(self.nested_column.null_value)
             # Prevent null map writing. Reset nested column nullable flag.
             self.nested_column.nullable = False
+            nested_is_nullable = True
 
             for x in items:
                 if x is None:
                     # Zero element for null.
                     keys.append(0)
 
                 else:
@@ -83,34 +90,46 @@
 
         # Do not write anything for empty column.
         # May happen while writing empty arrays.
         if not len(index):
             return
 
         int_type = int(log(len(index), 2) / 8)
-        int_column = self.int_types[int_type]()
+        int_column = self.int_types[int_type](**self.init_kwargs)
 
         serialization_type = self.serialization_type | int_type
 
         write_binary_int64(serialization_type, buf)
         write_binary_int64(len(index), buf)
 
-        self.nested_column.write_data(index, buf)
+        if nested_is_nullable:
+            # Given we reset nested column nullable flag above,
+            # we need to write null map manually. If to invoke
+            # write_data method, it will cause an exception,
+            # because `prepare_data` may not be able to handle
+            # null value correctly.
+            self.nested_column.write_items(
+                [self.nested_column.null_value], buf)
+            # Remove null map from index, because it is already written.
+            index_to_write = index[1:]
+            self.nested_column.write_data(index_to_write, buf)
+        else:
+            self.nested_column.write_data(index, buf)
         write_binary_int64(len(items), buf)
         int_column.write_items(keys, buf)
 
     def _read_data(self, n_items, buf, nulls_map=None):
         if not n_items:
             return tuple()
 
         serialization_type = read_binary_uint64(buf)
 
         # Lowest byte contains info about key type.
         key_type = serialization_type & 0xf
-        keys_column = self.int_types[key_type]()
+        keys_column = self.int_types[key_type](**self.init_kwargs)
 
         nullable = self.nested_column.nullable
         # Prevent null map reading. Reset nested column nullable flag.
         self.nested_column.nullable = False
 
         index_size = read_binary_uint64(buf)
         index = self.nested_column.read_data(index_size, buf)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/mapcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/mapcolumn.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
 class MapColumn(Column):
     py_types = (dict, )
 
     null_value = {}
 
     def __init__(self, key_column, value_column, **kwargs):
-        self.offset_column = UInt64Column()
+        self.offset_column = UInt64Column(**kwargs)
         self.key_column = key_column
         self.value_column = value_column
         super(MapColumn, self).__init__(**kwargs)
 
     def read_state_prefix(self, buf):
+        super(MapColumn, self).read_state_prefix(buf)
+
         self.key_column.read_state_prefix(buf)
         self.value_column.read_state_prefix(buf)
 
     def write_state_prefix(self, buf):
+        super(MapColumn, self).write_state_prefix(buf)
+
         self.key_column.write_state_prefix(buf)
         self.value_column.write_state_prefix(buf)
 
     def read_items(self, n_items, buf):
         offsets = list(self.offset_column.read_items(n_items, buf))
         last_offset = offsets[-1]
         keys = self.key_column.read_data(last_offset, buf)
@@ -53,14 +57,14 @@
 
         self.offset_column.write_items(offsets, buf)
         self.key_column.write_data(keys, buf)
         self.value_column.write_data(values, buf)
 
 
 def create_map_column(spec, column_by_spec_getter, column_options):
-    # Match commas outside of parentheses so we don't match the comma in
+    # Match commas outside of parentheses, so we don't match the comma in
     # Decimal types.
     key, value = comma_re.split(spec[4:-1])
     key_column = column_by_spec_getter(key.strip())
     value_column = column_by_spec_getter(value.strip())
 
     return MapColumn(key_column, value_column, **column_options)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/base.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/datetimecolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/datetimecolumn.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         self.offset_naive = offset_naive
         self.local_timezone = local_timezone
         super(NumpyDateTimeColumnBase, self).__init__(**kwargs)
 
     def apply_timezones_after_read(self, dt):
         timezone = self.timezone if self.timezone else self.local_timezone
 
-        ts = pd.to_datetime(dt, utc=True).tz_convert(timezone)
-
-        if self.offset_naive:
+        if self.offset_naive and timezone.zone != 'UTC':
+            ts = pd.to_datetime(dt, utc=True).tz_convert(timezone)
             ts = ts.tz_localize(None)
+            return ts.to_numpy(self.datetime_dtype)
 
-        return ts.to_numpy(self.datetime_dtype)
+        return dt
 
     def apply_timezones_before_write(self, items):
         if isinstance(items, pd.DatetimeIndex):
             ts = items
         else:
             timezone = self.timezone if self.timezone else self.local_timezone
             ts = pd.to_datetime(items).tz_localize(timezone)
@@ -61,33 +61,33 @@
 
     def read_items(self, n_items, buf):
         items = super(NumpyDateTimeColumn, self).read_items(n_items, buf)
         return self.apply_timezones_after_read(items.astype('datetime64[s]'))
 
 
 class NumpyDateTime64Column(NumpyDateTimeColumnBase):
-    dtype = np.dtype(np.uint64)
+    dtype = np.dtype(np.int64)
     datetime_dtype = 'datetime64[ns]'
 
     max_scale = 9
 
     def __init__(self, scale=0, **kwargs):
         self.scale = scale
         super(NumpyDateTime64Column, self).__init__(**kwargs)
 
     def read_items(self, n_items, buf):
-        scale = 10 ** self.scale
-        frac_scale = 10 ** (self.max_scale - self.scale)
-
+        # Clickhouse:     t seconds is represented as t * 10^scale.
+        # datetime64[ns]: t seconds is represented as t * 10^9.
+        # Since 0 <= scale <= 9, multiply by the integer 10^(9 - scale).
         items = super(NumpyDateTime64Column, self).read_items(n_items, buf)
 
-        seconds = (items // scale).astype('datetime64[s]')
-        microseconds = ((items % scale) * frac_scale).astype('timedelta64[ns]')
+        tmp = np.copy(items)
+        tmp *= 10 ** (9 - self.scale)
+        dt = tmp.view(dtype='datetime64[ns]')
 
-        dt = seconds + microseconds
         return self.apply_timezones_after_read(dt)
 
     def write_items(self, items, buf):
         # write int 'as is'.
         if self.is_items_integer(items):
             super(NumpyDateTime64Column, self).write_items(items, buf)
             return
@@ -116,28 +116,28 @@
             spec = params[1].strip() + ')'
     else:
         cls = NumpyDateTimeColumn
         spec = spec[9:]
 
     context = column_options['context']
 
-    tz_name = timezone = None
+    tz_name = None
     offset_naive = True
 
     # As Numpy do not use local timezone for converting timestamp to
     # datetime we need always detect local timezone for manual converting.
-    local_timezone = get_localzone_name_compat()
+    local_tz_name = get_localzone_name_compat()
 
     # Use column's timezone if it's specified.
     if spec and spec[-1] == ')':
         tz_name = spec[1:-2]
         offset_naive = False
     else:
         if not context.settings.get('use_client_time_zone', False):
-            if local_timezone != context.server_info.timezone:
+            if local_tz_name != context.server_info.timezone:
                 tz_name = context.server_info.timezone
 
-    if tz_name:
-        timezone = get_timezone(tz_name)
+    timezone = get_timezone(tz_name) if tz_name else None
+    local_timezone = get_timezone(local_tz_name) if local_tz_name else None
 
     return cls(timezone=timezone, offset_naive=offset_naive,
                local_timezone=local_timezone, **column_options)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/floatcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/floatcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/intcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/intcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/lowcardinalitycolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/lowcardinalitycolumn.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if isinstance(items, np.ndarray) and not self.nested_column.nullable:
             nulls = pd.isnull(items)
             items = np.where(nulls, self.nested_column.null_value, items)
 
         c = pd.Categorical(items)
 
         int_type = int(log(len(c.codes), 2) / 8)
-        int_column = self.int_types[int_type]()
+        int_column = self.int_types[int_type](**self.init_kwargs)
 
         serialization_type = self.serialization_type | int_type
 
         index = c.categories
         keys = c.codes
 
         if self.nested_column.nullable:
@@ -62,15 +62,15 @@
         if not n_items:
             return tuple()
 
         serialization_type = read_binary_uint64(buf)
 
         # Lowest byte contains info about key type.
         key_type = serialization_type & 0xf
-        keys_column = self.int_types[key_type]()
+        keys_column = self.int_types[key_type](**self.init_kwargs)
 
         nullable = self.nested_column.nullable
         # Prevent null map reading. Reset nested column nullable flag.
         self.nested_column.nullable = False
 
         index_size = read_binary_uint64(buf)
         index = self.nested_column.read_data(index_size, buf)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/service.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/service.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/stringcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/stringcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/numpy/tuplecolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/numpy/tuplecolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/service.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .floatcolumn import Float32Column, Float64Column
 from .intcolumn import (
     Int8Column, Int16Column, Int32Column, Int64Column,
     Int128Column, UInt128Column, Int256Column, UInt256Column,
     UInt8Column, UInt16Column, UInt32Column, UInt64Column
 )
 from .lowcardinalitycolumn import create_low_cardinality_column
+from .jsoncolumn import create_json_column
 from .mapcolumn import create_map_column
 from .nothingcolumn import NothingColumn
 from .nullcolumn import NullColumn
 from .nullablecolumn import create_nullable_column
 from .simpleaggregatefunctioncolumn import (
     create_simple_aggregate_function_column
 )
@@ -118,14 +119,19 @@
         )
 
     elif spec.startswith('Map'):
         return create_map_column(
             spec, create_column_with_options, column_options
         )
 
+    elif spec.startswith("Object('json')"):
+        return create_json_column(
+            spec, create_column_with_options, column_options
+        )
+
     else:
         for alias, primitive in aliases:
             if spec.startswith(alias):
                 return create_column_with_options(
                     primitive + spec[len(alias):]
                 )
 
@@ -133,16 +139,20 @@
             cls = column_by_type[spec]
             return cls(**column_options)
 
         except KeyError:
             raise errors.UnknownTypeError('Unknown type {}'.format(spec))
 
 
-def read_column(context, column_spec, n_items, buf, use_numpy=None):
-    column_options = {'context': context}
+def read_column(context, column_spec, n_items, buf, use_numpy=None,
+                has_custom_serialization=False):
+    column_options = {
+        'context': context,
+        'has_custom_serialization': has_custom_serialization
+    }
     col = get_column_by_spec(column_spec, column_options, use_numpy=use_numpy)
     col.read_state_prefix(buf)
     return col.read_data(n_items, buf)
 
 
 def write_column(context, column_name, column_spec, items, buf,
                  types_check=False):
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/stringcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/stringcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/util.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/util.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/columns/uuidcolumn.py` & `clickhouse-driver-0.2.6/clickhouse_driver/columns/uuidcolumn.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/compression/__init__.py` & `clickhouse-driver-0.2.6/clickhouse_driver/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/compression/base.py` & `clickhouse-driver-0.2.6/clickhouse_driver/compression/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/compression/lz4.py` & `clickhouse-driver-0.2.6/clickhouse_driver/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/compression/zstd.py` & `clickhouse-driver-0.2.6/clickhouse_driver/compression/zstd.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/connection.py` & `clickhouse-driver-0.2.6/clickhouse_driver/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import socket
 import ssl
 from collections import deque
 from contextlib import contextmanager
+from sys import platform
 from time import time
 from urllib.parse import urlparse
 
 from . import defines
 from . import errors
 from .block import RowOrientedBlock
 from .blockstreamprofileinfo import BlockStreamProfileInfo
@@ -17,17 +18,18 @@
 from .context import Context
 from .log import log_block
 from .progress import Progress
 from .protocol import Compression, ClientPacketTypes, ServerPacketTypes
 from .queryprocessingstage import QueryProcessingStage
 from .reader import read_binary_str
 from .readhelpers import read_exception
-from .settings.writer import write_settings
+from .settings.writer import write_settings, SettingsFlags
 from .streams.native import BlockInputStream, BlockOutputStream
 from .util.compat import threading
+from .util.escape import escape_params
 from .varint import write_varint, read_varint
 from .writer import write_binary_str
 
 logger = logging.getLogger(__name__)
 
 
 class Packet(object):
@@ -40,36 +42,38 @@
         self.multistring_message = None
 
         super(Packet, self).__init__()
 
 
 class ServerInfo(object):
     def __init__(self, name, version_major, version_minor, version_patch,
-                 revision, timezone, display_name):
+                 revision, timezone, display_name, used_revision):
         self.name = name
         self.version_major = version_major
         self.version_minor = version_minor
         self.version_patch = version_patch
         self.revision = revision
         self.timezone = timezone
         self.display_name = display_name
+        self.used_revision = used_revision
 
         super(ServerInfo, self).__init__()
 
     def version_tuple(self):
         return self.version_major, self.version_minor, self.version_patch
 
     def __repr__(self):
         version = '%s.%s.%s' % (
             self.version_major, self.version_minor, self.version_patch
         )
         items = [
             ('name', self.name),
             ('version', version),
             ('revision', self.revision),
+            ('used revision', self.used_revision),
             ('timezone', self.timezone),
             ('display_name', self.display_name)
         ]
 
         params = ', '.join('{}={}'.format(key, value) for key, value in items)
         return '<ServerInfo(%s)>' % (params)
 
@@ -120,14 +124,23 @@
                             to correctly identify the desired server via SNI.
     :param alt_hosts: list of alternative hosts for connection.
                       Example: alt_hosts=host1:port1,host2:port2.
     :param settings_is_important: ``False`` means unknown settings will be
                                   ignored, ``True`` means that the query will
                                   fail with UNKNOWN_SETTING error.
                                   Defaults to ``False``.
+    :param tcp_keepalive: enables `TCP keepalive <https://tldp.org/HOWTO/
+                          TCP-Keepalive-HOWTO/overview.html>`_ on established
+                          connection. If is set to ``True``` system keepalive
+                          settings are used. You can also specify custom
+                          keepalive setting with tuple:
+                          ``(idle_time_sec, interval_sec, probes)``.
+                          Defaults to ``False``.
+    :param client_revision: can be used for client version downgrading.
+                          Defaults to ``None``.
     """
 
     def __init__(
             self, host, port=None,
             database=defines.DEFAULT_DATABASE,
             user=defines.DEFAULT_USER, password=defines.DEFAULT_PASSWORD,
             client_name=defines.CLIENT_NAME,
@@ -139,14 +152,16 @@
             secure=False,
             # Secure socket parameters.
             verify=True, ssl_version=None, ca_certs=None, ciphers=None,
             keyfile=None, certfile=None,
             server_hostname=None,
             alt_hosts=None,
             settings_is_important=False,
+            tcp_keepalive=False,
+            client_revision=None
     ):
         if secure:
             default_port = defines.DEFAULT_SECURE_PORT
         else:
             default_port = defines.DEFAULT_PORT
 
         self.hosts = deque([(host, port or default_port)])
@@ -160,14 +175,18 @@
         self.user = user
         self.password = password
         self.client_name = defines.DBMS_NAME + ' ' + client_name
         self.connect_timeout = connect_timeout
         self.send_receive_timeout = send_receive_timeout
         self.sync_request_timeout = sync_request_timeout
         self.settings_is_important = settings_is_important
+        self.tcp_keepalive = tcp_keepalive
+        self.client_revision = min(
+            client_revision or defines.CLIENT_REVISION, defines.CLIENT_REVISION
+        )
 
         self.secure_socket = secure
         self.verify_cert = verify
 
         ssl_options = {}
         if ssl_version is not None:
             ssl_options['ssl_version'] = ssl_version
@@ -306,25 +325,59 @@
         self.socket = self._create_socket(host, port)
         self.connected = True
         self.host, self.port = host, port
         self.socket.settimeout(self.send_receive_timeout)
 
         # performance tweak
         self.socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+        if self.tcp_keepalive:
+            self._set_keepalive()
 
         self.fin = BufferedSocketReader(self.socket, defines.BUFFER_SIZE)
         self.fout = BufferedSocketWriter(self.socket, defines.BUFFER_SIZE)
 
         self.send_hello()
         self.receive_hello()
 
+        revision = self.server_info.used_revision
+        if revision >= defines.DBMS_MIN_PROTOCOL_VERSION_WITH_ADDENDUM:
+            self.send_addendum()
+
         self.block_in = self.get_block_in_stream()
         self.block_in_raw = BlockInputStream(self.fin, self.context)
         self.block_out = self.get_block_out_stream()
 
+    def _set_keepalive(self):
+        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+
+        if not isinstance(self.tcp_keepalive, tuple):
+            return
+
+        idle_time_sec, interval_sec, probes = self.tcp_keepalive
+
+        if platform == 'linux' or platform == 'win32':
+            # This should also work for Windows
+            # starting with Windows 10, version 1709.
+            self.socket.setsockopt(
+                socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, idle_time_sec
+            )
+            self.socket.setsockopt(
+                socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, interval_sec
+            )
+            self.socket.setsockopt(
+                socket.IPPROTO_TCP, socket.TCP_KEEPCNT, probes
+            )
+
+        elif platform == 'darwin':
+            TCP_KEEPALIVE = 0x10
+            # Only interval is available in mac os.
+            self.socket.setsockopt(
+                socket.IPPROTO_TCP, TCP_KEEPALIVE, interval_sec
+            )
+
     def _format_connection_error(self, e, host, port):
         err = (e.strerror + ' ') if e.strerror else ''
         return err + '({}:{})'.format(host, port)
 
     def connect(self):
         if self.connected:
             self.disconnect()
@@ -406,15 +459,15 @@
     def send_hello(self):
         write_varint(ClientPacketTypes.HELLO, self.fout)
         write_binary_str(self.client_name, self.fout)
         write_varint(defines.CLIENT_VERSION_MAJOR, self.fout)
         write_varint(defines.CLIENT_VERSION_MINOR, self.fout)
         # NOTE For backward compatibility of the protocol,
         # client cannot send its version_patch.
-        write_varint(defines.CLIENT_REVISION, self.fout)
+        write_varint(self.client_revision, self.fout)
         write_binary_str(self.database, self.fout)
         write_binary_str(self.user, self.fout)
         write_binary_str(self.password, self.fout)
 
         self.fout.flush()
 
     def receive_hello(self):
@@ -422,33 +475,35 @@
 
         if packet_type == ServerPacketTypes.HELLO:
             server_name = read_binary_str(self.fin)
             server_version_major = read_varint(self.fin)
             server_version_minor = read_varint(self.fin)
             server_revision = read_varint(self.fin)
 
+            used_revision = min(self.client_revision, server_revision)
+
             server_timezone = None
-            if server_revision >= \
+            if used_revision >= \
                     defines.DBMS_MIN_REVISION_WITH_SERVER_TIMEZONE:
                 server_timezone = read_binary_str(self.fin)
 
             server_display_name = ''
-            if server_revision >= \
+            if used_revision >= \
                     defines.DBMS_MIN_REVISION_WITH_SERVER_DISPLAY_NAME:
                 server_display_name = read_binary_str(self.fin)
 
             server_version_patch = server_revision
-            if server_revision >= \
+            if used_revision >= \
                     defines.DBMS_MIN_REVISION_WITH_VERSION_PATCH:
                 server_version_patch = read_varint(self.fin)
 
             self.server_info = ServerInfo(
                 server_name, server_version_major, server_version_minor,
                 server_version_patch, server_revision,
-                server_timezone, server_display_name
+                server_timezone, server_display_name, used_revision
             )
             self.context.server_info = self.server_info
 
             logger.debug(
                 'Connected to %s server version %s.%s.%s, revision: %s',
                 server_name, server_version_major, server_version_minor,
                 server_version_patch, server_revision
@@ -459,14 +514,22 @@
 
         else:
             message = self.unexpected_packet_message('Hello or Exception',
                                                      packet_type)
             self.disconnect()
             raise errors.UnexpectedPacketFromServerError(message)
 
+    def send_addendum(self):
+        revision = self.server_info.used_revision
+
+        if revision >= defines.DBMS_MIN_PROTOCOL_VERSION_WITH_QUOTA_KEY:
+            write_binary_str(
+                self.context.client_settings['quota_key'], self.fout
+            )
+
     def ping(self):
         timeout = self.sync_request_timeout
 
         with self.timeout_setter(timeout):
             try:
                 write_varint(ClientPacketTypes.PING, self.fout)
                 self.fout.flush()
@@ -563,29 +626,29 @@
                 self.compressor_cls, self.compress_block_size,
                 self.fout, self.context
             )
         else:
             return BlockOutputStream(self.fout, self.context)
 
     def receive_data(self, may_be_compressed=True, may_be_use_numpy=False):
-        revision = self.server_info.revision
+        revision = self.server_info.used_revision
 
         if revision >= defines.DBMS_MIN_REVISION_WITH_TEMPORARY_TABLES:
             read_binary_str(self.fin)
 
         reader = self.block_in if may_be_compressed else self.block_in_raw
         use_numpy = False if not may_be_use_numpy else None
         return reader.read(use_numpy=use_numpy)
 
     def receive_exception(self):
         return read_exception(self.fin)
 
     def receive_progress(self):
         progress = Progress()
-        progress.read(self.server_info.revision, self.fin)
+        progress.read(self.server_info, self.fin)
         return progress
 
     def receive_profile_info(self):
         profile_info = BlockStreamProfileInfo()
         profile_info.read(self.fin)
         return profile_info
 
@@ -593,51 +656,62 @@
         num = ServerPacketTypes.strings_in_message(packet_type)
         return [read_binary_str(self.fin) for _i in range(num)]
 
     def send_data(self, block, table_name=''):
         start = time()
         write_varint(ClientPacketTypes.DATA, self.fout)
 
-        revision = self.server_info.revision
+        revision = self.server_info.used_revision
         if revision >= defines.DBMS_MIN_REVISION_WITH_TEMPORARY_TABLES:
             write_binary_str(table_name, self.fout)
 
         self.block_out.write(block)
         logger.debug('Block "%s" send time: %f', table_name, time() - start)
 
-    def send_query(self, query, query_id=None):
+    def send_query(self, query, query_id=None, params=None):
         if not self.connected:
             self.connect()
 
         write_varint(ClientPacketTypes.QUERY, self.fout)
 
         write_binary_str(query_id or '', self.fout)
 
-        revision = self.server_info.revision
+        revision = self.server_info.used_revision
         if revision >= defines.DBMS_MIN_REVISION_WITH_CLIENT_INFO:
-            client_info = ClientInfo(self.client_name, self.context)
+            client_info = ClientInfo(self.client_name, self.context,
+                                     client_revision=self.client_revision)
             client_info.query_kind = ClientInfo.QueryKind.INITIAL_QUERY
 
             client_info.write(revision, self.fout)
 
         settings_as_strings = (
             revision >= defines
             .DBMS_MIN_REVISION_WITH_SETTINGS_SERIALIZED_AS_STRINGS
         )
+        settings_flags = 0
+        if self.settings_is_important:
+            settings_flags |= SettingsFlags.IMPORTANT
         write_settings(self.context.settings, self.fout, settings_as_strings,
-                       self.settings_is_important)
+                       settings_flags)
 
         if revision >= defines.DBMS_MIN_REVISION_WITH_INTERSERVER_SECRET:
             write_binary_str('', self.fout)
 
         write_varint(QueryProcessingStage.COMPLETE, self.fout)
         write_varint(self.compression, self.fout)
 
         write_binary_str(query, self.fout)
 
+        if revision >= defines.DBMS_MIN_PROTOCOL_VERSION_WITH_PARAMETERS:
+            # Always settings_as_strings = True
+            escaped = escape_params(
+                params or {}, self.context, for_server=True
+            )
+            write_settings(escaped, self.fout, True, SettingsFlags.CUSTOM)
+
         logger.debug('Query: %s', query)
 
         self.fout.flush()
 
     def send_cancel(self):
         write_varint(ClientPacketTypes.CANCEL, self.fout)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/context.py` & `clickhouse-driver-0.2.6/clickhouse_driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/dbapi/__init__.py` & `clickhouse-driver-0.2.6/clickhouse_driver/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/dbapi/connection.py` & `clickhouse-driver-0.2.6/clickhouse_driver/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/dbapi/cursor.py` & `clickhouse-driver-0.2.6/clickhouse_driver/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/dbapi/extras.py` & `clickhouse-driver-0.2.6/clickhouse_driver/dbapi/extras.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/defines.py` & `clickhouse-driver-0.2.6/clickhouse_driver/defines.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 DBMS_MIN_REVISION_WITH_SETTINGS_SERIALIZED_AS_STRINGS = 54429
 DBMS_MIN_REVISION_WITH_INTERSERVER_SECRET = 54441
 DBMS_MIN_REVISION_WITH_OPENTELEMETRY = 54442
 DBMS_MIN_PROTOCOL_VERSION_WITH_DISTRIBUTED_DEPTH = 54448
 DBMS_MIN_PROTOCOL_VERSION_WITH_INITIAL_QUERY_START_TIME = 54449
 DBMS_MIN_PROTOCOL_VERSION_WITH_INCREMENTAL_PROFILE_EVENTS = 54451
 DBMS_MIN_REVISION_WITH_PARALLEL_REPLICAS = 54453
+DBMS_MIN_REVISION_WITH_CUSTOM_SERIALIZATION = 54454
+DBMS_MIN_PROTOCOL_VERSION_WITH_ADDENDUM = 54458
+DBMS_MIN_PROTOCOL_VERSION_WITH_QUOTA_KEY = 54458
+DBMS_MIN_PROTOCOL_VERSION_WITH_PARAMETERS = 54459
 
 # Timeouts
 DBMS_DEFAULT_CONNECT_TIMEOUT_SEC = 10
 DBMS_DEFAULT_TIMEOUT_SEC = 300
 
 DBMS_DEFAULT_SYNC_REQUEST_TIMEOUT_SEC = 5
 
@@ -36,12 +40,12 @@
 DEFAULT_INSERT_BLOCK_SIZE = 1048576
 
 DBMS_NAME = 'ClickHouse'
 CLIENT_NAME = 'python-driver'
 CLIENT_VERSION_MAJOR = 20
 CLIENT_VERSION_MINOR = 10
 CLIENT_VERSION_PATCH = 2
-CLIENT_REVISION = 54453
+CLIENT_REVISION = DBMS_MIN_PROTOCOL_VERSION_WITH_PARAMETERS
 
 BUFFER_SIZE = 1048576
 
 STRINGS_ENCODING = 'utf-8'
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/errors.py` & `clickhouse-driver-0.2.6/clickhouse_driver/errors.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/log.py` & `clickhouse-driver-0.2.6/clickhouse_driver/log.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/numpy/helpers.py` & `clickhouse-driver-0.2.6/clickhouse_driver/numpy/helpers.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/numpy/result.py` & `clickhouse-driver-0.2.6/clickhouse_driver/numpy/result.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/opentelemetry.py` & `clickhouse-driver-0.2.6/clickhouse_driver/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/progress.py` & `clickhouse-driver-0.2.6/clickhouse_driver/progress.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,19 @@
         self.bytes = 0
         self.total_rows = 0
         self.written_rows = 0
         self.written_bytes = 0
 
         super(Progress, self).__init__()
 
-    def read(self, server_revision, fin):
+    def read(self, server_info, fin):
         self.rows = read_varint(fin)
         self.bytes = read_varint(fin)
 
-        revision = server_revision
+        revision = server_info.used_revision
         if revision >= defines.DBMS_MIN_REVISION_WITH_TOTAL_ROWS_IN_PROGRESS:
             self.total_rows = read_varint(fin)
 
         if revision >= defines.DBMS_MIN_REVISION_WITH_CLIENT_WRITE_INFO:
             self.written_rows = read_varint(fin)
             self.written_bytes = read_varint(fin)
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/protocol.py` & `clickhouse-driver-0.2.6/clickhouse_driver/protocol.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/reader.py` & `clickhouse-driver-0.2.6/clickhouse_driver/reader.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/readhelpers.py` & `clickhouse-driver-0.2.6/clickhouse_driver/readhelpers.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/result.py` & `clickhouse-driver-0.2.6/clickhouse_driver/result.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/settings/available.py` & `clickhouse-driver-0.2.6/clickhouse_driver/settings/available.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/settings/types.py` & `clickhouse-driver-0.2.6/clickhouse_driver/settings/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/settings/writer.py` & `clickhouse-driver-0.2.6/clickhouse_driver/settings/writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 from ..writer import write_binary_str, write_binary_uint8
 from .available import settings as available_settings
 
 
 logger = logging.getLogger(__name__)
 
 
-def write_settings(settings, buf, settings_as_strings, is_important=False):
+class SettingsFlags:
+    IMPORTANT = 0x1
+    CUSTOM = 0x2
+
+
+def write_settings(settings, buf, settings_as_strings, flags):
     for setting, value in (settings or {}).items():
         # If the server support settings as string we do not need to know
         # anything about them, so we can write any setting.
         if settings_as_strings:
             write_binary_str(setting, buf)
-            write_binary_uint8(int(is_important), buf)
+            write_binary_uint8(flags, buf)
             write_binary_str(str(value), buf)
 
         else:
             # If the server requires string in binary,
             # then they cannot be written without type.
             setting_writer = available_settings.get(setting)
             if not setting_writer:
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/streams/compressed.py` & `clickhouse-driver-0.2.6/clickhouse_driver/streams/compressed.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/streams/native.py` & `clickhouse-driver-0.2.6/clickhouse_driver/streams/native.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from ..block import ColumnOrientedBlock, BlockInfo
 from ..columns.service import read_column, write_column
-from ..reader import read_binary_str
+from ..reader import read_binary_str, read_binary_uint8
 from ..varint import write_varint, read_varint
-from ..writer import write_binary_str
+from ..writer import write_binary_str, write_binary_uint8
 from .. import defines
 
 
 class BlockOutputStream(object):
     def __init__(self, fout, context):
         self.fout = fout
         self.context = context
 
         super(BlockOutputStream, self).__init__()
 
     def write(self, block):
-        revision = self.context.server_info.revision
+        revision = self.context.server_info.used_revision
         if revision >= defines.DBMS_MIN_REVISION_WITH_BLOCK_INFO:
             block.info.write(self.fout)
 
         # We write transposed data.
         n_columns = block.num_columns
         n_rows = block.num_rows
 
@@ -31,14 +31,19 @@
 
             if n_columns:
                 try:
                     items = block.get_column_by_index(i)
                 except IndexError:
                     raise ValueError('Different rows length')
 
+                if revision >= \
+                        defines.DBMS_MIN_REVISION_WITH_CUSTOM_SERIALIZATION:
+                    # We write always sparse data without custom serialization.
+                    write_binary_uint8(0, self.fout)
+
                 write_column(self.context, col_name, col_type, items,
                              self.fout, types_check=block.types_check)
 
         self.finalize()
 
     def finalize(self):
         self.fout.flush()
@@ -50,15 +55,15 @@
         self.context = context
 
         super(BlockInputStream, self).__init__()
 
     def read(self, use_numpy=None):
         info = BlockInfo()
 
-        revision = self.context.server_info.revision
+        revision = self.context.server_info.used_revision
         if revision >= defines.DBMS_MIN_REVISION_WITH_BLOCK_INFO:
             info.read(self.fin)
 
         n_columns = read_varint(self.fin)
         n_rows = read_varint(self.fin)
 
         data, names, types = [], [], []
@@ -66,17 +71,24 @@
         for i in range(n_columns):
             column_name = read_binary_str(self.fin)
             column_type = read_binary_str(self.fin)
 
             names.append(column_name)
             types.append(column_type)
 
+            has_custom_serialization = False
+            if revision >= defines.DBMS_MIN_REVISION_WITH_CUSTOM_SERIALIZATION:
+                has_custom_serialization = bool(read_binary_uint8(self.fin))
+
             if n_rows:
-                column = read_column(self.context, column_type, n_rows,
-                                     self.fin, use_numpy=use_numpy)
+                column = read_column(
+                    self.context, column_type, n_rows,
+                    self.fin, use_numpy=use_numpy,
+                    has_custom_serialization=has_custom_serialization
+                )
                 data.append(column)
 
         if self.context.client_settings['use_numpy']:
             from ..numpy.block import NumpyColumnOrientedBlock
             block_cls = NumpyColumnOrientedBlock
         else:
             block_cls = ColumnOrientedBlock
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/util/helpers.py` & `clickhouse-driver-0.2.6/clickhouse_driver/util/helpers.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/varint.c` & `clickhouse-driver-0.2.6/clickhouse_driver/varint.c`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/varint.pyx` & `clickhouse-driver-0.2.6/clickhouse_driver/varint.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver/writer.py` & `clickhouse-driver-0.2.6/clickhouse_driver/writer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver.egg-info/PKG-INFO` & `clickhouse-driver-0.2.6/clickhouse_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-driver
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python driver with native interface for ClickHouse
 Home-page: https://github.com/mymarilyn/clickhouse-driver
 Author: Konstantin Lebedev
 Author-email: kostyan.lebedev@gmail.com
 License: MIT
 Project-URL: Documentation, https://clickhouse-driver.readthedocs.io
 Project-URL: Changes, https://github.com/mymarilyn/clickhouse-driver/blob/master/CHANGELOG.md
@@ -170,24 +170,23 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: lz4
 Provides-Extra: zstd
 Provides-Extra: numpy
```

### Comparing `clickhouse-driver-0.2.5/clickhouse_driver.egg-info/SOURCES.txt` & `clickhouse-driver-0.2.6/clickhouse_driver.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 clickhouse_driver/columns/decimalcolumn.py
 clickhouse_driver/columns/enumcolumn.py
 clickhouse_driver/columns/exceptions.py
 clickhouse_driver/columns/floatcolumn.py
 clickhouse_driver/columns/intcolumn.py
 clickhouse_driver/columns/intervalcolumn.py
 clickhouse_driver/columns/ipcolumn.py
+clickhouse_driver/columns/jsoncolumn.py
 clickhouse_driver/columns/largeint.c
 clickhouse_driver/columns/largeint.pyx
 clickhouse_driver/columns/lowcardinalitycolumn.py
 clickhouse_driver/columns/mapcolumn.py
 clickhouse_driver/columns/nestedcolumn.py
 clickhouse_driver/columns/nothingcolumn.py
 clickhouse_driver/columns/nullablecolumn.py
```

### Comparing `clickhouse-driver-0.2.5/setup.py` & `clickhouse-driver-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
 
         'Operating System :: OS Independent',
 
 
         'Programming Language :: SQL',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: PyPy',
 
@@ -116,15 +115,15 @@
     keywords='ClickHouse db database cloud analytics',
 
     project_urls={
         'Documentation': 'https://clickhouse-driver.readthedocs.io',
         'Changes': github_url + '/blob/master/CHANGELOG.md'
     },
     packages=find_packages('.', exclude=['tests*']),
-    python_requires='>=3.6, <4',
+    python_requires='>=3.7, <4',
     install_requires=[
         'pytz',
         'tzlocal'
     ],
     ext_modules=extensions,
     extras_require={
         'lz4': [
```

