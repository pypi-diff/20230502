# Comparing `tmp/satpy-0.9.3.tar.gz` & `tmp/satpy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/satpy-0.9.3.tar", last modified: Tue Sep 11 00:54:41 2018, max compression
+gzip compressed data, was "dist/satpy-0.9.4.tar", last modified: Sat Sep 29 16:53:44 2018, max compression
```

## Comparing `satpy-0.9.3.tar` & `satpy-0.9.4.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/doc/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/doc/source/
--rw-r--r--   0 travis    (2000) travis    (2000)     1715 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/composites.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     7857 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2500 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/examples.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     4675 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     2250 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/install.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     2746 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/multiscene.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     6360 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/overview.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     8438 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/quickstart.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     4020 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/readers.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       65 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/resample.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     3529 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/source/writers.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     3141 2018-09-11 00:43:35.000000 satpy-0.9.3/doc/Makefile
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/composites/
--rw-r--r--   0 travis    (2000) travis    (2000)    47076 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1499 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/abi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1472 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/ahi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2765 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/cloud_products.py
--rw-r--r--   0 travis    (2000) travis    (2000)    15336 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/crefl_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4308 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/sar.py
--rw-r--r--   0 travis    (2000) travis    (2000)    48427 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/composites/viirs.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/enhancements/
--rw-r--r--   0 travis    (2000) travis    (2000)     7620 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/enhancements/__init__.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/etc/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/etc/composites/
--rw-r--r--   0 travis    (2000) travis    (2000)     4944 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/abi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4713 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/ahi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      204 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/amsr2.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)       27 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/avhrr-3.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)       40 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/goes_imager.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1286 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/modis.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4503 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/msi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      429 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/msu-gs.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4940 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/olci.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)       23 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/sar-c.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      882 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/sar.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     7151 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/seviri.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      415 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/slstr.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    10772 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/viirs.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     7782 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/composites/visir.yaml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/etc/enhancements/
--rw-r--r--   0 travis    (2000) travis    (2000)    20145 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/enhancements/generic.yaml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/etc/readers/
--rw-r--r--   0 travis    (2000) travis    (2000)    11471 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/abi_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1078 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/acspo.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     9088 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/ahi_hsd.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     7909 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/amsr2_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     3346 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/avhrr_aapp_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     3704 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/avhrr_eps_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2641 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/avhrr_hrpt_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      929 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/clavrx.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     9303 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/fci_fdhsi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     3684 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/gac_lac_l1.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      593 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/generic_image.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     7518 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/geocat.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      518 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/ghrsst_osisaf.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      972 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/grib.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      959 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hdf4_caliopv3.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    10943 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hdfeos_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     7808 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hrit_electrol.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4101 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hrit_goes.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     8345 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hrit_jma.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     9254 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/hrit_msg.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2834 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/iasi_l2.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4385 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/li_l2.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2653 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/maia.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     5356 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/native_msg.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     9265 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nc_nwcsaf_msg.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     5078 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nc_nwcsaf_pps.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    10605 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nc_olci_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     8815 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nc_olci_l2.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     6499 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nc_slstr.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     3796 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/nucaps.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     5763 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/omps_edr.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     3394 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/safe_msi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     4214 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/safe_sar_c.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1050 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/scatsat1_l2b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    10144 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/viirs_compact.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    13914 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/viirs_l1b.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    19639 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/readers/viirs_sdr.yaml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/etc/writers/
--rw-r--r--   0 travis    (2000) travis    (2000)      204 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/cf.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      209 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/geotiff.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      215 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/mitiff.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      210 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/ninjotiff.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    15412 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/scmi.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      185 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/writers/simple_image.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)    28177 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/areas.def
--rw-r--r--   0 travis    (2000) travis    (2000)    80540 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/etc/eps_avhrrl1b_6.5.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/readers/
--rw-r--r--   0 travis    (2000) travis    (2000)    25061 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    22918 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/aapp_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7483 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/abi_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5722 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/acspo.py
--rw-r--r--   0 travis    (2000) travis    (2000)    20315 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/ahi_hsd.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2003 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/amsr2_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4713 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/clavrx.py
--rw-r--r--   0 travis    (2000) travis    (2000)    16242 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/eps_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2805 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/eum_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9052 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/fci_fdhsi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4564 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/file_handlers.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3605 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/gac_lac_l1.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2106 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/generic_image.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9081 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/geocat.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4649 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/ghrsst_osisaf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8951 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/grib.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3771 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hdf4_caliopv3.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3957 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hdf4_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3100 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hdf5_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17620 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hdfeos_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9383 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrit_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)    14585 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrit_electrol.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17712 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrit_goes.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7428 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrit_jma.py
--rw-r--r--   0 travis    (2000) travis    (2000)    15318 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrit_msg.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8911 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/hrpt.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5145 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/iasi_l2.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5862 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/li_l2.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5077 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/maia.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10001 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/msg_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17276 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/native_msg.py
--rw-r--r--   0 travis    (2000) travis    (2000)    36322 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/native_msg_hdr.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9953 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/nc_nwcsaf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5137 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/nc_nwcsaf_msg.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10304 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/nc_olci.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10807 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/nc_slstr.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5011 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/netcdf_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    14765 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/nucaps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4809 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/omps_edr.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7806 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/safe_msi.py
--rw-r--r--   0 travis    (2000) travis    (2000)    12049 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/safe_sar_c.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2841 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/scatsat1_l2b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6936 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17772 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/viirs_compact.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9811 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/viirs_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)    15117 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/viirs_sdr.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5973 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/xmlformat.py
--rw-r--r--   0 travis    (2000) travis    (2000)    31249 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/readers/yaml_reader.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/tests/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/tests/compositor_tests/
--rw-r--r--   0 travis    (2000) travis    (2000)     4788 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/compositor_tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2998 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/compositor_tests/test_abi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2804 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/compositor_tests/test_ahi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9140 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/compositor_tests/test_viirs.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/tests/reader_tests/
--rw-r--r--   0 travis    (2000) travis    (2000)     2565 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9345 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_abi_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6190 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_acspo.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5686 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_ahi_hsd.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7534 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_amsr2_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5572 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_clavrx.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3860 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_eum_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7655 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_geocat.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5890 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_grib.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4136 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_hdf4_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5187 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_hdf5_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5036 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_hrit_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7741 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_hrit_goes.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1867 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_msg_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6057 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_native_msg.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5251 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_netcdf_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    14987 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_nucaps.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8334 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_omps_edr.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9247 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_seviri_calibration.py
--rw-r--r--   0 travis    (2000) travis    (2000)    16108 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    12208 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_viirs_l1b.py
--rw-r--r--   0 travis    (2000) travis    (2000)    25583 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/reader_tests/test_viirs_sdr.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/tests/writer_tests/
--rw-r--r--   0 travis    (2000) travis    (2000)     1479 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5746 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_cf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3877 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_geotiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9170 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_mitiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1413 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_ninjotiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8904 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_scmi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2708 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/writer_tests/test_simple_image.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2045 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2256 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_dataset.py
--rw-r--r--   0 travis    (2000) travis    (2000)       91 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_doc.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5023 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_enhancements.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3752 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_file_handlers.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6874 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_multiscene.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1080 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_plugin.py
--rw-r--r--   0 travis    (2000) travis    (2000)    20724 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_readers.py
--rw-r--r--   0 travis    (2000) travis    (2000)    13148 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_resample.py
--rw-r--r--   0 travis    (2000) travis    (2000)    75852 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_scene.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6630 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)    11454 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_writers.py
--rw-r--r--   0 travis    (2000) travis    (2000)    22825 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/test_yaml_reader.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8943 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/tests/utils.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy/writers/
--rw-r--r--   0 travis    (2000) travis    (2000)    30491 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8971 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/cf_writer.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9010 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/geotiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)    27946 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/mitiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2932 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/ninjotiff.py
--rw-r--r--   0 travis    (2000) travis    (2000)    50391 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/scmi.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2704 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/writers/simple_image.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1960 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4249 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/config.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9966 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/dataset.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10167 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/multiscene.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17737 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/node.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2233 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/plugin_base.py
--rw-r--r--   0 travis    (2000) travis    (2000)    35778 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/resample.py
--rw-r--r--   0 travis    (2000) travis    (2000)    46692 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/scene.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6807 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)      832 2018-09-11 00:43:35.000000 satpy-0.9.3/satpy/version.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     1203 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     6120 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)      913 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        6 2018-09-11 00:54:41.000000 satpy-0.9.3/satpy.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)    35147 2018-09-11 00:43:35.000000 satpy-0.9.3/LICENSE.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      107 2018-09-11 00:43:35.000000 satpy-0.9.3/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     1047 2018-09-11 00:43:35.000000 satpy-0.9.3/README
--rw-r--r--   0 travis    (2000) travis    (2000)     1047 2018-09-11 00:43:35.000000 satpy-0.9.3/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      222 2018-09-11 00:54:41.000000 satpy-0.9.3/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     5143 2018-09-11 00:43:35.000000 satpy-0.9.3/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1203 2018-09-11 00:54:41.000000 satpy-0.9.3/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/doc/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/doc/source/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1715 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/composites.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     7857 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/conf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2500 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/examples.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     4675 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/index.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     2250 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/install.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     2746 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/multiscene.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     6360 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/overview.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     8438 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/quickstart.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     4020 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/readers.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)       65 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/resample.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     3529 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/source/writers.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     3141 2018-09-29 16:44:44.000000 satpy-0.9.4/doc/Makefile
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/composites/
+-rw-r--r--   0 travis    (2000) travis    (2000)    47076 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1499 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/abi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1472 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/ahi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2765 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/cloud_products.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    15336 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/crefl_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4308 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/sar.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    48427 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/composites/viirs.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/enhancements/
+-rw-r--r--   0 travis    (2000) travis    (2000)     7620 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/enhancements/__init__.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/etc/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/etc/composites/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4944 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/abi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4713 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/ahi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      204 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/amsr2.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)       27 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/avhrr-3.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)       40 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/goes_imager.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     1286 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/modis.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4503 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/msi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      429 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/msu-gs.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4940 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/olci.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)       23 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/sar-c.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      882 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/sar.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     7151 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/seviri.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      415 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/slstr.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    10772 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/viirs.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     7782 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/composites/visir.yaml
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/etc/enhancements/
+-rw-r--r--   0 travis    (2000) travis    (2000)    20145 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/enhancements/generic.yaml
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/etc/readers/
+-rw-r--r--   0 travis    (2000) travis    (2000)    11471 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/abi_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     1078 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/acspo.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     9088 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/ahi_hsd.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     7909 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/amsr2_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     3346 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/avhrr_aapp_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     3704 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/avhrr_eps_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     2641 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/avhrr_hrpt_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      929 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/clavrx.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     9303 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/fci_fdhsi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     3684 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/gac_lac_l1.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      593 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/generic_image.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     7518 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/geocat.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      518 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/ghrsst_osisaf.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      972 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/grib.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      959 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hdf4_caliopv3.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    10943 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hdfeos_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     7808 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hrit_electrol.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4101 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hrit_goes.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     9241 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hrit_jma.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     9254 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/hrit_msg.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     2834 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/iasi_l2.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4385 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/li_l2.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     2653 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/maia.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     5406 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/native_msg.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     9265 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nc_nwcsaf_msg.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     5078 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nc_nwcsaf_pps.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    10605 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nc_olci_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     8815 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nc_olci_l2.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     6499 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nc_slstr.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     3796 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/nucaps.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     5763 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/omps_edr.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     3394 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/safe_msi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     4214 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/safe_sar_c.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)     1050 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/scatsat1_l2b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    10144 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/viirs_compact.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    13914 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/viirs_l1b.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    19639 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/readers/viirs_sdr.yaml
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/etc/writers/
+-rw-r--r--   0 travis    (2000) travis    (2000)      204 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/cf.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      209 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/geotiff.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      215 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/mitiff.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      210 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/ninjotiff.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    15412 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/scmi.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)      185 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/writers/simple_image.yaml
+-rw-r--r--   0 travis    (2000) travis    (2000)    28177 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/areas.def
+-rw-r--r--   0 travis    (2000) travis    (2000)    80540 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/etc/eps_avhrrl1b_6.5.xml
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/readers/
+-rw-r--r--   0 travis    (2000) travis    (2000)    25183 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    21974 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/aapp_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7483 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/abi_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5722 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/acspo.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    20315 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/ahi_hsd.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2003 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/amsr2_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4713 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/clavrx.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    16615 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/eps_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2805 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/eum_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9052 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/fci_fdhsi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4564 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/file_handlers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3605 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/gac_lac_l1.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2106 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/generic_image.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9081 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/geocat.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4649 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/ghrsst_osisaf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8951 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/grib.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3771 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hdf4_caliopv3.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3957 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hdf4_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3100 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hdf5_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    17620 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hdfeos_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9383 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrit_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    14585 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrit_electrol.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    17712 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrit_goes.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7350 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrit_jma.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    15318 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrit_msg.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8911 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/hrpt.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5145 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/iasi_l2.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5862 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/li_l2.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5077 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/maia.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10001 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/msg_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    17272 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/native_msg.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    36322 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/native_msg_hdr.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9953 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/nc_nwcsaf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5137 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/nc_nwcsaf_msg.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10304 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/nc_olci.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10807 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/nc_slstr.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5011 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/netcdf_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    14765 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/nucaps.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4809 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/omps_edr.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7806 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/safe_msi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    12049 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/safe_sar_c.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2841 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/scatsat1_l2b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6936 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    17772 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/viirs_compact.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9811 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/viirs_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    15117 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/viirs_sdr.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5973 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/xmlformat.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    31249 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/readers/yaml_reader.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/tests/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/tests/compositor_tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4788 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/compositor_tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2998 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/compositor_tests/test_abi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2804 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/compositor_tests/test_ahi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9140 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/compositor_tests/test_viirs.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/tests/reader_tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)     2662 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9345 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_abi_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6190 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_acspo.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5686 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_ahi_hsd.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7534 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_amsr2_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5572 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_clavrx.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3860 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_eum_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7655 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_geocat.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5890 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_grib.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4136 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_hdf4_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5187 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_hdf5_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5036 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_hrit_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7741 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_hrit_goes.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4849 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_hrit_jma.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1867 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_msg_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6057 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_native_msg.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5251 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_netcdf_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    14987 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_nucaps.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8334 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_omps_edr.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9247 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_seviri_calibration.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    16108 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    12208 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_viirs_l1b.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    25583 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/reader_tests/test_viirs_sdr.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/tests/writer_tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1479 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5746 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_cf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3877 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_geotiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9170 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_mitiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1413 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_ninjotiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8904 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_scmi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2708 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/writer_tests/test_simple_image.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2045 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2256 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_dataset.py
+-rw-r--r--   0 travis    (2000) travis    (2000)       91 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_doc.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     5023 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_enhancements.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3752 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_file_handlers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6874 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_multiscene.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1080 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_plugin.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    20724 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_readers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    13148 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_resample.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    75852 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_scene.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6630 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    11454 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_writers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    22825 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/test_yaml_reader.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8943 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/tests/utils.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy/writers/
+-rw-r--r--   0 travis    (2000) travis    (2000)    30676 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     8971 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/cf_writer.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9010 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/geotiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    27946 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/mitiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2932 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/ninjotiff.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    50391 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/scmi.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2704 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/writers/simple_image.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1960 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4249 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/config.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9966 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/dataset.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10167 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/multiscene.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    17737 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/node.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2233 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/plugin_base.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    35778 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/resample.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    46692 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/scene.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     6807 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/utils.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      832 2018-09-29 16:44:44.000000 satpy-0.9.4/satpy/version.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1203 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)     6162 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (2000) travis    (2000)      913 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        6 2018-09-29 16:53:44.000000 satpy-0.9.4/satpy.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)    35147 2018-09-29 16:44:44.000000 satpy-0.9.4/LICENSE.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)      107 2018-09-29 16:44:44.000000 satpy-0.9.4/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     1047 2018-09-29 16:44:44.000000 satpy-0.9.4/README
+-rw-r--r--   0 travis    (2000) travis    (2000)     1047 2018-09-29 16:44:44.000000 satpy-0.9.4/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)      222 2018-09-29 16:53:44.000000 satpy-0.9.4/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)     5143 2018-09-29 16:44:44.000000 satpy-0.9.4/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1203 2018-09-29 16:53:44.000000 satpy-0.9.4/PKG-INFO
```

### Comparing `satpy-0.9.3/doc/source/composites.rst` & `satpy-0.9.4/doc/source/composites.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/conf.py` & `satpy-0.9.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/examples.rst` & `satpy-0.9.4/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/index.rst` & `satpy-0.9.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/install.rst` & `satpy-0.9.4/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/multiscene.rst` & `satpy-0.9.4/doc/source/multiscene.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/overview.rst` & `satpy-0.9.4/doc/source/overview.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/quickstart.rst` & `satpy-0.9.4/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/readers.rst` & `satpy-0.9.4/doc/source/readers.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/source/writers.rst` & `satpy-0.9.4/doc/source/writers.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/doc/Makefile` & `satpy-0.9.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/__init__.py` & `satpy-0.9.4/satpy/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/abi.py` & `satpy-0.9.4/satpy/composites/abi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/ahi.py` & `satpy-0.9.4/satpy/composites/ahi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/cloud_products.py` & `satpy-0.9.4/satpy/composites/cloud_products.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/crefl_utils.py` & `satpy-0.9.4/satpy/composites/crefl_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/sar.py` & `satpy-0.9.4/satpy/composites/sar.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/composites/viirs.py` & `satpy-0.9.4/satpy/composites/viirs.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/enhancements/__init__.py` & `satpy-0.9.4/satpy/enhancements/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/abi.yaml` & `satpy-0.9.4/satpy/etc/composites/abi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/ahi.yaml` & `satpy-0.9.4/satpy/etc/composites/ahi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/modis.yaml` & `satpy-0.9.4/satpy/etc/composites/modis.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/msi.yaml` & `satpy-0.9.4/satpy/etc/composites/msi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/olci.yaml` & `satpy-0.9.4/satpy/etc/composites/olci.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/sar.yaml` & `satpy-0.9.4/satpy/etc/composites/sar.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/seviri.yaml` & `satpy-0.9.4/satpy/etc/composites/seviri.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/viirs.yaml` & `satpy-0.9.4/satpy/etc/composites/viirs.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/composites/visir.yaml` & `satpy-0.9.4/satpy/etc/composites/visir.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/enhancements/generic.yaml` & `satpy-0.9.4/satpy/etc/enhancements/generic.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/abi_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/abi_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/acspo.yaml` & `satpy-0.9.4/satpy/etc/readers/acspo.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/ahi_hsd.yaml` & `satpy-0.9.4/satpy/etc/readers/ahi_hsd.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/amsr2_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/amsr2_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/avhrr_aapp_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/avhrr_aapp_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/avhrr_eps_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/avhrr_eps_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/avhrr_hrpt_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/avhrr_hrpt_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/clavrx.yaml` & `satpy-0.9.4/satpy/etc/readers/clavrx.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/fci_fdhsi.yaml` & `satpy-0.9.4/satpy/etc/readers/fci_fdhsi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/gac_lac_l1.yaml` & `satpy-0.9.4/satpy/etc/readers/gac_lac_l1.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/generic_image.yaml` & `satpy-0.9.4/satpy/etc/readers/generic_image.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/geocat.yaml` & `satpy-0.9.4/satpy/etc/readers/geocat.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/ghrsst_osisaf.yaml` & `satpy-0.9.4/satpy/etc/readers/ghrsst_osisaf.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/grib.yaml` & `satpy-0.9.4/satpy/etc/readers/grib.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/hdf4_caliopv3.yaml` & `satpy-0.9.4/satpy/etc/readers/hdf4_caliopv3.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/hdfeos_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/hdfeos_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/hrit_electrol.yaml` & `satpy-0.9.4/satpy/etc/readers/hrit_electrol.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/hrit_goes.yaml` & `satpy-0.9.4/satpy/etc/readers/hrit_goes.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/hrit_jma.yaml` & `satpy-0.9.4/satpy/etc/readers/hrit_jma.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -4,75 +4,107 @@
   sensors: [ahi]
   default_channels: []
   reader: !!python/name:satpy.readers.yaml_reader.FileYAMLReader
 
 file_types:
     hrit_b01:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B01_{start_time:%Y%m%d%H%M}_{segment:3s}']
+        file_patterns:
+        - 'IMG_DK01B01_{start_time:%Y%m%d%H%M}_{segment:3s}'
+        - 'IMG_DK01B01_{start_time:%Y%m%d%H%M}'
 
     hrit_b02:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B02_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B02_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B02_{start_time:%Y%m%d%H%M}'
 
     hrit_b03:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01VIS_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01VIS_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01VIS_{start_time:%Y%m%d%H%M}'
 
     hrit_b04:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B04_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B04_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B04_{start_time:%Y%m%d%H%M}'
 
     hrit_b05:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B05_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B05_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B05_{start_time:%Y%m%d%H%M}'
 
     hrit_b06:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B06_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B06_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B06_{start_time:%Y%m%d%H%M}'
 
     hrit_b07:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01IR4_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01IR4_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01IR4_{start_time:%Y%m%d%H%M}'
 
     hrit_b08:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01IR3_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01IR3_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01IR3_{start_time:%Y%m%d%H%M}'
 
     hrit_b09:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B09_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B09_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B09_{start_time:%Y%m%d%H%M}'
 
     hrit_b10:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B10_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B10_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B10_{start_time:%Y%m%d%H%M}'
 
     hrit_b11:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B11_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B11_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B11_{start_time:%Y%m%d%H%M}'
 
     hrit_b12:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B12_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B12_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B12_{start_time:%Y%m%d%H%M}'
 
     hrit_b13:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01IR1_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01IR1_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01IR1_{start_time:%Y%m%d%H%M}'
 
     hrit_b14:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B14_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B14_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B14_{start_time:%Y%m%d%H%M}'
 
     hrit_b15:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01IR2_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01IR2_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01IR2_{start_time:%Y%m%d%H%M}'
 
     hrit_b16:
         file_reader: !!python/name:satpy.readers.hrit_jma.HRITJMAFileHandler
-        file_patterns: ['IMG_DK01B16_{start_time:%Y%m%d%H%M}_{segment:03d}']
+        file_patterns:
+        - 'IMG_DK01B16_{start_time:%Y%m%d%H%M}_{segment:03d}'
+        - 'IMG_DK01B16_{start_time:%Y%m%d%H%M}'
 
 
 
 datasets:
   B01:
     name: B01
     sensor: ahi
```

### Comparing `satpy-0.9.3/satpy/etc/readers/hrit_msg.yaml` & `satpy-0.9.4/satpy/etc/readers/hrit_msg.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/iasi_l2.yaml` & `satpy-0.9.4/satpy/etc/readers/iasi_l2.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/li_l2.yaml` & `satpy-0.9.4/satpy/etc/readers/li_l2.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/maia.yaml` & `satpy-0.9.4/satpy/etc/readers/maia.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/native_msg.yaml` & `satpy-0.9.4/satpy/etc/readers/native_msg.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
   IR_016:
     name: IR_016
     resolution: 3000.403165817
     wavelength: [1.5, 1.64, 1.78]
     calibration:
       reflectance:
-        standard_name: reflectance
+        standard_name: toa_bidirectional_reflectance
         units: "%"
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -45,15 +45,15 @@
 
   IR_039:
     name: IR_039
     resolution: 3000.403165817
     wavelength: [3.48, 3.92, 4.36]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -61,15 +61,15 @@
 
   IR_087:
     name: IR_087
     resolution: 3000.403165817
     wavelength: [8.3, 8.7, 9.1]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -77,15 +77,15 @@
 
   IR_097:
     name: IR_097
     resolution: 3000.403165817
     wavelength: [9.38, 9.66, 9.94]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -93,15 +93,15 @@
 
   IR_108:
     name: IR_108
     resolution: 3000.403165817
     wavelength: [9.8, 10.8, 11.8]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -109,15 +109,15 @@
 
   IR_120:
     name: IR_120
     resolution: 3000.403165817
     wavelength: [11.0, 12.0, 13.0]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -125,15 +125,15 @@
 
   IR_134:
     name: IR_134
     resolution: 3000.403165817
     wavelength: [12.4, 13.4, 14.4]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: K
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -173,15 +173,15 @@
 
   WV_062:
     name: WV_062
     resolution: 3000.403165817
     wavelength: [5.35, 6.25, 7.15]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: "K"
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
@@ -189,15 +189,15 @@
 
   WV_073:
     name: WV_073
     resolution: 3000.403165817
     wavelength: [6.85, 7.35, 7.85]
     calibration:
       brightness_temperature:
-        standard_name: brightness_temperature
+        standard_name: toa_brightness_temperature
         units: "K"
       radiance:
         standard_name: toa_outgoing_radiance_per_unit_wavelength
         units: W m-2 um-1 sr-1
       counts:
         standard_name: counts
         units: count
```

### Comparing `satpy-0.9.3/satpy/etc/readers/nc_nwcsaf_msg.yaml` & `satpy-0.9.4/satpy/etc/readers/nc_nwcsaf_msg.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/nc_nwcsaf_pps.yaml` & `satpy-0.9.4/satpy/etc/readers/nc_nwcsaf_pps.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/nc_olci_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/nc_olci_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/nc_olci_l2.yaml` & `satpy-0.9.4/satpy/etc/readers/nc_olci_l2.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/nc_slstr.yaml` & `satpy-0.9.4/satpy/etc/readers/nc_slstr.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/nucaps.yaml` & `satpy-0.9.4/satpy/etc/readers/nucaps.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/omps_edr.yaml` & `satpy-0.9.4/satpy/etc/readers/omps_edr.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/safe_msi.yaml` & `satpy-0.9.4/satpy/etc/readers/safe_msi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/safe_sar_c.yaml` & `satpy-0.9.4/satpy/etc/readers/safe_sar_c.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/scatsat1_l2b.yaml` & `satpy-0.9.4/satpy/etc/readers/scatsat1_l2b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/viirs_compact.yaml` & `satpy-0.9.4/satpy/etc/readers/viirs_compact.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/viirs_l1b.yaml` & `satpy-0.9.4/satpy/etc/readers/viirs_l1b.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/readers/viirs_sdr.yaml` & `satpy-0.9.4/satpy/etc/readers/viirs_sdr.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/writers/scmi.yaml` & `satpy-0.9.4/satpy/etc/writers/scmi.yaml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/areas.def` & `satpy-0.9.4/satpy/etc/areas.def`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/etc/eps_avhrrl1b_6.5.xml` & `satpy-0.9.4/satpy/etc/eps_avhrrl1b_6.5.xml`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/__init__.py` & `satpy-0.9.4/satpy/readers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,16 +428,17 @@
 
     for config_file in config_files:
         config_basename = os.path.basename(config_file)
         reader_configs = config_search_paths(
             os.path.join("readers", config_basename), *search_paths)
 
         if not reader_configs:
-            LOG.warning("No reader configs found for '%s'", reader)
-            continue
+            # either the reader they asked for does not exist
+            # or satpy is improperly configured and can't find its own readers
+            raise ValueError("No reader(s) named: {}".format(reader))
 
         yield reader_configs
 
 
 def available_readers(as_dict=False):
     """Available readers based on current configuration.
```

### Comparing `satpy-0.9.3/satpy/readers/aapp_l1b.py` & `satpy-0.9.4/satpy/readers/aapp_l1b.py`

 * *Files 15% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         # return self._data.shape
         return self._shape
 
     def get_dataset(self, key, info):
         """Get a dataset from the file."""
 
         if key.name in CHANNEL_NAMES:
-            dataset = self.calibrate([key])[0]
+            dataset = self.calibrate(key)
         elif key.name in ['longitude', 'latitude']:
             if self.lons is None or self.lats is None:
                 self.navigate()
             if key.name == 'longitude':
                 dataset = create_xarray(self.lons)
             else:
                 dataset = create_xarray(self.lats)
@@ -218,75 +218,73 @@
             satint = SatelliteInterpolator(
                 (lons40km, lats40km), (rows40km, cols40km), (rows1km, cols1km),
                 along_track_order, cross_track_order)
             self.lons, self.lats = satint.interpolate()
             logger.debug("Navigation time %s", str(datetime.now() - tic))
 
     def calibrate(self,
-                  dataset_ids,
+                  dataset_id,
                   pre_launch_coeffs=False,
                   calib_coeffs=None):
         """Calibrate the data
         """
         tic = datetime.now()
 
         if calib_coeffs is None:
             calib_coeffs = {}
 
-        chns = dict((dataset_id.name, dataset_id)
-                    for dataset_id in dataset_ids)
-
-        res = []
-        # FIXME this should be done in _vis_calibrate
         units = {'reflectance': '%',
                  'brightness_temperature': 'K',
                  'counts': '',
                  'radiance': 'W*m-2*sr-1*cm ?'}
 
-        if ("3a" in chns or "3b" in chns) and self._is3b is None:
+        if dataset_id.name in ("3a", "3b") and self._is3b is None:
             # Is it 3a or 3b:
             is3b = np.expand_dims(
                 np.bitwise_and(
                     np.right_shift(self._data['scnlinbit'], 0), 1) == 1, 1)
             self._is3b = np.repeat(is3b,
                                    self._data['hrpt'][0].shape[0], axis=1)
 
-        for idx, name in enumerate(['1', '2', '3a']):
-            if name in chns:
-                coeffs = calib_coeffs.get('ch' + name)
-                # FIXME data should be masked before calibration
-                ds = create_xarray(
-                    _vis_calibrate(self._data,
-                                   idx,
-                                   chns[name].calibration,
-                                   pre_launch_coeffs,
-                                   coeffs,
-                                   mask=(name == '3a' and self._is3b)).filled(np.nan))
-
-                ds.attrs['units'] = units[chns[name].calibration]
-                ds.attrs.update(chns[name]._asdict())
-                res.append(ds)
-
-        for idx, name in enumerate(['3b', '4', '5']):
-            if name in chns:
-                ds = create_xarray(
-                    _ir_calibrate(self._header,
-                                  self._data,
-                                  idx,
-                                  chns[name].calibration,
-                                  mask=(name == '3b' and
-                                        (np.logical_not(self._is3b)))).filled(np.nan))
-
-                ds.attrs['units'] = units[chns[name].calibration]
-                ds.attrs.update(chns[name]._asdict())
-                res.append(ds)
+        try:
+            vis_idx = ['1', '2', '3a'].index(dataset_id.name)
+            ir_idx = None
+        except ValueError:
+            vis_idx = None
+            ir_idx = ['3b', '4', '5'].index(dataset_id.name)
+
+        if vis_idx is not None:
+            coeffs = calib_coeffs.get('ch' + dataset_id.name)
+            ds = create_xarray(
+                _vis_calibrate(self._data,
+                               vis_idx,
+                               dataset_id.calibration,
+                               pre_launch_coeffs,
+                               coeffs,
+                               mask=(dataset_id.name == '3a' and self._is3b)))
+        else:
+            ds = create_xarray(
+                _ir_calibrate(self._header,
+                              self._data,
+                              ir_idx,
+                              dataset_id.calibration,
+                              mask=(dataset_id.name == '3b' and
+                                    np.logical_not(self._is3b))))
+
+        if dataset_id.name == '3a' and np.all(np.isnan(ds)):
+            raise ValueError("Empty dataset for channel 3A")
+        if dataset_id.name == '3b' and np.all(np.isnan(ds)):
+            raise ValueError("Empty dataset for channel 3B")
+
+        ds.attrs['units'] = units[dataset_id.calibration]
+        ds.attrs.update(dataset_id._asdict())
 
         logger.debug("Calibration time %s", str(datetime.now() - tic))
 
-        return res
+        return ds
 
 
 AVHRR_CHANNEL_NAMES = ("1", "2", "3a", "3b", "4", "5")
 
 # AAPP 1b header
 
 _HEADERTYPE = np.dtype([("siteid", "S3"),
@@ -476,15 +474,17 @@
     # Calibration count to albedo, the calibration is performed separately for
     # two value ranges.
 
     if calib_type not in ['counts', 'radiance', 'reflectance']:
         raise ValueError('Calibration ' + calib_type + ' unknown!')
 
     arr = data["hrpt"][:, :, chn]
-    channel = np.ma.array(arr.astype(np.float), mask=mask * arr)
+    mask |= arr == 0
+
+    channel = arr.astype(np.float)
     if calib_type == 'counts':
         return channel
 
     if calib_type == 'radiance':
         logger.info("Radiances are not yet supported for " +
                     "the VIS/NIR channels!")
 
@@ -525,27 +525,31 @@
     mask2 = channel > np.expand_dims(intersection, 1)
 
     channel[mask1] = (channel * slope1 + intercept1)[mask1]
 
     channel[mask2] = (channel * slope2 + intercept2)[mask2]
 
     channel = channel.clip(min=0)
-    return np.ma.masked_invalid(channel)
+
+    return np.where(mask, np.nan, channel)
 
 
 def _ir_calibrate(header, data, irchn, calib_type, mask=False):
     """IR calibration
     *calib_type* in brightness_temperature, radiance, count
     """
 
-    count = data['hrpt'][:, :, irchn + 2].astype(np.float)
+    count = data["hrpt"][:, :, irchn + 2].astype(np.float)
 
     if calib_type == 0:
         return count
 
+    # Mask unnaturally low values
+    mask |= count == 0.0
+
     k1_ = np.expand_dims(data['calir'][:, irchn, 0, 0] / 1.0e9, 1)
     k2_ = np.expand_dims(data['calir'][:, irchn, 0, 1] / 1.0e6, 1)
     k3_ = np.expand_dims(data['calir'][:, irchn, 0, 2] / 1.0e6, 1)
 
     # Count to radiance conversion:
     rad = k1_ * count * count + k2_ * count + k3_
 
@@ -554,58 +558,37 @@
             np.equal(k1_, 0), np.equal(k2_, 0)), np.equal(k3_, 0))
     idx = np.indices((all_zero.shape[0], ))
     suspect_line_nums = np.repeat(idx[0], all_zero[:, 0])
     if suspect_line_nums.any():
         logger.info("Suspicious scan lines: %s", str(suspect_line_nums))
 
     if calib_type == 2:
-        return rad
+        mask |= rad <= 0.0
+        return np.where(mask, np.nan, rad)
 
     # Central wavenumber:
     cwnum = header['radtempcnv'][0, irchn, 0]
     if irchn == 0:
         cwnum = cwnum / 1.0e2
     else:
         cwnum = cwnum / 1.0e3
 
     bandcor_2 = header['radtempcnv'][0, irchn, 1] / 1e5
     bandcor_3 = header['radtempcnv'][0, irchn, 2] / 1e6
 
-    # Count to radiance conversion:
-    rad = k1_ * count * count + k2_ * count + k3_
-
-    if calib_type == 2:
-        return rad
-
-    all_zero = np.logical_and(
-        np.logical_and(
-            np.equal(k1_, 0), np.equal(k2_, 0)), np.equal(k3_, 0))
-    idx = np.indices((all_zero.shape[0], ))
-    suspect_line_nums = np.repeat(idx[0], all_zero[:, 0])
-    if suspect_line_nums.any():
-        logger.info("Suspect scan lines: %s", str(suspect_line_nums))
-
     ir_const_1 = 1.1910659e-5
     ir_const_2 = 1.438833
 
     t_planck = (ir_const_2 * cwnum) / \
         np.log(1 + ir_const_1 * cwnum * cwnum * cwnum / rad)
 
     # Band corrections applied to t_planck to get correct
     # brightness temperature for channel:
     if bandcor_2 < 0:  # Post AAPP-v4
         tb_ = bandcor_2 + bandcor_3 * t_planck
     else:  # AAPP 1 to 4
         tb_ = (t_planck - bandcor_2) / bandcor_3
 
-    # tb_[tb_ <= 0] = np.nan
-    # Data with count=0 are often related to erroneous (bad) lines, but in case
-    # of saturation (channel 3b) count=0 can be observed and associated to a
-    # real measurement. So we leave out this filtering to the user!
-    # tb_[count == 0] = np.nan
-    # tb_[rad == 0] = np.nan
-    tb_ = np.ma.masked_array(tb_, copy=False, mask=mask)
-    tb_ = np.ma.masked_invalid(tb_, copy=False)
-    if calib_type == 'brightness_temperature':
-        tb_ = np.ma.masked_less(tb_, 0.1, copy=False)
+    # Mask unnaturally low values
+    # mask |= tb_ < 0.1
 
-    return tb_
+    return np.where(mask, np.nan, tb_)
```

### Comparing `satpy-0.9.3/satpy/readers/abi_l1b.py` & `satpy-0.9.4/satpy/readers/abi_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/acspo.py` & `satpy-0.9.4/satpy/readers/acspo.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/ahi_hsd.py` & `satpy-0.9.4/satpy/readers/ahi_hsd.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/amsr2_l1b.py` & `satpy-0.9.4/satpy/readers/amsr2_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/clavrx.py` & `satpy-0.9.4/satpy/readers/clavrx.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/eps_l1b.py` & `satpy-0.9.4/satpy/readers/eps_l1b.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,27 +215,32 @@
         sat_zenith = np.hstack((self["ANGULAR_RELATIONS_FIRST"][:, [1]],
                                 self["ANGULAR_RELATIONS"][:, :, 1],
                                 self["ANGULAR_RELATIONS_LAST"][:, [1]]))
 
         solar_azimuth = np.hstack((self["ANGULAR_RELATIONS_FIRST"][:, [2]],
                                    self["ANGULAR_RELATIONS"][:, :, 2],
                                    self["ANGULAR_RELATIONS_LAST"][:, [2]]))
-
         sat_azimuth = np.hstack((self["ANGULAR_RELATIONS_FIRST"][:, [3]],
                                  self["ANGULAR_RELATIONS"][:, :, 3],
                                  self["ANGULAR_RELATIONS_LAST"][:, [3]]))
 
         nav_sample_rate = self["NAV_SAMPLE_RATE"]
         earth_views_per_scanline = self["EARTH_VIEWS_PER_SCANLINE"]
         if nav_sample_rate == 20 and earth_views_per_scanline == 2048:
             from geotiepoints import metop20kmto1km
+            # Note: interpolation asumes lat values values between -90 and 90
+            # Solar and satellite zenith is between 0 and 180.
+            solar_zenith -= 90
             self.sun_azi, self.sun_zen = metop20kmto1km(
                 solar_azimuth, solar_zenith)
+            self.sun_zen += 90
+            sat_zenith -= 90
             self.sat_azi, self.sat_zen = metop20kmto1km(
                 sat_azimuth, sat_zenith)
+            self.sat_zen += 90
         else:
             raise NotImplementedError("Angles expansion not implemented for " +
                                       "sample rate = " + str(nav_sample_rate) +
                                       " and earth views = " +
                                       str(earth_views_per_scanline))
         return self.sun_azi, self.sun_zen, self.sat_azi, self.sat_zen
 
@@ -355,14 +360,16 @@
                                        self["CH5_CONSTANT1"],
                                        self["CH5_CONSTANT2_SLOPE"]))
                 else:
                     array = np.ma.array(self["SCENE_RADIANCES"][:, 4, :])
 
             dataset = create_xarray(array.data).where(~array.mask)
 
+        dataset.attrs['platform_name'] = self.platform_name
+        dataset.attrs['sensor'] = self.sensor_name
         dataset.attrs.update(info)
         dataset.attrs.update(key.to_dict())
         return dataset
 
 
     def get_lonlats(self):
         if self.area is None:
```

### Comparing `satpy-0.9.3/satpy/readers/eum_base.py` & `satpy-0.9.4/satpy/readers/eum_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/fci_fdhsi.py` & `satpy-0.9.4/satpy/readers/fci_fdhsi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/file_handlers.py` & `satpy-0.9.4/satpy/readers/file_handlers.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/gac_lac_l1.py` & `satpy-0.9.4/satpy/readers/gac_lac_l1.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/generic_image.py` & `satpy-0.9.4/satpy/readers/generic_image.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/geocat.py` & `satpy-0.9.4/satpy/readers/geocat.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/ghrsst_osisaf.py` & `satpy-0.9.4/satpy/readers/ghrsst_osisaf.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/grib.py` & `satpy-0.9.4/satpy/readers/grib.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hdf4_caliopv3.py` & `satpy-0.9.4/satpy/readers/hdf4_caliopv3.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hdf4_utils.py` & `satpy-0.9.4/satpy/readers/hdf4_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hdf5_utils.py` & `satpy-0.9.4/satpy/readers/hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hdfeos_l1b.py` & `satpy-0.9.4/satpy/readers/hdfeos_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hrit_base.py` & `satpy-0.9.4/satpy/readers/hrit_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hrit_electrol.py` & `satpy-0.9.4/satpy/readers/hrit_electrol.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hrit_goes.py` & `satpy-0.9.4/satpy/readers/hrit_goes.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hrit_jma.py` & `satpy-0.9.4/satpy/readers/hrit_jma.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,28 +82,14 @@
 
 time_cds_expanded = np.dtype([('days', '>u2'),
                               ('milliseconds', '>u4'),
                               ('microseconds', '>u2'),
                               ('nanoseconds', '>u2')])
 
 
-def recarray2dict(arr):
-    res = {}
-    for dtuple in arr.dtype.descr:
-        key = dtuple[0]
-        ntype = dtuple[1]
-        data = arr[key]
-        if isinstance(ntype, list):
-            res[key] = recarray2dict(data)
-        else:
-            res[key] = data
-
-    return res
-
-
 class HRITJMAFileHandler(HRITFileHandler):
     """JMA HRIT format reader."""
 
     def __init__(self, filename, filename_info, filetype_info):
         """Initialize the reader."""
         super(HRITJMAFileHandler, self).__init__(filename, filename_info,
                                                  filetype_info,
@@ -172,27 +158,27 @@
             'some_area_name',
             "On-the-fly area",
             'geosmsg',
             proj_dict,
             ncols,
             nlines,
             area_extent)
-
-        self.area = area
-
         return area
 
     def get_dataset(self, key, info):
         """Get the dataset designated by *key*."""
         res = super(HRITJMAFileHandler, self).get_dataset(key, info)
 
         res = self.calibrate(res, key.calibration)
         res.attrs.update(info)
         res.attrs['platform_name'] = 'Himawari-8'
         res.attrs['sensor'] = 'ahi'
+        res.attrs['satellite_longitude'] = float(self.mda['projection_parameters']['SSP_longitude'])
+        res.attrs['satellite_latitude'] = 0.
+        res.attrs['satellite_altitude'] = float(self.mda['projection_parameters']['h'])
         return res
 
     def calibrate(self, data, calibration):
         """Calibrate the data."""
         tic = datetime.now()
 
         if calibration == 'counts':
```

### Comparing `satpy-0.9.3/satpy/readers/hrit_msg.py` & `satpy-0.9.4/satpy/readers/hrit_msg.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/hrpt.py` & `satpy-0.9.4/satpy/readers/hrpt.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/iasi_l2.py` & `satpy-0.9.4/satpy/readers/iasi_l2.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/li_l2.py` & `satpy-0.9.4/satpy/readers/li_l2.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/maia.py` & `satpy-0.9.4/satpy/readers/maia.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/msg_base.py` & `satpy-0.9.4/satpy/readers/msg_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/native_msg.py` & `satpy-0.9.4/satpy/readers/native_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,21 +79,21 @@
 
         # Read trailer
         self.trailer = {}
         self._read_trailer()
 
     @property
     def start_time(self):
-        return [self.header['15_DATA_HEADER']['ImageAcquisition'][
-            'PlannedAcquisitionTime']['TrueRepeatCycleStart']]
+        return self.header['15_DATA_HEADER']['ImageAcquisition'][
+            'PlannedAcquisitionTime']['TrueRepeatCycleStart']
 
     @property
     def end_time(self):
-        return [self.header['15_DATA_HEADER']['ImageAcquisition'][
-            'PlannedAcquisitionTime']['PlannedRepeatCycleEnd']]
+        return self.header['15_DATA_HEADER']['ImageAcquisition'][
+            'PlannedAcquisitionTime']['PlannedRepeatCycleEnd']
 
     def _get_data_dtype(self):
         """Get the dtype of the file based on the actual available channels"""
 
         pkhrec = [
             ('GP_PK_HEADER', GSDTRecords.gp_pk_header),
             ('GP_PK_SH1', GSDTRecords.gp_pk_sh1)
```

### Comparing `satpy-0.9.3/satpy/readers/native_msg_hdr.py` & `satpy-0.9.4/satpy/readers/native_msg_hdr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/nc_nwcsaf.py` & `satpy-0.9.4/satpy/readers/nc_nwcsaf.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/nc_nwcsaf_msg.py` & `satpy-0.9.4/satpy/readers/nc_nwcsaf_msg.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/nc_olci.py` & `satpy-0.9.4/satpy/readers/nc_olci.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/nc_slstr.py` & `satpy-0.9.4/satpy/readers/nc_slstr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/netcdf_utils.py` & `satpy-0.9.4/satpy/readers/netcdf_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/nucaps.py` & `satpy-0.9.4/satpy/readers/nucaps.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/omps_edr.py` & `satpy-0.9.4/satpy/readers/omps_edr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/safe_msi.py` & `satpy-0.9.4/satpy/readers/safe_msi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/safe_sar_c.py` & `satpy-0.9.4/satpy/readers/safe_sar_c.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/scatsat1_l2b.py` & `satpy-0.9.4/satpy/readers/scatsat1_l2b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/utils.py` & `satpy-0.9.4/satpy/readers/utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/viirs_compact.py` & `satpy-0.9.4/satpy/readers/viirs_compact.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/viirs_l1b.py` & `satpy-0.9.4/satpy/readers/viirs_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/viirs_sdr.py` & `satpy-0.9.4/satpy/readers/viirs_sdr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/xmlformat.py` & `satpy-0.9.4/satpy/readers/xmlformat.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/readers/yaml_reader.py` & `satpy-0.9.4/satpy/readers/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/compositor_tests/__init__.py` & `satpy-0.9.4/satpy/tests/compositor_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/compositor_tests/test_abi.py` & `satpy-0.9.4/satpy/tests/compositor_tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/compositor_tests/test_ahi.py` & `satpy-0.9.4/satpy/tests/compositor_tests/test_ahi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/compositor_tests/test_viirs.py` & `satpy-0.9.4/satpy/tests/compositor_tests/test_viirs.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/__init__.py` & `satpy-0.9.4/satpy/tests/reader_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
                                       test_viirs_sdr, test_viirs_l1b,
                                       test_native_msg, test_msg_base,
                                       test_hdf5_utils, test_netcdf_utils,
                                       test_hdf4_utils, test_utils,
                                       test_acspo, test_amsr2_l1b,
                                       test_omps_edr, test_nucaps, test_geocat,
                                       test_seviri_calibration, test_clavrx,
-                                      test_grib, test_hrit_goes, test_ahi_hsd)
+                                      test_grib, test_hrit_goes, test_ahi_hsd,
+                                      test_hrit_jma)
 
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
 
 
@@ -59,9 +60,10 @@
     mysuite.addTests(test_nucaps.suite())
     mysuite.addTests(test_geocat.suite())
     mysuite.addTests(test_seviri_calibration.suite())
     mysuite.addTests(test_clavrx.suite())
     mysuite.addTests(test_grib.suite())
     mysuite.addTests(test_hrit_goes.suite())
     mysuite.addTests(test_ahi_hsd.suite())
+    mysuite.addTests(test_hrit_jma.suite())
 
     return mysuite
```

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_abi_l1b.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_abi_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_acspo.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_acspo.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_ahi_hsd.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_ahi_hsd.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_amsr2_l1b.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_amsr2_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_clavrx.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_clavrx.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_eum_base.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_eum_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_geocat.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_geocat.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_grib.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_grib.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_hdf4_utils.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_hdf4_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_hdf5_utils.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_hrit_base.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_hrit_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_hrit_goes.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_hrit_goes.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_msg_base.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_msg_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_native_msg.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_native_msg.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_netcdf_utils.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_netcdf_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_nucaps.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_nucaps.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_omps_edr.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_omps_edr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_seviri_calibration.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_seviri_calibration.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_utils.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_viirs_l1b.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_viirs_l1b.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/reader_tests/test_viirs_sdr.py` & `satpy-0.9.4/satpy/tests/reader_tests/test_viirs_sdr.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/__init__.py` & `satpy-0.9.4/satpy/tests/writer_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_cf.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_cf.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_geotiff.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_geotiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_mitiff.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_mitiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_ninjotiff.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_ninjotiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_scmi.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_scmi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/writer_tests/test_simple_image.py` & `satpy-0.9.4/satpy/tests/writer_tests/test_simple_image.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/__init__.py` & `satpy-0.9.4/satpy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_dataset.py` & `satpy-0.9.4/satpy/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_enhancements.py` & `satpy-0.9.4/satpy/tests/test_enhancements.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_file_handlers.py` & `satpy-0.9.4/satpy/tests/test_file_handlers.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_multiscene.py` & `satpy-0.9.4/satpy/tests/test_multiscene.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_plugin.py` & `satpy-0.9.4/satpy/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_readers.py` & `satpy-0.9.4/satpy/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_resample.py` & `satpy-0.9.4/satpy/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_scene.py` & `satpy-0.9.4/satpy/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_utils.py` & `satpy-0.9.4/satpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_writers.py` & `satpy-0.9.4/satpy/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/test_yaml_reader.py` & `satpy-0.9.4/satpy/tests/test_yaml_reader.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/tests/utils.py` & `satpy-0.9.4/satpy/tests/utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/__init__.py` & `satpy-0.9.4/satpy/writers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         return "RGBA"
     else:
         raise RuntimeError("Can't determine 'mode' of dataset: %s" %
                            str(dataset))
 
 
 def add_overlay(orig, area, coast_dir, color=(0, 0, 0), width=0.5, resolution=None,
-                level_coast=1, level_borders=1):
+                level_coast=1, level_borders=1, fill_value=None):
     """Add coastline and political borders to image, using *color* (tuple
     of integers between 0 and 255).
     Warning: Loses the masks !
     *resolution* is chosen automatically if None (default), otherwise it should be one of:
     +-----+-------------------------+---------+
     | 'f' | Full resolution         | 0.04 km |
     | 'h' | High resolution         | 0.2 km  |
@@ -220,15 +220,15 @@
         elif res > 200:
             resolution = "h"
         else:
             resolution = "f"
 
         LOG.debug("Automagically choose resolution %s", resolution)
 
-    img = orig.pil_image()
+    img = orig.pil_image(fill_value=fill_value)
     cw_ = ContourWriterAGG(coast_dir)
     cw_.add_coastlines(img, area, outline=color,
                        resolution=resolution, width=width, level=level_coast)
     cw_.add_borders(img, area, outline=color,
                     resolution=resolution, width=width, level=level_borders)
 
     arr = da.from_array(np.array(img) / 255.0, chunks=CHUNK_SIZE)
@@ -273,15 +273,15 @@
 
     orig.data = xr.DataArray(arr, dims=['y', 'x', 'bands'],
                              coords={'y': orig.data.coords['y'],
                                      'x': orig.data.coords['x'],
                                      'bands': list(img.mode)})
 
 
-def add_decorate(orig, **decorate):
+def add_decorate(orig, fill_value=None, **decorate):
     """Decorate an image with text and/or logos/images.
 
     This call adds text/logos in order as given in the input to keep the
     alignment features available in pydecorate.
 
     An example of the decorate config::
 
@@ -308,15 +308,15 @@
     align is a special keyword telling where in the image to start adding features, top_bottom is either top or bottom
     and left_right is either left or right.
     """
     LOG.info("Decorate image.")
 
     # Need to create this here to possible keep the alignment
     # when adding text and/or logo with pydecorate
-    img_orig = orig.pil_image()
+    img_orig = orig.pil_image(fill_value=fill_value)
     from pydecorate import DecoratorAGG
     dc = DecoratorAGG(img_orig)
 
     # decorate need to be a list to maintain the alignment
     # as ordered in the list
     if 'decorate' in decorate:
         for dec in decorate['decorate']:
@@ -327,15 +327,16 @@
 
 
 def get_enhanced_image(dataset,
                        enhancer=None,
                        ppp_config_dir=None,
                        enhancement_config_file=None,
                        overlay=None,
-                       decorate=None):
+                       decorate=None,
+                       fill_value=None):
     if ppp_config_dir is None:
         ppp_config_dir = get_environ_config_dir()
 
     if enhancer is None:
         enhancer = Enhancer(ppp_config_dir, enhancement_config_file)
 
     # Create an image for enhancement
@@ -346,18 +347,18 @@
     else:
         if dataset.attrs.get("sensor", None):
             enhancer.add_sensor_enhancements(dataset.attrs["sensor"])
 
         enhancer.apply(img, **dataset.attrs)
 
     if overlay is not None:
-        add_overlay(img, dataset.attrs['area'], **overlay)
+        add_overlay(img, dataset.attrs['area'], fill_value=fill_value, **overlay)
 
     if decorate is not None:
-        add_decorate(img, **decorate)
+        add_decorate(img, fill_value=fill_value, **decorate)
 
     return img
 
 
 def show(dataset, **kwargs):
     """Display the dataset as an image.
     """
@@ -555,15 +556,15 @@
         This method creates an enhanced image using `get_enhanced_image`. The
         image is then passed to `save_image`. See both of these functions for
         more details on the arguments passed to this method.
 
         """
         img = get_enhanced_image(
             dataset.squeeze(), self.enhancer, overlay=overlay,
-            decorate=decorate)
+            decorate=decorate, fill_value=fill_value)
         return self.save_image(img, filename=filename, compute=compute,
                                fill_value=fill_value, **kwargs)
 
     def save_image(self, img, filename=None, compute=True, **kwargs):
         """Save Image object to a given ``filename``.
 
         Args:
```

### Comparing `satpy-0.9.3/satpy/writers/cf_writer.py` & `satpy-0.9.4/satpy/writers/cf_writer.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/geotiff.py` & `satpy-0.9.4/satpy/writers/geotiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/mitiff.py` & `satpy-0.9.4/satpy/writers/mitiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/ninjotiff.py` & `satpy-0.9.4/satpy/writers/ninjotiff.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/scmi.py` & `satpy-0.9.4/satpy/writers/scmi.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/writers/simple_image.py` & `satpy-0.9.4/satpy/writers/simple_image.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/__init__.py` & `satpy-0.9.4/satpy/__init__.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/config.py` & `satpy-0.9.4/satpy/config.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/dataset.py` & `satpy-0.9.4/satpy/dataset.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/multiscene.py` & `satpy-0.9.4/satpy/multiscene.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/node.py` & `satpy-0.9.4/satpy/node.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/plugin_base.py` & `satpy-0.9.4/satpy/plugin_base.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/resample.py` & `satpy-0.9.4/satpy/resample.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/scene.py` & `satpy-0.9.4/satpy/scene.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/utils.py` & `satpy-0.9.4/satpy/utils.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/satpy/version.py` & `satpy-0.9.4/satpy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Version file.
 """
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
```

### Comparing `satpy-0.9.3/satpy.egg-info/PKG-INFO` & `satpy-0.9.4/satpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satpy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Meteorological post processing package
 Home-page: https://github.com/pytroll/satpy
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `satpy-0.9.3/satpy.egg-info/SOURCES.txt` & `satpy-0.9.4/satpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 satpy/tests/reader_tests/test_eum_base.py
 satpy/tests/reader_tests/test_geocat.py
 satpy/tests/reader_tests/test_grib.py
 satpy/tests/reader_tests/test_hdf4_utils.py
 satpy/tests/reader_tests/test_hdf5_utils.py
 satpy/tests/reader_tests/test_hrit_base.py
 satpy/tests/reader_tests/test_hrit_goes.py
+satpy/tests/reader_tests/test_hrit_jma.py
 satpy/tests/reader_tests/test_msg_base.py
 satpy/tests/reader_tests/test_native_msg.py
 satpy/tests/reader_tests/test_netcdf_utils.py
 satpy/tests/reader_tests/test_nucaps.py
 satpy/tests/reader_tests/test_omps_edr.py
 satpy/tests/reader_tests/test_seviri_calibration.py
 satpy/tests/reader_tests/test_utils.py
```

### Comparing `satpy-0.9.3/satpy.egg-info/requires.txt` & `satpy-0.9.4/satpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/LICENSE.txt` & `satpy-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/README` & `satpy-0.9.4/README`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/README.rst` & `satpy-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/setup.py` & `satpy-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `satpy-0.9.3/PKG-INFO` & `satpy-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satpy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Meteorological post processing package
 Home-page: https://github.com/pytroll/satpy
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

