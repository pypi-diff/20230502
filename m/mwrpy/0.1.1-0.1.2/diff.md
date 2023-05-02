# Comparing `tmp/mwrpy-0.1.1.tar.gz` & `tmp/mwrpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.1.tar", last modified: Tue May  2 13:26:06 2023, max compression
+gzip compressed data, was "mwrpy-0.1.2.tar", last modified: Tue May  2 14:19:57 2023, max compression
```

## Comparing `mwrpy-0.1.1.tar` & `mwrpy-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,73 @@
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1078 2023-03-27 10:23:04.000000 mwrpy-0.1.1/LICENSE
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     5826 2023-05-02 13:26:06.409820 mwrpy-0.1.1/PKG-INFO
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     5475 2023-05-02 13:01:39.000000 mwrpy-0.1.1/README.md
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/mwrpy/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      156 2023-04-06 10:43:22.000000 mwrpy-0.1.1/mwrpy/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4562 2023-04-11 13:40:37.000000 mwrpy-0.1.1/mwrpy/atmos.py
--rwxrwxr-x   0 tukiains  (1000) tukiains  (1000)     1939 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/cli.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      471 2023-03-27 10:20:23.000000 mwrpy-0.1.1/mwrpy/constants.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/mwrpy/level1/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.1/mwrpy/level1/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10903 2023-05-02 12:53:20.000000 mwrpy-0.1.1/mwrpy/level1/lev1_meta_nc.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1091 2023-03-28 08:55:18.000000 mwrpy-0.1.1/mwrpy/level1/met_quality_control.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10143 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/level1/quality_control.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    48094 2023-05-02 13:05:25.000000 mwrpy-0.1.1/mwrpy/level1/rpg_bin.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    24760 2023-04-26 11:33:16.000000 mwrpy-0.1.1/mwrpy/level1/write_lev1_nc.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/mwrpy/level2/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.1/mwrpy/level2/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    26379 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/level2/get_ret_coeff.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8776 2023-05-02 12:53:25.000000 mwrpy-0.1.1/mwrpy/level2/lev2_meta_nc.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4229 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/level2/lwp_offset.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    23559 2023-04-11 13:46:20.000000 mwrpy-0.1.1/mwrpy/level2/write_lev2_nc.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/mwrpy/plots/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       44 2023-03-27 10:20:23.000000 mwrpy-0.1.1/mwrpy/plots/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    51855 2023-04-03 06:30:29.000000 mwrpy-0.1.1/mwrpy/plots/generate_plots.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6938 2023-04-03 06:30:29.000000 mwrpy-0.1.1/mwrpy/plots/plot_meta.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8292 2023-04-03 06:30:29.000000 mwrpy-0.1.1/mwrpy/plots/plot_utils.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7674 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/process_mwrpy.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     9306 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/rpg_mwr.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    15449 2023-04-06 10:42:59.000000 mwrpy-0.1.1/mwrpy/utils.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       71 2023-05-02 13:23:07.000000 mwrpy-0.1.1/mwrpy/version.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/mwrpy.egg-info/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     5826 2023-05-02 13:26:06.000000 mwrpy-0.1.1/mwrpy.egg-info/PKG-INFO
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      756 2023-05-02 13:26:06.000000 mwrpy-0.1.1/mwrpy.egg-info/SOURCES.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        1 2023-05-02 13:26:06.000000 mwrpy-0.1.1/mwrpy.egg-info/dependency_links.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      112 2023-05-02 13:26:06.000000 mwrpy-0.1.1/mwrpy.egg-info/requires.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        6 2023-05-02 13:26:06.000000 mwrpy-0.1.1/mwrpy.egg-info/top_level.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-05-02 13:26:06.409820 mwrpy-0.1.1/setup.cfg
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      970 2023-04-06 10:43:22.000000 mwrpy-0.1.1/setup.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 13:26:06.409820 mwrpy-0.1.1/tests/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    11157 2023-04-11 13:50:11.000000 mwrpy-0.1.1/tests/test_file_reading.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1078 2023-03-27 10:23:04.000000 mwrpy-0.1.2/LICENSE
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       64 2023-05-02 13:57:04.000000 mwrpy-0.1.2/MANIFEST.in
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7016 2023-05-02 14:19:57.665817 mwrpy-0.1.2/PKG-INFO
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6665 2023-05-02 13:40:32.000000 mwrpy-0.1.2/README.md
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      156 2023-04-06 10:43:22.000000 mwrpy-0.1.2/mwrpy/__init__.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4562 2023-04-11 13:40:37.000000 mwrpy-0.1.2/mwrpy/atmos.py
+-rwxrwxr-x   0 tukiains  (1000) tukiains  (1000)     1939 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/cli.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      471 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/constants.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/level1/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/level1/__init__.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10903 2023-05-02 12:53:20.000000 mwrpy-0.1.2/mwrpy/level1/lev1_meta_nc.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1091 2023-03-28 08:55:18.000000 mwrpy-0.1.2/mwrpy/level1/met_quality_control.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10143 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level1/quality_control.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    48094 2023-05-02 13:05:25.000000 mwrpy-0.1.2/mwrpy/level1/rpg_bin.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    24760 2023-04-26 11:33:16.000000 mwrpy-0.1.2/mwrpy/level1/write_lev1_nc.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/level2/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/level2/__init__.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    26379 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level2/get_ret_coeff.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8776 2023-05-02 12:53:25.000000 mwrpy-0.1.2/mwrpy/level2/lev2_meta_nc.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4229 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level2/lwp_offset.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    23559 2023-04-11 13:46:20.000000 mwrpy-0.1.2/mwrpy/level2/write_lev2_nc.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/plots/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       44 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/plots/__init__.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    51855 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/generate_plots.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6938 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/plot_meta.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8292 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/plot_utils.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7674 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/process_mwrpy.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     9306 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/rpg_mwr.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6234 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hatpro.yaml
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/hyytiala/
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    33953 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    73995 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    73995 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    80385 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    39550 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     2965 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/config.yaml
+-rw-r--r--   0 tukiains  (1000) tukiains  (1000)       12 2023-04-03 12:47:52.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/lwp_offset_1970.csv
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/juelich/
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6284 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3100 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3100 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8692 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6256 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 tukiains  (1000) tukiains  (1000)       12 2023-03-31 08:32:30.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/lwp_offset_1970.csv
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    15449 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/utils.py
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       71 2023-05-02 13:57:53.000000 mwrpy-0.1.2/mwrpy/version.py
+drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy.egg-info/
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7016 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/PKG-INFO
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     2460 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        1 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      112 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/requires.txt
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        6 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/top_level.txt
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-05-02 14:19:57.669818 mwrpy-0.1.2/setup.cfg
+-rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      970 2023-04-06 10:43:22.000000 mwrpy-0.1.2/setup.py
```

### Comparing `mwrpy-0.1.1/LICENSE` & `mwrpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/atmos.py` & `mwrpy-0.1.2/mwrpy/atmos.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/cli.py` & `mwrpy-0.1.2/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.1.2/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level1/met_quality_control.py` & `mwrpy-0.1.2/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level1/quality_control.py` & `mwrpy-0.1.2/mwrpy/level1/quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level1/rpg_bin.py` & `mwrpy-0.1.2/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.1.2/mwrpy/level1/write_lev1_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.1.2/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.1.2/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level2/lwp_offset.py` & `mwrpy-0.1.2/mwrpy/level2/lwp_offset.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.1.2/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/plots/generate_plots.py` & `mwrpy-0.1.2/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/plots/plot_meta.py` & `mwrpy-0.1.2/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/plots/plot_utils.py` & `mwrpy-0.1.2/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/process_mwrpy.py` & `mwrpy-0.1.2/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/rpg_mwr.py` & `mwrpy-0.1.2/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/mwrpy/utils.py` & `mwrpy-0.1.2/mwrpy/utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.1/setup.py` & `mwrpy-0.1.2/setup.py`

 * *Files identical despite different names*

