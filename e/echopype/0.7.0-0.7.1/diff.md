# Comparing `tmp/echopype-0.7.0.tar.gz` & `tmp/echopype-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echopype-0.7.0.tar", last modified: Sat Mar 25 21:23:59 2023, max compression
+gzip compressed data, was "echopype-0.7.1.tar", last modified: Tue May  2 01:06:07 2023, max compression
```

## Comparing `echopype-0.7.0.tar` & `echopype-0.7.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.626459 echopype-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-25 21:23:52.000000 echopype-0.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-03-25 21:23:52.000000 echopype-0.7.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-25 21:23:52.000000 echopype-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-03-25 21:23:52.000000 echopype-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-03-25 21:23:59.626459 echopype-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-03-25 21:23:52.000000 echopype-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-25 21:23:59.000000 echopype-0.7.0/_echopype_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype/
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype/calibrate/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    21767 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/cal_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     4358 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/calibrate_azfp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/calibrate_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23806 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/calibrate_ek.py
--rw-r--r--   0 runner    (1001) docker     (122)    19532 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/ecs.py
--rw-r--r--   0 runner    (1001) docker     (122)    11490 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/ek80_complex.py
--rw-r--r--   0 runner    (1001) docker     (122)    14142 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/env_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     9283 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/env_params_old.py
--rw-r--r--   0 runner    (1001) docker     (122)     8573 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/calibrate/range.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype/clean/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4839 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/clean/noise_est.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype/commongrid/
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/commongrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/commongrid/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/commongrid/mvbs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/commongrid/nasc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype/consolidate/
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/consolidate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14480 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/consolidate/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/consolidate/split_beam_angle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/convert/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44472 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/ad2cp_fields.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    17616 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    71989 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parse_ad2cp.py
--rw-r--r--   0 runner    (1001) docker     (122)    18846 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parse_azfp.py
--rw-r--r--   0 runner    (1001) docker     (122)    20045 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parse_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parse_ek60.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parse_ek80.py
--rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parsed_to_zarr.py
--rw-r--r--   0 runner    (1001) docker     (122)     9762 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parsed_to_zarr_ek60.py
--rw-r--r--   0 runner    (1001) docker     (122)    10434 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/parsed_to_zarr_ek80.py
--rw-r--r--   0 runner    (1001) docker     (122)    24676 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/set_groups_ad2cp.py
--rw-r--r--   0 runner    (1001) docker     (122)    17707 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/set_groups_azfp.py
--rw-r--r--   0 runner    (1001) docker     (122)    19517 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/set_groups_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34655 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/set_groups_ek60.py
--rw-r--r--   0 runner    (1001) docker     (122)    53557 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/set_groups_ek80.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/convert/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/utils/ek_date_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/utils/ek_raw_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    66076 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/convert/utils/ek_raw_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    25027 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/convention/
--rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/convention/1.0.yml
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/convention/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/convention/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    22986 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/echodata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/sensor_ep_version_mapping/
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    39212 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py
--rw-r--r--   0 runner    (1001) docker     (122)     9337 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/simrad.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.614459 echopype-0.7.0/echopype/echodata/widgets/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/widgets/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     6233 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/widgets/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/static/html/icons-svg-inline.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/echodata/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/templates/echodata.html.j2
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/templates/style.html.j2
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/widgets/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)    37868 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/echodata/zarr_combine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/mask/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26401 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/mask/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/metrics/summary_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.622459 echopype-0.7.0/echopype/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/preprocess/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.626459 echopype-0.7.0/echopype/qc/
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8885 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/qc/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.626459 echopype-0.7.0/echopype/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5476 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/coding.py
--rw-r--r--   0 runner    (1001) docker     (122)    14127 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)    12259 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/prov.py
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/utils/uwa.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.626459 echopype-0.7.0/echopype/visualize/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/visualize/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/visualize/cm.py
--rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-03-25 21:23:52.000000 echopype-0.7.0/echopype/visualize/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 21:23:59.618459 echopype-0.7.0/echopype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-03-25 21:23:59.000000 echopype-0.7.0/echopype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-03-25 21:23:59.000000 echopype-0.7.0/echopype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-25 21:23:59.000000 echopype-0.7.0/echopype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-25 21:23:59.000000 echopype-0.7.0/echopype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-25 21:23:59.000000 echopype-0.7.0/echopype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-03-25 21:23:52.000000 echopype-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-25 21:23:52.000000 echopype-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-03-25 21:23:52.000000 echopype-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-03-25 21:23:59.626459 echopype-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-03-25 21:23:52.000000 echopype-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-02 01:05:58.000000 echopype-0.7.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-05-02 01:05:58.000000 echopype-0.7.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-02 01:05:58.000000 echopype-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-05-02 01:05:58.000000 echopype-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-05-02 01:06:07.258118 echopype-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-05-02 01:05:58.000000 echopype-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-02 01:06:06.000000 echopype-0.7.1/_echopype_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.250117 echopype-0.7.1/echopype/
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22091 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/cal_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4358 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/calibrate_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/calibrate_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24272 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/calibrate_ek.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19532 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10072 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/ek80_complex.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14142 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/env_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9415 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/env_params_old.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8573 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/calibrate/range.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/clean/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4839 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/clean/noise_est.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/commongrid/
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/commongrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/commongrid/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/commongrid/mvbs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/commongrid/nasc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/consolidate/
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/consolidate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14480 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/consolidate/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/consolidate/split_beam_angle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/convert/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44472 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/ad2cp_fields.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    17616 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71989 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parse_ad2cp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18800 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parse_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20045 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parse_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parse_ek60.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parse_ek80.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parsed_to_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9762 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parsed_to_zarr_ek60.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10434 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/parsed_to_zarr_ek80.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24676 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/set_groups_ad2cp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19106 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/set_groups_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19517 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/set_groups_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34655 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/set_groups_ek60.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53586 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/set_groups_ek80.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/convert/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/utils/ek_date_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/utils/ek_raw_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66078 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/convert/utils/ek_raw_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.254117 echopype-0.7.1/echopype/echodata/
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25027 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/convention/
+-rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/convention/1.0.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/convention/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/convention/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22986 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/echodata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/sensor_ep_version_mapping/
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39212 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9337 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/simrad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.250117 echopype-0.7.1/echopype/echodata/widgets/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/widgets/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     6233 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/widgets/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/static/html/icons-svg-inline.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/echodata/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/templates/echodata.html.j2
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/templates/style.html.j2
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/widgets/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37902 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/echodata/zarr_combine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/mask/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26401 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/mask/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/metrics/summary_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/preprocess/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/qc/
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8885 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/qc/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6013 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/coding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14202 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12231 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/prov.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/utils/uwa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.258118 echopype-0.7.1/echopype/visualize/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/visualize/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/visualize/cm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-05-02 01:05:58.000000 echopype-0.7.1/echopype/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:06:07.250117 echopype-0.7.1/echopype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-05-02 01:06:07.000000 echopype-0.7.1/echopype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-02 01:06:07.000000 echopype-0.7.1/echopype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 01:06:07.000000 echopype-0.7.1/echopype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-02 01:06:07.000000 echopype-0.7.1/echopype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-02 01:06:07.000000 echopype-0.7.1/echopype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-02 01:05:58.000000 echopype-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-02 01:05:58.000000 echopype-0.7.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-05-02 01:05:58.000000 echopype-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-02 01:06:07.258118 echopype-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-02 01:05:58.000000 echopype-0.7.1/setup.py
```

### Comparing `echopype-0.7.0/CITATION.cff` & `echopype-0.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/LICENSE` & `echopype-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/PKG-INFO` & `echopype-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echopype
-Version: 0.7.0
+Version: 0.7.1
 Summary: Enhancing the interoperability and scalability in analyzing ocean sonar data
 Home-page: https://github.com/OSOceanAcoustics/echopype
 Author: Wu-Jung Lee
 Author-email: leewujung@gmail.com
 Maintainer: Wu-Jung Lee
 Maintainer-email: leewujung@gmail.com
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: echopype Version: 0.7.0 Summary: Enhancing the
+Metadata-Version: 2.1 Name: echopype Version: 0.7.1 Summary: Enhancing the
 interoperability and scalability in analyzing ocean sonar data Home-page:
 https://github.com/OSOceanAcoustics/echopype Author: Wu-Jung Lee Author-email:
 leewujung@gmail.com Maintainer: Wu-Jung Lee Maintainer-email:
 leewujung@gmail.com License: Apache License, Version 2.0 Platform: OS
 Independent Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

### Comparing `echopype-0.7.0/README.md` & `echopype-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/__init__.py` & `echopype-0.7.1/echopype/__init__.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/api.py` & `echopype-0.7.1/echopype/calibrate/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/cal_params.py` & `echopype-0.7.1/echopype/calibrate/cal_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,24 @@
         "equivalent_beam_angle",
         "angle_offset_alongship",
         "angle_offset_athwartship",
         "angle_sensitivity_alongship",
         "angle_sensitivity_athwartship",
         "beamwidth_alongship",
         "beamwidth_athwartship",
-        "impedance_transmit",  # z_et
-        "impedance_receive",  # z_er
+        "impedance_transducer",  # z_et
+        "impedance_transceiver",  # z_er
         "receiver_sampling_frequency",
     ),
     "AZFP": ("EL", "DS", "TVR", "VTX", "equivalent_beam_angle", "Sv_offset"),
 }
 
 EK80_DEFAULT_PARAMS = {
-    "impedance_transmit": 75,
-    "impedance_receive": 1000,
+    "impedance_transducer": 75,
+    "impedance_transceiver": 1000,
     "receiver_sampling_frequency": {  # default full sampling frequency [Hz]
         "default": 1500000,
         "GPT": 500000,
         "SBT": 50000,
         "WBAT": 1500000,
         "WBT TUBE": 1500000,
         "WBT MINI": 1500000,
@@ -199,15 +199,15 @@
     ----
     ``da_param`` is always an xr.DataArray from the Vendor-specific group.
     It is possible that only a subset of the channels have frequency-dependent parameter values.
     The output xr.DataArray here is constructed channel-by-channel to allow for this flexibility.
 
     ``alternative`` can be one of the following:
 
-    - scalar (int or float): this is the case for impedance_transmit
+    - scalar (int or float): this is the case for impedance_transducer
     - xr.DataArray with coordinates channel, ping_time, and beam:
         this is the case for parameters angle_offset_alongship, angle_offset_athwartship,
                                         beamwidth_alongship, beamwidth_athwartship
     - xr.DataArray with coordinates channel, ping_time:
         this is the case for sa_correction and gain_correction,
         which will be direct output of get_vend_cal_params_power()
     """
@@ -304,15 +304,27 @@
         vend[param]
         .expand_dims(dim={"ping_time": idxmin["ping_time"]})  # expand dims for direct indexing
         .sortby(idxmin.channel)  # sortby in case channel sequence differs in vend and beam
     )
 
     # Select corresponding index and clean up the original nan elements
     da_param = da_param.sel(pulse_length_bin=idxmin, drop=True)
-    return da_param.where(~transmit_isnull, np.nan)  # set the nan elements back to nan
+
+    # Set the nan elements back to nan.
+    # Doing the `.where` will result in float64,
+    # which is fine since we're dealing with nan
+    da_param = da_param.where(~transmit_isnull, np.nan)
+
+    # Clean up for leftover plb variable
+    # if exists
+    plb_var = "pulse_length_bin"
+    if plb_var in da_param.coords:
+        da_param = da_param.drop(plb_var)
+
+    return da_param
 
 
 def get_cal_params_AZFP(beam: xr.DataArray, vend: xr.DataArray, user_dict: dict) -> dict:
     """
     Get cal params using user inputs or values from data file.
 
     Parameters
@@ -427,32 +439,32 @@
 
     # Only fill in params that are None
     for p, v in out_dict.items():
         if v is None:
             # Those without CW or BB complications
             if p == "sa_correction":  # pull from data file
                 out_dict[p] = get_vend_cal_params_power(beam=beam, vend=vend, param=p)
-            elif p == "impedance_receive":  # from data file or default dict
-                out_dict[p] = default_params[p] if p not in vend else vend["impedance_receive"]
+            elif p == "impedance_transceiver":  # from data file or default dict
+                out_dict[p] = default_params[p] if p not in vend else vend["impedance_transceiver"]
             elif p == "receiver_sampling_frequency":  # from data file or default_params
                 out_dict[p] = _get_fs()
             else:
-                # CW: params do not require interpolation, except for impedance_transmit
+                # CW: params do not require interpolation, except for impedance_transducer
                 if waveform_mode == "CW":
                     if p in PARAM_BEAM_NAME_MAP.keys():
                         p_beam = PARAM_BEAM_NAME_MAP[p]
                         # pull from data file, these should always exist
                         if "beam" in beam[p_beam].coords:
                             out_dict[p] = beam[p_beam].isel(beam=0).drop("beam")
                         else:
                             out_dict[p] = beam[p_beam]
                     elif p == "gain_correction":
                         # pull from data file narrowband table
                         out_dict[p] = get_vend_cal_params_power(beam=beam, vend=vend, param=p)
-                    elif p == "impedance_transmit":
+                    elif p == "impedance_transducer":
                         # assemble each channel from data file or default dict
                         out_dict[p] = _get_interp_da(
                             da_param=None if p not in vend else vend[p],
                             freq_center=freq_center,
                             alternative=default_params[p],  # pull from default dict
                         )
                     else:
@@ -493,15 +505,15 @@
                         out_dict[p] = _get_interp_da(
                             da_param=None
                             if "gain" not in vend
                             else vend["gain"],  # freq-dep values
                             freq_center=freq_center,
                             alternative=get_vend_cal_params_power(beam=beam, vend=vend, param=p),
                         )
-                    elif p == "impedance_transmit":
+                    elif p == "impedance_transducer":
                         out_dict[p] = _get_interp_da(
                             da_param=None if p not in vend else vend[p],
                             freq_center=freq_center,
                             alternative=default_params[p],  # pull from default dict
                         )
                     else:
                         raise ValueError(f"{p} not in the defined set of calibration parameters.")
```

### Comparing `echopype-0.7.0/echopype/calibrate/calibrate_azfp.py` & `echopype-0.7.1/echopype/calibrate/calibrate_azfp.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/calibrate_base.py` & `echopype-0.7.1/echopype/calibrate/calibrate_base.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/calibrate_ek.py` & `echopype-0.7.1/echopype/calibrate/calibrate_ek.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
     def compute_TS(self, **kwargs):
         return self._cal_power_samples(cal_type="TS")
 
 
 class CalibrateEK80(CalibrateEK):
     # Default EK80 params: these parameters are only recorded in later versions of EK80 software
     EK80_params = {}
-    EK80_params["z_et"] = 75  # transmit impedance
-    EK80_params["z_er"] = 1000  # receive impedance
+    EK80_params["z_et"] = 75  # transducer impedance
+    EK80_params["z_er"] = 1000  # transceiver impedance
     EK80_params["fs"] = {  # default full sampling frequency [Hz]
         "default": 1500000,
         "GPT": 500000,
         "SBT": 50000,
         "WBAT": 1500000,
         "WBT TUBE": 1500000,
         "WBT MINI": 1500000,
@@ -391,26 +391,30 @@
             # Do nothing if ds_cal_BB is None
             return cal_params_dict
 
     def _get_power_from_complex(
         self,
         beam: xr.Dataset,
         chirp: Dict,
-        z_et,
-        z_er,
+        z_et: float,
+        z_er: float,
     ) -> xr.DataArray:
         """
         Get power from complex samples.
 
         Parameters
         ----------
         beam : xr.Dataset
             EchoData["Sonar/Beam_group1"] with selected channel subset
         chirp : dict
             a dictionary containing transmit chirp for BB channels
+        z_et : float
+            impedance of transducer [ohm]
+        z_er : float
+            impedance of transceiver [ohm]
 
         Returns
         -------
         prx : xr.DataArray
             Power computed from complex samples
         """
 
@@ -437,15 +441,18 @@
 
         return prx
 
     def _get_B_theta_phi_m(self):
         """
         Get transceiver gain compensation for BB mode.
 
-        ref: https://github.com/CI-CMG/pyEcholab/blob/RHT-EK80-Svf/echolab2/instruments/EK80.py#L4263-L4274  # noqa
+        Source: https://github.com/CRIMAC-WP4-Machine-learning/CRIMAC-Raw-To-Svf-TSf/blob/abd01f9c271bb2dbe558c80893dbd7eb0d06fe38/Core/EK80DataContainer.py#L261-L273  # noqa
+        From conversation with Lars Andersen, this correction is based on a longstanding
+        empirical formula used for fitting beampattern during calibration, based on
+        physically meaningful parameters such as the angle offset and beamwidth.
         """
         fac_along = (
             np.abs(-self.cal_params["angle_offset_alongship"])
             / (self.cal_params["beamwidth_alongship"] / 2)
         ) ** 2
         fac_athwart = (
             np.abs(-self.cal_params["angle_offset_athwartship"])
@@ -473,20 +480,20 @@
         beam = self.echodata[self.ed_beam_group].sel(channel=self.chan_sel)
         vend = self.echodata["Vendor_specific"].sel(channel=self.chan_sel)
 
         # Get transmit signal
         tx_coeff = get_filter_coeff(vend)
         fs = self.cal_params["receiver_sampling_frequency"]
 
-        # Switch to use Anderson implementation for transmit chirp starting v0.6.4
+        # Switch to use Andersen implementation for transmit chirp starting v0.6.4
         tx, tx_time = get_transmit_signal(beam, tx_coeff, self.waveform_mode, fs)
 
         # Params to clarity in use below
-        z_er = self.cal_params["impedance_receive"]
-        z_et = self.cal_params["impedance_transmit"]
+        z_er = self.cal_params["impedance_transceiver"]
+        z_et = self.cal_params["impedance_transducer"]
         gain = self.cal_params["gain_correction"]
 
         # Transceiver gain compensation for BB mode
         if self.waveform_mode == "BB":
             gain = gain - self._get_B_theta_phi_m()
 
         absorption = self.env_params["sound_absorption"]
```

### Comparing `echopype-0.7.0/echopype/calibrate/ecs.py` & `echopype-0.7.1/echopype/calibrate/ecs.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/ek80_complex.py` & `echopype-0.7.1/echopype/calibrate/ek80_complex.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,76 +6,49 @@
 from scipy import signal
 
 
 def tapered_chirp(
     fs,
     transmit_duration_nominal,
     slope,
-    transmit_power,
-    implementation="Anderson",
-    z_et=None,
     frequency_nominal=None,
     frequency_start=None,
     frequency_end=None,
 ):
-    """Create a baseline chirp template."""
+    """
+    Create the chirp replica following implementation from Lars Anderson.
+
+    Ref source: https://github.com/CRIMAC-WP4-Machine-learning/CRIMAC-Raw-To-Svf-TSf/blob/main/Core/Calculation.py  # noqa
+    """
     if frequency_start is None and frequency_end is None:  # CW waveform
         frequency_start = frequency_nominal
         frequency_end = frequency_nominal
 
-    if implementation == "Macaulay":
-        # z_et is required for Macaulay implementation
-        if z_et is None:
-            raise ValueError("z_et is needed for Macaulay implementation of transmit chirp!")
-
-        t = np.arange(0, transmit_duration_nominal, 1 / fs)
-        nwtx = int(2 * np.floor(slope * t.size))  # length of tapering window
-        wtx_tmp = np.hanning(nwtx)  # hanning window
-        nwtxh = int(np.round(nwtx / 2))  # half length of the hanning window
-        wtx = np.concatenate(
-            [wtx_tmp[0:nwtxh], np.ones((t.size - nwtx)), wtx_tmp[nwtxh:]]
-        )  # assemble full tapering window
-        chirp_fac = (
-            (frequency_end - frequency_start) / transmit_duration_nominal
-        ) * t / 2 + frequency_start
-        y_tmp = (
-            np.sqrt((transmit_power / 4) * (2 * z_et))  # amplitude
-            * np.cos(2 * np.pi * chirp_fac * t)  # chirp
-            * wtx  # tapering
-        )  # taper and scale linear chirp
-        return y_tmp / np.max(np.abs(y_tmp)), t  # amplitude needs to be normalized
-
-    elif implementation == "Anderson":
-        # Substitute to keep original form in Anderson implementation
-        # source: https://github.com/CRIMAC-WP4-Machine-learning/CRIMAC-Raw-To-Svf-TSf/blob/main/Core/Calculation.py  # noqa
-        tau = transmit_duration_nominal
-        f0 = frequency_start
-        f1 = frequency_end
-
-        nsamples = int(np.floor(tau * fs))
-        t = np.linspace(0, nsamples - 1, num=nsamples) * 1 / fs
-        a = np.pi * (f1 - f0) / tau
-        b = 2 * np.pi * f0
-        y = np.cos(a * t * t + b * t)
-        L = int(np.round(tau * fs * slope * 2.0))  # Length of hanning window
-        w = 0.5 * (1.0 - np.cos(2.0 * np.pi * np.arange(0, L, 1) / (L - 1)))
-        N = len(y)
-        w1 = w[0 : int(len(w) / 2)]
-        w2 = w[int(len(w) / 2) : -1]
-        i0 = 0
-        i1 = len(w1)
-        i2 = N - len(w2)
-        i3 = N
-        y[i0:i1] = y[i0:i1] * w1
-        y[i2:i3] = y[i2:i3] * w2
+    tau = transmit_duration_nominal
+    f0 = frequency_start
+    f1 = frequency_end
+
+    nsamples = int(np.floor(tau * fs))
+    t = np.linspace(0, nsamples - 1, num=nsamples) * 1 / fs
+    a = np.pi * (f1 - f0) / tau
+    b = 2 * np.pi * f0
+    y = np.cos(a * t * t + b * t)
+    L = int(np.round(tau * fs * slope * 2.0))  # Length of hanning window
+    w = 0.5 * (1.0 - np.cos(2.0 * np.pi * np.arange(0, L, 1) / (L - 1)))
+    N = len(y)
+    w1 = w[0 : int(len(w) / 2)]
+    w2 = w[int(len(w) / 2) : -1]
+    i0 = 0
+    i1 = len(w1)
+    i2 = N - len(w2)
+    i3 = N
+    y[i0:i1] = y[i0:i1] * w1
+    y[i2:i3] = y[i2:i3] * w2
 
-        return y / np.max(y), t  # amplitude needs to be normalized
-
-    else:
-        raise ValueError("Input implementation type not recognized!")
+    return y / np.max(y), t  # amplitude needs to be normalized
 
 
 def filter_decimate_chirp(coeff_ch: Dict, y_ch: np.array, fs: float):
     """Filter and decimate the transmit replica for one channel.
 
     Parameters
     ----------
@@ -249,23 +222,21 @@
     y_time_all = {}
     for ch in beam["channel"].values:
         # TODO: expand to deal with the case with varying tx param across ping_time
         if waveform_mode == "BB":
             tx_param_names = [
                 "transmit_duration_nominal",
                 "slope",
-                "transmit_power",
                 "frequency_start",
                 "frequency_end",
             ]
         else:
             tx_param_names = [
                 "transmit_duration_nominal",
                 "slope",
-                "transmit_power",
                 "frequency_nominal",
             ]
         tx_params = {}
         for p in tx_param_names:
             tx_params[p] = np.unique(beam[p].sel(channel=ch))
             if tx_params[p].size != 1:
                 raise TypeError("File contains changing %s!" % p)
```

### Comparing `echopype-0.7.0/echopype/calibrate/env_params.py` & `echopype-0.7.1/echopype/calibrate/env_params.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/calibrate/env_params_old.py` & `echopype-0.7.1/echopype/calibrate/env_params_old.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,16 +101,18 @@
                 )
 
         env_params = self.env_params
 
         if self.data_kind == "mobile":
             if np.isnan(echodata["Platform"]["time1"]).all():
                 raise ValueError("cannot perform mobile interpolation without time1")
+            # only grab needed variables for the interpolation
+            platform_data = echodata["Platform"][["latitude", "longitude"]]
             # compute_range needs indexing by ping_time
-            interp_plat = echodata["Platform"].interp(
+            interp_plat = platform_data.interp(
                 {"time1": echodata["Sonar/Beam_group1"]["ping_time"]}
             )
 
             result = {}
             for var, values in env_params.data_vars.items():
                 points = np.column_stack(
                     (env_params["latitude"].data, env_params["longitude"].data)
```

### Comparing `echopype-0.7.0/echopype/calibrate/range.py` & `echopype-0.7.1/echopype/calibrate/range.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/clean/api.py` & `echopype-0.7.1/echopype/clean/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/clean/noise_est.py` & `echopype-0.7.1/echopype/clean/noise_est.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/commongrid/api.py` & `echopype-0.7.1/echopype/commongrid/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/commongrid/mvbs.py` & `echopype-0.7.1/echopype/commongrid/mvbs.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/commongrid/nasc.py` & `echopype-0.7.1/echopype/commongrid/nasc.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/consolidate/api.py` & `echopype-0.7.1/echopype/consolidate/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/consolidate/split_beam_angle.py` & `echopype-0.7.1/echopype/consolidate/split_beam_angle.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/__init__.py` & `echopype-0.7.1/echopype/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/ad2cp_fields.yaml` & `echopype-0.7.1/echopype/convert/ad2cp_fields.yaml`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/api.py` & `echopype-0.7.1/echopype/convert/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parse_ad2cp.py` & `echopype-0.7.1/echopype/convert/parse_ad2cp.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parse_azfp.py` & `echopype-0.7.1/echopype/convert/parse_azfp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,119 @@
-import math
 import os
 import xml.dom.minidom
 from collections import defaultdict
 from datetime import datetime as dt
 from struct import unpack
 
 import fsspec
 import numpy as np
 
 from ..utils.log import _init_logger
 from .parse_base import ParseBase
 
 FILENAME_DATETIME_AZFP = "\\w+.01A"
+XML_INT_PARAMS = {
+    "NumFreq": "num_freq",
+    "SerialNumber": "serial_number",
+    "BurstInterval": "burst_interval",
+    "PingsPerBurst": "pings_per_burst",
+    "AverageBurstPings": "average_burst_pings",
+    "SensorsFlag": "sensors_flag",
+}
+XML_FLOAT_PARAMS = [
+    # Temperature coeffs
+    "ka",
+    "kb",
+    "kc",
+    "A",
+    "B",
+    "C",
+    # Tilt coeffs
+    "X_a",
+    "X_b",
+    "X_c",
+    "X_d",
+    "Y_a",
+    "Y_b",
+    "Y_c",
+    "Y_d",
+]
+XML_FREQ_PARAMS = {
+    "RangeSamples": "range_samples",
+    "RangeAveragingSamples": "range_averaging_samples",
+    "DigRate": "dig_rate",
+    "LockOutIndex": "lockout_index",
+    "Gain": "gain",
+    "PulseLen": "pulse_length",
+    "DS": "DS",
+    "EL": "EL",
+    "TVR": "TVR",
+    "VTX0": "VTX",
+    "BP": "BP",
+}
+HEADER_FIELDS = (
+    ("profile_flag", "u2"),
+    ("profile_number", "u2"),
+    ("serial_number", "u2"),
+    ("ping_status", "u2"),
+    ("burst_int", "u4"),
+    ("year", "u2"),  # Year
+    ("month", "u2"),  # Month
+    ("day", "u2"),  # Day
+    ("hour", "u2"),  # Hour
+    ("minute", "u2"),  # Minute
+    ("second", "u2"),  # Second
+    ("hundredths", "u2"),  # Hundredths of a second
+    ("dig_rate", "u2", 4),  # Digitalization rate for each channel
+    ("lockout_index", "u2", 4),  # Lockout index for each channel
+    ("num_bins", "u2", 4),  # Number of bins for each channel
+    (
+        "range_samples_per_bin",
+        "u2",
+        4,
+    ),  # Range samples per bin for each channel
+    ("ping_per_profile", "u2"),  # Number of pings per profile
+    ("avg_pings", "u2"),  # Flag indicating whether the pings average in time
+    ("num_acq_pings", "u2"),  # Pings acquired in the burst
+    ("ping_period", "u2"),  # Ping period in seconds
+    ("first_ping", "u2"),
+    ("last_ping", "u2"),
+    (
+        "data_type",
+        "u1",
+        4,
+    ),  # Datatype for each channel 1=Avg unpacked_data (5bytes), 0=raw (2bytes)
+    ("data_error", "u2"),  # Error number is an error occurred
+    ("phase", "u1"),  # Phase number used to acquire this profile
+    ("overrun", "u1"),  # 1 if an overrun occurred
+    ("num_chan", "u1"),  # 1, 2, 3, or 4
+    ("gain", "u1", 4),  # gain channel 1-4
+    ("spare_chan", "u1"),  # spare channel
+    ("pulse_length", "u2", 4),  # Pulse length chan 1-4 uS
+    ("board_num", "u2", 4),  # The board the data came from channel 1-4
+    ("frequency", "u2", 4),  # frequency for channel 1-4 in kHz
+    (
+        "sensor_flag",
+        "u2",
+    ),  # Flag indicating if pressure sensor or temperature sensor is available
+    ("ancillary", "u2", 5),  # Tilt-X, Y, Battery, Pressure, Temperature
+    ("ad", "u2", 2),  # AD channel 6 and 7
+)
 
 logger = _init_logger(__name__)
 
 
 class ParseAZFP(ParseBase):
     """Class for converting data from ASL Environmental Sciences AZFP echosounder."""
 
+    # Instrument specific constants
+    HEADER_SIZE = 124
+    HEADER_FORMAT = ">HHHHIHHHHHHHHHHHHHHHHHHHHHHHHHHHHHBBBBHBBBBBBBBHHHHHHHHHHHHHHHHHHHH"
+    FILE_TYPE = 64770
+
     def __init__(self, file, params, storage_options={}, dgram_zarr_vars={}):
         super().__init__(file, storage_options)
         # Parent class attributes
         #  regex pattern used to grab datetime embedded in filename
         self.timestamp_pattern = FILENAME_DATETIME_AZFP
         self.xml_path = params
 
@@ -36,248 +127,192 @@
         """Parses the AZFP  XML file.
         """
 
         def get_value_by_tag_name(tag_name, element=0):
             """Returns the value in an XML tag given the tag name and the number of occurrences."""
             return px.getElementsByTagName(tag_name)[element].childNodes[0].data
 
-        # TODO: consider writing a ParamAZFPxml class for storing parameters
-
         xmlmap = fsspec.get_mapper(self.xml_path, **self.storage_options)
         px = xml.dom.minidom.parse(xmlmap.fs.open(xmlmap.root))
 
-        int_params = {
-            "NumFreq": "num_freq",
-            "SerialNumber": "serial_number",
-            "BurstInterval": "burst_interval",
-            "PingsPerBurst": "pings_per_burst",
-            "AverageBurstPings": "average_burst_pings",
-            "SensorsFlag": "sensors_flag",
-        }
-        float_params = [
-            "ka",
-            "kb",
-            "kc",
-            "A",
-            "B",
-            "C",  # Temperature coeffs
-            "X_a",
-            "X_b",
-            "X_c",
-            "X_d",
-            "Y_a",
-            "Y_b",
-            "Y_c",
-            "Y_d",
-        ]  # Tilt coeffs]
-        freq_params = {
-            "RangeSamples": "range_samples",
-            "RangeAveragingSamples": "range_averaging_samples",
-            "DigRate": "dig_rate",
-            "LockOutIndex": "lockout_index",
-            "Gain": "gain",
-            "PulseLen": "pulse_length",
-            "DS": "DS",
-            "EL": "EL",
-            "TVR": "TVR",
-            "VTX0": "VTX",
-            "BP": "BP",
-        }
-
         # Retrieve integer parameters from the xml file
-        for old_name, new_name in int_params.items():
+        for old_name, new_name in XML_INT_PARAMS.items():
             self.parameters[new_name] = int(get_value_by_tag_name(old_name))
         # Retrieve floating point parameters from the xml file
-        for param in float_params:
+        for param in XML_FLOAT_PARAMS:
             self.parameters[param] = float(get_value_by_tag_name(param))
         # Retrieve frequency dependent parameters from the xml file
-        for old_name, new_name in freq_params.items():
+        for old_name, new_name in XML_FREQ_PARAMS.items():
             self.parameters[new_name] = [
                 float(get_value_by_tag_name(old_name, ch))
                 for ch in range(self.parameters["num_freq"])
             ]
 
-    def parse_raw(self):
-        """Parse raw data file from AZFP echosounder.
+    def _compute_temperature(self, ping_num, is_valid):
+        """
+        Compute temperature in celsius.
 
         Parameters
         ----------
-        raw : list
-            raw filename
+        ping_num
+            ping number
+        is_valid
+            whether the associated parameters have valid values
         """
+        if not is_valid:
+            return np.nan
+
+        counts = self.unpacked_data["ancillary"][ping_num][4]
+        v_in = 2.5 * (counts / 65535)
+        R = (self.parameters["ka"] + self.parameters["kb"] * v_in) / (self.parameters["kc"] - v_in)
+
+        # fmt: off
+        T = 1 / (
+            self.parameters["A"]
+            + self.parameters["B"] * (np.log(R))
+            + self.parameters["C"] * (np.log(R) ** 3)
+        ) - 273
+        # fmt: on
+        return T
 
-        # Start of computation subfunctions
-        def compute_temp(counts):
-            """
-            Returns the temperature in celsius given from xml data
-            and the counts from ancillary
-            """
-            v_in = 2.5 * (counts / 65535)
-            R = (self.parameters["ka"] + self.parameters["kb"] * v_in) / (
-                self.parameters["kc"] - v_in
-            )
-            # fmt: off
-            T = 1 / (
-                self.parameters["A"]
-                + self.parameters["B"] * (math.log(R))
-                + self.parameters["C"] * (math.log(R) ** 3)
-            ) - 273
-            # fmt: on
-            return T
+    def _compute_tilt(self, ping_num, xy, is_valid):
+        """
+        Compute instrument tilt.
 
-        def compute_tilt(N, a, b, c, d):
+        Parameters
+        ----------
+        ping_num
+            ping number
+        xy
+            either "X" or "Y"
+        is_valid
+            whether the associated parameters have valid values
+        """
+        if not is_valid:
+            return np.nan
+        else:
+            idx = 0 if xy == "X" else 1
+            N = self.unpacked_data["ancillary"][ping_num][idx]
+            a = self.parameters[f"{xy}_a"]
+            b = self.parameters[f"{xy}_b"]
+            c = self.parameters[f"{xy}_c"]
+            d = self.parameters[f"{xy}_d"]
             return a + b * N + c * N**2 + d * N**3
 
-        def compute_battery(N):
-            USL5_BAT_CONSTANT = (2.5 / 65536.0) * (86.6 + 475.0) / 86.6
-            return N * USL5_BAT_CONSTANT
-
-        # Instrument specific constants
-        HEADER_SIZE = 124
-        HEADER_FORMAT = ">HHHHIHHHHHHHHHHHHHHHHHHHHHHHHHHHHHBBBBHBBBBBBBBHHHHHHHHHHHHHHHHHHHH"
+    def _compute_battery(self, ping_num, battery_type):
+        """
+        Compute battery voltage.
+
+        Parameters
+        ----------
+        ping_num
+            ping number
+        type
+            either "main" or "tx"
+        """
+        USL5_BAT_CONSTANT = (2.5 / 65536.0) * (86.6 + 475.0) / 86.6
+
+        if battery_type == "main":
+            N = self.unpacked_data["ancillary"][ping_num][2]
+        elif battery_type == "tx":
+            N = self.unpacked_data["ad"][ping_num][0]
+
+        return N * USL5_BAT_CONSTANT
+
+    def parse_raw(self):
+        """
+        Parse raw data file from AZFP echosounder.
+        """
 
         # Read xml file into dict
         self.load_AZFP_xml()
         fmap = fsspec.get_mapper(self.source_file, **self.storage_options)
 
+        # Set flags for presence of valid parameters for temperature and tilt
+        def _test_valid_params(params):
+            if all([np.isclose(self.parameters[p], 0) for p in params]):
+                return False
+            else:
+                return True
+
+        temperature_is_valid = _test_valid_params(["ka", "kb", "kc"])
+        tilt_x_is_valid = _test_valid_params(["X_a", "X_b", "X_c"])
+        tilt_y_is_valid = _test_valid_params(["Y_a", "Y_b", "Y_c"])
+
         with fmap.fs.open(fmap.root, "rb") as file:
             ping_num = 0
             eof = False
             while not eof:
-                header_chunk = file.read(HEADER_SIZE)
+                header_chunk = file.read(self.HEADER_SIZE)
                 if header_chunk:
-                    header_unpacked = unpack(HEADER_FORMAT, header_chunk)
+                    header_unpacked = unpack(self.HEADER_FORMAT, header_chunk)
 
                     # Reading will stop if the file contains an unexpected flag
                     if self._split_header(file, header_unpacked):
                         # Appends the actual 'data values' to unpacked_data
                         self._add_counts(file, ping_num)
                         if ping_num == 0:
                             # Display information about the file that was loaded in
                             self._print_status()
                         # Compute temperature from unpacked_data[ii]['ancillary][4]
                         self.unpacked_data["temperature"].append(
-                            compute_temp(self.unpacked_data["ancillary"][ping_num][4])
+                            self._compute_temperature(ping_num, temperature_is_valid)
                         )
                         # compute x tilt from unpacked_data[ii]['ancillary][0]
                         self.unpacked_data["tilt_x"].append(
-                            compute_tilt(
-                                self.unpacked_data["ancillary"][ping_num][0],
-                                self.parameters["X_a"],
-                                self.parameters["X_b"],
-                                self.parameters["X_c"],
-                                self.parameters["X_d"],
-                            )
+                            self._compute_tilt(ping_num, "X", tilt_x_is_valid)
                         )
                         # Compute y tilt from unpacked_data[ii]['ancillary][1]
                         self.unpacked_data["tilt_y"].append(
-                            compute_tilt(
-                                self.unpacked_data["ancillary"][ping_num][1],
-                                self.parameters["Y_a"],
-                                self.parameters["Y_b"],
-                                self.parameters["Y_c"],
-                                self.parameters["Y_d"],
-                            )
+                            self._compute_tilt(ping_num, "Y", tilt_y_is_valid)
                         )
                         # Compute cos tilt magnitude from tilt x and y values
                         self.unpacked_data["cos_tilt_mag"].append(
-                            math.cos(
+                            np.cos(
                                 (
-                                    math.sqrt(
+                                    np.sqrt(
                                         self.unpacked_data["tilt_x"][ping_num] ** 2
                                         + self.unpacked_data["tilt_y"][ping_num] ** 2
                                     )
                                 )
-                                * math.pi
+                                * np.pi
                                 / 180
                             )
                         )
                         # Calculate voltage of main battery pack
                         self.unpacked_data["battery_main"].append(
-                            compute_battery(self.unpacked_data["ancillary"][ping_num][2])
+                            self._compute_battery(ping_num, battery_type="main")
                         )
                         # If there is a Tx battery pack
                         self.unpacked_data["battery_tx"].append(
-                            compute_battery(self.unpacked_data["ad"][ping_num][0])
+                            self._compute_battery(ping_num, battery_type="tx")
                         )
                     else:
                         break
                 else:
                     # End of file
                     eof = True
                 ping_num += 1
         self._check_uniqueness()
         self._get_ping_time()
+
         # Explicitly cast frequency to a float in accordance with the SONAR-netCDF4 convention
         self.unpacked_data["frequency"] = self.unpacked_data["frequency"].astype(np.float64)
 
         # cast unpacked_data values to np arrays, so they are easier to reference
         for key, val in self.unpacked_data.items():
             # if it is not a nested list, make the value into a ndarray
             if isinstance(val, list) and (not isinstance(val[0], list)):
                 self.unpacked_data[key] = np.asarray(val)
 
         # cast all list parameter values to np array, so they are easier to reference
         for key, val in self.parameters.items():
             if isinstance(val, list):
                 self.parameters[key] = np.asarray(val)
 
-    @staticmethod
-    def _get_fields():
-        """Returns the fields contained in each header of the raw file."""
-        _fields = (
-            ("profile_flag", "u2"),
-            ("profile_number", "u2"),
-            ("serial_number", "u2"),
-            ("ping_status", "u2"),
-            ("burst_int", "u4"),
-            ("year", "u2"),  # Year
-            ("month", "u2"),  # Month
-            ("day", "u2"),  # Day
-            ("hour", "u2"),  # Hour
-            ("minute", "u2"),  # Minute
-            ("second", "u2"),  # Second
-            ("hundredths", "u2"),  # Hundredths of a second
-            ("dig_rate", "u2", 4),  # Digitalization rate for each channel
-            ("lockout_index", "u2", 4),  # Lockout index for each channel
-            ("num_bins", "u2", 4),  # Number of bins for each channel
-            (
-                "range_samples_per_bin",
-                "u2",
-                4,
-            ),  # Range samples per bin for each channel
-            ("ping_per_profile", "u2"),  # Number of pings per profile
-            ("avg_pings", "u2"),  # Flag indicating whether the pings average in time
-            ("num_acq_pings", "u2"),  # Pings acquired in the burst
-            ("ping_period", "u2"),  # Ping period in seconds
-            ("first_ping", "u2"),
-            ("last_ping", "u2"),
-            (
-                "data_type",
-                "u1",
-                4,
-            ),  # Datatype for each channel 1=Avg unpacked_data (5bytes), 0=raw (2bytes)
-            ("data_error", "u2"),  # Error number is an error occurred
-            ("phase", "u1"),  # Phase number used to acquire this profile
-            ("overrun", "u1"),  # 1 if an overrun occurred
-            ("num_chan", "u1"),  # 1, 2, 3, or 4
-            ("gain", "u1", 4),  # gain channel 1-4
-            ("spare_chan", "u1"),  # spare channel
-            ("pulse_length", "u2", 4),  # Pulse length chan 1-4 uS
-            ("board_num", "u2", 4),  # The board the data came from channel 1-4
-            ("frequency", "u2", 4),  # frequency for channel 1-4 in kHz
-            (
-                "sensor_flag",
-                "u2",
-            ),  # Flag indicating if pressure sensor or temperature sensor is available
-            ("ancillary", "u2", 5),  # Tilt-X, Y, Battery, Pressure, Temperature
-            ("ad", "u2", 2),  # AD channel 6 and 7
-        )
-        return _fields
-
     def _print_status(self):
         """Prints message to console giving information about the raw file being parsed."""
         filename = os.path.basename(self.source_file)
         timestamp = dt(
             self.unpacked_data["year"][0],
             self.unpacked_data["month"][0],
             self.unpacked_data["day"][0],
@@ -300,18 +335,16 @@
         header_unpacked
             output of struct unpack of raw file
 
         Returns
         -------
             True or False depending on whether the unpacking was successful
         """
-        FILE_TYPE = 64770  # Instrument specific constant
-        fields = self._get_fields()
         if (
-            header_unpacked[0] != FILE_TYPE
+            header_unpacked[0] != self.FILE_TYPE
         ):  # first field should match hard-coded FILE_TYPE from manufacturer
             check_eof = raw.read(1)
             if check_eof:
                 logger.error("Unknown file type")
                 return False
         header_byte_cnt = 0
 
@@ -326,15 +359,15 @@
             "range_samples_per_bin",  # fields with num_freq data
             "data_type",
             "gain",
             "pulse_length",
             "board_num",
             "frequency",
         )
-        for field in fields:
+        for field in HEADER_FIELDS:
             if field[0] in field_w_freq:  # fields with num_freq data
                 self.unpacked_data[field[0]].append(
                     header_unpacked[header_byte_cnt : header_byte_cnt + self.parameters["num_freq"]]
                 )
                 header_byte_cnt += firmware_freq_len
             elif len(field) == 3:  # other longer fields ('ancillary' and 'ad')
                 self.unpacked_data[field[0]].append(
```

### Comparing `echopype-0.7.0/echopype/convert/parse_base.py` & `echopype-0.7.1/echopype/convert/parse_base.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parse_ek60.py` & `echopype-0.7.1/echopype/convert/parse_ek60.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parse_ek80.py` & `echopype-0.7.1/echopype/convert/parse_ek80.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parsed_to_zarr.py` & `echopype-0.7.1/echopype/convert/parsed_to_zarr.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parsed_to_zarr_ek60.py` & `echopype-0.7.1/echopype/convert/parsed_to_zarr_ek60.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/parsed_to_zarr_ek80.py` & `echopype-0.7.1/echopype/convert/parsed_to_zarr_ek80.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/set_groups_ad2cp.py` & `echopype-0.7.1/echopype/convert/set_groups_ad2cp.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/set_groups_azfp.py` & `echopype-0.7.1/echopype/convert/set_groups_azfp.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,29 +87,33 @@
         # @ngkavin: what modification?
         ping_time = self.parser_obj.ping_time
         ds = xr.Dataset(
             {
                 "temperature": (
                     ["time1"],
                     self.parser_obj.unpacked_data["temperature"],
+                    {
+                        "long_name": "Water temperature",
+                        "standard_name": "sea_water_temperature",
+                        "units": "deg_C",
+                    },
                 )
             },
             coords={
                 "time1": (
                     ["time1"],
                     ping_time,
                     {
                         "axis": "T",
                         "long_name": "Timestamp of each ping",
                         "standard_name": "time",
                         "comment": "Time coordinate corresponding to environmental variables.",
                     },
                 )
             },
-            attrs={"long_name": "Water temperature", "units": "C"},
         )
 
         return set_time_encodings(ds)
 
     def set_sonar(self) -> xr.Dataset:
         """Set the Sonar group."""
 
@@ -121,14 +125,15 @@
 
         # Assemble sonar group global attribute dictionary
         sonar_attr_dict = {
             "sonar_manufacturer": "ASL Environmental Sciences",
             "sonar_model": self.sonar_model,
             "sonar_serial_number": int(self.parser_obj.unpacked_data["serial_number"]),
             "sonar_software_name": "AZFP",
+            # TODO: software version is hardwired. Read it from the XML file's AZFP_Version node
             "sonar_software_version": "1.4",
             "sonar_type": "echosounder",
         }
         ds = ds.assign_attrs(sonar_attr_dict)
 
         return ds
 
@@ -140,16 +145,30 @@
             "platform_code_ICES": self.ui_param["platform_code_ICES"],
         }
         unpacked_data = self.parser_obj.unpacked_data
         time2 = self.parser_obj.ping_time
 
         ds = xr.Dataset(
             {
-                "tilt_x": (["time2"], unpacked_data["tilt_x"]),
-                "tilt_y": (["time2"], unpacked_data["tilt_y"]),
+                "tilt_x": (
+                    ["time2"],
+                    unpacked_data["tilt_x"],
+                    {
+                        "long_name": "Tilt X",
+                        "units": "degree",
+                    },
+                ),
+                "tilt_y": (
+                    ["time2"],
+                    unpacked_data["tilt_y"],
+                    {
+                        "long_name": "Tilt Y",
+                        "units": "degree",
+                    },
+                ),
                 **{
                     var: ([], np.nan, self._varattrs["platform_var_default"][var])
                     for var in [
                         "MRU_offset_x",
                         "MRU_offset_y",
                         "MRU_offset_z",
                         "MRU_rotation_x",
@@ -235,18 +254,42 @@
                     {
                         "units": "Hz",
                         "long_name": "Transducer frequency",
                         "valid_min": 0.0,
                         "standard_name": "sound_frequency",
                     },
                 ),
-                "backscatter_r": (["channel", "ping_time", "range_sample"], N),
-                "equivalent_beam_angle": (["channel"], parameters["BP"][self.freq_ind_sorted]),
-                "gain_correction": (["channel"], unpacked_data["gain"][self.freq_ind_sorted]),
-                "sample_interval": (["channel"], sample_int, {"units": "s"}),
+                "backscatter_r": (
+                    ["channel", "ping_time", "range_sample"],
+                    N,
+                    {"long_name": "Backscatter power", "units": "dB"},
+                ),
+                "equivalent_beam_angle": (
+                    ["channel"],
+                    parameters["BP"][self.freq_ind_sorted],
+                    {
+                        "long_name": "Equivalent beam angle",
+                        "units": "sr",
+                        "valid_range": (0.0, 4 * np.pi),
+                    },
+                ),
+                "gain_correction": (
+                    ["channel"],
+                    unpacked_data["gain"][self.freq_ind_sorted],
+                    {"long_name": "Gain correction", "units": "dB"},
+                ),
+                "sample_interval": (
+                    ["channel"],
+                    sample_int,
+                    {
+                        "long_name": "Interval between recorded raw data samples",
+                        "units": "s",
+                        "valid_min": 0.0,
+                    },
+                ),
                 "transmit_duration_nominal": (
                     ["channel"],
                     tdn,
                     {
                         "long_name": "Nominal bandwidth of transmitted pulse",
                         "units": "s",
                         "valid_min": 0.0,
```

### Comparing `echopype-0.7.0/echopype/convert/set_groups_base.py` & `echopype-0.7.1/echopype/convert/set_groups_base.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/set_groups_ek60.py` & `echopype-0.7.1/echopype/convert/set_groups_ek60.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/set_groups_ek80.py` & `echopype-0.7.1/echopype/convert/set_groups_ek80.py`

 * *Files 1% similar despite different names*

```diff
@@ -1162,15 +1162,15 @@
         #   - gain (indexed by pulse_length)
         # may not exist for data from earlier EK80 software:
         #   - impedance
         #   - receiver sampling frequency
         #   - transceiver type
         table_params = [
             "transducer_frequency",
-            "impedance",  # receive impedance (z_er), different from transmit impedance (z_et)
+            "impedance",  # transceiver impedance (z_er), different from transducer impedance (z_et)
             "rx_sample_frequency",  # receiver sampling frequency
             "transceiver_type",
             "pulse_duration",
             "sa_correction",
             "gain",
         ]
 
@@ -1230,21 +1230,21 @@
                     np.arange(param_dict["pulse_duration"].shape[1]),
                 ),
             },
         )
 
         # Parameters that may or may not exist (due to EK80 software version)
         if "impedance" in param_dict:
-            ds_table["impedance_receive"] = xr.DataArray(
+            ds_table["impedance_transceiver"] = xr.DataArray(
                 param_dict["impedance"],
                 dims=["channel"],
                 coords={"channel": ds_table["channel"]},
                 attrs={
                     "units": "ohm",
-                    "long_name": "Receiver impedance",
+                    "long_name": "Transceiver impedance",
                 },
             )
         if "rx_sample_frequency" in param_dict:
             ds_table["fs_receiver"] = xr.DataArray(
                 param_dict["rx_sample_frequency"].astype(float),
                 dims=["channel"],
                 coords={"channel": ds_table["channel"]},
@@ -1272,15 +1272,15 @@
             # TODO: consider using the full_ch_name below in place of channel id (ch_id)
             # full_ch_name = (f"{config[ch]['transceiver_type']} " +
             #                 f"{config[ch]['serial_number']}-" +
             #                 f"{config[ch]['hw_channel_configuration']} " +
             #                 f"{config[ch]['channel_id_short']}")
             cal_params = [
                 "gain",
-                "impedance",  # transmit impedance (z_et), different from receive impedance (z_er)
+                "impedance",  # transducer impedance (z_et), different from transceiver impedance (z_er)  # noqa
                 "phase",
                 "beamwidth_alongship",
                 "beamwidth_athwartship",
                 "angle_offset_alongship",
                 "angle_offset_athwartship",
             ]
             param_dict = {}
@@ -1304,15 +1304,15 @@
             ds_ch["cal_channel_id"].attrs[
                 "long_name"
             ] = "ID of channels containing broadband calibration information"
             ds_cal.append(ds_ch)
         ds_cal = xr.merge(ds_cal)
 
         if "impedance" in ds_cal:
-            ds_cal = ds_cal.rename_vars({"impedance": "impedance_transmit"})
+            ds_cal = ds_cal.rename_vars({"impedance": "impedance_transducer"})
 
         #  Save decimation factors and filter coefficients
         coeffs = dict()
         decimation_factors = dict()
         for ch in self.sorted_channel["all"]:
             # filter coeffs and decimation factor for wide band transceiver (WBT)
             if self.parser_obj.fil_coeffs and (ch in self.parser_obj.fil_coeffs.keys()):
```

### Comparing `echopype-0.7.0/echopype/convert/utils/ek_date_conversion.py` & `echopype-0.7.1/echopype/convert/utils/ek_date_conversion.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/utils/ek_raw_io.py` & `echopype-0.7.1/echopype/convert/utils/ek_raw_io.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/convert/utils/ek_raw_parsers.py` & `echopype-0.7.1/echopype/convert/utils/ek_raw_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,15 +847,15 @@
                             if f_par:
                                 cal_par = {
                                     "frequency": np.array(
                                         [int(f.attrib["Frequency"]) for f in f_par]
                                     ),
                                     "gain": np.array([float(f.attrib["Gain"]) for f in f_par]),
                                     "impedance": np.array(
-                                        [int(f.attrib["Impedance"]) for f in f_par]
+                                        [float(f.attrib["Impedance"]) for f in f_par]
                                     ),
                                     "phase": np.array([float(f.attrib["Phase"]) for f in f_par]),
                                     "beamwidth_alongship": np.array(
                                         [float(f.attrib["BeamWidthAlongship"]) for f in f_par]
                                     ),
                                     "beamwidth_athwartship": np.array(
                                         [float(f.attrib["BeamWidthAthwartship"]) for f in f_par]
```

### Comparing `echopype-0.7.0/echopype/core.py` & `echopype-0.7.1/echopype/core.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/api.py` & `echopype-0.7.1/echopype/echodata/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/combine.py` & `echopype-0.7.1/echopype/echodata/combine.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/convention/1.0.yml` & `echopype-0.7.1/echopype/echodata/convention/1.0.yml`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/convention/conv.py` & `echopype-0.7.1/echopype/echodata/convention/conv.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/convention/utils.py` & `echopype-0.7.1/echopype/echodata/convention/utils.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/echodata.py` & `echopype-0.7.1/echopype/echodata/echodata.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py` & `echopype-0.7.1/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     Notes
     -----
     The function directly modifies the input EchoData object.
     """
 
     if (0, 5, 0) <= echodata_obj.version_info < (0, 6, 0):
         convert_v05x_to_v06x(echodata_obj)
-    elif (0, 6, 0) <= echodata_obj.version_info < (0, 7, 0):
+    elif (0, 6, 0) <= echodata_obj.version_info < (0, 8, 0):
         pass
     else:
         str_version = ".".join(map(str, echodata_obj.version_info))
         raise NotImplementedError(
-            f"Conversion from echopype v{str_version} to"
-            + f" v{__version__} is not available. Please convert"
-            + f" to version {__version__} using open_raw."
+            f"Conversion of data from echopype v{str_version} format to"
+            + f" v{__version__} format is not available. Please use open_raw"
+            + f" to convert data to version {__version__} format."
         )
```

### Comparing `echopype-0.7.0/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py` & `echopype-0.7.1/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/simrad.py` & `echopype-0.7.1/echopype/echodata/simrad.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/widgets/static/css/style.css` & `echopype-0.7.1/echopype/echodata/widgets/static/css/style.css`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/widgets/static/html/icons-svg-inline.html` & `echopype-0.7.1/echopype/echodata/widgets/static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/widgets/templates/echodata.html.j2` & `echopype-0.7.1/echopype/echodata/widgets/templates/echodata.html.j2`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/widgets/utils.py` & `echopype-0.7.1/echopype/echodata/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/widgets/widgets.py` & `echopype-0.7.1/echopype/echodata/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/echodata/zarr_combine.py` & `echopype-0.7.1/echopype/echodata/zarr_combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import fsspec
 import numpy as np
 import pandas as pd
 import xarray as xr
 import zarr
 from dask.distributed import Lock
 
-from ..utils.coding import COMPRESSION_SETTINGS, get_zarr_compression
+from ..utils.coding import COMPRESSION_SETTINGS, get_zarr_compression, sanitize_dtypes
 from ..utils.io import env_indep_joinpath
 from ..utils.prov import echopype_prov_attrs
 from .api import open_converted
 from .echodata import EchoData
 
 
 class ZarrCombine:
@@ -733,15 +733,15 @@
         for var in const_vars:
             # make sure to choose the dataset with the largest size for variable
             if var in self.dims_df:
                 ds_list_ind = int(self.dims_df[var].argmax())
             else:
                 ds_list_ind = int(0)
 
-            ds_list[ds_list_ind][[var]].to_zarr(
+            sanitize_dtypes(ds_list[ds_list_ind][[var]]).to_zarr(
                 zarr_path,
                 group=zarr_group,
                 mode="a",
                 storage_options=storage_options,
                 consolidated=False,
             )
```

### Comparing `echopype-0.7.0/echopype/mask/api.py` & `echopype-0.7.1/echopype/mask/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/metrics/summary_statistics.py` & `echopype-0.7.1/echopype/metrics/summary_statistics.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/preprocess/api.py` & `echopype-0.7.1/echopype/preprocess/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/qc/api.py` & `echopype-0.7.1/echopype/qc/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/utils/coding.py` & `echopype-0.7.1/echopype/utils/coding.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,31 @@
     "ping_time_transmit": DEFAULT_TIME_ENCODING,
     "time1": DEFAULT_TIME_ENCODING,
     "time2": DEFAULT_TIME_ENCODING,
     "time3": DEFAULT_TIME_ENCODING,
 }
 
 
+EXPECTED_VAR_DTYPE = {"channel": np.str_, "beam": np.str_}  # channel name  # beam name
+
+
+def sanitize_dtypes(ds: xr.Dataset) -> xr.Dataset:
+    """
+    Validates and fixes data type for expected variables
+    """
+
+    if isinstance(ds, xr.Dataset):
+        for name, var in ds.variables.items():
+            if name in EXPECTED_VAR_DTYPE:
+                expected_dtype = EXPECTED_VAR_DTYPE[name]
+                if not np.issubdtype(var.dtype, expected_dtype):
+                    ds[name] = var.astype(expected_dtype)
+    return ds
+
+
 def _encode_dataarray(da, dtype):
     """Encodes and decode datetime64 array similar to writing to file"""
     if da.size == 0:
         return da
     read_encoding = {
         "units": "seconds since 1900-01-01T00:00:00+00:00",
         "calendar": "gregorian",
```

### Comparing `echopype-0.7.0/echopype/utils/io.py` & `echopype-0.7.1/echopype/utils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union
 
 import fsspec
 import xarray as xr
 from fsspec import FSMap
 from fsspec.implementations.local import LocalFileSystem
 
-from ..utils.coding import set_storage_encodings
+from ..utils.coding import sanitize_dtypes, set_storage_encodings
 from ..utils.log import _init_logger
 
 if TYPE_CHECKING:
     from ..core import PathHint
 SUPPORTED_ENGINES = {
     "netcdf4": {
         "ext": ".nc",
@@ -47,14 +47,16 @@
 
 def save_file(ds, path, mode, engine, group=None, compression_settings=None, **kwargs):
     """
     Saves a dataset to netcdf or zarr depending on the engine
     If ``compression_settings`` are set, compress all variables with those settings
     """
 
+    # validate and fix dtype
+    ds = sanitize_dtypes(ds)
     # set zarr or netcdf specific encodings for each variable in ds
     encoding = set_storage_encodings(ds, compression_settings, engine)
 
     # Allows saving both NetCDF and Zarr files from an xarray dataset
     if engine == "netcdf4":
         ds.to_netcdf(path=path, mode=mode, group=group, encoding=encoding, **kwargs)
     elif engine == "zarr":
```

### Comparing `echopype-0.7.0/echopype/utils/log.py` & `echopype-0.7.1/echopype/utils/log.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/utils/prov.py` & `echopype-0.7.1/echopype/utils/prov.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
         if len(func.__qualname__.split(".")) > 1:
             # Handle class methods
             @functools.wraps(func)
             def inner(self, *args, **kwargs):
                 func(self, *args, **kwargs)
                 processing_level = PROCESSING_LEVELS[processing_level_code]
                 self["Top-level"] = self["Top-level"].assign_attrs(_attrs_dict(processing_level))
-                return self
 
             return inner
         else:
             # Handle stand-alone module functions
             @functools.wraps(func)
             def inner(*args, **kwargs):
                 dataobj = func(*args, **kwargs)
```

### Comparing `echopype-0.7.0/echopype/utils/uwa.py` & `echopype-0.7.1/echopype/utils/uwa.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/visualize/api.py` & `echopype-0.7.1/echopype/visualize/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/visualize/cm.py` & `echopype-0.7.1/echopype/visualize/cm.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype/visualize/plot.py` & `echopype-0.7.1/echopype/visualize/plot.py`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/echopype.egg-info/PKG-INFO` & `echopype-0.7.1/echopype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echopype
-Version: 0.7.0
+Version: 0.7.1
 Summary: Enhancing the interoperability and scalability in analyzing ocean sonar data
 Home-page: https://github.com/OSOceanAcoustics/echopype
 Author: Wu-Jung Lee
 Author-email: leewujung@gmail.com
 Maintainer: Wu-Jung Lee
 Maintainer-email: leewujung@gmail.com
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: echopype Version: 0.7.0 Summary: Enhancing the
+Metadata-Version: 2.1 Name: echopype Version: 0.7.1 Summary: Enhancing the
 interoperability and scalability in analyzing ocean sonar data Home-page:
 https://github.com/OSOceanAcoustics/echopype Author: Wu-Jung Lee Author-email:
 leewujung@gmail.com Maintainer: Wu-Jung Lee Maintainer-email:
 leewujung@gmail.com License: Apache License, Version 2.0 Platform: OS
 Independent Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

### Comparing `echopype-0.7.0/echopype.egg-info/SOURCES.txt` & `echopype-0.7.1/echopype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/pyproject.toml` & `echopype-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echopype-0.7.0/setup.cfg` & `echopype-0.7.1/setup.cfg`

 * *Files identical despite different names*

