# Comparing `tmp/juriscraper-2.5.8.tar.gz` & `tmp/juriscraper-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juriscraper-2.5.8.tar", last modified: Tue Jul 26 21:59:56 2022, max compression
+gzip compressed data, was "juriscraper-2.5.9.tar", last modified: Thu Jul 28 21:00:26 2022, max compression
```

## Comparing `juriscraper-2.5.8.tar` & `juriscraper-2.5.9.tar`

### file list

```diff
@@ -1,417 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-26 21:59:48.000000 juriscraper-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-26 21:59:48.000000 juriscraper-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-26 21:59:48.000000 juriscraper-2.5.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    15915 2022-07-26 21:59:56.038100 juriscraper-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14807 2022-07-26 21:59:48.000000 juriscraper-2.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.006100 juriscraper-2.5.8/juriscraper/
--rw-r--r--   0 runner    (1001) docker     (121)    16942 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/AbstractSite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/DeferringList.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OpinionSite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OpinionSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OpinionSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OpinionSiteWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OralArgumentSite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OralArgumentSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/OralArgumentSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/WebDriven.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.006100 juriscraper-2.5.8/juriscraper/fdsys/
--rw-r--r--   0 runner    (1001) docker     (121)     8236 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/fdsys/FDSysSite.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/fdsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-07-26 21:59:48.000000 juriscraper-2.5.8/juriscraper/fdsys/scrape_court_names.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.006100 juriscraper-2.5.8/juriscraper/fdsys/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/fdsys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/fdsys/utils/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/fdsys/utils/get_xpath_results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.006100 juriscraper-2.5.8/juriscraper/lasc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lasc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lasc/fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)    18169 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lasc/http.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.010100 juriscraper-2.5.8/juriscraper/lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/cookie_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4144 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/diff_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9925 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/judge_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/log_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    26813 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.010100 juriscraper-2.5.8/juriscraper/opinions/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/opinion_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.010100 juriscraper-2.5.8/juriscraper/opinions/united_states/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.010100 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/asbca.py
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/bva.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.014100 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.014100 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.014100 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/dcd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.014100 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/afcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/ag.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/armfor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cavc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2907 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cgcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/nmcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/tax.py
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_u.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/alaska.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/alaskactapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ariz.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/arizctapp_div_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/arizctapp_div_2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ark.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/arkctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/cal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calag.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_1st.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_2nd.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_3rd.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_5th.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_6th.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_app_div.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/colo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/coloctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/conn.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/connappct.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/dc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/delaware.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/delch.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/delctcompl.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/delsuperct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fla.py
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_1_per_curiam.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_1_written.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_2_per_curiam.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_2_written.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_4_pc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_4_written.py
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ga.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/gactapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/haw.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/haw_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/hawapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/idaho_civil.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/idaho_criminal.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/illappct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/iowa.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/iowactapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/kan_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/kan_u.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/kanctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/kanctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ky.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/kyctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/la.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/lactapp_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mass.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/massappct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/massappct_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/masslandct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/md.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mdag.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mdctspecapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/me.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mich.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/michctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/minn.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/minnag.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/minnctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/miss.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/miss_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/missctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mo.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/moctapp_eastern.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/moctapp_southern.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/moctapp_western.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/mont.py
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nc.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ncctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/neb.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nebctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nev_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nev_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nh.py
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nj.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/njsuperctappdiv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nm.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nmctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyag.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (121)     6496 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappterm_1st.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappterm_2nd.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/nysupct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohio.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_10.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_11.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_12.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_7.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_8.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctapp_9.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctcl.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/okla.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklaag.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklacivapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/or.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/pa.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/pacommwct.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/pasuperct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ri_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/ri_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/sc.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/scctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/tenn.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/tenncrimapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/tennctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)    11749 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/tex.py
--rw-r--r--   0 runner    (1001) docker     (121)     6335 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texag.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_1.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_10.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_11.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_12.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_13.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_14.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_4.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_5.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_6.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_7.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_8.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texapp_9.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/texcrimapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/utah.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/utahctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/va.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vactapp_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vactapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vt.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vtsuperct_civil.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vtsuperct_criminal.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vtsuperct_family.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/vtsuperct_probate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/wash.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/washctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/washctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/wis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/wva.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/state/wyo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/as.py
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/guam.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/mp.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/pr.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states/territories/vi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (121)     5630 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (121)     7842 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.030100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
--rw-r--r--   0 runner    (1001) docker     (121)     5753 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.034100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.034100 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/me.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
--rw-r--r--   0 runner    (1001) docker     (121)     6103 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (121)    10853 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.034100 juriscraper-2.5.8/juriscraper/oral_args/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/oral_argument_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.034100 juriscraper-2.5.8/juriscraper/oral_args/united_states/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca11.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca9.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/scotus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/oral_args/united_states/state/md.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/juriscraper/pacer/
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29256 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/appellate_docket.py
--rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12767 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/case_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/case_query_advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/claims_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     9961 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/docket_history_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    51451 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/docket_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/docket_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17748 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/email.py
--rw-r--r--   0 runner    (1001) docker     (121)    13369 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/free_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)    10165 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/hidden_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13944 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/internet_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/mobile_query.py
--rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)    14884 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacer/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      598 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/pacerdocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/juriscraper/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.038100 juriscraper-2.5.8/juriscraper/video/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:49.000000 juriscraper-2.5.8/juriscraper/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:59:56.006100 juriscraper-2.5.8/juriscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15915 2022-07-26 21:59:55.000000 juriscraper-2.5.8/juriscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20852 2022-07-26 21:59:55.000000 juriscraper-2.5.8/juriscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 21:59:55.000000 juriscraper-2.5.8/juriscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-26 21:59:55.000000 juriscraper-2.5.8/juriscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-26 21:59:55.000000 juriscraper-2.5.8/juriscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-26 21:59:49.000000 juriscraper-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-26 21:59:49.000000 juriscraper-2.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-07-26 21:59:56.042100 juriscraper-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-07-26 21:59:49.000000 juriscraper-2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.718328 juriscraper-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-07-28 21:00:19.000000 juriscraper-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-28 21:00:19.000000 juriscraper-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-28 21:00:19.000000 juriscraper-2.5.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    15915 2022-07-28 21:00:26.718328 juriscraper-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14807 2022-07-28 21:00:19.000000 juriscraper-2.5.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/
+-rw-r--r--   0 runner    (1001) docker     (121)    16942 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/AbstractSite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/DeferringList.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OpinionSite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OpinionSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OpinionSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OpinionSiteWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OralArgumentSite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OralArgumentSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/OralArgumentSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/WebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/fdsys/
+-rw-r--r--   0 runner    (1001) docker     (121)     8236 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/FDSysSite.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/scrape_court_names.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/fdsys/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/utils/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/fdsys/utils/get_xpath_results.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/lasc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lasc/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18169 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lasc/http.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/cookie_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4144 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/diff_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9925 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/judge_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26813 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper/opinions/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/opinion_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.690327 juriscraper-2.5.9/juriscraper/opinions/united_states/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.690327 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/asbca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/bva.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.690327 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.690327 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.690327 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/dcd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.694327 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/afcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/ag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/armfor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cavc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2907 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cgcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/nmcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/tax.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/alaskactapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ariz.py
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/arizctapp_div_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/arizctapp_div_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ark.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/arkctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/cal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_1st.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_5th.py
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_6th.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_app_div.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/colo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/coloctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/conn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/connappct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/dc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/delch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/delctcompl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/delsuperct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fla.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_1_per_curiam.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_1_written.py
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_2_per_curiam.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_2_written.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_4_pc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_4_written.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ga.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/gactapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/haw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/haw_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/hawapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/idaho_civil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/idaho_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/illappct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/iowactapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/kan_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/kan_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/kanctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/kanctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ky.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/kyctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/la.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/lactapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/massappct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/massappct_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/masslandct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mdag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mdctspecapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mich.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/michctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/minn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/minnag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/minnctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/miss.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/miss_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/missctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/moctapp_eastern.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/moctapp_southern.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/moctapp_western.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/mont.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ncctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/neb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nebctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nev_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nev_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nj.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/njsuperctappdiv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nmctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6496 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappterm_1st.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappterm_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/nysupct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctcl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/okla.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklaag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/or.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/pa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/pacommwct.py
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/pasuperct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ri_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/ri_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/sc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/scctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/tenn.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/tenncrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/tennctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11749 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/tex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6335 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_13.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_14.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/texcrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/utah.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/utahctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/va.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vactapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vactapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vtsuperct_civil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vtsuperct_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vtsuperct_family.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/vtsuperct_probate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/wash.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/washctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/washctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/wis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/wva.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/state/wyo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/as.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/guam.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/mp.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/pr.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states/territories/vi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5630 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7842 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5753 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.710328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.714328 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6103 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10853 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.714328 juriscraper-2.5.9/juriscraper/oral_args/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/oral_argument_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.714328 juriscraper-2.5.9/juriscraper/oral_args/united_states/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.714328 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca11.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca9.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/scotus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.718328 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/oral_args/united_states/state/md.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.718328 juriscraper-2.5.9/juriscraper/pacer/
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29256 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/appellate_docket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12767 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/case_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/case_query_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/claims_register.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9961 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/docket_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51451 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/docket_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/docket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17748 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13369 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/free_documents.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10165 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/hidden_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13944 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/internet_archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/mobile_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14884 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacer/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      598 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/pacerdocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.718328 juriscraper-2.5.9/juriscraper/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.718328 juriscraper-2.5.9/juriscraper/video/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:19.000000 juriscraper-2.5.9/juriscraper/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 21:00:26.686327 juriscraper-2.5.9/juriscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15915 2022-07-28 21:00:26.000000 juriscraper-2.5.9/juriscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    20779 2022-07-28 21:00:26.000000 juriscraper-2.5.9/juriscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 21:00:26.000000 juriscraper-2.5.9/juriscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-28 21:00:26.000000 juriscraper-2.5.9/juriscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-28 21:00:26.000000 juriscraper-2.5.9/juriscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-28 21:00:19.000000 juriscraper-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-28 21:00:19.000000 juriscraper-2.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-07-28 21:00:26.718328 juriscraper-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-07-28 21:00:19.000000 juriscraper-2.5.9/setup.py
```

### Comparing `juriscraper-2.5.8/LICENSE` & `juriscraper-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/PKG-INFO` & `juriscraper-2.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.5.8
+Version: 2.5.9
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.5.8/README.rst` & `juriscraper-2.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/AbstractSite.py` & `juriscraper-2.5.9/juriscraper/AbstractSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/DeferringList.py` & `juriscraper-2.5.9/juriscraper/DeferringList.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/OpinionSite.py` & `juriscraper-2.5.9/juriscraper/OpinionSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/OpinionSiteLinear.py` & `juriscraper-2.5.9/juriscraper/OpinionSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/OralArgumentSite.py` & `juriscraper-2.5.9/juriscraper/OralArgumentSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/OralArgumentSiteLinear.py` & `juriscraper-2.5.9/juriscraper/OralArgumentSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/WebDriven.py` & `juriscraper-2.5.9/juriscraper/WebDriven.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/fdsys/FDSysSite.py` & `juriscraper-2.5.9/juriscraper/fdsys/FDSysSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/fdsys/scrape_court_names.py` & `juriscraper-2.5.9/juriscraper/fdsys/scrape_court_names.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/fdsys/utils/get_metadata.py` & `juriscraper-2.5.9/juriscraper/fdsys/utils/get_metadata.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/fdsys/utils/get_xpath_results.py` & `juriscraper-2.5.9/juriscraper/fdsys/utils/get_xpath_results.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lasc/fetch.py` & `juriscraper-2.5.9/juriscraper/lasc/fetch.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lasc/http.py` & `juriscraper-2.5.9/juriscraper/lasc/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/cookie_utils.py` & `juriscraper-2.5.9/juriscraper/lib/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/date_utils.py` & `juriscraper-2.5.9/juriscraper/lib/date_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/diff_tools.py` & `juriscraper-2.5.9/juriscraper/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/exceptions.py` & `juriscraper-2.5.9/juriscraper/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/html_utils.py` & `juriscraper-2.5.9/juriscraper/lib/html_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/importer.py` & `juriscraper-2.5.9/juriscraper/lib/importer.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/judge_parsers.py` & `juriscraper-2.5.9/juriscraper/lib/judge_parsers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/log_tools.py` & `juriscraper-2.5.9/juriscraper/lib/log_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/network_utils.py` & `juriscraper-2.5.9/juriscraper/lib/network_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/string_utils.py` & `juriscraper-2.5.9/juriscraper/lib/string_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/test_utils.py` & `juriscraper-2.5.9/juriscraper/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/lib/utils.py` & `juriscraper-2.5.9/juriscraper/lib/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/opinion_template.py` & `juriscraper-2.5.9/juriscraper/opinions/opinion_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/asbca.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/asbca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/bia.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/bva.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/bva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/mspb_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/mspb_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/mspb_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/mspb_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/administrative_agency/olc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca1.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca10.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca11_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca11_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca11_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca11_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca2_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca2_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca2_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca2_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca3_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca3_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca4.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/wyo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,60 @@
-from datetime import date, datetime, timedelta
+"""Scraper for Wyoming Supreme Court
+CourtID: wyo
+Court Short Name: Wyo.
+History:
+ - 2014-07-02: mlr: Created new version when court got new website.
+ - 2015-07-06: m4h7: Updated to use JSON!
+ - 2016-06-09: arderyp: Updated because json endpoint moved and was changed
+"""
 
-from dateutil.rrule import DAILY, rrule
+import re
+from datetime import date, datetime
 
-from juriscraper.AbstractSite import logger
-from juriscraper.lib.string_utils import clean_if_py3
 from juriscraper.OpinionSite import OpinionSite
 
 
 class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.url = "https://www.ca4.uscourts.gov/DataOpinions.aspx"
         self.court_id = self.__module__
-        td = date.today()
-        self.parameters = {
-            "CASENUM": "",
-            "FROMDATE": (td - timedelta(days=10)).strftime("%m-%d-%Y"),
-            "TITLE": "",
-            "TODATE": td.strftime("%m-%d-%Y"),
-        }
-        self.method = "POST"
-        self.interval = 30
-        self.back_scrape_iterable = [
-            i.date()
-            for i in rrule(
-                DAILY,
-                interval=self.interval,  # Every interval days
-                dtstart=date(1996, 1, 1),
-                until=date(2016, 1, 1),
-            )
-        ]
+        self.base_url = "http://www.courts.state.wy.us"
+        self.download_base = "https://documents.courts.state.wy.us/Opinions"
+        self.url = (
+            "https://opinions.courts.state.wy.us/Home/GetOpinions?StartDate=1%2F1%2F"
+            + str(date.today().year)
+        )
 
     def _get_case_names(self):
-        path = "//tr/td[4]/text()"
-        names = []
-        for s in self.html.xpath(path):
-            s = clean_if_py3(s)
-            if s.strip():
-                names.append(s)
-        logger.info(str(len(names)))
-        return names
+        return [
+            f"{opinion['Appellant']} v. {opinion['Appellee']}"
+            for opinion in self.html
+        ]
 
     def _get_download_urls(self):
-        path = "//tr/td[1]/a/@href"
-        return list(self.html.xpath(path))
+        download_urls = []
+        for record in self.html:
+            pdf_file_name = record["DocumentName"]
+            if pdf_file_name[:5] == "../..":
+                pdf_file_name = pdf_file_name[5:]
+            url = f"{self.download_base}/{pdf_file_name}".replace(" ", "%20")
+            download_urls.append(url)
+        return download_urls
 
     def _get_case_dates(self):
-        path = "//tr/td[3]/text()"
         case_dates = []
-        for date_string in self.html.xpath(path):
-            date_string = clean_if_py3(date_string).strip()
-            if date_string:
-                case_dates.append(
-                    datetime.strptime(date_string, "%m/%d/%Y").date()
-                )
+        date_re = re.compile(r"^/Date\((\d+)\)/$")
+        for record in self.html:
+            match = date_re.match(record["date_heard"])
+            if match:
+                timestamp = int(match.group(1)) / 1000
+                case_dates.append(datetime.fromtimestamp(timestamp).date())
         return case_dates
 
     def _get_docket_numbers(self):
-        path = "//tr/td[2]//text()"
-        docket_numbers = []
-        for s in self.html.xpath(path):
-            s = clean_if_py3(s).strip()
-            if s:
-                docket_numbers.append(s)
-        return docket_numbers
+        return [opinion["DocketNumber"] for opinion in self.html]
+
+    def _get_citations(self):
+        return [opinion["OpinionID"] for opinion in self.html]
 
     def _get_precedential_statuses(self):
-        statuses = []
-        # using download link, we can get the statuses
-        for download_url in self.download_urls:
-            file_name = download_url.split("/")[-1]
-            if "u" in file_name.lower():
-                statuses.append("Unpublished")
-            else:
-                statuses.append("Published")
-        return statuses
-
-    def _download_backwards(self, d):
-
-        self.parameters = {
-            "CASENUM": "",
-            "FROMDATE": d.strftime("%m-%d-%Y"),
-            "TITLE": "",
-            "TODATE": (d + timedelta(self.interval)).strftime("%m-%d-%Y"),
-        }
-
-        self.html = self._download()
-        if self.html is not None:
-            # Setting status is important because it prevents the download
-            # function from being run a second time by the parse method.
-            self.status = 200
+        return ["Published"] * len(self.case_names)
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca5.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca6.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca7.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca8.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca9_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca9_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/ca9_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/ca9_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cadc_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cadc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/cafc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/dcd.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/dcd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_district/ed_louisiana.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_district/ed_louisiana.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_memorandum.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_memorandum.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/acca_summary.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/acca_summary.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/afcca.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/afcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/ag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/ag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/armfor.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/armfor.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cavc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cavc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cgcca.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cgcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/cit.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/cit.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/nmcca.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/nmcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/tax.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/tax.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/__init__.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/alaska.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/alaska.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ariz.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ariz.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/arizctapp_div_2.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/arizctapp_div_2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ark.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ark.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/cal.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/cal.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/calag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/calag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/calctapp_1st.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/calctapp_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/colo.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/colo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/coloctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/coloctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/conn.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/conn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/connappct.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/connappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/dc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/dc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/delaware.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/delaware.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fla.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_1_per_curiam.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_1_per_curiam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_2_per_curiam.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_2_per_curiam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_3.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_4_written.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_4_written.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/fladistctapp_5.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/fladistctapp_5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ga.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ga.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/gactapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/gactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/haw.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/haw.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/haw_beginningofyear.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/haw_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/idaho_civil.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/idaho_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/idahoctapp_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/idahoctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ill.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/illappct.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/illappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ind.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/iowa.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/iowa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/iowactapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/iowactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/kan_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/kan_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ky.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ky.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/kyctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/kyctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/la.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/la.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/lactapp_1.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/lactapp_1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mass.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mass.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/massappct_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/massappct_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/masslandct.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/masslandct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/md.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mdag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mdag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mdctspecapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mdctspecapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/me.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mich.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mich.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/michctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/michctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/minn.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/minn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/minnag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/minnag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/miss.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/miss.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/miss_beginningofyear.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/miss_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mo.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/mont.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/mont.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ncctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ncctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nd.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/neb.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/neb.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nev_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nev_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nev_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nev_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nh.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nh.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nj.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nj.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nm.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nm.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ny.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappdiv_1st.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappdiv_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/nyappterm_1st.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/nyappterm_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohio.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohio.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/okla.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/okla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklaag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklaag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklacivapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklacivapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/oklacrimapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/oklacrimapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/or.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/or.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/pa.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/pa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/pacommwct.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/pacommwct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ri_p.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ri_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/ri_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/ri_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/sc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/sc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/scctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/scctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/sd.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/tenn.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/tenn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/tex.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/tex.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/texag.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/texag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/utah.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/utah.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/utahctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/va.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/va.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/vactapp_u.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/vactapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/vt.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/vt.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/wash.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/wash.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/wis.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/wis.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/wva.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/state/wva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/state/wyo.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/cadc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-"""Scraper for Wyoming Supreme Court
-CourtID: wyo
-Court Short Name: Wyo.
-History:
- - 2014-07-02: mlr: Created new version when court got new website.
- - 2015-07-06: m4h7: Updated to use JSON!
- - 2016-06-09: arderyp: Updated because json endpoint moved and was changed
+"""Scraper for D.C. Circuit of Appeals
+CourtID: cadc
+Court Short Name: cadc
+Author: Andrei Chelaru
+Reviewer: mlr
+Date created: 18 July 2014
 """
 
-import re
 from datetime import date, datetime
 
-from juriscraper.OpinionSite import OpinionSite
+from juriscraper.OralArgumentSite import OralArgumentSite
 
 
-class Site(OpinionSite):
+class Site(OralArgumentSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        self.base_url = "http://www.courts.state.wy.us"
-        self.download_base = "https://documents.courts.state.wy.us/Opinions"
-        self.url = (
-            "https://opinions.courts.state.wy.us/Home/GetOpinions?StartDate=1%2F1%2F"
-            + str(date.today().year)
+        d = date.today()
+        # d = date(month=5, day=1, year=2014)
+        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
+            yearmo=d.strftime("%Y%m")
         )
-
-    def _get_case_names(self):
-        return [
-            f"{opinion['Appellant']} v. {opinion['Appellee']}"
-            for opinion in self.html
+        self.back_scrape_iterable = [
+            "%s%02d" % (year, month)
+            for year in range(2007, d.year + 1)
+            for month in range(1, 13)
         ]
 
+    def _download(self, **kwargs):
+        # The certificate on their site has expired.
+        return super()._download(request_dict={"verify": False})
+
     def _get_download_urls(self):
-        download_urls = []
-        for record in self.html:
-            pdf_file_name = record["DocumentName"]
-            if pdf_file_name[:5] == "../..":
-                pdf_file_name = pdf_file_name[5:]
-            url = f"{self.download_base}/{pdf_file_name}".replace(" ", "%20")
-            download_urls.append(url)
-        return download_urls
+        path = "id('ViewBody')//div[contains(concat(' ',@class,' '),' row-entry')]//@href"
+        return list(self.html.xpath(path))
+
+    def _get_case_names(self):
+        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' column-two')]/div[1]/text()"
+        return list(self.html.xpath(path))
 
     def _get_case_dates(self):
-        case_dates = []
-        date_re = re.compile(r"^/Date\((\d+)\)/$")
-        for record in self.html:
-            match = date_re.match(record["date_heard"])
-            if match:
-                timestamp = int(match.group(1)) / 1000
-                case_dates.append(datetime.fromtimestamp(timestamp).date())
-        return case_dates
+        path = "id('ViewBody')//date/text()"
+        return list(map(self._return_case_date, self.html.xpath(path)))
 
-    def _get_docket_numbers(self):
-        return [opinion["DocketNumber"] for opinion in self.html]
+    @staticmethod
+    def _return_case_date(e):
+        e = "".join(e.split())
+        return datetime.strptime(e, "%m/%d/%Y").date()
 
-    def _get_citations(self):
-        return [opinion["OpinionID"] for opinion in self.html]
+    def _get_docket_numbers(self):
+        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' row-entry')]//a//text()"
+        return list(self.html.xpath(path))
 
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.case_names)
+    def _get_judges(self):
+        path = '//div[span[contains(., "Judges")]]/text()'
+        return [" ".join(s.split()) for s in self.html.xpath(path)]
+
+    def _download_backwards(self, yearmo):
+        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
+            yearmo=yearmo,
+        )
+        self.html = self._download()
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states/territories/guam.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states/territories/guam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca4.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,67 @@
-from datetime import date, datetime, timedelta
+# Scraper for the United States Court of International Trade
+# CourtID: cit
+# Court Short Name: Ct. Int'l Trade
+# Neutral Citation Format: Ct. Int'l Trade No. 12-1
+import re
+import time
+from datetime import date
+
+from lxml import html
 
 from juriscraper.OpinionSite import OpinionSite
 
 
 class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.url = "http://pacer.ca4.uscourts.gov/cgi-bin/opinions.pl"
+        # This is a special backscraper to deal with problems on the 2005 page.
+        self.url = "http://www.cit.uscourts.gov/SlipOpinions/SlipOps-2005.html"
         self.court_id = self.__module__
-        td = date.today()
-        self.parameters = {
-            "CASENUM": "",
-            "FROMDATE": (td - timedelta(days=20)).strftime("%m-%d-%Y"),
-            "TITLE": "",
-            "TODATE": td.strftime("%m-%d-%Y"),
-        }
-        self.method = "POST"
+
+    def _get_download_urls(self):
+        return [
+            t
+            for t in self.html.xpath(
+                "//table[3]/tr[position() > 1]/td[1]/a/@href | //table[3]/tr[position() > 1]/td[1]/font//@href"
+            )
+        ]
+
+    def _get_citations(self):
+        neutral_citations = []
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[1]/font/a"):
+            s = html.tostring(e, method="text", encoding="unicode").strip()
+            neutral_citations.append(s)
+        return neutral_citations
 
     def _get_case_names(self):
-        if self.only_get_unpublished:
-            # No precedential cases (or else dups)
-            path = "//tr/td[4][../td[1]/a/text()[contains(., 'U')]]/text()"
-        else:
-            path = "//tr/td[4]/text()"
-        names = []
-        for s in self.html.xpath(path):
-            if s.strip():
-                names.append(s)
-        return names
+        case_names = []
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[2]/font"):
+            s = html.tostring(e, method="text", encoding="unicode").strip()
+            # We strip "erratum: mm/dd/yyyy" from the case names of errata docs.
+            if "erratum" in s:
+                case_names.append(s.strip()[:-18])
+            else:
+                case_names.append(s.strip())
+        return case_names
 
-    def _get_download_urls(self):
-        if self.only_get_unpublished:
-            path = "//tr/td[1][../td[1]/a/text()[contains(., 'U')]]/a/@href"
-        else:
-            path = "//tr/td[1]/a/@href"
-        return list(self.html.xpath(path))
+    def _get_precedential_statuses(self):
+        return ["Published"] * len(self.case_names)
 
     def _get_case_dates(self):
-        if self.only_get_unpublished:
-            path = "//tr/td[3][../td[1]/a/text()[contains(., 'U')]]/text()"
-        else:
-            path = "//tr/td[3]/text()"
-        return [
-            datetime.strptime(date_string.strip(), "%Y/%m/%d").date()
-            for date_string in self.html.xpath(path)
-        ]
+        case_dates = []
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[3]/font"):
+            s = html.tostring(e, method="text", encoding="unicode").strip()
+            case_dates.append(
+                date.fromtimestamp(
+                    time.mktime(time.strptime(s.strip(), "%m/%d/%Y"))
+                )
+            )
+        return case_dates
 
+    # Because there can be multiple docket numbers we have to replace some newlines.
     def _get_docket_numbers(self):
-        if self.only_get_unpublished:
-            path = "//tr/td[2][../td[1]/a/text()[contains(., 'U')]]//text()"
-        else:
-            path = "//tr/td[2]//text()"
         docket_numbers = []
-        for s in self.html.xpath(path):
-            if s.strip():
-                docket_numbers.append(s)
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[4]"):
+            s = html.tostring(e, method="text", encoding="unicode").strip()
+            docket_numbers.append(s.replace("\r\n", " &"))
         return docket_numbers
-
-    def _get_precedential_statuses(self):
-        statuses = []
-        # using download link, we can get the statuses
-        for download_url in self.download_urls:
-            file_name = download_url.split("/")[-1]
-            if "u" in file_name.lower():
-                statuses.append("Unpublished")
-            else:
-                statuses.append("Published")
-        return statuses
-
-    def _download_backwards(self, dt):
-        self.end_date = dt + timedelta(days=6)
-        self.resource_org_end_date = date(2007, 7, 31)
-        # We only get unpublished docs when we're in a period of time during which we have resource.org docs.
-        self.only_get_unpublished = self.end_date < self.resource_org_end_date
-        self.parameters["FROMDATE"] = dt.strftime("%m-%d-%Y")
-        self.parameters["TODATE"] = self.end_date.strftime("%m-%d-%Y")
-        self.html = self._download()
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,40 +10,42 @@
 
 from juriscraper.OpinionSite import OpinionSite
 
 
 class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # This is a special backscraper to deal with problems on the 2005 page.
-        self.url = "http://www.cit.uscourts.gov/SlipOpinions/SlipOps-2005.html"
+        # This is a special backscraper to deal with problems on the 2007 page.
+        self.url = "http://www.cit.uscourts.gov/SlipOpinions/SlipOps-2007.html"
         self.court_id = self.__module__
 
     def _get_download_urls(self):
         return [
             t
             for t in self.html.xpath(
-                "//table[3]/tr[position() > 1]/td[1]/a/@href | //table[3]/tr[position() > 1]/td[1]/font//@href"
+                "//table[3]/tr[position() > 1]/td[1]/a/@href | //table[3]/tr[position() > 1]/td[1]/font/a/@href"
             )
         ]
 
     def _get_citations(self):
         neutral_citations = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[1]/font/a"):
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[1]"):
             s = html.tostring(e, method="text", encoding="unicode").strip()
             neutral_citations.append(s)
         return neutral_citations
 
     def _get_case_names(self):
         case_names = []
         for e in self.html.xpath("//table[3]/tr[position() > 1]/td[2]/font"):
             s = html.tostring(e, method="text", encoding="unicode").strip()
-            # We strip "erratum: mm/dd/yyyy" from the case names of errata docs.
+            # We strip "errat[um/a]: mm/dd/yyyy" from the case names of errata docs.
             if "erratum" in s:
-                case_names.append(s.strip()[:-18])
+                case_names.append(s.strip()[:-19])
+            elif "errata" in s:
+                case_names.append(s.strip()[:-17])
             else:
                 case_names.append(s.strip())
         return case_names
 
     def _get_precedential_statuses(self):
         return ["Published"] * len(self.case_names)
 
@@ -61,7 +63,16 @@
     # Because there can be multiple docket numbers we have to replace some newlines.
     def _get_docket_numbers(self):
         docket_numbers = []
         for e in self.html.xpath("//table[3]/tr[position() > 1]/td[4]"):
             s = html.tostring(e, method="text", encoding="unicode").strip()
             docket_numbers.append(s.replace("\r\n", " &"))
         return docket_numbers
+
+    # Comment out the following section if backscraping years 1999-2005.
+    # Because there are sometimes multiple judges we have to strip some whitespace.
+    def _get_judges(self):
+        judges = []
+        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[5]"):
+            s = html.tostring(e, method="text", encoding="unicode")
+            judges.append(s.strip())
+        return judges
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# Scraper for the United States Court of International Trade
-# CourtID: cit
-# Court Short Name: Ct. Int'l Trade
-# Neutral Citation Format: Ct. Int'l Trade No. 12-1
 import re
 import time
 from datetime import date
 
 from lxml import html
 
+from juriscraper.lib.string_utils import clean_string
 from juriscraper.OpinionSite import OpinionSite
 
 
 class Site(OpinionSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # This is a special backscraper to deal with problems on the 2007 page.
-        self.url = "http://www.cit.uscourts.gov/SlipOpinions/SlipOps-2007.html"
+        self.url = "http://www.isc.idaho.gov/opinions/cacivil.htm"
         self.court_id = self.__module__
 
-    def _get_download_urls(self):
-        return [
-            t
-            for t in self.html.xpath(
-                "//table[3]/tr[position() > 1]/td[1]/a/@href | //table[3]/tr[position() > 1]/td[1]/font/a/@href"
-            )
-        ]
-
-    def _get_citations(self):
-        neutral_citations = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[1]"):
-            s = html.tostring(e, method="text", encoding="unicode").strip()
-            neutral_citations.append(s)
-        return neutral_citations
+    def tweak_response_object(self):
+        """
+        This state uses an HTTP header to indicate an encoding of UTF-8,
+        but the encoding is actually ISO-8859-1, as indicated in the HTML
+        itself. When this page is rendered in Firefox, chardet fails, and
+        many unknown characters are displayed to the user. Setting the
+        character encoding manually fixes the issue.
+        """
+        self.request["response"].encoding = "ISO-8859-1"
 
     def _get_case_names(self):
         case_names = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[2]/font"):
-            s = html.tostring(e, method="text", encoding="unicode").strip()
-            # We strip "errat[um/a]: mm/dd/yyyy" from the case names of errata docs.
-            if "erratum" in s:
-                case_names.append(s.strip()[:-19])
-            elif "errata" in s:
-                case_names.append(s.strip()[:-17])
-            else:
-                case_names.append(s.strip())
+        for xelement in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]'):
+            # Our text nodes are randomly surrounded by HTML spans, so we start
+            # at a high level node, and strip down to just what we want.
+            data_html = html.tostring(xelement, encoding=str)
+            data_string = re.sub(r"<[^>]*?>", "", data_html)
+            data_string = " ".join(data_string.split())
+
+            # Several regexes are needed since we have hyphen-separated values
+            regexes = [
+                "(.*?)[-–](.*?)–",
+                "(.*?)[-–](.*)-",
+                "(.*?)[-–](.*)$",
+            ]
+            for regex in regexes:
+                try:
+                    case_names.append(re.search(regex, data_string).group(2))
+                    # Found what we're looking for...
+                    break
+                except AttributeError:
+                    # Try the next regex...
+                    continue
+
         return case_names
 
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.case_names)
+    def _get_download_urls(self):
+        download_urls = []
+        for e in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]/@href'):
+            download_urls.append(e)
+        return download_urls
 
     def _get_case_dates(self):
         case_dates = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[3]/font"):
-            s = html.tostring(e, method="text", encoding="unicode").strip()
-            case_dates.append(
-                date.fromtimestamp(
-                    time.mktime(time.strptime(s.strip(), "%m/%d/%Y"))
-                )
-            )
+        for e in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]'):
+            s = html.tostring(e, method="text", encoding="unicode")
+            # Cleanup...
+            s = s.split("-")[0]
+            s = s.split("–")[0]
+            date_formats = ["%B %d, %Y", "%B %d %Y", "%B %d , %Y"]
+            for format in date_formats:
+                try:
+                    case_date = date.fromtimestamp(
+                        time.mktime(time.strptime(clean_string(s), format))
+                    )
+                except ValueError:
+                    continue
+            case_dates.append(case_date)
         return case_dates
 
-    # Because there can be multiple docket numbers we have to replace some newlines.
-    def _get_docket_numbers(self):
-        docket_numbers = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[4]"):
-            s = html.tostring(e, method="text", encoding="unicode").strip()
-            docket_numbers.append(s.replace("\r\n", " &"))
-        return docket_numbers
-
-    # Comment out the following section if backscraping years 1999-2005.
-    # Because there are sometimes multiple judges we have to strip some whitespace.
-    def _get_judges(self):
-        judges = []
-        for e in self.html.xpath("//table[3]/tr[position() > 1]/td[5]"):
-            s = html.tostring(e, method="text", encoding="unicode")
-            judges.append(s.strip())
-        return judges
+    def _get_precedential_statuses(self):
+        return ["Published"] * len(self.case_names)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca8.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,60 @@
-import re
-import time
-from datetime import date
+"""Oral Argument Audio Scraper for Eighth Circuit Court of Appeals
+CourtID: ca8
+Court Short Name: 8th Cir.
+Author: Brian W. Carver
+Date created: 2014-06-21
+History:
+ - 2014-07-22: download_url fixed by mlr
+"""
 
-from lxml import html
+from datetime import datetime
 
-from juriscraper.lib.string_utils import clean_string
-from juriscraper.OpinionSite import OpinionSite
+from juriscraper.lib.string_utils import clean_if_py3
+from juriscraper.OralArgumentSite import OralArgumentSite
 
 
-class Site(OpinionSite):
+class Site(OralArgumentSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.url = "http://www.isc.idaho.gov/opinions/cacivil.htm"
         self.court_id = self.__module__
+        self.url = "http://media-oa.ca8.uscourts.gov/circ8rss.xml"
 
-    def tweak_response_object(self):
-        """
-        This state uses an HTTP header to indicate an encoding of UTF-8,
-        but the encoding is actually ISO-8859-1, as indicated in the HTML
-        itself. When this page is rendered in Firefox, chardet fails, and
-        many unknown characters are displayed to the user. Setting the
-        character encoding manually fixes the issue.
-        """
-        self.request["response"].encoding = "ISO-8859-1"
+    def _download(self, request_dict={}):
+        """Go through the items and filter out ones that aren't complete."""
+        self.items = []
+        html_tree = super()._download(request_dict=request_dict)
+        for item in html_tree.xpath("//item"):
+            case_name = item.xpath("./title/text()")[0].split(":", 1)[1]
+            if case_name.strip():
+                self.items.append(item)
+
+        # Set self.html to None so it can't be misused.
+        return None
+
+    def _get_download_urls(self):
+        return [item.xpath("./enclosure/@url")[0] for item in self.items]
 
     def _get_case_names(self):
         case_names = []
-        for xelement in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]'):
-            # Our text nodes are randomly surrounded by HTML spans, so we start
-            # at a high level node, and strip down to just what we want.
-            data_html = html.tostring(xelement, encoding=str)
-            data_string = re.sub(r"<[^>]*?>", "", data_html)
-            data_string = " ".join(data_string.split())
-
-            # Several regexes are needed since we have hyphen-separated values
-            regexes = [
-                "(.*?)[-–](.*?)–",
-                "(.*?)[-–](.*)-",
-                "(.*?)[-–](.*)$",
-            ]
-            for regex in regexes:
-                try:
-                    case_names.append(re.search(regex, data_string).group(2))
-                    # Found what we're looking for...
-                    break
-                except AttributeError:
-                    # Try the next regex...
-                    continue
-
+        for txt in [item.xpath("./title/text()")[0] for item in self.items]:
+            case_name = clean_if_py3(txt).split(": ", 1)[1]
+            case_names.append(case_name)
         return case_names
 
-    def _get_download_urls(self):
-        download_urls = []
-        for e in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]/@href'):
-            download_urls.append(e)
-        return download_urls
-
     def _get_case_dates(self):
         case_dates = []
-        for e in self.html.xpath('//li[@class="MsoNormal"]/span/a[1]'):
-            s = html.tostring(e, method="text", encoding="unicode")
-            # Cleanup...
-            s = s.split("-")[0]
-            s = s.split("–")[0]
-            date_formats = ["%B %d, %Y", "%B %d %Y", "%B %d , %Y"]
-            for format in date_formats:
-                try:
-                    case_date = date.fromtimestamp(
-                        time.mktime(time.strptime(clean_string(s), format))
-                    )
-                except ValueError:
-                    continue
-            case_dates.append(case_date)
+        for txt in [
+            item.xpath("./description/text()")[0] for item in self.items
+        ]:
+            # I can't see it, but there's apparently whitespace or a newline
+            # at the end of these dates that has to be removed or we error out.
+            case_date = clean_if_py3(txt).split("about ", 1)[1].strip()
+            case_dates.append(datetime.strptime(case_date, "%m/%d/%Y").date())
         return case_dates
 
-    def _get_precedential_statuses(self):
-        return ["Published"] * len(self.case_names)
+    def _get_docket_numbers(self):
+        docket_numbers = []
+        for txt in [item.xpath("./title/text()")[0] for item in self.items]:
+            docket_number = clean_if_py3(txt).split(": ", 1)[0]
+            docket_numbers.append(docket_number)
+        return docket_numbers
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ill.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ind.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/indctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/indctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/me.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/me_2013.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/me_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/nd.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/ny.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/sd.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py` & `juriscraper-2.5.9/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/oral_argument_template.py` & `juriscraper-2.5.9/juriscraper/oral_args/oral_argument_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca1.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca10.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca11.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca11.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca2.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca3.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca4.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca5.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca6.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca7.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/ca9.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/ca9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/cadc.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/scotus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-"""Scraper for D.C. Circuit of Appeals
-CourtID: cadc
-Court Short Name: cadc
-Author: Andrei Chelaru
-Reviewer: mlr
-Date created: 18 July 2014
+"""Scraper for Supreme Court of U.S.
+CourtID: scotus
+Court Short Name: scotus
+History:
+ - 2014-07-20 - Created by Andrei Chelaru, reviewed by MLR
+ - 2017-10-09 - Updated by MLR.
 """
 
-from datetime import date, datetime
+from datetime import datetime
 
 from juriscraper.OralArgumentSite import OralArgumentSite
 
 
 class Site(OralArgumentSite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
-        d = date.today()
-        # d = date(month=5, day=1, year=2014)
-        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
-            yearmo=d.strftime("%Y%m")
+        self.url = (
+            "http://www.supremecourt.gov/oral_arguments/argument_audio.aspx"
         )
-        self.back_scrape_iterable = [
-            "%s%02d" % (year, month)
-            for year in range(2007, d.year + 1)
-            for month in range(1, 13)
-        ]
-
-    def _download(self, **kwargs):
-        # The certificate on their site has expired.
-        return super()._download(request_dict={"verify": False})
+        self.back_scrape_iterable = list(range(2010, 2015))
 
     def _get_download_urls(self):
-        path = "id('ViewBody')//div[contains(concat(' ',@class,' '),' row-entry')]//@href"
-        return list(self.html.xpath(path))
+        path = "id('list')//tr//a/text()"
+        return list(map(self._return_download_url, self.html.xpath(path)))
+
+    @staticmethod
+    def _return_download_url(d):
+        file_type = "mp3"  # or 'wma' is also available for any case.
+        download_url = "http://www.supremecourt.gov/media/audio/{type}files/{docket_number}.{type}".format(
+            type=file_type, docket_number=d
+        )
+        return download_url
 
     def _get_case_names(self):
-        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' column-two')]/div[1]/text()"
-        return list(self.html.xpath(path))
+        path = "id('list')//tr/td/span/text()"
+        return [s.lstrip(". ") for s in self.html.xpath(path)]
 
     def _get_case_dates(self):
-        path = "id('ViewBody')//date/text()"
-        return list(map(self._return_case_date, self.html.xpath(path)))
-
-    @staticmethod
-    def _return_case_date(e):
-        e = "".join(e.split())
-        return datetime.strptime(e, "%m/%d/%Y").date()
+        path = "id('list')//tr/td[2]//text()"
+        return [
+            datetime.strptime(s, "%m/%d/%y").date()
+            for s in self.html.xpath(path)
+            if not "Date" in s
+        ]
 
     def _get_docket_numbers(self):
-        path = "id('ViewBody')//*[contains(concat(' ',@class,' '),' row-entry')]//a//text()"
+        path = "id('list')//tr//a/text()"
         return list(self.html.xpath(path))
 
-    def _get_judges(self):
-        path = '//div[span[contains(., "Judges")]]/text()'
-        return [" ".join(s.split()) for s in self.html.xpath(path)]
-
-    def _download_backwards(self, yearmo):
-        self.url = "http://www.cadc.uscourts.gov/recordings/recordings.nsf/DocsByRDate?OpenView&count=100&SKey={yearmo}".format(
-            yearmo=yearmo,
+    def _download_backwards(self, year):
+        self.url = (
+            f"http://www.supremecourt.gov/oral_arguments/argument_audio/{year}"
         )
         self.html = self._download()
```

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/federal_appellate/cafc.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/state/ill.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/state/illappct_1st_dist.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/state/illappct_1st_dist.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/oral_args/united_states/state/md.py` & `juriscraper-2.5.9/juriscraper/oral_args/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/__init__.py` & `juriscraper-2.5.9/juriscraper/pacer/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/appellate_docket.py` & `juriscraper-2.5.9/juriscraper/pacer/appellate_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/attachment_page.py` & `juriscraper-2.5.9/juriscraper/pacer/attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/case_query.py` & `juriscraper-2.5.9/juriscraper/pacer/case_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/case_query_advanced.py` & `juriscraper-2.5.9/juriscraper/pacer/case_query_advanced.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/claims_register.py` & `juriscraper-2.5.9/juriscraper/pacer/claims_register.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/docket_history_report.py` & `juriscraper-2.5.9/juriscraper/pacer/docket_history_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/docket_report.py` & `juriscraper-2.5.9/juriscraper/pacer/docket_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/docket_utils.py` & `juriscraper-2.5.9/juriscraper/pacer/docket_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/email.py` & `juriscraper-2.5.9/juriscraper/pacer/email.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/free_documents.py` & `juriscraper-2.5.9/juriscraper/pacer/free_documents.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/hidden_api.py` & `juriscraper-2.5.9/juriscraper/pacer/hidden_api.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/http.py` & `juriscraper-2.5.9/juriscraper/pacer/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/internet_archive.py` & `juriscraper-2.5.9/juriscraper/pacer/internet_archive.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/mobile_query.py` & `juriscraper-2.5.9/juriscraper/pacer/mobile_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/reports.py` & `juriscraper-2.5.9/juriscraper/pacer/reports.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/rss_feeds.py` & `juriscraper-2.5.9/juriscraper/pacer/rss_feeds.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacer/utils.py` & `juriscraper-2.5.9/juriscraper/pacer/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/pacerdocket.py` & `juriscraper-2.5.9/juriscraper/pacerdocket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper/report.py` & `juriscraper-2.5.9/juriscraper/report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.8/juriscraper.egg-info/PKG-INFO` & `juriscraper-2.5.9/juriscraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.5.8
+Version: 2.5.9
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.5.8/juriscraper.egg-info/SOURCES.txt` & `juriscraper-2.5.9/juriscraper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,14 @@
 juriscraper/opinions/united_states_backscrapers/__init__.py
 juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
 juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
 juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
 juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
 juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
 juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
-juriscraper/opinions/united_states_backscrapers/federal_appellate/ca4.py
 juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
 juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
 juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
 juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
 juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
 juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
 juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
```

### Comparing `juriscraper-2.5.8/setup.py` & `juriscraper-2.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 import os
 import unittest
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-VERSION = "2.5.8"
+VERSION = "2.5.9"
 AUTHOR = "Free Law Project"
 EMAIL = "info@free.law"
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 reqs_path = f"{HERE}/requirements.txt"
 with open(reqs_path) as reqs_file:
```

