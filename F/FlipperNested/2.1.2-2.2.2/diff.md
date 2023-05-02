# Comparing `tmp/FlipperNested-2.1.2.tar.gz` & `tmp/FlipperNested-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.1.2.tar", last modified: Sun Apr 30 14:45:46 2023, max compression
+gzip compressed data, was "FlipperNested-2.2.2.tar", last modified: Mon May  1 21:50:21 2023, max compression
```

## Comparing `FlipperNested-2.1.2.tar` & `FlipperNested-2.2.2.tar`

### file list

```diff
@@ -1,96 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.587293 FlipperNested-2.1.2/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.591293 FlipperNested-2.1.2/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.587293 FlipperNested-2.1.2/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.591293 FlipperNested-2.1.2/HardNestedSolver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/bucketsort.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/bucketsort.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    87569 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crapto1.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crapto1.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crypto1.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.599293 FlipperNested-2.1.2/HardNestedSolver/hardnested/
--rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    20997 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    24142 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_tables.c
--rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/library.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/library.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/parity.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.603293 FlipperNested-2.1.2/HardNestedSolver/pm3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3252 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ansi.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5556 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/common.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6876 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35936 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/comms.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/comms.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5824 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.h
--rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/emojis.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/emojis_alt.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    39500 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     9687 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    30683 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/pm3_cmd.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.603293 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    12654 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_win32.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    24666 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ui.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ui.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35946 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7580 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2874 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.m
--rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.472744 FlipperNested-2.2.2/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.476744 FlipperNested-2.2.2/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.472744 FlipperNested-2.2.2/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 21:50:21.000000 FlipperNested-2.2.2/FlipperNested.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.476744 FlipperNested-2.2.2/HardNestedSolver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/bucketsort.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/bucketsort.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    85176 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/cmdhfmfhard.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/cmdhfmfhard.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/crapto1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/crapto1.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/crypto1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.480744 FlipperNested-2.2.2/HardNestedSolver/hardnested/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bf_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bf_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19427 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bruteforce.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bruteforce.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/hardnested/tables.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/library.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/library.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/parity.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/HardNestedSolver/pm3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1608 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/ansi.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3405 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/commonutil.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/commonutil.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/emojis.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/emojis_alt.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13770 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/ui.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/ui.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/util.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/util.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/util_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/pm3/util_posix.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/HardNestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:50:21.484744 FlipperNested-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 21:50:12.000000 FlipperNested-2.2.2/tests/test_parse.py
```

### Comparing `FlipperNested-2.1.2/FlipperNested/bridge.py` & `FlipperNested-2.2.2/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/FlipperNested/cli.py` & `FlipperNested-2.2.2/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/FlipperNested/main.py` & `FlipperNested-2.2.2/FlipperNested/main.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-2.2.2/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/FlipperNested/proto/storage_pb2.py` & `FlipperNested-2.2.2/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-2.2.2/FlipperNested.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.1.2
+Version: 2.2.2
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.1.2/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-2.2.2/FlipperNested.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -30,48 +30,28 @@
 HardNestedSolver/hardnested/hardnested_benchmark_data.h
 HardNestedSolver/hardnested/hardnested_bf_core.c
 HardNestedSolver/hardnested/hardnested_bf_core.h
 HardNestedSolver/hardnested/hardnested_bitarray_core.c
 HardNestedSolver/hardnested/hardnested_bitarray_core.h
 HardNestedSolver/hardnested/hardnested_bruteforce.c
 HardNestedSolver/hardnested/hardnested_bruteforce.h
-HardNestedSolver/hardnested/hardnested_tables.c
 HardNestedSolver/hardnested/tables.c
 HardNestedSolver/hardnested/tables.h
 HardNestedSolver/pm3/ansi.h
 HardNestedSolver/pm3/common.h
 HardNestedSolver/pm3/commonutil.c
 HardNestedSolver/pm3/commonutil.h
-HardNestedSolver/pm3/comms.c
-HardNestedSolver/pm3/comms.h
-HardNestedSolver/pm3/crc.c
-HardNestedSolver/pm3/crc.h
-HardNestedSolver/pm3/crc16.c
-HardNestedSolver/pm3/crc16.h
-HardNestedSolver/pm3/crc32.c
-HardNestedSolver/pm3/crc32.h
-HardNestedSolver/pm3/crc64.c
-HardNestedSolver/pm3/crc64.h
 HardNestedSolver/pm3/emojis.h
 HardNestedSolver/pm3/emojis_alt.h
-HardNestedSolver/pm3/fileutils.c
-HardNestedSolver/pm3/fileutils.h
-HardNestedSolver/pm3/pm3_cmd.h
 HardNestedSolver/pm3/ui.c
 HardNestedSolver/pm3/ui.h
 HardNestedSolver/pm3/util.c
 HardNestedSolver/pm3/util.h
-HardNestedSolver/pm3/util_darwin.h
-HardNestedSolver/pm3/util_darwin.m
 HardNestedSolver/pm3/util_posix.c
 HardNestedSolver/pm3/util_posix.h
-HardNestedSolver/pm3/uart/README.md
-HardNestedSolver/pm3/uart/uart.h
-HardNestedSolver/pm3/uart/uart_posix.c
-HardNestedSolver/pm3/uart/uart_win32.c
 NestedSolver/bucketsort.c
 NestedSolver/bucketsort.h
 NestedSolver/crapto1.c
 NestedSolver/crapto1.h
 NestedSolver/crypto1.c
 NestedSolver/library.c
 NestedSolver/library.h
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/bucketsort.c` & `FlipperNested-2.2.2/HardNestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/bucketsort.h` & `FlipperNested-2.2.2/HardNestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.c` & `FlipperNested-2.2.2/HardNestedSolver/cmdhfmfhard.c`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 #include "crapto1.h"
 #include "parity.h"
 #include "hardnested/hardnested_bruteforce.h"
 #include "hardnested/hardnested_bf_core.h"
 #include "hardnested/hardnested_bitarray_core.h"
 #include "pm3/ui.h"
-#include "pm3/fileutils.h"
 #include "pm3/commonutil.h"
 #include "pm3/util_posix.h"
 #include "hardnested/tables.h"
 #include <lzma.h>
 
 #define NUM_CHECK_BITFLIPS_THREADS      (num_CPUs())
 #if defined(_MSC_VER)
@@ -980,79 +979,14 @@
                 qsort(nonces[i].sum_a8_guess, NUM_SUMS, sizeof(guess_sum_a8_t), compare_sum_a8_guess);
                 nonces[i].sum_a8_guess_dirty = false;
             }
         }
     }
 }
 
-static int read_nonce_file(char *filename) {
-
-    if (filename == NULL) {
-        PrintAndLogEx(WARNING, "Filename is NULL");
-        return PM3_EINVARG;
-    }
-    FILE *fnonces = NULL;
-    char progress_text[80] = "";
-    uint8_t read_buf[9];
-
-    num_acquired_nonces = 0;
-    if ((fnonces = fopen(filename, "rb")) == NULL) {
-        PrintAndLogEx(WARNING, "Could not open file "
-                               _YELLOW_("%s"), filename);
-        return PM3_EFILE;
-    }
-
-    snprintf(progress_text, 80, "Reading nonces from file "
-                                _YELLOW_("%s"), filename);
-    hardnested_print_progress(0, progress_text, (float) (1LL << 47), 0);
-    size_t bytes_read = fread(read_buf, 1, 6, fnonces);
-    if (bytes_read != 6) {
-        PrintAndLogEx(ERR, "File reading error.");
-        fclose(fnonces);
-        return PM3_EFILE;
-    }
-    cuid = bytes_to_num(read_buf, 4);
-    uint8_t trgBlockNo = bytes_to_num(read_buf + 4, 1);
-    uint8_t trgKeyType = bytes_to_num(read_buf + 5, 1);
-
-    bytes_read = fread(read_buf, 1, 9, fnonces);
-    while (bytes_read == 9) {
-        uint32_t nt_enc1 = bytes_to_num(read_buf, 4);
-        uint32_t nt_enc2 = bytes_to_num(read_buf + 4, 4);
-        uint8_t par_enc = bytes_to_num(read_buf + 8, 1);
-        add_nonce(nt_enc1, par_enc >> 4);
-        add_nonce(nt_enc2, par_enc & 0x0f);
-        num_acquired_nonces += 2;
-        bytes_read = fread(read_buf, 1, 9, fnonces);
-    }
-    fclose(fnonces);
-
-    char progress_string[80];
-    snprintf(progress_string, sizeof(progress_string), "Read %u nonces from file. cuid = %08x", num_acquired_nonces,
-             cuid);
-    hardnested_print_progress(num_acquired_nonces, progress_string, (float) (1LL << 47), 0);
-    snprintf(progress_string, sizeof(progress_string), "Target Block=%d, Keytype=%c", trgBlockNo,
-             trgKeyType == 0 ? 'A' : 'B');
-    hardnested_print_progress(num_acquired_nonces, progress_string, (float) (1LL << 47), 0);
-
-    bool got_match = false;
-    for (uint8_t i = 0; i < NUM_SUMS; i++) {
-        if (first_byte_Sum == sums[i]) {
-            first_byte_Sum = i;
-            got_match = true;
-            break;
-        }
-    }
-    if (got_match == false) {
-        PrintAndLogEx(FAILED, "No match for the First_Byte_Sum (%u), is the card a genuine MFC Ev1? ", first_byte_Sum);
-        return PM3_ESOFT;
-    }
-    return 0;
-}
-
 static noncelistentry_t *SearchFor2ndByte(uint8_t b1, uint8_t b2) {
     noncelistentry_t *p = nonces[b1].first;
     while (p != NULL) {
         if ((p->nonce_enc >> 16 & 0xff) == b2) {
             return p;
         }
         p = p->next;
@@ -1258,14 +1192,15 @@
         uint8_t par_enc = 0;
 
         if (fgets(line, sizeof(line), fp) != NULL) {
             sscanf(line, "%u|%hhu", &nt_enc, &par_enc);
             num_acquired_nonces += add_nonce(nt_enc, par_enc);
             total_num_nonces++;
         }
+
         if (num_acquired_nonces % 256 == 0) {
             hardnested_print_progress(num_acquired_nonces, "Loading nonces from file", brute_force_depth, 0);
         }
 
         last_sample_clock = msclock();
 
         if (first_byte_num == 256) {
@@ -1279,15 +1214,15 @@
                         break;
                     }
                 }
 
                 if (got_match == false) {
                     PrintAndLogEx(FAILED, "No match for the First_Byte_Sum (%u), is the card a genuine MFC Ev1? ",
                                   first_byte_Sum);
-                    return PM3_ESOFT;
+                    return -1;
                 }
 
                 hardnested_stage |= CHECK_2ND_BYTES;
                 apply_sum_a0();
             }
             update_nonce_data(true);
             acquisition_completed = shrink_key_space(&brute_force_depth);
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.h` & `FlipperNested-2.2.2/HardNestedSolver/cmdhfmfhard.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/crapto1.c` & `FlipperNested-2.2.2/HardNestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/crapto1.h` & `FlipperNested-2.2.2/HardNestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/crypto1.c` & `FlipperNested-2.2.2/HardNestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.c` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bf_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.h` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bf_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.c` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bruteforce.c`

 * *Files 6% similar despite different names*

```diff
@@ -52,37 +52,31 @@
 #include <inttypes.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <pthread.h>
 #include <string.h>
 #include <stdlib.h>
 
-//#include "../pm3/common.h"
-//#include "../cmdhfmfhard.h"
 #include "hardnested_bf_core.h"
 #include "../pm3/ui.h"
-//#include "../pm3/util.h"
 #include "../pm3/util_posix.h"
 #include "../crapto1.h"
 #include "../parity.h"
 #include "../cmdhfmfhard.h"
-//#include "../pm3/fileutils.h"
-//#include "../pm3/pm3_cmd.h"
 #include "hardnested_benchmark_data.h"
 
 #define NUM_BRUTE_FORCE_THREADS         (num_CPUs())
 #ifdef _WIN32
     #define NUM_BRUTE_FORCE_THREADS_ALLOC   128
 #else
     #define NUM_BRUTE_FORCE_THREADS_ALLOC   (num_CPUs())
 #endif
 #define DEFAULT_BRUTE_FORCE_RATE        (120000000.0) // if benchmark doesn't succeed
 #define TEST_BENCH_SIZE                 (6000)        // number of odd and even states for brute force benchmark
-#define TEST_BENCH_FILENAME             "hardnested_bf_bench_data.bin"
-//#define WRITE_BENCH_FILE
+
 #ifdef _MSC_VER
     #include <Windows.h>
 	#include <share.h>
 	#include <io.h>
 	#include <fcntl.h>
 	#include <sys/stat.h>
     #define atomic_add(num, val) (InterlockedExchangeAdd64(num, val) + val)
@@ -224,15 +218,15 @@
                 hardnested_print_progress(thread_arg->num_acquired_nonces, progress_text, 0.0, 0);
                 break;
             } else if (keys_found) {
                 break;
             } else {
                 if (!thread_arg->silent) {
                     char progress_text[80];
-                    snprintf(progress_text, sizeof(progress_text), "Brute force phase: %6.02f%%\t", 100.0 * (float)num_keys_tested / (float)(thread_arg->maximum_states));
+                    snprintf(progress_text, sizeof(progress_text), "Brute force phase: %6.02f%%", 100.0 * (float)num_keys_tested / (float)(thread_arg->maximum_states));
                     float remaining_bruteforce = thread_arg->nonces[thread_arg->best_first_bytes[0]].expected_num_brute_force - (float)num_keys_tested / 2;
                     hardnested_print_progress(thread_arg->num_acquired_nonces, progress_text, remaining_bruteforce, 5000);
                 }
             }
         }
         current_bucket += NUM_BRUTE_FORCE_THREADS;
     }
@@ -305,45 +299,14 @@
     for (uint32_t j = 0; j < 4 && j < nonces_to_bruteforce; j++) {
         bf_test_nonce[j] = bf_test_nonce_temp[j];
         bf_test_nonce_par[j] = bf_test_nonce_par_temp[j];
         bf_test_nonce_2nd_byte[j] = bf_test_nonce_2nd_byte_temp[j];
     }
 }
 
-
-#if defined (WRITE_BENCH_FILE)
-static void write_benchfile(statelist_t *candidates) {
-
-    PrintAndLogEx(NORMAL, "Writing brute force benchmark data in " RESOURCES_SUBDIR " subdirectory...");
-    FILE *benchfile = fopen(RESOURCES_SUBDIR TEST_BENCH_FILENAME, "wb");
-    if (benchfile == NULL) {
-        PrintAndLogEx(ERR, "Can't write " RESOURCES_SUBDIR TEST_BENCH_FILENAME", abort!");
-        return;
-    }
-    fwrite(&nonces_to_bruteforce, 1, sizeof(nonces_to_bruteforce), benchfile);
-    for (uint32_t i = 0; i < nonces_to_bruteforce; i++) {
-        fwrite(&(bf_test_nonce[i]), 1, sizeof(bf_test_nonce[i]), benchfile);
-        fwrite(&(bf_test_nonce_par[i]), 1, sizeof(bf_test_nonce_par[i]), benchfile);
-    }
-    uint32_t num_states = MIN(candidates->len[EVEN_STATE], TEST_BENCH_SIZE);
-    fwrite(&num_states, 1, sizeof(num_states), benchfile);
-    for (uint32_t i = 0; i < num_states; i++) {
-        fwrite(&(candidates->states[EVEN_STATE][i]), 1, sizeof(uint32_t), benchfile);
-    }
-    num_states = MIN(candidates->len[ODD_STATE], TEST_BENCH_SIZE);
-    fwrite(&num_states, 1, sizeof(num_states), benchfile);
-    for (uint32_t i = 0; i < num_states; i++) {
-        fwrite(&(candidates->states[ODD_STATE][i]), 1, sizeof(uint32_t), benchfile);
-    }
-    fclose(benchfile);
-    PrintAndLogEx(NORMAL, "Done");
-}
-#endif
-
-
 bool brute_force_bs(float *bf_rate, statelist_t *candidates, uint32_t cuid, uint32_t num_acquired_nonces, uint64_t maximum_states, noncelist_t *nonces, uint8_t *best_first_bytes, uint64_t *found_key) {
 #if defined (WRITE_BENCH_FILE)
     write_benchfile(candidates);
 #endif
     bool silent = (bf_rate != NULL);
 
     keys_found = 0;
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.h` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/hardnested_bruteforce.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.c` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/tables.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.h` & `FlipperNested-2.2.2/HardNestedSolver/hardnested/tables.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/parity.h` & `FlipperNested-2.2.2/HardNestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/util.h`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,32 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // See LICENSE.txt for the text of the license.
 //-----------------------------------------------------------------------------
-// CRC64 ECMA
+// utilities
 //-----------------------------------------------------------------------------
-
-#ifndef __CRC64_H
-#define __CRC64_H
+#ifndef __UTIL_H_
+#define __UTIL_H_
 
 #include "common.h"
 
-void crc64(const uint8_t *data, const size_t len, uint64_t *crc) ;
+#ifdef ANDROID
+#include <endian.h>
+#endif
+
+// used for save/load files
+#ifndef FILE_PATH_SIZE
+# define FILE_PATH_SIZE 1000
+#endif
+
+extern uint8_t g_debugMode;
+extern uint8_t g_printAndLog;
+
+#define PRINTANDLOG_PRINT 1
+#define PRINTANDLOG_LOG   2
+
+int num_CPUs(void); // number of logical CPUs
 
 #endif
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/emojis.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/emojis.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/emojis_alt.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/emojis_alt.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/ui.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/ui.h`

 * *Files 9% similar despite different names*

```diff
@@ -63,26 +63,15 @@
 
 extern session_arg_t g_session;
 #ifndef M_PI
 #define M_PI 3.14159265358979323846264338327
 #endif
 #define MAX_PRINT_BUFFER 2048
 
-#define PROMPT_CLEARLINE PrintAndLogEx(INPLACE, "                                          \r")
-void PrintAndLogOptions(const char *str[][2], size_t size, size_t space);
 void PrintAndLogEx(logLevel_t level, const char *fmt, ...);
-void SetFlushAfterWrite(bool value);
-bool GetFlushAfterWrite(void);
 void memcpy_filter_ansi(void *dest, const void *src, size_t n, bool filter);
-void memcpy_filter_rlmarkers(void *dest, const void *src, size_t n);
 void memcpy_filter_emoji(void *dest, const void *src, size_t n, emojiMode_t mode);
 
-int searchHomeFilePath(char **foundpath, const char *subdir, const char *filename, bool create_home);
-
-void print_progress(size_t count, uint64_t max, barMode_t style);
-
-void iceIIR_Butterworth(int *data, const size_t len);
-void iceSimple_Filter(int *data, const size_t len, uint8_t k);
 #ifdef __cplusplus
 }
 #endif
 #endif
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/commonutil.h`

 * *Files 24% similar despite different names*

```diff
@@ -9,26 +9,46 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // See LICENSE.txt for the text of the license.
 //-----------------------------------------------------------------------------
-// macOS framework bindings
+// Utility functions used in many places, not specific to any piece of code.
 //-----------------------------------------------------------------------------
 
-#ifndef UTIL_DARWIN_H__
-#define UTIL_DARWIN_H__
+#ifndef __COMMONUTIL_H
+#define __COMMONUTIL_H
 
-#ifdef __cplusplus
-extern "C" {
+#include "common.h"
+
+// endian change for 16bit
+#ifdef __GNUC__
+#ifndef BSWAP_16
+#define BSWAP_16(x) __builtin_bswap16(x)
+#endif
+#else
+#ifdef _MSC_VER
+#ifndef BSWAP_16
+#define BSWAP_16(x) _byteswap_ushort(x)
+#endif
+#else
+#ifndef BSWAP_16
+# define BSWAP_16(x) ((( ((x) & 0xFF00 ) >> 8))| ( (((x) & 0x00FF) << 8)))
+#endif
+#endif
 #endif
 
-void disableAppNap(const char *reason);
-void enableAppNap(void);
-void makeUnfocusable(void);
-void makeFocusable(void);
+#ifndef BITMASK
+# define BITMASK(X) (1 << (X))
+#endif
+#ifndef ARRAYLEN
+# define ARRAYLEN(x) (sizeof(x)/sizeof((x)[0]))
+#endif
 
-#ifdef __cplusplus
-}
+#ifndef NTIME
+# define NTIME(n) for (int _index = 0; _index < n; _index++)
 #endif
+
+uint64_t bytes_to_num(uint8_t *src, size_t len);
+
 #endif
```

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.c` & `FlipperNested-2.2.2/HardNestedSolver/pm3/util_posix.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.h` & `FlipperNested-2.2.2/HardNestedSolver/pm3/util_posix.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/HardNestedSolver/python.c` & `FlipperNested-2.2.2/HardNestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/LICENSE.md` & `FlipperNested-2.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/bucketsort.c` & `FlipperNested-2.2.2/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/bucketsort.h` & `FlipperNested-2.2.2/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/crapto1.c` & `FlipperNested-2.2.2/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/crapto1.h` & `FlipperNested-2.2.2/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/crypto1.c` & `FlipperNested-2.2.2/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/library.c` & `FlipperNested-2.2.2/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/library.h` & `FlipperNested-2.2.2/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/parity.h` & `FlipperNested-2.2.2/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/progress.c` & `FlipperNested-2.2.2/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/NestedSolver/python.c` & `FlipperNested-2.2.2/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/PKG-INFO` & `FlipperNested-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.1.2
+Version: 2.2.2
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.1.2/README.md` & `FlipperNested-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.2/tests/test_calculate.py` & `FlipperNested-2.2.2/tests/test_calculate.py`

 * *Files identical despite different names*

