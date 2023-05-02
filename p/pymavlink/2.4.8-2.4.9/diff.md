# Comparing `tmp/pymavlink-2.4.8.tar.gz` & `tmp/pymavlink-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymavlink-2.4.8.tar", last modified: Tue Apr 21 23:56:13 2020, max compression
+gzip compressed data, was "dist/pymavlink-2.4.9.tar", last modified: Sat Jun 20 04:59:55 2020, max compression
```

## Comparing `pymavlink-2.4.8.tar` & `pymavlink-2.4.9.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6525 2019-09-16 00:38:26.000000 pymavlink-2.4.8/mavparm.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/message_definitions/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/message_definitions/v1.0/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-02-01 01:38:33.000000 pymavlink-2.4.8/message_definitions/v1.0/uAvionix.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2017-03-27 22:53:42.000000 pymavlink-2.4.8/message_definitions/v1.0/standard.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2017-03-27 22:53:42.000000 pymavlink-2.4.8/message_definitions/v1.0/python_array_test.xml
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2019-11-10 19:48:58.000000 pymavlink-2.4.8/message_definitions/v1.0/slugs.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2017-03-27 22:53:42.000000 pymavlink-2.4.8/message_definitions/v1.0/ualberta.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2018-05-07 12:08:45.000000 pymavlink-2.4.8/message_definitions/v1.0/icarous.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2019-11-10 19:48:58.000000 pymavlink-2.4.8/message_definitions/v1.0/matrixpilot.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2019-11-10 19:48:58.000000 pymavlink-2.4.8/message_definitions/v1.0/ASLUAV.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    93796 2020-03-28 01:45:48.000000 pymavlink-2.4.8/message_definitions/v1.0/ardupilotmega.xml
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2017-03-27 22:53:42.000000 pymavlink-2.4.8/message_definitions/v1.0/paparazzi.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2017-03-27 22:53:42.000000 pymavlink-2.4.8/message_definitions/v1.0/test.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-02-01 01:38:33.000000 pymavlink-2.4.8/message_definitions/v1.0/minimal.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-04-21 23:51:16.000000 pymavlink-2.4.8/message_definitions/v1.0/common.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2019-11-10 19:48:58.000000 pymavlink-2.4.8/message_definitions/v1.0/autoquad.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)       79 2019-09-16 00:38:25.000000 pymavlink-2.4.8/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    23139 2019-09-16 00:38:26.000000 pymavlink-2.4.8/mavwp.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     7606 2020-04-21 23:50:12.000000 pymavlink-2.4.8/setup.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/dialects/
--rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.8/dialects/__init__.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/dialects/v10/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1099789 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/ASLUAV.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/uAvionix.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/standard.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/python_array_test.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    90864 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/minimal.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    37411 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/uAvionix.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/slugs.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/ualberta.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1026906 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/ualberta.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.8/dialects/v10/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/icarous.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/matrixpilot.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1027599 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/paparazzi.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/ASLUAV.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1014813 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/common.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    93796 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/ardupilotmega.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1161890 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/matrixpilot.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1283214 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/ardupilotmega.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/paparazzi.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1036189 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/python_array_test.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/test.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    28580 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/icarous.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/minimal.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    34771 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/test.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1035835 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v10/autoquad.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1014828 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/standard.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/common.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1088125 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/slugs.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v10/autoquad.xml
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/dialects/v20/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1268840 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/ASLUAV.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/uAvionix.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/standard.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/python_array_test.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    96531 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/minimal.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    54480 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v20/uAvionix.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/slugs.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/ualberta.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1195957 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/ualberta.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.8/dialects/v20/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/icarous.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/matrixpilot.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1196650 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/paparazzi.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/ASLUAV.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1183864 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/common.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    93796 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/ardupilotmega.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1330941 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/matrixpilot.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1524906 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/ardupilotmega.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/paparazzi.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1205240 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v20/python_array_test.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/test.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    37386 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/icarous.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/minimal.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    34771 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/test.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1204886 2020-04-21 23:56:13.000000 pymavlink-2.4.8/dialects/v20/autoquad.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1183879 2020-04-21 23:56:11.000000 pymavlink-2.4.8/dialects/v20/standard.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/common.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  1257176 2020-04-21 23:56:12.000000 pymavlink-2.4.8/dialects/v20/slugs.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2020-04-21 23:56:10.000000 pymavlink-2.4.8/dialects/v20/autoquad.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    60815 2020-04-05 23:01:28.000000 pymavlink-2.4.8/mavextra.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     3210 2020-02-19 08:16:12.000000 pymavlink-2.4.8/README.md
--rw-r--r--   0 tridge    (1000) tridge    (1000)    93172 2020-04-21 23:49:05.000000 pymavlink-2.4.8/mavutil.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)      909 2019-09-16 00:38:26.000000 pymavlink-2.4.8/mavexpression.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/mavnative/
--rw-r--r--   0 tridge    (1000) tridge    (1000)      438 2019-09-16 00:38:26.000000 pymavlink-2.4.8/mavnative/mavlink_defaults.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)    31450 2019-09-16 00:38:26.000000 pymavlink-2.4.8/mavnative/mavnative.c
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       20 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/top_level.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       12 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/requires.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/dependency_links.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4529 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/SOURCES.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1007 2020-04-21 23:56:13.000000 pymavlink-2.4.8/pymavlink.egg-info/PKG-INFO
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    16337 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavgen_wlua.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    19551 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavgen_java.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    15028 2019-11-29 11:38:47.000000 pymavlink-2.4.8/generator/mavgen_swift.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    11955 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavgen_cs.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4079 2020-03-28 01:45:38.000000 pymavlink-2.4.8/generator/mavgen_lua.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    22849 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavparse.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    25104 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/mavgen_c.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13299 2020-03-28 01:45:38.000000 pymavlink-2.4.8/generator/mavschema.xsd
--rw-r--r--   0 tridge    (1000) tridge    (1000)       31 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/__init__.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3607 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavtestgen.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    10585 2020-04-21 23:56:06.000000 pymavlink-2.4.8/generator/mavgen.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13575 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavgen_objc.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12742 2019-12-18 00:01:06.000000 pymavlink-2.4.8/generator/mavgen_cpp11.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/C/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/C/include_v2.0/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2245 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v2.0/mavlink_get_info.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)    36552 2019-09-26 23:55:54.000000 pymavlink-2.4.8/generator/C/include_v2.0/mavlink_helpers.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12255 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v2.0/protocol.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6421 2020-03-28 01:45:38.000000 pymavlink-2.4.8/generator/C/include_v2.0/mavlink_conversions.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)    11336 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v2.0/mavlink_types.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     7026 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v2.0/mavlink_sha256.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2253 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v2.0/checksum.h
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/C/include_v1.0/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    21292 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v1.0/mavlink_helpers.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12673 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v1.0/protocol.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6477 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v1.0/mavlink_conversions.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     8535 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v1.0/mavlink_types.h
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2198 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/C/include_v1.0/checksum.h
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/java/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/java/lib/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     3965 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/java/lib/Parser.java
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/java/lib/Messages/
--rw-r--r--   0 tridge    (1000) tridge    (1000)      823 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkMessage.java
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4625 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkStats.java
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5905 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkPayload.java
--rw-r--r--   0 tridge    (1000) tridge    (1000)    22184 2020-01-17 06:00:07.000000 pymavlink-2.4.8/generator/mavgen_javascript.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5626 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavtemplate.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    37825 2020-01-17 06:00:07.000000 pymavlink-2.4.8/generator/mavgen_python.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/CS/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/CS/common/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    15301 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/CS/common/Mavlink.cs
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6927 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/CS/common/ByteArrayUtil.cs
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6004 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/CS/common/FrameworkBitConverter.cs
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/swift/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    43759 2019-11-29 11:38:47.000000 pymavlink-2.4.8/generator/swift/MAVLink.swift
--rw-r--r--   0 tridge    (1000) tridge    (1000)      930 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/mavcrc.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5693 2019-09-16 00:38:26.000000 pymavlink-2.4.8/generator/mavgen_typescript.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/CPP11/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/generator/CPP11/include_v2.0/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     3055 2019-09-16 00:38:25.000000 pymavlink-2.4.8/generator/CPP11/include_v2.0/message.hpp
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5772 2019-12-06 01:13:08.000000 pymavlink-2.4.8/generator/CPP11/include_v2.0/msgmap.hpp
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2020-04-21 23:56:13.000000 pymavlink-2.4.8/tools/
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2773 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavflightmodes.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2743 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavflighttime.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6660 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavsummarize.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3129 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavtomfile.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4512 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/magfit_delta.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3081 2020-03-28 01:45:38.000000 pymavlink-2.4.8/tools/mavmission.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    10266 2020-04-21 23:49:05.000000 pymavlink-2.4.8/tools/mavfft_isb.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13470 2019-11-29 11:38:47.000000 pymavlink-2.4.8/tools/mavlogdump.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13903 2020-03-28 01:45:32.000000 pymavlink-2.4.8/tools/magfit_WMM.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2202 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavloss.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1768 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavgen.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)      938 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavlink_bitmask_decoder.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     7096 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavkml.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3914 2019-10-08 03:28:05.000000 pymavlink-2.4.8/tools/mavextract.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)      947 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavparmdiff.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     5024 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/magfit.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1417 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavparms.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2087 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavgpslock.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2490 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavfft.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2873 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavtogpx.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4800 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/magfit_motors.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1956 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavsigloss.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    11728 2020-04-21 23:49:05.000000 pymavlink-2.4.8/tools/mavgraph.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     8746 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavplayback.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4960 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/magfit_gps.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1180 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/mavsearch.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     6439 2019-09-16 00:38:26.000000 pymavlink-2.4.8/tools/MPU6KSearch.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    42275 2020-04-21 23:49:05.000000 pymavlink-2.4.8/DFReader.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)       38 2020-04-21 23:56:13.000000 pymavlink-2.4.8/setup.cfg
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18869 2019-09-16 00:38:26.000000 pymavlink-2.4.8/quaternion.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1007 2020-04-21 23:56:13.000000 pymavlink-2.4.8/PKG-INFO
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13183 2019-11-29 11:38:47.000000 pymavlink-2.4.8/rotmat.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     9809 2019-09-16 00:38:25.000000 pymavlink-2.4.8/fgFDM.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6525 2019-09-16 00:38:26.000000 pymavlink-2.4.9/mavparm.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/message_definitions/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/message_definitions/v1.0/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-02-01 01:38:33.000000 pymavlink-2.4.9/message_definitions/v1.0/uAvionix.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2017-03-27 22:53:42.000000 pymavlink-2.4.9/message_definitions/v1.0/standard.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2017-03-27 22:53:42.000000 pymavlink-2.4.9/message_definitions/v1.0/python_array_test.xml
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2019-11-10 19:48:58.000000 pymavlink-2.4.9/message_definitions/v1.0/slugs.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2017-03-27 22:53:42.000000 pymavlink-2.4.9/message_definitions/v1.0/ualberta.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2018-05-07 12:08:45.000000 pymavlink-2.4.9/message_definitions/v1.0/icarous.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2019-11-10 19:48:58.000000 pymavlink-2.4.9/message_definitions/v1.0/matrixpilot.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2019-11-10 19:48:58.000000 pymavlink-2.4.9/message_definitions/v1.0/ASLUAV.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    98159 2020-06-16 04:25:34.000000 pymavlink-2.4.9/message_definitions/v1.0/ardupilotmega.xml
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2017-03-27 22:53:42.000000 pymavlink-2.4.9/message_definitions/v1.0/paparazzi.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2017-03-27 22:53:42.000000 pymavlink-2.4.9/message_definitions/v1.0/test.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-02-01 01:38:33.000000 pymavlink-2.4.9/message_definitions/v1.0/minimal.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-04-21 23:51:16.000000 pymavlink-2.4.9/message_definitions/v1.0/common.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2019-11-10 19:48:58.000000 pymavlink-2.4.9/message_definitions/v1.0/autoquad.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       79 2019-09-16 00:38:25.000000 pymavlink-2.4.9/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    23139 2019-09-16 00:38:26.000000 pymavlink-2.4.9/mavwp.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     7606 2020-06-20 04:58:26.000000 pymavlink-2.4.9/setup.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.9/dialects/__init__.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v10/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1099789 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/ASLUAV.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/uAvionix.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/standard.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/python_array_test.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    90864 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/minimal.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    37411 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/uAvionix.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/slugs.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/ualberta.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1026906 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/ualberta.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.9/dialects/v10/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/icarous.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/matrixpilot.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1027599 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/paparazzi.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/ASLUAV.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1014813 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/common.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    98159 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/ardupilotmega.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1161890 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/matrixpilot.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1287917 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/ardupilotmega.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/paparazzi.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1036189 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/python_array_test.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/test.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    28580 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/icarous.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/minimal.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    34771 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/test.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1035835 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v10/autoquad.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1014828 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/standard.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/common.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1088125 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/slugs.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v10/autoquad.xml
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1268840 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/ASLUAV.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     9296 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/uAvionix.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      227 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/standard.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3300 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/python_array_test.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    96531 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/minimal.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    54480 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v20/uAvionix.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    19234 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/slugs.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3395 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/ualberta.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1195957 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/ualberta.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)        0 2019-09-16 00:38:25.000000 pymavlink-2.4.9/dialects/v20/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/icarous.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    27240 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/matrixpilot.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1196650 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/paparazzi.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18813 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/ASLUAV.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1183864 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/common.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    98159 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/ardupilotmega.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1330941 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/matrixpilot.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1529609 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/ardupilotmega.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     2076 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/paparazzi.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1205240 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/python_array_test.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1557 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/test.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    37386 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/icarous.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    42430 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/minimal.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    34771 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/test.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1204886 2020-06-20 04:59:55.000000 pymavlink-2.4.9/dialects/v20/autoquad.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1183879 2020-06-20 04:59:53.000000 pymavlink-2.4.9/dialects/v20/standard.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)   402759 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/common.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  1257176 2020-06-20 04:59:54.000000 pymavlink-2.4.9/dialects/v20/slugs.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     8764 2020-06-20 04:59:52.000000 pymavlink-2.4.9/dialects/v20/autoquad.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    60815 2020-04-05 23:01:28.000000 pymavlink-2.4.9/mavextra.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3358 2020-06-16 04:25:41.000000 pymavlink-2.4.9/README.md
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    93156 2020-06-20 04:58:19.000000 pymavlink-2.4.9/mavutil.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      909 2019-09-16 00:38:26.000000 pymavlink-2.4.9/mavexpression.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/mavnative/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      438 2019-09-16 00:38:26.000000 pymavlink-2.4.9/mavnative/mavlink_defaults.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    31450 2019-09-16 00:38:26.000000 pymavlink-2.4.9/mavnative/mavnative.c
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       20 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/top_level.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       12 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/requires.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4529 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1007 2020-06-20 04:59:55.000000 pymavlink-2.4.9/pymavlink.egg-info/PKG-INFO
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    16337 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavgen_wlua.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    19551 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavgen_java.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    15028 2019-11-29 11:38:47.000000 pymavlink-2.4.9/generator/mavgen_swift.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    11955 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavgen_cs.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4079 2020-03-28 01:45:38.000000 pymavlink-2.4.9/generator/mavgen_lua.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    22885 2020-05-12 11:13:24.000000 pymavlink-2.4.9/generator/mavparse.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    25313 2020-05-11 00:12:06.000000 pymavlink-2.4.9/generator/mavgen_c.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    13493 2020-05-11 00:12:06.000000 pymavlink-2.4.9/generator/mavschema.xsd
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       31 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/__init__.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3607 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavtestgen.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)    10635 2020-05-11 00:12:06.000000 pymavlink-2.4.9/generator/mavgen.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    13575 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavgen_objc.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12742 2019-12-18 00:01:06.000000 pymavlink-2.4.9/generator/mavgen_cpp11.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/C/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/C/include_v2.0/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2245 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v2.0/mavlink_get_info.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    36552 2019-09-26 23:55:54.000000 pymavlink-2.4.9/generator/C/include_v2.0/mavlink_helpers.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12255 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v2.0/protocol.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6421 2020-03-28 01:45:38.000000 pymavlink-2.4.9/generator/C/include_v2.0/mavlink_conversions.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    11336 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v2.0/mavlink_types.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     7026 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v2.0/mavlink_sha256.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2253 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v2.0/checksum.h
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/C/include_v1.0/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    21292 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v1.0/mavlink_helpers.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12673 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v1.0/protocol.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6477 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v1.0/mavlink_conversions.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     8535 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v1.0/mavlink_types.h
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2198 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/C/include_v1.0/checksum.h
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/java/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/java/lib/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     3965 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/java/lib/Parser.java
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/java/lib/Messages/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      823 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkMessage.java
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4625 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkStats.java
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5905 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkPayload.java
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    22184 2020-01-17 06:00:07.000000 pymavlink-2.4.9/generator/mavgen_javascript.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5626 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavtemplate.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    37825 2020-01-17 06:00:07.000000 pymavlink-2.4.9/generator/mavgen_python.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/CS/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/CS/common/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    15301 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/CS/common/Mavlink.cs
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6927 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/CS/common/ByteArrayUtil.cs
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6004 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/CS/common/FrameworkBitConverter.cs
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/swift/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    43759 2019-11-29 11:38:47.000000 pymavlink-2.4.9/generator/swift/MAVLink.swift
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      930 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/mavcrc.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5693 2019-09-16 00:38:26.000000 pymavlink-2.4.9/generator/mavgen_typescript.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/CPP11/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/generator/CPP11/include_v2.0/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     3055 2019-09-16 00:38:25.000000 pymavlink-2.4.9/generator/CPP11/include_v2.0/message.hpp
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5772 2019-12-06 01:13:08.000000 pymavlink-2.4.9/generator/CPP11/include_v2.0/msgmap.hpp
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2020-06-20 04:59:55.000000 pymavlink-2.4.9/tools/
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2773 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavflightmodes.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2743 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavflighttime.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6660 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavsummarize.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3129 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavtomfile.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4512 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/magfit_delta.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3081 2020-03-28 01:45:38.000000 pymavlink-2.4.9/tools/mavmission.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    10266 2020-04-21 23:49:05.000000 pymavlink-2.4.9/tools/mavfft_isb.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13470 2019-11-29 11:38:47.000000 pymavlink-2.4.9/tools/mavlogdump.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)    14090 2020-06-20 04:58:19.000000 pymavlink-2.4.9/tools/magfit_WMM.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2202 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavloss.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1768 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavgen.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)      938 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavlink_bitmask_decoder.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     7096 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavkml.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3914 2019-10-08 03:28:05.000000 pymavlink-2.4.9/tools/mavextract.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)      947 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavparmdiff.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     5024 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/magfit.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1417 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavparms.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2087 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavgpslock.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2490 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavfft.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     2873 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavtogpx.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4800 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/magfit_motors.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1956 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavsigloss.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    11728 2020-04-21 23:49:05.000000 pymavlink-2.4.9/tools/mavgraph.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     8746 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavplayback.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4960 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/magfit_gps.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1180 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/mavsearch.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     6439 2019-09-16 00:38:26.000000 pymavlink-2.4.9/tools/MPU6KSearch.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    42275 2020-04-21 23:49:05.000000 pymavlink-2.4.9/DFReader.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       38 2020-06-20 04:59:55.000000 pymavlink-2.4.9/setup.cfg
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18869 2019-09-16 00:38:26.000000 pymavlink-2.4.9/quaternion.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1007 2020-06-20 04:59:55.000000 pymavlink-2.4.9/PKG-INFO
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13183 2019-11-29 11:38:47.000000 pymavlink-2.4.9/rotmat.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     9809 2019-09-16 00:38:25.000000 pymavlink-2.4.9/fgFDM.py
```

### Comparing `pymavlink-2.4.8/mavparm.py` & `pymavlink-2.4.9/mavparm.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/uAvionix.xml` & `pymavlink-2.4.9/message_definitions/v1.0/uAvionix.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/python_array_test.xml` & `pymavlink-2.4.9/message_definitions/v1.0/python_array_test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/slugs.xml` & `pymavlink-2.4.9/message_definitions/v1.0/slugs.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/ualberta.xml` & `pymavlink-2.4.9/message_definitions/v1.0/ualberta.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/icarous.xml` & `pymavlink-2.4.9/message_definitions/v1.0/icarous.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/matrixpilot.xml` & `pymavlink-2.4.9/message_definitions/v1.0/matrixpilot.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/ASLUAV.xml` & `pymavlink-2.4.9/message_definitions/v1.0/ASLUAV.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/ardupilotmega.xml` & `pymavlink-2.4.9/message_definitions/v1.0/ardupilotmega.xml`

 * *Files 3% similar despite different names*

#### Comparing `pymavlink-2.4.8/message_definitions/v1.0/ardupilotmega.xml` & `pymavlink-2.4.9/message_definitions/v1.0/ardupilotmega.xml`

```diff
@@ -13,29 +13,37 @@
       <entry value="3" name="ACCELCAL_VEHICLE_POS_RIGHT"/>
       <entry value="4" name="ACCELCAL_VEHICLE_POS_NOSEDOWN"/>
       <entry value="5" name="ACCELCAL_VEHICLE_POS_NOSEUP"/>
       <entry value="6" name="ACCELCAL_VEHICLE_POS_BACK"/>
       <entry value="16777215" name="ACCELCAL_VEHICLE_POS_SUCCESS"/>
       <entry value="16777216" name="ACCELCAL_VEHICLE_POS_FAILED"/>
     </enum>
+    <enum name="HEADING_TYPE">
+      <entry value="0" name="HEADING_TYPE_COURSE_OVER_GROUND"/>
+      <entry value="1" name="HEADING_TYPE_HEADING"/>
+    </enum>
+    <enum name="SPEED_TYPE">
+      <entry value="0" name="SPEED_TYPE_AIRSPEED"/>
+      <entry value="1" name="SPEED_TYPE_GROUNDSPEED"/>
+    </enum>
     <!-- ardupilot specific MAV_CMD_* commands -->
     <enum name="MAV_CMD">
-      <entry value="211" name="MAV_CMD_DO_GRIPPER">
+      <entry value="211" name="MAV_CMD_DO_GRIPPER" hasLocation="false" isDestination="false">
         <description>Mission command to operate EPM gripper.</description>
-        <param index="1">Gripper number (a number from 1 to max number of grippers on the vehicle).</param>
-        <param index="2">Gripper action (0=release, 1=grab. See GRIPPER_ACTIONS enum).</param>
+        <param index="1" label="Instance" minValue="1" increment="1">Gripper instance number (from 1 to max number of grippers on the vehicle).</param>
+        <param index="2" label="Action" enum="GRIPPER_ACTIONS">Gripper action.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE">
+      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE" hasLocation="false" isDestination="false">
         <description>Enable/disable autotune.</description>
-        <param index="1">Enable (1: enable, 0:disable).</param>
+        <param index="1" label="Enable" minValue="0" maxValue="1" increment="1">Enable (1: enable, 0:disable).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
@@ -45,81 +53,81 @@
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT">
+      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT" hasLocation="false" isDestination="false">
         <description>Mission command to wait for an altitude or downwards vertical speed. This is meant for high altitude balloon launches, allowing the aircraft to be idle until either an altitude is reached or a negative vertical speed is reached (indicating early balloon burst). The wiggle time is how often to wiggle the control surfaces to prevent them seizing up.</description>
-        <param index="1">Altitude (m).</param>
-        <param index="2">Descent speed (m/s).</param>
-        <param index="3">Wiggle Time (s).</param>
+        <param index="1" label="Altitude" units="m">Altitude.</param>
+        <param index="2" label="Descent Speed" units="m/s">Descent speed.</param>
+        <param index="3" label="Wiggle Time" units="s">How long to wiggle the control surfaces to prevent them seizing up.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED">
+      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED" hasLocation="false" isDestination="false">
         <description>A system wide power-off event has been initiated.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <!-- MAV_CMD_SOLO_BTN_* are here to provide vendor-specific support for 3DR Solo until a better solution is found to atomically make multiple commands with control flow -->
-      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK">
+      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK" hasLocation="false" isDestination="false">
         <description>FLY button has been clicked.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD">
+      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD" hasLocation="false" isDestination="false">
         <description>FLY button has been held for 1.5 seconds.</description>
-        <param index="1">Takeoff altitude.</param>
+        <param index="1" label="Takeoff Altitude" units="m">Takeoff altitude.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK">
+      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK" hasLocation="false" isDestination="false">
         <description>PAUSE button has been clicked.</description>
-        <param index="1">1 if Solo is in a shot mode, 0 otherwise.</param>
+        <param index="1" label="Shot Mode" minValue="0" maxValue="1" increment="1">1 if Solo is in a shot mode, 0 otherwise.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL">
+      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Magnetometer calibration based on fixed position
         in earth field given by inclination, declination and intensity.</description>
-        <param index="1">MagDeclinationDegrees.</param>
-        <param index="2">MagInclinationDegrees.</param>
-        <param index="3">MagIntensityMilliGauss.</param>
-        <param index="4">YawDegrees.</param>
+        <param index="1" label="Declination" units="deg">Magnetic declination.</param>
+        <param index="2" label="Inclination" units="deg">Magnetic inclination.</param>
+        <param index="3" label="Intensity" units="mgauss">Magnetic intensity.</param>
+        <param index="4" label="Yaw" units="deg">Yaw.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD">
-        <description>Magnetometer calibration based on fixed expected field values in milliGauss.</description>
-        <param index="1">FieldX.</param>
-        <param index="2">FieldY.</param>
-        <param index="3">FieldZ.</param>
+      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD" hasLocation="false" isDestination="false">
+        <description>Magnetometer calibration based on fixed expected field values.</description>
+        <param index="1" label="Field X" units="mgauss">Field strength X.</param>
+        <param index="2" label="Field Y" units="mgauss">Field strength Y.</param>
+        <param index="3" label="Field Z" units="mgauss">Field strength Z.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42006" name="MAV_CMD_FIXED_MAG_CAL_YAW">
         <description>Magnetometer calibration based on provided known yaw. This allows for fast calibration using WMM field tables in the vehicle, given only the known yaw of the vehicle. If Latitude and longitude are both zero then use the current vehicle location.</description>
@@ -127,131 +135,131 @@
         <param index="2" label="CompassMask">CompassMask, 0 for all.</param>
         <param index="3" label="Lattitude" units="deg">Latitude.</param>
         <param index="4" label="Longitude" units="deg">Longitude.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL">
+      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
-        <param index="2">Automatically retry on failure (0=no retry, 1=retry).</param>
-        <param index="3">Save without user input (0=require input, 1=autosave).</param>
-        <param index="4">Delay (seconds).</param>
-        <param index="5">Autoreboot (0=user reboot, 1=autoreboot).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to calibrate. Use 0 to calibrate all sensors that can be started (sensors may not start if disabled, unhealthy, etc.). The command will NACK if calibration does not start for a sensor explicitly specified by the bitmask.</param>
+        <param index="2" label="Retry on Failure" minValue="0" maxValue="1" increment="1">Automatically retry on failure (0=no retry, 1=retry).</param>
+        <param index="3" label="Autosave" minValue="0" maxValue="1" increment="1">Save without user input (0=require input, 1=autosave).</param>
+        <param index="4" label="Delay" units="s">Delay.</param>
+        <param index="5" label="Autoreboot" minValue="0" maxValue="1" increment="1">Autoreboot (0=user reboot, 1=autoreboot).</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL">
-        <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL" hasLocation="false" isDestination="false">
+        <description>Accept a magnetometer calibration.</description>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers that calibration is accepted (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL">
+      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Cancel a running magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to cancel a running calibration (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS">
+      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS" hasLocation="false" isDestination="false">
         <description>Used when doing accelerometer calibration. When sent to the GCS tells it what position to put the vehicle in. When sent to the vehicle says what position the vehicle is in.</description>
-        <param index="1">Position, one of the ACCELCAL_VEHICLE_POS enum values.</param>
+        <param index="1" label="Position" enum="ACCELCAL_VEHICLE_POS">Position.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER">
+      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER" hasLocation="false" isDestination="false">
         <description>Reply with the version banner.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE">
+      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE" hasLocation="false" isDestination="false">
         <description>Command autopilot to get into factory test/diagnostic mode.</description>
-        <param index="1">0 means get out of test mode, 1 means get into test mode.</param>
+        <param index="1" label="Test Mode" minValue="0" maxValue="1" increment="1">0: activate test mode, 1: exit test mode.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42501" name="MAV_CMD_GIMBAL_RESET">
+      <entry value="42501" name="MAV_CMD_GIMBAL_RESET" hasLocation="false" isDestination="false">
         <description>Causes the gimbal to reset and boot as if it was just powered on.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS">
+      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS" hasLocation="false" isDestination="false">
         <description>Reports progress and success or failure of gimbal axis calibration procedure.</description>
-        <param index="1">Gimbal axis we're reporting calibration progress for.</param>
-        <param index="2">Current calibration progress for this axis, 0x64=100%.</param>
-        <param index="3">Status of the calibration.</param>
+        <param index="1" label="Axis" enum="GIMBAL_AXIS">Gimbal axis we're reporting calibration progress for.</param>
+        <param index="2" label="Progress" units="%" minValue="0" maxValue="100">Current calibration progress for this axis.</param>
+        <param index="3" label="Status" enum="GIMBAL_AXIS_CALIBRATION_STATUS">Status of the calibration.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION">
+      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION" hasLocation="false" isDestination="false">
         <description>Starts commutation calibration on the gimbal.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET">
+      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET" hasLocation="false" isDestination="false">
         <description>Erases gimbal application and parameters.</description>
         <param index="1">Magic number.</param>
         <param index="2">Magic number.</param>
         <param index="3">Magic number.</param>
         <param index="4">Magic number.</param>
         <param index="5">Magic number.</param>
         <param index="6">Magic number.</param>
         <param index="7">Magic number.</param>
       </entry>
-      <entry value="42600" name="MAV_CMD_DO_WINCH">
+      <entry value="42600" name="MAV_CMD_DO_WINCH" hasLocation="false" isDestination="false">
         <description>Command to operate winch.</description>
-        <param index="1">Winch number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
-        <param index="2">Action (0=relax, 1=relative length control, 2=rate control. See WINCH_ACTIONS enum.).</param>
-        <param index="3">Release length (cable distance to unwind in meters, negative numbers to wind in cable).</param>
-        <param index="4">Release rate (meters/second).</param>
+        <param index="1" label="Instance" minValue="0" increment="1">Winch instance number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
+        <param index="2" label="Action" enum="WINCH_ACTIONS">Action.</param>
+        <param index="3" label="Length" units="m">Release length (cable distance to unwind, negative numbers to wind in cable).</param>
+        <param index="4" label="Rate" units="m/s">Release rate.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER">
+      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER" hasLocation="false" isDestination="false">
         <description>Update the bootloader</description>
         <param index="1">Empty</param>
         <param index="2">Empty</param>
         <param index="3">Empty</param>
         <param index="4">Empty</param>
-        <param index="5">Magic number - set to 290876 to actually flash</param>
+        <param index="5" label="Magic Number" increment="1">Magic number - set to 290876 to actually flash</param>
         <param index="6">Empty</param>
         <param index="7">Empty</param>
       </entry>
       <entry value="42651" name="MAV_CMD_BATTERY_RESET" hasLocation="false" isDestination="false">
         <description>Reset battery capacity for batteries that accumulate consumed battery via integration.</description>
         <param index="1" label="battery mask">Bitmask of batteries to reset. Least significant bit is for the first battery.</param>
         <param index="2" label="percentage" minValue="0" maxValue="100" increment="1">Battery percentage remaining to set.</param>
@@ -266,14 +274,44 @@
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42701" name="MAV_CMD_SCRIPTING">
         <description>Control onboard scripting.</description>
         <param index="1" enum="SCRIPTING_CMD">Scripting command to execute</param>
       </entry>
+      <entry value="43000" name="MAV_CMD_GUIDED_CHANGE_SPEED">
+        <description>Change flight speed at a given rate. This slews the vehicle at a controllable rate between it's previous speed and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="speed type" enum="SPEED_TYPE">Airspeed or groundspeed.</param>
+        <param index="2" label="speed target" units="m/s">Target Speed</param>
+        <param index="3" label="speed rate-of-change" units="m/s/s">Acceleration rate, 0 to take effect instantly</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
+      <entry value="43001" name="MAV_CMD_GUIDED_CHANGE_ALTITUDE">
+        <description>Change target altitude at a given rate. This slews the vehicle at a controllable rate between it's previous altitude and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1">Empty</param>
+        <param index="2">Empty</param>
+        <param index="3" label="alt rate-of-change" units="m/s/s" minValue="0">Rate of change, toward new altitude. 0 for maximum rate change. Positive numbers only, as negative numbers will not converge on the new target alt.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7" label="target alt" units="m">Target Altitude</param>
+      </entry>
+      <entry value="43002" name="MAV_CMD_GUIDED_CHANGE_HEADING">
+        <description>Change to target heading at a given rate, overriding previous heading/s. This slews the vehicle at a controllable rate between it's previous heading and the new one. (affects GUIDED only. Exiting GUIDED returns aircraft to normal behaviour defined elsewhere. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="heading type" enum="HEADING_TYPE">course-over-ground or raw vehicle heading.</param>
+        <param index="2" label="heading target" units="deg" minValue="0" maxValue="359.99">Target heading.</param>
+        <param index="3" label="heading rate-of-change" units="m/s/s">Maximum centripetal accelearation, ie rate of change,  toward new heading.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
     </enum>
     <enum name="SCRIPTING_CMD">
       <entry value="0" name="SCRIPTING_CMD_REPL_START">
         <description>Start a REPL session.</description>
       </entry>
       <entry value="1" name="SCRIPTING_CMD_REPL_STOP">
         <description>End a REPL session.</description>
@@ -1291,15 +1329,14 @@
       <field type="uint16_t" name="throttle" units="d%">Throttle.</field>
       <field type="float" name="current" units="A">Current.</field>
       <field type="uint16_t" name="interference" units="%">Interference.</field>
       <field type="float" name="CompensationX">Motor Compensation X.</field>
       <field type="float" name="CompensationY">Motor Compensation Y.</field>
       <field type="float" name="CompensationZ">Motor Compensation Z.</field>
     </message>
-    <!-- Coming soon <message name="RALLY_LAND_POINT" id="177"> <description>A rally landing point. An aircraft loitering at a rally point may choose one of these points to land at.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> <field name="count" type="uint8_t">Total number of points (for sanity checking).</field> <field name="lat" type="int32_t">Latitude of point.</field> <field name="lng" type="int32_t">Longitude of point.</field> <field name="alt" type="uint16_t">Ground AGL (usually 0).</field> </message> <message name="RALLY_LAND_FETCH_POINT" id="178"> <description>Request a current rally land point from MAV.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> </message> -->
     <message id="178" name="AHRS2">
       <description>Status of secondary AHRS filter if available.</description>
       <field type="float" name="roll" units="rad">Roll angle.</field>
       <field type="float" name="pitch" units="rad">Pitch angle.</field>
       <field type="float" name="yaw" units="rad">Yaw angle.</field>
       <field type="float" name="altitude" units="m">Altitude (MSL).</field>
       <field type="int32_t" name="lat" units="degE7">Latitude.</field>
@@ -1444,16 +1481,16 @@
       <extensions/>
       <field type="float" name="airspeed_variance">Airspeed variance.</field>
     </message>
     <!-- realtime PID tuning message -->
     <message id="194" name="PID_TUNING">
       <description>PID tuning information.</description>
       <field type="uint8_t" name="axis" enum="PID_TUNING_AXIS">Axis.</field>
-      <field type="float" name="desired" units="deg/s">Desired rate.</field>
-      <field type="float" name="achieved" units="deg/s">Achieved rate.</field>
+      <field type="float" name="desired">Desired rate.</field>
+      <field type="float" name="achieved">Achieved rate.</field>
       <field type="float" name="FF">FF component.</field>
       <field type="float" name="P">P component.</field>
       <field type="float" name="I">I component.</field>
       <field type="float" name="D">D component.</field>
     </message>
     <message id="195" name="DEEPSTALL">
       <description>Deepstall path planning.</description>
```

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/paparazzi.xml` & `pymavlink-2.4.9/message_definitions/v1.0/paparazzi.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/test.xml` & `pymavlink-2.4.9/message_definitions/v1.0/test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/minimal.xml` & `pymavlink-2.4.9/message_definitions/v1.0/minimal.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/common.xml` & `pymavlink-2.4.9/message_definitions/v1.0/common.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/message_definitions/v1.0/autoquad.xml` & `pymavlink-2.4.9/message_definitions/v1.0/autoquad.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/mavwp.py` & `pymavlink-2.4.9/mavwp.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/setup.py` & `pymavlink-2.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ascii = codecs.lookup('ascii')
     func = lambda name, enc=ascii: {True: enc}.get(name=='mbcs')
     codecs.register(func)
 
 from setuptools import setup, Extension
 import glob, os, shutil, fnmatch, platform, sys
 
-version = '2.4.8'
+version = '2.4.9'
 
 
 def generate_content():
     # generate the file content...
     from generator import mavgen, mavparse
 
     # path to message_definitions directory
```

### Comparing `pymavlink-2.4.8/dialects/v10/ASLUAV.py` & `pymavlink-2.4.9/dialects/v10/ASLUAV.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/uAvionix.xml` & `pymavlink-2.4.9/dialects/v10/uAvionix.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/python_array_test.xml` & `pymavlink-2.4.9/dialects/v10/python_array_test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/minimal.py` & `pymavlink-2.4.9/dialects/v10/minimal.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/uAvionix.py` & `pymavlink-2.4.9/dialects/v10/uAvionix.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/slugs.xml` & `pymavlink-2.4.9/dialects/v10/slugs.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/ualberta.xml` & `pymavlink-2.4.9/dialects/v10/ualberta.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/ualberta.py` & `pymavlink-2.4.9/dialects/v10/ualberta.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/icarous.xml` & `pymavlink-2.4.9/dialects/v10/icarous.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/matrixpilot.xml` & `pymavlink-2.4.9/dialects/v10/matrixpilot.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/paparazzi.py` & `pymavlink-2.4.9/dialects/v10/paparazzi.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/ASLUAV.xml` & `pymavlink-2.4.9/dialects/v10/ASLUAV.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/common.py` & `pymavlink-2.4.9/dialects/v10/common.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/ardupilotmega.xml` & `pymavlink-2.4.9/dialects/v10/ardupilotmega.xml`

 * *Files 3% similar despite different names*

#### Comparing `pymavlink-2.4.8/dialects/v10/ardupilotmega.xml` & `pymavlink-2.4.9/dialects/v10/ardupilotmega.xml`

```diff
@@ -13,29 +13,37 @@
       <entry value="3" name="ACCELCAL_VEHICLE_POS_RIGHT"/>
       <entry value="4" name="ACCELCAL_VEHICLE_POS_NOSEDOWN"/>
       <entry value="5" name="ACCELCAL_VEHICLE_POS_NOSEUP"/>
       <entry value="6" name="ACCELCAL_VEHICLE_POS_BACK"/>
       <entry value="16777215" name="ACCELCAL_VEHICLE_POS_SUCCESS"/>
       <entry value="16777216" name="ACCELCAL_VEHICLE_POS_FAILED"/>
     </enum>
+    <enum name="HEADING_TYPE">
+      <entry value="0" name="HEADING_TYPE_COURSE_OVER_GROUND"/>
+      <entry value="1" name="HEADING_TYPE_HEADING"/>
+    </enum>
+    <enum name="SPEED_TYPE">
+      <entry value="0" name="SPEED_TYPE_AIRSPEED"/>
+      <entry value="1" name="SPEED_TYPE_GROUNDSPEED"/>
+    </enum>
     <!-- ardupilot specific MAV_CMD_* commands -->
     <enum name="MAV_CMD">
-      <entry value="211" name="MAV_CMD_DO_GRIPPER">
+      <entry value="211" name="MAV_CMD_DO_GRIPPER" hasLocation="false" isDestination="false">
         <description>Mission command to operate EPM gripper.</description>
-        <param index="1">Gripper number (a number from 1 to max number of grippers on the vehicle).</param>
-        <param index="2">Gripper action (0=release, 1=grab. See GRIPPER_ACTIONS enum).</param>
+        <param index="1" label="Instance" minValue="1" increment="1">Gripper instance number (from 1 to max number of grippers on the vehicle).</param>
+        <param index="2" label="Action" enum="GRIPPER_ACTIONS">Gripper action.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE">
+      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE" hasLocation="false" isDestination="false">
         <description>Enable/disable autotune.</description>
-        <param index="1">Enable (1: enable, 0:disable).</param>
+        <param index="1" label="Enable" minValue="0" maxValue="1" increment="1">Enable (1: enable, 0:disable).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
@@ -45,81 +53,81 @@
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT">
+      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT" hasLocation="false" isDestination="false">
         <description>Mission command to wait for an altitude or downwards vertical speed. This is meant for high altitude balloon launches, allowing the aircraft to be idle until either an altitude is reached or a negative vertical speed is reached (indicating early balloon burst). The wiggle time is how often to wiggle the control surfaces to prevent them seizing up.</description>
-        <param index="1">Altitude (m).</param>
-        <param index="2">Descent speed (m/s).</param>
-        <param index="3">Wiggle Time (s).</param>
+        <param index="1" label="Altitude" units="m">Altitude.</param>
+        <param index="2" label="Descent Speed" units="m/s">Descent speed.</param>
+        <param index="3" label="Wiggle Time" units="s">How long to wiggle the control surfaces to prevent them seizing up.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED">
+      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED" hasLocation="false" isDestination="false">
         <description>A system wide power-off event has been initiated.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <!-- MAV_CMD_SOLO_BTN_* are here to provide vendor-specific support for 3DR Solo until a better solution is found to atomically make multiple commands with control flow -->
-      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK">
+      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK" hasLocation="false" isDestination="false">
         <description>FLY button has been clicked.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD">
+      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD" hasLocation="false" isDestination="false">
         <description>FLY button has been held for 1.5 seconds.</description>
-        <param index="1">Takeoff altitude.</param>
+        <param index="1" label="Takeoff Altitude" units="m">Takeoff altitude.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK">
+      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK" hasLocation="false" isDestination="false">
         <description>PAUSE button has been clicked.</description>
-        <param index="1">1 if Solo is in a shot mode, 0 otherwise.</param>
+        <param index="1" label="Shot Mode" minValue="0" maxValue="1" increment="1">1 if Solo is in a shot mode, 0 otherwise.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL">
+      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Magnetometer calibration based on fixed position
         in earth field given by inclination, declination and intensity.</description>
-        <param index="1">MagDeclinationDegrees.</param>
-        <param index="2">MagInclinationDegrees.</param>
-        <param index="3">MagIntensityMilliGauss.</param>
-        <param index="4">YawDegrees.</param>
+        <param index="1" label="Declination" units="deg">Magnetic declination.</param>
+        <param index="2" label="Inclination" units="deg">Magnetic inclination.</param>
+        <param index="3" label="Intensity" units="mgauss">Magnetic intensity.</param>
+        <param index="4" label="Yaw" units="deg">Yaw.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD">
-        <description>Magnetometer calibration based on fixed expected field values in milliGauss.</description>
-        <param index="1">FieldX.</param>
-        <param index="2">FieldY.</param>
-        <param index="3">FieldZ.</param>
+      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD" hasLocation="false" isDestination="false">
+        <description>Magnetometer calibration based on fixed expected field values.</description>
+        <param index="1" label="Field X" units="mgauss">Field strength X.</param>
+        <param index="2" label="Field Y" units="mgauss">Field strength Y.</param>
+        <param index="3" label="Field Z" units="mgauss">Field strength Z.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42006" name="MAV_CMD_FIXED_MAG_CAL_YAW">
         <description>Magnetometer calibration based on provided known yaw. This allows for fast calibration using WMM field tables in the vehicle, given only the known yaw of the vehicle. If Latitude and longitude are both zero then use the current vehicle location.</description>
@@ -127,131 +135,131 @@
         <param index="2" label="CompassMask">CompassMask, 0 for all.</param>
         <param index="3" label="Lattitude" units="deg">Latitude.</param>
         <param index="4" label="Longitude" units="deg">Longitude.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL">
+      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
-        <param index="2">Automatically retry on failure (0=no retry, 1=retry).</param>
-        <param index="3">Save without user input (0=require input, 1=autosave).</param>
-        <param index="4">Delay (seconds).</param>
-        <param index="5">Autoreboot (0=user reboot, 1=autoreboot).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to calibrate. Use 0 to calibrate all sensors that can be started (sensors may not start if disabled, unhealthy, etc.). The command will NACK if calibration does not start for a sensor explicitly specified by the bitmask.</param>
+        <param index="2" label="Retry on Failure" minValue="0" maxValue="1" increment="1">Automatically retry on failure (0=no retry, 1=retry).</param>
+        <param index="3" label="Autosave" minValue="0" maxValue="1" increment="1">Save without user input (0=require input, 1=autosave).</param>
+        <param index="4" label="Delay" units="s">Delay.</param>
+        <param index="5" label="Autoreboot" minValue="0" maxValue="1" increment="1">Autoreboot (0=user reboot, 1=autoreboot).</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL">
-        <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL" hasLocation="false" isDestination="false">
+        <description>Accept a magnetometer calibration.</description>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers that calibration is accepted (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL">
+      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Cancel a running magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to cancel a running calibration (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS">
+      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS" hasLocation="false" isDestination="false">
         <description>Used when doing accelerometer calibration. When sent to the GCS tells it what position to put the vehicle in. When sent to the vehicle says what position the vehicle is in.</description>
-        <param index="1">Position, one of the ACCELCAL_VEHICLE_POS enum values.</param>
+        <param index="1" label="Position" enum="ACCELCAL_VEHICLE_POS">Position.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER">
+      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER" hasLocation="false" isDestination="false">
         <description>Reply with the version banner.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE">
+      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE" hasLocation="false" isDestination="false">
         <description>Command autopilot to get into factory test/diagnostic mode.</description>
-        <param index="1">0 means get out of test mode, 1 means get into test mode.</param>
+        <param index="1" label="Test Mode" minValue="0" maxValue="1" increment="1">0: activate test mode, 1: exit test mode.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42501" name="MAV_CMD_GIMBAL_RESET">
+      <entry value="42501" name="MAV_CMD_GIMBAL_RESET" hasLocation="false" isDestination="false">
         <description>Causes the gimbal to reset and boot as if it was just powered on.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS">
+      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS" hasLocation="false" isDestination="false">
         <description>Reports progress and success or failure of gimbal axis calibration procedure.</description>
-        <param index="1">Gimbal axis we're reporting calibration progress for.</param>
-        <param index="2">Current calibration progress for this axis, 0x64=100%.</param>
-        <param index="3">Status of the calibration.</param>
+        <param index="1" label="Axis" enum="GIMBAL_AXIS">Gimbal axis we're reporting calibration progress for.</param>
+        <param index="2" label="Progress" units="%" minValue="0" maxValue="100">Current calibration progress for this axis.</param>
+        <param index="3" label="Status" enum="GIMBAL_AXIS_CALIBRATION_STATUS">Status of the calibration.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION">
+      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION" hasLocation="false" isDestination="false">
         <description>Starts commutation calibration on the gimbal.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET">
+      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET" hasLocation="false" isDestination="false">
         <description>Erases gimbal application and parameters.</description>
         <param index="1">Magic number.</param>
         <param index="2">Magic number.</param>
         <param index="3">Magic number.</param>
         <param index="4">Magic number.</param>
         <param index="5">Magic number.</param>
         <param index="6">Magic number.</param>
         <param index="7">Magic number.</param>
       </entry>
-      <entry value="42600" name="MAV_CMD_DO_WINCH">
+      <entry value="42600" name="MAV_CMD_DO_WINCH" hasLocation="false" isDestination="false">
         <description>Command to operate winch.</description>
-        <param index="1">Winch number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
-        <param index="2">Action (0=relax, 1=relative length control, 2=rate control. See WINCH_ACTIONS enum.).</param>
-        <param index="3">Release length (cable distance to unwind in meters, negative numbers to wind in cable).</param>
-        <param index="4">Release rate (meters/second).</param>
+        <param index="1" label="Instance" minValue="0" increment="1">Winch instance number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
+        <param index="2" label="Action" enum="WINCH_ACTIONS">Action.</param>
+        <param index="3" label="Length" units="m">Release length (cable distance to unwind, negative numbers to wind in cable).</param>
+        <param index="4" label="Rate" units="m/s">Release rate.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER">
+      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER" hasLocation="false" isDestination="false">
         <description>Update the bootloader</description>
         <param index="1">Empty</param>
         <param index="2">Empty</param>
         <param index="3">Empty</param>
         <param index="4">Empty</param>
-        <param index="5">Magic number - set to 290876 to actually flash</param>
+        <param index="5" label="Magic Number" increment="1">Magic number - set to 290876 to actually flash</param>
         <param index="6">Empty</param>
         <param index="7">Empty</param>
       </entry>
       <entry value="42651" name="MAV_CMD_BATTERY_RESET" hasLocation="false" isDestination="false">
         <description>Reset battery capacity for batteries that accumulate consumed battery via integration.</description>
         <param index="1" label="battery mask">Bitmask of batteries to reset. Least significant bit is for the first battery.</param>
         <param index="2" label="percentage" minValue="0" maxValue="100" increment="1">Battery percentage remaining to set.</param>
@@ -266,14 +274,44 @@
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42701" name="MAV_CMD_SCRIPTING">
         <description>Control onboard scripting.</description>
         <param index="1" enum="SCRIPTING_CMD">Scripting command to execute</param>
       </entry>
+      <entry value="43000" name="MAV_CMD_GUIDED_CHANGE_SPEED">
+        <description>Change flight speed at a given rate. This slews the vehicle at a controllable rate between it's previous speed and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="speed type" enum="SPEED_TYPE">Airspeed or groundspeed.</param>
+        <param index="2" label="speed target" units="m/s">Target Speed</param>
+        <param index="3" label="speed rate-of-change" units="m/s/s">Acceleration rate, 0 to take effect instantly</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
+      <entry value="43001" name="MAV_CMD_GUIDED_CHANGE_ALTITUDE">
+        <description>Change target altitude at a given rate. This slews the vehicle at a controllable rate between it's previous altitude and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1">Empty</param>
+        <param index="2">Empty</param>
+        <param index="3" label="alt rate-of-change" units="m/s/s" minValue="0">Rate of change, toward new altitude. 0 for maximum rate change. Positive numbers only, as negative numbers will not converge on the new target alt.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7" label="target alt" units="m">Target Altitude</param>
+      </entry>
+      <entry value="43002" name="MAV_CMD_GUIDED_CHANGE_HEADING">
+        <description>Change to target heading at a given rate, overriding previous heading/s. This slews the vehicle at a controllable rate between it's previous heading and the new one. (affects GUIDED only. Exiting GUIDED returns aircraft to normal behaviour defined elsewhere. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="heading type" enum="HEADING_TYPE">course-over-ground or raw vehicle heading.</param>
+        <param index="2" label="heading target" units="deg" minValue="0" maxValue="359.99">Target heading.</param>
+        <param index="3" label="heading rate-of-change" units="m/s/s">Maximum centripetal accelearation, ie rate of change,  toward new heading.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
     </enum>
     <enum name="SCRIPTING_CMD">
       <entry value="0" name="SCRIPTING_CMD_REPL_START">
         <description>Start a REPL session.</description>
       </entry>
       <entry value="1" name="SCRIPTING_CMD_REPL_STOP">
         <description>End a REPL session.</description>
@@ -1291,15 +1329,14 @@
       <field type="uint16_t" name="throttle" units="d%">Throttle.</field>
       <field type="float" name="current" units="A">Current.</field>
       <field type="uint16_t" name="interference" units="%">Interference.</field>
       <field type="float" name="CompensationX">Motor Compensation X.</field>
       <field type="float" name="CompensationY">Motor Compensation Y.</field>
       <field type="float" name="CompensationZ">Motor Compensation Z.</field>
     </message>
-    <!-- Coming soon <message name="RALLY_LAND_POINT" id="177"> <description>A rally landing point. An aircraft loitering at a rally point may choose one of these points to land at.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> <field name="count" type="uint8_t">Total number of points (for sanity checking).</field> <field name="lat" type="int32_t">Latitude of point.</field> <field name="lng" type="int32_t">Longitude of point.</field> <field name="alt" type="uint16_t">Ground AGL (usually 0).</field> </message> <message name="RALLY_LAND_FETCH_POINT" id="178"> <description>Request a current rally land point from MAV.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> </message> -->
     <message id="178" name="AHRS2">
       <description>Status of secondary AHRS filter if available.</description>
       <field type="float" name="roll" units="rad">Roll angle.</field>
       <field type="float" name="pitch" units="rad">Pitch angle.</field>
       <field type="float" name="yaw" units="rad">Yaw angle.</field>
       <field type="float" name="altitude" units="m">Altitude (MSL).</field>
       <field type="int32_t" name="lat" units="degE7">Latitude.</field>
@@ -1444,16 +1481,16 @@
       <extensions/>
       <field type="float" name="airspeed_variance">Airspeed variance.</field>
     </message>
     <!-- realtime PID tuning message -->
     <message id="194" name="PID_TUNING">
       <description>PID tuning information.</description>
       <field type="uint8_t" name="axis" enum="PID_TUNING_AXIS">Axis.</field>
-      <field type="float" name="desired" units="deg/s">Desired rate.</field>
-      <field type="float" name="achieved" units="deg/s">Achieved rate.</field>
+      <field type="float" name="desired">Desired rate.</field>
+      <field type="float" name="achieved">Achieved rate.</field>
       <field type="float" name="FF">FF component.</field>
       <field type="float" name="P">P component.</field>
       <field type="float" name="I">I component.</field>
       <field type="float" name="D">D component.</field>
     </message>
     <message id="195" name="DEEPSTALL">
       <description>Deepstall path planning.</description>
```

### Comparing `pymavlink-2.4.8/dialects/v10/matrixpilot.py` & `pymavlink-2.4.9/dialects/v10/matrixpilot.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/ardupilotmega.py` & `pymavlink-2.4.9/dialects/v10/ardupilotmega.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,32 @@
 ACCELCAL_VEHICLE_POS_SUCCESS = 16777215 # 
 enums['ACCELCAL_VEHICLE_POS'][16777215] = EnumEntry('ACCELCAL_VEHICLE_POS_SUCCESS', '''''')
 ACCELCAL_VEHICLE_POS_FAILED = 16777216 # 
 enums['ACCELCAL_VEHICLE_POS'][16777216] = EnumEntry('ACCELCAL_VEHICLE_POS_FAILED', '''''')
 ACCELCAL_VEHICLE_POS_ENUM_END = 16777217 # 
 enums['ACCELCAL_VEHICLE_POS'][16777217] = EnumEntry('ACCELCAL_VEHICLE_POS_ENUM_END', '''''')
 
+# HEADING_TYPE
+enums['HEADING_TYPE'] = {}
+HEADING_TYPE_COURSE_OVER_GROUND = 0 # 
+enums['HEADING_TYPE'][0] = EnumEntry('HEADING_TYPE_COURSE_OVER_GROUND', '''''')
+HEADING_TYPE_HEADING = 1 # 
+enums['HEADING_TYPE'][1] = EnumEntry('HEADING_TYPE_HEADING', '''''')
+HEADING_TYPE_ENUM_END = 2 # 
+enums['HEADING_TYPE'][2] = EnumEntry('HEADING_TYPE_ENUM_END', '''''')
+
+# SPEED_TYPE
+enums['SPEED_TYPE'] = {}
+SPEED_TYPE_AIRSPEED = 0 # 
+enums['SPEED_TYPE'][0] = EnumEntry('SPEED_TYPE_AIRSPEED', '''''')
+SPEED_TYPE_GROUNDSPEED = 1 # 
+enums['SPEED_TYPE'][1] = EnumEntry('SPEED_TYPE_GROUNDSPEED', '''''')
+SPEED_TYPE_ENUM_END = 2 # 
+enums['SPEED_TYPE'][2] = EnumEntry('SPEED_TYPE_ENUM_END', '''''')
+
 # MAV_CMD
 enums['MAV_CMD'] = {}
 MAV_CMD_NAV_WAYPOINT = 16 # Navigate to waypoint.
 enums['MAV_CMD'][16] = EnumEntry('MAV_CMD_NAV_WAYPOINT', '''Navigate to waypoint.''')
 enums['MAV_CMD'][16].param[1] = '''Hold time. (ignored by fixed wing, time to stay at waypoint for rotary wing)'''
 enums['MAV_CMD'][16].param[2] = '''Acceptance radius (if the sphere with this radius is hit, the waypoint counts as reached)'''
 enums['MAV_CMD'][16].param[3] = '''0 to pass through the WP, if > 0 radius to pass by WP. Positive value for clockwise orbit, negative value for counter-clockwise orbit. Allows trajectory control.'''
@@ -449,17 +467,17 @@
                         # launches, allowing the aircraft to be idle
                         # until either an altitude is reached or a
                         # negative vertical speed is reached
                         # (indicating early balloon burst). The wiggle
                         # time is how often to wiggle the control
                         # surfaces to prevent them seizing up.
 enums['MAV_CMD'][83] = EnumEntry('MAV_CMD_NAV_ALTITUDE_WAIT', '''Mission command to wait for an altitude or downwards vertical speed. This is meant for high altitude balloon launches, allowing the aircraft to be idle until either an altitude is reached or a negative vertical speed is reached (indicating early balloon burst). The wiggle time is how often to wiggle the control surfaces to prevent them seizing up.''')
-enums['MAV_CMD'][83].param[1] = '''Altitude (m).'''
-enums['MAV_CMD'][83].param[2] = '''Descent speed (m/s).'''
-enums['MAV_CMD'][83].param[3] = '''Wiggle Time (s).'''
+enums['MAV_CMD'][83].param[1] = '''Altitude.'''
+enums['MAV_CMD'][83].param[2] = '''Descent speed.'''
+enums['MAV_CMD'][83].param[3] = '''How long to wiggle the control surfaces to prevent them seizing up.'''
 enums['MAV_CMD'][83].param[4] = '''Empty.'''
 enums['MAV_CMD'][83].param[5] = '''Empty.'''
 enums['MAV_CMD'][83].param[6] = '''Empty.'''
 enums['MAV_CMD'][83].param[7] = '''Empty.'''
 MAV_CMD_NAV_VTOL_TAKEOFF = 84 # Takeoff from ground using VTOL mode, and transition to forward flight
                         # with specified heading.
 enums['MAV_CMD'][84] = EnumEntry('MAV_CMD_NAV_VTOL_TAKEOFF', '''Takeoff from ground using VTOL mode, and transition to forward flight with specified heading.''')
@@ -903,16 +921,16 @@
 enums['MAV_CMD'][210].param[3] = '''Empty'''
 enums['MAV_CMD'][210].param[4] = '''Empty'''
 enums['MAV_CMD'][210].param[5] = '''Empty'''
 enums['MAV_CMD'][210].param[6] = '''Empty'''
 enums['MAV_CMD'][210].param[7] = '''Empty'''
 MAV_CMD_DO_GRIPPER = 211 # Mission command to operate EPM gripper.
 enums['MAV_CMD'][211] = EnumEntry('MAV_CMD_DO_GRIPPER', '''Mission command to operate EPM gripper.''')
-enums['MAV_CMD'][211].param[1] = '''Gripper number (a number from 1 to max number of grippers on the vehicle).'''
-enums['MAV_CMD'][211].param[2] = '''Gripper action (0=release, 1=grab. See GRIPPER_ACTIONS enum).'''
+enums['MAV_CMD'][211].param[1] = '''Gripper instance number (from 1 to max number of grippers on the vehicle).'''
+enums['MAV_CMD'][211].param[2] = '''Gripper action.'''
 enums['MAV_CMD'][211].param[3] = '''Empty.'''
 enums['MAV_CMD'][211].param[4] = '''Empty.'''
 enums['MAV_CMD'][211].param[5] = '''Empty.'''
 enums['MAV_CMD'][211].param[6] = '''Empty.'''
 enums['MAV_CMD'][211].param[7] = '''Empty.'''
 MAV_CMD_DO_AUTOTUNE_ENABLE = 212 # Enable/disable autotune.
 enums['MAV_CMD'][212] = EnumEntry('MAV_CMD_DO_AUTOTUNE_ENABLE', '''Enable/disable autotune.''')
@@ -1710,27 +1728,26 @@
 enums['MAV_CMD'][42003].param[6] = '''Empty.'''
 enums['MAV_CMD'][42003].param[7] = '''Empty.'''
 MAV_CMD_FIXED_MAG_CAL = 42004 # Magnetometer calibration based on fixed position         in earth
                         # field given by inclination, declination and
                         # intensity.
 enums['MAV_CMD'][42004] = EnumEntry('MAV_CMD_FIXED_MAG_CAL', '''Magnetometer calibration based on fixed position
         in earth field given by inclination, declination and intensity.''')
-enums['MAV_CMD'][42004].param[1] = '''MagDeclinationDegrees.'''
-enums['MAV_CMD'][42004].param[2] = '''MagInclinationDegrees.'''
-enums['MAV_CMD'][42004].param[3] = '''MagIntensityMilliGauss.'''
-enums['MAV_CMD'][42004].param[4] = '''YawDegrees.'''
+enums['MAV_CMD'][42004].param[1] = '''Magnetic declination.'''
+enums['MAV_CMD'][42004].param[2] = '''Magnetic inclination.'''
+enums['MAV_CMD'][42004].param[3] = '''Magnetic intensity.'''
+enums['MAV_CMD'][42004].param[4] = '''Yaw.'''
 enums['MAV_CMD'][42004].param[5] = '''Empty.'''
 enums['MAV_CMD'][42004].param[6] = '''Empty.'''
 enums['MAV_CMD'][42004].param[7] = '''Empty.'''
-MAV_CMD_FIXED_MAG_CAL_FIELD = 42005 # Magnetometer calibration based on fixed expected field values in
-                        # milliGauss.
-enums['MAV_CMD'][42005] = EnumEntry('MAV_CMD_FIXED_MAG_CAL_FIELD', '''Magnetometer calibration based on fixed expected field values in milliGauss.''')
-enums['MAV_CMD'][42005].param[1] = '''FieldX.'''
-enums['MAV_CMD'][42005].param[2] = '''FieldY.'''
-enums['MAV_CMD'][42005].param[3] = '''FieldZ.'''
+MAV_CMD_FIXED_MAG_CAL_FIELD = 42005 # Magnetometer calibration based on fixed expected field values.
+enums['MAV_CMD'][42005] = EnumEntry('MAV_CMD_FIXED_MAG_CAL_FIELD', '''Magnetometer calibration based on fixed expected field values.''')
+enums['MAV_CMD'][42005].param[1] = '''Field strength X.'''
+enums['MAV_CMD'][42005].param[2] = '''Field strength Y.'''
+enums['MAV_CMD'][42005].param[3] = '''Field strength Z.'''
 enums['MAV_CMD'][42005].param[4] = '''Empty.'''
 enums['MAV_CMD'][42005].param[5] = '''Empty.'''
 enums['MAV_CMD'][42005].param[6] = '''Empty.'''
 enums['MAV_CMD'][42005].param[7] = '''Empty.'''
 MAV_CMD_FIXED_MAG_CAL_YAW = 42006 # Magnetometer calibration based on provided known yaw. This allows for
                         # fast calibration using WMM field tables in
                         # the vehicle, given only the known yaw of the
@@ -1742,42 +1759,42 @@
 enums['MAV_CMD'][42006].param[3] = '''Latitude.'''
 enums['MAV_CMD'][42006].param[4] = '''Longitude.'''
 enums['MAV_CMD'][42006].param[5] = '''Empty.'''
 enums['MAV_CMD'][42006].param[6] = '''Empty.'''
 enums['MAV_CMD'][42006].param[7] = '''Empty.'''
 MAV_CMD_DO_START_MAG_CAL = 42424 # Initiate a magnetometer calibration.
 enums['MAV_CMD'][42424] = EnumEntry('MAV_CMD_DO_START_MAG_CAL', '''Initiate a magnetometer calibration.''')
-enums['MAV_CMD'][42424].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+enums['MAV_CMD'][42424].param[1] = '''Bitmask of magnetometers to calibrate. Use 0 to calibrate all sensors that can be started (sensors may not start if disabled, unhealthy, etc.). The command will NACK if calibration does not start for a sensor explicitly specified by the bitmask.'''
 enums['MAV_CMD'][42424].param[2] = '''Automatically retry on failure (0=no retry, 1=retry).'''
 enums['MAV_CMD'][42424].param[3] = '''Save without user input (0=require input, 1=autosave).'''
-enums['MAV_CMD'][42424].param[4] = '''Delay (seconds).'''
+enums['MAV_CMD'][42424].param[4] = '''Delay.'''
 enums['MAV_CMD'][42424].param[5] = '''Autoreboot (0=user reboot, 1=autoreboot).'''
 enums['MAV_CMD'][42424].param[6] = '''Empty.'''
 enums['MAV_CMD'][42424].param[7] = '''Empty.'''
-MAV_CMD_DO_ACCEPT_MAG_CAL = 42425 # Initiate a magnetometer calibration.
-enums['MAV_CMD'][42425] = EnumEntry('MAV_CMD_DO_ACCEPT_MAG_CAL', '''Initiate a magnetometer calibration.''')
-enums['MAV_CMD'][42425].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+MAV_CMD_DO_ACCEPT_MAG_CAL = 42425 # Accept a magnetometer calibration.
+enums['MAV_CMD'][42425] = EnumEntry('MAV_CMD_DO_ACCEPT_MAG_CAL', '''Accept a magnetometer calibration.''')
+enums['MAV_CMD'][42425].param[1] = '''Bitmask of magnetometers that calibration is accepted (0 means all).'''
 enums['MAV_CMD'][42425].param[2] = '''Empty.'''
 enums['MAV_CMD'][42425].param[3] = '''Empty.'''
 enums['MAV_CMD'][42425].param[4] = '''Empty.'''
 enums['MAV_CMD'][42425].param[5] = '''Empty.'''
 enums['MAV_CMD'][42425].param[6] = '''Empty.'''
 enums['MAV_CMD'][42425].param[7] = '''Empty.'''
 MAV_CMD_DO_CANCEL_MAG_CAL = 42426 # Cancel a running magnetometer calibration.
 enums['MAV_CMD'][42426] = EnumEntry('MAV_CMD_DO_CANCEL_MAG_CAL', '''Cancel a running magnetometer calibration.''')
-enums['MAV_CMD'][42426].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+enums['MAV_CMD'][42426].param[1] = '''Bitmask of magnetometers to cancel a running calibration (0 means all).'''
 enums['MAV_CMD'][42426].param[2] = '''Empty.'''
 enums['MAV_CMD'][42426].param[3] = '''Empty.'''
 enums['MAV_CMD'][42426].param[4] = '''Empty.'''
 enums['MAV_CMD'][42426].param[5] = '''Empty.'''
 enums['MAV_CMD'][42426].param[6] = '''Empty.'''
 enums['MAV_CMD'][42426].param[7] = '''Empty.'''
 MAV_CMD_SET_FACTORY_TEST_MODE = 42427 # Command autopilot to get into factory test/diagnostic mode.
 enums['MAV_CMD'][42427] = EnumEntry('MAV_CMD_SET_FACTORY_TEST_MODE', '''Command autopilot to get into factory test/diagnostic mode.''')
-enums['MAV_CMD'][42427].param[1] = '''0 means get out of test mode, 1 means get into test mode.'''
+enums['MAV_CMD'][42427].param[1] = '''0: activate test mode, 1: exit test mode.'''
 enums['MAV_CMD'][42427].param[2] = '''Empty.'''
 enums['MAV_CMD'][42427].param[3] = '''Empty.'''
 enums['MAV_CMD'][42427].param[4] = '''Empty.'''
 enums['MAV_CMD'][42427].param[5] = '''Empty.'''
 enums['MAV_CMD'][42427].param[6] = '''Empty.'''
 enums['MAV_CMD'][42427].param[7] = '''Empty.'''
 MAV_CMD_DO_SEND_BANNER = 42428 # Reply with the version banner.
@@ -1790,15 +1807,15 @@
 enums['MAV_CMD'][42428].param[6] = '''Empty.'''
 enums['MAV_CMD'][42428].param[7] = '''Empty.'''
 MAV_CMD_ACCELCAL_VEHICLE_POS = 42429 # Used when doing accelerometer calibration. When sent to the GCS tells
                         # it what position to put the vehicle in. When
                         # sent to the vehicle says what position the
                         # vehicle is in.
 enums['MAV_CMD'][42429] = EnumEntry('MAV_CMD_ACCELCAL_VEHICLE_POS', '''Used when doing accelerometer calibration. When sent to the GCS tells it what position to put the vehicle in. When sent to the vehicle says what position the vehicle is in.''')
-enums['MAV_CMD'][42429].param[1] = '''Position, one of the ACCELCAL_VEHICLE_POS enum values.'''
+enums['MAV_CMD'][42429].param[1] = '''Position.'''
 enums['MAV_CMD'][42429].param[2] = '''Empty.'''
 enums['MAV_CMD'][42429].param[3] = '''Empty.'''
 enums['MAV_CMD'][42429].param[4] = '''Empty.'''
 enums['MAV_CMD'][42429].param[5] = '''Empty.'''
 enums['MAV_CMD'][42429].param[6] = '''Empty.'''
 enums['MAV_CMD'][42429].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_RESET = 42501 # Causes the gimbal to reset and boot as if it was just powered on.
@@ -1810,15 +1827,15 @@
 enums['MAV_CMD'][42501].param[5] = '''Empty.'''
 enums['MAV_CMD'][42501].param[6] = '''Empty.'''
 enums['MAV_CMD'][42501].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS = 42502 # Reports progress and success or failure of gimbal axis calibration
                         # procedure.
 enums['MAV_CMD'][42502] = EnumEntry('MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS', '''Reports progress and success or failure of gimbal axis calibration procedure.''')
 enums['MAV_CMD'][42502].param[1] = '''Gimbal axis we're reporting calibration progress for.'''
-enums['MAV_CMD'][42502].param[2] = '''Current calibration progress for this axis, 0x64=100%.'''
+enums['MAV_CMD'][42502].param[2] = '''Current calibration progress for this axis.'''
 enums['MAV_CMD'][42502].param[3] = '''Status of the calibration.'''
 enums['MAV_CMD'][42502].param[4] = '''Empty.'''
 enums['MAV_CMD'][42502].param[5] = '''Empty.'''
 enums['MAV_CMD'][42502].param[6] = '''Empty.'''
 enums['MAV_CMD'][42502].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION = 42503 # Starts commutation calibration on the gimbal.
 enums['MAV_CMD'][42503] = EnumEntry('MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION', '''Starts commutation calibration on the gimbal.''')
@@ -1836,18 +1853,18 @@
 enums['MAV_CMD'][42505].param[3] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[4] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[5] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[6] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[7] = '''Magic number.'''
 MAV_CMD_DO_WINCH = 42600 # Command to operate winch.
 enums['MAV_CMD'][42600] = EnumEntry('MAV_CMD_DO_WINCH', '''Command to operate winch.''')
-enums['MAV_CMD'][42600].param[1] = '''Winch number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).'''
-enums['MAV_CMD'][42600].param[2] = '''Action (0=relax, 1=relative length control, 2=rate control. See WINCH_ACTIONS enum.).'''
-enums['MAV_CMD'][42600].param[3] = '''Release length (cable distance to unwind in meters, negative numbers to wind in cable).'''
-enums['MAV_CMD'][42600].param[4] = '''Release rate (meters/second).'''
+enums['MAV_CMD'][42600].param[1] = '''Winch instance number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).'''
+enums['MAV_CMD'][42600].param[2] = '''Action.'''
+enums['MAV_CMD'][42600].param[3] = '''Release length (cable distance to unwind, negative numbers to wind in cable).'''
+enums['MAV_CMD'][42600].param[4] = '''Release rate.'''
 enums['MAV_CMD'][42600].param[5] = '''Empty.'''
 enums['MAV_CMD'][42600].param[6] = '''Empty.'''
 enums['MAV_CMD'][42600].param[7] = '''Empty.'''
 MAV_CMD_FLASH_BOOTLOADER = 42650 # Update the bootloader
 enums['MAV_CMD'][42650] = EnumEntry('MAV_CMD_FLASH_BOOTLOADER', '''Update the bootloader''')
 enums['MAV_CMD'][42650].param[1] = '''Empty'''
 enums['MAV_CMD'][42650].param[2] = '''Empty'''
@@ -1881,16 +1898,62 @@
 enums['MAV_CMD'][42701].param[1] = '''Scripting command to execute'''
 enums['MAV_CMD'][42701].param[2] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[3] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[4] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[5] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[6] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[7] = '''Reserved (default:0)'''
-MAV_CMD_ENUM_END = 42702 # 
-enums['MAV_CMD'][42702] = EnumEntry('MAV_CMD_ENUM_END', '''''')
+MAV_CMD_GUIDED_CHANGE_SPEED = 43000 # Change flight speed at a given rate. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # speed and the new one. (affects GUIDED only.
+                        # Outside GUIDED, aircraft ignores these
+                        # commands. Designed for onboard companion-
+                        # computer command-and-control, not normally
+                        # operator/GCS control.)
+enums['MAV_CMD'][43000] = EnumEntry('MAV_CMD_GUIDED_CHANGE_SPEED', '''Change flight speed at a given rate. This slews the vehicle at a controllable rate between it's previous speed and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43000].param[1] = '''Airspeed or groundspeed.'''
+enums['MAV_CMD'][43000].param[2] = '''Target Speed'''
+enums['MAV_CMD'][43000].param[3] = '''Acceleration rate, 0 to take effect instantly'''
+enums['MAV_CMD'][43000].param[4] = '''Empty'''
+enums['MAV_CMD'][43000].param[5] = '''Empty'''
+enums['MAV_CMD'][43000].param[6] = '''Empty'''
+enums['MAV_CMD'][43000].param[7] = '''Empty'''
+MAV_CMD_GUIDED_CHANGE_ALTITUDE = 43001 # Change target altitude at a given rate. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # altitude and the new one. (affects GUIDED
+                        # only. Outside GUIDED, aircraft ignores these
+                        # commands. Designed for onboard companion-
+                        # computer command-and-control, not normally
+                        # operator/GCS control.)
+enums['MAV_CMD'][43001] = EnumEntry('MAV_CMD_GUIDED_CHANGE_ALTITUDE', '''Change target altitude at a given rate. This slews the vehicle at a controllable rate between it's previous altitude and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43001].param[1] = '''Empty'''
+enums['MAV_CMD'][43001].param[2] = '''Empty'''
+enums['MAV_CMD'][43001].param[3] = '''Rate of change, toward new altitude. 0 for maximum rate change. Positive numbers only, as negative numbers will not converge on the new target alt.'''
+enums['MAV_CMD'][43001].param[4] = '''Empty'''
+enums['MAV_CMD'][43001].param[5] = '''Empty'''
+enums['MAV_CMD'][43001].param[6] = '''Empty'''
+enums['MAV_CMD'][43001].param[7] = '''Target Altitude'''
+MAV_CMD_GUIDED_CHANGE_HEADING = 43002 # Change to target heading at a given rate, overriding previous
+                        # heading/s. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # heading and the new one. (affects GUIDED
+                        # only. Exiting GUIDED returns aircraft to
+                        # normal behaviour defined elsewhere. Designed
+                        # for onboard companion-computer command-and-
+                        # control, not normally operator/GCS control.)
+enums['MAV_CMD'][43002] = EnumEntry('MAV_CMD_GUIDED_CHANGE_HEADING', '''Change to target heading at a given rate, overriding previous heading/s. This slews the vehicle at a controllable rate between it's previous heading and the new one. (affects GUIDED only. Exiting GUIDED returns aircraft to normal behaviour defined elsewhere. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43002].param[1] = '''course-over-ground or raw vehicle heading.'''
+enums['MAV_CMD'][43002].param[2] = '''Target heading.'''
+enums['MAV_CMD'][43002].param[3] = '''Maximum centripetal accelearation, ie rate of change,  toward new heading.'''
+enums['MAV_CMD'][43002].param[4] = '''Empty'''
+enums['MAV_CMD'][43002].param[5] = '''Empty'''
+enums['MAV_CMD'][43002].param[6] = '''Empty'''
+enums['MAV_CMD'][43002].param[7] = '''Empty'''
+MAV_CMD_ENUM_END = 43003 # 
+enums['MAV_CMD'][43003] = EnumEntry('MAV_CMD_ENUM_END', '''''')
 
 # SCRIPTING_CMD
 enums['SCRIPTING_CMD'] = {}
 SCRIPTING_CMD_REPL_START = 0 # Start a REPL session.
 enums['SCRIPTING_CMD'][0] = EnumEntry('SCRIPTING_CMD_REPL_START', '''Start a REPL session.''')
 SCRIPTING_CMD_REPL_STOP = 1 # End a REPL session.
 enums['SCRIPTING_CMD'][1] = EnumEntry('SCRIPTING_CMD_REPL_STOP', '''End a REPL session.''')
@@ -6536,15 +6599,15 @@
         id = MAVLINK_MSG_ID_PID_TUNING
         name = 'PID_TUNING'
         fieldnames = ['axis', 'desired', 'achieved', 'FF', 'P', 'I', 'D']
         ordered_fieldnames = ['desired', 'achieved', 'FF', 'P', 'I', 'D', 'axis']
         fieldtypes = ['uint8_t', 'float', 'float', 'float', 'float', 'float', 'float']
         fielddisplays_by_name = {}
         fieldenums_by_name = {"axis": "PID_TUNING_AXIS"}
-        fieldunits_by_name = {"desired": "deg/s", "achieved": "deg/s"}
+        fieldunits_by_name = {}
         format = '<ffffffB'
         native_format = bytearray('<ffffffB', 'ascii')
         orders = [6, 0, 1, 2, 3, 4, 5]
         lengths = [1, 1, 1, 1, 1, 1, 1]
         array_lengths = [0, 0, 0, 0, 0, 0, 0]
         crc_extra = 98
         unpacker = struct.Struct('<ffffffB')
@@ -13642,31 +13705,31 @@
                 return self.send(self.ekf_status_report_encode(flags, velocity_variance, pos_horiz_variance, pos_vert_variance, compass_variance, terrain_alt_variance), force_mavlink1=force_mavlink1)
 
         def pid_tuning_encode(self, axis, desired, achieved, FF, P, I, D):
                 '''
                 PID tuning information.
 
                 axis                      : Axis. (type:uint8_t, values:PID_TUNING_AXIS)
-                desired                   : Desired rate. [deg/s] (type:float)
-                achieved                  : Achieved rate. [deg/s] (type:float)
+                desired                   : Desired rate. (type:float)
+                achieved                  : Achieved rate. (type:float)
                 FF                        : FF component. (type:float)
                 P                         : P component. (type:float)
                 I                         : I component. (type:float)
                 D                         : D component. (type:float)
 
                 '''
                 return MAVLink_pid_tuning_message(axis, desired, achieved, FF, P, I, D)
 
         def pid_tuning_send(self, axis, desired, achieved, FF, P, I, D, force_mavlink1=False):
                 '''
                 PID tuning information.
 
                 axis                      : Axis. (type:uint8_t, values:PID_TUNING_AXIS)
-                desired                   : Desired rate. [deg/s] (type:float)
-                achieved                  : Achieved rate. [deg/s] (type:float)
+                desired                   : Desired rate. (type:float)
+                achieved                  : Achieved rate. (type:float)
                 FF                        : FF component. (type:float)
                 P                         : P component. (type:float)
                 I                         : I component. (type:float)
                 D                         : D component. (type:float)
 
                 '''
                 return self.send(self.pid_tuning_encode(axis, desired, achieved, FF, P, I, D), force_mavlink1=force_mavlink1)
```

### Comparing `pymavlink-2.4.8/dialects/v10/paparazzi.xml` & `pymavlink-2.4.9/dialects/v10/paparazzi.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/python_array_test.py` & `pymavlink-2.4.9/dialects/v10/python_array_test.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/test.xml` & `pymavlink-2.4.9/dialects/v10/test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/icarous.py` & `pymavlink-2.4.9/dialects/v10/icarous.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/minimal.xml` & `pymavlink-2.4.9/dialects/v10/minimal.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/test.py` & `pymavlink-2.4.9/dialects/v10/test.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/autoquad.py` & `pymavlink-2.4.9/dialects/v10/autoquad.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/standard.py` & `pymavlink-2.4.9/dialects/v10/standard.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/common.xml` & `pymavlink-2.4.9/dialects/v10/common.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/slugs.py` & `pymavlink-2.4.9/dialects/v10/slugs.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v10/autoquad.xml` & `pymavlink-2.4.9/dialects/v10/autoquad.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ASLUAV.py` & `pymavlink-2.4.9/dialects/v20/ASLUAV.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/uAvionix.xml` & `pymavlink-2.4.9/dialects/v20/uAvionix.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/python_array_test.xml` & `pymavlink-2.4.9/dialects/v20/python_array_test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/minimal.py` & `pymavlink-2.4.9/dialects/v20/minimal.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/uAvionix.py` & `pymavlink-2.4.9/dialects/v20/uAvionix.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/slugs.xml` & `pymavlink-2.4.9/dialects/v20/slugs.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ualberta.xml` & `pymavlink-2.4.9/dialects/v20/ualberta.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ualberta.py` & `pymavlink-2.4.9/dialects/v20/ualberta.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/icarous.xml` & `pymavlink-2.4.9/dialects/v20/icarous.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/matrixpilot.xml` & `pymavlink-2.4.9/dialects/v20/matrixpilot.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/paparazzi.py` & `pymavlink-2.4.9/dialects/v20/paparazzi.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ASLUAV.xml` & `pymavlink-2.4.9/dialects/v20/ASLUAV.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/common.py` & `pymavlink-2.4.9/dialects/v20/common.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ardupilotmega.xml` & `pymavlink-2.4.9/dialects/v20/ardupilotmega.xml`

 * *Files 3% similar despite different names*

#### Comparing `pymavlink-2.4.8/dialects/v20/ardupilotmega.xml` & `pymavlink-2.4.9/dialects/v20/ardupilotmega.xml`

```diff
@@ -13,29 +13,37 @@
       <entry value="3" name="ACCELCAL_VEHICLE_POS_RIGHT"/>
       <entry value="4" name="ACCELCAL_VEHICLE_POS_NOSEDOWN"/>
       <entry value="5" name="ACCELCAL_VEHICLE_POS_NOSEUP"/>
       <entry value="6" name="ACCELCAL_VEHICLE_POS_BACK"/>
       <entry value="16777215" name="ACCELCAL_VEHICLE_POS_SUCCESS"/>
       <entry value="16777216" name="ACCELCAL_VEHICLE_POS_FAILED"/>
     </enum>
+    <enum name="HEADING_TYPE">
+      <entry value="0" name="HEADING_TYPE_COURSE_OVER_GROUND"/>
+      <entry value="1" name="HEADING_TYPE_HEADING"/>
+    </enum>
+    <enum name="SPEED_TYPE">
+      <entry value="0" name="SPEED_TYPE_AIRSPEED"/>
+      <entry value="1" name="SPEED_TYPE_GROUNDSPEED"/>
+    </enum>
     <!-- ardupilot specific MAV_CMD_* commands -->
     <enum name="MAV_CMD">
-      <entry value="211" name="MAV_CMD_DO_GRIPPER">
+      <entry value="211" name="MAV_CMD_DO_GRIPPER" hasLocation="false" isDestination="false">
         <description>Mission command to operate EPM gripper.</description>
-        <param index="1">Gripper number (a number from 1 to max number of grippers on the vehicle).</param>
-        <param index="2">Gripper action (0=release, 1=grab. See GRIPPER_ACTIONS enum).</param>
+        <param index="1" label="Instance" minValue="1" increment="1">Gripper instance number (from 1 to max number of grippers on the vehicle).</param>
+        <param index="2" label="Action" enum="GRIPPER_ACTIONS">Gripper action.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE">
+      <entry value="212" name="MAV_CMD_DO_AUTOTUNE_ENABLE" hasLocation="false" isDestination="false">
         <description>Enable/disable autotune.</description>
-        <param index="1">Enable (1: enable, 0:disable).</param>
+        <param index="1" label="Enable" minValue="0" maxValue="1" increment="1">Enable (1: enable, 0:disable).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
@@ -45,81 +53,81 @@
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT">
+      <entry value="83" name="MAV_CMD_NAV_ALTITUDE_WAIT" hasLocation="false" isDestination="false">
         <description>Mission command to wait for an altitude or downwards vertical speed. This is meant for high altitude balloon launches, allowing the aircraft to be idle until either an altitude is reached or a negative vertical speed is reached (indicating early balloon burst). The wiggle time is how often to wiggle the control surfaces to prevent them seizing up.</description>
-        <param index="1">Altitude (m).</param>
-        <param index="2">Descent speed (m/s).</param>
-        <param index="3">Wiggle Time (s).</param>
+        <param index="1" label="Altitude" units="m">Altitude.</param>
+        <param index="2" label="Descent Speed" units="m/s">Descent speed.</param>
+        <param index="3" label="Wiggle Time" units="s">How long to wiggle the control surfaces to prevent them seizing up.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED">
+      <entry value="42000" name="MAV_CMD_POWER_OFF_INITIATED" hasLocation="false" isDestination="false">
         <description>A system wide power-off event has been initiated.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <!-- MAV_CMD_SOLO_BTN_* are here to provide vendor-specific support for 3DR Solo until a better solution is found to atomically make multiple commands with control flow -->
-      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK">
+      <entry value="42001" name="MAV_CMD_SOLO_BTN_FLY_CLICK" hasLocation="false" isDestination="false">
         <description>FLY button has been clicked.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD">
+      <entry value="42002" name="MAV_CMD_SOLO_BTN_FLY_HOLD" hasLocation="false" isDestination="false">
         <description>FLY button has been held for 1.5 seconds.</description>
-        <param index="1">Takeoff altitude.</param>
+        <param index="1" label="Takeoff Altitude" units="m">Takeoff altitude.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK">
+      <entry value="42003" name="MAV_CMD_SOLO_BTN_PAUSE_CLICK" hasLocation="false" isDestination="false">
         <description>PAUSE button has been clicked.</description>
-        <param index="1">1 if Solo is in a shot mode, 0 otherwise.</param>
+        <param index="1" label="Shot Mode" minValue="0" maxValue="1" increment="1">1 if Solo is in a shot mode, 0 otherwise.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL">
+      <entry value="42004" name="MAV_CMD_FIXED_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Magnetometer calibration based on fixed position
         in earth field given by inclination, declination and intensity.</description>
-        <param index="1">MagDeclinationDegrees.</param>
-        <param index="2">MagInclinationDegrees.</param>
-        <param index="3">MagIntensityMilliGauss.</param>
-        <param index="4">YawDegrees.</param>
+        <param index="1" label="Declination" units="deg">Magnetic declination.</param>
+        <param index="2" label="Inclination" units="deg">Magnetic inclination.</param>
+        <param index="3" label="Intensity" units="mgauss">Magnetic intensity.</param>
+        <param index="4" label="Yaw" units="deg">Yaw.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD">
-        <description>Magnetometer calibration based on fixed expected field values in milliGauss.</description>
-        <param index="1">FieldX.</param>
-        <param index="2">FieldY.</param>
-        <param index="3">FieldZ.</param>
+      <entry value="42005" name="MAV_CMD_FIXED_MAG_CAL_FIELD" hasLocation="false" isDestination="false">
+        <description>Magnetometer calibration based on fixed expected field values.</description>
+        <param index="1" label="Field X" units="mgauss">Field strength X.</param>
+        <param index="2" label="Field Y" units="mgauss">Field strength Y.</param>
+        <param index="3" label="Field Z" units="mgauss">Field strength Z.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42006" name="MAV_CMD_FIXED_MAG_CAL_YAW">
         <description>Magnetometer calibration based on provided known yaw. This allows for fast calibration using WMM field tables in the vehicle, given only the known yaw of the vehicle. If Latitude and longitude are both zero then use the current vehicle location.</description>
@@ -127,131 +135,131 @@
         <param index="2" label="CompassMask">CompassMask, 0 for all.</param>
         <param index="3" label="Lattitude" units="deg">Latitude.</param>
         <param index="4" label="Longitude" units="deg">Longitude.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL">
+      <entry value="42424" name="MAV_CMD_DO_START_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
-        <param index="2">Automatically retry on failure (0=no retry, 1=retry).</param>
-        <param index="3">Save without user input (0=require input, 1=autosave).</param>
-        <param index="4">Delay (seconds).</param>
-        <param index="5">Autoreboot (0=user reboot, 1=autoreboot).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to calibrate. Use 0 to calibrate all sensors that can be started (sensors may not start if disabled, unhealthy, etc.). The command will NACK if calibration does not start for a sensor explicitly specified by the bitmask.</param>
+        <param index="2" label="Retry on Failure" minValue="0" maxValue="1" increment="1">Automatically retry on failure (0=no retry, 1=retry).</param>
+        <param index="3" label="Autosave" minValue="0" maxValue="1" increment="1">Save without user input (0=require input, 1=autosave).</param>
+        <param index="4" label="Delay" units="s">Delay.</param>
+        <param index="5" label="Autoreboot" minValue="0" maxValue="1" increment="1">Autoreboot (0=user reboot, 1=autoreboot).</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL">
-        <description>Initiate a magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+      <entry value="42425" name="MAV_CMD_DO_ACCEPT_MAG_CAL" hasLocation="false" isDestination="false">
+        <description>Accept a magnetometer calibration.</description>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers that calibration is accepted (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL">
+      <entry value="42426" name="MAV_CMD_DO_CANCEL_MAG_CAL" hasLocation="false" isDestination="false">
         <description>Cancel a running magnetometer calibration.</description>
-        <param index="1">uint8_t bitmask of magnetometers (0 means all).</param>
+        <param index="1" label="Magnetometers Bitmask" minValue="0" maxValue="255" increment="1">Bitmask of magnetometers to cancel a running calibration (0 means all).</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS">
+      <entry value="42429" name="MAV_CMD_ACCELCAL_VEHICLE_POS" hasLocation="false" isDestination="false">
         <description>Used when doing accelerometer calibration. When sent to the GCS tells it what position to put the vehicle in. When sent to the vehicle says what position the vehicle is in.</description>
-        <param index="1">Position, one of the ACCELCAL_VEHICLE_POS enum values.</param>
+        <param index="1" label="Position" enum="ACCELCAL_VEHICLE_POS">Position.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER">
+      <entry value="42428" name="MAV_CMD_DO_SEND_BANNER" hasLocation="false" isDestination="false">
         <description>Reply with the version banner.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE">
+      <entry value="42427" name="MAV_CMD_SET_FACTORY_TEST_MODE" hasLocation="false" isDestination="false">
         <description>Command autopilot to get into factory test/diagnostic mode.</description>
-        <param index="1">0 means get out of test mode, 1 means get into test mode.</param>
+        <param index="1" label="Test Mode" minValue="0" maxValue="1" increment="1">0: activate test mode, 1: exit test mode.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42501" name="MAV_CMD_GIMBAL_RESET">
+      <entry value="42501" name="MAV_CMD_GIMBAL_RESET" hasLocation="false" isDestination="false">
         <description>Causes the gimbal to reset and boot as if it was just powered on.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS">
+      <entry value="42502" name="MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS" hasLocation="false" isDestination="false">
         <description>Reports progress and success or failure of gimbal axis calibration procedure.</description>
-        <param index="1">Gimbal axis we're reporting calibration progress for.</param>
-        <param index="2">Current calibration progress for this axis, 0x64=100%.</param>
-        <param index="3">Status of the calibration.</param>
+        <param index="1" label="Axis" enum="GIMBAL_AXIS">Gimbal axis we're reporting calibration progress for.</param>
+        <param index="2" label="Progress" units="%" minValue="0" maxValue="100">Current calibration progress for this axis.</param>
+        <param index="3" label="Status" enum="GIMBAL_AXIS_CALIBRATION_STATUS">Status of the calibration.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION">
+      <entry value="42503" name="MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION" hasLocation="false" isDestination="false">
         <description>Starts commutation calibration on the gimbal.</description>
         <param index="1">Empty.</param>
         <param index="2">Empty.</param>
         <param index="3">Empty.</param>
         <param index="4">Empty.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET">
+      <entry value="42505" name="MAV_CMD_GIMBAL_FULL_RESET" hasLocation="false" isDestination="false">
         <description>Erases gimbal application and parameters.</description>
         <param index="1">Magic number.</param>
         <param index="2">Magic number.</param>
         <param index="3">Magic number.</param>
         <param index="4">Magic number.</param>
         <param index="5">Magic number.</param>
         <param index="6">Magic number.</param>
         <param index="7">Magic number.</param>
       </entry>
-      <entry value="42600" name="MAV_CMD_DO_WINCH">
+      <entry value="42600" name="MAV_CMD_DO_WINCH" hasLocation="false" isDestination="false">
         <description>Command to operate winch.</description>
-        <param index="1">Winch number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
-        <param index="2">Action (0=relax, 1=relative length control, 2=rate control. See WINCH_ACTIONS enum.).</param>
-        <param index="3">Release length (cable distance to unwind in meters, negative numbers to wind in cable).</param>
-        <param index="4">Release rate (meters/second).</param>
+        <param index="1" label="Instance" minValue="0" increment="1">Winch instance number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).</param>
+        <param index="2" label="Action" enum="WINCH_ACTIONS">Action.</param>
+        <param index="3" label="Length" units="m">Release length (cable distance to unwind, negative numbers to wind in cable).</param>
+        <param index="4" label="Rate" units="m/s">Release rate.</param>
         <param index="5">Empty.</param>
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
-      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER">
+      <entry value="42650" name="MAV_CMD_FLASH_BOOTLOADER" hasLocation="false" isDestination="false">
         <description>Update the bootloader</description>
         <param index="1">Empty</param>
         <param index="2">Empty</param>
         <param index="3">Empty</param>
         <param index="4">Empty</param>
-        <param index="5">Magic number - set to 290876 to actually flash</param>
+        <param index="5" label="Magic Number" increment="1">Magic number - set to 290876 to actually flash</param>
         <param index="6">Empty</param>
         <param index="7">Empty</param>
       </entry>
       <entry value="42651" name="MAV_CMD_BATTERY_RESET" hasLocation="false" isDestination="false">
         <description>Reset battery capacity for batteries that accumulate consumed battery via integration.</description>
         <param index="1" label="battery mask">Bitmask of batteries to reset. Least significant bit is for the first battery.</param>
         <param index="2" label="percentage" minValue="0" maxValue="100" increment="1">Battery percentage remaining to set.</param>
@@ -266,14 +274,44 @@
         <param index="6">Empty.</param>
         <param index="7">Empty.</param>
       </entry>
       <entry value="42701" name="MAV_CMD_SCRIPTING">
         <description>Control onboard scripting.</description>
         <param index="1" enum="SCRIPTING_CMD">Scripting command to execute</param>
       </entry>
+      <entry value="43000" name="MAV_CMD_GUIDED_CHANGE_SPEED">
+        <description>Change flight speed at a given rate. This slews the vehicle at a controllable rate between it's previous speed and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="speed type" enum="SPEED_TYPE">Airspeed or groundspeed.</param>
+        <param index="2" label="speed target" units="m/s">Target Speed</param>
+        <param index="3" label="speed rate-of-change" units="m/s/s">Acceleration rate, 0 to take effect instantly</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
+      <entry value="43001" name="MAV_CMD_GUIDED_CHANGE_ALTITUDE">
+        <description>Change target altitude at a given rate. This slews the vehicle at a controllable rate between it's previous altitude and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1">Empty</param>
+        <param index="2">Empty</param>
+        <param index="3" label="alt rate-of-change" units="m/s/s" minValue="0">Rate of change, toward new altitude. 0 for maximum rate change. Positive numbers only, as negative numbers will not converge on the new target alt.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7" label="target alt" units="m">Target Altitude</param>
+      </entry>
+      <entry value="43002" name="MAV_CMD_GUIDED_CHANGE_HEADING">
+        <description>Change to target heading at a given rate, overriding previous heading/s. This slews the vehicle at a controllable rate between it's previous heading and the new one. (affects GUIDED only. Exiting GUIDED returns aircraft to normal behaviour defined elsewhere. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)</description>
+        <param index="1" label="heading type" enum="HEADING_TYPE">course-over-ground or raw vehicle heading.</param>
+        <param index="2" label="heading target" units="deg" minValue="0" maxValue="359.99">Target heading.</param>
+        <param index="3" label="heading rate-of-change" units="m/s/s">Maximum centripetal accelearation, ie rate of change,  toward new heading.</param>
+        <param index="4">Empty</param>
+        <param index="5">Empty</param>
+        <param index="6">Empty</param>
+        <param index="7">Empty</param>
+      </entry>
     </enum>
     <enum name="SCRIPTING_CMD">
       <entry value="0" name="SCRIPTING_CMD_REPL_START">
         <description>Start a REPL session.</description>
       </entry>
       <entry value="1" name="SCRIPTING_CMD_REPL_STOP">
         <description>End a REPL session.</description>
@@ -1291,15 +1329,14 @@
       <field type="uint16_t" name="throttle" units="d%">Throttle.</field>
       <field type="float" name="current" units="A">Current.</field>
       <field type="uint16_t" name="interference" units="%">Interference.</field>
       <field type="float" name="CompensationX">Motor Compensation X.</field>
       <field type="float" name="CompensationY">Motor Compensation Y.</field>
       <field type="float" name="CompensationZ">Motor Compensation Z.</field>
     </message>
-    <!-- Coming soon <message name="RALLY_LAND_POINT" id="177"> <description>A rally landing point. An aircraft loitering at a rally point may choose one of these points to land at.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> <field name="count" type="uint8_t">Total number of points (for sanity checking).</field> <field name="lat" type="int32_t">Latitude of point.</field> <field name="lng" type="int32_t">Longitude of point.</field> <field name="alt" type="uint16_t">Ground AGL (usually 0).</field> </message> <message name="RALLY_LAND_FETCH_POINT" id="178"> <description>Request a current rally land point from MAV.</description> <field name="target_system" type="uint8_t">System ID.</field> <field name="target_component" type="uint8_t">Component ID.</field> <field name="idx" type="uint8_t">Point index (first point is 0).</field> </message> -->
     <message id="178" name="AHRS2">
       <description>Status of secondary AHRS filter if available.</description>
       <field type="float" name="roll" units="rad">Roll angle.</field>
       <field type="float" name="pitch" units="rad">Pitch angle.</field>
       <field type="float" name="yaw" units="rad">Yaw angle.</field>
       <field type="float" name="altitude" units="m">Altitude (MSL).</field>
       <field type="int32_t" name="lat" units="degE7">Latitude.</field>
@@ -1444,16 +1481,16 @@
       <extensions/>
       <field type="float" name="airspeed_variance">Airspeed variance.</field>
     </message>
     <!-- realtime PID tuning message -->
     <message id="194" name="PID_TUNING">
       <description>PID tuning information.</description>
       <field type="uint8_t" name="axis" enum="PID_TUNING_AXIS">Axis.</field>
-      <field type="float" name="desired" units="deg/s">Desired rate.</field>
-      <field type="float" name="achieved" units="deg/s">Achieved rate.</field>
+      <field type="float" name="desired">Desired rate.</field>
+      <field type="float" name="achieved">Achieved rate.</field>
       <field type="float" name="FF">FF component.</field>
       <field type="float" name="P">P component.</field>
       <field type="float" name="I">I component.</field>
       <field type="float" name="D">D component.</field>
     </message>
     <message id="195" name="DEEPSTALL">
       <description>Deepstall path planning.</description>
```

### Comparing `pymavlink-2.4.8/dialects/v20/matrixpilot.py` & `pymavlink-2.4.9/dialects/v20/matrixpilot.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/ardupilotmega.py` & `pymavlink-2.4.9/dialects/v20/ardupilotmega.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,32 @@
 ACCELCAL_VEHICLE_POS_SUCCESS = 16777215 # 
 enums['ACCELCAL_VEHICLE_POS'][16777215] = EnumEntry('ACCELCAL_VEHICLE_POS_SUCCESS', '''''')
 ACCELCAL_VEHICLE_POS_FAILED = 16777216 # 
 enums['ACCELCAL_VEHICLE_POS'][16777216] = EnumEntry('ACCELCAL_VEHICLE_POS_FAILED', '''''')
 ACCELCAL_VEHICLE_POS_ENUM_END = 16777217 # 
 enums['ACCELCAL_VEHICLE_POS'][16777217] = EnumEntry('ACCELCAL_VEHICLE_POS_ENUM_END', '''''')
 
+# HEADING_TYPE
+enums['HEADING_TYPE'] = {}
+HEADING_TYPE_COURSE_OVER_GROUND = 0 # 
+enums['HEADING_TYPE'][0] = EnumEntry('HEADING_TYPE_COURSE_OVER_GROUND', '''''')
+HEADING_TYPE_HEADING = 1 # 
+enums['HEADING_TYPE'][1] = EnumEntry('HEADING_TYPE_HEADING', '''''')
+HEADING_TYPE_ENUM_END = 2 # 
+enums['HEADING_TYPE'][2] = EnumEntry('HEADING_TYPE_ENUM_END', '''''')
+
+# SPEED_TYPE
+enums['SPEED_TYPE'] = {}
+SPEED_TYPE_AIRSPEED = 0 # 
+enums['SPEED_TYPE'][0] = EnumEntry('SPEED_TYPE_AIRSPEED', '''''')
+SPEED_TYPE_GROUNDSPEED = 1 # 
+enums['SPEED_TYPE'][1] = EnumEntry('SPEED_TYPE_GROUNDSPEED', '''''')
+SPEED_TYPE_ENUM_END = 2 # 
+enums['SPEED_TYPE'][2] = EnumEntry('SPEED_TYPE_ENUM_END', '''''')
+
 # MAV_CMD
 enums['MAV_CMD'] = {}
 MAV_CMD_NAV_WAYPOINT = 16 # Navigate to waypoint.
 enums['MAV_CMD'][16] = EnumEntry('MAV_CMD_NAV_WAYPOINT', '''Navigate to waypoint.''')
 enums['MAV_CMD'][16].param[1] = '''Hold time. (ignored by fixed wing, time to stay at waypoint for rotary wing)'''
 enums['MAV_CMD'][16].param[2] = '''Acceptance radius (if the sphere with this radius is hit, the waypoint counts as reached)'''
 enums['MAV_CMD'][16].param[3] = '''0 to pass through the WP, if > 0 radius to pass by WP. Positive value for clockwise orbit, negative value for counter-clockwise orbit. Allows trajectory control.'''
@@ -449,17 +467,17 @@
                         # launches, allowing the aircraft to be idle
                         # until either an altitude is reached or a
                         # negative vertical speed is reached
                         # (indicating early balloon burst). The wiggle
                         # time is how often to wiggle the control
                         # surfaces to prevent them seizing up.
 enums['MAV_CMD'][83] = EnumEntry('MAV_CMD_NAV_ALTITUDE_WAIT', '''Mission command to wait for an altitude or downwards vertical speed. This is meant for high altitude balloon launches, allowing the aircraft to be idle until either an altitude is reached or a negative vertical speed is reached (indicating early balloon burst). The wiggle time is how often to wiggle the control surfaces to prevent them seizing up.''')
-enums['MAV_CMD'][83].param[1] = '''Altitude (m).'''
-enums['MAV_CMD'][83].param[2] = '''Descent speed (m/s).'''
-enums['MAV_CMD'][83].param[3] = '''Wiggle Time (s).'''
+enums['MAV_CMD'][83].param[1] = '''Altitude.'''
+enums['MAV_CMD'][83].param[2] = '''Descent speed.'''
+enums['MAV_CMD'][83].param[3] = '''How long to wiggle the control surfaces to prevent them seizing up.'''
 enums['MAV_CMD'][83].param[4] = '''Empty.'''
 enums['MAV_CMD'][83].param[5] = '''Empty.'''
 enums['MAV_CMD'][83].param[6] = '''Empty.'''
 enums['MAV_CMD'][83].param[7] = '''Empty.'''
 MAV_CMD_NAV_VTOL_TAKEOFF = 84 # Takeoff from ground using VTOL mode, and transition to forward flight
                         # with specified heading.
 enums['MAV_CMD'][84] = EnumEntry('MAV_CMD_NAV_VTOL_TAKEOFF', '''Takeoff from ground using VTOL mode, and transition to forward flight with specified heading.''')
@@ -903,16 +921,16 @@
 enums['MAV_CMD'][210].param[3] = '''Empty'''
 enums['MAV_CMD'][210].param[4] = '''Empty'''
 enums['MAV_CMD'][210].param[5] = '''Empty'''
 enums['MAV_CMD'][210].param[6] = '''Empty'''
 enums['MAV_CMD'][210].param[7] = '''Empty'''
 MAV_CMD_DO_GRIPPER = 211 # Mission command to operate EPM gripper.
 enums['MAV_CMD'][211] = EnumEntry('MAV_CMD_DO_GRIPPER', '''Mission command to operate EPM gripper.''')
-enums['MAV_CMD'][211].param[1] = '''Gripper number (a number from 1 to max number of grippers on the vehicle).'''
-enums['MAV_CMD'][211].param[2] = '''Gripper action (0=release, 1=grab. See GRIPPER_ACTIONS enum).'''
+enums['MAV_CMD'][211].param[1] = '''Gripper instance number (from 1 to max number of grippers on the vehicle).'''
+enums['MAV_CMD'][211].param[2] = '''Gripper action.'''
 enums['MAV_CMD'][211].param[3] = '''Empty.'''
 enums['MAV_CMD'][211].param[4] = '''Empty.'''
 enums['MAV_CMD'][211].param[5] = '''Empty.'''
 enums['MAV_CMD'][211].param[6] = '''Empty.'''
 enums['MAV_CMD'][211].param[7] = '''Empty.'''
 MAV_CMD_DO_AUTOTUNE_ENABLE = 212 # Enable/disable autotune.
 enums['MAV_CMD'][212] = EnumEntry('MAV_CMD_DO_AUTOTUNE_ENABLE', '''Enable/disable autotune.''')
@@ -1710,27 +1728,26 @@
 enums['MAV_CMD'][42003].param[6] = '''Empty.'''
 enums['MAV_CMD'][42003].param[7] = '''Empty.'''
 MAV_CMD_FIXED_MAG_CAL = 42004 # Magnetometer calibration based on fixed position         in earth
                         # field given by inclination, declination and
                         # intensity.
 enums['MAV_CMD'][42004] = EnumEntry('MAV_CMD_FIXED_MAG_CAL', '''Magnetometer calibration based on fixed position
         in earth field given by inclination, declination and intensity.''')
-enums['MAV_CMD'][42004].param[1] = '''MagDeclinationDegrees.'''
-enums['MAV_CMD'][42004].param[2] = '''MagInclinationDegrees.'''
-enums['MAV_CMD'][42004].param[3] = '''MagIntensityMilliGauss.'''
-enums['MAV_CMD'][42004].param[4] = '''YawDegrees.'''
+enums['MAV_CMD'][42004].param[1] = '''Magnetic declination.'''
+enums['MAV_CMD'][42004].param[2] = '''Magnetic inclination.'''
+enums['MAV_CMD'][42004].param[3] = '''Magnetic intensity.'''
+enums['MAV_CMD'][42004].param[4] = '''Yaw.'''
 enums['MAV_CMD'][42004].param[5] = '''Empty.'''
 enums['MAV_CMD'][42004].param[6] = '''Empty.'''
 enums['MAV_CMD'][42004].param[7] = '''Empty.'''
-MAV_CMD_FIXED_MAG_CAL_FIELD = 42005 # Magnetometer calibration based on fixed expected field values in
-                        # milliGauss.
-enums['MAV_CMD'][42005] = EnumEntry('MAV_CMD_FIXED_MAG_CAL_FIELD', '''Magnetometer calibration based on fixed expected field values in milliGauss.''')
-enums['MAV_CMD'][42005].param[1] = '''FieldX.'''
-enums['MAV_CMD'][42005].param[2] = '''FieldY.'''
-enums['MAV_CMD'][42005].param[3] = '''FieldZ.'''
+MAV_CMD_FIXED_MAG_CAL_FIELD = 42005 # Magnetometer calibration based on fixed expected field values.
+enums['MAV_CMD'][42005] = EnumEntry('MAV_CMD_FIXED_MAG_CAL_FIELD', '''Magnetometer calibration based on fixed expected field values.''')
+enums['MAV_CMD'][42005].param[1] = '''Field strength X.'''
+enums['MAV_CMD'][42005].param[2] = '''Field strength Y.'''
+enums['MAV_CMD'][42005].param[3] = '''Field strength Z.'''
 enums['MAV_CMD'][42005].param[4] = '''Empty.'''
 enums['MAV_CMD'][42005].param[5] = '''Empty.'''
 enums['MAV_CMD'][42005].param[6] = '''Empty.'''
 enums['MAV_CMD'][42005].param[7] = '''Empty.'''
 MAV_CMD_FIXED_MAG_CAL_YAW = 42006 # Magnetometer calibration based on provided known yaw. This allows for
                         # fast calibration using WMM field tables in
                         # the vehicle, given only the known yaw of the
@@ -1742,42 +1759,42 @@
 enums['MAV_CMD'][42006].param[3] = '''Latitude.'''
 enums['MAV_CMD'][42006].param[4] = '''Longitude.'''
 enums['MAV_CMD'][42006].param[5] = '''Empty.'''
 enums['MAV_CMD'][42006].param[6] = '''Empty.'''
 enums['MAV_CMD'][42006].param[7] = '''Empty.'''
 MAV_CMD_DO_START_MAG_CAL = 42424 # Initiate a magnetometer calibration.
 enums['MAV_CMD'][42424] = EnumEntry('MAV_CMD_DO_START_MAG_CAL', '''Initiate a magnetometer calibration.''')
-enums['MAV_CMD'][42424].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+enums['MAV_CMD'][42424].param[1] = '''Bitmask of magnetometers to calibrate. Use 0 to calibrate all sensors that can be started (sensors may not start if disabled, unhealthy, etc.). The command will NACK if calibration does not start for a sensor explicitly specified by the bitmask.'''
 enums['MAV_CMD'][42424].param[2] = '''Automatically retry on failure (0=no retry, 1=retry).'''
 enums['MAV_CMD'][42424].param[3] = '''Save without user input (0=require input, 1=autosave).'''
-enums['MAV_CMD'][42424].param[4] = '''Delay (seconds).'''
+enums['MAV_CMD'][42424].param[4] = '''Delay.'''
 enums['MAV_CMD'][42424].param[5] = '''Autoreboot (0=user reboot, 1=autoreboot).'''
 enums['MAV_CMD'][42424].param[6] = '''Empty.'''
 enums['MAV_CMD'][42424].param[7] = '''Empty.'''
-MAV_CMD_DO_ACCEPT_MAG_CAL = 42425 # Initiate a magnetometer calibration.
-enums['MAV_CMD'][42425] = EnumEntry('MAV_CMD_DO_ACCEPT_MAG_CAL', '''Initiate a magnetometer calibration.''')
-enums['MAV_CMD'][42425].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+MAV_CMD_DO_ACCEPT_MAG_CAL = 42425 # Accept a magnetometer calibration.
+enums['MAV_CMD'][42425] = EnumEntry('MAV_CMD_DO_ACCEPT_MAG_CAL', '''Accept a magnetometer calibration.''')
+enums['MAV_CMD'][42425].param[1] = '''Bitmask of magnetometers that calibration is accepted (0 means all).'''
 enums['MAV_CMD'][42425].param[2] = '''Empty.'''
 enums['MAV_CMD'][42425].param[3] = '''Empty.'''
 enums['MAV_CMD'][42425].param[4] = '''Empty.'''
 enums['MAV_CMD'][42425].param[5] = '''Empty.'''
 enums['MAV_CMD'][42425].param[6] = '''Empty.'''
 enums['MAV_CMD'][42425].param[7] = '''Empty.'''
 MAV_CMD_DO_CANCEL_MAG_CAL = 42426 # Cancel a running magnetometer calibration.
 enums['MAV_CMD'][42426] = EnumEntry('MAV_CMD_DO_CANCEL_MAG_CAL', '''Cancel a running magnetometer calibration.''')
-enums['MAV_CMD'][42426].param[1] = '''uint8_t bitmask of magnetometers (0 means all).'''
+enums['MAV_CMD'][42426].param[1] = '''Bitmask of magnetometers to cancel a running calibration (0 means all).'''
 enums['MAV_CMD'][42426].param[2] = '''Empty.'''
 enums['MAV_CMD'][42426].param[3] = '''Empty.'''
 enums['MAV_CMD'][42426].param[4] = '''Empty.'''
 enums['MAV_CMD'][42426].param[5] = '''Empty.'''
 enums['MAV_CMD'][42426].param[6] = '''Empty.'''
 enums['MAV_CMD'][42426].param[7] = '''Empty.'''
 MAV_CMD_SET_FACTORY_TEST_MODE = 42427 # Command autopilot to get into factory test/diagnostic mode.
 enums['MAV_CMD'][42427] = EnumEntry('MAV_CMD_SET_FACTORY_TEST_MODE', '''Command autopilot to get into factory test/diagnostic mode.''')
-enums['MAV_CMD'][42427].param[1] = '''0 means get out of test mode, 1 means get into test mode.'''
+enums['MAV_CMD'][42427].param[1] = '''0: activate test mode, 1: exit test mode.'''
 enums['MAV_CMD'][42427].param[2] = '''Empty.'''
 enums['MAV_CMD'][42427].param[3] = '''Empty.'''
 enums['MAV_CMD'][42427].param[4] = '''Empty.'''
 enums['MAV_CMD'][42427].param[5] = '''Empty.'''
 enums['MAV_CMD'][42427].param[6] = '''Empty.'''
 enums['MAV_CMD'][42427].param[7] = '''Empty.'''
 MAV_CMD_DO_SEND_BANNER = 42428 # Reply with the version banner.
@@ -1790,15 +1807,15 @@
 enums['MAV_CMD'][42428].param[6] = '''Empty.'''
 enums['MAV_CMD'][42428].param[7] = '''Empty.'''
 MAV_CMD_ACCELCAL_VEHICLE_POS = 42429 # Used when doing accelerometer calibration. When sent to the GCS tells
                         # it what position to put the vehicle in. When
                         # sent to the vehicle says what position the
                         # vehicle is in.
 enums['MAV_CMD'][42429] = EnumEntry('MAV_CMD_ACCELCAL_VEHICLE_POS', '''Used when doing accelerometer calibration. When sent to the GCS tells it what position to put the vehicle in. When sent to the vehicle says what position the vehicle is in.''')
-enums['MAV_CMD'][42429].param[1] = '''Position, one of the ACCELCAL_VEHICLE_POS enum values.'''
+enums['MAV_CMD'][42429].param[1] = '''Position.'''
 enums['MAV_CMD'][42429].param[2] = '''Empty.'''
 enums['MAV_CMD'][42429].param[3] = '''Empty.'''
 enums['MAV_CMD'][42429].param[4] = '''Empty.'''
 enums['MAV_CMD'][42429].param[5] = '''Empty.'''
 enums['MAV_CMD'][42429].param[6] = '''Empty.'''
 enums['MAV_CMD'][42429].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_RESET = 42501 # Causes the gimbal to reset and boot as if it was just powered on.
@@ -1810,15 +1827,15 @@
 enums['MAV_CMD'][42501].param[5] = '''Empty.'''
 enums['MAV_CMD'][42501].param[6] = '''Empty.'''
 enums['MAV_CMD'][42501].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS = 42502 # Reports progress and success or failure of gimbal axis calibration
                         # procedure.
 enums['MAV_CMD'][42502] = EnumEntry('MAV_CMD_GIMBAL_AXIS_CALIBRATION_STATUS', '''Reports progress and success or failure of gimbal axis calibration procedure.''')
 enums['MAV_CMD'][42502].param[1] = '''Gimbal axis we're reporting calibration progress for.'''
-enums['MAV_CMD'][42502].param[2] = '''Current calibration progress for this axis, 0x64=100%.'''
+enums['MAV_CMD'][42502].param[2] = '''Current calibration progress for this axis.'''
 enums['MAV_CMD'][42502].param[3] = '''Status of the calibration.'''
 enums['MAV_CMD'][42502].param[4] = '''Empty.'''
 enums['MAV_CMD'][42502].param[5] = '''Empty.'''
 enums['MAV_CMD'][42502].param[6] = '''Empty.'''
 enums['MAV_CMD'][42502].param[7] = '''Empty.'''
 MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION = 42503 # Starts commutation calibration on the gimbal.
 enums['MAV_CMD'][42503] = EnumEntry('MAV_CMD_GIMBAL_REQUEST_AXIS_CALIBRATION', '''Starts commutation calibration on the gimbal.''')
@@ -1836,18 +1853,18 @@
 enums['MAV_CMD'][42505].param[3] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[4] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[5] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[6] = '''Magic number.'''
 enums['MAV_CMD'][42505].param[7] = '''Magic number.'''
 MAV_CMD_DO_WINCH = 42600 # Command to operate winch.
 enums['MAV_CMD'][42600] = EnumEntry('MAV_CMD_DO_WINCH', '''Command to operate winch.''')
-enums['MAV_CMD'][42600].param[1] = '''Winch number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).'''
-enums['MAV_CMD'][42600].param[2] = '''Action (0=relax, 1=relative length control, 2=rate control. See WINCH_ACTIONS enum.).'''
-enums['MAV_CMD'][42600].param[3] = '''Release length (cable distance to unwind in meters, negative numbers to wind in cable).'''
-enums['MAV_CMD'][42600].param[4] = '''Release rate (meters/second).'''
+enums['MAV_CMD'][42600].param[1] = '''Winch instance number (0 for the default winch, otherwise a number from 1 to max number of winches on the vehicle).'''
+enums['MAV_CMD'][42600].param[2] = '''Action.'''
+enums['MAV_CMD'][42600].param[3] = '''Release length (cable distance to unwind, negative numbers to wind in cable).'''
+enums['MAV_CMD'][42600].param[4] = '''Release rate.'''
 enums['MAV_CMD'][42600].param[5] = '''Empty.'''
 enums['MAV_CMD'][42600].param[6] = '''Empty.'''
 enums['MAV_CMD'][42600].param[7] = '''Empty.'''
 MAV_CMD_FLASH_BOOTLOADER = 42650 # Update the bootloader
 enums['MAV_CMD'][42650] = EnumEntry('MAV_CMD_FLASH_BOOTLOADER', '''Update the bootloader''')
 enums['MAV_CMD'][42650].param[1] = '''Empty'''
 enums['MAV_CMD'][42650].param[2] = '''Empty'''
@@ -1881,16 +1898,62 @@
 enums['MAV_CMD'][42701].param[1] = '''Scripting command to execute'''
 enums['MAV_CMD'][42701].param[2] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[3] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[4] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[5] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[6] = '''Reserved (default:0)'''
 enums['MAV_CMD'][42701].param[7] = '''Reserved (default:0)'''
-MAV_CMD_ENUM_END = 42702 # 
-enums['MAV_CMD'][42702] = EnumEntry('MAV_CMD_ENUM_END', '''''')
+MAV_CMD_GUIDED_CHANGE_SPEED = 43000 # Change flight speed at a given rate. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # speed and the new one. (affects GUIDED only.
+                        # Outside GUIDED, aircraft ignores these
+                        # commands. Designed for onboard companion-
+                        # computer command-and-control, not normally
+                        # operator/GCS control.)
+enums['MAV_CMD'][43000] = EnumEntry('MAV_CMD_GUIDED_CHANGE_SPEED', '''Change flight speed at a given rate. This slews the vehicle at a controllable rate between it's previous speed and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43000].param[1] = '''Airspeed or groundspeed.'''
+enums['MAV_CMD'][43000].param[2] = '''Target Speed'''
+enums['MAV_CMD'][43000].param[3] = '''Acceleration rate, 0 to take effect instantly'''
+enums['MAV_CMD'][43000].param[4] = '''Empty'''
+enums['MAV_CMD'][43000].param[5] = '''Empty'''
+enums['MAV_CMD'][43000].param[6] = '''Empty'''
+enums['MAV_CMD'][43000].param[7] = '''Empty'''
+MAV_CMD_GUIDED_CHANGE_ALTITUDE = 43001 # Change target altitude at a given rate. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # altitude and the new one. (affects GUIDED
+                        # only. Outside GUIDED, aircraft ignores these
+                        # commands. Designed for onboard companion-
+                        # computer command-and-control, not normally
+                        # operator/GCS control.)
+enums['MAV_CMD'][43001] = EnumEntry('MAV_CMD_GUIDED_CHANGE_ALTITUDE', '''Change target altitude at a given rate. This slews the vehicle at a controllable rate between it's previous altitude and the new one. (affects GUIDED only. Outside GUIDED, aircraft ignores these commands. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43001].param[1] = '''Empty'''
+enums['MAV_CMD'][43001].param[2] = '''Empty'''
+enums['MAV_CMD'][43001].param[3] = '''Rate of change, toward new altitude. 0 for maximum rate change. Positive numbers only, as negative numbers will not converge on the new target alt.'''
+enums['MAV_CMD'][43001].param[4] = '''Empty'''
+enums['MAV_CMD'][43001].param[5] = '''Empty'''
+enums['MAV_CMD'][43001].param[6] = '''Empty'''
+enums['MAV_CMD'][43001].param[7] = '''Target Altitude'''
+MAV_CMD_GUIDED_CHANGE_HEADING = 43002 # Change to target heading at a given rate, overriding previous
+                        # heading/s. This slews the vehicle at a
+                        # controllable rate between it's previous
+                        # heading and the new one. (affects GUIDED
+                        # only. Exiting GUIDED returns aircraft to
+                        # normal behaviour defined elsewhere. Designed
+                        # for onboard companion-computer command-and-
+                        # control, not normally operator/GCS control.)
+enums['MAV_CMD'][43002] = EnumEntry('MAV_CMD_GUIDED_CHANGE_HEADING', '''Change to target heading at a given rate, overriding previous heading/s. This slews the vehicle at a controllable rate between it's previous heading and the new one. (affects GUIDED only. Exiting GUIDED returns aircraft to normal behaviour defined elsewhere. Designed for onboard companion-computer command-and-control, not normally operator/GCS control.)''')
+enums['MAV_CMD'][43002].param[1] = '''course-over-ground or raw vehicle heading.'''
+enums['MAV_CMD'][43002].param[2] = '''Target heading.'''
+enums['MAV_CMD'][43002].param[3] = '''Maximum centripetal accelearation, ie rate of change,  toward new heading.'''
+enums['MAV_CMD'][43002].param[4] = '''Empty'''
+enums['MAV_CMD'][43002].param[5] = '''Empty'''
+enums['MAV_CMD'][43002].param[6] = '''Empty'''
+enums['MAV_CMD'][43002].param[7] = '''Empty'''
+MAV_CMD_ENUM_END = 43003 # 
+enums['MAV_CMD'][43003] = EnumEntry('MAV_CMD_ENUM_END', '''''')
 
 # SCRIPTING_CMD
 enums['SCRIPTING_CMD'] = {}
 SCRIPTING_CMD_REPL_START = 0 # Start a REPL session.
 enums['SCRIPTING_CMD'][0] = EnumEntry('SCRIPTING_CMD_REPL_START', '''Start a REPL session.''')
 SCRIPTING_CMD_REPL_STOP = 1 # End a REPL session.
 enums['SCRIPTING_CMD'][1] = EnumEntry('SCRIPTING_CMD_REPL_STOP', '''End a REPL session.''')
@@ -6582,15 +6645,15 @@
         id = MAVLINK_MSG_ID_PID_TUNING
         name = 'PID_TUNING'
         fieldnames = ['axis', 'desired', 'achieved', 'FF', 'P', 'I', 'D']
         ordered_fieldnames = ['desired', 'achieved', 'FF', 'P', 'I', 'D', 'axis']
         fieldtypes = ['uint8_t', 'float', 'float', 'float', 'float', 'float', 'float']
         fielddisplays_by_name = {}
         fieldenums_by_name = {"axis": "PID_TUNING_AXIS"}
-        fieldunits_by_name = {"desired": "deg/s", "achieved": "deg/s"}
+        fieldunits_by_name = {}
         format = '<ffffffB'
         native_format = bytearray('<ffffffB', 'ascii')
         orders = [6, 0, 1, 2, 3, 4, 5]
         lengths = [1, 1, 1, 1, 1, 1, 1]
         array_lengths = [0, 0, 0, 0, 0, 0, 0]
         crc_extra = 98
         unpacker = struct.Struct('<ffffffB')
@@ -15168,31 +15231,31 @@
                 return self.send(self.ekf_status_report_encode(flags, velocity_variance, pos_horiz_variance, pos_vert_variance, compass_variance, terrain_alt_variance, airspeed_variance), force_mavlink1=force_mavlink1)
 
         def pid_tuning_encode(self, axis, desired, achieved, FF, P, I, D):
                 '''
                 PID tuning information.
 
                 axis                      : Axis. (type:uint8_t, values:PID_TUNING_AXIS)
-                desired                   : Desired rate. [deg/s] (type:float)
-                achieved                  : Achieved rate. [deg/s] (type:float)
+                desired                   : Desired rate. (type:float)
+                achieved                  : Achieved rate. (type:float)
                 FF                        : FF component. (type:float)
                 P                         : P component. (type:float)
                 I                         : I component. (type:float)
                 D                         : D component. (type:float)
 
                 '''
                 return MAVLink_pid_tuning_message(axis, desired, achieved, FF, P, I, D)
 
         def pid_tuning_send(self, axis, desired, achieved, FF, P, I, D, force_mavlink1=False):
                 '''
                 PID tuning information.
 
                 axis                      : Axis. (type:uint8_t, values:PID_TUNING_AXIS)
-                desired                   : Desired rate. [deg/s] (type:float)
-                achieved                  : Achieved rate. [deg/s] (type:float)
+                desired                   : Desired rate. (type:float)
+                achieved                  : Achieved rate. (type:float)
                 FF                        : FF component. (type:float)
                 P                         : P component. (type:float)
                 I                         : I component. (type:float)
                 D                         : D component. (type:float)
 
                 '''
                 return self.send(self.pid_tuning_encode(axis, desired, achieved, FF, P, I, D), force_mavlink1=force_mavlink1)
```

### Comparing `pymavlink-2.4.8/dialects/v20/paparazzi.xml` & `pymavlink-2.4.9/dialects/v20/paparazzi.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/python_array_test.py` & `pymavlink-2.4.9/dialects/v20/python_array_test.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/test.xml` & `pymavlink-2.4.9/dialects/v20/test.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/icarous.py` & `pymavlink-2.4.9/dialects/v20/icarous.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/minimal.xml` & `pymavlink-2.4.9/dialects/v20/minimal.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/test.py` & `pymavlink-2.4.9/dialects/v20/test.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/autoquad.py` & `pymavlink-2.4.9/dialects/v20/autoquad.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/standard.py` & `pymavlink-2.4.9/dialects/v20/standard.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/common.xml` & `pymavlink-2.4.9/dialects/v20/common.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/slugs.py` & `pymavlink-2.4.9/dialects/v20/slugs.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/dialects/v20/autoquad.xml` & `pymavlink-2.4.9/dialects/v20/autoquad.xml`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/mavextra.py` & `pymavlink-2.4.9/mavextra.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/README.md` & `pymavlink-2.4.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 # Pymavlink
 This is a python implementation of the MAVLink protocol.
 It includes a source code generator (generator/mavgen.py) to create MAVLink protocol implementations for other programming languages as well.
 Also contains tools for analizing flight logs.
 
 # Documentation
 
-Please see http://ardupilot.org/dev/docs/mavlink-commands.html for documentation.
+Please see http://ardupilot.org/dev/docs/mavlink-commands.html for mavlink command reference.
 
-For realtime discussion please see the pymavlink gitter channel here
-https://gitter.im/ArduPilot/pymavlink
+For realtime discussion please see the pymavlink [gitter channel](https://gitter.im/ArduPilot/pymavlink)
+
+Examples can be found [in the repository](examples/) or in the [ArduSub book](https://www.ardusub.com/developers/pymavlink.html)
 
 
 # Installation 
 
 Pymavlink supports both python2 and python3.
 
 The following instructions assume you are using Python 2 and a Debian-based (like Ubuntu) installation.
 
 ## Dependencies
 
 Pymavlink has several dependencies :
 
-    - future : for python 2 and python 3 interoperability (http://python-future.org/)
-    - lxml : for checking and parsing xml file (http://lxml.de/installation.html)
+    - [future](http://python-future.org/) : for python 2 and python 3 interoperability 
+    - [lxml](http://lxml.de/installation.html) : for checking and parsing xml file 
     - python-dev : for mavnative
     - a C compiler : for mavnative
 
 Optional :
 
     - numpy : for FFT
     - pytest : for tests
@@ -79,36 +80,29 @@
 
 ```bash
 sudo DISABLE_MAVNATIVE=True pip2 install -U pymavlink
 ```
 
 ### For developers
 
-On the pymavlink directory, you can use :
+From the pymavlink directory, you can use :
 
 ```bash
 sudo MDEF=PATH_TO_message_definitions pip2 install . -v
 ```
 
-The -v parameter will output the installation commands on the terminal.
-The MDEF usage is require as pip install is done from /tmp directory, so it is necessary to use MDEF variable to 
-point on the message_definitions directory.
-Use pip should auto install dependencies and allow to keep them up-to-date with pip. 
+Since pip installation is executed from /tmp, it is necessary to point to the directory containing message definitions with MDEF. MDEF should not be set to any particular message version directory but the parent folder instead. If you have cloned from mavlink/mavlink then this is ```/mavlink/message_definitions``` . Using pip should auto install dependencies and allow you to keep them up-to-date. 
 
 Or:
 
 ```bash
 sudo python2 setup.py install
 ```
 
 
-### Advanced usage
-
-Please see Pip documentation : https://pip.pypa.io/en/stable/
-
 # License
 ---------
 
 pymavlink is released under the GNU Lesser General Public License v3 or later.
 
 The source code generated by generator/mavgen.py is available under the permissive MIT License.
```

### Comparing `pymavlink-2.4.8/mavutil.py` & `pymavlink-2.4.9/mavutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,17 +639,25 @@
         if isinstance(mode, str):
             mode_map = self.mode_mapping()
             if mode_map is None or mode not in mode_map:
                 print("Unknown mode '%s'" % mode)
                 return
             mode = mode_map[mode]
         # set mode by integer mode number for ArduPilot
-        self.mav.set_mode_send(self.target_system,
-                               mavlink.MAV_MODE_FLAG_CUSTOM_MODE_ENABLED,
-                               mode)
+        self.mav.command_long_send(self.target_system,
+                                   self.target_component,
+                                   mavlink.MAV_CMD_DO_SET_MODE,
+                                   0,
+                                   mavlink.MAV_MODE_FLAG_CUSTOM_MODE_ENABLED,
+                                   mode,
+                                   0,
+                                   0,
+                                   0,
+                                   0,
+                                   0)
 
     def set_mode_px4(self, mode, custom_mode, custom_sub_mode):
         '''enter arbitrary mode'''
         if isinstance(mode, str):
             mode_map = self.mode_mapping()
             if mode_map is None or mode not in mode_map:
                 print("Unknown mode '%s'" % mode)
@@ -754,19 +762,14 @@
             if hold_in_bootloader:
                 param1 = 3
             else:
                 param1 = 1
             self.mav.command_long_send(self.target_system, self.target_component,
                                        mavlink.MAV_CMD_PREFLIGHT_REBOOT_SHUTDOWN, 0,
                                        param1, 0, 0, 0, 0, 0, 0)
-            # send an old style reboot immediately afterwards in case it is an older firmware
-            # that doesn't understand the new convention
-            self.mav.command_long_send(self.target_system, self.target_component,
-                                       mavlink.MAV_CMD_PREFLIGHT_REBOOT_SHUTDOWN, 0,
-                                       1, 0, 0, 0, 0, 0, 0)
 
     def wait_gps_fix(self):
         self.recv_match(type='VFR_HUD', blocking=True)
         if self.mavlink10():
             self.recv_match(type='GPS_RAW_INT', blocking=True,
                             condition='GPS_RAW_INT.fix_type>=3 and GPS_RAW_INT.lat != 0')
         else:
```

### Comparing `pymavlink-2.4.8/mavexpression.py` & `pymavlink-2.4.9/mavexpression.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/mavnative/mavnative.c` & `pymavlink-2.4.9/mavnative/mavnative.c`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/pymavlink.egg-info/SOURCES.txt` & `pymavlink-2.4.9/pymavlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/pymavlink.egg-info/PKG-INFO` & `pymavlink-2.4.9/pymavlink.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymavlink
-Version: 2.4.8
+Version: 2.4.9
 Summary: Python MAVLink code
 Home-page: https://github.com/ArduPilot/pymavlink/
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: LGPLv3
 Description: A Python library for handling MAVLink protocol streams and log files. This allows for the creation of simple scripts to analyse telemetry logs from autopilots such as ArduPilot which use the MAVLink protocol. See the scripts that come with the package for examples of small, useful scripts that use pymavlink. For more information about the MAVLink protocol see https://mavlink.io/en/
 Platform: UNKNOWN
```

### Comparing `pymavlink-2.4.8/generator/mavgen_wlua.py` & `pymavlink-2.4.9/generator/mavgen_wlua.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_java.py` & `pymavlink-2.4.9/generator/mavgen_java.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_swift.py` & `pymavlink-2.4.9/generator/mavgen_swift.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_cs.py` & `pymavlink-2.4.9/generator/mavgen_cs.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_lua.py` & `pymavlink-2.4.9/generator/mavgen_lua.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavparse.py` & `pymavlink-2.4.9/generator/mavparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         self.name_lower = name.lower()
         self.linenumber = linenumber
         self.id = int(id)
         self.description = description
         self.fields = []
         self.fieldnames = []
         self.extensions_start = None
+        self.needs_pack = False
 
     def base_fields(self):
         '''return number of non-extended fields'''
         if self.extensions_start is None:
             return len(self.fields)
         return len(self.fields[:self.extensions_start])
 
@@ -322,17 +323,15 @@
         f.close()
    
 
         #Post process to add reserved params (for docs)
         for current_enum in self.enum:
             if not 'MAV_CMD' in current_enum.name:
                 continue
-            print(current_enum.name)
             for enum_entry in current_enum.entry:
-                print(enum_entry.name)
                 if len(enum_entry.param) == 7:
                     continue
                 params_dict=dict()
                 for param_index in range (1,8):
                     params_dict[param_index] = MAVEnumParam(param_index, label='', units='', enum='', increment='', 
                                                         minValue='', maxValue='', default='0', reserved='True')
 
@@ -395,14 +394,20 @@
                 else:
                     m.fieldlengths.append(L)
                 m.fieldtypes.append(f.type)
             for i in range(len(m.ordered_fields)):
                 f = m.ordered_fields[i]
                 f.wire_offset = m.wire_length
                 m.wire_length += f.wire_length
+                field_el_length = f.wire_length
+                if f.array_length > 1:
+                    field_el_length = f.wire_length / f.array_length
+                if f.wire_offset % field_el_length != 0:
+                    # misaligned field, structure will need packing in C
+                    m.needs_pack = True
                 if m.extensions_start is None or i < m.extensions_start:
                     m.wire_min_length = m.wire_length
                 m.ordered_fieldnames.append(f.name)
                 m.ordered_fieldtypes.append(f.type)
                 f.set_test_value()
                 if f.name.find('[') != -1:
                     raise MAVParseError("invalid field name with array descriptor %s" % f.name)
@@ -427,17 +432,14 @@
             self.message_flags[key] = m.message_flags
             self.message_target_system_ofs[key] = m.target_system_ofs
             self.message_target_component_ofs[key] = m.target_component_ofs
 
             if m.wire_length > self.largest_payload:
                 self.largest_payload = m.wire_length
 
-            if m.wire_length+8 > 64:
-                print("Note: message %s is longer than 64 bytes long (%u bytes), which can cause fragmentation since many radio modems use 64 bytes as maximum air transfer unit." % (m.name, m.wire_length+8))
-
     def __str__(self):
         return "MAVXML for %s from %s (%u message, %u enums)" % (
             self.basename, self.filename, len(self.message), len(self.enum))
 
 
 def message_checksum(msg):
     '''calculate a 8-bit checksum of the key fields of a message, so we
```

### Comparing `pymavlink-2.4.8/generator/mavgen_c.py` & `pymavlink-2.4.9/generator/mavgen_c.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,19 +173,19 @@
     f = open(os.path.join(directory, 'mavlink_msg_%s.h' % m.name_lower), mode='w')
     t.write(f, '''
 #pragma once
 // MESSAGE ${name} PACKING
 
 #define MAVLINK_MSG_ID_${name} ${id}
 
-MAVPACKED(
+${MAVPACKED_START}
 typedef struct __mavlink_${name_lower}_t {
 ${{ordered_fields: ${type} ${name}${array_suffix}; /*< ${units} ${description}*/
 }}
-}) mavlink_${name_lower}_t;
+}${MAVPACKED_END} mavlink_${name_lower}_t;
 
 #define MAVLINK_MSG_ID_${name}_LEN ${wire_length}
 #define MAVLINK_MSG_ID_${name}_MIN_LEN ${wire_min_length}
 #define MAVLINK_MSG_ID_${id}_LEN ${wire_length}
 #define MAVLINK_MSG_ID_${id}_MIN_LEN ${wire_min_length}
 
 #define MAVLINK_MSG_ID_${name}_CRC ${crc_extra}
@@ -670,14 +670,20 @@
                     f.c_test_value = "'%s'" % f.test_value
                 elif f.type == 'uint64_t':
                     f.c_test_value = "%sULL" % f.test_value                    
                 elif f.type == 'int64_t':
                     f.c_test_value = "%sLL" % f.test_value                    
                 else:
                     f.c_test_value = f.test_value
+        if m.needs_pack:
+            m.MAVPACKED_START = "MAVPACKED("
+            m.MAVPACKED_END = ")"
+        else:
+            m.MAVPACKED_START = ""
+            m.MAVPACKED_END = ""
 
     # cope with uint8_t_mavlink_version
     for m in xml.message:
         m.arg_fields = []
         m.array_fields = []
         m.scalar_fields = []
         for f in m.ordered_fields:
```

### Comparing `pymavlink-2.4.8/generator/mavschema.xsd` & `pymavlink-2.4.9/generator/mavschema.xsd`

 * *Files 0% similar despite different names*

#### Comparing `pymavlink-2.4.8/generator/mavschema.xsd` & `pymavlink-2.4.9/generator/mavschema.xsd`

```diff
@@ -176,14 +176,17 @@
       <xs:enumeration value="gauss"/>
       <!-- Gauss -->
       <xs:enumeration value="mgauss"/>
       <!-- milli-Gauss -->
       <!-- energy -->
       <xs:enumeration value="hJ"/>
       <!-- hecto-Joule -->
+      <!-- power -->
+      <xs:enumeration value="W"/>
+      <!-- Watt -->
       <!-- force -->
       <xs:enumeration value="mG"/>
       <!-- milli-G -->
       <!-- mass -->
       <xs:enumeration value="g"/>
       <!-- grams -->
       <!-- pressure -->
@@ -308,23 +311,25 @@
       </xs:sequence>
       <xs:attribute ref="value"/>
       <xs:attribute ref="name" use="required"/>
       <xs:attribute ref="hasLocation"/>
       <xs:attribute ref="isDestination"/>
     </xs:complexType>
   </xs:element>
+  <!-- definition entry elements attributes (like the ones used on MAV_CMD for example) -->
+  <xs:attribute name="bitmask" type="xs:boolean" default="false"/>
   <xs:element name="enum">
     <xs:complexType>
       <xs:sequence>
         <xs:element ref="deprecated" minOccurs="0" maxOccurs="1"/>
         <xs:element ref="description" minOccurs="0"/>
         <xs:element ref="entry" maxOccurs="unbounded"/>
       </xs:sequence>
       <xs:attribute ref="name" use="required"/>
-      <xs:attribute ref="bitmask" type="xs:boolean" default="false"/>
+      <xs:attribute ref="bitmask"/>
     </xs:complexType>
   </xs:element>
   <xs:element name="message">
     <xs:complexType>
       <xs:sequence>
         <xs:sequence minOccurs="1" maxOccurs="1">
           <xs:choice minOccurs="0" maxOccurs="1">
```

### Comparing `pymavlink-2.4.8/generator/mavtestgen.py` & `pymavlink-2.4.9/generator/mavtestgen.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen.py` & `pymavlink-2.4.9/generator/mavgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         except ImportError:
             print("WARNING: Failed to import lxml module etree. Are lxml, libxml2 and libxslt installed? XML validation will not be performed", file=sys.stderr)
             opts.validate = False
         except etree.XMLSyntaxError as err:
             print("WARNING: XML Syntax Errors detected in %s XML schema file. XML validation will not be performed" % schemaFile, file=sys.stderr)
             print(str(err.error_log), file=sys.stderr)
             opts.validate = False
-        except:
+        except Exception as e:
+            print("Exception:", e)
             print("WARNING: Unable to load XML validator libraries. XML validation will not be performed", file=sys.stderr)
             opts.validate = False
 
     def expand_includes():
         """Expand includes in current list of all files, ignoring those already parsed."""
         for x in xml[:]:
             for i in x.include:
```

### Comparing `pymavlink-2.4.8/generator/mavgen_objc.py` & `pymavlink-2.4.9/generator/mavgen_objc.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_cpp11.py` & `pymavlink-2.4.9/generator/mavgen_cpp11.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/mavlink_get_info.h` & `pymavlink-2.4.9/generator/C/include_v2.0/mavlink_get_info.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/mavlink_helpers.h` & `pymavlink-2.4.9/generator/C/include_v2.0/mavlink_helpers.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/protocol.h` & `pymavlink-2.4.9/generator/C/include_v2.0/protocol.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/mavlink_conversions.h` & `pymavlink-2.4.9/generator/C/include_v2.0/mavlink_conversions.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/mavlink_types.h` & `pymavlink-2.4.9/generator/C/include_v2.0/mavlink_types.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/mavlink_sha256.h` & `pymavlink-2.4.9/generator/C/include_v2.0/mavlink_sha256.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v2.0/checksum.h` & `pymavlink-2.4.9/generator/C/include_v2.0/checksum.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v1.0/mavlink_helpers.h` & `pymavlink-2.4.9/generator/C/include_v1.0/mavlink_helpers.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v1.0/protocol.h` & `pymavlink-2.4.9/generator/C/include_v1.0/protocol.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v1.0/mavlink_conversions.h` & `pymavlink-2.4.9/generator/C/include_v1.0/mavlink_conversions.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v1.0/mavlink_types.h` & `pymavlink-2.4.9/generator/C/include_v1.0/mavlink_types.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/C/include_v1.0/checksum.h` & `pymavlink-2.4.9/generator/C/include_v1.0/checksum.h`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/java/lib/Parser.java` & `pymavlink-2.4.9/generator/java/lib/Parser.java`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkMessage.java` & `pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkMessage.java`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkStats.java` & `pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkStats.java`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/java/lib/Messages/MAVLinkPayload.java` & `pymavlink-2.4.9/generator/java/lib/Messages/MAVLinkPayload.java`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_javascript.py` & `pymavlink-2.4.9/generator/mavgen_javascript.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavtemplate.py` & `pymavlink-2.4.9/generator/mavtemplate.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_python.py` & `pymavlink-2.4.9/generator/mavgen_python.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/CS/common/Mavlink.cs` & `pymavlink-2.4.9/generator/CS/common/Mavlink.cs`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/CS/common/ByteArrayUtil.cs` & `pymavlink-2.4.9/generator/CS/common/ByteArrayUtil.cs`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/CS/common/FrameworkBitConverter.cs` & `pymavlink-2.4.9/generator/CS/common/FrameworkBitConverter.cs`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/swift/MAVLink.swift` & `pymavlink-2.4.9/generator/swift/MAVLink.swift`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavcrc.py` & `pymavlink-2.4.9/generator/mavcrc.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/mavgen_typescript.py` & `pymavlink-2.4.9/generator/mavgen_typescript.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/CPP11/include_v2.0/message.hpp` & `pymavlink-2.4.9/generator/CPP11/include_v2.0/message.hpp`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/generator/CPP11/include_v2.0/msgmap.hpp` & `pymavlink-2.4.9/generator/CPP11/include_v2.0/msgmap.hpp`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavflightmodes.py` & `pymavlink-2.4.9/tools/mavflightmodes.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavflighttime.py` & `pymavlink-2.4.9/tools/mavflighttime.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavsummarize.py` & `pymavlink-2.4.9/tools/mavsummarize.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavtomfile.py` & `pymavlink-2.4.9/tools/mavtomfile.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/magfit_delta.py` & `pymavlink-2.4.9/tools/magfit_delta.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavmission.py` & `pymavlink-2.4.9/tools/mavmission.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavfft_isb.py` & `pymavlink-2.4.9/tools/mavfft_isb.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavlogdump.py` & `pymavlink-2.4.9/tools/mavlogdump.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/magfit_WMM.py` & `pymavlink-2.4.9/tools/magfit_WMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,18 @@
     return c
 
 def remove_offsets(MAG, BAT, c):
     '''remove all corrections to get raw sensor data'''
     correction_matrix = Matrix3(Vector3(c.diag.x,    c.offdiag.x, c.offdiag.y),
                                 Vector3(c.offdiag.x, c.diag.y,    c.offdiag.z),
                                 Vector3(c.offdiag.y, c.offdiag.z, c.diag.z))
-    correction_matrix = correction_matrix.invert()
+    try:
+        correction_matrix = correction_matrix.invert()
+    except Exception:
+        return False
 
     field = Vector3(MAG.MagX, MAG.MagY, MAG.MagZ)
     if BAT is not None and not math.isnan(BAT.Curr):
         field -= c.cmot * BAT.Curr
     field = correction_matrix * field
     field *= 1.0 / c.scaling
     field -= Vector3(MAG.OfsX, MAG.OfsY, MAG.OfsZ)
@@ -276,14 +279,16 @@
 
     old_corrections.offsets = Vector3(parameters.get('COMPASS_OFS%s_X' % mag_idx,0.0),
                                       parameters.get('COMPASS_OFS%s_Y' % mag_idx,0.0),
                                       parameters.get('COMPASS_OFS%s_Z' % mag_idx,0.0))
     old_corrections.diag = Vector3(parameters.get('COMPASS_DIA%s_X' % mag_idx,1.0),
                                    parameters.get('COMPASS_DIA%s_Y' % mag_idx,1.0),
                                    parameters.get('COMPASS_DIA%s_Z' % mag_idx,1.0))
+    if old_corrections.diag == Vector3(0,0,0):
+        old_corrections.diag = Vector3(1,1,1)
     old_corrections.offdiag = Vector3(parameters.get('COMPASS_ODI%s_X' % mag_idx,0.0),
                                       parameters.get('COMPASS_ODI%s_Y' % mag_idx,0.0),
                                       parameters.get('COMPASS_ODI%s_Z' % mag_idx,0.0))
     if parameters.get('COMPASS_MOTCT',0) == 2:
         # only support current based corrections for now
         old_corrections.cmot = Vector3(parameters.get('COMPASS_MOT%s_X' % mag_idx,0.0),
                                        parameters.get('COMPASS_MOT%s_Y' % mag_idx,0.0),
@@ -301,14 +306,16 @@
         if remove_offsets(MAG, BAT, old_corrections):
             data2.append((MAG,ATT,BAT))
     data = data2
 
     print("Extracted %u points" % len(data))
     print("Current: %s diag: %s offdiag: %s cmot: %s scale: %.2f" % (
         old_corrections.offsets, old_corrections.diag, old_corrections.offdiag, old_corrections.cmot, old_corrections.scaling))
+    if len(data) == 0:
+        return
 
     # do fit
     c = fit_WWW()
 
     # normalise diagonals to scale factor
     if force_scale:
         avgdiag = (c.diag.x + c.diag.y + c.diag.z)/3.0
```

### Comparing `pymavlink-2.4.8/tools/mavloss.py` & `pymavlink-2.4.9/tools/mavloss.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavgen.py` & `pymavlink-2.4.9/tools/mavgen.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavlink_bitmask_decoder.py` & `pymavlink-2.4.9/tools/mavlink_bitmask_decoder.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavkml.py` & `pymavlink-2.4.9/tools/mavkml.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavextract.py` & `pymavlink-2.4.9/tools/mavextract.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavparmdiff.py` & `pymavlink-2.4.9/tools/mavparmdiff.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/magfit.py` & `pymavlink-2.4.9/tools/magfit.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavparms.py` & `pymavlink-2.4.9/tools/mavparms.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavgpslock.py` & `pymavlink-2.4.9/tools/mavgpslock.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavfft.py` & `pymavlink-2.4.9/tools/mavfft.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavtogpx.py` & `pymavlink-2.4.9/tools/mavtogpx.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/magfit_motors.py` & `pymavlink-2.4.9/tools/magfit_motors.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavsigloss.py` & `pymavlink-2.4.9/tools/mavsigloss.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavgraph.py` & `pymavlink-2.4.9/tools/mavgraph.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavplayback.py` & `pymavlink-2.4.9/tools/mavplayback.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/magfit_gps.py` & `pymavlink-2.4.9/tools/magfit_gps.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/mavsearch.py` & `pymavlink-2.4.9/tools/mavsearch.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/tools/MPU6KSearch.py` & `pymavlink-2.4.9/tools/MPU6KSearch.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/DFReader.py` & `pymavlink-2.4.9/DFReader.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/quaternion.py` & `pymavlink-2.4.9/quaternion.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/PKG-INFO` & `pymavlink-2.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymavlink
-Version: 2.4.8
+Version: 2.4.9
 Summary: Python MAVLink code
 Home-page: https://github.com/ArduPilot/pymavlink/
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: LGPLv3
 Description: A Python library for handling MAVLink protocol streams and log files. This allows for the creation of simple scripts to analyse telemetry logs from autopilots such as ArduPilot which use the MAVLink protocol. See the scripts that come with the package for examples of small, useful scripts that use pymavlink. For more information about the MAVLink protocol see https://mavlink.io/en/
 Platform: UNKNOWN
```

### Comparing `pymavlink-2.4.8/rotmat.py` & `pymavlink-2.4.9/rotmat.py`

 * *Files identical despite different names*

### Comparing `pymavlink-2.4.8/fgFDM.py` & `pymavlink-2.4.9/fgFDM.py`

 * *Files identical despite different names*

