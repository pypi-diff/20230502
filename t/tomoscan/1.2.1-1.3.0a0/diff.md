# Comparing `tmp/tomoscan-1.2.1.tar.gz` & `tmp/tomoscan-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomoscan-1.2.1.tar", last modified: Thu Mar  2 10:46:50 2023, max compression
+gzip compressed data, was "tomoscan-1.3.0a0.tar", last modified: Tue May  2 07:43:22 2023, max compression
```

## Comparing `tomoscan-1.2.1.tar` & `tomoscan-1.3.0a0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.115280 tomoscan-1.2.1/
--rw-r--r--   0 payno     (1000) payno     (1000)     1253 2021-04-06 11:24:41.000000 tomoscan-1.2.1/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)      951 2023-03-02 10:46:50.115280 tomoscan-1.2.1/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      691 2023-03-02 10:31:26.000000 tomoscan-1.2.1/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     1213 2023-03-02 10:46:50.115280 tomoscan-1.2.1/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)     1487 2022-06-30 08:57:01.000000 tomoscan-1.2.1/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.107281 tomoscan-1.2.1/tomoscan/
--rw-r--r--   0 payno     (1000) payno     (1000)       67 2022-01-04 09:22:29.000000 tomoscan-1.2.1/tomoscan/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/esrf/
--rw-r--r--   0 payno     (1000) payno     (1000)     1994 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      263 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/edfscan.py
--rw-r--r--   0 payno     (1000) payno     (1000)      266 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/hdf5scan.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/esrf/identifier/
--rw-r--r--   0 payno     (1000) payno     (1000)     1765 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2926 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/edfidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5570 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/folderidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5841 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/hdf5Identifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2302 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/jp2kidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2829 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/rawidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3718 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/tiffidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2748 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/identifier/url_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)      254 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/mock.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/esrf/scan/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/scan/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    43771 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/scan/edfscan.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/
--rw-r--r--   0 payno     (1000) payno     (1000)      118 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    25347 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/edfframereducer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8557 2022-12-07 11:57:13.000000 tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    59580 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/esrf/scan/hdf5scan.py
--rw-r--r--   0 payno     (1000) payno     (1000)    37290 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/esrf/scan/mock.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22713 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/esrf/scan/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)      257 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/esrf/volume/
--rw-r--r--   0 payno     (1000) payno     (1000)     1637 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/volume/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5367 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/volume/edfvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    18915 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/volume/hdf5volume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8742 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/volume/jp2kvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3034 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/esrf/volume/mock.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17045 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/volume/rawvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15112 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/volume/singleframebase.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17457 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/esrf/volume/tiffvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8677 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/esrf/volume/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10005 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/factory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3559 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/framereducerbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2434 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/identifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6030 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/nexus/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/nexus/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.111281 tomoscan-1.2.1/tomoscan/nexus/paths/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/nexus/paths/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      831 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      406 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      250 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      540 2022-03-18 14:18:17.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      276 2022-07-06 14:29:40.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11200 2023-03-02 10:30:17.000000 tomoscan-1.2.1/tomoscan/nexus/paths/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5450 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3251 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/progress.py
--rw-r--r--   0 payno     (1000) payno     (1000)    66320 2023-03-02 10:31:26.000000 tomoscan-1.2.1/tomoscan/scanbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)      303 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/scanfactory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8248 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/serie.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.115280 tomoscan-1.2.1/tomoscan/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2021-04-19 05:14:56.000000 tomoscan-1.2.1/tomoscan/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      265 2022-08-03 13:26:18.000000 tomoscan-1.2.1/tomoscan/test/conftest.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1731 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_framereducerbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)      450 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/test/test_hdf5_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2848 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_io.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7464 2022-11-04 06:48:56.000000 tomoscan-1.2.1/tomoscan/test/test_normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2013 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_progress.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9003 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/test/test_scanbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4567 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/test/test_scanfactory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6218 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_serie.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1610 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_tomoobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3703 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/test/test_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11615 2022-09-04 15:06:50.000000 tomoscan-1.2.1/tomoscan/test/test_validator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1502 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/test/test_version.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2908 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/test/test_volume_base.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6184 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/test/test_volume_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8646 2022-09-04 15:06:50.000000 tomoscan-1.2.1/tomoscan/test/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2339 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/tomoobject.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.115280 tomoscan-1.2.1/tomoscan/unitsystem/
--rw-r--r--   0 payno     (1000) payno     (1000)     1657 2022-06-17 12:04:52.000000 tomoscan-1.2.1/tomoscan/unitsystem/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2449 2022-06-17 12:04:52.000000 tomoscan-1.2.1/tomoscan/unitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3273 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/unitsystem/energysystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6543 2022-06-30 08:57:01.000000 tomoscan-1.2.1/tomoscan/unitsystem/metricsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3167 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/unitsystem/timesystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1846 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/unitsystem/unit.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1977 2022-03-18 13:52:39.000000 tomoscan-1.2.1/tomoscan/unitsystem/voltagesystem.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.115280 tomoscan-1.2.1/tomoscan/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)      175 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1122 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/decorator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2976 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/geometry.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2710 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/hdf5.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1512 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/io.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8872 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/utils/volume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17049 2022-12-07 12:43:52.000000 tomoscan-1.2.1/tomoscan/validator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4346 2023-03-02 10:45:07.000000 tomoscan-1.2.1/tomoscan/version.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19264 2023-01-19 12:46:27.000000 tomoscan-1.2.1/tomoscan/volumebase.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-03-02 10:46:50.107281 tomoscan-1.2.1/tomoscan.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)      951 2023-03-02 10:46:50.000000 tomoscan-1.2.1/tomoscan.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     2741 2023-03-02 10:46:50.000000 tomoscan-1.2.1/tomoscan.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-03-02 10:46:50.000000 tomoscan-1.2.1/tomoscan.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      300 2023-03-02 10:46:50.000000 tomoscan-1.2.1/tomoscan.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        9 2023-03-02 10:46:50.000000 tomoscan-1.2.1/tomoscan.egg-info/top_level.txt
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1253 2021-08-04 06:21:11.000000 tomoscan-1.3.0a0/LICENSE
+-rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)      609 2023-03-08 13:26:14.000000 tomoscan-1.3.0a0/README.md
+-rw-r--r--   0 payno    (81067) soft      (3401)     1213 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/setup.cfg
+-rw-r--r--   0 payno    (81067) soft      (3401)     1486 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/setup.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.192546 tomoscan-1.3.0a0/tomoscan/
+-rw-r--r--   0 payno    (81067) soft      (3401)       67 2022-03-24 14:18:52.000000 tomoscan-1.3.0a0/tomoscan/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1992 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      263 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/edfscan.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      266 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/hdf5scan.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/identifier/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1765 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2926 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/edfidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5467 2023-03-30 07:26:18.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/folderidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5781 2023-03-30 07:26:20.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/hdf5Identifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2302 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/jp2kidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2732 2023-03-30 07:20:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/rawidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3621 2023-03-30 07:26:24.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/tiffidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2436 2023-03-30 07:19:36.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/url_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      254 2023-02-20 15:01:41.000000 tomoscan-1.3.0a0/tomoscan/esrf/mock.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/scan/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2023-02-08 14:54:26.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    43737 2023-03-30 14:34:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/edfscan.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/
+-rw-r--r--   0 payno    (81067) soft      (3401)      118 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    25256 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/edfframereducer.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8542 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    58032 2023-05-02 07:34:41.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/hdf5scan.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    37157 2023-04-28 09:11:19.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/mock.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    22716 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      257 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/utils.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/esrf/volume/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1637 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5369 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/edfvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    18937 2023-04-28 14:23:39.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/hdf5volume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8775 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/jp2kvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3035 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/mock.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17047 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/rawvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    15152 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/singleframebase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17517 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/tiffvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     9222 2023-05-02 07:34:38.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    10003 2023-04-28 09:02:37.000000 tomoscan-1.3.0a0/tomoscan/factory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3757 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/framereducerbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2434 2023-02-01 10:03:58.000000 tomoscan-1.3.0a0/tomoscan/identifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6006 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/io.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/nexus/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a0/tomoscan/nexus/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/nexus/paths/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      831 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxdetector.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      406 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxinstrument.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      250 2023-02-01 10:03:58.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxmonitor.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      540 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsample.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      276 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsource.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    11151 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxtomo.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5438 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/normalization.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3214 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/progress.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    66281 2023-03-31 07:57:09.000000 tomoscan-1.3.0a0/tomoscan/scanbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      303 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/scanfactory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8224 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/serie.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-12-06 12:48:08.000000 tomoscan-1.3.0a0/tomoscan/test/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      266 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/conftest.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1732 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_framereducerbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      451 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_hdf5_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2850 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_io.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     7466 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_normalization.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2013 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_progress.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8976 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_scanbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4569 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_scanfactory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6223 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_serie.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1611 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_tomoobject.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3704 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    11616 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_validator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1502 2022-12-06 12:48:08.000000 tomoscan-1.3.0a0/tomoscan/test/test_version.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2909 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_volume_base.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6186 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_volume_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8574 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2341 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/tomoobject.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/unitsystem/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1657 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2447 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3270 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/energysystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6542 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/metricsystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3165 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/timesystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1846 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/unit.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1975 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/voltagesystem.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/utils/
+-rw-r--r--   0 payno    (81067) soft      (3401)      175 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1120 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/decorator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2976 2023-01-05 08:34:39.000000 tomoscan-1.3.0a0/tomoscan/utils/geometry.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2666 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/hdf5.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1512 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/io.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8884 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/volume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17014 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/validator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4346 2023-05-02 07:43:05.000000 tomoscan-1.3.0a0/tomoscan/version.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    19307 2023-05-02 07:34:38.000000 tomoscan-1.3.0a0/tomoscan/volumebase.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan.egg-info/
+-rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)     2741 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/SOURCES.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/dependency_links.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)      300 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/requires.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        9 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/top_level.txt
```

### Comparing `tomoscan-1.2.1/LICENSE` & `tomoscan-1.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/PKG-INFO` & `tomoscan-1.3.0a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.2.1
+Version: 1.3.0a0
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.2.1/setup.cfg` & `tomoscan-1.3.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/setup.py` & `tomoscan-1.3.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,10 +27,9 @@
 __authors__ = ["H. Payno", "P. Paleo", "C. Nemoz"]
 __date__ = "26/07/2021"
 __license__ = "MIT"
 
 
 import setuptools
 
-
 if __name__ == "__main__":
     setuptools.setup()
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/__init__.py` & `tomoscan-1.3.0a0/tomoscan/esrf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,20 @@
 #############################################################################
 
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "09/08/2018"
 
+from .scan.edfscan import EDFTomoScan  # noqa F401
 from .scan.hdf5scan import HDF5TomoScan  # noqa F401
 from .scan.hdf5scan import HDF5XRD3DScan  # noqa F401
-from .scan.edfscan import EDFTomoScan  # noqa F401
-
-from .volume.hdf5volume import HDF5Volume  # noqa F401
 from .volume.edfvolume import EDFVolume  # noqa F401
-from .volume.tiffvolume import TIFFVolume  # noqa F401
-from .volume.tiffvolume import MultiTIFFVolume  # noqa F401
+from .volume.hdf5volume import HDF5Volume  # noqa F401
 from .volume.jp2kvolume import JP2KVolume  # noqa F401
-from .volume.rawvolume import RawVolume  # noqa F401
-
 from .volume.jp2kvolume import has_glymur  # noqa F401
+from .volume.rawvolume import RawVolume  # noqa F401
+from .volume.tiffvolume import MultiTIFFVolume  # noqa F401
+from .volume.tiffvolume import TIFFVolume  # noqa F401
 from .volume.tiffvolume import has_tifffile  # noqa F401
 
 TYPES = ["EDF", "HDF5"]
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/__init__.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 # ###########################################################################*/
 
 """This module is dedicated to instances of :class:`BaseIdentifier` used at esrf"""
 
-from .hdf5Identifier import HDF5TomoScanIdentifier  # noqa F401
 from .edfidentifier import EDFTomoScanIdentifier  # noqa F401
+from .hdf5Identifier import HDF5TomoScanIdentifier  # noqa F401
 from .jp2kidentifier import JP2KVolumeIdentifier  # noqa F401
-from .tiffidentifier import TIFFVolumeIdentifier  # noqa F401
-from .tiffidentifier import MultiTiffVolumeIdentifier  # noqa F401
 from .rawidentifier import RawVolumeIdentifier  # noqa F401
+from .tiffidentifier import MultiTiffVolumeIdentifier  # noqa F401
+from .tiffidentifier import TIFFVolumeIdentifier  # noqa F401
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/edfidentifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/edfidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/folderidentifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/folderidentifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,37 +26,36 @@
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "01/02/2022"
 
 
 import os
 from urllib.parse import ParseResult, urlparse
+
 from tomoscan.esrf.identifier.url_utils import (
     UrlSettings,
     join_path,
     join_query,
     split_path,
     split_query,
-    reduce_file_path,
 )
 
 
 class BaseFolderIdentifierMixIn:
     """Identifier specific to a folder. Used for single frame edf and jp2g for example"""
 
     def __init__(self, object, folder, tomo_type):
         super().__init__(object)
         self._folder = os.path.realpath(os.path.abspath(folder))
         self.__tomo_type = tomo_type
 
     def short_description(self) -> str:
-        folder_name = reduce_file_path(os.path.basename(self.folder))
         return ParseResult(
-            scheme="",
-            path=join_path((self.tomo_type, folder_name)),
+            scheme=self.scheme,
+            path=join_path((self.tomo_type, os.path.basename(self.folder))),
             query=None,
             netloc=None,
             params=None,
             fragment=None,
         ).geturl()
 
     @property
@@ -99,18 +98,17 @@
 
     def short_description(self) -> str:
         query = []
         if self.file_prefix not in (None, ""):
             query.append(
                 ("file_prefix", self.file_prefix),
             )
-        file_path = reduce_file_path(self.folder)
         return ParseResult(
-            scheme="",
-            path=join_path((self.tomo_type, file_path)),
+            scheme=self.scheme,
+            path=join_path((self.tomo_type, self.folder)),
             query=join_query(query),
             netloc=None,
             params=None,
             fragment=None,
         ).geturl()
 
     @property
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/hdf5Identifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/hdf5Identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "10/01/2022"
 
 
+import os
 from urllib.parse import ParseResult, urlparse
+
 from tomoscan.esrf.identifier.url_utils import (
     UrlSettings,
     join_path,
     join_query,
     split_path,
     split_query,
-    reduce_file_path,
 )
 from tomoscan.identifier import ScanIdentifier, VolumeIdentifier
-import os
 from tomoscan.utils import docstring
 
 
 class _HDF5IdentifierMixIn:
     def __init__(self, object, hdf5_file, entry, tomo_type):
         super().__init__(object)
         self._file_path = os.path.realpath(os.path.abspath(hdf5_file))
@@ -51,19 +51,18 @@
 
     @property
     def tomo_type(self):
         return self._tomo_type
 
     @docstring(ScanIdentifier)
     def short_description(self) -> str:
-        file_name = reduce_file_path(os.path.basename(self._file_path))
         return ParseResult(
-            scheme="",
+            scheme=self.scheme,
             path=join_path(
-                (self.tomo_type, file_name),
+                (self.tomo_type, os.path.basename(self._file_path)),
             ),
             query=join_query(
                 ((UrlSettings.DATA_PATH_KEY, self.data_path),),
             ),
             netloc=None,
             params=None,
             fragment=None,
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/jp2kidentifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/jp2kidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/rawidentifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/rawidentifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,31 +24,30 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "04/07/2022"
 
 
-from tomoscan.identifier import VolumeIdentifier
 import os
+
+from tomoscan.identifier import VolumeIdentifier
 from tomoscan.utils import docstring
-from tomoscan.esrf.identifier.url_utils import reduce_file_path
 
 
 class RawVolumeIdentifier(VolumeIdentifier):
     """Identifier for the .vol volume"""
 
     def __init__(self, object, file_path):
         super().__init__(object)
         self._file_path = os.path.realpath(os.path.abspath(file_path))
 
     @docstring(VolumeIdentifier)
     def short_description(self) -> str:
-        file_path = reduce_file_path(os.path.basename(self._file_path))
-        return f"{self.tomo_type}:{file_path}"
+        return f"{self.scheme}:{self.tomo_type}:{os.path.basename(self._file_path)}"
 
     @property
     def file_path(self):
         return self._file_path
 
     @property
     @docstring(VolumeIdentifier)
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/tiffidentifier.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/tiffidentifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "01/02/2022"
 
 
+import os
+
 from tomoscan.esrf.identifier.folderidentifier import (
     BaseFolderAndfilePrefixIdentifierMixIn,
 )
 from tomoscan.identifier import VolumeIdentifier
-import os
 from tomoscan.utils import docstring
-from tomoscan.esrf.identifier.url_utils import reduce_file_path
 
 
 class TIFFVolumeIdentifier(BaseFolderAndfilePrefixIdentifierMixIn, VolumeIdentifier):
     """Identifier specific to (single frame) tiff volume"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs, tomo_type=VolumeIdentifier.TOMO_TYPE)
@@ -64,16 +64,15 @@
 class MultiTiffVolumeIdentifier(VolumeIdentifier):
     def __init__(self, object, tiff_file):
         super().__init__(object)
         self._file_path = os.path.realpath(os.path.abspath(tiff_file))
 
     @docstring(VolumeIdentifier)
     def short_description(self) -> str:
-        file_path = reduce_file_path(os.path.basename(self._file_path))
-        return f"{self.tomo_type}:{file_path}"
+        return f"{self.scheme}:{self.tomo_type}:{os.path.basename(self._file_path)}"
 
     @property
     def file_path(self):
         return self._file_path
 
     @property
     @docstring(VolumeIdentifier)
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/identifier/url_utils.py` & `tomoscan-1.3.0a0/tomoscan/esrf/identifier/url_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,17 +69,7 @@
     if not isinstance(path_items, tuple):
         raise TypeError
     return ":".join(path_items)
 
 
 def split_path(path: str):
     return path.split(":")
-
-
-def reduce_file_path(file_path):
-    """
-    util used by the short_description in order to display only the beginning and the end of a string
-    it this one is longer than the expected value
-    """
-    if len(file_path) > 23:
-        file_path = f"{file_path[:10]}...{file_path[-10:]}"
-    return file_path
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/edfscan.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/edfscan.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,36 +26,36 @@
 
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "10/10/2019"
 
 
-import os
-import re
-import fabio
 import copy
-from lxml import etree
-import json
 import io
-from typing import Union, Iterable, Optional
+import json
+import logging
+import os
+import re
+from typing import Iterable, Optional, Union
 
+import fabio
 import numpy
-
+from lxml import etree
 from silx.io.url import DataUrl
 from silx.utils.deprecation import deprecated
+
 from tomoscan.esrf.identifier.edfidentifier import EDFTomoScanIdentifier
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.scanbase import Source
-from .utils import get_parameters_frm_par_or_info, extract_urls_from_edf
+from tomoscan.identifier import ScanIdentifier
+from tomoscan.scanbase import Source, TomoScanBase
 from tomoscan.unitsystem.metricsystem import MetricSystem
 from tomoscan.utils import docstring
+
 from .framereducer import EDFFrameReducer
-import logging
-from tomoscan.identifier import ScanIdentifier
+from .utils import extract_urls_from_edf, get_parameters_frm_par_or_info
 
 _logger = logging.getLogger(__name__)
 
 
 class EDFTomoScan(TomoScanBase):
     """
     TomoScanBase instanciation for scan defined from .edf files
@@ -908,15 +908,15 @@
         def get_next_free_index(key, keys):
             """return next free key from keys by converting it to a string
             with `key_value (n)` after it
             """
             new_key = key
             index = 2
             while new_key in keys:
-                new_key = "%s (%s)" % (key, index)
+                new_key = f"{key} ({index})"
                 index += 1
             return new_key
 
         def ignore_file(file_name, to_ignore):
             if to_ignore is None:
                 return False
             for pattern in to_ignore:
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/edfframereducer.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/edfframereducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,26 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "04/01/2022"
 
 
-from typing import Optional
-from tomoscan.framereducerbase import (
-    REDUCER_TARGET,
-    FrameReducerBase,
-    ReduceMethod,
-)
-from tomoscan.scanbase import TomoScanBase, ReducedFramesInfos
-from lxml import etree
-import os
-import numpy
-import fabio
 import logging
+import os
 import re
 from glob import glob
+from typing import Optional
+
+import fabio
+import numpy
+from lxml import etree
+
+from tomoscan.framereducerbase import REDUCER_TARGET, FrameReducerBase, ReduceMethod
+from tomoscan.scanbase import ReducedFramesInfos, TomoScanBase
 
 _logger = logging.getLogger(__name__)
 
 
 class EDFFrameReducer(FrameReducerBase):
     RAW_FLAT_RE = "ref*.*[0-9]{3,4}_[0-9]{3,4}"
     """regular expression to discover flat files"""
@@ -273,20 +271,20 @@
                         self.out_prefix.rstrip(self._file_ext)
                         + self.serievec[i]
                         + self._file_ext
                     )
                 fileName = os.path.join(directory, fileName)
                 if os.path.isfile(fileName):
                     if self.overwrite is False:
-                        _logger.info("skip creation of %s, already existing" % fileName)
+                        _logger.info(f"skip creation of {fileName}, already existing")
                         continue
 
                 if self.nFilePerSerie == 1:
                     fSerieName = os.path.join(directory, self.series[i])
-                    header = {"method": self.reduced_method.name + " on 1 image"}
+                    header = {"method": f"{self.reduced_method.name} on 1 image"}
                     header["SRCUR"] = self.get_closest_SR_current(
                         scan_dir=directory, refFile=fSerieName
                     )
                     header["Count_time"] = self.get_closest_count_time(
                         scan_dir=directory,
                         refFile=fSerieName,
                     )
@@ -340,16 +338,15 @@
                     data = largeMat[0]
                 elif self.reduced_method is ReduceMethod.LAST:
                     data = largeMat[-1]
                 elif self.reduced_method is ReduceMethod.NONE:
                     return
                 else:
                     raise ValueError(
-                        "Unrecognized calculation type request {}"
-                        "".format(self.reduced_method)
+                        f"Unrecognized calculation type request {self.reduced_method}"
                     )
 
                 if (
                     self.reducer_target is REDUCER_TARGET.DARKS and self.nacq > 1
                 ):  # and self.nframes == 1:
                     nacq = self.getDARK_N(directory) or 1
                     data = data / nacq
@@ -414,16 +411,15 @@
             for _file in self.filelist_fullname
         ]
         self.fileNameList = sorted(self.fileNameList)
         self.nfiles = len(self.filelist_fullname)
         # if nothing to process
         if self.nfiles == 0:
             _logger.info(
-                "no %s for %s, because no file to compute found"
-                % (self.reducer_target, directory)
+                f"no {self.reducer_target} for {directory}, because no file to compute found"
             )
             return False
 
         self.fid = fabio.open(self.filelist_fullname[0])
         self.nframes = self.fid.nframes
         self.nacq = 0
         # get the info of number of acquisitions
@@ -504,15 +500,15 @@
         serieFiles = {}
         unattributedFiles = files.copy()
         for serie in series:
             serieFiles[serie] = findFileEndingWithSerie(unattributedFiles, serie)
             [unattributedFiles.remove(_f) for _f in serieFiles[serie]]
 
         if len(unattributedFiles) > 0:
-            _logger.error("Failed to associate %s to any serie" % unattributedFiles)
+            _logger.error(f"Failed to associate {unattributedFiles} to any serie")
             return {}, 0
 
         checkSeriesFilesLength(serieFiles)
 
         return serieFiles, len(serieFiles[list(serieFiles.keys())[0]])
 
     @staticmethod
@@ -585,15 +581,15 @@
             )
             return None, None
         assert len(serievec) <= 2
         if len(serievec) > 1:
             key = serievec[-1]
             tomoN = self.getTomo_N(self.scan)
             if tomoN is None:
-                _logger.error("Fail to found information %s. Can't find TOMO_N")
+                _logger.error("Fail to found information TOMO_N")
             del serievec[-1]
             serievec.append(str(tomoN).zfill(4))
             filesPerSerie[serievec[-1]] = filesPerSerie[key]
             del filesPerSerie[key]
             assert len(serievec) == 2
             assert len(filesPerSerie) == 2
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/hdf5framereducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,23 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "04/01/2022"
 
 
+import logging
+
+import numpy
 from silx.io.url import DataUrl
-from tomoscan.framereducerbase import (
-    REDUCER_TARGET,
-    FrameReducerBase,
-    ReduceMethod,
-)
+from silx.io.utils import get_data
+
 from tomoscan.esrf.scan.utils import get_compacted_dataslices
+from tomoscan.framereducerbase import REDUCER_TARGET, FrameReducerBase, ReduceMethod
 from tomoscan.scanbase import ReducedFramesInfos
-from silx.io.utils import get_data
-import numpy
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class HDF5FrameReducer(FrameReducerBase):
     """Frame reducer dedicated to HDF5"""
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/hdf5scan.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/hdf5scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,38 +26,39 @@
 
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "09/08/2018"
 
 
-from silx.utils.deprecation import deprecated
-from tomoscan.esrf.scan.framereducer.hdf5framereducer import HDF5FrameReducer
-from tomoscan.unitsystem import electriccurrentsystem, energysystem, timesystem
-from tomoscan.scanbase import TomoScanBase, FOV
-from tomoscan.scanbase import Source
-import json
 import io
+import json
+import logging
 import os
+import typing
+
 import h5py
 import numpy
 from silx.io.url import DataUrl
+from silx.io.utils import get_data, h5py_read_dataset
+from silx.utils.deprecation import deprecated
 from silx.utils.enum import Enum as _Enum
-from tomoscan.utils import BoundingBox1D, BoundingBox3D, docstring
-from tomoscan.io import HDF5File
-from tomoscan.identifier import ScanIdentifier
+
 from tomoscan.esrf.identifier.hdf5Identifier import HDF5TomoScanIdentifier
-from silx.io.utils import get_data
-from tomoscan.unitsystem.unit import Unit
-from tomoscan.unitsystem.metricsystem import MetricSystem
+from tomoscan.esrf.scan.framereducer.hdf5framereducer import HDF5FrameReducer
+from tomoscan.identifier import ScanIdentifier
+from tomoscan.io import HDF5File
 from tomoscan.nexus.paths.nxtomo import get_paths as _get_nexus_paths
+from tomoscan.scanbase import FOV, Source, TomoScanBase
+from tomoscan.unitsystem import electriccurrentsystem, energysystem, timesystem
+from tomoscan.unitsystem.metricsystem import MetricSystem
+from tomoscan.unitsystem.unit import Unit
+from tomoscan.utils import BoundingBox1D, BoundingBox3D, docstring
+
 from .utils import get_compacted_dataslices
-from silx.io.utils import h5py_read_dataset
-import typing
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class ImageKey(_Enum):
     ALIGNMENT = -1
     PROJECTION = 0
@@ -166,17 +167,15 @@
         if scan is None:
             self._entry = None
         else:
             self._entry = entry or self._get_entry_at(
                 index=index, file_path=self.master_file
             )
             if self._entry is None:
-                raise ValueError(
-                    "unable to find a valid entry for %s" % self.master_file
-                )
+                raise ValueError(f"unable to find a valid entry for {self.master_file}")
         # for now the default entry is 1_tomo but should change with time
         self._name = None
         self._sample_name = None
         self._grp_size = None
         # data caches
         self._projections_compacted = None
         self._flats = None
@@ -666,15 +665,15 @@
 
     @property
     @deprecated(replacement="count_time", since_version="1.0.0")
     def exposure_time(self) -> typing.Optional[list]:
         return self.count_time
 
     @property
-    def electric_current(self) -> dict:
+    def electric_current(self) -> typing.Optional[list]:
         return self._get_generic_key(
             "_electric_current",
             self.nexus_path.ELECTRIC_CURRENT_PATH,
             unit=electriccurrentsystem.ElectricCurrentSystem.AMPERE,
         )
 
     @property
@@ -972,30 +971,14 @@
 
     @property
     def intensity_monitor(self):
         return self._get_generic_key(
             "_intensity_monitor", self.nexus_path.INTENSITY_MONITOR_PATH
         )
 
-    @staticmethod
-    def _is_return_frame(
-        img_key, lframe, llast_proj_frame, ldelta_angle, return_already_reach
-    ) -> tuple:
-        """return is_return, delta_angle"""
-        if ImageKey.from_value(img_key) is not ImageKey.PROJECTION:
-            return False, None
-        if ldelta_angle is None and llast_proj_frame is not None:
-            delta_angle = lframe.rotation_angle - llast_proj_frame.rotation_angle
-            return False, delta_angle
-        elif return_already_reach:
-            return True, ldelta_angle
-        else:
-            current_angle = lframe.rotation_angle - llast_proj_frame.rotation_angle
-            return abs(current_angle) <= 2 * ldelta_angle, ldelta_angle
-
     @property
     def frames(self) -> typing.Optional[tuple]:
         """return tuple of frames. Frames contains"""
         if self._frames is None:
             image_keys = self.image_key
             rotation_angles = self.rotation_angle
             x_translation = self.x_translation
@@ -1008,24 +991,19 @@
             if z_translation is None and image_keys is not None:
                 z_translation = [None] * len(image_keys)
             intensity_monitor = self.intensity_monitor
             if intensity_monitor is None and image_keys is not None:
                 intensity_monitor = [None] * len(image_keys)
             if image_keys is not None and len(image_keys) != len(rotation_angles):
                 raise ValueError(
-                    "`rotation_angle` and `image_key` have "
-                    "incoherent size (%s vs %s). Unable to "
-                    "deduce frame properties" % (len(rotation_angles), len(image_keys))
+                    "`rotation_angle` and `image_key` have incoherent size "
+                    f"({len(rotation_angles)} vs {len(image_keys)}). Unable to deduce frame properties"
                 )
             self._frames = []
 
-            delta_angle = None
-            last_proj_frame = None
-            return_already_reach = False
-
             if image_keys is None:
                 # in the case there is no frame / image keys registered at all
                 return self._frames
 
             for i_frame, rot_a, img_key, x_tr, y_tr, z_tr, i_m in zip(
                 range(len(rotation_angles)),
                 rotation_angles,
@@ -1062,25 +1040,20 @@
                         )
                     except Exception:
                         _logger.warning(
                             f"Unable to deduce if {frame.index} is a control frame. Consider it is not"
                         )
                         is_control_frame = False
                 else:
-                    return_already_reach, delta_angle = self._is_return_frame(
-                        img_key=img_key,
-                        lframe=frame,
-                        llast_proj_frame=last_proj_frame,
-                        ldelta_angle=delta_angle,
-                        return_already_reach=return_already_reach,
-                    )
-                    is_control_frame = return_already_reach
+                    # if there is no image_key_control it is ambiguous to determine which
+                    # projection is a return or not. Even if an angle is repeated this wouldn't be sure at 100%
+                    # so the better is to consider there is no return / alignment projection
+                    is_control_frame = False
                 frame.is_control = is_control_frame
                 self._frames.append(frame)
-                last_proj_frame = frame
             self._frames = tuple(self._frames)
         return self._frames
 
     @docstring(TomoScanBase.get_proj_angle_url)
     def get_proj_angle_url(self) -> typing.Optional[dict]:
         if self.frames is not None:
             res = {}
@@ -1109,15 +1082,15 @@
         **kwargs,
     ) -> numpy.array:
         if (
             len(self.projections) is not None
             and self.dim_2 is not None
             and line > self.dim_2
         ) or line < 0:
-            raise ValueError("requested line {} is not in the scan".format(line))
+            raise ValueError(f"requested line {line} is not in the scan")
 
         if not isinstance(subsampling, int):
             raise TypeError("subsampling expected to be an int")
         if subsampling <= 0:
             raise ValueError("subsampling expected to be higher than 1")
 
         if self.projections is not None:
@@ -1191,18 +1164,16 @@
         :rtype: dict
         """
         if self._projections_compacted is None:
             self._projections_compacted = get_compacted_dataslices(self.projections)
         return self._projections_compacted
 
     def __str__(self):
-        return "hdf5 scan(master_file: %s, entry: %s)" % (
-            os.sep.join(os.path.abspath(self.master_file).split(os.sep)[-3:]),
-            self.entry,
-        )
+        file_id = os.sep.join(os.path.abspath(self.master_file).split(os.sep)[-3:])
+        return f"hdf5 scan(master_file: {file_id}, entry: {self.entry})"
 
     @staticmethod
     def _get_value(node: h5py.Group, default_unit: Unit):
         """convert the value contained in the node to the adapted unit.
         Unit can be defined in on of the group attributes. It it is the case
         will pick this unit, otherwise will use the default unit
         """
@@ -1226,16 +1197,15 @@
         if self.master_file is None:
             raise ValueError("No master file provided")
         if self.entry is None:
             raise ValueError("No entry provided")
         with HDF5File(self.master_file, "r") as h5_file:
             if self._entry not in h5_file:
                 raise ValueError(
-                    "Given entry %s is not in the master "
-                    "file %s" % (self._entry, self.master_file)
+                    f"Given entry {self._entry} is not in the master file {self.master_file}"
                 )
 
     def get_flat_expected_location(self):
         return DataUrl(
             file_path=self.master_file,
             data_path=_get_nexus_paths(self.nexus_version).PROJ_PATH,
         ).path()
@@ -1460,23 +1430,19 @@
             if rocking is None and image_keys is not None:
                 rocking = [None] * len(image_keys)
             base_tilt = self.base_tilt
             if base_tilt is None and image_keys is not None:
                 base_tilt = [None] * len(image_keys)
             if image_keys is not None and len(image_keys) != len(rotation_angles):
                 raise ValueError(
-                    "`rotation_angle` and `image_key` have "
-                    "incoherent size (%s vs %s). Unable to "
-                    "deduce frame properties" % (len(rotation_angles), len(image_keys))
+                    "`rotation_angle` and `image_key` have incoherent size "
+                    f"({len(rotation_angles)} vs {len(image_keys)}). Unable to deduce frame properties"
                 )
             self._frames = []
 
-            delta_angle = None
-            last_proj_frame = None
-            return_already_reach = False
             for i_frame, rot_a, img_key, x_tr, y_tr, z_tr, rck, bt in zip(
                 range(len(rotation_angles)),
                 rotation_angles,
                 image_keys,
                 x_translation,
                 y_translation,
                 z_translation,
@@ -1515,25 +1481,19 @@
                         )
                     except Exception:
                         _logger.warning(
                             f"Unable to deduce if {frame.index} is a control frame. Consider it is not"
                         )
                         is_control_frame = False
                 else:
-                    return_already_reach, delta_angle = self._is_return_frame(
-                        img_key=img_key,
-                        lframe=frame,
-                        llast_proj_frame=last_proj_frame,
-                        ldelta_angle=delta_angle,
-                        return_already_reach=return_already_reach,
-                    )
-                    is_control_frame = return_already_reach
+                    # if there is no image_key_control then we consider it is
+                    # unsafe to determine what is a return / alignment frame
+                    is_control_frame = False
                 frame._is_control_frame = is_control_frame
                 self._frames.append(frame)
-                last_proj_frame = frame
             self._frames = tuple(self._frames)
         return self._frames
 
 
 class TomoFrame:
     """class to store all metadata information of a NXTomo frame"""
 
@@ -1670,11 +1630,9 @@
 
     @property
     def base_tilt(self) -> typing.Optional[float]:
         return self._base_tilt
 
     def __str__(self):
         p_str = super(XRD3DFrame, self).__str__()
-        p_str += "rocking: {rocking}," "base-tilt: {base_tilt}".format(
-            rocking=self.rocking, base_tilt=self.base_tilt
-        )
+        p_str += f"rocking: {self.rocking}, base-tilt: {self.base_tilt}"
         return p_str
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/mock.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,28 @@
 Utils to mock scans
 """
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "30/09/2019"
 
-import h5py
-import numpy
+import logging
 import os
 from xml.etree import cElementTree
+
 import fabio
 import fabio.edfimage
-from .hdf5scan import ImageKey, HDF5TomoScan
-from tomoscan.esrf.volume.hdf5volume import HDF5Volume
+import h5py
+import numpy
 from silx.io.utils import h5py_read_dataset
+
+from tomoscan.esrf.volume.hdf5volume import HDF5Volume
+
+from .hdf5scan import HDF5TomoScan, ImageKey
 from .utils import dump_info_file
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class ScanMock:
     """Base class to mock as scan (radios, darks, flats, reconstructions...)"""
 
@@ -152,15 +155,15 @@
                 return r
 
             radii = _compute_radius_to_center(background)
             scale = 1
             background[radii < radius * scale] = 1.0
             return background
         else:
-            raise ValueError("selected scene %s is no managed" % self.scene)
+            raise ValueError(f"selected scene {self.scene} is no managed")
 
 
 class MockHDF5(ScanMock):
     """
     Mock an acquisition in a hdf5 file.
 
     note: for now the Mock class only manage one initial flat and one final
@@ -716,17 +719,15 @@
     def add_radio(self, index=None):
         if index is not None:
             self._last_radio_index = index
             index_ = index
         else:
             self._last_radio_index += 1
             index_ = self._last_radio_index
-        file_name = (
-            os.path.basename(self.scan_path) + "_{0:04d}".format(index_) + ".edf"
-        )
+        file_name = f"{os.path.basename(self.scan_path)}_{index_:04}.edf"
         f = os.path.join(self.scan_path, file_name)
         if not os.path.exists(f):
             if index_ < len(self._proj_rotation_angles):
                 rotation_angle = self._proj_rotation_angles[index_]
             else:
                 rotation_angle = 0.0
             if index_ < len(self._srcurrent):
@@ -744,15 +745,15 @@
                     "counter_pos": f"{srcurrent};",
                     "counter_mne": "srcur;",
                 },
             )
             edf_writer.write(f)
 
     def add_dark(self, index):
-        file_name = "darkend{0:04d}.edf".format(index)
+        file_name = f"darkend{index:04}.edf"
         file_path = os.path.join(self.scan_path, file_name)
         if not os.path.exists(file_path):
             data = numpy.random.random((self.det_height * self.det_width)).reshape(
                 (self.det_width, self.det_height)
             )
             edf_writer = fabio.edfimage.EdfImage(
                 data=data,
@@ -762,15 +763,15 @@
                     "counter_pos": f"{self._srcurrent[0]};",
                     "counter_mne": "srcur;",
                 },
             )
             edf_writer.write(file_path)
 
     def add_flat(self, index):
-        file_name = "refHST{0:04d}.edf".format(index)
+        file_name = f"refHST{index:04}.edf"
         file_path = os.path.join(self.scan_path, file_name)
         if not os.path.exists(file_path):
             data = numpy.random.random((self.det_height * self.det_width)).reshape(
                 (self.det_width, self.det_height)
             )
             edf_writer = fabio.edfimage.EdfImage(
                 data=data,
@@ -838,25 +839,25 @@
     ):
         assert len(shape) == 3
         f = open(filePath, "w")
         f.writelines(
             "\n".join(
                 [
                     "! PyHST_SLAVE VOLUME INFO FILE",
-                    "NUM_X =  %s" % shape[2],
-                    "NUM_Y =  %s" % shape[1],
-                    "NUM_Z =  %s" % shape[0],
-                    "voxelSize =  %s" % voxelSize,
+                    f"NUM_X =  {shape[2]}",
+                    f"NUM_Y =  {shape[1]}",
+                    f"NUM_Z =  {shape[0]}",
+                    f"voxelSize =  {voxelSize}",
                     "BYTEORDER = LOWBYTEFIRST",
-                    "ValMin =  %s" % valMin,
-                    "ValMax =  %s" % valMax,
-                    "s1 =  %s" % s1,
-                    "s2 =  %s" % s2,
-                    "S1 =  %s" % S1,
-                    "S2 =  %s" % S2,
+                    f"ValMin =  {valMin}",
+                    f"ValMax =  {valMax}",
+                    f"s1 =  {s1}",
+                    f"s2 =  {s2}",
+                    f"S1 =  {S1}",
+                    f"S2 =  {S2}",
                 ]
             )
         )
         f.close()
 
     @staticmethod
     def fastMockAcquisition(folder, n_radio=20, n_extra_radio=0, scan_range=360):
@@ -876,15 +877,15 @@
             # write the info file
             with open(info_file, "w") as info_file:
                 info_file.write("TOMO_N=                 " + str(n_radio) + "\n")
                 info_file.write("ScanRange=                 " + str(scan_range) + "\n")
 
         # create scan files
         for i in range((n_radio + n_extra_radio)):
-            file_name = basename + "_{0:04d}".format(i) + ".edf"
+            file_name = f"{basename}_{i:04}.edf"
             f = os.path.join(folder, file_name)
             if not os.path.exists(f):
                 data = numpy.random.random(dim * dim).reshape(dim, dim)
                 edf_writer = fabio.edfimage.EdfImage(data=data, header={"tata": "toto"})
                 edf_writer.write(f)
 
         # create xml file
@@ -975,28 +976,28 @@
                 data=end_flat_data,
             )
 
         return Factory.create_scan_object(scanID)
 
     @staticmethod
     def add_flat_serie(scan_path, n_elmt, index, dim, data):
-        ref_file = os.path.join(scan_path, "ref0000_{}.edf".format(str(index).zfill(4)))
+        ref_file = os.path.join(scan_path, f"ref0000_{index:04}.edf")
         if data is None:
             data = numpy.array(
                 numpy.random.random(n_elmt * dim * dim) * 100, numpy.uint32
             )
         data.shape = (n_elmt, dim, dim)
         edf_writer = fabio.edfimage.EdfImage(data=data[0], header={"tata": "toto"})
         for frame in data[1:]:
             edf_writer.append_frame(data=frame)
         edf_writer.write(ref_file)
 
     @staticmethod
     def add_dark_serie(scan_path, n_elmt, index, dim, data):
-        dark_file = os.path.join(scan_path, "darkend{}.edf".format(str(index).zfill(4)))
+        dark_file = os.path.join(scan_path, f"darkend{index:04}.edf")
         if data is None:
             data = numpy.array(
                 numpy.random.random(n_elmt * dim * dim) * 100, numpy.uint32
             )
         data.shape = (n_elmt, dim, dim)
         edf_writer = fabio.edfimage.EdfImage(data=data[0], header={"tata": "toto"})
         for frame in data[1:]:
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/scan/utils.py` & `tomoscan-1.3.0a0/tomoscan/esrf/scan/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,34 +24,34 @@
 
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "10/10/2019"
 
 
-import os
-import fabio
-from silx.io.url import DataUrl
-from silx.utils.deprecation import deprecated
-from silx.io.utils import h5py_read_dataset, get_data as silx_get_data
-from silx.io.dictdump import h5todict
-from typing import Union
-from typing import Iterable
-import numpy
+import contextlib
+import fnmatch
 import logging
+import os
 import sys
-from tomoscan.io import HDF5File
 import warnings
-import contextlib
-import fnmatch
+from typing import Iterable, Union
+
+import fabio
 import h5py
+import numpy
+from silx.io.dictdump import h5todict
+from silx.io.url import DataUrl
+from silx.io.utils import get_data as silx_get_data
+from silx.io.utils import h5py_read_dataset
+from silx.utils.deprecation import deprecated
 
+from tomoscan.io import HDF5File
 from tomoscan.scanbase import ReducedFramesInfos, TomoScanBase
 
-
 _logger = logging.getLogger(__name__)
 
 
 def get_parameters_frm_par_or_info(file_: str) -> dict:
     """
     Create a dictionary from the file with the information name as keys and
     their values as values
@@ -73,15 +73,15 @@
         if "#" in line_:
             line_ = line_.split("#")[0]
         if line_ == "":
             continue
         try:
             key, value = line_.split("=")
         except ValueError:
-            raise ValueError('fail to extract information from "%s"' % line_)
+            raise ValueError(f"fail to extract information from {line_}")
         else:
             # try to cast the value on int, else float else don't
             try:
                 value = int(value)
             except Exception:
                 try:
                     value = float(value)
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/__init__.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 # ###########################################################################*/
 
 """This module is dedicated to instances of :class:`VolumeBase` used at esrf"""
 
 from .edfvolume import EDFVolume  # noqa F401
 from .hdf5volume import HDF5Volume  # noqa F401
 from .jp2kvolume import JP2KVolume  # noqa F401
-from .tiffvolume import MultiTIFFVolume, TIFFVolume  # noqa F401
 from .rawvolume import RawVolume  # noqa F401
+from .tiffvolume import MultiTIFFVolume, TIFFVolume  # noqa F401
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/edfvolume.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/edfvolume.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
+import os
 from typing import Optional
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.esrf.volume.singleframebase import VolumeSingleFrameBase
-from tomoscan.esrf.identifier.edfidentifier import EDFVolumeIdentifier
+
+import fabio
 import numpy
 from silx.io.url import DataUrl
+
+from tomoscan.esrf.identifier.edfidentifier import EDFVolumeIdentifier
+from tomoscan.esrf.volume.singleframebase import VolumeSingleFrameBase
+from tomoscan.scanbase import TomoScanBase
 from tomoscan.utils import docstring
-import fabio
-import os
 
 
 class EDFVolume(VolumeSingleFrameBase):
     """
     Save volume data to single frame edf and metadata to .txt files
 
     :warning: each file saved under {volume_basename}_{index_zfill6}.edf is considered to be a slice of the volume.
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/hdf5volume.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/hdf5volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
+import logging
 import os
 from typing import Optional
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.volumebase import VolumeBase
-from tomoscan.esrf.identifier.hdf5Identifier import HDF5VolumeIdentifier
-from silx.io.url import DataUrl
-from tomoscan.utils import docstring
-from tomoscan.io import HDF5File
+
+import h5py
+import numpy
 from silx.io.dictdump import dicttonx, nxtodict
+from silx.io.url import DataUrl
 from silx.utils.deprecation import deprecated_warning
-import numpy
-import logging
-import h5py
+
+from tomoscan.esrf.identifier.hdf5Identifier import HDF5VolumeIdentifier
+from tomoscan.io import HDF5File
+from tomoscan.scanbase import TomoScanBase
+from tomoscan.utils import docstring
+from tomoscan.volumebase import VolumeBase
 
 _logger = logging.getLogger(__name__)
 
 
 class HDF5Volume(VolumeBase):
     """
     Volume where both data and metadata are store in a HDF5 file but at a different location.
@@ -457,26 +459,26 @@
             .get_identifier()
             .to_str()
         )
 
     @docstring(VolumeBase)
     def browse_slices(self, url=None):
         if url is None and self.data is not None:
-            for slice in self.data:
-                yield slice
+            for data_slice in self.data:
+                yield data_slice
         else:
             url = url or self.data_url
             if url is None:
                 raise ValueError(
                     "No data and data_url know and no url provided. Uanble to browse slices"
                 )
             with HDF5File(filename=url.file_path(), mode="r") as h5s:
                 if url.data_path() in h5s:
-                    for slice in h5s[url.data_path()]:
-                        yield slice
+                    for data_slice in h5s[url.data_path()]:
+                        yield data_slice
                 else:
                     raise KeyError(f"Data path {url.data_path()} not found.")
 
     @docstring(VolumeBase)
     def load_chunk(self, chunk, url=None):
         url = url or self.data_url
         if url is None:
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/jp2kvolume.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/jp2kvolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,40 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
-from typing import Optional
+import logging
 import os
+from typing import Optional
+
 import numpy
+from packaging.version import parse as parse_version
+from silx.io.url import DataUrl
+
 from tomoscan.esrf.identifier.jp2kidentifier import JP2KVolumeIdentifier
 from tomoscan.scanbase import TomoScanBase
-from .singleframebase import VolumeSingleFrameBase
-from silx.io.url import DataUrl
-from packaging.version import parse as parse_version
 from tomoscan.utils import docstring
-import logging
+
+from .singleframebase import VolumeSingleFrameBase
 
 try:
     import glymur  # noqa #F401 needed for later possible lazy loading
 except ImportError:
     has_glymur = False
     has_minimal_openjpeg = False
     glymur_version = None
     openjpeg_version = None
 else:
     has_glymur = True
     from glymur import set_option as glymur_set_option
-    from glymur.version import openjpeg_version, version as glymur_version
+    from glymur.version import openjpeg_version
+    from glymur.version import version as glymur_version
 
     if openjpeg_version < "2.3.0":
         has_minimal_openjpeg = False
     else:
         has_minimal_openjpeg = True
 
 _logger = logging.getLogger(__name__)
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/mock.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 # THE SOFTWARE.
 #
 # ###########################################################################*/
 """module to mock volume"""
 
 
 from typing import Sized, Union
+
 import numpy
-from silx.utils.enum import Enum as _Enum
 from silx.image.phantomgenerator import PhantomGenerator
+from silx.utils.enum import Enum as _Enum
 
 
 class Scene(_Enum):
     SHEPP_LOGAN = "Shepp-Logan"
 
 
 def create_volume(
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/rawvolume.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/rawvolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,30 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "10/01/2023"
 
 
-import sys
-import os
-from xml.dom.minidom import parseString as parse_xml_string
 import logging
+import os
+import sys
 from typing import Optional
-import numpy
+from xml.dom.minidom import parseString as parse_xml_string
+
 import h5py
+import numpy
 from dicttoxml import dicttoxml
-from silx.io.url import DataUrl
 from silx.io.dictdump import dicttoini
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.volumebase import VolumeBase
+from silx.io.url import DataUrl
+
 from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
+from tomoscan.scanbase import TomoScanBase
 from tomoscan.utils import docstring
+from tomoscan.volumebase import VolumeBase
 
 _logger = logging.getLogger(__name__)
 
 
 class RawVolume(VolumeBase):
     """
     Volume where data si saved under .vol binary file and metadata are saved in .vol.info and or .vol.xml
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/singleframebase.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/singleframebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,24 +26,27 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
-from typing import Optional
+import logging
 import os
 import re
+from typing import Optional
+
 import numpy
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.volumebase import VolumeBase
+from silx.io.dictdump import dicttoini
+from silx.io.dictdump import load as load_ini
 from silx.io.url import DataUrl
-from silx.io.dictdump import dicttoini, load as load_ini
+
+from tomoscan.scanbase import TomoScanBase
 from tomoscan.utils import docstring
-import logging
+from tomoscan.volumebase import VolumeBase
 
 _logger = logging.getLogger(__name__)
 
 
 class VolumeSingleFrameBase(VolumeBase):
     """
     Base class for Volume where each slice is saved in a separate file like edf, jp2k or tiff.
@@ -392,16 +395,16 @@
                 file_path=data_file,
                 scheme=url.scheme(),
             )
 
     @docstring(VolumeBase)
     def browse_slices(self, url=None):
         if url is None and self.data is not None:
-            for slice in self.data:
-                yield slice
+            for data_slice in self.data:
+                yield data_slice
         else:
             url = url or self.data_url
             if url is None:
                 raise ValueError(
                     "No data and data_url know and no url provided. Uanble to browse slices"
                 )
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/tiffvolume.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/tiffvolume.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,29 @@
 
 
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "01/02/2022"
 
 
+import os
 from typing import Optional
+
 import numpy
+from silx.io.dictdump import dicttoini
+from silx.io.dictdump import load as load_ini
+from silx.io.url import DataUrl
+
 from tomoscan.esrf.identifier.tiffidentifier import (
     MultiTiffVolumeIdentifier,
     TIFFVolumeIdentifier,
 )
-from tomoscan.scanbase import TomoScanBase
 from tomoscan.esrf.volume.singleframebase import VolumeSingleFrameBase
+from tomoscan.scanbase import TomoScanBase
 from tomoscan.utils import docstring, get_subvolume_shape
-from silx.io.url import DataUrl
-from silx.io.dictdump import dicttoini, load as load_ini
-import os
 from tomoscan.volumebase import VolumeBase
 
 try:
     import tifffile  # noqa #F401 needed for later possible lazy loading
 except ImportError:
     has_tifffile = False
 else:
@@ -248,16 +251,16 @@
             else:
                 _logger.info(f"save data to {url.path()}")
 
             with TiffWriter(url.file_path(), bigtiff=True, append=self.append) as tif:
                 if self.data.ndim == 2:
                     tif.write(self.data)
                 elif self.data.ndim == 3:
-                    for slice in self.data:
-                        tif.write(slice)
+                    for data_slice in self.data:
+                        tif.write(data_slice)
                 else:
                     raise ValueError(f"data should be 3D and not {self.data.ndim}D")
 
         else:
             raise ValueError(f"Scheme {url.scheme()} is not handled")
 
     @docstring(VolumeBase)
@@ -408,16 +411,16 @@
                 file_path=data_file,
                 scheme=url.scheme(),
             )
 
     @docstring(VolumeBase)
     def browse_slices(self, url=None):
         if url is None and self.data is not None:
-            for slice in self.data:
-                yield slice
+            for data_slice in self.data:
+                yield data_slice
         else:
             url = url or self.data_url
             if url is None:
                 raise ValueError(
                     "No data and data_url know and no url provided. Uanble to browse slices"
                 )
             if url.scheme() == "tifffile":
@@ -425,16 +428,16 @@
                     raise ValueError("data_path is not handle by multiframe tiff")
 
                 url = url or self.data_url
                 reader = TiffFile(url.file_path())
                 for serie in reader.series:
                     data = serie.asarray()
                     if data.ndim == 3:
-                        for slice in data:
-                            yield slice
+                        for data_slice in data:
+                            yield data_slice
                     elif data.ndim == 2:
                         yield data
                     else:
                         raise ValueError("serie is expected to be 2D or 3D")
             else:
                 raise ValueError(
                     f"Scheme {url.scheme()} is not handled by multiframe tiff"
```

### Comparing `tomoscan-1.2.1/tomoscan/esrf/volume/utils.py` & `tomoscan-1.3.0a0/tomoscan/esrf/volume/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,32 +28,34 @@
 __authors__ = [
     "H. Payno",
 ]
 __license__ = "MIT"
 __date__ = "11/07/2022"
 
 
+import logging
 import os
+from typing import Optional
+
 import h5py
-from tomoscan.esrf.volume.edfvolume import EDFVolume
-from tomoscan.esrf.volume.hdf5volume import HDF5Volume
-from tomoscan.esrf.volume.tiffvolume import MultiTIFFVolume, TIFFVolume
-from tomoscan.esrf.volume.jp2kvolume import JP2KVolume
-from tomoscan.esrf.volume.rawvolume import RawVolume
+
 from tomoscan.esrf.identifier.edfidentifier import EDFVolumeIdentifier
 from tomoscan.esrf.identifier.hdf5Identifier import HDF5VolumeIdentifier
+from tomoscan.esrf.identifier.jp2kidentifier import JP2KVolumeIdentifier
+from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
 from tomoscan.esrf.identifier.tiffidentifier import (
-    TIFFVolumeIdentifier,
     MultiTiffVolumeIdentifier,
+    TIFFVolumeIdentifier,
 )
-from tomoscan.esrf.identifier.jp2kidentifier import JP2KVolumeIdentifier
-from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
+from tomoscan.esrf.volume.edfvolume import EDFVolume
+from tomoscan.esrf.volume.hdf5volume import HDF5Volume
+from tomoscan.esrf.volume.jp2kvolume import JP2KVolume
+from tomoscan.esrf.volume.rawvolume import RawVolume
+from tomoscan.esrf.volume.tiffvolume import MultiTIFFVolume, TIFFVolume
 from tomoscan.io import HDF5File
-from typing import Optional
-import logging
 
 _logger = logging.getLogger(__name__)
 
 _DEFAULT_SCHEME_TO_VOL = {
     EDFVolumeIdentifier.scheme: EDFVolume,
     HDF5VolumeIdentifier.scheme: HDF5Volume,
     TIFFVolumeIdentifier.scheme: TIFFVolume,
@@ -91,15 +93,17 @@
                         )
                     )
                 return tuple(res)
 
         return tuple()
 
 
-def guess_volumes(path, scheme_to_vol: Optional[dict] = None) -> tuple:
+def guess_volumes(
+    path, scheme_to_vol: Optional[dict] = None, filter_histograms=True
+) -> tuple:
     """
     from a file path or a folder path try to guess volume(s)
 
     :param str path: file or folder path
     :param dict scheme_to_vol: dict to know which constructor to call. Key if the scheme, value if the volume constructor.
                                usefull for libraries redefining volume or adding some like tomwer.
                                If none provided will take the tomoscan default one
@@ -119,14 +123,27 @@
                 assert isinstance(data_path, str)
                 res.append(
                     scheme_to_vol[HDF5VolumeIdentifier.scheme](
                         file_path=path,
                         data_path=data_path,
                     )
                 )
+            # filter potential 'nabu histogram'
+            # as nabu histograms looks like volume simply look at the name
+            # could also be on data ndim
+            if filter_histograms is True:
+
+                def is_not_histogram(vol_identifier):
+                    return not (
+                        hasattr(vol_identifier, "data_path")
+                        and vol_identifier.data_path.endswith("histogram")
+                    )
+
+                res = tuple(filter(is_not_histogram, res))
+
             return tuple(res)
         elif path.lower().endswith((".tif", ".tiff")):
             return (scheme_to_vol[MultiTiffVolumeIdentifier.scheme](file_path=path),)
         elif path.lower().endswith((".vol", ".raw")):
             return (scheme_to_vol[RawVolumeIdentifier.scheme](file_path=path),)
     elif os.path.isdir(path):
         most_common_extension = get_most_common_extension(path)
```

### Comparing `tomoscan-1.2.1/tomoscan/factory.py` & `tomoscan-1.3.0a0/tomoscan/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,37 +24,39 @@
 """Contains the Factory class and dedicated functions"""
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "27/02/2019"
 
 
+import os
+from typing import Union
 from urllib.parse import urlparse
+
 from tomoscan.esrf.identifier.jp2kidentifier import JP2KVolumeIdentifier
+from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
 from tomoscan.esrf.identifier.tiffidentifier import (
     MultiTiffVolumeIdentifier,
     TIFFVolumeIdentifier,
 )
-from tomoscan.esrf.identifier.rawidentifier import RawVolumeIdentifier
 from tomoscan.esrf.identifier.url_utils import split_path
 from tomoscan.esrf.volume.edfvolume import EDFVolume
 from tomoscan.esrf.volume.hdf5volume import HDF5Volume
 from tomoscan.esrf.volume.jp2kvolume import JP2KVolume
-from tomoscan.esrf.volume.tiffvolume import MultiTIFFVolume, TIFFVolume
 from tomoscan.esrf.volume.rawvolume import RawVolume
+from tomoscan.esrf.volume.tiffvolume import MultiTIFFVolume, TIFFVolume
+from tomoscan.identifier import BaseIdentifier, ScanIdentifier, VolumeIdentifier
 from tomoscan.tomoobject import TomoObject
-from .scanbase import TomoScanBase
-from .esrf.scan.edfscan import EDFTomoScan
-from .esrf.scan.hdf5scan import HDF5TomoScan
+
+from . import identifier as _identifier_mod
 from .esrf.identifier.edfidentifier import EDFTomoScanIdentifier, EDFVolumeIdentifier
 from .esrf.identifier.hdf5Identifier import HDF5TomoScanIdentifier, HDF5VolumeIdentifier
-from tomoscan.identifier import BaseIdentifier, ScanIdentifier, VolumeIdentifier
-from . import identifier as _identifier_mod
-from typing import Union
-import os
+from .esrf.scan.edfscan import EDFTomoScan
+from .esrf.scan.hdf5scan import HDF5TomoScan
+from .scanbase import TomoScanBase
 
 
 class Factory:
     """
     Factory any TomoObject
     """
 
@@ -167,15 +169,15 @@
         # remove any final separator (otherwise basename might fail)
         scan_path = scan_path.rstrip(os.path.sep)
         if EDFTomoScan.is_tomoscan_dir(scan_path):
             return EDFTomoScan(scan=scan_path)
         elif HDF5TomoScan.is_tomoscan_dir(scan_path):
             return HDF5TomoScan(scan=scan_path)
         else:
-            raise ValueError("%s is not a valid scan path" % scan_path)
+            raise ValueError(f"{scan_path} is not a valid scan path")
 
     @staticmethod
     def create_scan_objects(scan_path: str) -> tuple:
         """
 
         :param str scan_path: path to the scan directory or file
         :return: all possible instances of TomoScanBase contained in the given
@@ -189,15 +191,15 @@
             scans = []
             master_file = HDF5TomoScan.get_master_file(scan_path=scan_path)
             entries = HDF5TomoScan.get_valid_entries(master_file)
             for entry in entries:
                 scans.append(HDF5TomoScan(scan=scan_path, entry=entry, index=None))
             return tuple(scans)
 
-        raise ValueError("%s is not a valid scan path" % scan_path)
+        raise ValueError(f"{scan_path} is not a valid scan path")
 
     @staticmethod
     def create_scan_object_frm_dict(_dict: dict) -> TomoScanBase:
         """
         Create a TomoScanBase instance from a dictionary. It should contains
         the TomoScanBase._DICT_TYPE_KEY key at least.
```

### Comparing `tomoscan-1.2.1/tomoscan/framereducerbase.py` & `tomoscan-1.3.0a0/tomoscan/framereducerbase.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,34 +26,48 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "07/08/2019"
 
 
 from typing import Optional
+
+import numpy
+from numpy.core.numerictypes import generic as numy_generic
 from silx.utils.enum import Enum as _Enum
+
 from tomoscan.scanbase import TomoScanBase
-from numpy.core.numerictypes import generic as numy_generic
-import numpy
 
 
 class ReduceMethod(_Enum):
+    """
+    possible method to compute reduced darks / flats
+    """
+
     MEAN = "mean"  # compute the mean of dark / flat frames serie
     MEDIAN = "median"  # compute the median of dark / flat frames serie
     FIRST = "first"  # take the first frame of the dark / flat serie
     LAST = "last"  # take the last frame of the dark / flat serie
     NONE = "none"
 
 
 class REDUCER_TARGET(_Enum):
+    """
+    type of frame to reduce
+    """
+
     DARKS = "darks"
     FLATS = "flats"
 
 
 class FrameReducerBase:
+    """
+    Base class for frame reduced. We expect one per file format
+    """
+
     def __init__(
         self,
         scan: TomoScanBase,
         reduced_method: ReduceMethod,
         target: REDUCER_TARGET,
         output_dtype: Optional[numpy.dtype] = None,
         overwrite=False,
```

### Comparing `tomoscan-1.2.1/tomoscan/identifier.py` & `tomoscan-1.3.0a0/tomoscan/identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/io.py` & `tomoscan-1.3.0a0/tomoscan/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 #
 # ###########################################################################*/
 
 __authors__ = ["W. de Nolf"]
 __license__ = "MIT"
 __date__ = "25/08/2020"
 
-from contextlib import contextmanager
+import errno
 import logging
 import os
 import traceback
-import errno
+from contextlib import contextmanager
+
 import h5py
+
 from tomoscan.utils import SharedLockPool
 
 HASSWMR = h5py.version.hdf5_version_tuple >= h5py.get_config().swmr_min_hdf5_version
 _logger = logging.getLogger(__name__)
 
 
 class HDF5File(h5py.File):
@@ -53,15 +55,15 @@
         :param str mode:
         :param bool enable_file_locking: by default it is disabled for `mode=='r'`
                                          and enabled in all other modes
         :param bool swmr: when not specified: try both modes when `mode=='r'`
         :param **kwargs: see `h5py.File.__init__`
         """
         if mode not in ("r", "w", "w-", "x", "a"):
-            raise ValueError("invalid mode {}".format(mode))
+            raise ValueError(f"invalid mode {mode}")
 
         with self._protect_init(filename):
             # https://support.hdfgroup.org/HDF5/docNewFeatures/SWMR/Design-HDF5-FileLocking.pdf
             if not HASSWMR and swmr:
                 swmr = False
             libver = kwargs.get("libver")
             if swmr:
@@ -123,37 +125,37 @@
 
 def isErrno(e, errno):
     """
     :param OSError e:
     :returns bool:
     """
     # Because e.__cause__ is None for chained exceptions
-    return "errno = {}".format(errno) in "".join(traceback.format_exc())
+    return f"errno = {errno}" in "".join(traceback.format_exc())
 
 
 def check_virtual_sources_exist(fname, data_path):
     """
     Check that a virtual dataset points to actual data.
 
     :param str fname: HDF5 file path
     :param str data_path: Path within the HDF5 file
 
     :return bool res: Whether the virtual dataset points to actual data.
     """
     with HDF5File(fname, "r") as f:
         if data_path not in f:
-            _logger.error("No dataset %s in file %s" % (data_path, fname))
+            _logger.error(f"No dataset {data_path} in file {fname}")
             return False
         dptr = f[data_path]
         if not dptr.is_virtual:
             return True
         for vsource in dptr.virtual_sources():
             vsource_fname = os.path.join(
                 os.path.dirname(dptr.file.filename), vsource.file_name
             )
             if not os.path.isfile(vsource_fname):
-                _logger.error("No such file: %s" % vsource_fname)
+                _logger.error(f"No such file: {vsource_fname}")
                 return False
             elif not check_virtual_sources_exist(vsource_fname, vsource.dset_name):
-                _logger.error("Error with virtual source %s" % vsource_fname)
+                _logger.error(f"Error with virtual source {vsource_fname}")
                 return False
     return True
```

### Comparing `tomoscan-1.2.1/tomoscan/nexus/paths/nxdetector.py` & `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/nexus/paths/nxsample.py` & `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/nexus/paths/nxtomo.py` & `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxtomo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+import logging
 from typing import Optional
-from . import nxdetector
-from . import nxinstrument
-from . import nxsample
-from . import nxsource
-from . import nxmonitor
+
 from silx.utils.deprecation import deprecated
-import logging
+
 import tomoscan
 
+from . import nxdetector, nxinstrument, nxmonitor, nxsample, nxsource
+
 _logger = logging.getLogger(__name__)
 
 
 LATEST_VERSION = 1.2
 
 
 class NXtomo_PATH:
```

### Comparing `tomoscan-1.2.1/tomoscan/normalization.py` & `tomoscan-1.3.0a0/tomoscan/normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 __authors__ = [
     "H. Payno",
 ]
 __license__ = "MIT"
 __date__ = "25/06/2021"
 
 
-from silx.utils.enum import Enum as _Enum
+import logging
 import typing
+
 import numpy
-import logging
+from silx.utils.enum import Enum as _Enum
 
 _logger = logging.getLogger(__name__)
 
 
 class Method(_Enum):
     NONE = "none"
     SUBTRACTION = "subtraction"
@@ -152,15 +153,15 @@
     @staticmethod
     def from_dict(dict_):
         res = IntensityNormalization()
         res.load_from_dict(dict_)
         return res
 
     def __str__(self):
-        return "method: {}, extra-infos: {}".format(self.method, self.get_extra_infos())
+        return f"method: {self.method}, extra-infos: {self.get_extra_infos()}"
 
 
 def normalize_chebyshev_2D(sino):
     Nr, Nc = sino.shape
     J = numpy.arange(Nc)
     x = 2.0 * (J + 0.5 - Nc / 2) / Nc
     sum0 = Nc
@@ -175,15 +176,15 @@
     return sino
 
 
 def normalize_lsqr_spline_2D(sino):
     try:
         from scipy.interpolate import splev, splrep
     except ImportError:
-        _logger.error("You should install scipy to do the lsqr spline " "normalization")
+        _logger.error("You should install scipy to do the lsqr spline normalization")
         return None
 
     Nr, Nc = sino.shape
     # correction = numpy.zeros_like(sino)
     for i in range(Nr):
         line = sino[i, :]
         spline = splrep(range(len(line)), sino[i, :], k=1)
```

### Comparing `tomoscan-1.2.1/tomoscan/progress.py` & `tomoscan-1.3.0a0/tomoscan/progress.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 """module for giving information on process progress"""
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "07/08/2019"
 
 
+import logging
 import sys
 from enum import Enum
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class _Advancement(Enum):
     step_1 = "\\"
     step_2 = "-"
@@ -78,17 +78,15 @@
 
     def startProcess(self):
         self.setAdvancement(0)
 
     def setAdvancement(self, value):
         length = 20  # modify this to change the length
         block = int(round(length * value / 100))
-        msg = "\r{0}: [{1}] {2}%".format(
-            self._name, "#" * block + "-" * (length - block), round(value, 2)
-        )
+        msg = f"\r{self._name}: [{'#' * block + '-' * (length - block)}] {round(value, 2)}%"
         if value >= 100:
             msg += " DONE\r\n"
         sys.stdout.write(msg)
         sys.stdout.flush()
 
     def endProcess(self):
         self.setAdvancement(100)
```

### Comparing `tomoscan-1.2.1/tomoscan/scanbase.py` & `tomoscan-1.3.0a0/tomoscan/scanbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,43 +24,43 @@
 """This modules contains base class for TomoScanBase"""
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "09/10/2019"
 
 
-import fabio
+import logging
 import os
+import pathlib
 import typing
-import logging
+from bisect import bisect_left
+from collections import OrderedDict
+from math import ceil
+from typing import Iterable, Optional, Union
+
+import fabio
 import h5py
 import numpy
-from typing import Union, Iterable, Optional
-from collections import OrderedDict
-import pathlib
+import silx.io.utils
+from silx.io.url import DataUrl
+from silx.io.utils import get_data
+from silx.utils.deprecation import deprecated
+from silx.utils.enum import Enum as _Enum
+
 from tomoscan.identifier import ScanIdentifier
 from tomoscan.io import HDF5File
+from tomoscan.normalization import IntensityNormalization
+from tomoscan.normalization import Method as _IntensityMethod
+from tomoscan.normalization import normalize_chebyshev_2D, normalize_lsqr_spline_2D
 from tomoscan.unitsystem.electriccurrentsystem import ElectricCurrentSystem
 from tomoscan.unitsystem.timesystem import TimeSystem
-from .unitsystem.metricsystem import MetricSystem
-from silx.utils.enum import Enum as _Enum
-from silx.io.url import DataUrl
-from silx.io.utils import get_data
-import silx.io.utils
-from math import ceil
+
 from .progress import Progress
-from bisect import bisect_left
-from tomoscan.normalization import (
-    IntensityNormalization,
-    Method as _IntensityMethod,
-    normalize_chebyshev_2D,
-    normalize_lsqr_spline_2D,
-)
-from silx.utils.deprecation import deprecated
 from .tomoobject import TomoObject
+from .unitsystem.metricsystem import MetricSystem
 
 _logger = logging.getLogger(__name__)
 
 
 class FOV(_Enum):
     """Possible existing field of view"""
 
@@ -822,26 +822,23 @@
         :rtype: numpy.array
         """
         if (
             self.projections is not None
             and self.dim_2 is not None
             and line > self.dim_2
         ) or line < 0:
-            raise ValueError("requested line {} is not in the scan".format(line))
+            raise ValueError(f"requested line {line} is not in the scan")
         if self.projections is not None:
             y_dim = ceil(len(self.projections) / subsampling)
             sinogram = numpy.empty((y_dim, self.dim_1))
             _logger.debug(
-                "compute sinogram for line {} of {} (subsampling: {})".format(
-                    line, self.path, subsampling
-                )
+                f"compute sinogram for line {line} of {self.path} (subsampling: {subsampling})"
             )
             advancement = Progress(
-                name="compute sinogram for {}, line={},"
-                "sampling={}".format(os.path.basename(self.path), line, subsampling)
+                name=f"compute sinogram for {os.path.basename(self.path)}, line={line},sampling={subsampling}"
             )
             advancement.setMaxAdvancement(len(self.projections))
             projections = self.projections
             o_keys = list(projections.keys())
             o_keys.sort()
             for i_proj, proj_index in enumerate(o_keys):
                 if i_proj % subsampling == 0:
```

### Comparing `tomoscan-1.2.1/tomoscan/serie.py` & `tomoscan-1.3.0a0/tomoscan/serie.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 """Module with utils in order to define series of scan (TomoScanBase)"""
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "10/01/2021"
 
 
+import logging
 from typing import Iterable, Optional
+
 from tomoscan.scanbase import TomoScanBase
 from tomoscan.tomoobject import TomoObject
+
 from .factory import Factory
 from .identifier import BaseIdentifier
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 class Serie(list):
     """
     A serie can be view as an extented list of :class:`TomoObject`.
@@ -61,16 +63,15 @@
     def name(self) -> str:
         return self._name
 
     @name.setter
     def name(self, name: str):
         if not isinstance(name, str):
             raise TypeError("name is expected to be an instance of str")
-        else:
-            self._name = name
+        self._name = name
 
     @property
     def use_identifiers(self):
         return self.__use_identifiers
 
     def append(self, object: TomoObject):
         if not isinstance(object, TomoObject):
@@ -208,15 +209,15 @@
     :rtype: bool
     """
     if len(scans) == 0:
         return True
     try:
         check_serie_is_consistant_frm_sample_name(scans=scans)
     except Exception as e:
-        _logger.error("provided group is invalid. {}".format(e))
+        _logger.error(f"provided group is invalid. {e}")
         raise e
     else:
         group_size = next(iter(scans)).group_size
         if group_size is None:
             _logger.warning("No information found regarding group size")
             return True
         elif group_size == len(scans):
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_framereducerbase.py` & `tomoscan-1.3.0a0/tomoscan/test/test_framereducerbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "06/01/2022"
 
 
-from tomoscan.framereducerbase import FrameReducerBase
-from tomoscan.esrf.mock import MockHDF5
 import pytest
 
+from tomoscan.esrf.mock import MockHDF5
+from tomoscan.framereducerbase import FrameReducerBase
+
 
 def test_FrameReducerBase_instanciation(tmp_path):
     scan = MockHDF5(tmp_path, n_proj=2).scan
     reducer = FrameReducerBase(scan=scan, reduced_method="mean", target="darks")
     with pytest.raises(NotImplementedError):
         reducer.run()
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_io.py` & `tomoscan-1.3.0a0/tomoscan/test/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "18/09/2020"
 
 
 import os
-import h5py
-import numpy
 import shutil
-import unittest
 import tempfile
+import unittest
+
+import h5py
+import numpy
+
 from tomoscan.io import check_virtual_sources_exist
 
 
 class TestCheckVirtualSourcesExists(unittest.TestCase):
     """insure the check_virtual_sources_exist function exists"""
 
     def setUp(self) -> None:
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_normalization.py` & `tomoscan-1.3.0a0/tomoscan/test/test_normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,28 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "31/08/2021"
 
 
-from tomoscan.test.utils import HDF5MockContext
-from tomoscan.nexus.paths.nxtomo import nx_tomo_path_latest
-import tomoscan.esrf.hdf5scan
-import tomoscan.normalization
 import os
 import tempfile
-import numpy
-import pytest
 from typing import Union
+
 import h5py
+import numpy
+import pytest
 from silx.io.url import DataUrl
 
+import tomoscan.esrf.hdf5scan
+import tomoscan.normalization
+from tomoscan.nexus.paths.nxtomo import nx_tomo_path_latest
+from tomoscan.test.utils import HDF5MockContext
+
 try:
     import scipy.interpolate  # noqa F401
 except ImportError:
     has_scipy = False
 else:
     has_scipy = True
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_progress.py` & `tomoscan-1.3.0a0/tomoscan/test/test_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """Simple test of the Progress API"""
     progress = tomoscan.progress.Progress("this is progress")
     progress.reset()
     progress.startProcess()
     progress.setMaxAdvancement(80)
     for adv in (10, 20, 50, 70):
         progress.setAdvancement(adv)
-    for i in range(10):
+    for _ in range(10):
         progress.increaseAdvancement(1)
 
 
 def test_advancement():
     """Simple test of the _Advancement API"""
     for i in range(4):
         tomoscan.progress._Advancement.getNextStep(
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_scanbase.py` & `tomoscan-1.3.0a0/tomoscan/test/test_scanbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,27 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "01/09/2021"
 
 
-from copy import deepcopy
-import unittest
-import numpy.random
-from tomoscan.scanbase import ReducedFramesInfos, TomoScanBase
-from tomoscan.scanbase import Source, SourceType
-from tomoscan.test.utils import HDF5MockContext
+import os
 import shutil
 import tempfile
-from silx.io.url import DataUrl
+import unittest
+from copy import deepcopy
+
 import h5py
-import os
+import numpy.random
 import pytest
+from silx.io.url import DataUrl
+
+from tomoscan.scanbase import ReducedFramesInfos, Source, SourceType, TomoScanBase
+from tomoscan.test.utils import HDF5MockContext
 
 
 class TestFlatFieldCorrection(unittest.TestCase):
     def setUp(self):
         self.data_dir = tempfile.mkdtemp()
         self.scan = TomoScanBase(None, None)
         self.scan.set_reduced_darks(
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_scanfactory.py` & `tomoscan-1.3.0a0/tomoscan/test/test_scanfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "24/01/2017"
 
 
 import os
+import tempfile
+
+import pytest
+
 from tomoscan.esrf.edfscan import EDFTomoScan
 from tomoscan.esrf.hdf5scan import HDF5TomoScan
-from tomoscan.scanbase import TomoScanBase
+from tomoscan.esrf.mock import MockEDF
 from tomoscan.factory import Factory
+from tomoscan.scanbase import TomoScanBase
 from tomoscan.test.utils import UtilsTest
-from tomoscan.esrf.mock import MockEDF
-import tempfile
-import pytest
 
 
 def test_scan_edf():
     """can we create a TomoScanBase object from a folder containing a
     valid .edf acquisition"""
     scan_dir = UtilsTest.getDataset("test10")
     scan = Factory.create_scan_object(scan_dir)
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_serie.py` & `tomoscan-1.3.0a0/tomoscan/test/test_serie.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,38 +24,40 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "10/01/2021"
 
 
+import os
+import tempfile
+
 import pytest
+
+from tomoscan.esrf.mock import MockHDF5
+from tomoscan.esrf.volume.edfvolume import EDFVolume
 from tomoscan.serie import (
     Serie,
-    sequences_to_series_from_sample_name,
     check_serie_is_consistant_frm_sample_name,
+    sequences_to_series_from_sample_name,
     serie_is_complete_from_group_size,
 )
-from tomoscan.esrf.mock import MockHDF5
-from tomoscan.esrf.volume.edfvolume import EDFVolume
-import tempfile
-import os
 
 
 @pytest.mark.parametrize("use_identifiers", [True, False])
 def test_serie_scan(use_identifiers):
     """simple test of a serie"""
-    with tempfile.TemporaryDirectory() as dir:
+    with tempfile.TemporaryDirectory() as dir_:
         serie1 = Serie(use_identifiers=use_identifiers)
         assert isinstance(serie1.name, str)
         serie2 = Serie("test", use_identifiers=use_identifiers)
         assert serie2.name == "test"
         assert len(serie2) == 0
-        scan1 = MockHDF5(dir, n_proj=2).scan
-        scan2 = MockHDF5(dir, n_proj=2).scan
+        scan1 = MockHDF5(dir_, n_proj=2).scan
+        scan2 = MockHDF5(dir_, n_proj=2).scan
         serie3 = Serie("test", [scan1, scan2], use_identifiers=use_identifiers)
         assert serie3.name == "test"
         assert len(serie3) == 2
 
         with pytest.raises(TypeError):
             serie1.append("toto")
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_tomoobject.py` & `tomoscan-1.3.0a0/tomoscan/test/test_tomoobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # THE SOFTWARE.
 #
 # ###########################################################################*/
 """test of the tomoscan.tomoobject module"""
 
 
 import pytest
+
 from tomoscan.tomoobject import TomoObject
 
 
 def test_tomoobject():
     obj = TomoObject()
     with pytest.raises(NotImplementedError):
         obj.from_identifier("test")
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_utils.py` & `tomoscan-1.3.0a0/tomoscan/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "03/05/2022"
 
 
 import pytest
+
 from tomoscan.utils.geometry import BoundingBox1D, BoundingBox3D, _BoundingBox
 
 
 def test_bounding_box_base():
     bb = _BoundingBox(0, 1)
     with pytest.raises(NotImplementedError):
         bb.get_overlap(None)
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_validator.py` & `tomoscan-1.3.0a0/tomoscan/test/test_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,23 +25,24 @@
 """Module containing validators"""
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "25/08/2021"
 
 
-import tomoscan.validator
-from tomoscan.test.utils import HDF5MockContext
 import os
-import pytest
+import sys
 import tempfile
-import numpy
+
 import h5py
-import sys
+import numpy
+import pytest
 
+import tomoscan.validator
+from tomoscan.test.utils import HDF5MockContext
 
 frame_validators = (
     tomoscan.validator.FlatEntryValidator,
     tomoscan.validator.DarkEntryValidator,
     tomoscan.validator.ProjectionEntryValidator,
 )
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_version.py` & `tomoscan-1.3.0a0/tomoscan/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/test/test_volume_base.py` & `tomoscan-1.3.0a0/tomoscan/test/test_volume_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 """Module containing validators"""
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "07/07/2022"
 
 
-from tomoscan.volumebase import VolumeBase
 import pytest
 
+from tomoscan.volumebase import VolumeBase
+
 
 def test_volume_base():
     """Test VolumeBase file"""
 
     class UnplemetnedVolumeBase(VolumeBase):
         def deduce_data_and_metadata_urls(self, url):
             return None, None
```

### Comparing `tomoscan-1.2.1/tomoscan/test/test_volume_utils.py` & `tomoscan-1.3.0a0/tomoscan/test/test_volume_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
+from copy import deepcopy
+
 import numpy
 import pytest
-from copy import deepcopy
-from tomoscan.utils.volume import concatenate, update_metadata
+
 from tomoscan.esrf.volume.edfvolume import EDFVolume
 from tomoscan.esrf.volume.hdf5volume import HDF5Volume
 from tomoscan.esrf.volume.jp2kvolume import JP2KVolume, has_minimal_openjpeg
 from tomoscan.esrf.volume.tiffvolume import TIFFVolume, has_tifffile
+from tomoscan.utils.volume import concatenate, update_metadata
 
 _clases_to_test = [EDFVolume, HDF5Volume]
 if has_minimal_openjpeg:
     _clases_to_test.append(JP2KVolume)
 if has_tifffile:
     _clases_to_test.append(TIFFVolume)
```

### Comparing `tomoscan-1.2.1/tomoscan/test/utils.py` & `tomoscan-1.3.0a0/tomoscan/test/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 
 __doc__ = """test modules for pyFAI."""
 __authors__ = ["Jérôme Kieffer", "Valentin Valls", "Henri Payno"]
 __license__ = "MIT"
 __copyright__ = "European Synchrotron Radiation Facility, Grenoble, France"
 __date__ = "07/02/2017"
 
+import logging
 import os
 import shutil
-from urllib.request import urlopen, ProxyHandler, build_opener
-from tomoscan.esrf.mock import MockHDF5
-import logging
 import tempfile
+from urllib.request import ProxyHandler, build_opener, urlopen
+
+from tomoscan.esrf.mock import MockHDF5
 
 try:
     from contextlib import AbstractContextManager
 except ImportError:
     from tomwer.third_party.contextlib import AbstractContextManager
 
 logging.basicConfig(level=logging.WARNING)
@@ -77,23 +78,23 @@
     def getH5Dataset(cls, folderID):
         path = os.path.abspath(
             os.path.join(cls.getDatasets(name="h5_datasets"), folderID)
         )
         if os.path.exists(path):
             return path
         else:
-            raise RuntimeError("Coul'd find folder containing scan %s" % folderID)
+            raise RuntimeError(f"Coul'd find folder containing scan {folderID}")
 
     @classmethod
     def getOrangeTestFile(cls, folderID):
         path = os.path.abspath(os.path.join(cls.getOrangeTestFiles(), folderID))
         if os.path.isfile(path):
             return path
         else:
-            raise RuntimeError("Coul'd find folder containing scan %s" % folderID)
+            raise RuntimeError(f"Coul'd find folder containing scan {folderID}")
 
     @classmethod
     def getOrangeTestFiles(cls):
         return cls.getDatasets(name="orangetestfiles")
 
     @classmethod
     def getDataset(cls, name):
@@ -129,15 +130,15 @@
                     "please set both environment variable http_proxy and https_proxy. "
                     "This even works under windows ! \n "
                     f"Otherwise please try to download the images manually from {url_base} / {archive_file}"
                 )
 
         # decompress if needed
         if os.path.isfile(archive_file):
-            logger.info("decompressing %s." % archive_file)
+            logger.info(f"decompressing {archive_file}.")
             outdir = "".join((os.path.dirname(__file__)))
             shutil.unpack_archive(archive_file, extract_dir=outdir, format="bztar")
             os.remove(archive_file)
         else:
             logger.info("not trying to decompress it")
         return archive_folder
 
@@ -147,16 +148,16 @@
         The id of the internal test is to have some large scan accessible
         which are stored locally. This should be used only for unit test that
         can be skipped
         """
         if "TOMWER_ADDITIONAL_TESTS_DIR" not in os.environ:
             return False
         else:
-            dir = os.path.join(os.environ["TOMWER_ADDITIONAL_TESTS_DIR"], dataset)
-        return os.path.isdir(dir)
+            dir_ = os.path.join(os.environ["TOMWER_ADDITIONAL_TESTS_DIR"], dataset)
+        return os.path.isdir(dir_)
 
     @classmethod
     def getInternalTestDir(cls, dataset):
         if cls.hasInternalTest(dataset) is False:
             return None
         else:
             return os.path.join(os.environ["TOMWER_ADDITIONAL_TESTS_DIR"], dataset)
@@ -165,43 +166,39 @@
 url_base = "http://www.edna-site.org/pub/tomoscan/"
 
 
 def DownloadDataset(dataset, output_folder, timeout, unpack=False):
     # create if needed path scan
     url = url_base + dataset
 
-    logger.info("Trying to download scan %s, timeout set to %ss", dataset, timeout)
+    logger.info(f"Trying to download scan {dataset}, timeout set to {timeout}s")
     dictProxies = {}
     if "http_proxy" in os.environ:
         dictProxies["http"] = os.environ["http_proxy"]
         dictProxies["https"] = os.environ["http_proxy"]
     if "https_proxy" in os.environ:
         dictProxies["https"] = os.environ["https_proxy"]
     if dictProxies:
         proxy_handler = ProxyHandler(dictProxies)
         opener = build_opener(proxy_handler).open
     else:
         opener = urlopen
-    logger.info("wget %s" % url)
+    logger.info(f"wget {url}")
     data = opener(url, data=None, timeout=timeout).read()
-    logger.info("Image %s successfully downloaded." % dataset)
+    logger.info(f"Image {dataset} successfully downloaded.")
 
     if not os.path.isdir(output_folder):
         os.mkdir(output_folder)
 
     try:
         archive_folder = os.path.join(output_folder, os.path.basename(dataset))
         with open(archive_folder, "wb") as outfile:
             outfile.write(data)
     except IOError:
-        raise IOError(
-            "unable to write downloaded \
-                        data to disk at %s"
-            % archive_folder
-        )
+        raise IOError(f"unable to write downloaded data to disk at {archive_folder}")
 
     if unpack is True:
         shutil.unpack_archive(archive_folder, extract_dir=output_folder, format="bztar")
         os.remove(archive_folder)
 
 
 class MockContext(AbstractContextManager):
```

### Comparing `tomoscan-1.2.1/tomoscan/tomoobject.py` & `tomoscan-1.3.0a0/tomoscan/tomoobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 """Module containing the TomoObject class. Parent class of any tomo object"""
 
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
-from typing import Union, Optional
-from .identifier import BaseIdentifier
+from typing import Optional, Union
+
 from tomoscan.utils import BoundingBox1D
 
+from .identifier import BaseIdentifier
+
 
 class TomoObject:
     """Parent class of all tomographic object in tomoscan"""
 
     @staticmethod
     def from_identifier(identifier: Union[str, BaseIdentifier]):
         """Return the Dataset from a identifier"""
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/__init__.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 # ###########################################################################*/
 """module for the unit system"""
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "09/02/2021"
 
-from .unit import Unit  # noqa F401
+from .electriccurrentsystem import ElectricCurrentSystem  # noqa F401
 from .energysystem import EnergySI  # noqa F401
 from .metricsystem import MetricSystem  # noqa F401
 from .timesystem import TimeSystem  # noqa F401
-from .electriccurrentsystem import ElectricCurrentSystem  # noqa F401
+from .unit import Unit  # noqa F401
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/electriccurrentsystem.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/electriccurrentsystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if value.lower() in ("a", "ampere"):
             return ElectricCurrentSystem.AMPERE
         elif value.lower() in ("ma", "milliampere"):
             return ElectricCurrentSystem.MILLIAMPERE
         elif value.lower() in ("ka", "kiloampere"):
             return ElectricCurrentSystem.KILOAMPERE
         else:
-            raise ValueError("Cannot convert: %s" % value)
+            raise ValueError(f"Cannot convert: {value}")
 
     def __str__(self):
         if self == ElectricCurrentSystem.AMPERE:
             return "A"
         elif self == ElectricCurrentSystem.MILLIAMPERE:
             return "mA"
         elif self == ElectricCurrentSystem.KILOAMPERE:
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/energysystem.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/energysystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 __authors__ = ["P. Paleo", "H. Payno"]
 __license__ = "MIT"
 __date__ = "09/02/2022"
 
 
 from tomoscan.unitsystem.unit import Unit
 
-
 # Constants
 _elementary_charge_coulomb = 1.602176634e-19
 
 
 _joule_si = 1.0
 
 
@@ -62,15 +61,15 @@
         elif value.lower() in ("mev", "megaelectronvolt"):
             return EnergySI.MEGAELECTRONVOLT
         elif value.lower() in ("gev", "gigaelectronvolt"):
             return EnergySI.GIGAELECTRONVOLT
         elif value.lower() in ("e", "qe"):
             return EnergySI.ELEMCHARGE
         else:
-            raise ValueError("Cannot convert: %s" % value)
+            raise ValueError(f"Cannot convert: {value}")
 
     def __str__(self):
         if self is EnergySI.JOULE:
             return "J"
         elif self is EnergySI.KILOJOULE:
             return "kJ"
         elif self is EnergySI.ELECTRONVOLT:
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/metricsystem.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/metricsystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # ###########################################################################*/
 __authors__ = ["P. Paleo", "H. Payno"]
 __license__ = "MIT"
 __date__ = "09/02/2022"
 
 
 from silx.utils.deprecation import deprecated_warning
+
 from tomoscan.unitsystem.energysystem import (
     EnergySI,
 )  # noqa F401  kept for bacward compatibility
 from tomoscan.unitsystem.unit import Unit
 
 # Default units:
 #  - lenght: meter (m)
@@ -108,15 +109,15 @@
                 "MetricSystem.from_str for energies",
                 reason="Must be part of EnergySI instead",
                 replacement="EnergySI.from_str",
                 since_version="0.8.0",
             )
             return MetricSystem.KILOJOULE
         else:
-            raise ValueError("Cannot convert: %s" % value)
+            raise ValueError(f"Cannot convert: {value}")
 
     def __str__(self):
         if self == MetricSystem.METER:
             return "m"
         elif self == MetricSystem.CENTIMETER:
             return "cm"
         elif self == MetricSystem.MILLIMETER:
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/timesystem.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/timesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         elif value.lower() in ("ns", "nanosecond", "nano-second"):
             return TimeSystem.NANO_SECOND
         elif value.lower() in ("microsecond", "micro-second"):
             return TimeSystem.MICRO_SECOND
         elif value.lower() in ("millisecond", "milli-second"):
             return TimeSystem.MILLI_SECOND
         else:
-            raise ValueError("Cannot convert: %s" % value)
+            raise ValueError(f"Cannot convert: {value}")
 
     def __str__(self):
         if self == TimeSystem.SECOND:
             return "second"
         elif self == TimeSystem.MINUTE:
             return "minute"
         elif self == TimeSystem.HOUR:
```

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/unit.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/unit.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/unitsystem/voltagesystem.py` & `tomoscan-1.3.0a0/tomoscan/unitsystem/voltagesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     @classmethod
     def from_str(cls, value: str):
         assert isinstance(value, str)
         if value.lower() in ("v", "volt"):
             return VoltageSystem.VOLT
         else:
-            raise ValueError("Cannot convert: %s" % value)
+            raise ValueError(f"Cannot convert: {value}")
 
     def __str__(self):
         if self == VoltageSystem.VOLT:
             return "volt"
         else:
             raise ValueError("Cannot convert: to voltage system")
```

### Comparing `tomoscan-1.2.1/tomoscan/utils/decorator.py` & `tomoscan-1.3.0a0/tomoscan/utils/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     It patches dest.__doc__.
     """
     if not isinstance(dest, type) and isinstance(origin, type):
         # func is not a class, but origin is, get the method with the same name
         try:
             origin = getattr(origin, dest.__name__)
         except AttributeError:
-            raise ValueError("origin class has no %s method" % dest.__name__)
+            raise ValueError(f"origin class has no {dest.__name__} method")
 
     dest.__doc__ = origin.__doc__
     return dest
 
 
 def docstring(origin):
     """Decorator to initialize the docstring from another source.
```

### Comparing `tomoscan-1.2.1/tomoscan/utils/geometry.py` & `tomoscan-1.3.0a0/tomoscan/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.2.1/tomoscan/utils/hdf5.py` & `tomoscan-1.3.0a0/tomoscan/utils/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "23/02/2022"
 
 
 import contextlib
+
 import h5py
+
 from tomoscan.io import HDF5File
 
 try:
     import hdf5plugin  # noqa F401
 except ImportError:
     pass
 from silx.io.url import DataUrl
@@ -61,12 +63,10 @@
     """Context manager used to read a bliss node"""
 
     def __enter__(self):
         self._file_handler = HDF5File(filename=self._url.file_path(), mode="r")
         entry = self._file_handler[self._url.data_path()]
         if not isinstance(entry, h5py.Dataset):
             raise ValueError(
-                "Data path ({}) should point to a dataset (h5py.Dataset)".format(
-                    self._url.path()
-                )
+                f"Data path ({self._url.path()}) should point to a dataset (h5py.Dataset)"
             )
         return entry
```

### Comparing `tomoscan-1.2.1/tomoscan/utils/io.py` & `tomoscan-1.3.0a0/tomoscan/utils/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from contextlib import contextmanager, ExitStack
 import threading
+from contextlib import ExitStack, contextmanager
 
 
 class SharedLockPool:
     """
     Allows to acquire locks identified by name (hashable type) recursively.
     """
```

### Comparing `tomoscan-1.2.1/tomoscan/utils/volume.py` & `tomoscan-1.3.0a0/tomoscan/utils/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import logging
 import os
+from collections.abc import Mapping
+
 import h5py
 import numpy
-import logging
-from tomoscan.volumebase import VolumeBase
+
 from tomoscan.esrf.volume import HDF5Volume
 from tomoscan.io import HDF5File
 from tomoscan.utils.hdf5 import DatasetReader
-from collections.abc import Mapping
+from tomoscan.volumebase import VolumeBase
 
 _logger = logging.getLogger(__name__)
 
 
 def concatenate(output_volume: VolumeBase, volumes: tuple, axis: int) -> None:
     """
     Function to do 'raw' concatenation on volumes.
@@ -143,16 +145,16 @@
     else:
         # 2.1 default case (duplicate all input data slice by slice)
         # 2.1.1 special case of the concatenation other axis 0
         if axis == 0:
 
             def iter_input():
                 for vol in volumes:
-                    for slice in vol.browse_slices():
-                        yield slice
+                    for data_slice in vol.browse_slices():
+                        yield data_slice
 
             for frame_dumper, input_slice in zip(
                 output_volume.data_file_saver_generator(
                     n_frames=final_shape[0],
                     data_url=output_volume.data_url,
                     overwrite=output_volume.overwrite,
                 ),
```

### Comparing `tomoscan-1.2.1/tomoscan/validator.py` & `tomoscan-1.3.0a0/tomoscan/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 # ###########################################################################*/
 """Module containing validators"""
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "24/08/2021"
 
+import logging
+import weakref
+from typing import Optional
+
 import numpy
+from silx.io.utils import get_data
 
+from tomoscan.esrf.scan.utils import dataset_has_broken_vds, get_compacted_dataslices
 from tomoscan.scanbase import TomoScanBase
-from tomoscan.esrf.scan.utils import dataset_has_broken_vds
-from tomoscan.esrf.scan.utils import get_compacted_dataslices
-from silx.io.utils import get_data
-import logging
-from typing import Optional
-import weakref
 
 _logger = logging.getLogger(__name__)
 
 
 _VALIDATOR_NAME_TXT_AJUST = 15
 
 _LOCATION_TXT_AJUST = 40
```

### Comparing `tomoscan-1.2.1/tomoscan/version.py` & `tomoscan-1.3.0a0/tomoscan/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     "beta": 11,
     "gamma": 12,
     "rc": 13,
     "final": 15,
 }
 
 MAJOR = 1
-MINOR = 2
-MICRO = 1
-RELEV = "final"  # <16
+MINOR = 3
+MICRO = 0
+RELEV = "alpha"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
```

### Comparing `tomoscan-1.2.1/tomoscan/volumebase.py` & `tomoscan-1.3.0a0/tomoscan/volumebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
-import numpy
-from tomoscan.identifier import VolumeIdentifier
-from tomoscan.tomoobject import TomoObject
-from tomoscan.scanbase import TomoScanBase
-from tomoscan.utils import BoundingBox1D, BoundingBox3D
-from tomoscan.unitsystem.metricsystem import MetricSystem
 from typing import Optional, Union
+
+import numpy
 from silx.io.url import DataUrl
 from silx.math.combo import (  # pylint: disable=E0611 (not found from the pyx file)
     min_max,
 )
 from silx.utils.deprecation import deprecated_warning
 
+from tomoscan.identifier import VolumeIdentifier
+from tomoscan.scanbase import TomoScanBase
+from tomoscan.tomoobject import TomoObject
+from tomoscan.unitsystem.metricsystem import MetricSystem
+from tomoscan.utils import BoundingBox1D, BoundingBox3D
+
 
 class VolumeBase(TomoObject):
     """
     context: we aim at having a common way of saving and loading volumes through the tomotools suite.
     The goal is to aim handling of volumes when creating them or doing some operations with those like stitching...
 
     :param DataUlr url: url of the volume. Could be path to a master file if we can provide one per each volume. Otherwise could be a pattern of edf files or tiff file with a data range
@@ -237,19 +239,23 @@
         if "reconstruction" not in ddict["processing_options"]:
             ddict["processing_options"]["reconstruction"] = {}
 
     @property
     def position(self) -> tuple:
         """position are provided as a tuple using the same reference for axis as the volume data"""
         metadata = self.metadata or self.load_metadata()
-        return tuple(
+        position = (
             metadata.get("processing_options", {})
             .get("reconstruction", {})
             .get("position", None)
         )
+        if position is None:
+            return None
+        else:
+            return tuple(position)
 
     @position.setter
     def position(self, position) -> None:
         if self.metadata is None:
             self.metadata = {}
         self._insure_reconstruction_dict_exists(self.metadata)
         self.metadata["processing_options"]["reconstruction"]["position"] = numpy.array(
@@ -262,16 +268,15 @@
         pixel_size = (
             metadata.get("processing_options", {})
             .get("reconstruction", {})
             .get("pixel_size_cm", None)
         )
         if pixel_size is not None:
             return pixel_size * MetricSystem.CENTIMETER.value
-        else:
-            return None
+        return None
 
     @pixel_size.setter
     def pixel_size(self, pixel_size) -> None:
         if self.metadata is None:
             self.metadata = {}
         self._insure_reconstruction_dict_exists(self.metadata)
         self.metadata["processing_options"]["reconstruction"]["pixel_size_cm"] = (
@@ -304,27 +309,26 @@
         if pixel_size is None:
             missing.append("pixel_size")
 
         if len(missing) > 0:
             raise ValueError(
                 f"Unable to get bounding box. Missing information: {'; '.join(missing)}"
             )
+        assert axis is not None
+        if axis == "x":
+            idx = 2
+        elif axis == "y":
+            idx = 1
+        elif axis == "z":
+            idx = 0
         else:
-            assert axis is not None
-            if axis == "x":
-                idx = 2
-            elif axis == "y":
-                idx = 1
-            elif axis == "z":
-                idx = 0
-            else:
-                raise ValueError(f"axis '{axis}' is not handled")
-            min_pos_in_meter = position[idx] - pixel_size * shape[idx] / 2.0
-            max_pos_in_meter = position[idx] + pixel_size * shape[idx] / 2.0
-            return BoundingBox1D(min_pos_in_meter, max_pos_in_meter)
+            raise ValueError(f"axis '{axis}' is not handled")
+        min_pos_in_meter = position[idx] - pixel_size * shape[idx] / 2.0
+        max_pos_in_meter = position[idx] + pixel_size * shape[idx] / 2.0
+        return BoundingBox1D(min_pos_in_meter, max_pos_in_meter)
 
     def get_min_max(self) -> tuple:
         """
         compute min max of the volume. Can take some time but avoid to load the full volume in memory
         """
         if self.data is not None:
             return self.data.min(), self.data.max()
@@ -483,20 +487,20 @@
         """
         min_v = None
         max_v = None
         if self.data is not None:
             data = self.data
         else:
             data = self.browse_slices(url=url)
-        for slice in data:
+        for data_slice in data:
             if min_v is None:
-                min_v = slice.min()
-                max_v = slice.max()
+                min_v = data_slice.min()
+                max_v = data_slice.max()
             else:
-                min_lv, max_lv = min_max(slice, finite=True)
+                min_lv, max_lv = min_max(data_slice, finite=True)
                 min_v = min(min_v, min_lv)
                 max_v = max(max_v, max_lv)
         return min_v, max_v
 
     def data_file_saver_generator(self, n_frames, data_url: DataUrl, overwrite: bool):
         """
         Provide a helper class to dump data frame by frame. For know the only possible interaction is
```

### Comparing `tomoscan-1.2.1/tomoscan.egg-info/PKG-INFO` & `tomoscan-1.3.0a0/tomoscan.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.2.1
+Version: 1.3.0a0
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.2.1/tomoscan.egg-info/SOURCES.txt` & `tomoscan-1.3.0a0/tomoscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

