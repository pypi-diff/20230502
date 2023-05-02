# Comparing `tmp/eodatasets3-0.9.2.tar.gz` & `tmp/eodatasets3-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eodatasets3-0.9.2.tar", last modified: Thu Jun 11 06:09:51 2020, max compression
+gzip compressed data, was "dist/eodatasets3-0.9.3.tar", last modified: Fri Jul  3 07:13:01 2020, max compression
```

## Comparing `eodatasets3-0.9.2.tar` & `eodatasets3-0.9.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/
--rw-rw-r--   0 jez       (1000) jez       (1000)    11358 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/LICENSE
--rw-rw-r--   0 jez       (1000) jez       (1000)     5325 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/pylintrc
--rwxrwxr-x   0 jez       (1000) jez       (1000)     2377 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/setup.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      485 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.coveragerc
--rwxrwxr-x   0 jez       (1000) jez       (1000)      244 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/check-code.sh
--rw-rw-r--   0 jez       (1000) jez       (1000)      815 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/setup.cfg
--rw-rw-r--   0 jez       (1000) jez       (1000)      195 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.gitattributes
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/
--rw-rw-r--   0 jez       (1000) jez       (1000)     8097 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/SOURCES.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)      304 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/entry_points.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/dependency_links.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)       12 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/top_level.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     8988 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/PKG-INFO
--rw-rw-r--   0 jez       (1000) jez       (1000)      561 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3.egg-info/requires.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)      365 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.pre-commit-config.yaml
--rw-rw-r--   0 jez       (1000) jez       (1000)      278 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/pyproject.toml
--rw-rw-r--   0 jez       (1000) jez       (1000)      252 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.gitignore
--rw-rw-r--   0 jez       (1000) jez       (1000)      376 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/conftest.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/docs/
--rw-rw-r--   0 jez       (1000) jez       (1000)     4809 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/index.rst
--rw-rw-r--   0 jez       (1000) jez       (1000)      760 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/make.bat
--rw-rw-r--   0 jez       (1000) jez       (1000)      634 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/Makefile
--rw-rw-r--   0 jez       (1000) jez       (1000)        8 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/.gitignore
--rw-rw-r--   0 jez       (1000) jez       (1000)     1522 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/conf.py
--rw-rw-r--   0 jez       (1000) jez       (1000)       27 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/docs/requirements.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     6823 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/README.md
--rw-rw-r--   0 jez       (1000) jez       (1000)     8988 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/PKG-INFO
--rw-rw-r--   0 jez       (1000) jez       (1000)     3026 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.travis.yml
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/utils/
--rwxrwxr-x   0 jez       (1000) jez       (1000)     2112 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/utils/subset_noaa_c_c_prwtreatm_1
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/
--rw-rw-r--   0 jez       (1000) jez       (1000)      572 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_serialise.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     4114 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/h5downsample.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     2021 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/common.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/
--rw-rw-r--   0 jez       (1000) jez       (1000)   430181 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LT05_L1TP_090085_19970406_20161231_01_T1.tar.gz
--rw-rw-r--   0 jez       (1000) jez       (1000)  1989815 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/S2B_OPER_MSI_L1C_TL_EPAE_20180617T013729_A006677_T55JGF_N02.06.AWSPDS.zip
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B11.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B3.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     8633 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_MTL.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B10.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B8.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)   117392 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_ANG.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B6.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B1.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B4.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B5.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_BQA.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B7.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B9.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B2.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)  1837225 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/S2A_MSIL1C_20180629T000241_N0206_R030_T56JMM_20180629T012042.zip
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/
--rw-rw-r--   0 jez       (1000) jez       (1000)     2739 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_IDF.xml
--rw-rw-r--   0 jez       (1000) jez       (1000)      256 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_MD5.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/406.000.2018001004744204.ASN
--rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/407.001.2018001004824874.ASN
--rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/407.000.2018001004819738.ASN
--rw-rw-r--   0 jez       (1000) jez       (1000)      456 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/package.sha1
--rw-rw-r--   0 jez       (1000) jez       (1000)      948 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/ga-metadata.yaml
--rw-rw-r--   0 jez       (1000) jez       (1000)    34477 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LE07_L1GT_104078_20131209_20161119_01_T2.tar.gz
--rw-rw-r--   0 jez       (1000) jez       (1000)     2430 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_089080_20160302_20170328_01_T1.yaml
--rw-rw-r--   0 jez       (1000) jez       (1000)   143360 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LE07_L1TP_104078_20130429_20161124_01_T1.tar
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/noaa_c_c_prwtreatm_1/
--rw-rw-r--   0 jez       (1000) jez       (1000)   113307 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/noaa_c_c_prwtreatm_1/pr_wtr.eatm.2018.test.nc
--rw-rw-r--   0 jez       (1000) jez       (1000)    87879 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1.tar.gz
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/
--rwxrwxr-x   0 jez       (1000) jez       (1000)     2485 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC08_L1TP_092084_20160628_20170323_01_T1.yaml
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/
--rw-rw-r--   0 jez       (1000) jez       (1000)    43878 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img
--rwxrwxr-x   0 jez       (1000) jez       (1000)      547 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.yaml
--rw-rw-r--   0 jez       (1000) jez       (1000)  5742248 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.wagl.h5
--rw-rw-r--   0 jez       (1000) jez       (1000)     1612 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-0242778241.aux.xml
--rwxrwxr-x   0 jez       (1000) jez       (1000)     1612 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-8404334440.aux.xml
--rw-rw-r--   0 jez       (1000) jez       (1000)      186 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.tmp..img.aux.xml
--rwxrwxr-x   0 jez       (1000) jez       (1000)      122 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.tesp.yaml
--rwxrwxr-x   0 jez       (1000) jez       (1000)      896 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.gqa.yaml
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B4.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B3.TIF
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/extras/
--rw-rw-r--   0 jez       (1000) jez       (1000)       62 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/extras/example-file.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B2.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     6693 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_MTL.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     8686 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/README.GTF
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B5.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_BQA.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)    34884 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_ANG.txt
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B1.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B6.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B7.TIF
--rw-rw-r--   0 jez       (1000) jez       (1000)    15433 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_assemble.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     2628 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/__init__.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/
--rw-rw-r--   0 jez       (1000) jez       (1000)    99552 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/LC08_L1TP_091075_20161213_20170316_01_T2.tar.gz
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/
--rw-rw-r--   0 jez       (1000) jez       (1000)   155648 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/LE07_L1GT_091080_20080114_20161231_01_T2.tar.gz
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/
--rw-rw-r--   0 jez       (1000) jez       (1000)    28918 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2.tar.gz
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/tests/integration/prepare/
--rw-rw-r--   0 jez       (1000) jez       (1000)    12205 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/prepare/test_prepare_s2a_l1c_safe.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     3920 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/prepare/test_prepare_landsat_l1.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     4354 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/prepare/test_noaa_c_c_prwtreatm_1.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     9636 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/prepare/test_prepare_s2b_l1c_awspds.py
--rw-rw-r--   0 jez       (1000) jez       (1000)        0 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/prepare/__init__.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    18512 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/conftest.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    16920 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_recompress.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     7071 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_image.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    15329 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_validate.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    25570 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/integration/test_packagewagl.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     3042 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/test_verify.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     6412 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/__init__.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     3405 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/tests/test_documents.py
--rw-rw-r--   0 jez       (1000) jez       (1000)       99 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/MANIFEST.in
--rw-rw-r--   0 jez       (1000) jez       (1000)    68765 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/versioneer.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      416 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.readthedocs.yml
--rw-rw-r--   0 jez       (1000) jez       (1000)      114 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/.flake8
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3/
--rw-rw-r--   0 jez       (1000) jez       (1000)     1995 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/ui.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    34560 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/assemble.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     2644 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/dataset.schema.yaml
--rw-rw-r--   0 jez       (1000) jez       (1000)    24075 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/wagl.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3/metadata/
--rw-rw-r--   0 jez       (1000) jez       (1000)     3338 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/metadata/groundstations.json
--rw-rw-r--   0 jez       (1000) jez       (1000)     1483 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/metadata/__init__.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     2488 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/metadata/valid_region.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    12239 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/metadata/sensors.json
--rw-rw-r--   0 jez       (1000) jez       (1000)     3223 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/utils.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    19263 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/validate.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3/scripts/
--rw-rw-r--   0 jez       (1000) jez       (1000)     2511 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/scripts/tostac.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     2311 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/scripts/packagewagl.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      657 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/scripts/prepare.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    15942 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/scripts/recompress.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      310 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/scripts/__init__.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      330 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/__init__.py
-drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3/prepare/
--rw-rw-r--   0 jez       (1000) jez       (1000)    17462 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/s2_l1c_aws_pds_prepare.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     4589 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/noaa_c_c_prwtreatm_1_prepare.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    23189 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/s2_prepare_cophub_zip.py
--rw-rw-r--   0 jez       (1000) jez       (1000)        0 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/__init__.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     7525 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/nasa_c_m_mcd43a1_6_prepare.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    17681 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/prepare/landsat_l1_prepare.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     8967 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/documents.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    12868 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/model.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    28421 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/images.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     5330 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/verify.py
--rw-rw-r--   0 jez       (1000) jez       (1000)      497 2020-06-11 06:09:51.000000 eodatasets3-0.9.2/eodatasets3/_version.py
--rw-rw-r--   0 jez       (1000) jez       (1000)     9833 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/serialise.py
--rw-rw-r--   0 jez       (1000) jez       (1000)    14622 2020-06-11 06:06:11.000000 eodatasets3-0.9.2/eodatasets3/properties.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.694911 eodatasets3-0.9.3/
+-rw-rw-r--   0 jez       (1000) jez       (1000)      485 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.coveragerc
+-rw-rw-r--   0 jez       (1000) jez       (1000)      114 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.flake8
+-rw-rw-r--   0 jez       (1000) jez       (1000)      195 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.gitattributes
+-rw-rw-r--   0 jez       (1000) jez       (1000)      252 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.gitignore
+-rw-rw-r--   0 jez       (1000) jez       (1000)      365 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.pre-commit-config.yaml
+-rw-rw-r--   0 jez       (1000) jez       (1000)      416 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/.readthedocs.yml
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3040 2020-07-03 07:10:30.000000 eodatasets3-0.9.3/.travis.yml
+-rw-rw-r--   0 jez       (1000) jez       (1000)    11358 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/LICENSE
+-rw-rw-r--   0 jez       (1000) jez       (1000)       99 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/MANIFEST.in
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8988 2020-07-03 07:13:01.695911 eodatasets3-0.9.3/PKG-INFO
+-rw-rw-r--   0 jez       (1000) jez       (1000)     6823 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/README.md
+-rwxrwxr-x   0 jez       (1000) jez       (1000)      244 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/check-code.sh
+-rw-rw-r--   0 jez       (1000) jez       (1000)      376 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/conftest.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.674911 eodatasets3-0.9.3/docs/
+-rw-rw-r--   0 jez       (1000) jez       (1000)        8 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/.gitignore
+-rw-rw-r--   0 jez       (1000) jez       (1000)      634 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/Makefile
+-rw-rw-r--   0 jez       (1000) jez       (1000)     1522 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/conf.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     4809 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/index.rst
+-rw-rw-r--   0 jez       (1000) jez       (1000)      760 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/make.bat
+-rw-rw-r--   0 jez       (1000) jez       (1000)       27 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/docs/requirements.txt
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.696911 eodatasets3-0.9.3/eodatasets3/
+-rw-rw-r--   0 jez       (1000) jez       (1000)      330 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)      497 2020-07-03 07:13:01.696911 eodatasets3-0.9.3/eodatasets3/_version.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    34560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/assemble.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2644 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/dataset.schema.yaml
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8967 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/documents.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    28472 2020-07-03 07:10:30.000000 eodatasets3-0.9.3/eodatasets3/images.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.676911 eodatasets3-0.9.3/eodatasets3/metadata/
+-rw-rw-r--   0 jez       (1000) jez       (1000)     1483 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/metadata/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3338 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/metadata/groundstations.json
+-rw-rw-r--   0 jez       (1000) jez       (1000)    12239 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/metadata/sensors.json
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2488 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/metadata/valid_region.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    12868 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/model.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.677911 eodatasets3-0.9.3/eodatasets3/prepare/
+-rw-rw-r--   0 jez       (1000) jez       (1000)        0 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/prepare/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    17742 2020-07-03 07:10:30.000000 eodatasets3-0.9.3/eodatasets3/prepare/landsat_l1_prepare.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7525 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/prepare/nasa_c_m_mcd43a1_6_prepare.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     4589 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/prepare/noaa_c_c_prwtreatm_1_prepare.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    17462 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/prepare/s2_l1c_aws_pds_prepare.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    23189 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/prepare/s2_prepare_cophub_zip.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    14622 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/properties.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.677911 eodatasets3-0.9.3/eodatasets3/scripts/
+-rw-rw-r--   0 jez       (1000) jez       (1000)      310 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/scripts/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2311 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/scripts/packagewagl.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)      657 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/scripts/prepare.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    15942 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/scripts/recompress.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2511 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/scripts/tostac.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     9833 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/serialise.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     1995 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/ui.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3223 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/utils.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    19263 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/validate.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     5330 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/verify.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    24075 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/eodatasets3/wagl.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.676911 eodatasets3-0.9.3/eodatasets3.egg-info/
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8988 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/PKG-INFO
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8097 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/SOURCES.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/dependency_links.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)      304 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/entry_points.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)      561 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/requires.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)       12 2020-07-03 07:13:01.000000 eodatasets3-0.9.3/eodatasets3.egg-info/top_level.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)     5325 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/pylintrc
+-rw-rw-r--   0 jez       (1000) jez       (1000)      278 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/pyproject.toml
+-rw-rw-r--   0 jez       (1000) jez       (1000)      815 2020-07-03 07:13:01.695911 eodatasets3-0.9.3/setup.cfg
+-rwxrwxr-x   0 jez       (1000) jez       (1000)     2377 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/setup.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.677911 eodatasets3-0.9.3/tests/
+-rw-rw-r--   0 jez       (1000) jez       (1000)     6412 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/__init__.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.679911 eodatasets3-0.9.3/tests/integration/
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2628 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2021 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/common.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    20818 2020-07-03 07:10:30.000000 eodatasets3-0.9.3/tests/integration/conftest.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.682911 eodatasets3-0.9.3/tests/integration/data/
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2430 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_089080_20160302_20170328_01_T1.yaml
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.686911 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/
+-rw-rw-r--   0 jez       (1000) jez       (1000)   117392 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_ANG.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B1.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B10.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B11.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B2.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B3.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B4.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B5.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B6.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B7.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B8.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B9.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_BQA.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8633 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_MTL.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)    87879 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1.tar.gz
+-rw-rw-r--   0 jez       (1000) jez       (1000)    34477 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LE07_L1GT_104078_20131209_20161119_01_T2.tar.gz
+-rw-rw-r--   0 jez       (1000) jez       (1000)   143360 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LE07_L1TP_104078_20130429_20161124_01_T1.tar
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.686911 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/
+-rw-rw-r--   0 jez       (1000) jez       (1000)      948 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/ga-metadata.yaml
+-rw-rw-r--   0 jez       (1000) jez       (1000)      456 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/package.sha1
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.686911 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/
+-rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/406.000.2018001004744204.ASN
+-rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/407.000.2018001004819738.ASN
+-rw-rw-r--   0 jez       (1000) jez       (1000)        1 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/407.001.2018001004824874.ASN
+-rw-rw-r--   0 jez       (1000) jez       (1000)     2739 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_IDF.xml
+-rw-rw-r--   0 jez       (1000) jez       (1000)      256 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_MD5.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)   430181 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/LT05_L1TP_090085_19970406_20161231_01_T1.tar.gz
+-rw-rw-r--   0 jez       (1000) jez       (1000)  1837225 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/S2A_MSIL1C_20180629T000241_N0206_R030_T56JMM_20180629T012042.zip
+-rw-rw-r--   0 jez       (1000) jez       (1000)  1989815 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/S2B_OPER_MSI_L1C_TL_EPAE_20180617T013729_A006677_T55JGF_N02.06.AWSPDS.zip
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.686911 eodatasets3-0.9.3/tests/integration/data/noaa_c_c_prwtreatm_1/
+-rw-rw-r--   0 jez       (1000) jez       (1000)   113307 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/noaa_c_c_prwtreatm_1/pr_wtr.eatm.2018.test.nc
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.687911 eodatasets3-0.9.3/tests/integration/data/wagl-input/
+-rwxrwxr-x   0 jez       (1000) jez       (1000)     2485 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC08_L1TP_092084_20160628_20170323_01_T1.yaml
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.688911 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/
+-rw-rw-r--   0 jez       (1000) jez       (1000)    43878 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img
+-rw-rw-r--   0 jez       (1000) jez       (1000)     1612 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-0242778241.aux.xml
+-rwxrwxr-x   0 jez       (1000) jez       (1000)     1612 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-8404334440.aux.xml
+-rw-rw-r--   0 jez       (1000) jez       (1000)      186 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.tmp..img.aux.xml
+-rwxrwxr-x   0 jez       (1000) jez       (1000)      547 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.yaml
+-rwxrwxr-x   0 jez       (1000) jez       (1000)      896 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.gqa.yaml
+-rwxrwxr-x   0 jez       (1000) jez       (1000)      122 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.tesp.yaml
+-rw-rw-r--   0 jez       (1000) jez       (1000)  5742248 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.wagl.h5
+-rw-rw-r--   0 jez       (1000) jez       (1000)     4114 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/h5downsample.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.692911 eodatasets3-0.9.3/tests/integration/prepare/
+-rw-rw-r--   0 jez       (1000) jez       (1000)        0 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/prepare/__init__.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     4354 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/prepare/test_noaa_c_c_prwtreatm_1.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3920 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/prepare/test_prepare_landsat_l1.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    12205 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/prepare/test_prepare_s2a_l1c_safe.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     9636 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/prepare/test_prepare_s2b_l1c_awspds.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.670911 eodatasets3-0.9.3/tests/integration/recompress_packed/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.670911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.670911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.670911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.693911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/
+-rw-rw-r--   0 jez       (1000) jez       (1000)    99552 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/LC08_L1TP_091075_20161213_20170316_01_T2.tar.gz
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.693911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/
+-rw-rw-r--   0 jez       (1000) jez       (1000)   155648 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/LE07_L1GT_091080_20080114_20161231_01_T2.tar.gz
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.693911 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/
+-rw-rw-r--   0 jez       (1000) jez       (1000)    28918 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2.tar.gz
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.671911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.694911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/
+-rw-rw-r--   0 jez       (1000) jez       (1000)    34884 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_ANG.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B1.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B2.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B3.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B4.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B5.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B6.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3960 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B7.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7560 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_BQA.TIF
+-rw-rw-r--   0 jez       (1000) jez       (1000)     6693 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_MTL.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)     8686 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/README.GTF
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.694911 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/extras/
+-rw-rw-r--   0 jez       (1000) jez       (1000)       62 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/extras/example-file.txt
+-rw-rw-r--   0 jez       (1000) jez       (1000)    15433 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_assemble.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     7071 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_image.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    25570 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_packagewagl.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    16920 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_recompress.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)      572 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_serialise.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)    15329 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/integration/test_validate.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3405 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/test_documents.py
+-rw-rw-r--   0 jez       (1000) jez       (1000)     3042 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/test_verify.py
+drwxrwxr-x   0 jez       (1000) jez       (1000)        0 2020-07-03 07:13:01.694911 eodatasets3-0.9.3/tests/utils/
+-rwxrwxr-x   0 jez       (1000) jez       (1000)     2112 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/tests/utils/subset_noaa_c_c_prwtreatm_1
+-rw-rw-r--   0 jez       (1000) jez       (1000)    68765 2020-06-11 06:06:11.000000 eodatasets3-0.9.3/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eodatasets3-0.9.2/LICENSE` & `eodatasets3-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/pylintrc` & `eodatasets3-0.9.3/pylintrc`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/setup.py` & `eodatasets3-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/setup.cfg` & `eodatasets3-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3.egg-info/SOURCES.txt` & `eodatasets3-0.9.3/eodatasets3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3.egg-info/PKG-INFO` & `eodatasets3-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodatasets3
-Version: 0.9.2
+Version: 0.9.3
 Summary: Packaging, metadata and provenance for OpenDataCube EO3 datasets
 Home-page: https://github.com/GeoscienceAustralia/eo-datasets
 Author: Open Data Cube
 License: Apache Software License 2.0
 Description: ## EO Datasets
         
         [![Build Status](
```

### Comparing `eodatasets3-0.9.2/eodatasets3.egg-info/requires.txt` & `eodatasets3-0.9.3/eodatasets3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/docs/index.rst` & `eodatasets3-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/docs/make.bat` & `eodatasets3-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/docs/Makefile` & `eodatasets3-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/docs/conf.py` & `eodatasets3-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/README.md` & `eodatasets3-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/PKG-INFO` & `eodatasets3-0.9.3/eodatasets3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodatasets3
-Version: 0.9.2
+Version: 0.9.3
 Summary: Packaging, metadata and provenance for OpenDataCube EO3 datasets
 Home-page: https://github.com/GeoscienceAustralia/eo-datasets
 Author: Open Data Cube
 License: Apache Software License 2.0
 Description: ## EO Datasets
         
         [![Build Status](
```

### Comparing `eodatasets3-0.9.2/.travis.yml` & `eodatasets3-0.9.3/.travis.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     - liblapack-dev
     - libproj-dev
 install:
 - export CPLUS_INCLUDE_PATH="/usr/include/gdal"
 - export C_INCLUDE_PATH="/usr/include/gdal"
   # The python gdal bindings version need to match the gdal version of the system
 - travis_retry pip install --upgrade pip cattrs
-- travis_retry pip install --upgrade pytest pytest-cov coveralls GDAL==1.10.0 rasterio[s3]
+- travis_retry pip install --upgrade pytest pytest-cov coveralls GDAL==1.10.0 rasterio[s3] 'scipy<1.5.0'
   # flake8 version should match .pre-commit-config.yaml
 - travis_retry pip install flake8==3.8.2
 - travis_retry pip install -e .[test]
 - pip freeze
   # Either both set or none. See: https://github.com/mapbox/rasterio/issues/1494
 - '[ "${AWS_SECRET_ACCESS_KEY}" ] || unset AWS_ACCESS_KEY_ID'
```

### Comparing `eodatasets3-0.9.2/tests/utils/subset_noaa_c_c_prwtreatm_1` & `eodatasets3-0.9.3/tests/utils/subset_noaa_c_c_prwtreatm_1`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/test_serialise.py` & `eodatasets3-0.9.3/tests/integration/test_serialise.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/h5downsample.py` & `eodatasets3-0.9.3/tests/integration/h5downsample.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/common.py` & `eodatasets3-0.9.3/tests/integration/common.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LT05_L1TP_090085_19970406_20161231_01_T1.tar.gz` & `eodatasets3-0.9.3/tests/integration/data/LT05_L1TP_090085_19970406_20161231_01_T1.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/S2B_OPER_MSI_L1C_TL_EPAE_20180617T013729_A006677_T55JGF_N02.06.AWSPDS.zip` & `eodatasets3-0.9.3/tests/integration/data/S2B_OPER_MSI_L1C_TL_EPAE_20180617T013729_A006677_T55JGF_N02.06.AWSPDS.zip`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B11.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B11.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B3.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B3.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_MTL.txt` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_MTL.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B10.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B10.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B8.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B8.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_ANG.txt` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_ANG.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B6.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B6.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B1.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B1.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B4.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B4.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B5.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B5.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_BQA.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_BQA.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B7.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B7.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B9.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B9.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B2.TIF` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1/LC08_L1TP_090084_20160121_20170405_01_T1_B2.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/S2A_MSIL1C_20180629T000241_N0206_R030_T56JMM_20180629T012042.zip` & `eodatasets3-0.9.3/tests/integration/data/S2A_MSIL1C_20180629T000241_N0206_R030_T56JMM_20180629T012042.zip`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_IDF.xml` & `eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/product/LC80840720742017365LGN00_IDF.xml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/ga-metadata.yaml` & `eodatasets3-0.9.3/tests/integration/data/LS8_OLITIRS_STD-MD_P00_LC80840720742017365LGN00_084_072-074_20180101T004644Z20180101T004824_1/ga-metadata.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LE07_L1GT_104078_20131209_20161119_01_T2.tar.gz` & `eodatasets3-0.9.3/tests/integration/data/LE07_L1GT_104078_20131209_20161119_01_T2.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_089080_20160302_20170328_01_T1.yaml` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_089080_20160302_20170328_01_T1.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LE07_L1TP_104078_20130429_20161124_01_T1.tar` & `eodatasets3-0.9.3/tests/integration/data/LE07_L1TP_104078_20130429_20161124_01_T1.tar`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/noaa_c_c_prwtreatm_1/pr_wtr.eatm.2018.test.nc` & `eodatasets3-0.9.3/tests/integration/data/noaa_c_c_prwtreatm_1/pr_wtr.eatm.2018.test.nc`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1.tar.gz` & `eodatasets3-0.9.3/tests/integration/data/LC08_L1TP_090084_20160121_20170405_01_T1.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC08_L1TP_092084_20160628_20170323_01_T1.yaml` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC08_L1TP_092084_20160628_20170323_01_T1.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.yaml` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.wagl.h5` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.wagl.h5`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-0242778241.aux.xml` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-0242778241.aux.xml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-8404334440.aux.xml` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.fmask.img-luigi-tmp-8404334440.aux.xml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.gqa.yaml` & `eodatasets3-0.9.3/tests/integration/data/wagl-input/LC80920842016180LGN01/LC80920842016180LGN01.gqa.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B4.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B4.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B3.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B3.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B2.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B2.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_MTL.txt` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_MTL.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/README.GTF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/README.GTF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B5.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B5.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_BQA.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_BQA.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_ANG.txt` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_ANG.txt`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B1.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B1.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B6.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B6.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B7.TIF` & `eodatasets3-0.9.3/tests/integration/recompress_unpackaged/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2_B7.TIF`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/test_assemble.py` & `eodatasets3-0.9.3/tests/integration/test_assemble.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/__init__.py` & `eodatasets3-0.9.3/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/LC08_L1TP_091075_20161213_20170316_01_T2.tar.gz` & `eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_075/LC80910752016348/LC08_L1TP_091075_20161213_20170316_01_T2.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/LE07_L1GT_091080_20080114_20161231_01_T2.tar.gz` & `eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/091_080/LE70910802008014/LE07_L1GT_091080_20080114_20161231_01_T2.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2.tar.gz` & `eodatasets3-0.9.3/tests/integration/recompress_packed/USGS/L1/Landsat/C1/092_091/LT50920911991126/LT05_L1GS_092091_19910506_20170126_01_T2.tar.gz`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/prepare/test_prepare_s2a_l1c_safe.py` & `eodatasets3-0.9.3/tests/integration/prepare/test_prepare_s2a_l1c_safe.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/prepare/test_prepare_landsat_l1.py` & `eodatasets3-0.9.3/tests/integration/prepare/test_prepare_landsat_l1.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/prepare/test_noaa_c_c_prwtreatm_1.py` & `eodatasets3-0.9.3/tests/integration/prepare/test_noaa_c_c_prwtreatm_1.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/prepare/test_prepare_s2b_l1c_awspds.py` & `eodatasets3-0.9.3/tests/integration/prepare/test_prepare_s2b_l1c_awspds.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/conftest.py` & `eodatasets3-0.9.3/tests/integration/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,23 +174,33 @@
             "landsat:processing_software_version": "LPGS_2.7.0",
             "landsat:station_id": "LGN",
             "landsat:wrs_path": 90,
             "landsat:wrs_row": 84,
         },
         "crs": "epsg:32655",
         "geometry": {
-            "coordinates": (
-                (
-                    (879_315.0, -3_714_585.0),
-                    (879_315.0, -3_953_115.0),
-                    (641_985.0, -3_953_115.0),
-                    (641_985.0, -3_714_585.0),
-                    (879_315.0, -3_714_585.0),
-                ),
-            ),
+            "coordinates": [
+                [
+                    [879307.5, -3776885.4340469087],
+                    [879307.5, -3778240.713151076],
+                    [839623.3108524992, -3938223.736900397],
+                    [832105.7835592609, -3953107.5],
+                    [831455.8296215904, -3953107.5],
+                    [831453.7930575205, -3953115.0],
+                    [819969.5411349908, -3953115.0],
+                    [641985.0, -3906446.160824098],
+                    [641985.0, -3889797.3351159613],
+                    [685647.6920251067, -3717468.346156044],
+                    [688909.3673333039, -3714585.0],
+                    [708011.4230769231, -3714585.0],
+                    [879315.0, -3761214.3020833335],
+                    [879315.0, -3776857.8139976147],
+                    [879307.5, -3776885.4340469087],
+                ]
+            ],
             "type": "Polygon",
         },
         "grids": {
             "default": {
                 "shape": (60, 60),
                 "transform": (
                     3955.5,
@@ -331,23 +341,45 @@
             "landsat:processing_software_version": "LPGS_12.8.2",
             "landsat:station_id": "ASA",
             "landsat:scan_gap_interpolation": 2.0,
             "landsat:wrs_path": 104,
             "landsat:wrs_row": 78,
         },
         "geometry": {
-            "coordinates": (
-                (
-                    (770_115.0, -2_768_985.0),
-                    (770_115.0, -2_981_715.0),
-                    (525_285.0, -2_981_715.0),
-                    (525_285.0, -2_768_985.0),
-                    (770_115.0, -2_768_985.0),
-                ),
-            ),
+            "coordinates": [
+                [
+                    [563899.8055973209, -2773901.091688032],
+                    [565174.4110839436, -2768992.5],
+                    [570160.9334151996, -2768992.5],
+                    [570170.5, -2768985.0],
+                    [570223.8384207273, -2768992.5],
+                    [588295.85185022, -2768992.5],
+                    [721491.3496511441, -2790262.4648538055],
+                    [721949.2518894314, -2790326.8512143376],
+                    [758758.6847331291, -2797433.428778118],
+                    [770115.0, -2803848.537800015],
+                    [770115.0, -2819232.438669062],
+                    [745548.1744650088, -2936338.4604302375],
+                    [730486.820264895, -2981715.0],
+                    [707958.3856497289, -2981715.0],
+                    [707665.2711912903, -2981666.327459585],
+                    [695862.7971396025, -2981638.6536404933],
+                    [593801.8189357058, -2963902.554008508],
+                    [537007.2875722996, -2953328.054250119],
+                    [536671.5165534337, -2953272.2984591112],
+                    [526480.1507793682, -2945221.547092697],
+                    [525364.2405528432, -2927837.1702428674],
+                    [529047.5112406499, -2911836.1482165447],
+                    [529451.9856980122, -2906561.9692719015],
+                    [536583.4124976253, -2879098.363725102],
+                    [545784.6687009194, -2839125.873061804],
+                    [562106.6687009194, -2775306.873061804],
+                    [563899.8055973209, -2773901.091688032],
+                ]
+            ],
             "type": "Polygon",
         },
         "grids": {
             "default": {
                 "shape": (60, 60),
                 "transform": (
                     4080.500_000_000_000_5,
@@ -471,23 +503,30 @@
             "landsat:landsat_scene_id": "LT50900851997096ASA00",
             "landsat:processing_software_version": "LPGS_12.8.2",
             "landsat:station_id": "ASA",
             "landsat:wrs_path": 90,
             "landsat:wrs_row": 85,
         },
         "geometry": {
-            "coordinates": (
-                (
-                    (835_815.0, -3_881_685.0),
-                    (593_385.0, -3_881_685.0),
-                    (593_385.0, -4_101_015.0),
-                    (835_815.0, -4_101_015.0),
-                    (835_815.0, -3_881_685.0),
-                ),
-            ),
+            "coordinates": [
+                [
+                    [636860.78, -3881685.0],
+                    [593385.0, -4045573.25],
+                    [593385.0, -4062038.8525309917],
+                    [636850.5348070407, -4075317.3559092814],
+                    [768589.1325495897, -4101015.0],
+                    [790215.8408397632, -4101015.0],
+                    [795289.3607718372, -4094590.58897732],
+                    [835815.0, -3937552.555313688],
+                    [835815.0, -3920661.1474690083],
+                    [792349.4651929593, -3907382.6440907186],
+                    [657073.5519714399, -3881685.0],
+                    [636860.78, -3881685.0],
+                ]
+            ],
             "type": "Polygon",
         },
         "grids": {
             "default": {
                 "shape": (60, 60),
                 "transform": (
                     4040.5,
```

### Comparing `eodatasets3-0.9.2/tests/integration/test_recompress.py` & `eodatasets3-0.9.3/tests/integration/test_recompress.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/test_image.py` & `eodatasets3-0.9.3/tests/integration/test_image.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/test_validate.py` & `eodatasets3-0.9.3/tests/integration/test_validate.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/integration/test_packagewagl.py` & `eodatasets3-0.9.3/tests/integration/test_packagewagl.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/test_verify.py` & `eodatasets3-0.9.3/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/__init__.py` & `eodatasets3-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/tests/test_documents.py` & `eodatasets3-0.9.3/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/versioneer.py` & `eodatasets3-0.9.3/versioneer.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/ui.py` & `eodatasets3-0.9.3/eodatasets3/ui.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/assemble.py` & `eodatasets3-0.9.3/eodatasets3/assemble.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/dataset.schema.yaml` & `eodatasets3-0.9.3/eodatasets3/dataset.schema.yaml`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/wagl.py` & `eodatasets3-0.9.3/eodatasets3/wagl.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/metadata/groundstations.json` & `eodatasets3-0.9.3/eodatasets3/metadata/groundstations.json`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/metadata/__init__.py` & `eodatasets3-0.9.3/eodatasets3/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/metadata/valid_region.py` & `eodatasets3-0.9.3/eodatasets3/metadata/valid_region.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/metadata/sensors.json` & `eodatasets3-0.9.3/eodatasets3/metadata/sensors.json`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/utils.py` & `eodatasets3-0.9.3/eodatasets3/utils.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/validate.py` & `eodatasets3-0.9.3/eodatasets3/validate.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/scripts/tostac.py` & `eodatasets3-0.9.3/eodatasets3/scripts/tostac.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/scripts/packagewagl.py` & `eodatasets3-0.9.3/eodatasets3/scripts/packagewagl.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/scripts/prepare.py` & `eodatasets3-0.9.3/eodatasets3/scripts/prepare.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/scripts/recompress.py` & `eodatasets3-0.9.3/eodatasets3/scripts/recompress.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/prepare/s2_l1c_aws_pds_prepare.py` & `eodatasets3-0.9.3/eodatasets3/prepare/s2_l1c_aws_pds_prepare.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/prepare/noaa_c_c_prwtreatm_1_prepare.py` & `eodatasets3-0.9.3/eodatasets3/prepare/noaa_c_c_prwtreatm_1_prepare.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/prepare/s2_prepare_cophub_zip.py` & `eodatasets3-0.9.3/eodatasets3/prepare/s2_prepare_cophub_zip.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/prepare/nasa_c_m_mcd43a1_6_prepare.py` & `eodatasets3-0.9.3/eodatasets3/prepare/nasa_c_m_mcd43a1_6_prepare.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/prepare/landsat_l1_prepare.py` & `eodatasets3-0.9.3/eodatasets3/prepare/landsat_l1_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,15 @@
 
         band_aliases = get_band_alias_mappings(p.platform, p.instrument)
         for usgs_band_id, file_location in _iter_bands_paths(mtl_doc):
             p.note_measurement(
                 band_aliases[usgs_band_id],
                 file_location,
                 relative_to_dataset_location=True,
+                expand_valid_data=usgs_band_id != "quality",
             )
 
         p.add_accessory_file("metadata:landsat_mtl", Path(mtl_filename))
 
         return p.done()
```

### Comparing `eodatasets3-0.9.2/eodatasets3/documents.py` & `eodatasets3-0.9.3/eodatasets3/documents.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/model.py` & `eodatasets3-0.9.3/eodatasets3/model.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/images.py` & `eodatasets3-0.9.3/eodatasets3/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,17 @@
                 )
 
         self._measurements_per_grid[grid][name] = path
         if expand_valid_data:
             self._expand_valid_data_mask(grid, img, nodata)
 
     def _expand_valid_data_mask(self, grid: GridSpec, img: numpy.ndarray, nodata):
+        if nodata is None:
+            nodata = 0
+
         mask = self.mask_by_grid.get(grid)
         if mask is None:
             mask = img != nodata
         else:
             mask |= img != nodata
         self.mask_by_grid[grid] = mask
```

### Comparing `eodatasets3-0.9.2/eodatasets3/verify.py` & `eodatasets3-0.9.3/eodatasets3/verify.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/serialise.py` & `eodatasets3-0.9.3/eodatasets3/serialise.py`

 * *Files identical despite different names*

### Comparing `eodatasets3-0.9.2/eodatasets3/properties.py` & `eodatasets3-0.9.3/eodatasets3/properties.py`

 * *Files identical despite different names*

