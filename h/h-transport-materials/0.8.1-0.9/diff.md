# Comparing `tmp/h_transport_materials-0.8.1.tar.gz` & `tmp/h_transport_materials-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h_transport_materials-0.8.1.tar", last modified: Wed Jan 18 17:56:53 2023, max compression
+gzip compressed data, was "h_transport_materials-0.9.tar", last modified: Mon Jan 23 19:03:24 2023, max compression
```

## Comparing `h_transport_materials-0.8.1.tar` & `h_transport_materials-0.9.tar`

### file list

```diff
@@ -1,187 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.261502 h_transport_materials-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.265502 h_transport_materials-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/.github/ISSUE_TEMPLATE/PROPERTY-SUGGESTION.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.265502 h_transport_materials-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.265502 h_transport_materials-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/examples/plot_copper.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/examples/plot_cucrzr.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/examples/plot_lipb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/examples/plot_tungsten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.265502 h_transport_materials-0.8.1/h_transport_materials/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.269502 h_transport_materials-0.8.1/h_transport_materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.269502 h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/aluminium.py
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/young_1998.tar
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/young_diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/beryllium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/carbon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.269502 h_transport_materials-0.8.1/h_transport_materials/materials/copper/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/copper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/copper/copper.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/copper/katz_1971_diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/copper/katz_1971_diffusivity.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.269502 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/cucrzr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_diffusivity.tar
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_diffusivity_1998.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_solubility.tar
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_solubility_1998.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flibe/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flibe/flibe.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flibe/oishi_1989_diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flibe/oishi_1989_diffusivity.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/flinak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/
--rw-r--r--   0 runner    (1001) docker     (123)    57550 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/Fukada.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/data_fukada_2006.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/wpd_project (2).json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/
--rw-r--r--   0 runner    (1001) docker     (123)    50755 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/Capture d’écran 2022-01-24 134538.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/data_fukada_2006.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/fukada_2006.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/data_lam_2020_t.csv
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/data_lam_2020_t_ions.csv
--rw-r--r--   0 runner    (1001) docker     (123)   138565 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/diffusivities_flinak.png
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/lam_2020.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/data_nakamura_2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)    68622 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/diffusivity.png
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/wpd_project (3).json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/
--rw-r--r--   0 runner    (1001) docker     (123)    87575 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/Capture d’écran 2022-01-24 134911.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/data_nakamura_2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/nakamura_2015.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.273502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/diffusivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/diffusivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/diffusivity/data_zeng_2014.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/solubility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/solubility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2014/solubility/data_zeng_2014.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/diffusivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/diffusivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/diffusivity/data_zeng_2019.csv
--rw-r--r--   0 runner    (1001) docker     (123)   245760 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/diffusivity/zeng_2019.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/data_zeng_2019.csv
--rw-r--r--   0 runner    (1001) docker     (123)   245760 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/project.tar
--rw-r--r--   0 runner    (1001) docker     (123)   223870 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/properties.png
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/gold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/hastelloy_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/hastelloy_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/incoloy_800.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/inconel_600.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/inconel_625.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/inconel_750.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/iron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/aiello_2006/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/aiello_2006/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/aiello_2006/aiello_solubility_lipb_2006.tar
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/aiello_2006/solubility_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/lipb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/reiter_diffusivity.tar
--rw-r--r--   0 runner    (1001) docker     (123)    61440 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/reiter_solubility.tar
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/solubility.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92160 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/schumacher.tar
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/solubility.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.277502 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61440 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/alire_1976.tar
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/lithium/lithium.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/molybdenum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/nickel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/nimonic_80A.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/niobium.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/palladium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/palladium_alloy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/diffusivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)   133120 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/serra_diffusivity.tar
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/solubility.csv
--rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/solubility.tar
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/rafm_steel.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/series_300_steel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/ss_304.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/steel_316L.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/tantalum.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/titanium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/tungsten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/vanadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/vanadium_alloy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/yamanaka_1989/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/yamanaka_1989/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/yamanaka_1989/solubility.csv
--rw-r--r--   0 runner    (1001) docker     (123)    92160 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/yamanaka_1989/yamanaka_1989.tar
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/zirconium.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/properties_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/property.py
--rw-r--r--   0 runner    (1001) docker     (123)   167145 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/h_transport_materials/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.265502 h_transport_materials-0.8.1/h_transport_materials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-18 17:56:53.000000 h_transport_materials-0.8.1/h_transport_materials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:53.281502 h_transport_materials-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_arhenius_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_diffusivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_properties_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_solubility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-18 17:56:43.000000 h_transport_materials-0.8.1/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.560932 h_transport_materials-0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.532933 h_transport_materials-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.536933 h_transport_materials-0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-23 19:03:13.000000 h_transport_materials-0.9/.github/ISSUE_TEMPLATE/PROPERTY-SUGGESTION.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.536933 h_transport_materials-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-23 19:03:13.000000 h_transport_materials-0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-23 19:03:13.000000 h_transport_materials-0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-23 19:03:13.000000 h_transport_materials-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-23 19:03:13.000000 h_transport_materials-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-23 19:03:24.560932 h_transport_materials-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-01-23 19:03:13.000000 h_transport_materials-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.540933 h_transport_materials-0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-23 19:03:13.000000 h_transport_materials-0.9/examples/plot_copper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-23 19:03:13.000000 h_transport_materials-0.9/examples/plot_cucrzr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-23 19:03:13.000000 h_transport_materials-0.9/examples/plot_lipb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-23 19:03:13.000000 h_transport_materials-0.9/examples/plot_tungsten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.540933 h_transport_materials-0.9/h_transport_materials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/properties_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/aluminium/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/aluminium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/aluminium/aluminium.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/aluminium/young_1998.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/aluminium/young_diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/beryllium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/carbon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/copper/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/copper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/copper/copper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/copper/katz_1971_diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/copper/katz_1971_diffusivity.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/cucrzr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_diffusivity.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_diffusivity_1998.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_solubility.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_solubility_1998.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/flibe/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flibe/flibe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flibe/oishi_1989_diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flibe/oishi_1989_diffusivity.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/flinak/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/flinak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (123)    57550 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/Fukada.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/data_fukada_2006.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/wpd_project (2).json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.544932 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/
+-rw-r--r--   0 runner    (1001) docker     (123)    50755 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/Capture d’écran 2022-01-24 134538.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/data_fukada_2006.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/fukada_2006.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/data_lam_2020_t.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/data_lam_2020_t_ions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   138565 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/diffusivities_flinak.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/lam_2020.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/data_nakamura_2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68622 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/diffusivity.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/wpd_project (3).json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/
+-rw-r--r--   0 runner    (1001) docker     (123)    87575 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/Capture d’écran 2022-01-24 134911.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/data_nakamura_2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/nakamura_2015.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/diffusivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/diffusivity/data_zeng_2014.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/solubility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/solubility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2014/solubility/data_zeng_2014.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/diffusivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/diffusivity/data_zeng_2019.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   245760 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/diffusivity/zeng_2019.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.548933 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/data_zeng_2019.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   245760 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/project.tar
+-rw-r--r--   0 runner    (1001) docker     (123)   223870 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/properties.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/gold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/hastelloy_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/hastelloy_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/incoloy_800.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/inconel_600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/inconel_625.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/inconel_750.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/iron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lipb/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lipb/aiello_2006/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/aiello_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/aiello_2006/aiello_solubility_lipb_2006.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/aiello_2006/solubility_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/lipb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/reiter_diffusivity.tar
+-rw-r--r--   0 runner    (1001) docker     (123)    61440 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/reiter_solubility.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/solubility.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92160 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/schumacher.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/solubility.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lithium/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lithium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61440 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/alire_1976.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/lithium/lithium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/molybdenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/nickel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/nimonic_80A.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/niobium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/palladium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/pdag/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/palladium_alloy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   133120 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/serra_diffusivity.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/solubility.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/solubility.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/rafm_steel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/series_300_steel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/ss_304.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.552933 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/diffusivity_solubility.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   276480 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/diffusivity_solubility.tar
+-rw-r--r--   0 runner    (1001) docker     (123)   307200 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/lee_2011_permeability.tar
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/lee_2011/permeability.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/steel_316L.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tantalum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/titanium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/diffusivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   174080 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/diffusivity.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/permeability.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   256000 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/liu_2016/permeablity.tar
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/tungsten/tungsten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/vanadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/vanadium_alloy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/yamanaka_1989/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/yamanaka_1989/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/yamanaka_1989/solubility.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    92160 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/yamanaka_1989/yamanaka_1989.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/property_database/zirconium/zirconium.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188526 2023-01-23 19:03:13.000000 h_transport_materials-0.9/h_transport_materials/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.540933 h_transport_materials-0.9/h_transport_materials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-23 19:03:24.000000 h_transport_materials-0.9/h_transport_materials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-23 19:03:13.000000 h_transport_materials-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-23 19:03:24.560932 h_transport_materials-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-23 19:03:13.000000 h_transport_materials-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:24.556933 h_transport_materials-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_arhenius_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_diffusivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_properties_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_solubility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-23 19:03:13.000000 h_transport_materials-0.9/tests/test_system.py
```

### Comparing `h_transport_materials-0.8.1/.github/ISSUE_TEMPLATE/PROPERTY-SUGGESTION.yml` & `h_transport_materials-0.9/.github/ISSUE_TEMPLATE/PROPERTY-SUGGESTION.yml`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/.github/workflows/ci.yml` & `h_transport_materials-0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/.github/workflows/python-publish.yml` & `h_transport_materials-0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/.gitignore` & `h_transport_materials-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/LICENSE` & `h_transport_materials-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/PKG-INFO` & `h_transport_materials-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h_transport_materials
-Version: 0.8.1
+Version: 0.9
 Summary: Handle H transport properties
 Home-page: https://github.com/RemDelaporteMathurin/h_transport_materials
 Author: Remi Delaporte-Mathurin
 Author-email: rdelaportemathurin@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/RemDelaporteMathurin/h_transport_materials
 Project-URL: Tracker, https://github.com/RemDelaporteMathurin/h_transport_materials/issues
@@ -55,15 +55,16 @@
 
 
 plt.yscale("log")
 plt.ylabel("Diffusivity (m$^2$/s)")
 plt.legend()
 plt.show()
 ```
-![Figure_1](https://user-images.githubusercontent.com/40028739/169280320-c4d45d9b-7f33-4628-a4fd-72e81be16124.svg)
+![Figure_1](https://user-images.githubusercontent.com/40028739/213814746-9dadb8dc-599e-4004-8135-e496b19fd8bc.png)
+
 >
 ### Add custom properties
 
 ```python
 import h_transport_materials as htm
 
 import numpy as np
```

### Comparing `h_transport_materials-0.8.1/README.md` & `h_transport_materials-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 
 plt.yscale("log")
 plt.ylabel("Diffusivity (m$^2$/s)")
 plt.legend()
 plt.show()
 ```
-![Figure_1](https://user-images.githubusercontent.com/40028739/169280320-c4d45d9b-7f33-4628-a4fd-72e81be16124.svg)
+![Figure_1](https://user-images.githubusercontent.com/40028739/213814746-9dadb8dc-599e-4004-8135-e496b19fd8bc.png)
+
 >
 ### Add custom properties
 
 ```python
 import h_transport_materials as htm
 
 import numpy as np
```

### Comparing `h_transport_materials-0.8.1/examples/plot_copper.py` & `h_transport_materials-0.9/examples/plot_copper.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/examples/plot_cucrzr.py` & `h_transport_materials-0.9/examples/plot_cucrzr.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/examples/plot_lipb.py` & `h_transport_materials-0.9/examples/plot_lipb.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/examples/plot_tungsten.py` & `h_transport_materials-0.9/examples/plot_tungsten.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/__init__.py` & `h_transport_materials-0.9/h_transport_materials/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,19 @@
     RecombinationCoeff,
     DissociationCoeff,
 )
 from .properties_group import PropertiesGroup
 from . import conversion
 from . import fitting
 from . import plotting
+from .material import *
 
 database = PropertiesGroup()
 
-from .materials import *
+from . import property_database
 
 diffusivities = PropertiesGroup(
     prop for prop in database if isinstance(prop, Diffusivity)
 )
 
 solubilities = PropertiesGroup(
     prop for prop in database if isinstance(prop, Solubility)
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/conversion.py` & `h_transport_materials-0.9/h_transport_materials/conversion.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/fitting.py` & `h_transport_materials-0.9/h_transport_materials/fitting.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/__init__.py` & `h_transport_materials-0.9/h_transport_materials/property_database/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from .material import Material
-
 from . import aluminium
 
 from . import copper
 
 from . import cucrzr
 
 from . import flinak
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/aluminium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/niobium.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 import h_transport_materials as htm
 from h_transport_materials import Diffusivity, Solubility
-from pathlib import Path
-import numpy as np
+import h_transport_materials.conversion as c
 
+NIOBIUM_MOLAR_VOLUME = 1.08e-8  # m3/mol https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/niobium
 
-# Fig 6 of Young's paper
-data_diffusivity_young = np.genfromtxt(
-    str(Path(__file__).parent) + "/young_diffusivity.csv",
-    delimiter=",",
+volkl_diffusivity = Diffusivity(
+    D_0=5.00e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
+    E_D=10.2 * htm.ureg.kJ * htm.ureg.mol**-1,
+    range=(273 * htm.ureg.K, 773 * htm.ureg.K),
+    source="volkl_5_1975",
+    isotope="H",
 )
 
-young_diffusivity = Diffusivity(
-    data_T=1e3 / data_diffusivity_young[:, 0] * htm.ureg.K,
-    data_y=np.exp(data_diffusivity_young[:, 1]) * htm.ureg.cm**2 * htm.ureg.s**-1,
+schober_diffusivity = Diffusivity(
+    D_0=4.4e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
+    E_D=12.8 * htm.ureg.kJ * htm.ureg.mol**-1,
+    source="schober_h_1990",
     isotope="H",
-    source="young_diffusion_1998",
 )
 
-ransley_solubility = Solubility(
+veleckis_solubility = Solubility(
+    units="m-3 Pa-1/2",
+    S_0=1.26e-1 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
+    E_S=-35.3 * htm.ureg.kJ * htm.ureg.mol**-1,
+    range=(625 * htm.ureg.K, 944 * htm.ureg.K),
+    source="veleckis_thermodynamic_1969",
     isotope="H",
+)
+
+reiter_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=2.32e-2 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=39.7 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(723 * htm.ureg.K, 873 * htm.ureg.K),
-    author="ransley",
-    year=1948,
-    source="Ransley, C.E., Neufeld, H., 1948. J. Inst. Met. 74, 599–620",
+    S_0=3.6e-6
+    / NIOBIUM_MOLAR_VOLUME
+    * htm.ureg.mol
+    * htm.ureg.m**-3
+    * htm.ureg.Pa**-0.5,
+    E_S=-33.9 * htm.ureg.kJ * htm.ureg.mol**-1,
+    source="reiter_compilation_1996",
+    isotope="H",
 )
 
-properties = [young_diffusivity, ransley_solubility]
+properties = [
+    volkl_diffusivity,
+    schober_diffusivity,
+    veleckis_solubility,
+    reiter_solubility,
+]
 
 for prop in properties:
-    prop.material = "aluminium"
+    prop.material = htm.NIOBIUM
 
 htm.database += properties
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/young_1998.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/aluminium/young_1998.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/aluminium/young_diffusivity.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/aluminium/young_diffusivity.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/beryllium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/beryllium.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
 jones_diffusivity = Diffusivity(
     isotope="T",
     D_0=np.exp(-6.53) * htm.ureg.cm**2 * htm.ureg.s**-1,
     E_D=965 * htm.ureg.K * htm.k_B,
     range=(400 * htm.ureg.K, 900 * htm.ureg.K),
     source="jones_hydrogen_1967",
+    note="Jones also gives a solubility but the units are weird",
 )
 
 dolan_recombination = RecombinationCoeff(
     pre_exp=1.46e-29 * htm.ureg.m**4 * htm.ureg.s**-1 * htm.ureg.particle**-1,
     act_energy=0.214 * htm.ureg.eV * htm.ureg.particle**-1,
     source="dolan_assessment_1994",
     isotope="H",
-    note="Jones also gives a solubility but the units are weird",
 )
 
 
 properties = [
     shapovalov_solubility,
     abramov_diffusivity,
     jones_diffusivity,
     dolan_recombination,
 ]
 
 for prop in properties:
-    prop.material = "beryllium"
+    prop.material = htm.BERYLLIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/carbon.py` & `h_transport_materials-0.9/h_transport_materials/property_database/carbon.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,10 +30,10 @@
     source="atsumi_absorption_1988",
     isotope="H",
 )
 
 properties = [causey_diffusivity, atsumi_diffusivity, atsumi_solubility]
 
 for prop in properties:
-    prop.material = "carbon"
+    prop.material = htm.CARBON
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/copper/copper.py` & `h_transport_materials-0.9/h_transport_materials/property_database/copper/copper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import h_transport_materials as htm
 from h_transport_materials.property import (
     Diffusivity,
     Permeability,
     RecombinationCoeff,
     Solubility,
 )
-from h_transport_materials.materials import Material
 from pathlib import Path
 import numpy as np
 
 COPPER_MOLAR_VOLUME = 7.11e-6  # m3/mol  https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/copper
 
 # ################# REITER 1996 #############################
 
@@ -301,10 +300,10 @@
     eichenauer_solubility_copper_h,
     mclellan_solubility,
     anderl_recombination,
     houben_permeability,
 ]
 
 for prop in properties:
-    prop.material = "copper"
+    prop.material = htm.COPPER
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/copper/katz_1971_diffusivity.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/copper/katz_1971_diffusivity.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/copper/katz_1971_diffusivity.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/copper/katz_1971_diffusivity.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/cucrzr.py` & `h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/cucrzr.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,10 +181,10 @@
     nog_solubility_cucrzr_t_2,
     penalva_solubility_cucrzr_h,
     anderl_recombination,
     houben_permeability,
 ]
 
 for prop in properties:
-    prop.material = "cucrzr"
+    prop.material = htm.CUCRZR
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_diffusivity.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_diffusivity.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_diffusivity_1998.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_diffusivity_1998.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_solubility.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_solubility.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/cucrzr/serra_solubility_1998.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/cucrzr/serra_solubility_1998.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flibe/flibe.py` & `h_transport_materials-0.9/h_transport_materials/property_database/flibe/flibe.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,10 +141,10 @@
     field_solubility_h,
     field_solubility_d,
     maulinauskas_solubility_h,
     maulinauskas_solubility_d,
 ]
 
 for prop in properties:
-    prop.material = "flibe"
+    prop.material = htm.FLIBE
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flibe/oishi_1989_diffusivity.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/flibe/oishi_1989_diffusivity.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/flinak.py` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/flinak.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,10 +144,10 @@
     nakamura_solubility_h,
     fukada_solubility_h,
     zeng_solubility_h_2019,
     zeng_solubility_h_2014,
 ]
 
 for prop in properties:
-    prop.material = "flinak"
+    prop.material = htm.FLINAK
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/Fukada.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/Fukada.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/diffusivity/wpd_project (2).json` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/diffusivity/wpd_project (2).json`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/Capture d’écran 2022-01-24 134538.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/Capture d’écran 2022-01-24 134538.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/fukada_2006/solubility/fukada_2006.json` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/fukada_2006/solubility/fukada_2006.json`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/diffusivities_flinak.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/diffusivities_flinak.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/lam_2020/lam_2020.json` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/lam_2020/lam_2020.json`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/diffusivity.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/diffusivity.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/diffusivity/wpd_project (3).json` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/diffusivity/wpd_project (3).json`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/Capture d’écran 2022-01-24 134911.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/Capture d’écran 2022-01-24 134911.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/nakamura_2015/solubility/nakamura_2015.json` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/nakamura_2015/solubility/nakamura_2015.json`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/diffusivity/zeng_2019.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/diffusivity/zeng_2019.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/project.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/project.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/flinak/zeng_2019/solubility/properties.png` & `h_transport_materials-0.9/h_transport_materials/property_database/flinak/zeng_2019/solubility/properties.png`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/gold.py` & `h_transport_materials-0.9/h_transport_materials/property_database/gold.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
     isotope="H",
 )
 
 
 properties = [eichenauer_diffusivity, shimada_solubility, mclellan_solubility]
 
 for prop in properties:
-    prop.material = "gold"
+    prop.material = htm.GOLD
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/hastelloy_n.py` & `h_transport_materials-0.9/h_transport_materials/property_database/hastelloy_n.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,10 @@
     zhang_diffusivity_h,
     zhang_diffusivity_d,
     zhang_solubility_h,
     zhang_solubility_d,
 ]
 
 for prop in properties:
-    prop.material = "hastelloy_n"
+    prop.material = htm.HASTELLOY_N
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/hastelloy_x.py` & `h_transport_materials-0.9/h_transport_materials/property_database/nimonic_80A.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,32 @@
     Solubility,
     Permeability,
     DissociationCoeff,
     RecombinationCoeff,
 )
 
 kishimoto_diffusivity = Diffusivity(
-    D_0=4.9e-3 * htm.ureg.cm**2 * htm.ureg.s**-1,
-    E_D=0.45 * htm.ureg.eV * htm.ureg.particle**-1,
+    D_0=1.4e-2 * htm.ureg.cm**2 * htm.ureg.s**-1,
+    E_D=0.55 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
     range=(873 * htm.ureg.K, 1173 * htm.ureg.K),
     source="kishimoto_hydrogen_1985",
 )
 
 kishimoto_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=41 * htm.ureg.ccNTP * htm.ureg.cm**-3 * htm.ureg.MPa**-0.5,
-    E_S=0.22 * htm.ureg.eV * htm.ureg.particle**-1,
+    S_0=17 * htm.ureg.ccNTP * htm.ureg.cm**-3 * htm.ureg.MPa**-0.5,
+    E_S=0.12 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
     range=(873 * htm.ureg.K, 1173 * htm.ureg.K),
     source="kishimoto_hydrogen_1985",
 )
 
 kishimoto_permeability = Permeability(
-    pre_exp=7.2e3
+    pre_exp=8.1e3
     * htm.ureg.ccNTP
     * htm.ureg.mm
     * htm.ureg.cm**-2
     * htm.ureg.h**-1
     * htm.ureg.MPa**-0.5,
     act_energy=0.67 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
@@ -40,10 +40,10 @@
 properties = [
     kishimoto_diffusivity,
     kishimoto_solubility,
     kishimoto_permeability,
 ]
 
 for prop in properties:
-    prop.material = "hastelloy_x"
+    prop.material = htm.NIMONIC_80A
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/incoloy_800.py` & `h_transport_materials-0.9/h_transport_materials/property_database/incoloy_800.py`

 * *Files 15% similar despite different names*

```diff
@@ -103,24 +103,41 @@
     range=(427 * u.K, 780 * u.K),
     isotope="D",
     source="esteban_diffusive_2002",
     note="oxidised surface",
 )
 
 
+masui_permeability = Permeability(
+    pre_exp=2440
+    * htm.ureg.ccNTP
+    * htm.ureg.mm
+    * htm.ureg.cm**-2
+    * htm.ureg.h**-1
+    * htm.ureg.atm**-0.5,
+    act_energy=16500 * htm.ureg.cal * htm.ureg.mol**-1,
+    range=(
+        htm.ureg.Quantity(800, htm.ureg.degC),
+        htm.ureg.Quantity(1000, htm.ureg.degC),
+    ),
+    isotope="H",
+    source="masui_hydrogen_1978",
+)
+
 properties = [
     schmidt_diffusivity,
     schmidt_permeability,
     schmidt_solubility,
     esteban_permeability,
     esteban_diffusivity,
     esteban_solubility,
     esteban_diss_coeff_non_oxidised,
     esteban_recomb_coeff_non_oxidised,
     esteban_diss_coeff_oxidised,
     esteban_recomb_coeff_oxidised,
+    masui_permeability,
 ]
 
 for prop in properties:
-    prop.material = "incoloy_800"
+    prop.material = htm.INCOLOY_800
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/inconel_600.py` & `h_transport_materials-0.9/h_transport_materials/property_database/inconel_600.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,27 +169,44 @@
     range=(
         htm.ureg.Quantity(150, htm.ureg.degC),
         htm.ureg.Quantity(400, htm.ureg.degC),
     ),
     source="rota_measurements_1982",
 )
 
+masui_permeability = Permeability(
+    pre_exp=2540
+    * htm.ureg.ccNTP
+    * htm.ureg.mm
+    * htm.ureg.cm**-2
+    * htm.ureg.h**-1
+    * htm.ureg.atm**-0.5,
+    act_energy=15800 * htm.ureg.cal * htm.ureg.mol**-1,
+    range=(
+        htm.ureg.Quantity(800, htm.ureg.degC),
+        htm.ureg.Quantity(1000, htm.ureg.degC),
+    ),
+    isotope="H",
+    source="masui_hydrogen_1978",
+)
+
 properties = [
     kishimoto_diffusivity,
     kishimoto_solubility,
     kishimoto_permeability,
     rota_diffusivity_h,
     rota_diffusivity_d,
     rota_permeability_h,
     rota_permeability_d,
     rota_solubility_h,
     rota_solubility_d,
     rota_dissociation_coeff_h,
     rota_dissociation_coeff_d,
     rota_recombination_coeff_h,
     rota_recombination_coeff_d,
+    masui_permeability,
 ]
 
 for prop in properties:
-    prop.material = "inconel_600"
+    prop.material = htm.INCONEL_600
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/inconel_625.py` & `h_transport_materials-0.9/h_transport_materials/property_database/inconel_625.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,10 +85,10 @@
     perujo_dissociation_coeff_clean,
     perujo_recombination_coeff_clean,
     perujo_dissociation_coeff_oxidised,
     perujo_recombination_coeff_oxidised,
 ]
 
 for prop in properties:
-    prop.material = "inconel_625"
+    prop.material = htm.INCONEL_625
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/inconel_750.py` & `h_transport_materials-0.9/h_transport_materials/property_database/inconel_750.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 properties = [
     kishimoto_diffusivity,
     kishimoto_solubility,
     kishimoto_permeability,
 ]
 
 for prop in properties:
-    prop.material = "inconel_750"
+    prop.material = htm.INCONEL_750
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/aiello_2006/aiello_solubility_lipb_2006.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/aiello_2006/aiello_solubility_lipb_2006.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/lipb.py` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/lipb.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,10 +375,10 @@
     okitsu_diffusivity_h,
     okitsu_diffusivity_d,
     okitsu_solubility_h,
     okitsu_solubility_d,
 ]
 
 for prop in properties:
-    prop.material = "lipb"
+    prop.material = htm.LIPB
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/diffusivity.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/diffusivity.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/reiter_diffusivity.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/reiter_diffusivity.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/reiter_solubility.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/reiter_solubility.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/reiter_1991/solubility.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/reiter_1991/solubility.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/schumacher.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/schumacher.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lipb/schumacher_1990/solubility.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/lipb/schumacher_1990/solubility.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/alire_1976.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/alire_1976.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lithium/alire_1976/diffusivity.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/lithium/alire_1976/diffusivity.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/lithium/lithium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/lithium/lithium.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     isotope="H",
     units="m-3 Pa-1/2",
 )
 
 properties = [alire_diffusivity, veleckis_solubility]
 
 for prop in properties:
-    prop.material = "lithium"
+    prop.material = htm.LITHIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/molybdenum.py` & `h_transport_materials-0.9/h_transport_materials/property_database/molybdenum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import h_transport_materials as htm
-from h_transport_materials import Diffusivity, Solubility
-import h_transport_materials.conversion as c
+from h_transport_materials import Diffusivity, Solubility, Permeability
 
 import numpy as np
 
 tanabe_diffusivity = Diffusivity(
     D_0=4.00e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
     E_D=22.3 * htm.ureg.kJ * htm.ureg.mol**-1,
     isotope="H",
@@ -33,18 +32,39 @@
     units="m-3 Pa-1/2",
     S_0=np.exp(8.703) * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
     E_S=7.863e3 * htm.ureg.K * htm.k_B,
     isotope="H",
     source="katsuta_diffusivity_1982",
 )
 
+
+frauenfelder_p_0 = (
+    7.1e-4
+    * htm.ureg.torr
+    * htm.ureg.liter
+    * htm.ureg.cm**-1
+    * htm.ureg.s**-1
+    * htm.ureg.torr**-0.5
+)
+frauenfelder_permeability = Permeability(
+    pre_exp=frauenfelder_p_0 / (htm.Rg * 300 * htm.ureg.K),
+    act_energy=21.5 * htm.ureg.kcal * htm.ureg.mol**-1,
+    isotope="H",
+    range=(
+        htm.ureg.Quantity(1050, htm.ureg.degC),
+        htm.ureg.Quantity(2400, htm.ureg.degC),
+    ),
+    source="frauenfelder_permeation_1968",
+)
+
 properties = [
     tanabe_diffusivity,
     katsuta_diffusivity,
     tanabe_solubility,
     katsuta_solubility,
+    frauenfelder_permeability,
 ]
 
 for prop in properties:
-    prop.material = "molybdenum"
+    prop.material = htm.MOLYBDENUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/nickel.py` & `h_transport_materials-0.9/h_transport_materials/property_database/nickel.py`

 * *Files 24% similar despite different names*

```diff
@@ -94,25 +94,41 @@
     pre_exp=1.44e-6 * u.mol * u.m**-2 * u.s**-1 * u.Pa**-1,
     act_energy=29.68 * u.kJ * u.mol**-1,
     range=(373 * u.K, 623 * u.K),
     isotope="H",
     source="altunoglu_permeation_1991",
 )
 
+masui_permeability = Permeability(
+    pre_exp=1340
+    * htm.ureg.ccNTP
+    * htm.ureg.mm
+    * htm.ureg.cm**-2
+    * htm.ureg.h**-1
+    * htm.ureg.atm**-0.5,
+    act_energy=13000 * htm.ureg.cal * htm.ureg.mol**-1,
+    range=(
+        htm.ureg.Quantity(300, htm.ureg.degC),
+        htm.ureg.Quantity(1000, htm.ureg.degC),
+    ),
+    isotope="H",
+    source="masui_hydrogen_1978",
+)
 
 properties = [
     volkl_diffusivity,
     robertson_diffusivity,
     louthan_diffusivity_H,
     louthan_diffusivity_D,
     louthan_diffusivity_T,
     robertson_solubility,
     louthan_solubility,
     altunoglu_permeability,
     altonoglu_diffusivity,
     altonoglu_dissociation_coeff,
+    masui_permeability,
 ]
 
 for prop in properties:
-    prop.material = "nickel"
+    prop.material = htm.NICKEL
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/nimonic_80A.py` & `h_transport_materials-0.9/h_transport_materials/property_database/hastelloy_x.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,46 +4,64 @@
     Solubility,
     Permeability,
     DissociationCoeff,
     RecombinationCoeff,
 )
 
 kishimoto_diffusivity = Diffusivity(
-    D_0=1.4e-2 * htm.ureg.cm**2 * htm.ureg.s**-1,
-    E_D=0.55 * htm.ureg.eV * htm.ureg.particle**-1,
+    D_0=4.9e-3 * htm.ureg.cm**2 * htm.ureg.s**-1,
+    E_D=0.45 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
     range=(873 * htm.ureg.K, 1173 * htm.ureg.K),
     source="kishimoto_hydrogen_1985",
 )
 
 kishimoto_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=17 * htm.ureg.ccNTP * htm.ureg.cm**-3 * htm.ureg.MPa**-0.5,
-    E_S=0.12 * htm.ureg.eV * htm.ureg.particle**-1,
+    S_0=41 * htm.ureg.ccNTP * htm.ureg.cm**-3 * htm.ureg.MPa**-0.5,
+    E_S=0.22 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
     range=(873 * htm.ureg.K, 1173 * htm.ureg.K),
     source="kishimoto_hydrogen_1985",
 )
 
 kishimoto_permeability = Permeability(
-    pre_exp=8.1e3
+    pre_exp=7.2e3
     * htm.ureg.ccNTP
     * htm.ureg.mm
     * htm.ureg.cm**-2
     * htm.ureg.h**-1
     * htm.ureg.MPa**-0.5,
     act_energy=0.67 * htm.ureg.eV * htm.ureg.particle**-1,
     isotope="H",
     range=(873 * htm.ureg.K, 1173 * htm.ureg.K),
     source="kishimoto_hydrogen_1985",
 )
 
+
+masui_permeability = Permeability(
+    pre_exp=2290
+    * htm.ureg.ccNTP
+    * htm.ureg.mm
+    * htm.ureg.cm**-2
+    * htm.ureg.h**-1
+    * htm.ureg.atm**-0.5,
+    act_energy=16000 * htm.ureg.cal * htm.ureg.mol**-1,
+    range=(
+        htm.ureg.Quantity(800, htm.ureg.degC),
+        htm.ureg.Quantity(1000, htm.ureg.degC),
+    ),
+    isotope="H",
+    source="masui_hydrogen_1978",
+)
+
 properties = [
     kishimoto_diffusivity,
     kishimoto_solubility,
     kishimoto_permeability,
+    masui_permeability,
 ]
 
 for prop in properties:
-    prop.material = "nimonic_80A"
+    prop.material = htm.HASTELLOY_X
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/niobium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/vanadium.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import h_transport_materials as htm
 from h_transport_materials import Diffusivity, Solubility
 import h_transport_materials.conversion as c
 
-NIOBIUM_MOLAR_VOLUME = 1.08e-8  # m3/mol https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/niobium
+VANADIUM_MOLAR_VOLUME = 8.34e-6  # m3/mol  https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/vanadium
 
-volkl_diffusivity = Diffusivity(
-    D_0=5.00e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=10.2 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(273 * htm.ureg.K, 773 * htm.ureg.K),
-    source="volkl_5_1975",
-    isotope="H",
-)
-
-schober_diffusivity = Diffusivity(
-    D_0=4.4e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=12.8 * htm.ureg.kJ * htm.ureg.mol**-1,
-    source="schober_h_1990",
+volk_diffusivity = Diffusivity(
+    D_0=2.9e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
+    E_D=4.2 * htm.ureg.kJ * htm.ureg.mol**-1,
     isotope="H",
+    source="volkl_5_1975",
+    range=(173 * htm.ureg.K, 573 * htm.ureg.K),
 )
 
 veleckis_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=1.26e-1 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=-35.3 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(625 * htm.ureg.K, 944 * htm.ureg.K),
-    source="veleckis_thermodynamic_1969",
     isotope="H",
+    range=(519 * htm.ureg.K, 827 * htm.ureg.K),
+    S_0=1.38e-1 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
+    E_S=-29.0 * htm.ureg.kJ * htm.ureg.mol**-1,
+    source="veleckis_thermodynamic_1969",
 )
 
+schober_diffusivity = Diffusivity(
+    D_0=5.6e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
+    E_D=9.1 * htm.ureg.kJ * htm.ureg.mol**-1,
+    range=(
+        htm.ureg.Quantity(-150, htm.ureg.degC),
+        htm.ureg.Quantity(200, htm.ureg.degC),
+    ),
+    source="schober_h_1990",
+    isotope="H",
+    note="found in Assessment of Database for Interaction of Tritium with ITER Plasma Facing Materials",
+)  # TODO get data from experimental points, see issue #64
+
 reiter_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=3.6e-6
-    / NIOBIUM_MOLAR_VOLUME
+    S_0=2.1e-6
+    / VANADIUM_MOLAR_VOLUME
     * htm.ureg.mol
     * htm.ureg.m**-3
     * htm.ureg.Pa**-0.5,
-    E_S=-33.9 * htm.ureg.kJ * htm.ureg.mol**-1,
+    E_S=-32.2 * htm.ureg.kJ * htm.ureg.mol**-1,
     source="reiter_compilation_1996",
     isotope="H",
 )
 
-properties = [
-    volkl_diffusivity,
-    schober_diffusivity,
-    veleckis_solubility,
-    reiter_solubility,
-]
+properties = [volk_diffusivity, veleckis_solubility]
 
 for prop in properties:
-    prop.material = "niobium"
+    prop.material = htm.VANADIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/palladium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/palladium.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,10 +256,10 @@
     source="favreau_solubility_1954",
     isotope="H",
 )
 
 properties = [volkl_diffusivity, favreau_solubility_t, favreau_solubility_h]
 
 for prop in properties:
-    prop.material = "palladium"
+    prop.material = htm.PALLADIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/pdag/palladium_alloy.py` & `h_transport_materials-0.9/h_transport_materials/property_database/pdag/palladium_alloy.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     serra_diffusivity_h,
     serra_diffusivity_d,
     serra_solubility_h,
     serra_solubility_d,
 ]
 
 for prop in properties:
-    prop.material = "pdag"
+    prop.material = htm.PDAG
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/diffusivity.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/diffusivity.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/serra_diffusivity.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/serra_diffusivity.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/solubility.csv` & `h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/solubility.csv`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/pdag/serra_1998/solubility.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/pdag/serra_1998/solubility.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/rafm_steel.py` & `h_transport_materials-0.9/h_transport_materials/property_database/rafm_steel.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,10 +256,10 @@
     kulsartov_solubility_h,
     kulsartov_solubility_d,
     serra_solubility_f82h,
     serra_solubility_batman,
 ]
 
 for prop in properties:
-    prop.material = "rafm_steel"
+    prop.material = htm.STEEL_RAFM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/series_300_steel.py` & `h_transport_materials-0.9/h_transport_materials/property_database/series_300_steel.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     isotope="H",
     source="perng_effects_1986",
 )
 
 properties = [perng_diffusivity, perng_solubility]
 
 for prop in properties:
-    prop.material = "300_series_steel"
+    prop.material = htm.STEEL_SERIES_300
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/silver.py` & `h_transport_materials-0.9/h_transport_materials/property_database/silver.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,10 @@
     isotope="H",
     note="there is likely a mistake in Shimada's 2020 Review",
 )
 
 properties = [katsuta_diffusivity, mclellan_solubility]
 
 for prop in properties:
-    prop.material = "silver"
+    prop.material = htm.SILVER
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/ss_304.py` & `h_transport_materials-0.9/h_transport_materials/property_database/ss_304.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,10 +155,10 @@
     braun_recombination_coeff,
     braun_dissociation_coeff,
     braun_permeability,
     hawkins_solubility,
 ]
 
 for prop in properties:
-    prop.material = "ss_304"
+    prop.material = htm.STEEL_304
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/steel_316L.py` & `h_transport_materials-0.9/h_transport_materials/property_database/steel_316L/steel_316L.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from h_transport_materials import (
     Diffusivity,
     Solubility,
     Permeability,
     DissociationCoeff,
     RecombinationCoeff,
 )
-import h_transport_materials.conversion as c
-from h_transport_materials.materials.iron import IRON_MOLAR_VOLUME
-
+from h_transport_materials.property_database.iron import IRON_MOLAR_VOLUME
+from pathlib import Path
+import numpy as np
 
 reiter_diffusivity = Diffusivity(
     D_0=3.70e-7 * htm.ureg.m**2 * htm.ureg.s**-1,
     E_D=51.9 * htm.ureg.kJ * htm.ureg.mol**-1,
     range=(500 * htm.ureg.K, 1200 * htm.ureg.K),
     isotope="H",
     source="reiter_compilation_1996",
@@ -179,14 +179,54 @@
         htm.ureg.Quantity(200, htm.ureg.degC),
         htm.ureg.Quantity(430, htm.ureg.degC),
     ),
     isotope="H",
     source="xiukui_hydrogen_1989",
 )
 
+lee_permeability_data = np.genfromtxt(
+    str(Path(__file__).parent) + "/lee_2011/permeability.csv",
+    delimiter=",",
+    names=True,
+)
+lee_data_invT = lee_permeability_data["X"] * htm.ureg.K**-1
+lee_permeability = Permeability(
+    data_T=1 / lee_data_invT,
+    data_y=lee_permeability_data["Y"]
+    * htm.ureg.mol
+    * htm.ureg.s**-1
+    * htm.ureg.m**-1
+    * htm.ureg.Pa**-0.5,
+    isotope="H",
+    source="lee_hydrogen_2011",
+)
+
+lee_diffsol_data = np.genfromtxt(
+    str(Path(__file__).parent) + "/lee_2011/diffusivity_solubility.csv",
+    delimiter=",",
+    names=True,
+)
+lee_data_invT = lee_diffsol_data["diffusivityX"] * htm.ureg.K**-1
+lee_diffusivity = Diffusivity(
+    data_T=1 / lee_data_invT,
+    data_y=lee_diffsol_data["diffusivityY"] * htm.ureg.m**2 * htm.ureg.s**-1,
+    isotope="H",
+    source="lee_hydrogen_2011",
+)
+lee_data_invT = lee_diffsol_data["solubilityX"] * htm.ureg.K**-1
+lee_solubility = Solubility(
+    units="m-3 Pa-1/2",
+    data_T=1 / lee_data_invT,
+    data_y=lee_diffsol_data["solubilityY"]
+    * htm.ureg.mol
+    * htm.ureg.m**-3
+    * htm.ureg.Pa**-0.5,
+    isotope="H",
+    source="lee_hydrogen_2011",
+)
 
 properties = [
     reiter_diffusivity,
     reiter_solubility,
     houben_permeability,
     kishimoto_permeability,
     kishimoto_diffusivity,
@@ -196,13 +236,16 @@
     esteban_dissociation_coeff_oxidised,
     esteban_recombination_coeff_oxidised,
     forcey_permeability,
     forcey_diffusivity,
     forcey_solubility,
     xiukui_permeability,
     xiukui_diffusivity,
+    lee_permeability,
+    lee_diffusivity,
+    lee_solubility,
 ]
 
 for prop in properties:
-    prop.material = "steel_316l"
+    prop.material = htm.STEEL_316L
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/tantalum.py` & `h_transport_materials-0.9/h_transport_materials/property_database/tantalum.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,10 +19,10 @@
     range=(623 * htm.ureg.K, 904 * htm.ureg.K),
     source="veleckis_thermodynamic_1969",
 )
 
 properties = [volkl_diffusivity, veleckis_solubility]
 
 for prop in properties:
-    prop.material = "tantalum"
+    prop.material = htm.TANTALUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/titanium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/titanium.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     isotope="T",
     source="reiter_compilation_1996",
 )
 
 properties = [reiter_diffusivity, reiter_solubility]
 
 for prop in properties:
-    prop.material = "titanium"
+    prop.material = htm.TITANIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/tungsten.py` & `h_transport_materials-0.9/tests/test_properties_group.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,195 @@
 import h_transport_materials as htm
-from h_transport_materials.property import Diffusivity, RecombinationCoeff, Solubility
-
-frauenfelder_src = "frauenfelder_solution_1969"
-frauenfelder_diffusivity = Diffusivity(
-    D_0=4.1e-7 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.39 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(1100 * htm.ureg.K, 2400 * htm.ureg.K),
-    source=frauenfelder_src,
-    name="Frauenfelder (1969)",
-    isotope="H",
-)
-frauenfelder_solubility = Solubility(
-    S_0=1.87e24 * htm.ureg.particle * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=1.04 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(1100 * htm.ureg.K, 2400 * htm.ureg.K),
-    source=frauenfelder_src,
-    name="Frauenfelder (1969)",
-    isotope="H",
-    units="m-3 Pa-1/2",
-)
-
-
-liu_src = "liu_hydrogen_2014"
-liu_diffusivity_tungsten = Diffusivity(
-    D_0=5.13e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.21 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(200 * htm.ureg.K, 3000 * htm.ureg.K),
-    source=liu_src,
-    name="H Liu (2014)",
-    isotope="H",
-)
-
-
-heinola_src = "heinola_diffusion_2010"
-heinola_diffusivity_tungsten = Diffusivity(
-    D_0=5.2e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.21 * htm.ureg.eV * htm.ureg.particle**-1,
-    source=heinola_src,
-    name="H Heinola (2010)",
-    isotope="H",
-)
-
-johnson_src = "johnson_hydrogen_2010"
-johnson_diffusivity_tungsten_h = Diffusivity(
-    D_0=6.32e-7 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.39 * htm.ureg.eV * htm.ureg.particle**-1,
-    source=johnson_src,
-    name="H Johnson (2010)",
-    isotope="H",
-)
-
-johnson_diffusivity_tungsten_t = Diffusivity(
-    D_0=5.16e-7 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.40 * htm.ureg.eV * htm.ureg.particle**-1,
-    source=johnson_src,
-    name="T Johnson (2010)",
-    isotope="T",
-)
-
-
-moore_diffusivity_tungsten_t = Diffusivity(
-    D_0=7.2e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=173.7 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(1510 * htm.ureg.K, 1902 * htm.ureg.K),
-    source="moore_adsorptiondesorption_1964",
-    name="T Moore (1964)",
-    isotope="T",
-)
-
-
-zakharov_diffusivity_tungsten_h = Diffusivity(
-    D_0=6.0e-4 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=103.4 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(400 * htm.ureg.K, 1200 * htm.ureg.K),
-    source="zakharov_hydrogen_1975",
-    name="H Zakharov (1973)",
-    isotope="H",
-)
-
-ryabchikov_diffusivity_tungsten_h = Diffusivity(
-    D_0=8.1e-6 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=82.9 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(1055 * htm.ureg.K, 1570 * htm.ureg.K),
-    source="ryabchikov_notitle_1964",
-    name="H Ryabchikov (1964)",
-    isotope="H",
-)
-
-esteban_src = "esteban_hydrogen_2001"
-esteban_diffusivity_tungsten_h = Diffusivity(
-    D_0=5.68e-10 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=9.3 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="H Esteban (2001)",
-    isotope="H",
-)
-
-esteban_diffusivity_tungsten_d = Diffusivity(
-    D_0=5.49e-10 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=10 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="D Esteban (2001)",
-    isotope="D",
-)
-
-esteban_diffusivity_tungsten_t = Diffusivity(
-    D_0=5.34e-10 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=11.2 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="T Esteban (2001)",
-    isotope="T",
-)
-
-
-esteban_solubility_tungsten_h = Solubility(
-    S_0=2.9e-2 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=26.9 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="H Esteban (2001)",
-    isotope="H",
-    units="m-3 Pa-1/2",
-)
-
-esteban_solubility_tungsten_d = Solubility(
-    S_0=0.75e-2 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=28.7 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="D Esteban (2001)",
-    isotope="D",
-    units="m-3 Pa-1/2",
-)
-
-esteban_solubility_tungsten_t = Solubility(
-    S_0=2.25e-2 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=27.8 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(673 * htm.ureg.K, 1073 * htm.ureg.K),
-    source=esteban_src,
-    name="T Esteban (2001)",
-    isotope="T",
-    units="m-3 Pa-1/2",
-)
-
-holzner_src = "holzner_solute_2020"
-holzner_diffusivity_tungsten_h = Diffusivity(
-    D_0=2.06e-3 * htm.ureg.cm**2 * htm.ureg.s**-1,
-    E_D=0.28 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(1600 * htm.ureg.K, 2600 * htm.ureg.K),
-    source=holzner_src,
-    name="H Holzner (2020)",
-    isotope="H",
-)
-holzner_diffusivity_tungsten_d = Diffusivity(
-    D_0=1.60e-3 * htm.ureg.cm**2 * htm.ureg.s**-1,
-    E_D=0.28 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(1600 * htm.ureg.K, 2600 * htm.ureg.K),
-    source=holzner_src,
-    name="D Holzner (2020)",
-    isotope="D",
-)
-
-fernandez_diffusivity_tungsten_h = Diffusivity(
-    D_0=1.93e-7 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=0.20 * htm.ureg.eV * htm.ureg.particle**-1,
-    range=(300 * htm.ureg.K, 1200 * htm.ureg.K),
-    name="H Fernandez (2015)",
-    source="fernandez_hydrogen_2015",
-    isotope="H",
-)
-
-anderl_recomb = RecombinationCoeff(
-    pre_exp=3.2e-15 * htm.ureg.m**4 * htm.ureg.s**-1 * htm.ureg.particle**-1,
-    act_energy=1.16 * htm.ureg.eV * htm.ureg.particle**-1,
-    isotope="D",
-    source="anderl_deuterium_1992",
-)
-
-properties = [
-    frauenfelder_diffusivity,
-    liu_diffusivity_tungsten,
-    heinola_diffusivity_tungsten,
-    johnson_diffusivity_tungsten_h,
-    johnson_diffusivity_tungsten_t,
-    moore_diffusivity_tungsten_t,
-    zakharov_diffusivity_tungsten_h,
-    ryabchikov_diffusivity_tungsten_h,
-    esteban_diffusivity_tungsten_h,
-    esteban_diffusivity_tungsten_d,
-    esteban_diffusivity_tungsten_t,
-    holzner_diffusivity_tungsten_h,
-    holzner_diffusivity_tungsten_d,
-    fernandez_diffusivity_tungsten_h,
-    frauenfelder_solubility,
-    esteban_solubility_tungsten_h,
-    esteban_solubility_tungsten_d,
-    esteban_solubility_tungsten_t,
-    anderl_recomb,
-]
-
-for prop in properties:
-    prop.material = "tungsten"
-
-htm.database += properties
+import numpy as np
+import json
+import pytest
+from pybtex.database import BibliographyData
+
+
+def test_iterable():
+    """Checks that PropertiesGroup can be iterated through"""
+    my_group = htm.PropertiesGroup(htm.Property() for _ in range(10))
+
+    for prop in my_group:
+        assert isinstance(prop, htm.Property)
+
+
+def test_adding_two_groups():
+    """Checks two groups can be added"""
+    my_group1 = htm.PropertiesGroup(htm.Property() for _ in range(10))
+    my_group2 = htm.PropertiesGroup(htm.Property() for _ in range(10))
+
+    sum_of_groups = my_group1 + my_group2
+    assert len(sum_of_groups) == len(my_group1) + len(my_group2)
+
+
+def test_filter_author_lower_case():
+    """Checks that PropertiesGroup can filter authors even
+    if the attributes are not lowercase"""
+
+    my_prop = htm.Property(author="ReM")
+
+    my_group = htm.PropertiesGroup([my_prop])
+
+    filtered_group = my_group.filter(author="rem")
+
+    assert filtered_group[0] == my_prop
+
+
+def test_filter_isotope_lower_case():
+    """Checks that PropertiesGroup can filter isotopes even
+    if the attributes are not lowercase"""
+
+    my_prop = htm.Property(isotope="H")
+
+    my_group = htm.PropertiesGroup([my_prop])
+
+    filtered_group = my_group.filter(isotope="h")
+
+    assert filtered_group[0] == my_prop
+
+
+@pytest.mark.parametrize(
+    "mean_D_0,mean_E_D",
+    [
+        (D_0, E_D)
+        for D_0 in np.linspace(2, 60, num=3)
+        for E_D in np.linspace(0.1, 3, num=3)
+    ],
+)
+def test_mean(mean_D_0, mean_E_D):
+    """Creates a PropertiesGroup object with a list of properties that
+    have their activation energy and pre-exponential factor varying
+    around mean values. The method .mean() is called and the computed
+    mean values are compared with the theoretical ones.
+
+    Args:
+        mean_D_0 (float): mean pre-exponential factor
+        mean_E_D (float): mean activation energy
+    """
+    # build
+    my_group = htm.PropertiesGroup()
+    nb_props = 30
+
+    noise_D_0 = np.random.normal(0, mean_D_0 / 10, nb_props)
+    noise_E_D = np.random.normal(0, mean_E_D / 10, nb_props)
+
+    # create properties with noise
+    for i in range(nb_props):
+        my_group.append(
+            htm.ArrheniusProperty(
+                pre_exp=(mean_D_0 + noise_D_0[i]) * htm.ureg.m**2 * htm.ureg.s**-1,
+                act_energy=(mean_E_D + noise_E_D[i])
+                * htm.ureg.eV
+                * htm.ureg.particle**-1,
+            )
+        )
+
+    # run
+    mean_prop = my_group.mean()
+
+    # test
+    assert mean_prop.pre_exp == pytest.approx(mean_D_0, rel=0.2)
+    assert mean_prop.act_energy.magnitude == pytest.approx(mean_E_D, rel=0.2)
+
+
+def test_mean_is_type_arrhenius_property():
+    my_prop = htm.ArrheniusProperty(
+        0.1 * htm.ureg.dimensionless, 0.1 * htm.ureg.eV * htm.ureg.particle**-1
+    )
+    my_group = htm.PropertiesGroup([my_prop])
+
+    assert isinstance(my_group.mean(), htm.ArrheniusProperty)
+
+
+def test_bibdata():
+    source_bib = """@article{article-minimal,
+        author = "L[eslie] B. Lamport",
+        title = "The Gnats and Gnus Document Preparation System",
+        journal = "G-Animal's Journal",
+        year = "1986"
+    }
+    """
+
+    my_group = htm.PropertiesGroup(
+        [
+            htm.Property(material="my_mat", source=source_bib),
+            htm.Property(material="my_mat", source="source"),
+        ]
+    )
+
+    assert isinstance(my_group.bibdata, BibliographyData)
+
+
+def test_export_bib():
+    source_bib = """@article{article-minimal,
+        author = "L[eslie] B. Lamport",
+        title = "The Gnats and Gnus Document Preparation System",
+        journal = "G-Animal's Journal",
+        year = "1986"
+    }
+    """
+
+    my_group = htm.PropertiesGroup(
+        [
+            htm.Property(material="my_mat", source=source_bib),
+            htm.Property(material="my_mat", source="source"),
+        ]
+    )
+    my_group.export_bib("out.bib")
+
+
+def test_export_to_json():
+    # build
+
+    my_group = htm.database
+
+    # run
+
+    my_group.export_to_json("out.json")
+
+    # test
+    with open("out.json") as json_file:
+        data_in = json.load(json_file)
+
+    for prop_file, prop_ref in zip(data_in, my_group):
+        for key, val in prop_file.items():
+            if hasattr(prop_ref, key):
+                if isinstance(val, list):
+                    if key == "range":
+                        prop_range = getattr(prop_ref, key)
+                        assert [prop_range[0].magnitude, prop_range[1].magnitude] == val
+                    else:
+                        for item1, item2 in zip(val, getattr(prop_ref, key)):
+                            assert item1 == item2
+                else:
+                    if key == "units":
+                        assert f"{getattr(prop_ref, key):~}" == val
+                    elif key in ["pre_exp", "act_energy"]:
+                        assert getattr(prop_ref, key).magnitude == val
+                    else:
+                        assert getattr(prop_ref, key) == val
+
+
+def test_filter_warns_when_no_props():
+    with pytest.warns(UserWarning):
+        htm.diffusivities.filter(material="material_that_doesn_not_exist")
+
+
+def test_units_property():
+    """Checks the units property returns the expected value"""
+    diff = htm.Diffusivity(
+        D_0=1 * htm.ureg.m**2 * htm.ureg.s**-1,
+        E_D=0.1 * htm.ureg.eV * htm.ureg.particle**-1,
+    )
+    sol = htm.Solubility(
+        units="m-3 Pa-1",
+        S_0=1 * htm.ureg.particle * htm.ureg.m**-3 * htm.ureg.Pa**-1,
+        E_S=0.1 * htm.ureg.eV * htm.ureg.particle**-1,
+    )
+
+    assert (
+        htm.PropertiesGroup([sol, sol]).units
+        == htm.ureg.particle * htm.ureg.m**-3 * htm.ureg.Pa**-1
+    )
+    assert htm.PropertiesGroup([diff, diff]).units == htm.ureg.m**2 * htm.ureg.s**-1
+    assert htm.PropertiesGroup([sol, diff]).units == "mixed units"
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/vanadium.py` & `h_transport_materials-0.9/h_transport_materials/property_database/zirconium/zirconium.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 import h_transport_materials as htm
 from h_transport_materials import Diffusivity, Solubility
-import h_transport_materials.conversion as c
 
-VANADIUM_MOLAR_VOLUME = 8.34e-6  # m3/mol  https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/vanadium
+import numpy as np
+from pathlib import Path
 
-volk_diffusivity = Diffusivity(
-    D_0=2.9e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=4.2 * htm.ureg.kJ * htm.ureg.mol**-1,
+
+ZIRCONIUM_MOLAR_VOLUME = 1.4e-5  # m3/mol https://www.aqua-calc.com/calculate/mole-to-volume-and-weight/substance/zirconium
+
+kearns_diffusivity = Diffusivity(
+    D_0=7.73e-3 * htm.ureg.cm**2 * htm.ureg.s**-1,
+    E_D=10.830 * htm.ureg.kcal * htm.ureg.mol**-1,
+    range=(548 * htm.ureg.K, 973 * htm.ureg.K),
     isotope="H",
-    source="volkl_5_1975",
-    range=(173 * htm.ureg.K, 573 * htm.ureg.K),
+    source="kearns_diffusion_1972",
+)
+
+hsu_diffusivity = Diffusivity(
+    D_0=2.7e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
+    E_D=24.9 * htm.ureg.kJ * htm.ureg.mol**-1,
+    isotope="T",
+    source="hsu_palladium-catalyzed_1986",
 )
 
-veleckis_solubility = Solubility(
+kearns_solubility = Solubility(
     units="m-3 Pa-1/2",
+    S_0=4.30e-1 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
+    E_S=-49.5 * htm.ureg.kJ * htm.ureg.mol**-1,
     isotope="H",
-    range=(519 * htm.ureg.K, 827 * htm.ureg.K),
-    S_0=1.38e-1 * htm.ureg.mol * htm.ureg.m**-3 * htm.ureg.Pa**-0.5,
-    E_S=-29.0 * htm.ureg.kJ * htm.ureg.mol**-1,
-    source="veleckis_thermodynamic_1969",
+    source="kearns_terminal_1967",
+    range=(602 * htm.ureg.K, 1069 * htm.ureg.K),
+    note="this was found in Shimada 2020 review 'Tritium Transport in Fusion Reactor Materials'"
+    + "however, I can't find this activation energy in Kearns paper",
 )
 
-schober_diffusivity = Diffusivity(
-    D_0=5.6e-8 * htm.ureg.m**2 * htm.ureg.s**-1,
-    E_D=9.1 * htm.ureg.kJ * htm.ureg.mol**-1,
-    range=(
-        htm.ureg.Quantity(-150, htm.ureg.degC),
-        htm.ureg.Quantity(200, htm.ureg.degC),
-    ),
-    source="schober_h_1990",
-    isotope="H",
-    note="found in Assessment of Database for Interaction of Tritium with ITER Plasma Facing Materials",
-)  # TODO get data from experimental points, see issue #64
+yamanaka_solubility_data = np.genfromtxt(
+    str(Path(__file__).parent) + "/yamanaka_1989/solubility.csv",
+    delimiter=",",
+)
 
-reiter_solubility = Solubility(
+yamanaka_solubility = Solubility(
     units="m-3 Pa-1/2",
-    S_0=2.1e-6
-    / VANADIUM_MOLAR_VOLUME
+    data_T=1e4 / yamanaka_solubility_data[:, 0] * htm.ureg.K,
+    data_y=np.exp(yamanaka_solubility_data[:, 1])
+    / ZIRCONIUM_MOLAR_VOLUME
     * htm.ureg.mol
     * htm.ureg.m**-3
     * htm.ureg.Pa**-0.5,
-    E_S=-32.2 * htm.ureg.kJ * htm.ureg.mol**-1,
-    source="reiter_compilation_1996",
+    source="yamanaka_effect_1989",
     isotope="H",
 )
 
-properties = [volk_diffusivity, veleckis_solubility]
+properties = [
+    kearns_diffusivity,
+    hsu_diffusivity,
+    kearns_solubility,
+    yamanaka_solubility,
+]
 
 for prop in properties:
-    prop.material = "vanadium"
+    prop.material = htm.ZIRCONIUM
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/vanadium_alloy.py` & `h_transport_materials-0.9/h_transport_materials/property_database/vanadium_alloy.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     source="klepikov_hydrogen_2000",
     note="taken from Table 2",
 )
 
 properties = [hashizume_diffusivity, klepikov_solubility]
 
 for prop in properties:
-    prop.material = "v4cr4ti"
+    prop.material = htm.V4CR4TI
 
 htm.database += properties
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/materials/zirconium/yamanaka_1989/yamanaka_1989.tar` & `h_transport_materials-0.9/h_transport_materials/property_database/zirconium/yamanaka_1989/yamanaka_1989.tar`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/plotting.py` & `h_transport_materials-0.9/h_transport_materials/plotting.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/h_transport_materials/properties_group.py` & `h_transport_materials-0.9/h_transport_materials/properties_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         for prop in self:
 
             prop_dict = {key: getattr(prop, key) for key in keys if hasattr(prop, key)}
             if "units" in prop_dict:
                 prop_dict["units"] = f"{prop_dict['units']:~}"
             prop_dict["pre_exp"] = prop_dict["pre_exp"].magnitude
             prop_dict["act_energy"] = prop_dict["act_energy"].magnitude
+            prop_dict["material"] = prop_dict["material"].name
             if prop_dict["range"]:
                 prop_dict["range"] = (
                     prop_dict["range"][0].magnitude,
                     prop_dict["range"][1].magnitude,
                 )
             data.append(prop_dict)
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/property.py` & `h_transport_materials-0.9/h_transport_materials/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         self.data_T = data_T
         self.data_y = data_y
         super().__init__(**kwargs)
 
     def __str__(self) -> str:
         val = f"""
         Author: {self.author.capitalize()}
-        Material: {self.material}
+        Material: {self.material.name}
         Year: {self.year}
         Isotope: {self.isotope}
         Pre-exponential factor: {self.pre_exp:.2e~P}
         Activation energy: {self.act_energy:.2e~P}
         """
         return val
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials/references.bib` & `h_transport_materials-0.9/h_transport_materials/references.bib`

 * *Files 2% similar despite different names*

```diff
@@ -1817,15 +1817,15 @@
 	language = {en},
 	number = {7},
 	urldate = {2023-01-17},
 	journal = {Fusion Engineering and Design},
 	author = {Okitsu, Hiroaki and Edao, Yuki and Okada, Makoto and Fukada, Satoshi},
 	month = aug,
 	year = {2012},
-	keywords = {Diffusivity, Isotope effects, Lead–lithium, Liquid blanket, Permeability, Solubility},
+	keywords = {Solubility, Diffusivity, Permeability, Liquid blanket, Isotope effects, Lead–lithium},
 	pages = {1324--1328},
 	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\FPH2LKWX\\Okitsu et al. - 2012 - Analysis of diffusion and dissolution of two-compo.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\6P9JE23V\\S0920379612002074.html:text/html},
 }
 
 @article{edao_permeation_2011,
 	title = {Permeation of {Two}-{Component} {Hydrogen} {Isotopes} in {Lithium}-{Lead} {Eutectic} {Alloy}},
 	volume = {60},
@@ -1857,7 +1857,263 @@
 	journal = {Materials Science and Engineering: A},
 	author = {Xiukui, Sun and Jian, Xu and Yiyi, Li},
 	month = jul,
 	year = {1989},
 	pages = {179--187},
 	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\J2DDAM6D\\Xiukui et al. - 1989 - Hydrogen permeation behaviour in austenitic stainl.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\VBLWBRZD\\0921509389908575.html:text/html},
 }
+
+@article{lee_hydrogen_2011,
+	title = {Hydrogen {Permeability}, {Diffusivity}, and {Solubility} of {SUS} {316L} {Stainless} {Steel} in the {Temperature} {Range} 400 to 800  {C} for {Fusion} {Reactor} {Applications}},
+	volume = {59},
+	url = {https://www.jkps.or.kr/journal/view.html?doi=10.3938/jkps.59.3019},
+	doi = {10.3938/jkps.59.3019},
+	abstract = {S. K. Lee, H. S. Kim, S. J. Noh, J. H. Han. J. Korean Phys. Soc. 2011;59:3019-23. https://doi.org/10.3938/jkps.59.3019},
+	language = {en},
+	number = {5},
+	urldate = {2023-01-20},
+	journal = {Journal of the Korean Physical Society},
+	author = {Lee, S. K. and Kim, H. S. and Noh, S. J. and Han, J. H.},
+	month = nov,
+	year = {2011},
+	note = {Publisher: The Korean Physical Society},
+	pages = {3019--3023},
+	file = {Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\IKM72TFG\\Lee et al. - 2011 - Hydrogen Permeability, Diffusivity, and Solubility.pdf:application/pdf},
+}
+
+@article{eichenauer_notitle_1961,
+	volume = {52},
+	journal = {Z. Metallkd.},
+	author = {Eichenauer, W. and Hattenbach, Karl and Pebler, Alfred},
+	year = {1961},
+	pages = {682},
+}
+
+@article{cochran_permeability_1961,
+	title = {The {Permeability} of {Aluminum} to {Hydrogen}},
+	volume = {108},
+	issn = {1945-7111},
+	url = {https://iopscience.iop.org/article/10.1149/1.2428079/meta},
+	doi = {10.1149/1.2428079},
+	language = {en},
+	number = {4},
+	urldate = {2023-01-20},
+	journal = {Journal of The Electrochemical Society},
+	author = {Cochran, C. N.},
+	month = apr,
+	year = {1961},
+	note = {Publisher: IOP Publishing},
+	pages = {317},
+	file = {Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\AJ8BPYAW\\Cochran - 1961 - The Permeability of Aluminum to Hydrogen.pdf:application/pdf},
+}
+
+@article{song_study_1997,
+	title = {A study of hydrogen permeation in aluminum alloy treated by various oxidation processes},
+	volume = {246},
+	issn = {0022-3115},
+	url = {https://www.sciencedirect.com/science/article/pii/S0022311597001463},
+	doi = {10.1016/S0022-3115(97)00146-3},
+	abstract = {A set of oxide coatings was formed on the surface of an Al alloy (wt\%: Fe, 0.24; Si, 1.16; Cu, 0.05–0.2; Zn, 0.1; Al, residual) by means of various oxidation processes. The hydrogen permeability through the aluminum alloy and its coating materials was determined by a vapor phase permeation technique at temperatures ranging from 400 to 500°C using high-purity H2 (99.9999\%) gas with an upstream hydrogen pressure of 104−105 Pa. The experimental results show that the hydrogen permeability through aluminum oxide coating is 100–2000 times lower than that through the aluminum alloy substrate. This means that the aluminum oxide is a significant hydrogen permeation barrier. A high hydrogen permeation resistance was observed in an oxide layer prefilmed in 200°C water, while an anodized aluminum oxide film had a less obstructive effect, possibly caused by the porous structure of the anodic oxide. The hydrogen permeability through films of aluminum oxide was not a simple function of the aluminum-oxide phase configuration.},
+	language = {en},
+	number = {2},
+	urldate = {2023-01-20},
+	journal = {Journal of Nuclear Materials},
+	author = {Song, Wenhai and Du, Jiaju and Xu, Yongli and Long, Bin},
+	month = aug,
+	year = {1997},
+	keywords = {66.30.J, pacs:28.52.F},
+	pages = {139--143},
+	file = {ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\PWF6VTFT\\S0022311597001463.html:text/html},
+}
+
+@article{saitoh_hydrogen_1994,
+	title = {Hydrogen diffusivity in aluminium measured by a glow discharge permeation method},
+	volume = {42},
+	issn = {0956-7151},
+	url = {https://www.sciencedirect.com/science/article/pii/0956715194903298},
+	doi = {10.1016/0956-7151(94)90329-8},
+	abstract = {The diffusion coefficient of hydrogen in aluminium has been determined in the temperature range between 446 and 681 K by a glow discharge permeation method which enables us to extend the temperature range of measurements by enhancement of the permeation flux in spite of the small equilibrium solubility of hydrogen in solid aluminium. The temperature dependence of the diffusion coefficient of hydrogen in aluminium shows a linear Arrhenius relationship with the pre-exponential factor (6.1 ± 0.5) × 10−5 m2 s−1 and with the activation energy (54.8 ± 0.4) kJmol−1. These values are higher than those estimated by several previous authors with hydrogen evolution techniques in high temperature regions. However, the present values are well consistent with the results by Ishikawa and McLellan using an electrolytic permeation method around room temperature, suggesting that hydrogen atoms in aluminium diffuse by the interstitial mechanism in the whole temperature range.},
+	language = {en},
+	number = {7},
+	urldate = {2023-01-20},
+	journal = {Acta Metallurgica et Materialia},
+	author = {Saitoh, Hideyuki and Iijima, Yoshiaki and Tanaka, Hiroshi},
+	month = jul,
+	year = {1994},
+	pages = {2493--2498},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\YH72Y4BN\\Saitoh et al. - 1994 - Hydrogen diffusivity in aluminium measured by a gl.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\YVQG9R5D\\0956715194903298.html:text/html},
+}
+
+@article{hashimoto_hydrogen_1983,
+	title = {Hydrogen diffusion in aluminium at high temperatures},
+	volume = {13},
+	issn = {0305-4608},
+	url = {https://dx.doi.org/10.1088/0305-4608/13/6/013},
+	doi = {10.1088/0305-4608/13/6/013},
+	abstract = {The diffusion of hydrogen in aluminium has been measured by the permeation method using a quadrupole mass spectrometer. Hydrogen was introduced by gas phase charging in the temperature range of 300-400 degrees C, and by electrochemical charging at room temperature. It was found that the diffusivity of hydrogen depends on the relative concentration of vacancies to the dissolved hydrogen concentration. The activation energy for the diffusion of hydrogen was found to be 0.61-0.62 eV at high temperatures where the concentration of vacancies was much higher than that of dissolved hydrogen. The value is near the migration energy of a vacancy in aluminium. On the other hand, at room temperature where the hydrogen showed a diffusivity considerably larger than that extrapolated from high temperatures. These facts suggest that hydrogen in aluminium migrates together with a vacancy at high temperatures due to a large binding energy between them.},
+	language = {en},
+	number = {6},
+	urldate = {2023-01-20},
+	journal = {Journal of Physics F: Metal Physics},
+	author = {Hashimoto, E. and Kino, T.},
+	month = jun,
+	year = {1983},
+	pages = {1157},
+	file = {IOP Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\2RTB7R39\\Hashimoto and Kino - 1983 - Hydrogen diffusion in aluminium at high temperatur.pdf:application/pdf},
+}
+
+@article{ichimura_grain_1991,
+	title = {Grain {Boundary} {Effect} on {Diffusion} of {Hydrogen} in {Pure} {Aluminum}},
+	volume = {32},
+	doi = {10.2320/matertrans1989.32.1109},
+	abstract = {Hydrogen diffusivity and solubility in pure solid aluminum were measured in a high temperature range from 573 to 923 K, by means of a desorption technique, which was an outgassing study from thermally hydrogen-charged cylindrical samples with various grain sizes. The diffusion coefficient depended linearly upon an inverse of temperature in the Arrhenius plot. There were two characteristics in the plot; one of them was a change of apparent activation energy for diffusion being a fixed diffusivity at about 900 K, while another was a correlation between the increase of activation energy and the decrease of grain size. We proposed a simple model for grain size dependence of the hydrogen diffusivity. The decrease in diffusivity at a lower temperature for the smaller grain size was explained by trapping of hydrogen at nodes of grain boundaries. In a very large grain size, there was a possibility of a fast diffusion along the grain boundary. The increase in solubility usually expected from a trapping process was not found in this study.},
+	number = {12},
+	journal = {Materials Transactions, JIM},
+	author = {Ichimura, Minoru and Sasajima, Yasushi and Imabayashi, Mamoru},
+	year = {1991},
+	keywords = {aluminum, diffusivity, enhanced diffusion, grain boundary, hydrogen, solubility, trapping},
+	pages = {1109--1114},
+	file = {Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\NEBBP679\\Ichimura et al. - 1991 - Grain Boundary Effect on Diffusion of Hydrogen in .pdf:application/pdf;J-Stage - Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\MDGU7WEX\\ja.html:text/html},
+}
+
+@article{outlaw_diffusion_1982,
+	title = {Diffusion of hydrogen in pure large grain aluminum},
+	volume = {16},
+	issn = {0036-9748},
+	url = {https://www.sciencedirect.com/science/article/pii/0036974882903544},
+	doi = {10.1016/0036-9748(82)90354-4},
+	abstract = {The solubility of hydrogen at 600°C and the diffusion rate at a given temperature were both found to be lower than reported previously. The activation energy for diffusion was nearly the same as in several earlier reports indicating that diffusion was the rate controlling step in all cases. Hydrogen diffusion in large grained high purity aluminum followed the expression: D = 1.01 × 10−5 (m2/sec) exp − 47.7 kJ/RT.},
+	language = {en},
+	number = {3},
+	urldate = {2023-01-20},
+	journal = {Scripta Metallurgica},
+	author = {Outlaw, R. A. and Peterson, D. T. and Schmidt, F. A.},
+	month = mar,
+	year = {1982},
+	pages = {287--292},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\XIT24QWK\\Outlaw et al. - 1982 - Diffusion of hydrogen in pure large grain aluminum.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\F59XSU66\\0036974882903544.html:text/html},
+}
+
+@article{ishikawa_diffusivity_1986,
+	title = {The diffusivity of hydrogen in aluminum},
+	volume = {34},
+	issn = {0001-6160},
+	url = {https://www.sciencedirect.com/science/article/pii/0001616086902191},
+	doi = {10.1016/0001-6160(86)90219-1},
+	abstract = {Using an electrolytic method employing a viscous electrolyte, the diffusivity of hydrogen in aluminum has been measured in the temperature range 285–328 K. The results show that H diffuses by a single-stage process from 285 K up to the melting temperature and no departures from Arrhenius behavior due to trapping effects involving lattice vacancies are observed.
+Résumé
+Nous avons mesuré la diffusivité de l'hydrogène dans l'aluminium entre 285 et 328 K, par une méthode électrolytique utilisant une électrolyte visqueux. Nos résultats montrent que l'hydrogène diffuse par un mécanisme à stade unique de 285 K jusqu'à la température de fusion; l'on n'observe pas d'écart par rapport à un comportement d'Arrhenius, écart qui serait dû à des effets de piègeage mettant en jeu des lacunes.
+Zusammenfassung
+Mit einer elektrolytischen Methode wurde die Diffusivität von Wasserstoff in Aluminium im Temperaturbereich zwischen 285 und 328 K in einem viskosen Elektrolyten gemessen. Aus den Ergebnissen folgt, daβ H über einen einstufigen Prozeβ zwischen 285 K und der Schmelztemperatur diffundiert. Abweichungen vom Arrhenius-Verhalten durch Einfangeffekte an Gitterleerstellen werden nicht beobachtet.},
+	language = {en},
+	number = {6},
+	urldate = {2023-01-20},
+	journal = {Acta Metallurgica},
+	author = {Ishikawa, T. and McLellan, R. B.},
+	month = jun,
+	year = {1986},
+	pages = {1091--1095},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\BIEPC6FH\\Ishikawa and McLellan - 1986 - The diffusivity of hydrogen in aluminum.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\REBNCUJ8\\0001616086902191.html:text/html},
+}
+
+@article{addach_hydrogen_2005,
+	title = {Hydrogen permeation in iron at different temperatures},
+	volume = {59},
+	issn = {0167-577X},
+	url = {https://www.sciencedirect.com/science/article/pii/S0167577X04009814},
+	doi = {10.1016/j.matlet.2004.12.037},
+	abstract = {The electrochemical hydrogen permeation method is used to determine the effective diffusivity, permeation rate and apparent solubility of hydrogen in pure iron at different temperatures. The experimental results reveal that the temperature of permeation experiment is influenced, in accordance with the literature. Furthermore, it is also shown that the steady-state current is influenced by a variation of the temperature. In a second step, a gas chromatography system is used to determine quantitatively the amount of hydrogen thermally desorbed.},
+	language = {en},
+	number = {11},
+	urldate = {2023-01-20},
+	journal = {Materials Letters},
+	author = {Addach, H. and Berçot, P. and Rezrazi, M. and Wery, M.},
+	month = may,
+	year = {2005},
+	keywords = {Desorption, Diffusion, Hydrogen embrittlement, Hydrogen permeation, Iron},
+	pages = {1347--1351},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\8P4456NF\\Addach et al. - 2005 - Hydrogen permeation in iron at different temperatu.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\VVJ2HGQ8\\S0167577X04009814.html:text/html},
+}
+
+@article{masui_hydrogen_1978,
+	title = {Hydrogen {Permeation} through {Iron}, {Nickel}, and {Heat} {Resisting} {Alloys} at {Elevated} {Temperatures}},
+	volume = {64},
+	doi = {10.2355/tetsutohagane1955.64.5_615},
+	abstract = {Hydrogen permeabilities of several metals and alloys were measured over the temperature range of 200-1000°C and some factors affecting the hydrogen permeability were discussed. Materials studied were iron, nickel, 80Ni-20Cr alloy, 50Fe-30Ni-20Cr alloy, HK 40, Incoloy 800, Hastelloy X, and Inconel 600. The hydrogen permeability of nickel was proportional to the square root of the pressure and inversely proportional to the membrane thickness. The activation energy and pre-exponential factor for the hydrogen permeation through these metals and alloys were derived from the temperature coefficient. The hydrogen permeability of nickel was larger than that of iron (γ), and the permeabilities of the heat resisting alloys were between those of nickel and iron (γ). There was a close correlation between the hydrogen permeability and nickel content in the alloys, that is, the permeability increased with the increase of the nickel content in the alloys. The formation of the oxide film on the alloy surface in wet hydrogen resulted in a remarkable reduction of the hydrogen permeability at elevated temperatures.},
+	number = {5},
+	journal = {Tetsu-to-Hagane},
+	author = {Masui, Kanji and Yoshida, Heitaro and Watanabe, Yoji},
+	year = {1978},
+	pages = {615--620},
+	file = {Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\PZBZVQEF\\Masui et al. - 1978 - Hydrogen Permeation through Iron, Nickel, and Heat.pdf:application/pdf;J-Stage - Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\3ZB5SP5H\\_article.html:text/html},
+}
+
+@article{frauenfelder_permeation_1968,
+	title = {Permeation of {Hydrogen} through {Tungsten} and {Molybdenum}},
+	volume = {48},
+	issn = {0021-9606},
+	url = {https://aip.scitation.org/doi/10.1063/1.1669720},
+	doi = {10.1063/1.1669720},
+	number = {9},
+	urldate = {2023-01-20},
+	journal = {The Journal of Chemical Physics},
+	author = {Frauenfelder, R.},
+	month = may,
+	year = {1968},
+	note = {Publisher: American Institute of Physics},
+	pages = {3955--3965},
+}
+
+@article{zhao_deuterium_2020,
+	title = {Deuterium {Permeation} {Behavior} in {Fe} {Ion} {Damaged} {Tungsten} {Studied} by {Gas}-{Driven} {Permeation} {Method}},
+	volume = {76},
+	issn = {1536-1055},
+	url = {https://doi.org/10.1080/15361055.2019.1705727},
+	doi = {10.1080/15361055.2019.1705727},
+	abstract = {The deuterium (D) permeation behavior for 1 displacement per atom Fe2+ damaged tungsten (W) was studied by the gas-driven permeation method and compared with undamaged W. The results of thermal desorption spectroscopy showed that dislocation loops and voids were formed in damaged W. It was found that the D permeation behavior in W was affected by irradiation defects. The effective diffusivity and permeability in the damaged W were lower than that in undamaged W. However, the difference in effective diffusivity and permeability between the undamaged sample and the damaged sample was reduced with increasing the heating temperature. Under 965 K, which was enough for D detrapping from voids, the permeability for damaged W was consistent with that for undamaged W.},
+	number = {3},
+	urldate = {2023-01-20},
+	journal = {Fusion Science and Technology},
+	author = {Zhao, Mingzhong and Nakata, Moeko and Sun, Fei and Hatano, Yuji and Someya, Yoji and Tobita, Kenji and Oya, Yasuhisa},
+	month = apr,
+	year = {2020},
+	note = {Publisher: Taylor \& Francis
+\_eprint: https://doi.org/10.1080/15361055.2019.1705727},
+	keywords = {gas-driven permeation, irradiation damage, Tungsten},
+	pages = {246--251},
+	file = {Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\F5EM4LLM\\Zhao et al. - 2020 - Deuterium Permeation Behavior in Fe Ion Damaged Tu.pdf:application/pdf},
+}
+
+@article{liang_deuterium_2018,
+	title = {Deuterium permeation behaviors in tungsten implanted with nitrogen},
+	volume = {505},
+	issn = {0022-3115},
+	url = {https://www.sciencedirect.com/science/article/pii/S0022311517314563},
+	doi = {10.1016/j.jnucmat.2018.04.021},
+	abstract = {Surface modification of tungsten due to the cooling species nitrogen seeded in the divertor region, i.e., by nitrogen ion implantation or re-deposition, is considered to affect the permeation behavior of H isotopes. This work focuses on the effect of nitrogen ion implantation into tungsten (W-N) on the deuterium gas-driven permeation behavior. For comparison, both permeation in tungsten implanted with W ion (W-W) and without implantation (pristine W) are studied. These three samples were characterized by scanning electron microscopy (SEM), X-ray diffraction (XRD), and X-ray photo-electron spectroscopy (XPS). The SEM results revealed that the W-W sample has various voids on the surface, and the W-N sample has a rough surface with pretty fine microstructures. These are different from the pristine W sample with a smooth and compact surface. The XRD patterns show the disappearance of crystallinity on both W-W and W-N sample surfaces. It indicates that the ion implantation process results in an almost complete conversion from crystalline to amorphous in the sample surfaces. The sputter-depth profiling XPS spectra show that the implanted nitrogen prefers to form a 140 nm thick tungsten nitride layer. In permeation experiments, it was found that the D permeability is temperature dependent. Interestingly, the W-N sample presented a lower D permeability than the W-W sample, but higher than the pristine W sample. Such behavior implies that tungsten nitride acts as a permeation barrier, while defects created by ions implantation can promote permeability. The possible permeation mechanism correlated with sample surface composition and microstructure is consequently discussed in this work.},
+	language = {en},
+	urldate = {2023-01-20},
+	journal = {Journal of Nuclear Materials},
+	author = {Liang, Chuan-hui and Wang, Dongping and Jin, Wei and Lou, Yuanfu and Wang, Wei and Ye, Xiaoqiu and Chen, Chang-an and Liu, Kezhao and Xu, Haiyan and Wang, Xiaoying and Kleyn, Aart W.},
+	month = jul,
+	year = {2018},
+	pages = {174--182},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\FRWHJTQG\\Liang et al. - 2018 - Deuterium permeation behaviors in tungsten implant.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\382BJEIS\\S0022311517314563.html:text/html},
+}
+
+@article{liu_gas-driven_2016,
+	title = {Gas-driven permeation of deuterium through tungsten with different microstructures},
+	volume = {113},
+	issn = {0920-3796},
+	url = {https://www.sciencedirect.com/science/article/pii/S0920379616305701},
+	doi = {10.1016/j.fusengdes.2016.09.003},
+	abstract = {Permeation behavior of deuterium (D) through various tungsten (W) materials, including rolled, annealed, recrystallized W and ZrC/La2O3-dispersion strengthened W, has been studied. Experiments were performed using a gas-driven permeation facility in the temperature range of 700–1000K. The permeability of D was not sensitive to the dislocations/vacancies or ZrC/La2O3 phases in W, and the measured permeation values are comparable to Frauenfelder and Zahkarov’s data. The diffusivity of D, however, is microstructure dependent. The higher the density of defects was, the lower the effective diffusivity was measured. These results imply that dislocations/vacancies or small amounts of ZrC/La2O3 phases in W will not influence the hydrogen isotopes steady state permeation flux through the first wall.},
+	language = {en},
+	urldate = {2023-01-20},
+	journal = {Fusion Engineering and Design},
+	author = {Liu, Feng and Zhou, Haishan and Xu, Yuping and Li, Xiao-Chun and Zhao, Mingzhong and Zhang, Tao and Xie, Zhuoming and Yan, Qing-Zhi and Zhang, Xiaoxin and Ding, Fang and Liu, Songlin and Luo, Guang-Nan},
+	month = dec,
+	year = {2016},
+	keywords = {Diffusion, Fusion materials, Hydrogen isotopes, Permeation, Tungsten},
+	pages = {216--220},
+	file = {ScienceDirect Full Text PDF:C\:\\Users\\remidm\\Zotero\\storage\\SMJBV2UT\\Liu et al. - 2016 - Gas-driven permeation of deuterium through tungste.pdf:application/pdf;ScienceDirect Snapshot:C\:\\Users\\remidm\\Zotero\\storage\\4YTC4I4G\\S0920379616305701.html:text/html},
+}
```

### Comparing `h_transport_materials-0.8.1/h_transport_materials.egg-info/PKG-INFO` & `h_transport_materials-0.9/h_transport_materials.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h-transport-materials
-Version: 0.8.1
+Version: 0.9
 Summary: Handle H transport properties
 Home-page: https://github.com/RemDelaporteMathurin/h_transport_materials
 Author: Remi Delaporte-Mathurin
 Author-email: rdelaportemathurin@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/RemDelaporteMathurin/h_transport_materials
 Project-URL: Tracker, https://github.com/RemDelaporteMathurin/h_transport_materials/issues
@@ -55,15 +55,16 @@
 
 
 plt.yscale("log")
 plt.ylabel("Diffusivity (m$^2$/s)")
 plt.legend()
 plt.show()
 ```
-![Figure_1](https://user-images.githubusercontent.com/40028739/169280320-c4d45d9b-7f33-4628-a4fd-72e81be16124.svg)
+![Figure_1](https://user-images.githubusercontent.com/40028739/213814746-9dadb8dc-599e-4004-8135-e496b19fd8bc.png)
+
 >
 ### Add custom properties
 
 ```python
 import h_transport_materials as htm
 
 import numpy as np
```

### Comparing `h_transport_materials-0.8.1/setup.cfg` & `h_transport_materials-0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_arhenius_property.py` & `h_transport_materials-0.9/tests/test_arhenius_property.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_diffusivity.py` & `h_transport_materials-0.9/tests/test_diffusivity.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_fitting.py` & `h_transport_materials-0.9/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_plotting.py` & `h_transport_materials-0.9/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_property.py` & `h_transport_materials-0.9/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `h_transport_materials-0.8.1/tests/test_system.py` & `h_transport_materials-0.9/tests/test_system.py`

 * *Files identical despite different names*

