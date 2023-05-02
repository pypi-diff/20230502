# Comparing `tmp/medicc2-0.9.1.tar.gz` & `tmp/medicc2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicc2-0.9.1.tar", last modified: Mon Mar 20 14:39:03 2023, max compression
+gzip compressed data, was "medicc2-0.9.2.tar", last modified: Tue May  2 13:33:53 2023, max compression
```

## Comparing `medicc2-0.9.1.tar` & `medicc2-0.9.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.405919 medicc2-0.9.1/
--rw-r--r--   0 tom        (501) staff       (20)    36109 2022-08-03 09:58:17.000000 medicc2-0.9.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)    19534 2023-03-20 14:39:03.405601 medicc2-0.9.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    18950 2023-03-20 13:00:04.000000 medicc2-0.9.1/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.384048 medicc2-0.9.1/fstlib/
--rw-r--r--   0 tom        (501) staff       (20)      527 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    16808 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/algos.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.390110 medicc2-0.9.1/fstlib/cext/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/cext/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      578 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cintegral_types.pxd
--rw-r--r--   0 tom        (501) staff       (20)     2109 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cios.pxd
--rw-r--r--   0 tom        (501) staff       (20)      184 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cmemory.pxd
--rw-r--r--   0 tom        (501) staff       (20)     8608 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cops.h
--rw-r--r--   0 tom        (501) staff       (20)      565 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cops.pxd
--rw-r--r--   0 tom        (501) staff       (20)    22206 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cpywrapfst.pxd
--rw-r--r--   0 tom        (501) staff       (20)     1351 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/cutility.pxd
--rw-r--r--   0 tom        (501) staff       (20)   243695 2023-03-20 14:39:01.000000 medicc2-0.9.1/fstlib/cext/ops.cpp
--rw-r--r--   0 tom        (501) staff       (20)     1526 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/ops.pyx
--rw-r--r--   0 tom        (501) staff       (20)  2724531 2023-03-20 14:39:02.000000 medicc2-0.9.1/fstlib/cext/pywrapfst.cpp
--rw-r--r--   0 tom        (501) staff       (20)    15924 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/pywrapfst.pxd
--rw-r--r--   0 tom        (501) staff       (20)   144735 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/cext/pywrapfst.pyx
--rw-r--r--   0 tom        (501) staff       (20)    17891 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/core.py
--rw-r--r--   0 tom        (501) staff       (20)     3139 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/ext.py
--rw-r--r--   0 tom        (501) staff       (20)    10679 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/factory.py
--rw-r--r--   0 tom        (501) staff       (20)      397 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/logging_conf.yaml
--rw-r--r--   0 tom        (501) staff       (20)     1446 2022-08-03 09:58:19.000000 medicc2-0.9.1/fstlib/test_fstlib.py
--rw-r--r--   0 tom        (501) staff       (20)     7873 2023-03-17 09:59:17.000000 medicc2-0.9.1/fstlib/tools.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.395187 medicc2-0.9.1/medicc/
--rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-20 12:44:27.000000 medicc2-0.9.1/medicc/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3540 2023-01-20 01:27:33.000000 medicc2-0.9.1/medicc/ancestors.py
--rw-r--r--   0 tom        (501) staff       (20)    10035 2023-03-19 23:31:02.000000 medicc2-0.9.1/medicc/bootstrap.py
--rw-r--r--   0 tom        (501) staff       (20)    20585 2023-03-20 01:17:36.000000 medicc2-0.9.1/medicc/core.py
--rw-r--r--   0 tom        (501) staff       (20)    23763 2023-03-20 13:02:00.000000 medicc2-0.9.1/medicc/event_reconstruction.py
--rw-r--r--   0 tom        (501) staff       (20)     8045 2023-03-20 00:17:58.000000 medicc2-0.9.1/medicc/factory.py
--rw-r--r--   0 tom        (501) staff       (20)    15681 2023-03-20 01:16:57.000000 medicc2-0.9.1/medicc/io.py
--rw-r--r--   0 tom        (501) staff       (20)      780 2022-08-03 09:58:17.000000 medicc2-0.9.1/medicc/logging_conf.yaml
--rw-r--r--   0 tom        (501) staff       (20)     5483 2022-08-03 09:58:17.000000 medicc2-0.9.1/medicc/nj.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.402821 medicc2-0.9.1/medicc/objects/
--rw-r--r--   0 tom        (501) staff       (20)    56129 2022-08-03 09:58:17.000000 medicc2-0.9.1/medicc/objects/Davoli_2013_TSG_OG_genes.bed
--rw-r--r--   0 tom        (501) staff       (20)     1382 2023-02-15 23:55:13.000000 medicc2-0.9.1/medicc/objects/hg19_chromosome_arms.bed
--rw-r--r--   0 tom        (501) staff       (20)     1382 2023-02-15 23:54:54.000000 medicc2-0.9.1/medicc/objects/hg38_chromosome_arms.bed
--rw-r--r--   0 tom        (501) staff       (20)   253982 2023-03-20 00:37:17.000000 medicc2-0.9.1/medicc/objects/no_wgd_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   572114 2023-03-20 00:37:19.000000 medicc2-0.9.1/medicc/objects/wgd_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   689774 2023-03-20 00:37:22.000000 medicc2-0.9.1/medicc/objects/wgd_2_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   783870 2023-03-20 00:37:03.000000 medicc2-0.9.1/medicc/objects/wgd_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   546246 2023-03-20 00:37:14.000000 medicc2-0.9.1/medicc/objects/wgd_total_cn_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   656310 2023-03-20 00:37:11.000000 medicc2-0.9.1/medicc/objects/wgd_total_cn_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   519890 2023-03-20 00:37:09.000000 medicc2-0.9.1/medicc/objects/wgd_x2_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   591554 2023-03-20 00:37:06.000000 medicc2-0.9.1/medicc/objects/wgd_x2_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)    42216 2023-03-20 01:30:46.000000 medicc2-0.9.1/medicc/plot.py
--rw-r--r--   0 tom        (501) staff       (20)     7644 2022-11-07 15:22:08.000000 medicc2-0.9.1/medicc/sim.py
--rw-r--r--   0 tom        (501) staff       (20)     2646 2022-08-03 09:58:17.000000 medicc2-0.9.1/medicc/stats.py
--rw-r--r--   0 tom        (501) staff       (20)     4934 2023-03-20 00:30:49.000000 medicc2-0.9.1/medicc/test_fsts.py
--rw-r--r--   0 tom        (501) staff       (20)    18549 2023-03-20 12:56:11.000000 medicc2-0.9.1/medicc/test_medicc.py
--rw-r--r--   0 tom        (501) staff       (20)     5141 2023-02-15 13:46:05.000000 medicc2-0.9.1/medicc/tools.py
--rwxr-xr-x   0 tom        (501) staff       (20)    14892 2023-03-20 12:50:13.000000 medicc2-0.9.1/medicc2
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 14:39:03.405245 medicc2-0.9.1/medicc2.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    19534 2023-03-20 14:39:03.000000 medicc2-0.9.1/medicc2.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     1327 2023-03-20 14:39:03.000000 medicc2-0.9.1/medicc2.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 14:39:03.000000 medicc2-0.9.1/medicc2.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      120 2023-03-20 14:39:03.000000 medicc2-0.9.1/medicc2.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       14 2023-03-20 14:39:03.000000 medicc2-0.9.1/medicc2.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       70 2022-08-03 09:58:17.000000 medicc2-0.9.1/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-20 14:39:03.405986 medicc2-0.9.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1982 2023-03-20 14:38:26.000000 medicc2-0.9.1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.778024 medicc2-0.9.2/
+-rw-r--r--   0 tom        (501) staff       (20)    36109 2023-05-02 11:56:04.000000 medicc2-0.9.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)    19534 2023-05-02 13:33:53.777681 medicc2-0.9.2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    18950 2023-05-02 12:03:22.000000 medicc2-0.9.2/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.751977 medicc2-0.9.2/fstlib/
+-rw-r--r--   0 tom        (501) staff       (20)      527 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    16808 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/algos.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.760917 medicc2-0.9.2/fstlib/cext/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      578 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cintegral_types.pxd
+-rw-r--r--   0 tom        (501) staff       (20)     2109 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cios.pxd
+-rw-r--r--   0 tom        (501) staff       (20)      184 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cmemory.pxd
+-rw-r--r--   0 tom        (501) staff       (20)     8608 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cops.h
+-rw-r--r--   0 tom        (501) staff       (20)      565 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cops.pxd
+-rw-r--r--   0 tom        (501) staff       (20)    22206 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cpywrapfst.pxd
+-rw-r--r--   0 tom        (501) staff       (20)     1351 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/cutility.pxd
+-rw-r--r--   0 tom        (501) staff       (20)   246353 2023-05-02 13:33:51.000000 medicc2-0.9.2/fstlib/cext/ops.cpp
+-rw-r--r--   0 tom        (501) staff       (20)     1526 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/ops.pyx
+-rw-r--r--   0 tom        (501) staff       (20)  2724666 2023-05-02 13:33:53.000000 medicc2-0.9.2/fstlib/cext/pywrapfst.cpp
+-rw-r--r--   0 tom        (501) staff       (20)    15924 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/pywrapfst.pxd
+-rw-r--r--   0 tom        (501) staff       (20)   144735 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/cext/pywrapfst.pyx
+-rw-r--r--   0 tom        (501) staff       (20)    17719 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     3139 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/ext.py
+-rw-r--r--   0 tom        (501) staff       (20)    10679 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/factory.py
+-rw-r--r--   0 tom        (501) staff       (20)      397 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/logging_conf.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     1446 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/test_fstlib.py
+-rw-r--r--   0 tom        (501) staff       (20)     7631 2023-05-02 11:56:08.000000 medicc2-0.9.2/fstlib/tools.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.766334 medicc2-0.9.2/medicc/
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-02 12:03:22.000000 medicc2-0.9.2/medicc/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3540 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/ancestors.py
+-rw-r--r--   0 tom        (501) staff       (20)    10115 2023-05-02 13:29:21.000000 medicc2-0.9.2/medicc/bootstrap.py
+-rw-r--r--   0 tom        (501) staff       (20)    20683 2023-05-02 13:29:21.000000 medicc2-0.9.2/medicc/core.py
+-rw-r--r--   0 tom        (501) staff       (20)    23763 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/event_reconstruction.py
+-rw-r--r--   0 tom        (501) staff       (20)     8045 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/factory.py
+-rw-r--r--   0 tom        (501) staff       (20)    15900 2023-05-02 13:32:43.000000 medicc2-0.9.2/medicc/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      780 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/logging_conf.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     5483 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/nj.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.774767 medicc2-0.9.2/medicc/objects/
+-rw-r--r--   0 tom        (501) staff       (20)    56129 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/Davoli_2013_TSG_OG_genes.bed
+-rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/hg19_chromosome_arms.bed
+-rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/hg38_chromosome_arms.bed
+-rw-r--r--   0 tom        (501) staff       (20)   253982 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/no_wgd_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   572114 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   689774 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_2_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   783870 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   546246 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_total_cn_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   656310 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_total_cn_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   519890 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_x2_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   591554 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/objects/wgd_x2_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)    42216 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/plot.py
+-rw-r--r--   0 tom        (501) staff       (20)     7644 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/sim.py
+-rw-r--r--   0 tom        (501) staff       (20)     2646 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/stats.py
+-rw-r--r--   0 tom        (501) staff       (20)     4934 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/test_fsts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21224 2023-05-02 13:29:21.000000 medicc2-0.9.2/medicc/test_medicc.py
+-rw-r--r--   0 tom        (501) staff       (20)     5141 2023-05-02 11:56:04.000000 medicc2-0.9.2/medicc/tools.py
+-rw-r--r--   0 tom        (501) staff       (20)    14892 2023-05-02 12:07:28.000000 medicc2-0.9.2/medicc2
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-02 13:33:53.777277 medicc2-0.9.2/medicc2.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    19534 2023-05-02 13:33:53.000000 medicc2-0.9.2/medicc2.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     1327 2023-05-02 13:33:53.000000 medicc2-0.9.2/medicc2.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-02 13:33:53.000000 medicc2-0.9.2/medicc2.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      120 2023-05-02 13:33:53.000000 medicc2-0.9.2/medicc2.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       14 2023-05-02 13:33:53.000000 medicc2-0.9.2/medicc2.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       70 2023-05-02 11:56:04.000000 medicc2-0.9.2/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-02 13:33:53.778112 medicc2-0.9.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2169 2023-05-02 13:29:21.000000 medicc2-0.9.2/setup.py
```

### Comparing `medicc2-0.9.1/LICENSE` & `medicc2-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/PKG-INFO` & `medicc2-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicc2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Whole-genome doubling-aware copy number phylogenies for cancer evolution
 Home-page: https://bitbucket.org/schwarzlab/medicc2
 Author: Tom L Kaufmann, Marina Petkovic, Roland F Schwarz
 Author-email: tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com
 License: GPL-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medicc2-0.9.1/README.md` & `medicc2-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/__init__.py` & `medicc2-0.9.2/fstlib/__init__.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/algos.py` & `medicc2-0.9.2/fstlib/algos.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cintegral_types.pxd` & `medicc2-0.9.2/fstlib/cext/cintegral_types.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cios.pxd` & `medicc2-0.9.2/fstlib/cext/cios.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cops.h` & `medicc2-0.9.2/fstlib/cext/cops.h`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cops.pxd` & `medicc2-0.9.2/fstlib/cext/cops.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cpywrapfst.pxd` & `medicc2-0.9.2/fstlib/cext/cpywrapfst.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/cutility.pxd` & `medicc2-0.9.2/fstlib/cext/cutility.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/ops.cpp` & `medicc2-0.9.2/fstlib/cext/ops.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "fstlib/cext/cops.h"
         ],
         "extra_compile_args": [
-            "-std=c++17"
+            "-std=c++17",
+            "-stdlib=libc++",
+            "-mmacosx-version-min=10.12"
         ],
         "include_dirs": [
             "./fstlib/cext",
             "fstlib/cext"
         ],
         "language": "c++",
         "libraries": [
@@ -34,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -228,15 +230,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -267,15 +269,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2399,20 +2401,28 @@
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -3952,68 +3962,87 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("fstlib.cext.pywrapfst"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Weight = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Weight", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Weight = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Weight", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Weight) __PYX_ERR(2, 71, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Weight = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Weight*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Weight->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Weight)) __PYX_ERR(2, 71, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView) __PYX_ERR(2, 107, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTableView)) __PYX_ERR(2, 107, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_EncodeMapperSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_EncodeMapperSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView) __PYX_ERR(2, 138, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView)) __PYX_ERR(2, 138, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_FstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_FstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView) __PYX_ERR(2, 146, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__FstSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__FstSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__FstSymbolTableView)) __PYX_ERR(2, 146, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableSymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableSymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable) __PYX_ERR(2, 154, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableSymbolTable = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableSymbolTable*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableSymbolTable)) __PYX_ERR(2, 154, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableFstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableFstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView) __PYX_ERR(2, 167, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView)) __PYX_ERR(2, 167, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable) __PYX_ERR(2, 175, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTable = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTable*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTable)) __PYX_ERR(2, 175, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_SymbolTableIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_SymbolTableIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator) __PYX_ERR(2, 198, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "EncodeMapper", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "EncodeMapper", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper) __PYX_ERR(2, 210, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_EncodeMapper = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_EncodeMapper*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_EncodeMapper)) __PYX_ERR(2, 210, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Fst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Fst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Fst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Fst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Fst) __PYX_ERR(2, 247, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Fst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Fst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Fst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Fst)) __PYX_ERR(2, 247, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "MutableFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "MutableFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst) __PYX_ERR(2, 313, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_MutableFst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_MutableFst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_MutableFst)) __PYX_ERR(2, 313, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "VectorFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "VectorFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst) __PYX_ERR(2, 394, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_VectorFst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_VectorFst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_VectorFst)) __PYX_ERR(2, 394, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Arc = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Arc", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Arc = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Arc", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Arc) __PYX_ERR(2, 416, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Arc = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Arc*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Arc->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Arc)) __PYX_ERR(2, 416, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_ArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_ArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator) __PYX_ERR(2, 426, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__ArcIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__ArcIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__ArcIterator)) __PYX_ERR(2, 426, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator) __PYX_ERR(2, 448, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableArcIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableArcIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableArcIterator)) __PYX_ERR(2, 448, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_StateIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_StateIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator) __PYX_ERR(2, 472, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__StateIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__StateIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__StateIterator)) __PYX_ERR(2, 472, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Compiler", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Compiler", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler) __PYX_ERR(2, 592, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Compiler = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Compiler*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Compiler)) __PYX_ERR(2, 592, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarReader", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarReader", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader) __PYX_ERR(2, 613, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarReader = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarReader*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarReader)) __PYX_ERR(2, 613, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarWriter", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarWriter", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter) __PYX_ERR(2, 638, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarWriter = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarWriter*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarWriter)) __PYX_ERR(2, 638, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -4544,44 +4573,62 @@
     return 0;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `medicc2-0.9.1/fstlib/cext/ops.pyx` & `medicc2-0.9.2/fstlib/cext/ops.pyx`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/pywrapfst.cpp` & `medicc2-0.9.2/fstlib/cext/pywrapfst.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
-            "-std=c++17"
+            "-std=c++17",
+            "-stdlib=libc++",
+            "-mmacosx-version-min=10.12"
         ],
         "include_dirs": [
             "fstlib/cext"
         ],
         "language": "c++",
         "libraries": [
             "fst",
@@ -31,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -225,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -264,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -55373,28 +55375,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `medicc2-0.9.1/fstlib/cext/pywrapfst.pxd` & `medicc2-0.9.2/fstlib/cext/pywrapfst.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/cext/pywrapfst.pyx` & `medicc2-0.9.2/fstlib/cext/pywrapfst.pyx`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/core.py` & `medicc2-0.9.2/fstlib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,23 +368,17 @@
     @classmethod
     def read(cls, source):
         ofst = pywrapfst.Fst.read(source)
         return Fst(ofst)
 
     @classmethod
     def read_from_string(cls, state):
-        ofst = pywrapfst.Fst.read_from_string(state)
+        ofst = pywrapfst.Fst.read(state)
         return Fst(ofst)
 
-    def __getstate__(self):
-        return self.write_to_string()
-
-    def __setstate__(self, state):
-        self.fst = pywrapfst.Fst.read_from_string(state)
-
 class Path(list):
     """ simple extension of list class that includes a final weight """
     __attributes = ["finalWeight"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args)
         self.finalWeight = kwargs.get("finalWeight", 0)
```

### Comparing `medicc2-0.9.1/fstlib/ext.py` & `medicc2-0.9.2/fstlib/ext.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/factory.py` & `medicc2-0.9.2/fstlib/factory.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/test_fstlib.py` & `medicc2-0.9.2/fstlib/test_fstlib.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/fstlib/tools.py` & `medicc2-0.9.2/fstlib/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,40 +44,36 @@
             
     paths=list()
     scores=list()
     for path in algo.get_paths():
         if tape == 'input':
             syms = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.input_symbols()])
             seq = delimiter.join([syms[p.ilabel] if syms is not None else str(p.ilabel) for p in path])
-            paths.append(seq)
         elif tape == 'output':
             syms = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.output_symbols()])
             seq = delimiter.join([syms[p.olabel] if syms is not None else str(p.olabel) for p in path])
-            paths.append(seq)
         elif tape == 'both':
-            syms_in = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.input_symbols()])
-            seq_in = delimiter.join([syms_in[p.ilabel] if syms_in is not None else str(p.ilabel) for p in path])
-            syms_out = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.output_symbols()])
-            seq_out = delimiter.join([syms_out[p.olabel] if syms_out is not None else str(p.olabel) for p in path])
-            paths.append((seq_in, seq_out))
+            isyms = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.input_symbols()])
+            osyms = dict([(i,s if isinstance(s, str) else str(s, 'utf-8')) for i,s in infst.output_symbols()])
+            seq = delimiter.join(["%s:%s" % 
+                         (isyms[p.ilabel] if isyms is not None else str(p.ilabel), 
+                          osyms[p.olabel] if osyms is not None else str(p.olabel)) for p in path])
         else:
             raise FstToolsError('Unknown tape parameter %s' % tape)
         if infst.arc_type() == fstlib.Semiring.LOG or infst.arc_type() == fstlib.Semiring.TROPICAL:
             score = functools.reduce(fstlib.times, [p.weight for p in path] + [path.finalWeight,])
         else:
             raise FstToolsError('semiring not implemented')
+        paths.append(seq)
         scores.append(float(score))
     if len(paths)==0:
         paths.append('[no path]')
         scores.append(np.inf)
     digits = int(np.log10(len(paths)))+1
-    if tape == 'both':
-        result = pd.DataFrame(data={'input': [p[0] for p in paths], 'output': [p[1] for p in paths], 'weight': scores})
-    else:
-        result = pd.DataFrame(data=list(zip(paths, scores)), columns=['string', 'weight'])
+    result = pd.DataFrame(data=list(zip(paths, scores)), columns=['string','weight'])
     result.sort_values('weight', inplace=True)
     result.index=[("path%%.%dd" % digits) % i for i in range(len(paths))]
     if to_real:
         result.weight = np.exp(-result.weight)
 
     return result
```

### Comparing `medicc2-0.9.1/medicc/__init__.py` & `medicc2-0.9.2/medicc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 from medicc.core import *
 from medicc.factory import *
 
 with open(os.path.join(os.path.dirname(__file__), 'logging_conf.yaml'), 'rt') as f:
     config = yaml.safe_load(f.read())
 logging.config.dictConfig(config)
 
-__version__ = pkg_resources.require("medicc2")[0].version
+try:
+    __version__ = pkg_resources.require("medicc2")[0].version
+except pkg_resources.DistributionNotFound:
+    __version__ = 'not installed'
```

### Comparing `medicc2-0.9.1/medicc/ancestors.py` & `medicc2-0.9.2/medicc/ancestors.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/bootstrap.py` & `medicc2-0.9.2/medicc/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     for i, cur_chrom in enumerate(cur_chroms):
         cur_data = input_df.reset_index().loc[(input_df.reset_index()['chrom'] == cur_chrom).values]
         cur_data['chrom'] = 'chr{}'.format(i+1)
         bootstrap_df = pd.concat([bootstrap_df, cur_data])
 
     bootstrap_df['chrom'] = tools.format_chromosomes(bootstrap_df['chrom'])
+    bootstrap_df[['start', 'end']] = bootstrap_df[['start', 'end']].astype(int)
     bootstrap_df.set_index(['sample_id', 'chrom', 'start', 'end'], inplace=True)
     bootstrap_df.sort_index(inplace=True)
 
     logger.debug("Created chr-wise bootstrap dataframe")
 
     return bootstrap_df
```

### Comparing `medicc2-0.9.1/medicc/core.py` & `medicc2-0.9.2/medicc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,17 @@
                                                                                                     len(cns),
                                                                                                     nr_alleles))
         nr_chroms = int(len(cns) // nr_alleles)
         for i, allele in enumerate(alleles):
             cn = list(''.join(cns[(i*nr_chroms):((i+1)*nr_chroms)]))
             internal_cns[(allele, node)] = cn
 
-    output_df = (pd.concat([output_df, pd.DataFrame(internal_cns, index=output_df.index)], axis=1)
+    internal_cns_df = pd.DataFrame(internal_cns, index=output_df.index)
+    internal_cns_df.columns.names = ['allele', 'sample_id']
+    output_df = (pd.concat([output_df, internal_cns_df], axis=1)
                  .stack('sample_id')
                  .reorder_levels(['sample_id', 'chrom', 'start', 'end'])
                  .sort_index())
 
     return output_df
```

### Comparing `medicc2-0.9.1/medicc/event_reconstruction.py` & `medicc2-0.9.2/medicc/event_reconstruction.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/factory.py` & `medicc2-0.9.2/medicc/factory.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/io.py` & `medicc2-0.9.2/medicc/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 
 from medicc import plot, tools
 
 matplotlib.use("Agg")
 logger = logging.getLogger(__name__)
 
 
-def read_and_parse_input_data(filename, normal_name='diploid', input_type='tsv', separator='X', 
-                              allele_columns=['cn_a', 'cn_b'], maxcn=8, total_copy_numbers=False):
+def read_and_parse_input_data(filename, normal_name='diploid', input_type='tsv', separator='X',
+                              chrom_column='chrom', allele_columns=['cn_a', 'cn_b'], maxcn=8,
+                              total_copy_numbers=False):
 
     if len(allele_columns) == 1 and not total_copy_numbers:
         logger.warn('You have provided only one allele column but the --total-copy-numbers flag was not set')
     if total_copy_numbers and not len(allele_columns) == 1:
         raise MEDICCIOError("You have set the --total-copy-numbers flag but provided more than one allele column. "
                             "Set allele columns with the flag --input-allele-columns")
 
     ## Read in input data
     if input_type.lower() == "fasta" or input_type.lower() == 'f':
         logger.info("Reading FASTA input.")
         input_df = _read_fasta_as_dataframe(filename, separator=separator, allele_columns=allele_columns, maxcn=maxcn)
     elif input_type.lower() == "tsv" or input_type.lower() == 't':
         logger.info("Reading Refphase TSV input.")
-        input_df = _read_tsv_as_dataframe(filename, allele_columns=allele_columns, maxcn=maxcn)
+        input_df = _read_tsv_as_dataframe(
+            filename, allele_columns=allele_columns, maxcn=maxcn, chrom_column=chrom_column)
     else:
         raise MEDICCIOError("Unknown input type, possible options are 'fasta' or 'tsv'.")
 
     input_df.columns.name = 'allele'
     input_df_stacked = input_df.stack('allele').unstack('sample_id').T
 
     duplicated_entries = input_df_stacked.duplicated(keep=False)
@@ -44,17 +46,17 @@
     normal_samples = np.setdiff1d(input_df_stacked.index[
         (input_df_stacked == normal_value).all(axis=1)], normal_name)
     if len(normal_samples) > 0:
         logger.warn(f"Normal samples found in input data: {normal_samples}")
     
     ## Add normal sample if needed
     input_df = add_normal_sample(input_df, normal_name, allele_columns=allele_columns, 
-                                    total_copy_numbers=total_copy_numbers)
+                                    total_copy_numbers=total_copy_numbers, chrom_column=chrom_column)
     nsamples = input_df.index.get_level_values('sample_id').unique().shape[0]
-    nchr = input_df.index.get_level_values('chrom').unique().shape[0]
+    nchr = input_df.index.get_level_values(chrom_column).unique().shape[0]
     nsegs = input_df.loc[normal_name,:].shape[0]
     logger.info("Read %d samples, %d chromosomes, %d segments per sample", nsamples, nchr, nsegs)
 
     gaps = (input_df.loc[normal_name].eval('start') - 
             np.roll(input_df.loc[normal_name].eval('end'), 1)).values
     total_gaps = gaps[gaps>0].sum()
     if total_gaps > 1e8:
@@ -159,18 +161,18 @@
 
 
 def filter_by_segment_length(input_df, filter_size):
     segment_length = input_df.eval('end+1-start')
     return input_df.loc[segment_length > float(filter_size)]
 
 
-def _read_tsv_as_dataframe(path, allele_columns=['cn_a','cn_b'], maxcn=8):
+def _read_tsv_as_dataframe(path, allele_columns=['cn_a','cn_b'], maxcn=8, chrom_column='chrom'):
     logger.info("Reading TSV file %s", path)
     input_file = pd.read_csv(path, sep = "\t")
-    columnn_names = ['sample_id', 'chrom', 'start', 'end'] + allele_columns
+    columnn_names = ['sample_id', chrom_column, 'start', 'end'] + allele_columns
     if len(np.setdiff1d(columnn_names, input_file.columns)) > 0:
         raise MEDICCIOError(f"TSV file needs the following columns: sample_id, chrom, start, end and the allele columns ({allele_columns})"
                             "\nMissing columns are: {}".format(
                                 np.setdiff1d(columnn_names, input_file.columns)))
 
     logger.info("Successfully read input file. Using columns {%s}" % ', '.join(columnn_names))
     input_file = input_file[columnn_names]
@@ -178,18 +180,18 @@
         if input_file[c].dtype in [np.dtype('float64'), np.dtype('float32')]:
             logger.warning("Floating point payload! I will round, but this might not be intended.")
             input_file[c] = input_file[c].round().astype('int')
         if input_file[c].dtype in [np.dtype('int64'), np.dtype('int32')]:
             if np.any(input_file[c]>maxcn):
                 logger.warning("Integer CN > maxcn %d, capping.", maxcn)
                 input_file[c] = np.fmin(input_file[c], maxcn)
-    input_file['chrom'] = tools.format_chromosomes(input_file['chrom'])
-    if input_file['chrom'].apply(lambda x: "Y" in str(x)).any():
+    input_file[chrom_column] = tools.format_chromosomes(input_file[chrom_column])
+    if input_file[chrom_column].apply(lambda x: "Y" in str(x)).any():
         logger.warn("Y chromosome detected in input. This might cause errors down the line!")
-    input_file.set_index(['sample_id', 'chrom', 'start', 'end'], inplace=True)
+    input_file.set_index(['sample_id', chrom_column, 'start', 'end'], inplace=True)
     input_file.sort_index(inplace=True)
     input_file[allele_columns] = input_file[allele_columns].astype(str)
 
     return input_file
 
 
 def _read_fasta_as_dataframe(infile: str, separator: str = 'X', allele_columns = ['cn_a','cn_b'], maxcn: int = 8):
@@ -245,15 +247,16 @@
     result['chrom'] = tools.format_chromosomes(result['chrom'])
     result.sort_values(['sample_id', 'chrom', 'start', 'end'], inplace=True)
     result.set_index(['sample_id', 'chrom', 'start', 'end'], inplace=True)
     result.sort_index(inplace=True)
 
     return result
 
-def add_normal_sample(df, normal_name, allele_columns=['cn_a','cn_b'], total_copy_numbers=False):
+def add_normal_sample(df, normal_name, allele_columns=['cn_a','cn_b'], total_copy_numbers=False,
+                      chrom_column='chrom'):
     """Adds an artificial normal samples with the supplied name to the data frame.
     The normal sample has CN=1 on all supplied alleles. """
     samples = df.index.get_level_values('sample_id').unique()
 
     if total_copy_numbers:
         normal_value = '2'
     else:
@@ -261,15 +264,15 @@
 
     if normal_name is not None and normal_name not in samples:
         logger.info("Normal sample '%s' not found, adding artifical normal by the name: '%s'.", normal_name, normal_name)
         tmp = df.unstack('sample_id')
         for col in allele_columns:
             tmp.loc[:, (col, normal_name)] = normal_value
         tmp = tmp.stack('sample_id')
-        tmp = tmp.reorder_levels(['sample_id', 'chrom', 'start', 'end']).sort_index()
+        tmp = tmp.reorder_levels(['sample_id', chrom_column, 'start', 'end']).sort_index()
     else:
         logger.info("Sample '%s' was found in data is is used as normal", normal_name)
         if np.any(df.loc[normal_name] == '0'):
             logger.warn("The provided normal sample contains segments with copy number 0. "
                         "If any other sample has non-zero values in these segments, MEDICC will crash")
         if np.any(df.loc[normal_name] != normal_value):
             logger.warn("The provided normal sample contains segments with copy number != {}.".format(normal_value))
```

### Comparing `medicc2-0.9.1/medicc/logging_conf.yaml` & `medicc2-0.9.2/medicc/logging_conf.yaml`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/nj.py` & `medicc2-0.9.2/medicc/nj.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/Davoli_2013_TSG_OG_genes.bed` & `medicc2-0.9.2/medicc/objects/Davoli_2013_TSG_OG_genes.bed`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/hg19_chromosome_arms.bed` & `medicc2-0.9.2/medicc/objects/hg19_chromosome_arms.bed`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/hg38_chromosome_arms.bed` & `medicc2-0.9.2/medicc/objects/hg38_chromosome_arms.bed`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/no_wgd_asymm.fst` & `medicc2-0.9.2/medicc/objects/no_wgd_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_1_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_2_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_2_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_total_cn_1_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_total_cn_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_total_cn_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_total_cn_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_x2_1_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_x2_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/objects/wgd_x2_asymm.fst` & `medicc2-0.9.2/medicc/objects/wgd_x2_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/plot.py` & `medicc2-0.9.2/medicc/plot.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/sim.py` & `medicc2-0.9.2/medicc/sim.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/stats.py` & `medicc2-0.9.2/medicc/stats.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/test_fsts.py` & `medicc2-0.9.2/medicc/test_fsts.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc/test_medicc.py` & `medicc2-0.9.2/medicc/test_medicc.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,14 +142,70 @@
 
     assert process.returncode == 0, 'Error while running MEDICC'
     assert np.all(all_files_exist), "Some files were not created! Missing files are: {}".format(
         np.array(expected_files)[~np.array(all_files_exist)])
     assert nr_events == tree_size, f"Number of events is {nr_events}, but tree size is {tree_size}"
 
 
+def test_medicc_with_testing_example_parallelization():
+    "Testing small example"
+    output_dir = 'examples/test_output_parallelization'
+    process = subprocess.Popen(['python', "medicc2", "examples/testing_example/testing_example.tsv", 
+                                output_dir, "--n-cores", "4", "--events", "--chromosomes-bed", "default", "--regions-bed", "default"],
+                               stdout=subprocess.PIPE,
+                               cwd=pathlib.Path(__file__).parent.parent.absolute())
+
+    while process.poll() is None:
+        # Process hasn't exited yet
+        time.sleep(0.5)
+
+    expected_files = ['testing_example_cn_profiles.pdf', 'testing_example_final_cn_profiles.tsv',
+                      'testing_example_final_tree.new', 'testing_example_final_tree.png',
+                      'testing_example_final_tree.xml', 'testing_example_pairwise_distances.tsv',
+                      'testing_example_summary.tsv', 'testing_example_copynumber_events_df.tsv',
+                      'testing_example_events_overlap.tsv', 'testing_example_branch_lengths.tsv']
+    all_files_exist = [os.path.isfile(os.path.join(output_dir, f))
+                       for f in expected_files]
+    nr_events, tree_size = get_number_of_events(output_dir, 'testing_example')
+    subprocess.Popen(["rm", output_dir, "-rf"])
+
+    assert process.returncode == 0, 'Error while running MEDICC'
+    assert np.all(all_files_exist), "Some files were not created! Missing files are: {}".format(
+        np.array(expected_files)[~np.array(all_files_exist)])
+    assert nr_events == tree_size, f"Number of events is {nr_events}, but tree size is {tree_size}"
+
+
+def test_medicc_with_testing_example_parallelization():
+    "Testing small example"
+    output_dir = 'examples/test_output_parallelization'
+    process = subprocess.Popen(['python', "medicc2", "examples/testing_example/testing_example.tsv", 
+                                output_dir, "--n-cores", "4", "--events", "--chromosomes-bed", "default", "--regions-bed", "default"],
+                               stdout=subprocess.PIPE,
+                               cwd=pathlib.Path(__file__).parent.parent.absolute())
+
+    while process.poll() is None:
+        # Process hasn't exited yet
+        time.sleep(0.5)
+
+    expected_files = ['testing_example_cn_profiles.pdf', 'testing_example_final_cn_profiles.tsv',
+                      'testing_example_final_tree.new', 'testing_example_final_tree.png',
+                      'testing_example_final_tree.xml', 'testing_example_pairwise_distances.tsv',
+                      'testing_example_summary.tsv', 'testing_example_copynumber_events_df.tsv',
+                      'testing_example_events_overlap.tsv', 'testing_example_branch_lengths.tsv']
+    all_files_exist = [os.path.isfile(os.path.join(output_dir, f))
+                       for f in expected_files]
+    nr_events, tree_size = get_number_of_events(output_dir, 'testing_example')
+    subprocess.Popen(["rm", output_dir, "-rf"])
+
+    assert process.returncode == 0, 'Error while running MEDICC'
+    assert np.all(all_files_exist), "Some files were not created! Missing files are: {}".format(
+        np.array(expected_files)[~np.array(all_files_exist)])
+    assert nr_events == tree_size, f"Number of events is {nr_events}, but tree size is {tree_size}"
+
+
 def test_medicc_with_testing_example_nowgd():
     "Testing small example"
     output_dir = 'examples/test_output_nowgd'
     process = subprocess.Popen(['python', "medicc2", "examples/testing_example/testing_example.tsv", 
                                 output_dir, "--no-wgd", "--events", "--chromosomes-bed", "default", "--regions-bed", "default"],
                                stdout=subprocess.PIPE,
                                cwd=pathlib.Path(__file__).parent.parent.absolute())
@@ -160,15 +216,16 @@
 
     expected_files = ['testing_example_cn_profiles.pdf', 'testing_example_final_cn_profiles.tsv',
                       'testing_example_final_tree.new', 'testing_example_final_tree.png',
                       'testing_example_final_tree.xml', 'testing_example_pairwise_distances.tsv',
                       'testing_example_summary.tsv', 'testing_example_copynumber_events_df.tsv',
                       'testing_example_events_overlap.tsv', 'testing_example_branch_lengths.tsv']
     all_files_exist = [os.path.isfile(os.path.join(output_dir, f))
-                       for f in expected_files]
+                        for f in expected_files]
+
     nr_events, tree_size = get_number_of_events(output_dir, 'testing_example')
     subprocess.Popen(["rm", output_dir, "-rf"])
 
     assert process.returncode == 0, 'Error while running MEDICC'
     assert np.all(all_files_exist), "Some files were not created! Missing files are: {}".format(
         np.array(expected_files)[~np.array(all_files_exist)])
     assert nr_events == tree_size, f"Number of events is {nr_events}, but tree size is {tree_size}"
@@ -293,31 +350,14 @@
 
     assert process.returncode == 0, f'Error while running MEDICC for Gundem et al patient {patient}'
     assert np.all(all_files_exist), "Some files were not created! Missing files are: {}".format(
         np.array(expected_files)[~np.array(all_files_exist)])
     assert nr_events == tree_size, f"Number of events is {nr_events}, but tree size is {tree_size}"
 
 
-all_py_notebooks = [x for x in os.listdir('notebooks') if '.py' in x]
-@pytest.mark.parametrize("notebook", all_py_notebooks)
-def test_all_py_notebooks(notebook):
-    "Testing if all notebooks (with ending .py) work"
-
-    process = subprocess.Popen(['python', 
-                                f"{notebook}"],
-                               stdout=subprocess.PIPE,
-                               cwd=os.path.join(pathlib.Path(__file__).parent.parent.absolute(), 'notebooks'))
-
-    while process.poll() is None:
-        # Process hasn't exited yet
-        time.sleep(0.5)
-
-    assert process.returncode == 0, f'Error while running notebook {notebook}'
-
-
 all_ipynb_notebooks = [x for x in os.listdir('notebooks') if '.ipynb' in x]
 @pytest.mark.parametrize("notebook", all_ipynb_notebooks)
 def test_all_ipynb_notebooks(notebook):
     "Testing if all notebooks (with ending .ipynb) work"
 
     process = subprocess.Popen([f'ipython -c "%run {notebook}"'],
                                stdout=subprocess.PIPE,
```

### Comparing `medicc2-0.9.1/medicc/tools.py` & `medicc2-0.9.2/medicc/tools.py`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc2` & `medicc2-0.9.2/medicc2`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/medicc2.egg-info/PKG-INFO` & `medicc2-0.9.2/medicc2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicc2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Whole-genome doubling-aware copy number phylogenies for cancer evolution
 Home-page: https://bitbucket.org/schwarzlab/medicc2
 Author: Tom L Kaufmann, Marina Petkovic, Roland F Schwarz
 Author-email: tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com
 License: GPL-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medicc2-0.9.1/medicc2.egg-info/SOURCES.txt` & `medicc2-0.9.2/medicc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicc2-0.9.1/setup.py` & `medicc2-0.9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 from pathlib import Path
 
 from Cython.Build import cythonize
 from setuptools import Extension, setup
 
 sys.path.append('fstlib/cext')
 
+extra_compile_args = ['-std=c++17']
+if sys.platform.startswith("darwin"):
+  extra_compile_args.append("-stdlib=libc++")
+  extra_compile_args.append("-mmacosx-version-min=10.12")
+
 setup(
     name='medicc2',
-    version='0.9.1',
+    version='0.9.2',
     author='Tom L Kaufmann, Marina Petkovic, Roland F Schwarz',
     author_email='tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com',
     description='Whole-genome doubling-aware copy number phylogenies for cancer evolution',
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/schwarzlab/medicc2',
     classifiers=[
@@ -39,18 +44,18 @@
         "fstlib": ["logging_conf.yaml", "cext/*.pxd", "cext/*.pyx", "cext/*.h"],
     },
     ext_modules = cythonize([
         Extension("fstlib.cext.pywrapfst", 
                   ["fstlib/cext/pywrapfst.pyx"],
                   include_dirs=['fstlib/cext'],
                   libraries=["fst", "fstfar", "fstscript", "fstfarscript"],
-                  extra_compile_args=['-std=c++17'],
+                  extra_compile_args=extra_compile_args,
                   language = "c++"),
 
         Extension("fstlib.cext.ops", 
                   ["fstlib/cext/ops.pyx"],
                   include_dirs=['fstlib/cext'],
                   libraries=["fst", "fstfar", "fstscript", "fstfarscript"],
-                  extra_compile_args=['-std=c++17'],
+                  extra_compile_args=extra_compile_args,
                   language = "c++")
     ])
 )
```

