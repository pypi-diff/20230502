# Comparing `tmp/SMACT-2.5.0.tar.gz` & `tmp/SMACT-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMACT-2.5.0.tar", last modified: Thu Dec 22 20:01:40 2022, max compression
+gzip compressed data, was "SMACT-2.5.1.tar", last modified: Tue May  2 12:17:57 2023, max compression
```

## Comparing `SMACT-2.5.0.tar` & `SMACT-2.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:40.356661 SMACT-2.5.0/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1098 2021-11-05 10:17:45.000000 SMACT-2.5.0/LICENSE
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)       40 2021-11-05 10:17:45.000000 SMACT-2.5.0/MANIFEST.in
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    12646 2022-12-22 20:01:40.352659 SMACT-2.5.0/PKG-INFO
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    11915 2022-12-22 19:12:52.000000 SMACT-2.5.0/README.md
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:39.216662 SMACT-2.5.0/SMACT.egg-info/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    12646 2022-12-22 20:01:38.000000 SMACT-2.5.0/SMACT.egg-info/PKG-INFO
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1490 2022-12-22 20:01:38.000000 SMACT-2.5.0/SMACT.egg-info/SOURCES.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        1 2022-12-22 20:01:38.000000 SMACT-2.5.0/SMACT.egg-info/dependency_links.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        1 2022-10-07 08:25:52.000000 SMACT-2.5.0/SMACT.egg-info/not-zip-safe
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)       46 2022-12-22 20:01:38.000000 SMACT-2.5.0/SMACT.egg-info/requires.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        6 2022-12-22 20:01:38.000000 SMACT-2.5.0/SMACT.egg-info/top_level.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      294 2022-12-22 16:02:49.000000 SMACT-2.5.0/pyproject.toml
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)       38 2022-12-22 20:01:40.357662 SMACT-2.5.0/setup.cfg
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     2300 2022-12-22 20:01:07.000000 SMACT-2.5.0/setup.py
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:39.457664 SMACT-2.5.0/smact/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    17648 2022-12-22 16:49:52.000000 SMACT-2.5.0/smact/__init__.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     2416 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/builder.py
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:39.950658 SMACT-2.5.0/smact/data/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1755 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/Covalent_radii.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1811 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/HHIs.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1127 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/SSE.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      816 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/SSE_2015.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      813 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/SSE_Pauling.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    17321 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/element_data.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      854 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/ionic_radii.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      462 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/ordered_periodic.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    37149 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/oxidation_state_probability_table.json
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1696 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/oxidation_states.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      875 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/oxidation_states_SP.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1226 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/oxidation_states_icsd.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1053 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/oxidation_states_pmg.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1666 2022-09-23 09:25:53.000000 SMACT-2.5.0/smact/data/oxidation_states_wiki.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      962 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/oxidationstates.data
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    11433 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/shannon_radii.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    30745 2021-11-05 10:17:45.000000 SMACT-2.5.0/smact/data/shannon_radii_ML_extended.csv
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     2039 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/solid_properties.txt
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    43658 2021-02-11 09:13:29.000000 SMACT-2.5.0/smact/data/solid_properties.xlsx
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    24651 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/data_loader.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     3684 2022-12-20 16:30:47.000000 SMACT-2.5.0/smact/distorter.py
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:40.003660 SMACT-2.5.0/smact/dopant_prediction/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      353 2022-12-22 15:26:27.000000 SMACT-2.5.0/smact/dopant_prediction/__init__.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     6985 2022-12-22 18:56:01.000000 SMACT-2.5.0/smact/dopant_prediction/doper.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     1587 2022-12-20 16:30:47.000000 SMACT-2.5.0/smact/lattice.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     7624 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/lattice_parameters.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      234 2022-12-20 16:30:47.000000 SMACT-2.5.0/smact/mainpage.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     6819 2022-12-22 16:49:52.000000 SMACT-2.5.0/smact/oxidation_states.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     5219 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/properties.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    13660 2022-12-22 18:55:49.000000 SMACT-2.5.0/smact/screening.py
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:40.200658 SMACT-2.5.0/smact/structure_prediction/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)      374 2022-10-24 10:12:11.000000 SMACT-2.5.0/smact/structure_prediction/__init__.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     9573 2022-12-22 19:29:40.000000 SMACT-2.5.0/smact/structure_prediction/database.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    14853 2022-12-22 16:03:00.000000 SMACT-2.5.0/smact/structure_prediction/mutation.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    10052 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/structure_prediction/prediction.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     3657 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/structure_prediction/probability_models.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    22383 2022-12-22 19:29:40.000000 SMACT-2.5.0/smact/structure_prediction/structure.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     2362 2022-12-22 19:29:40.000000 SMACT-2.5.0/smact/structure_prediction/utilities.py
-drwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-12-22 20:01:40.321658 SMACT-2.5.0/smact/tests/
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)        0 2022-09-23 09:25:53.000000 SMACT-2.5.0/smact/tests/__init__.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    11774 2022-12-22 16:03:00.000000 SMACT-2.5.0/smact/tests/test_core.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)     2054 2022-12-22 16:02:59.000000 SMACT-2.5.0/smact/tests/test_doper.py
--rwxrwxrwx   0 aonwu     (1000) aonwu     (1000)    22153 2022-12-22 19:29:40.000000 SMACT-2.5.0/smact/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 12:17:42.000000 SMACT-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 12:17:42.000000 SMACT-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-02 12:17:57.055828 SMACT-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-05-02 12:17:42.000000 SMACT-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.043828 SMACT-2.5.1/SMACT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:17:56.000000 SMACT-2.5.1/SMACT.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 12:17:42.000000 SMACT-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:17:57.055828 SMACT-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-02 12:17:42.000000 SMACT-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.047828 SMACT-2.5.1/smact/
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.051828 SMACT-2.5.1/smact/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/Covalent_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/HHIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE_2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE_Pauling.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/element_data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/ionic_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/ordered_periodic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37149 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_state_probability_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_SP.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_icsd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_pmg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_wiki.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidationstates.data
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/shannon_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29754 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/shannon_radii_ML_extended.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/solid_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43658 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/solid_properties.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/distorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.051828 SMACT-2.5.1/smact/dopant_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/dopant_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/dopant_prediction/doper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/mainpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/oxidation_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/screening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/smact/structure_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/probability_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22383 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/smact/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12333 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_doper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_structure.py
```

### Comparing `SMACT-2.5.0/LICENSE` & `SMACT-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/PKG-INFO` & `SMACT-2.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMACT
-Version: 2.5.0
+Version: 2.5.1
 Summary: Semiconducting Materials by Analogy and Chemical Theory
 Home-page: https://github.com/WMD-group/SMACT
 Author: Daniel W. Davies
 Author-email: d.w.davies@imperial.ac.uk
 Maintainer: Anthony O. Onwuli
 Maintainer-email: anthony.onwuli16@imperial.ac.uk
 License: MIT
@@ -29,14 +29,16 @@
 [![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
 ![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
 [![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
 ![python version](https://img.shields.io/pypi/pyversions/smact)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
+[![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
 
 
 SMACT
 =====
 
 **Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
 
@@ -154,34 +156,14 @@
 ### Tests
 Testing modules should be pass/fail and wrapped into **tests/test_core.py** or another **tests/test_something.py** file added, if appropriate. 
 Run the tests using `python -m pytest -v`.
 (The final `-v` is optional and adds more detail to the output.)
 
 We also use integrated testing on Github via [GitHub Actions](hhttps://github.com/features/actions).
 
-### List of Developers
-Contributors to SMACT: 
-- Keith Butler
-- Daniel Davies
-- Jarvist Frost
-- Tim Gauntlet
-- Adam Jackson
-- Chloe (Jiwoo) Lee (이지우)
-- Alex Moriarty
-- Kazuki Morita
-- Anthony Onwuli
-- Jonathan Skelton
-- Aron Walsh
-
- Thanks to [JOSS](https://github.com/openjournals/joss-reviews/issues/1361) reviewers and editors: 
- - Adam Symington
- - Alex Ganose
- - Daniel Katz
- - Lorena Barba
-
 References
 ----------
 
 [D. W. Davies et al,
 "SMACT: Semiconducting Materials by Analogy and Chemical Theory" *JOSS* **4**, 1361 (2019)](https://joss.theoj.org/papers/7efd2f2ad60d25bdccee3fbd3fc11448)
 
 [D. W. Davies et al,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SMACT-2.5.0/README.md` & `SMACT-2.5.1/SMACT.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,177 +1,183 @@
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
-[![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
-[![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
-![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
-[![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
-![python version](https://img.shields.io/pypi/pyversions/smact)
-
-
-SMACT
-=====
-
-**Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
-
-- **Documentation:** https://smact.readthedocs.io/en/latest/
-- **Examples folder:** https://github.com/WMD-group/SMACT/tree/master/examples
-
-![](SMACT.png)
-
-*If you torture the data enough, nature will always confess* - Roland Coase (from 'How should economists choose?')
-
-Statement of need
---------
-There is a strong demand for functional materials across a wide range of technologies. The motivation can include cost reduction, performance enhancement, or to enable a new application. Data collections such as the [Materials Project](https://www.materialsproject.org), [NREL Materials Database](http://materials.nrel.gov) and the [Open Quantum Materials Database](http://oqmd.org) are valuable resources, but they largely cover the properties of *known* compounds as calculated using high-level quantum mechanical theories.
-
-We have developed low-cost procedures for screening hypothetical materials in SMACT. This framework can be used for simple calculations on your own computer. SMACT follows a top-down approach where a set of element combinations is generated and then screened using rapid chemical filters. It can be used as part of a multi-technique workflow or to feed machine learning models for materials.
-
-
-![](smact_simple.gif)
-
-
-Getting started
------
-
-SMACT's features are accessed through Python scripts, importing classes and functions as needed.
-The best place to start is looking at [the docs](https://smact.readthedocs.io/en/latest/), which highlight some simple examples of how these classes and functions can be used.
-Extended examples are available in [our examples folder](https://github.com/WMD-group/SMACT/tree/master/examples).
-
-Code features
---------
-- At the core of SMACT are [Element](https://smact.readthedocs.io/en/latest/smact.html#smact.Element) and [Species](https://smact.readthedocs.io/en/latest/smact.html#smact.Species) (element in a given oxidation state) classes that have various properties associated with them. 
-
-- The various oxidation states that are accessible to each element are included in their properties.
-
-- Element compositions can be screened through based on the heuristic filters of charge neutrality and electronegativity order. This is handled using the [screening module](https://smact.readthedocs.io/en/latest/smact.screening.html) and [this publication](https://www.cell.com/chem/fulltext/S2451-9294(16)30155-3) describes the underlying theory. An example procedure is [outlined in the docs](https://smact.readthedocs.io/en/latest/examples.html#neutral-combinations) and further examples can be found in the [counting examples subfolder](https://github.com/WMD-group/SMACT/tree/master/examples/Counting).
-
-- Further filters can be applied to generated lists of compositions in order to screen for particular properties. These properties are either intrinsic properties of elements or are calculated for compositions using the [properties module](https://smact.readthedocs.io/en/latest/smact.properties.html). For example: 
-  - A use case is shown in [this publication](https://pubs.rsc.org/en/content/articlehtml/2018/sc/c7sc03961a), in which 160,000 chemical compositions are screened based on optical band gap calculated using the [solid-state energy scale](https://www.sciencedirect.com/science/article/pii/S0022459615300888).
-  - The [oxidation_states module](https://smact.readthedocs.io/en/latest/smact.oxidation_states.html) can be used to filter out compositions containing metals in unlikely oxidation states according to [a data-driven model](https://pubs.rsc.org/en/content/articlelanding/2018/fd/c8fd00032h#!divAbstract).
-
-- Compositions can also be filtered based on sustainability via the abundance of elements in the Earth's crust or via the [HHI scale](https://pubs.acs.org/doi/10.1021/cm400893e). 
-
-- Compositions can easily be converted for use in Pymatgen or for representation to machine learning algorithms ([see "next steps" in this example](https://github.com/WMD-group/SMACT/blob/master/examples/Counting/Generate_compositions_lists.ipynb)).
-
-- The code also has some tools for manipulating common crystal lattice types: 
- - Common crystal structure types can be built using the [builder module](https://smact.readthedocs.io/en/latest/smact.builder.html)
- - Lattice parameters can be quickly estimated using ionic radii of the elements for various common crystal structure types using the [lattice_parameters module](https://smact.readthedocs.io/en/latest/smact.lattice_parameters.html).
- - The [lattice module](https://smact.readthedocs.io/en/latest/smact.lattice.html) and [distorter module](https://smact.readthedocs.io/en/latest/smact.distorter.html) rely on the [Atomic Simulation Environment](https://wiki.fysik.dtu.dk/ase/) and can be used to generate unique atomic substitutions on a given crystal structure.  
-
-List of modules
--------
-
-* **smact** library containing:
-  * **\_\_init\_\_.py** Contains the core `Element` and `Species` classes.
-  *  **data_loader.py** Handles the loading of external data used to initialise the core `smact.Element` and `smact.Species` classes.
-  *  **screening.py** Used for generating and applying filters to compositional search spaces.
-  *  **properties.py** A collection of tools for estimating useful properties based on composition.
-  * **lattice.py** Given the sites, multiplicities and possible oxidation states
-    at those sites, this reads from the database and generates all possible
-    stoichiometeries.
-  * **builder.py** Builds some common lattice structures, given the chemical
-    composition.
-  * **lattice_parameters.py** Estimation of lattice parameters for various lattice types using covalent/ionic radii.
-  * **distorter.py** A collection of functions for enumerating and then
-    substituting on inequivalent sites of a sub-lattice.
-
-Requirements
-------------
-
-The main language is Python 3 and has been tested using Python 3.8+.
-Basic requirements are Numpy and Scipy.
-The [Atomic Simulation Environment](https://wiki.fysik.dtu.dk/ase) (ASE),  [spglib](http://atztogo.github.io/spglib), and [pymatgen](www.pymatgen.org) are also required for many components.
-
-Installation
-------------
-The latest stable release of SMACT can be installed via pip which will automatically setup other Python packages as required:
-
-    pip install smact  
-
-Alternatively, the very latest version can be installed using:
-
-    pip install git+git://github.com/WMD-group/SMACT.git
-
-For developer installation SMACT can be installed from a copy of the source
-repository (https://github.com/wmd-group/smact); this will be preferred if using experimental code branches.
-
-To clone the project from Github and make a local installation:
-
-    git clone https://github.com/wmd-group/smact.git
-    cd smact
-    pip install --user -e .
-
-With -e pip will create links to the source folder so that that changes
-to the code will be immediately reflected on the PATH.
-
-
-License and attribution
------------------------
-
-Python code and original data tables are licensed under the MIT License.
-
-Development notes
------------------
-
-### Bugs, features and questions
-Please use the [Issue Tracker](https://github.com/WMD-group/smact/issues) to report bugs or request features in the first instance. While we hope that most questions can be answered by searching [the docs](https://smact.readthedocs.io/en/latest/), we welcome new questions on the issue tracker, especially if they helps us improve the docs! For other queries about any aspect of the code, please contact either Dan Davies (author) or Anthony Onwuli (maintainer) by e-mail: d.w.davies@imperial.ac.uk or anthony.onwuli16@imperial.ac.uk respectively.
-
-### Code contributions
-We are always looking for ways to make SMACT better and more useful to the wider community; contributions are very welcome. Please use the ["Fork and Pull"](https://guides.github.com/activities/forking/) workflow to make contributions and stick as closely as possible to the following:
-
-- Code style should comply with [PEP8](http://www.python.org/dev/peps/pep-0008) where possible. [Google's house style](https://google.github.io/styleguide/pyguide.html)
-is also helpful, including a good model for docstrings.
-- Please use comments liberally when adding nontrivial features, and take the chance to clean up other people's code while looking at it.
-- Add tests wherever possible, and use the test suite to check if you broke anything.
-
-### Tests
-Testing modules should be pass/fail and wrapped into **tests/test_core.py** or another **tests/test_something.py** file added, if appropriate. 
-Run the tests using `python -m pytest -v`.
-(The final `-v` is optional and adds more detail to the output.)
-
-We also use integrated testing on Github via [GitHub Actions](hhttps://github.com/features/actions).
-
-### List of Developers
-Contributors to SMACT: 
-- Keith Butler
-- Daniel Davies
-- Jarvist Frost
-- Tim Gauntlet
-- Adam Jackson
-- Chloe (Jiwoo) Lee (이지우)
-- Alex Moriarty
-- Kazuki Morita
-- Anthony Onwuli
-- Jonathan Skelton
-- Aron Walsh
-
- Thanks to [JOSS](https://github.com/openjournals/joss-reviews/issues/1361) reviewers and editors: 
- - Adam Symington
- - Alex Ganose
- - Daniel Katz
- - Lorena Barba
-
-References
-----------
-
-[D. W. Davies et al,
-"SMACT: Semiconducting Materials by Analogy and Chemical Theory" *JOSS* **4**, 1361 (2019)](https://joss.theoj.org/papers/7efd2f2ad60d25bdccee3fbd3fc11448)
-
-[D. W. Davies et al, 
-"Data-driven discovery of photoactive quaternary oxides using first-principles machine learning" *Chem. Mater.* **31**, 7221 (2019)](https://pubs.acs.org/doi/abs/10.1021/acs.chemmater.9b01519)
-
-[D. W. Davies et al,
-"Materials discovery by chemical analogy: role of oxidation states in structure prediction" *Faraday Discuss.* **211**, 553 (2018)](https://pubs.rsc.org/en/Content/ArticleLanding/2018/FD/C8FD00032H)
-
-[D. W. Davies et al,
-"Computer-aided design of metal chalcohalide semiconductors: from chemical composition to crystal structure" *Chem. Sci.* **9**, 1022 (2018)](http://www.cell.com/chem/abstract/S2451-9294(16)30155-3)
-
-[D. W. Davies et al,
-"Computational screening of all stoichiometric inorganic materials" *Chem* **1**, 617 (2016)](http://www.cell.com/chem/abstract/S2451-9294(16)30155-3)
-
-[B. R. Pamplin, "A systematic method of deriving new semiconducting
-compounds by structural analogy", *J. Phys. Chem. Solids*
-**25**, 675 (1964)](http://www.sciencedirect.com/science/article/pii/0022369764901763)
+Metadata-Version: 2.1
+Name: SMACT
+Version: 2.5.1
+Summary: Semiconducting Materials by Analogy and Chemical Theory
+Home-page: https://github.com/WMD-group/SMACT
+Author: Daniel W. Davies
+Author-email: d.w.davies@imperial.ac.uk
+Maintainer: Anthony O. Onwuli
+Maintainer-email: anthony.onwuli16@imperial.ac.uk
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
+[![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
+[![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
+![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
+[![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
+![python version](https://img.shields.io/pypi/pyversions/smact)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
+[![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
+
+
+SMACT
+=====
+
+**Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
+
+- **Documentation:** https://smact.readthedocs.io/en/latest/
+- **Examples folder:** https://github.com/WMD-group/SMACT/tree/master/examples
+
+![](SMACT.png)
+
+*If you torture the data enough, nature will always confess* - Roland Coase (from 'How should economists choose?')
+
+Statement of need
+--------
+There is a strong demand for functional materials across a wide range of technologies. The motivation can include cost reduction, performance enhancement, or to enable a new application. Data collections such as the [Materials Project](https://www.materialsproject.org), [NREL Materials Database](http://materials.nrel.gov) and the [Open Quantum Materials Database](http://oqmd.org) are valuable resources, but they largely cover the properties of *known* compounds as calculated using high-level quantum mechanical theories.
+
+We have developed low-cost procedures for screening hypothetical materials in SMACT. This framework can be used for simple calculations on your own computer. SMACT follows a top-down approach where a set of element combinations is generated and then screened using rapid chemical filters. It can be used as part of a multi-technique workflow or to feed machine learning models for materials.
+
+
+![](smact_simple.gif)
+
+
+Getting started
+-----
+
+SMACT's features are accessed through Python scripts, importing classes and functions as needed.
+The best place to start is looking at [the docs](https://smact.readthedocs.io/en/latest/), which highlight some simple examples of how these classes and functions can be used.
+Extended examples are available in [our examples folder](https://github.com/WMD-group/SMACT/tree/master/examples).
+
+Code features
+--------
+- At the core of SMACT are [Element](https://smact.readthedocs.io/en/latest/smact.html#smact.Element) and [Species](https://smact.readthedocs.io/en/latest/smact.html#smact.Species) (element in a given oxidation state) classes that have various properties associated with them. 
+
+- The various oxidation states that are accessible to each element are included in their properties.
+
+- Element compositions can be screened through based on the heuristic filters of charge neutrality and electronegativity order. This is handled using the [screening module](https://smact.readthedocs.io/en/latest/smact.screening.html) and [this publication](https://www.cell.com/chem/fulltext/S2451-9294(16)30155-3) describes the underlying theory. An example procedure is [outlined in the docs](https://smact.readthedocs.io/en/latest/examples.html#neutral-combinations) and further examples can be found in the [counting examples subfolder](https://github.com/WMD-group/SMACT/tree/master/examples/Counting).
+
+- Further filters can be applied to generated lists of compositions in order to screen for particular properties. These properties are either intrinsic properties of elements or are calculated for compositions using the [properties module](https://smact.readthedocs.io/en/latest/smact.properties.html). For example: 
+  - A use case is shown in [this publication](https://pubs.rsc.org/en/content/articlehtml/2018/sc/c7sc03961a), in which 160,000 chemical compositions are screened based on optical band gap calculated using the [solid-state energy scale](https://www.sciencedirect.com/science/article/pii/S0022459615300888).
+  - The [oxidation_states module](https://smact.readthedocs.io/en/latest/smact.oxidation_states.html) can be used to filter out compositions containing metals in unlikely oxidation states according to [a data-driven model](https://pubs.rsc.org/en/content/articlelanding/2018/fd/c8fd00032h#!divAbstract).
+
+- Compositions can also be filtered based on sustainability via the abundance of elements in the Earth's crust or via the [HHI scale](https://pubs.acs.org/doi/10.1021/cm400893e). 
+
+- Compositions can easily be converted for use in Pymatgen or for representation to machine learning algorithms ([see "next steps" in this example](https://github.com/WMD-group/SMACT/blob/master/examples/Counting/Generate_compositions_lists.ipynb)).
+
+- The code also has some tools for manipulating common crystal lattice types: 
+ - Common crystal structure types can be built using the [builder module](https://smact.readthedocs.io/en/latest/smact.builder.html)
+ - Lattice parameters can be quickly estimated using ionic radii of the elements for various common crystal structure types using the [lattice_parameters module](https://smact.readthedocs.io/en/latest/smact.lattice_parameters.html).
+ - The [lattice module](https://smact.readthedocs.io/en/latest/smact.lattice.html) and [distorter module](https://smact.readthedocs.io/en/latest/smact.distorter.html) rely on the [Atomic Simulation Environment](https://wiki.fysik.dtu.dk/ase/) and can be used to generate unique atomic substitutions on a given crystal structure.  
+
+List of modules
+-------
+
+* **smact** library containing:
+  * **\_\_init\_\_.py** Contains the core `Element` and `Species` classes.
+  *  **data_loader.py** Handles the loading of external data used to initialise the core `smact.Element` and `smact.Species` classes.
+  *  **screening.py** Used for generating and applying filters to compositional search spaces.
+  *  **properties.py** A collection of tools for estimating useful properties based on composition.
+  * **lattice.py** Given the sites, multiplicities and possible oxidation states
+    at those sites, this reads from the database and generates all possible
+    stoichiometeries.
+  * **builder.py** Builds some common lattice structures, given the chemical
+    composition.
+  * **lattice_parameters.py** Estimation of lattice parameters for various lattice types using covalent/ionic radii.
+  * **distorter.py** A collection of functions for enumerating and then
+    substituting on inequivalent sites of a sub-lattice.
+
+Requirements
+------------
+
+The main language is Python 3 and has been tested using Python 3.8+.
+Basic requirements are Numpy and Scipy.
+The [Atomic Simulation Environment](https://wiki.fysik.dtu.dk/ase) (ASE),  [spglib](http://atztogo.github.io/spglib), and [pymatgen](www.pymatgen.org) are also required for many components.
+
+Installation
+------------
+The latest stable release of SMACT can be installed via pip which will automatically setup other Python packages as required:
+
+    pip install smact  
+
+Alternatively, the very latest version can be installed using:
+
+    pip install git+git://github.com/WMD-group/SMACT.git
+
+For developer installation SMACT can be installed from a copy of the source
+repository (https://github.com/wmd-group/smact); this will be preferred if using experimental code branches.
+
+To clone the project from Github and make a local installation:
+
+    git clone https://github.com/wmd-group/smact.git
+    cd smact
+    pip install --user -e .
+
+With -e pip will create links to the source folder so that that changes
+to the code will be immediately reflected on the PATH.
+
+
+License and attribution
+-----------------------
+
+Python code and original data tables are licensed under the MIT License.
+
+Development notes
+-----------------
+
+### Bugs, features and questions
+Please use the [Issue Tracker](https://github.com/WMD-group/smact/issues) to report bugs or request features in the first instance. While we hope that most questions can be answered by searching [the docs](https://smact.readthedocs.io/en/latest/), we welcome new questions on the issue tracker, especially if they helps us improve the docs! For other queries about any aspect of the code, please contact either Dan Davies (author) or Anthony Onwuli (maintainer) by e-mail: d.w.davies@imperial.ac.uk or anthony.onwuli16@imperial.ac.uk respectively.
+
+### Code contributions
+We are always looking for ways to make SMACT better and more useful to the wider community; contributions are very welcome. Please use the ["Fork and Pull"](https://guides.github.com/activities/forking/) workflow to make contributions and stick as closely as possible to the following:
+
+- Code style should comply with [PEP8](http://www.python.org/dev/peps/pep-0008) where possible. [Google's house style](https://google.github.io/styleguide/pyguide.html)
+is also helpful, including a good model for docstrings.
+- Please use comments liberally when adding nontrivial features, and take the chance to clean up other people's code while looking at it.
+- Add tests wherever possible, and use the test suite to check if you broke anything.
+
+### Tests
+Testing modules should be pass/fail and wrapped into **tests/test_core.py** or another **tests/test_something.py** file added, if appropriate. 
+Run the tests using `python -m pytest -v`.
+(The final `-v` is optional and adds more detail to the output.)
+
+We also use integrated testing on Github via [GitHub Actions](hhttps://github.com/features/actions).
+
+References
+----------
+
+[D. W. Davies et al,
+"SMACT: Semiconducting Materials by Analogy and Chemical Theory" *JOSS* **4**, 1361 (2019)](https://joss.theoj.org/papers/7efd2f2ad60d25bdccee3fbd3fc11448)
+
+[D. W. Davies et al, 
+"Data-driven discovery of photoactive quaternary oxides using first-principles machine learning" *Chem. Mater.* **31**, 7221 (2019)](https://pubs.acs.org/doi/abs/10.1021/acs.chemmater.9b01519)
+
+[D. W. Davies et al,
+"Materials discovery by chemical analogy: role of oxidation states in structure prediction" *Faraday Discuss.* **211**, 553 (2018)](https://pubs.rsc.org/en/Content/ArticleLanding/2018/FD/C8FD00032H)
+
+[D. W. Davies et al,
+"Computer-aided design of metal chalcohalide semiconductors: from chemical composition to crystal structure" *Chem. Sci.* **9**, 1022 (2018)](http://www.cell.com/chem/abstract/S2451-9294(16)30155-3)
+
+[D. W. Davies et al,
+"Computational screening of all stoichiometric inorganic materials" *Chem* **1**, 617 (2016)](http://www.cell.com/chem/abstract/S2451-9294(16)30155-3)
+
+[B. R. Pamplin, "A systematic method of deriving new semiconducting
+compounds by structural analogy", *J. Phys. Chem. Solids*
+**25**, 675 (1964)](http://www.sciencedirect.com/science/article/pii/0022369764901763)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SMACT-2.5.0/SMACT.egg-info/PKG-INFO` & `SMACT-2.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,20 @@
-Metadata-Version: 2.1
-Name: SMACT
-Version: 2.5.0
-Summary: Semiconducting Materials by Analogy and Chemical Theory
-Home-page: https://github.com/WMD-group/SMACT
-Author: Daniel W. Davies
-Author-email: d.w.davies@imperial.ac.uk
-Maintainer: Anthony O. Onwuli
-Maintainer-email: anthony.onwuli16@imperial.ac.uk
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
 [![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
 ![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
 [![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
 ![python version](https://img.shields.io/pypi/pyversions/smact)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
+[![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
 
 
 SMACT
 =====
 
 **Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
 
@@ -154,34 +132,14 @@
 ### Tests
 Testing modules should be pass/fail and wrapped into **tests/test_core.py** or another **tests/test_something.py** file added, if appropriate. 
 Run the tests using `python -m pytest -v`.
 (The final `-v` is optional and adds more detail to the output.)
 
 We also use integrated testing on Github via [GitHub Actions](hhttps://github.com/features/actions).
 
-### List of Developers
-Contributors to SMACT: 
-- Keith Butler
-- Daniel Davies
-- Jarvist Frost
-- Tim Gauntlet
-- Adam Jackson
-- Chloe (Jiwoo) Lee (이지우)
-- Alex Moriarty
-- Kazuki Morita
-- Anthony Onwuli
-- Jonathan Skelton
-- Aron Walsh
-
- Thanks to [JOSS](https://github.com/openjournals/joss-reviews/issues/1361) reviewers and editors: 
- - Adam Symington
- - Alex Ganose
- - Daniel Katz
- - Lorena Barba
-
 References
 ----------
 
 [D. W. Davies et al,
 "SMACT: Semiconducting Materials by Analogy and Chemical Theory" *JOSS* **4**, 1361 (2019)](https://joss.theoj.org/papers/7efd2f2ad60d25bdccee3fbd3fc11448)
 
 [D. W. Davies et al,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SMACT-2.5.0/SMACT.egg-info/SOURCES.txt` & `SMACT-2.5.1/SMACT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/setup.py` & `SMACT-2.5.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#!/usr/bin/env python
-
-__author__ = "Daniel W. Davies"
-__author_email__ = "d.w.davies@imperial.ac.uk"
-__copyright__ = (
-    "Copyright Daniel W. Davies, Adam J. Jackson, Keith T. Butler (2019)"
-)
-__version__ = "2.5.0"
-__maintainer__ = "Anthony O. Onwuli"
-__maintaier_email__ = "anthony.onwuli16@imperial.ac.uk"
-__date__ = "December 22 2022"
-
-import os
-import unittest
-
-from setuptools import Extension, setup
-
-module_dir = os.path.dirname(os.path.abspath(__file__))
-
-if __name__ == "__main__":
-    setup(
-        name="SMACT",
-        version=__version__,
-        description="Semiconducting Materials by Analogy and Chemical Theory",
-        long_description=open(os.path.join(module_dir, "README.md")).read(),
-        long_description_content_type="text/markdown",
-        url="https://github.com/WMD-group/SMACT",
-        author=__author__,
-        author_email=__author_email__,
-        maintainer=__maintainer__,
-        maintainer_email=__maintaier_email__,
-        license="MIT",
-        packages=[
-            "smact",
-            "smact.tests",
-            "smact.structure_prediction",
-            "smact.dopant_prediction",
-        ],
-        package_data={
-            "smact": [
-                "data/*.txt",
-                "data/*.csv",
-                "data/*.data",
-                "data/*.xlsx",
-                "data/*.json",
-            ]
-        },
-        zip_safe=False,
-        test_suite="smact.tests.test",
-        install_requires=[
-            "scipy",
-            "numpy",
-            "spglib",
-            "pymatgen",
-            "ase",
-            "pandas",
-            "pathos",
-        ],
-        classifiers=[
-            "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3.10",
-            "Development Status :: 5 - Production/Stable",
-            "Intended Audience :: Science/Research",
-            "Operating System :: OS Independent",
-            "License :: OSI Approved :: MIT License",
-            "Topic :: Scientific/Engineering",
-            "Topic :: Scientific/Engineering :: Chemistry",
-        ],
-        python_requires=">=3.8",
-    )
+#!/usr/bin/env python
+
+__author__ = "Daniel W. Davies"
+__author_email__ = "d.w.davies@imperial.ac.uk"
+__copyright__ = (
+    "Copyright Daniel W. Davies, Adam J. Jackson, Keith T. Butler (2019)"
+)
+__version__ = "2.5.1"
+__maintainer__ = "Anthony O. Onwuli"
+__maintaier_email__ = "anthony.onwuli16@imperial.ac.uk"
+__date__ = "May 2 2023"
+
+import os
+import unittest
+
+from setuptools import Extension, setup
+
+module_dir = os.path.dirname(os.path.abspath(__file__))
+
+if __name__ == "__main__":
+    setup(
+        name="SMACT",
+        version=__version__,
+        description="Semiconducting Materials by Analogy and Chemical Theory",
+        long_description=open(os.path.join(module_dir, "README.md")).read(),
+        long_description_content_type="text/markdown",
+        url="https://github.com/WMD-group/SMACT",
+        author=__author__,
+        author_email=__author_email__,
+        maintainer=__maintainer__,
+        maintainer_email=__maintaier_email__,
+        license="MIT",
+        packages=[
+            "smact",
+            "smact.tests",
+            "smact.structure_prediction",
+            "smact.dopant_prediction",
+        ],
+        package_data={
+            "smact": [
+                "data/*.txt",
+                "data/*.csv",
+                "data/*.data",
+                "data/*.xlsx",
+                "data/*.json",
+            ]
+        },
+        zip_safe=False,
+        test_suite="smact.tests.test",
+        install_requires=[
+            "scipy",
+            "numpy",
+            "spglib",
+            "pymatgen",
+            "ase",
+            "pandas",
+            "pathos",
+        ],
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Development Status :: 5 - Production/Stable",
+            "Intended Audience :: Science/Research",
+            "Operating System :: OS Independent",
+            "License :: OSI Approved :: MIT License",
+            "Topic :: Scientific/Engineering",
+            "Topic :: Scientific/Engineering :: Chemistry",
+        ],
+        python_requires=">=3.8",
+    )
```

### Comparing `SMACT-2.5.0/smact/__init__.py` & `SMACT-2.5.1/smact/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
         self.coordination = coordination
 
         # Get shannon radius for the oxidation state and coordination.
 
         self.shannon_radius = None
 
         if radii_source == "shannon":
-
             shannon_data = data_loader.lookup_element_shannon_radius_data(
                 symbol
             )
 
         elif radii_source == "extended":
             shannon_data = (
                 data_loader.lookup_element_shannon_radius_data_extendedML(
@@ -388,15 +387,15 @@
         stoichs (tuple): Stoichiometry values corresponding to `oxidations`
     """
     return 0 == sum(map(multiply, oxidations, stoichs))
 
 
 def neutral_ratios_iter(
     oxidations: List[int],
-    stoichs: Union[bool, List[int]] = False,
+    stoichs: Union[bool, List[List[int]]] = False,
     threshold: Optional[int] = 5,
 ):
     """
     Iterator for charge-neutral stoichiometries
 
     Given a list of oxidation states of arbitrary length, yield ratios in which
     these form a charge-neutral compound. Stoichiometries may be provided as a
@@ -421,15 +420,17 @@
         lambda x: _isneutral(oxidations, x) and _gcd_recursive(*x) == 1,
         # Generator: enumerate all combinations of stoichiometry
         itertools.product(*stoichs),
     )
 
 
 def neutral_ratios(
-    oxidations: List[int], stoichs: Union[bool, List[int]] = False, threshold=5
+    oxidations: List[int],
+    stoichs: Union[bool, List[List[int]]] = False,
+    threshold=5,
 ):
     """
     Get a list of charge-neutral compounds
 
     Given a list of oxidation states of arbitrary length, yield ratios in which
     these form a charge-neutral compound. Stoichiometries may be provided as a
     set of legal stoichiometries per site (e.g. a known family of compounds);
```

### Comparing `SMACT-2.5.0/smact/builder.py` & `SMACT-2.5.1/smact/builder.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/Covalent_radii.csv` & `SMACT-2.5.1/smact/data/Covalent_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/HHIs.txt` & `SMACT-2.5.1/smact/data/HHIs.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/SSE.csv` & `SMACT-2.5.1/smact/data/SSE.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/SSE_2015.csv` & `SMACT-2.5.1/smact/data/SSE_2015.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/SSE_Pauling.csv` & `SMACT-2.5.1/smact/data/SSE_Pauling.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/element_data.txt` & `SMACT-2.5.1/smact/data/element_data.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/ionic_radii.csv` & `SMACT-2.5.1/smact/data/ionic_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_state_probability_table.json` & `SMACT-2.5.1/smact/data/oxidation_state_probability_table.json`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_states.txt` & `SMACT-2.5.1/smact/data/oxidation_states.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_states_SP.txt` & `SMACT-2.5.1/smact/data/oxidation_states_SP.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_states_icsd.txt` & `SMACT-2.5.1/smact/data/oxidation_states_icsd.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_states_pmg.txt` & `SMACT-2.5.1/smact/data/oxidation_states_pmg.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidation_states_wiki.txt` & `SMACT-2.5.1/smact/data/oxidation_states_wiki.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/oxidationstates.data` & `SMACT-2.5.1/smact/data/oxidationstates.data`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/shannon_radii.csv` & `SMACT-2.5.1/smact/data/shannon_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/shannon_radii_ML_extended.csv` & `SMACT-2.5.1/smact/data/shannon_radii_ML_extended.csv`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,991 +1,991 @@
-ion,charge,coordination,crystal_radius,ionic_radius,reference
-Ac,3,6,1.2600000000000002,1.12,Shannon
-Ac,3,8,1.392,1.252,ML Work
-Ag,2,2,0.6920000000000001,0.552,ML Work
-Ag,1,1,0.703,0.563,ML Work
-Ag,1,2,0.81,0.67,Shannon
-Ag,3,4,0.81,0.67,Shannon
-Ag,3,6,0.89,0.75,Shannon
-Ag,2,4,0.93,0.79,Shannon
-Ag,1,3,0.984,0.844,ML Work
-Ag,3,8,1.022,0.882,ML Work
-Ag,2,6,1.08,0.94,Shannon
-Ag,1,4,1.1400000000000001,1.0,Shannon
-Ag,2,8,1.2160000000000002,1.076,ML Work
-Ag,1,5,1.23,1.09,Shannon
-Ag,1,6,1.29,1.15,Shannon
-Ag,1,7,1.3599999999999999,1.22,Shannon
-Ag,1,8,1.42,1.28,Shannon
-Ag,1,9,1.4900000000000002,1.35,ML Work
-Ag,1,10,1.5550000000000002,1.415,ML Work
-Ag,1,11,1.6190000000000002,1.479,ML Work
-Ag,1,12,1.682,1.542,ML Work
-Al,3,3,0.453,0.313,ML Work
-Al,3,4,0.53,0.39,Shannon
-Al,3,5,0.62,0.48,Shannon
-Al,3,6,0.675,0.535,Shannon
-Al,3,7,0.751,0.611,ML Work
-Am,4,6,0.99,0.85,Shannon
-Am,4,8,1.0899999999999999,0.95,Shannon
-Am,3,6,1.115,0.975,Shannon
-Am,3,8,1.23,1.09,Shannon
-Am,2,7,1.35,1.21,Shannon
-Am,2,8,1.4,1.26,Shannon
-Am,2,9,1.4500000000000002,1.31,Shannon
-As,5,3,0.395,0.255,ML Work
-As,5,4,0.47500000000000003,0.335,Shannon
-As,5,5,0.535,0.395,ML Work
-As,3,3,0.5529999999999999,0.413,ML Work
-As,5,6,0.6000000000000001,0.46,Shannon
-As,3,4,0.611,0.471,ML Work
-As,3,5,0.664,0.524,ML Work
-As,5,8,0.717,0.577,ML Work
-As,3,6,0.72,0.58,Shannon
-At,7,6,0.76,0.62,Shannon
-Au,5,6,0.71,0.57,Shannon
-Au,3,4,0.8200000000000001,0.68,Shannon
-Au,2,3,0.847,0.707,ML Work
-Au,3,5,0.902,0.762,ML Work
-Au,3,6,0.99,0.85,Shannon
-Au,1,2,1.0,0.86,ML Work
-Au,3,8,1.1059999999999999,0.966,ML Work
-Au,3,10,1.23,1.09,ML Work
-Au,3,12,1.3559999999999999,1.216,ML Work
-Au,1,6,1.5100000000000002,1.37,Shannon
-B,3,3,0.15000000000000002,0.01,Shannon
-B,3,4,0.25,0.11,Shannon
-B,3,5,0.328,0.188,ML Work
-B,3,6,0.41000000000000003,0.27,Shannon
-Ba,2,1,1.119,0.979,ML Work
-Ba,2,2,1.193,1.053,ML Work
-Ba,2,3,1.2679999999999998,1.128,ML Work
-Ba,2,4,1.343,1.203,ML Work
-Ba,2,5,1.4140000000000001,1.274,ML Work
-Ba,2,6,1.4900000000000002,1.35,Shannon
-Ba,2,7,1.52,1.38,Shannon
-Ba,2,8,1.56,1.42,Shannon
-Ba,2,9,1.6099999999999999,1.47,Shannon
-Ba,2,10,1.6600000000000001,1.52,Shannon
-Ba,2,11,1.71,1.57,Shannon
-Ba,2,12,1.75,1.61,Shannon
-Be,2,3,0.30000000000000004,0.16,Shannon
-Be,2,4,0.41000000000000003,0.27,Shannon
-Be,2,5,0.499,0.359,ML Work
-Be,2,6,0.5900000000000001,0.45,Shannon
-Bi,5,2,0.5589999999999999,0.419,ML Work
-Bi,5,4,0.732,0.592,ML Work
-Bi,3,1,0.754,0.614,ML Work
-Bi,5,5,0.8160000000000001,0.676,ML Work
-Bi,3,2,0.845,0.705,ML Work
-Bi,5,6,0.9,0.76,Shannon
-Bi,3,3,0.935,0.795,ML Work
-Bi,5,8,1.018,0.878,ML Work
-Bi,3,4,1.02,0.88,ML Work
-Bi,3,5,1.1,0.96,Shannon
-Bi,3,6,1.17,1.03,Shannon
-Bi,3,7,1.237,1.097,ML Work
-Bi,3,8,1.31,1.17,Shannon
-Bi,3,9,1.3599999999999999,1.22,ML Work
-Bi,3,10,1.415,1.275,ML Work
-Bi,3,11,1.4700000000000002,1.33,ML Work
-Bi,3,12,1.525,1.385,ML Work
-Bk,4,6,0.97,0.83,Shannon
-Bk,4,8,1.07,0.93,Shannon
-Bk,3,6,1.1,0.96,Shannon
-Br,7,4,0.39,0.25,Shannon
-Br,5,3,0.45,0.31,Shannon
-Br,7,6,0.53,0.39,Shannon
-Br,3,4,0.73,0.59,Shannon
-Br,5,6,0.775,0.635,ML Work
-Br,1,2,1.161,1.021,ML Work
-Br,-1,6,1.8199999999999998,1.96,Shannon
-C,3,2,0.167,0.027,ML Work
-C,4,3,0.21000000000000002,0.07,ML Work
-C,3,3,0.22400000000000003,0.084,ML Work
-C,2,1,0.245,0.105,ML Work
-C,4,4,0.29000000000000004,0.15,Shannon
-C,2,2,0.29600000000000004,0.156,ML Work
-C,4,6,0.30000000000000004,0.16,Shannon
-Ca,2,1,0.741,0.601,ML Work
-Ca,2,2,0.8250000000000001,0.685,ML Work
-Ca,2,3,0.909,0.769,ML Work
-Ca,2,4,0.99,0.85,ML Work
-Ca,2,5,1.0670000000000002,0.927,ML Work
-Ca,2,6,1.1400000000000001,1.0,Shannon
-Ca,2,7,1.2000000000000002,1.06,Shannon
-Ca,2,8,1.2600000000000002,1.12,Shannon
-Ca,2,9,1.3199999999999998,1.18,Shannon
-Ca,2,10,1.37,1.23,Shannon
-Ca,2,11,1.4260000000000002,1.286,ML Work
-Ca,2,12,1.48,1.34,Shannon
-Cd,2,2,0.726,0.586,ML Work
-Cd,2,3,0.83,0.69,ML Work
-Cd,2,4,0.92,0.78,Shannon
-Cd,2,5,1.01,0.87,Shannon
-Cd,2,6,1.0899999999999999,0.95,Shannon
-Cd,2,7,1.17,1.03,Shannon
-Cd,2,8,1.2400000000000002,1.1,Shannon
-Cd,2,9,1.291,1.151,ML Work
-Cd,2,10,1.3439999999999999,1.204,ML Work
-Cd,2,12,1.4500000000000002,1.31,Shannon
-Ce,3,2,0.912,0.772,ML Work
-Ce,4,6,1.01,0.87,Shannon
-Ce,3,4,1.0350000000000001,0.895,ML Work
-Ce,4,7,1.053,0.913,ML Work
-Ce,3,5,1.093,0.953,ML Work
-Ce,4,8,1.1099999999999999,0.97,Shannon
-Ce,3,6,1.15,1.01,Shannon
-Ce,4,9,1.1629999999999998,1.023,ML Work
-Ce,3,7,1.21,1.07,Shannon
-Ce,4,10,1.21,1.07,Shannon
-Ce,4,12,1.2799999999999998,1.14,Shannon
-Ce,3,8,1.283,1.143,Shannon
-Ce,3,9,1.3359999999999999,1.196,Shannon
-Ce,2,6,1.375,1.235,ML Work
-Ce,3,10,1.3900000000000001,1.25,Shannon
-Ce,3,11,1.4129999999999998,1.273,ML Work
-Ce,3,12,1.48,1.34,Shannon
-Cf,4,6,0.961,0.821,Shannon
-Cf,4,8,1.06,0.92,Shannon
-Cf,3,6,1.0899999999999999,0.95,Shannon
-Cl,5,2,0.192,0.052,ML Work
-Cl,7,4,0.22000000000000003,0.08,Shannon
-Cl,5,3,0.26,0.12,Shannon
-Cl,4,2,0.339,0.199,ML Work
-Cl,7,6,0.41000000000000003,0.27,Shannon
-Cl,1,1,1.083,0.943,ML Work
-Cl,1,2,1.137,0.997,ML Work
-Cl,-1,6,1.67,1.81,Shannon
-Cm,4,6,0.99,0.85,Shannon
-Cm,4,8,1.0899999999999999,0.95,Shannon
-Cm,3,6,1.1099999999999999,0.97,Shannon
-Co,3,1,0.398,0.258,ML Work
-Co,4,4,0.54,0.4,Shannon
-Co,3,3,0.55,0.41,ML Work
-Co,2,2,0.552,0.412,ML Work
-Co,4,5,0.607,0.467,ML Work
-Co,3,4,0.612,0.472,ML Work
-Co,1,2,0.627,0.487,ML Work
-Co,2,3,0.636,0.496,ML Work
-Co,3,5,0.666,0.526,ML Work
-Co,4,6,0.67,0.53,Shannon
-Co,3,6,0.685,0.545,Shannon
-Co,2,4,0.72,0.58,Shannon
-Co,2,6,0.79,0.65,Shannon
-Co,3,7,0.795,0.655,ML Work
-Co,2,5,0.81,0.67,Shannon
-Co,2,7,0.922,0.782,ML Work
-Co,2,8,1.04,0.9,Shannon
-Co,2,9,1.135,0.995,ML Work
-Cr,5,3,0.394,0.254,ML Work
-Cr,6,4,0.4,0.26,Shannon
-Cr,5,4,0.485,0.345,Shannon
-Cr,6,5,0.495,0.355,ML Work
-Cr,3,2,0.515,0.375,ML Work
-Cr,4,4,0.55,0.41,Shannon
-Cr,5,5,0.5609999999999999,0.421,ML Work
-Cr,6,6,0.5800000000000001,0.44,Shannon
-Cr,4,5,0.625,0.485,ML Work
-Cr,5,6,0.63,0.49,Shannon
-Cr,3,4,0.641,0.501,ML Work
-Cr,4,6,0.6900000000000001,0.55,Shannon
-Cr,5,8,0.71,0.57,Shannon
-Cr,2,3,0.732,0.592,ML Work
-Cr,3,6,0.755,0.615,Shannon
-Cr,2,4,0.791,0.651,ML Work
-Cr,3,7,0.829,0.689,ML Work
-Cr,2,5,0.845,0.705,ML Work
-Cr,2,6,0.87,0.73,Shannon
-Cr,2,7,0.994,0.854,ML Work
-Cr,3,9,1.004,0.864,ML Work
-Cr,3,10,1.089,0.949,ML Work
-Cr,2,8,1.0899999999999999,0.95,ML Work
-Cs,1,1,1.6,1.46,ML Work
-Cs,1,2,1.6469999999999998,1.507,ML Work
-Cs,1,3,1.6909999999999998,1.551,ML Work
-Cs,1,4,1.733,1.593,ML Work
-Cs,1,5,1.7719999999999998,1.632,ML Work
-Cs,1,6,1.81,1.67,Shannon
-Cs,1,7,1.8450000000000002,1.705,ML Work
-Cs,1,8,1.88,1.74,Shannon
-Cs,1,9,1.92,1.78,Shannon
-Cs,1,10,1.9500000000000002,1.81,Shannon
-Cs,1,11,1.9900000000000002,1.85,Shannon
-Cs,1,12,2.02,1.88,Shannon
-Cs,1,13,2.069,1.929,ML Work
-Cu,2,2,0.526,0.386,ML Work
-Cu,3,4,0.5920000000000001,0.452,ML Work
-Cu,1,2,0.6000000000000001,0.46,Shannon
-Cu,2,3,0.615,0.475,ML Work
-Cu,3,5,0.645,0.505,ML Work
-Cu,1,3,0.675,0.535,ML Work
-Cu,3,6,0.68,0.54,Shannon
-Cu,2,4,0.71,0.57,Shannon
-Cu,1,4,0.74,0.6,Shannon
-Cu,2,5,0.79,0.65,Shannon
-Cu,3,8,0.846,0.706,ML Work
-Cu,1,5,0.865,0.725,ML Work
-Cu,2,6,0.87,0.73,Shannon
-Cu,1,6,0.91,0.77,Shannon
-Cu,2,7,0.9410000000000001,0.801,ML Work
-Cu,2,8,1.021,0.881,ML Work
-Cu,1,7,1.068,0.928,ML Work
-Cu,2,9,1.1019999999999999,0.962,ML Work
-Cu,3,12,1.1480000000000001,1.008,ML Work
-Cu,1,8,1.1629999999999998,1.023,ML Work
-Cu,2,10,1.178,1.038,ML Work
-Cu,1,9,1.2530000000000001,1.113,ML Work
-Cu,2,12,1.319,1.179,ML Work
-Cu,1,10,1.338,1.198,ML Work
-Dy,3,2,0.803,0.663,ML Work
-Dy,3,3,0.866,0.726,ML Work
-Dy,3,4,0.928,0.788,ML Work
-Dy,3,5,0.989,0.849,ML Work
-Dy,3,6,1.052,0.912,Shannon
-Dy,3,7,1.1099999999999999,0.97,Shannon
-Dy,3,8,1.1669999999999998,1.027,Shannon
-Dy,2,6,1.21,1.07,Shannon
-Dy,3,9,1.2229999999999999,1.083,Shannon
-Dy,3,10,1.2690000000000001,1.129,ML Work
-Dy,2,7,1.27,1.13,Shannon
-Dy,3,12,1.327,1.187,ML Work
-Dy,2,8,1.33,1.19,Shannon
-Er,3,2,0.776,0.636,ML Work
-Er,3,3,0.84,0.7,ML Work
-Er,3,5,0.965,0.825,ML Work
-Er,3,6,1.03,0.89,Shannon
-Er,3,7,1.085,0.945,Shannon
-Er,3,8,1.1440000000000001,1.004,Shannon
-Er,3,9,1.202,1.062,Shannon
-Er,3,10,1.2429999999999999,1.103,ML Work
-Eu,3,1,0.785,0.645,ML Work
-Eu,3,2,0.849,0.709,ML Work
-Eu,3,4,0.972,0.832,ML Work
-Eu,2,1,0.982,0.842,ML Work
-Eu,3,5,1.03,0.89,ML Work
-Eu,2,2,1.049,0.909,ML Work
-Eu,3,6,1.087,0.947,Shannon
-Eu,3,7,1.15,1.01,Shannon
-Eu,3,8,1.206,1.066,Shannon
-Eu,2,5,1.2389999999999999,1.099,ML Work
-Eu,3,9,1.2600000000000002,1.12,Shannon
-Eu,2,6,1.31,1.17,Shannon
-Eu,3,10,1.3119999999999998,1.172,ML Work
-Eu,2,7,1.3399999999999999,1.2,Shannon
-Eu,3,11,1.3439999999999999,1.204,ML Work
-Eu,3,12,1.371,1.231,ML Work
-Eu,2,8,1.3900000000000001,1.25,Shannon
-Eu,2,9,1.44,1.3,Shannon
-Eu,2,10,1.4900000000000002,1.35,Shannon
-Eu,2,11,1.545,1.405,ML Work
-Eu,2,12,1.592,1.452,ML Work
-F,7,6,0.22000000000000003,0.08,Shannon
-F,-1,2,1.145,1.285,Shannon
-F,-1,3,1.1600000000000001,1.3,Shannon
-F,-1,4,1.17,1.31,Shannon
-F,-1,6,1.19,1.33,Shannon
-Fe,6,4,0.39,0.25,Shannon
-Fe,5,4,0.465,0.325,ML Work
-Fe,4,4,0.5640000000000001,0.424,ML Work
-Fe,3,3,0.5820000000000001,0.442,ML Work
-Fe,2,2,0.618,0.478,ML Work
-Fe,3,4,0.63,0.49,Shannon
-Fe,4,5,0.636,0.496,ML Work
-Fe,3,6,0.6900000000000001,0.55,Shannon
-Fe,2,3,0.6970000000000001,0.557,ML Work
-Fe,1,2,0.7020000000000001,0.562,ML Work
-Fe,3,5,0.72,0.58,Shannon
-Fe,4,6,0.725,0.585,Shannon
-Fe,2,6,0.75,0.61,Shannon
-Fe,2,4,0.77,0.63,Shannon
-Fe,2,5,0.784,0.644,ML Work
-Fe,3,7,0.806,0.666,ML Work
-Fe,3,8,0.92,0.78,Shannon
-Fe,2,7,0.924,0.784,ML Work
-Fe,2,8,1.06,0.92,Shannon
-Fe,2,9,1.166,1.026,ML Work
-Fe,2,10,1.2600000000000002,1.12,ML Work
-Fe,2,12,1.4020000000000001,1.262,ML Work
-Fr,1,6,1.94,1.8,Shannon
-Ga,3,4,0.61,0.47,Shannon
-Ga,3,5,0.6900000000000001,0.55,Shannon
-Ga,3,6,0.76,0.62,Shannon
-Ga,3,7,0.8240000000000001,0.684,ML Work
-Ga,3,8,0.89,0.75,ML Work
-Gd,3,1,0.751,0.611,ML Work
-Gd,3,2,0.8150000000000001,0.675,ML Work
-Gd,3,4,0.9430000000000001,0.803,ML Work
-Gd,3,5,1.006,0.866,ML Work
-Gd,3,6,1.0779999999999998,0.938,Shannon
-Gd,3,7,1.1400000000000001,1.0,Shannon
-Gd,3,8,1.193,1.053,Shannon
-Gd,3,9,1.2469999999999999,1.107,Shannon
-Gd,3,10,1.2879999999999998,1.148,ML Work
-Gd,2,8,1.339,1.199,ML Work
-Gd,3,12,1.346,1.206,ML Work
-Ge,4,3,0.46,0.32,ML Work
-Ge,4,4,0.53,0.39,Shannon
-Ge,4,5,0.599,0.459,ML Work
-Ge,3,4,0.607,0.467,ML Work
-Ge,4,6,0.67,0.53,Shannon
-Ge,2,3,0.677,0.537,ML Work
-Ge,4,7,0.72,0.58,ML Work
-Ge,4,8,0.776,0.636,ML Work
-Ge,2,6,0.87,0.73,Shannon
-H,1,1,-0.24,-0.38,Shannon
-H,1,2,-0.03999999999999998,-0.18,Shannon
-Hf,4,4,0.72,0.58,Shannon
-Hf,4,6,0.85,0.71,Shannon
-Hf,4,7,0.9,0.76,Shannon
-Hf,4,8,0.97,0.83,Shannon
-Hg,2,2,0.83,0.69,Shannon
-Hg,1,1,0.878,0.738,ML Work
-Hg,2,3,0.963,0.823,ML Work
-Hg,1,2,0.994,0.854,ML Work
-Hg,2,4,1.1,0.96,Shannon
-Hg,1,3,1.1099999999999999,0.97,Shannon
-Hg,2,5,1.146,1.006,ML Work
-Hg,2,6,1.1600000000000001,1.02,Shannon
-Hg,1,4,1.209,1.069,ML Work
-Hg,2,7,1.2389999999999999,1.099,ML Work
-Hg,2,8,1.2799999999999998,1.14,Shannon
-Hg,1,5,1.2879999999999998,1.148,ML Work
-Hg,1,6,1.33,1.19,Shannon
-Hg,2,9,1.3319999999999999,1.192,ML Work
-Hg,2,10,1.383,1.243,ML Work
-Hg,1,7,1.4169999999999998,1.277,ML Work
-Hg,1,8,1.48,1.34,ML Work
-Hg,2,12,1.491,1.351,ML Work
-Hg,1,9,1.5390000000000001,1.399,ML Work
-Hg,1,10,1.5939999999999999,1.454,ML Work
-Ho,3,2,0.79,0.65,ML Work
-Ho,3,3,0.853,0.713,ML Work
-Ho,3,4,0.915,0.775,ML Work
-Ho,3,5,0.977,0.837,ML Work
-Ho,3,6,1.041,0.901,Shannon
-Ho,3,7,1.099,0.959,ML Work
-Ho,3,8,1.1549999999999998,1.015,Shannon
-Ho,3,9,1.2120000000000002,1.072,Shannon
-Ho,3,10,1.2600000000000002,1.12,Shannon
-Ho,3,11,1.287,1.147,ML Work
-Ho,3,12,1.314,1.174,ML Work
-I,7,4,0.56,0.42,Shannon
-I,5,3,0.5800000000000001,0.44,Shannon
-I,7,5,0.633,0.493,ML Work
-I,7,6,0.67,0.53,Shannon
-I,5,4,0.755,0.615,ML Work
-I,7,8,0.851,0.711,ML Work
-I,5,5,0.922,0.782,ML Work
-I,5,6,1.0899999999999999,0.95,Shannon
-I,5,7,1.177,1.037,ML Work
-I,5,8,1.2530000000000001,1.113,ML Work
-I,5,9,1.3090000000000002,1.169,ML Work
-I,-1,6,2.06,2.2,Shannon
-In,3,3,0.6960000000000001,0.556,ML Work
-In,3,4,0.76,0.62,Shannon
-In,3,5,0.853,0.713,ML Work
-In,3,6,0.9400000000000001,0.8,Shannon
-In,3,7,1.0,0.86,ML Work
-In,3,8,1.06,0.92,Shannon
-In,2,6,1.1640000000000001,1.024,ML Work
-In,2,7,1.237,1.097,ML Work
-In,2,8,1.302,1.162,ML Work
-In,1,9,1.625,1.485,ML Work
-In,1,10,1.6749999999999998,1.535,ML Work
-Ir,4,4,0.621,0.481,ML Work
-Ir,6,6,0.672,0.532,ML Work
-Ir,5,6,0.71,0.57,Shannon
-Ir,4,6,0.765,0.625,Shannon
-Ir,3,6,0.8200000000000001,0.68,Shannon
-K,1,1,1.3410000000000002,1.201,ML Work
-K,1,2,1.404,1.264,ML Work
-K,1,3,1.459,1.319,ML Work
-K,1,4,1.5100000000000002,1.37,Shannon
-K,1,6,1.52,1.38,Shannon
-K,1,5,1.541,1.401,ML Work
-K,1,7,1.6,1.46,Shannon
-K,1,8,1.65,1.51,Shannon
-K,1,9,1.69,1.55,Shannon
-K,1,10,1.73,1.59,Shannon
-K,1,11,1.75,1.61,ML Work
-K,1,12,1.7799999999999998,1.64,Shannon
-K,1,13,1.8130000000000002,1.673,ML Work
-La,3,1,0.863,0.723,ML Work
-La,3,2,0.928,0.788,ML Work
-La,3,3,0.992,0.852,ML Work
-La,3,4,1.053,0.913,ML Work
-La,3,5,1.113,0.973,ML Work
-La,3,6,1.1720000000000002,1.032,Shannon
-La,3,7,1.2400000000000002,1.1,Shannon
-La,3,8,1.2999999999999998,1.16,Shannon
-La,3,9,1.3559999999999999,1.216,Shannon
-La,2,6,1.3890000000000002,1.249,ML Work
-La,3,10,1.4100000000000001,1.27,Shannon
-La,3,11,1.439,1.299,ML Work
-La,2,8,1.4849999999999999,1.345,ML Work
-La,3,12,1.5,1.36,Shannon
-La,2,9,1.537,1.397,ML Work
-La,2,10,1.5910000000000002,1.451,ML Work
-La,2,12,1.689,1.549,ML Work
-Li,1,1,0.589,0.449,ML Work
-Li,1,2,0.635,0.495,ML Work
-Li,1,3,0.683,0.543,ML Work
-Li,1,4,0.73,0.59,Shannon
-Li,1,5,0.8130000000000001,0.673,ML Work
-Li,1,6,0.9,0.76,Shannon
-Li,1,7,0.978,0.838,ML Work
-Li,1,8,1.06,0.92,Shannon
-Li,1,9,1.129,0.989,ML Work
-Li,1,10,1.194,1.054,ML Work
-Li,1,12,1.307,1.167,ML Work
-Lu,3,2,0.76,0.62,ML Work
-Lu,3,3,0.8230000000000001,0.683,ML Work
-Lu,3,5,0.9420000000000001,0.802,ML Work
-Lu,3,6,1.001,0.861,Shannon
-Lu,3,7,1.0590000000000002,0.919,ML Work
-Lu,3,8,1.117,0.977,Shannon
-Lu,3,9,1.1720000000000002,1.032,Shannon
-Lu,3,10,1.222,1.082,ML Work
-Mg,2,3,0.618,0.478,ML Work
-Mg,2,4,0.71,0.57,Shannon
-Mg,2,5,0.8,0.66,Shannon
-Mg,2,6,0.86,0.72,Shannon
-Mg,2,7,0.9480000000000001,0.808,ML Work
-Mg,2,8,1.03,0.89,Shannon
-Mg,2,9,1.097,0.957,ML Work
-Mn,7,4,0.39,0.25,Shannon
-Mn,6,4,0.395,0.255,Shannon
-Mn,5,4,0.47000000000000003,0.33,Shannon
-Mn,4,4,0.53,0.39,Shannon
-Mn,7,6,0.6000000000000001,0.46,Shannon
-Mn,4,5,0.625,0.485,ML Work
-Mn,3,4,0.66,0.52,ML Work
-Mn,2,2,0.662,0.522,ML Work
-Mn,4,6,0.67,0.53,Shannon
-Mn,3,5,0.72,0.58,Shannon
-Mn,3,6,0.72,0.58,Shannon
-Mn,2,3,0.739,0.599,ML Work
-Mn,2,4,0.8,0.66,Shannon
-Mn,2,6,0.81,0.67,Shannon
-Mn,3,7,0.83,0.69,ML Work
-Mn,2,5,0.89,0.75,Shannon
-Mn,3,8,0.924,0.784,ML Work
-Mn,2,7,1.04,0.9,Shannon
-Mn,2,8,1.1,0.96,Shannon
-Mn,2,9,1.197,1.057,ML Work
-Mn,3,12,1.241,1.101,ML Work
-Mn,2,10,1.283,1.143,ML Work
-Mn,2,12,1.42,1.28,ML Work
-Mo,5,1,0.356,0.216,ML Work
-Mo,6,2,0.368,0.228,ML Work
-Mo,6,3,0.455,0.315,ML Work
-Mo,5,3,0.518,0.378,ML Work
-Mo,6,4,0.55,0.41,Shannon
-Mo,5,4,0.6000000000000001,0.46,Shannon
-Mo,6,5,0.64,0.5,Shannon
-Mo,5,5,0.681,0.541,ML Work
-Mo,6,6,0.73,0.59,Shannon
-Mo,5,6,0.75,0.61,Shannon
-Mo,4,6,0.79,0.65,Shannon
-Mo,3,6,0.83,0.69,Shannon
-Mo,6,7,0.87,0.73,Shannon
-Mo,6,8,0.919,0.779,ML Work
-N,5,6,0.27,0.13,Shannon
-N,3,6,0.30000000000000004,0.16,Shannon
-N,-3,4,1.3199999999999998,1.46,Shannon
-Na,1,1,0.958,0.818,ML Work
-Na,1,2,1.017,0.877,ML Work
-Na,1,3,1.069,0.929,ML Work
-Na,1,4,1.13,0.99,Shannon
-Na,1,5,1.1400000000000001,1.0,Shannon
-Na,1,6,1.1600000000000001,1.02,Shannon
-Na,1,7,1.2600000000000002,1.12,Shannon
-Na,1,8,1.3199999999999998,1.18,Shannon
-Na,1,9,1.38,1.24,Shannon
-Na,1,10,1.4340000000000002,1.294,ML Work
-Na,1,11,1.484,1.344,ML Work
-Na,1,12,1.5299999999999998,1.39,Shannon
-Nb,5,4,0.62,0.48,Shannon
-Nb,4,4,0.6890000000000001,0.549,ML Work
-Nb,5,5,0.703,0.563,ML Work
-Nb,3,4,0.749,0.609,ML Work
-Nb,4,5,0.756,0.616,ML Work
-Nb,5,6,0.78,0.64,Shannon
-Nb,3,5,0.805,0.665,ML Work
-Nb,4,6,0.8200000000000001,0.68,Shannon
-Nb,5,7,0.83,0.69,Shannon
-Nb,3,6,0.86,0.72,Shannon
-Nb,5,8,0.88,0.74,Shannon
-Nb,2,4,0.895,0.755,ML Work
-Nb,4,8,0.93,0.79,Shannon
-Nb,2,5,0.956,0.816,ML Work
-Nb,2,6,1.024,0.884,ML Work
-Nd,3,1,0.828,0.688,ML Work
-Nd,3,2,0.892,0.752,ML Work
-Nd,3,3,0.954,0.814,ML Work
-Nd,3,4,1.014,0.874,ML Work
-Nd,3,5,1.072,0.932,ML Work
-Nd,3,6,1.123,0.983,Shannon
-Nd,3,7,1.189,1.049,ML Work
-Nd,3,8,1.249,1.109,Shannon
-Nd,3,9,1.303,1.163,Shannon
-Nd,3,10,1.3559999999999999,1.216,ML Work
-Nd,3,11,1.3890000000000002,1.249,ML Work
-Nd,3,12,1.4100000000000001,1.27,Shannon
-Nd,2,8,1.4300000000000002,1.29,Shannon
-Nd,2,9,1.4900000000000002,1.35,Shannon
-Nd,2,12,1.645,1.505,ML Work
-Ni,2,2,0.509,0.369,ML Work
-Ni,1,2,0.585,0.445,ML Work
-Ni,2,3,0.5900000000000001,0.45,ML Work
-Ni,3,4,0.5900000000000001,0.45,ML Work
-Ni,4,6,0.62,0.48,Shannon
-Ni,2,4,0.63,0.49,Shannon
-Ni,3,6,0.7000000000000001,0.56,Shannon
-Ni,2,5,0.77,0.63,Shannon
-Ni,2,6,0.83,0.69,Shannon
-Ni,2,7,0.926,0.786,ML Work
-Ni,2,8,1.018,0.878,ML Work
-Ni,2,9,1.1099999999999999,0.97,ML Work
-No,2,6,1.2400000000000002,1.1,Shannon
-Np,6,2,0.569,0.429,ML Work
-Np,5,2,0.653,0.513,ML Work
-Np,6,5,0.758,0.618,ML Work
-Np,5,5,0.8220000000000001,0.682,ML Work
-Np,7,6,0.85,0.71,Shannon
-Np,6,6,0.86,0.72,Shannon
-Np,5,6,0.89,0.75,Shannon
-Np,6,7,0.932,0.792,ML Work
-Np,5,7,0.962,0.822,ML Work
-Np,6,8,0.995,0.855,ML Work
-Np,4,6,1.01,0.87,Shannon
-Np,5,8,1.025,0.885,ML Work
-Np,4,8,1.12,0.98,Shannon
-Np,3,6,1.15,1.01,Shannon
-Np,2,6,1.2400000000000002,1.1,Shannon
-O,-2,2,1.21,1.35,Shannon
-O,-2,3,1.2200000000000002,1.36,Shannon
-O,-2,4,1.2399999999999998,1.38,Shannon
-O,-2,6,1.2599999999999998,1.4,Shannon
-O,-2,8,1.2799999999999998,1.42,Shannon
-Os,8,4,0.53,0.39,Shannon
-Os,7,5,0.603,0.463,ML Work
-Os,6,5,0.63,0.49,Shannon
-Os,7,6,0.665,0.525,Shannon
-Os,6,6,0.685,0.545,Shannon
-Os,5,6,0.715,0.575,Shannon
-Os,4,6,0.77,0.63,Shannon
-P,4,3,0.30100000000000005,0.161,ML Work
-P,5,4,0.31000000000000005,0.17,Shannon
-P,4,4,0.371,0.231,ML Work
-P,3,3,0.40700000000000003,0.267,ML Work
-P,5,5,0.43,0.29,Shannon
-P,5,6,0.52,0.38,Shannon
-P,3,6,0.5800000000000001,0.44,Shannon
-Pa,5,6,0.92,0.78,Shannon
-Pa,4,6,1.04,0.9,Shannon
-Pa,5,8,1.05,0.91,Shannon
-Pa,5,9,1.0899999999999999,0.95,Shannon
-Pa,4,8,1.15,1.01,Shannon
-Pa,3,6,1.1800000000000002,1.04,Shannon
-Pb,4,4,0.79,0.65,Shannon
-Pb,2,1,0.841,0.701,ML Work
-Pb,4,5,0.87,0.73,Shannon
-Pb,4,6,0.915,0.775,Shannon
-Pb,2,2,0.936,0.796,ML Work
-Pb,2,3,1.032,0.892,ML Work
-Pb,4,8,1.08,0.94,Shannon
-Pb,2,4,1.12,0.98,Shannon
-Pb,2,5,1.229,1.089,ML Work
-Pb,2,6,1.33,1.19,Shannon
-Pb,2,7,1.37,1.23,Shannon
-Pb,2,8,1.4300000000000002,1.29,Shannon
-Pb,2,9,1.4900000000000002,1.35,Shannon
-Pb,2,10,1.54,1.4,Shannon
-Pb,2,11,1.5899999999999999,1.45,Shannon
-Pb,2,12,1.63,1.49,Shannon
-Pd,2,2,0.601,0.461,ML Work
-Pd,1,2,0.73,0.59,Shannon
-Pd,4,6,0.755,0.615,Shannon
-Pd,2,4,0.78,0.64,Shannon
-Pd,3,6,0.9,0.76,Shannon
-Pd,2,6,1.0,0.86,Shannon
-Pd,2,7,1.08,0.94,ML Work
-Pd,2,8,1.1640000000000001,1.024,ML Work
-Pd,2,10,1.322,1.182,ML Work
-Pm,3,6,1.1099999999999999,0.97,Shannon
-Pm,3,8,1.233,1.093,Shannon
-Pm,3,9,1.2839999999999998,1.144,Shannon
-Po,6,6,0.81,0.67,Shannon
-Po,4,6,1.08,0.94,Shannon
-Po,4,8,1.2200000000000002,1.08,Shannon
-Pr,3,1,0.844,0.704,ML Work
-Pr,3,2,0.908,0.768,ML Work
-Pr,4,5,0.922,0.782,ML Work
-Pr,3,3,0.971,0.831,ML Work
-Pr,4,6,0.99,0.85,Shannon
-Pr,3,4,1.0310000000000001,0.891,ML Work
-Pr,4,7,1.0430000000000001,0.903,ML Work
-Pr,3,5,1.088,0.948,ML Work
-Pr,4,8,1.1,0.96,Shannon
-Pr,3,6,1.13,0.99,Shannon
-Pr,3,7,1.205,1.065,ML Work
-Pr,3,8,1.266,1.126,Shannon
-Pr,3,9,1.319,1.179,Shannon
-Pr,3,10,1.3719999999999999,1.232,ML Work
-Pr,2,6,1.3780000000000001,1.238,ML Work
-Pr,3,11,1.4060000000000001,1.266,ML Work
-Pr,3,12,1.4340000000000002,1.294,ML Work
-Pr,2,8,1.4660000000000002,1.326,ML Work
-Pr,2,12,1.665,1.525,ML Work
-Pt,2,2,0.6020000000000001,0.462,ML Work
-Pt,6,6,0.657,0.517,ML Work
-Pt,5,6,0.71,0.57,Shannon
-Pt,2,4,0.74,0.6,Shannon
-Pt,4,6,0.765,0.625,Shannon
-Pt,2,6,0.9400000000000001,0.8,Shannon
-Pt,2,7,1.0630000000000002,0.923,ML Work
-Pt,2,8,1.166,1.026,ML Work
-Pu,6,2,0.562,0.422,ML Work
-Pu,5,2,0.645,0.505,ML Work
-Pu,6,6,0.85,0.71,Shannon
-Pu,5,6,0.88,0.74,Shannon
-Pu,6,8,0.985,0.845,ML Work
-Pu,4,6,1.0,0.86,Shannon
-Pu,5,8,1.014,0.874,ML Work
-Pu,3,4,1.028,0.888,ML Work
-Pu,4,7,1.06,0.92,ML Work
-Pu,3,5,1.081,0.941,ML Work
-Pu,4,8,1.1,0.96,Shannon
-Pu,3,6,1.1400000000000001,1.0,Shannon
-Pu,3,8,1.25,1.11,ML Work
-Ra,2,8,1.62,1.48,Shannon
-Ra,2,12,1.8399999999999999,1.7,Shannon
-Rb,1,1,1.3450000000000002,1.205,ML Work
-Rb,1,2,1.416,1.276,ML Work
-Rb,1,3,1.484,1.344,ML Work
-Rb,1,4,1.548,1.408,ML Work
-Rb,1,5,1.6059999999999999,1.466,ML Work
-Rb,1,6,1.6600000000000001,1.52,Shannon
-Rb,1,7,1.7000000000000002,1.56,Shannon
-Rb,1,8,1.75,1.61,Shannon
-Rb,1,9,1.77,1.63,Shannon
-Rb,1,10,1.7999999999999998,1.66,Shannon
-Rb,1,11,1.83,1.69,Shannon
-Rb,1,12,1.8599999999999999,1.72,Shannon
-Rb,1,13,1.9129999999999998,1.773,ML Work
-Rb,1,14,1.9700000000000002,1.83,Shannon
-Re,7,4,0.52,0.38,Shannon
-Re,6,4,0.539,0.399,ML Work
-Re,5,4,0.581,0.441,ML Work
-Re,7,5,0.5960000000000001,0.456,ML Work
-Re,6,5,0.617,0.477,ML Work
-Re,4,4,0.63,0.49,ML Work
-Re,7,6,0.67,0.53,Shannon
-Re,6,6,0.6900000000000001,0.55,Shannon
-Re,5,6,0.72,0.58,Shannon
-Re,4,6,0.77,0.63,Shannon
-Re,7,8,0.807,0.667,ML Work
-Rh,5,6,0.6900000000000001,0.55,Shannon
-Rh,4,6,0.74,0.6,Shannon
-Rh,3,6,0.805,0.665,Shannon
-Rh,3,8,0.978,0.838,ML Work
-Ru,8,4,0.5,0.36,Shannon
-Ru,7,4,0.52,0.38,Shannon
-Ru,6,4,0.526,0.386,ML Work
-Ru,5,4,0.569,0.429,ML Work
-Ru,6,5,0.609,0.469,ML Work
-Ru,5,5,0.642,0.502,ML Work
-Ru,3,4,0.671,0.531,ML Work
-Ru,6,6,0.6910000000000001,0.551,ML Work
-Ru,5,6,0.705,0.565,Shannon
-Ru,4,6,0.76,0.62,Shannon
-Ru,3,6,0.8200000000000001,0.68,Shannon
-Ru,4,7,0.8250000000000001,0.685,ML Work
-Ru,4,8,0.892,0.752,ML Work
-S,5,3,0.231,0.091,ML Work
-S,6,4,0.26,0.12,Shannon
-S,4,2,0.263,0.123,ML Work
-S,4,3,0.328,0.188,ML Work
-S,6,6,0.43,0.29,Shannon
-S,3,3,0.48200000000000004,0.342,ML Work
-S,5,6,0.496,0.356,ML Work
-S,4,6,0.51,0.37,Shannon
-S,2,1,0.623,0.483,ML Work
-S,2,2,0.67,0.53,ML Work
-S,2,3,0.719,0.579,ML Work
-S,2,4,0.768,0.628,ML Work
-S,-2,6,1.7000000000000002,1.84,Shannon
-Sb,5,3,0.534,0.394,ML Work
-Sb,5,5,0.682,0.542,ML Work
-Sb,5,6,0.74,0.6,Shannon
-Sb,3,3,0.8180000000000001,0.678,ML Work
-Sb,3,4,0.9,0.76,Shannon
-Sb,3,6,0.9,0.76,Shannon
-Sb,3,5,0.9400000000000001,0.8,Shannon
-Sb,3,7,0.998,0.858,ML Work
-Sb,3,8,1.072,0.932,ML Work
-Sb,3,9,1.154,1.014,ML Work
-Sb,3,10,1.2349999999999999,1.095,ML Work
-Sc,3,2,0.569,0.429,ML Work
-Sc,3,5,0.799,0.659,ML Work
-Sc,3,6,0.885,0.745,Shannon
-Sc,3,7,0.9440000000000001,0.804,ML Work
-Sc,3,8,1.01,0.87,Shannon
-Sc,2,6,1.064,0.924,ML Work
-Sc,3,9,1.081,0.941,ML Work
-Sc,3,10,1.146,1.006,ML Work
-Se,4,1,0.265,0.125,ML Work
-Se,6,3,0.34,0.2,ML Work
-Se,4,3,0.41200000000000003,0.272,ML Work
-Se,6,4,0.42000000000000004,0.28,Shannon
-Se,6,5,0.49,0.35,ML Work
-Se,4,4,0.492,0.352,ML Work
-Se,6,6,0.56,0.42,Shannon
-Se,4,5,0.5740000000000001,0.434,ML Work
-Se,4,6,0.64,0.5,Shannon
-Se,2,1,0.659,0.519,ML Work
-Se,2,2,0.722,0.582,ML Work
-Se,4,7,0.751,0.611,ML Work
-Se,2,3,0.786,0.646,ML Work
-Se,4,8,0.843,0.703,ML Work
-Se,4,9,0.929,0.789,ML Work
-Se,2,8,1.1320000000000001,0.992,ML Work
-Se,-2,6,1.8399999999999999,1.98,Shannon
-Si,4,4,0.4,0.26,Shannon
-Si,4,5,0.47200000000000003,0.332,ML Work
-Si,4,6,0.54,0.4,Shannon
-Si,4,8,0.671,0.531,ML Work
-Sm,3,1,0.798,0.658,ML Work
-Sm,3,2,0.861,0.721,ML Work
-Sm,3,3,0.924,0.784,ML Work
-Sm,3,4,0.984,0.844,ML Work
-Sm,3,5,1.042,0.902,ML Work
-Sm,3,6,1.0979999999999999,0.958,Shannon
-Sm,3,7,1.1600000000000001,1.02,Shannon
-Sm,3,8,1.2189999999999999,1.079,Shannon
-Sm,3,9,1.2719999999999998,1.132,Shannon
-Sm,2,6,1.31,1.17,ML Work
-Sm,3,10,1.3250000000000002,1.185,ML Work
-Sm,3,11,1.358,1.218,ML Work
-Sm,2,7,1.3599999999999999,1.22,Shannon
-Sm,3,12,1.38,1.24,Shannon
-Sm,2,8,1.4100000000000001,1.27,Shannon
-Sm,2,9,1.46,1.32,Shannon
-Sn,4,4,0.6900000000000001,0.55,Shannon
-Sn,4,5,0.76,0.62,Shannon
-Sn,4,6,0.83,0.69,Shannon
-Sn,2,2,0.837,0.697,ML Work
-Sn,4,7,0.89,0.75,Shannon
-Sn,2,3,0.922,0.782,ML Work
-Sn,4,8,0.9500000000000001,0.81,Shannon
-Sn,2,4,1.002,0.862,ML Work
-Sn,2,5,1.073,0.933,ML Work
-Sn,2,6,1.139,0.999,ML Work
-Sn,2,7,1.2029999999999998,1.063,ML Work
-Sn,2,8,1.2679999999999998,1.128,ML Work
-Sn,2,9,1.335,1.195,ML Work
-Sn,2,10,1.404,1.264,ML Work
-Sr,2,1,0.9500000000000001,0.81,ML Work
-Sr,2,2,1.0310000000000001,0.891,ML Work
-Sr,2,3,1.111,0.971,ML Work
-Sr,2,4,1.186,1.046,ML Work
-Sr,2,5,1.255,1.115,ML Work
-Sr,2,6,1.3199999999999998,1.18,Shannon
-Sr,2,7,1.35,1.21,Shannon
-Sr,2,8,1.4,1.26,Shannon
-Sr,2,9,1.4500000000000002,1.31,Shannon
-Sr,2,10,1.5,1.36,Shannon
-Sr,2,11,1.541,1.401,ML Work
-Sr,2,12,1.58,1.44,Shannon
-Ta,5,4,0.618,0.478,ML Work
-Ta,5,5,0.6990000000000001,0.559,ML Work
-Ta,4,5,0.753,0.613,ML Work
-Ta,5,6,0.78,0.64,Shannon
-Ta,4,6,0.8200000000000001,0.68,Shannon
-Ta,5,7,0.83,0.69,Shannon
-Ta,3,6,0.86,0.72,Shannon
-Ta,5,8,0.88,0.74,Shannon
-Tb,3,1,0.752,0.612,ML Work
-Tb,3,2,0.8160000000000001,0.676,ML Work
-Tb,4,5,0.843,0.703,ML Work
-Tb,4,6,0.9,0.76,Shannon
-Tb,4,7,0.964,0.824,ML Work
-Tb,3,5,1.001,0.861,ML Work
-Tb,4,8,1.02,0.88,Shannon
-Tb,3,6,1.0630000000000002,0.923,Shannon
-Tb,3,7,1.12,0.98,Shannon
-Tb,3,8,1.1800000000000002,1.04,Shannon
-Tb,4,12,1.186,1.046,ML Work
-Tb,3,9,1.2349999999999999,1.095,Shannon
-Tb,3,10,1.2810000000000001,1.141,ML Work
-Tb,3,12,1.3399999999999999,1.2,ML Work
-Tc,7,4,0.51,0.37,Shannon
-Tc,7,5,0.609,0.469,ML Work
-Tc,7,6,0.7000000000000001,0.56,Shannon
-Tc,5,6,0.74,0.6,Shannon
-Tc,4,6,0.785,0.645,Shannon
-Tc,7,8,0.864,0.724,ML Work
-Te,4,2,0.5549999999999999,0.415,ML Work
-Te,6,4,0.5700000000000001,0.43,Shannon
-Te,6,5,0.638,0.498,ML Work
-Te,4,3,0.66,0.52,Shannon
-Te,6,6,0.7000000000000001,0.56,Shannon
-Te,5,5,0.79,0.65,ML Work
-Te,6,7,0.791,0.651,ML Work
-Te,4,4,0.8,0.66,Shannon
-Te,5,6,0.9,0.76,ML Work
-Te,4,5,0.9490000000000001,0.809,ML Work
-Te,4,6,1.1099999999999999,0.97,Shannon
-Te,4,7,1.149,1.009,ML Work
-Te,4,8,1.202,1.062,ML Work
-Te,4,9,1.2480000000000002,1.108,ML Work
-Te,4,10,1.2959999999999998,1.156,ML Work
-Te,-2,6,2.07,2.21,Shannon
-Th,4,4,0.937,0.797,ML Work
-Th,4,5,0.998,0.858,ML Work
-Th,4,6,1.08,0.94,Shannon
-Th,4,7,1.113,0.973,ML Work
-Th,4,8,1.19,1.05,Shannon
-Th,4,9,1.23,1.09,Shannon
-Th,4,10,1.27,1.13,Shannon
-Th,4,11,1.3199999999999998,1.18,Shannon
-Th,4,12,1.35,1.21,Shannon
-Th,3,12,1.504,1.364,ML Work
-Ti,4,1,0.323,0.183,ML Work
-Ti,4,2,0.402,0.262,ML Work
-Ti,4,3,0.48300000000000004,0.343,ML Work
-Ti,4,4,0.56,0.42,Shannon
-Ti,4,5,0.65,0.51,Shannon
-Ti,4,6,0.745,0.605,Shannon
-Ti,3,5,0.755,0.615,ML Work
-Ti,3,6,0.81,0.67,Shannon
-Ti,2,4,0.862,0.722,ML Work
-Ti,4,8,0.88,0.74,Shannon
-Ti,3,7,0.902,0.762,ML Work
-Ti,2,5,0.929,0.789,ML Work
-Ti,4,9,0.936,0.796,ML Work
-Ti,4,10,0.99,0.85,ML Work
-Ti,2,6,1.0,0.86,Shannon
-Tl,3,1,0.633,0.493,ML Work
-Tl,3,2,0.72,0.58,ML Work
-Tl,3,3,0.806,0.666,ML Work
-Tl,3,4,0.89,0.75,Shannon
-Tl,3,5,0.962,0.822,ML Work
-Tl,3,6,1.025,0.885,Shannon
-Tl,1,1,1.03,0.89,ML Work
-Tl,3,7,1.099,0.959,ML Work
-Tl,3,8,1.12,0.98,Shannon
-Tl,1,2,1.158,1.018,ML Work
-Tl,3,9,1.226,1.086,ML Work
-Tl,1,3,1.29,1.15,ML Work
-Tl,3,12,1.4009999999999998,1.261,ML Work
-Tl,1,4,1.4180000000000001,1.278,ML Work
-Tl,1,5,1.532,1.392,ML Work
-Tl,1,6,1.6400000000000001,1.5,Shannon
-Tl,1,7,1.685,1.545,ML Work
-Tl,1,8,1.73,1.59,Shannon
-Tl,1,9,1.7600000000000002,1.62,ML Work
-Tl,1,10,1.79,1.65,ML Work
-Tl,1,11,1.8199999999999998,1.68,ML Work
-Tl,1,12,1.8399999999999999,1.7,Shannon
-Tm,3,2,0.764,0.624,ML Work
-Tm,3,3,0.8270000000000001,0.687,ML Work
-Tm,3,6,1.02,0.88,Shannon
-Tm,3,7,1.076,0.936,ML Work
-Tm,3,8,1.134,0.994,Shannon
-Tm,2,6,1.17,1.03,Shannon
-Tm,3,9,1.1920000000000002,1.052,Shannon
-Tm,2,7,1.23,1.09,Shannon
-Tm,3,10,1.2309999999999999,1.091,ML Work
-Tm,2,8,1.287,1.147,ML Work
-Tm,3,12,1.29,1.15,ML Work
-Tm,2,12,1.4900000000000002,1.35,ML Work
-U,6,2,0.5900000000000001,0.45,Shannon
-U,6,3,0.624,0.484,ML Work
-U,6,4,0.66,0.52,Shannon
-U,5,2,0.664,0.524,ML Work
-U,6,5,0.769,0.629,ML Work
-U,5,5,0.834,0.694,ML Work
-U,6,6,0.87,0.73,Shannon
-U,5,6,0.9,0.76,Shannon
-U,6,7,0.9500000000000001,0.81,Shannon
-U,5,7,0.98,0.84,Shannon
-U,6,8,1.0,0.86,Shannon
-U,4,6,1.03,0.89,Shannon
-U,5,8,1.038,0.898,ML Work
-U,4,7,1.0899999999999999,0.95,Shannon
-U,4,8,1.1400000000000001,1.0,Shannon
-U,3,6,1.165,1.025,Shannon
-U,4,9,1.19,1.05,Shannon
-U,4,12,1.31,1.17,Shannon
-V,5,1,0.22300000000000003,0.083,ML Work
-V,5,2,0.31100000000000005,0.171,ML Work
-V,4,1,0.323,0.183,ML Work
-V,4,2,0.403,0.263,ML Work
-V,5,3,0.403,0.263,ML Work
-V,4,3,0.486,0.346,ML Work
-V,5,4,0.495,0.355,Shannon
-V,4,4,0.571,0.431,ML Work
-V,3,3,0.589,0.449,ML Work
-V,5,5,0.6000000000000001,0.46,Shannon
-V,3,4,0.653,0.513,ML Work
-V,4,5,0.67,0.53,Shannon
-V,5,6,0.68,0.54,Shannon
-V,3,5,0.716,0.576,ML Work
-V,4,6,0.72,0.58,Shannon
-V,5,8,0.77,0.63,ML Work
-V,3,6,0.78,0.64,Shannon
-V,4,8,0.86,0.72,Shannon
-V,2,6,0.93,0.79,Shannon
-W,6,3,0.47800000000000004,0.338,ML Work
-W,6,4,0.56,0.42,Shannon
-W,6,5,0.65,0.51,Shannon
-W,6,6,0.74,0.6,Shannon
-W,5,6,0.76,0.62,Shannon
-W,4,6,0.8,0.66,Shannon
-W,6,7,0.811,0.671,ML Work
-W,5,7,0.8250000000000001,0.685,ML Work
-W,6,8,0.877,0.737,ML Work
-Xe,8,4,0.54,0.4,Shannon
-Xe,8,6,0.62,0.48,Shannon
-Y,3,2,0.752,0.612,ML Work
-Y,3,3,0.8260000000000001,0.686,ML Work
-Y,3,4,0.899,0.759,ML Work
-Y,3,5,0.969,0.829,ML Work
-Y,3,6,1.04,0.9,Shannon
-Y,3,7,1.1,0.96,Shannon
-Y,3,8,1.1589999999999998,1.019,Shannon
-Y,2,6,1.2069999999999999,1.067,ML Work
-Y,3,9,1.2149999999999999,1.075,Shannon
-Y,3,10,1.266,1.126,ML Work
-Y,3,12,1.359,1.219,ML Work
-Yb,3,2,0.751,0.611,ML Work
-Yb,3,3,0.8150000000000001,0.675,ML Work
-Yb,3,5,0.9430000000000001,0.803,ML Work
-Yb,3,6,1.008,0.868,Shannon
-Yb,3,7,1.065,0.925,Shannon
-Yb,3,8,1.125,0.985,Shannon
-Yb,2,6,1.1600000000000001,1.02,Shannon
-Yb,3,9,1.182,1.042,Shannon
-Yb,3,10,1.2189999999999999,1.079,ML Work
-Yb,2,7,1.2200000000000002,1.08,Shannon
-Yb,3,12,1.278,1.138,ML Work
-Yb,2,8,1.2799999999999998,1.14,Shannon
-Yb,2,12,1.476,1.336,ML Work
-Zn,2,1,0.463,0.323,ML Work
-Zn,2,2,0.554,0.414,ML Work
-Zn,2,3,0.646,0.506,ML Work
-Zn,2,4,0.74,0.6,Shannon
-Zn,2,5,0.8200000000000001,0.68,Shannon
-Zn,2,6,0.88,0.74,Shannon
-Zn,2,7,0.961,0.821,ML Work
-Zn,2,8,1.04,0.9,Shannon
-Zn,2,9,1.1059999999999999,0.966,ML Work
-Zr,4,4,0.73,0.59,Shannon
-Zr,4,5,0.8,0.66,Shannon
-Zr,4,6,0.86,0.72,Shannon
-Zr,4,7,0.92,0.78,Shannon
-Zr,4,8,0.98,0.84,Shannon
-Zr,4,9,1.03,0.89,Shannon
-Zr,4,10,1.088,0.948,ML Work
+ion,charge,coordination,crystal_radius,ionic_radius,reference
+Ac,3,6,1.2600000000000002,1.12,Shannon
+Ac,3,8,1.392,1.252,ML Work
+Ag,2,2,0.6920000000000001,0.552,ML Work
+Ag,1,1,0.703,0.563,ML Work
+Ag,1,2,0.81,0.67,Shannon
+Ag,3,4,0.81,0.67,Shannon
+Ag,3,6,0.89,0.75,Shannon
+Ag,2,4,0.93,0.79,Shannon
+Ag,1,3,0.984,0.844,ML Work
+Ag,3,8,1.022,0.882,ML Work
+Ag,2,6,1.08,0.94,Shannon
+Ag,1,4,1.1400000000000001,1.0,Shannon
+Ag,2,8,1.2160000000000002,1.076,ML Work
+Ag,1,5,1.23,1.09,Shannon
+Ag,1,6,1.29,1.15,Shannon
+Ag,1,7,1.3599999999999999,1.22,Shannon
+Ag,1,8,1.42,1.28,Shannon
+Ag,1,9,1.4900000000000002,1.35,ML Work
+Ag,1,10,1.5550000000000002,1.415,ML Work
+Ag,1,11,1.6190000000000002,1.479,ML Work
+Ag,1,12,1.682,1.542,ML Work
+Al,3,3,0.453,0.313,ML Work
+Al,3,4,0.53,0.39,Shannon
+Al,3,5,0.62,0.48,Shannon
+Al,3,6,0.675,0.535,Shannon
+Al,3,7,0.751,0.611,ML Work
+Am,4,6,0.99,0.85,Shannon
+Am,4,8,1.0899999999999999,0.95,Shannon
+Am,3,6,1.115,0.975,Shannon
+Am,3,8,1.23,1.09,Shannon
+Am,2,7,1.35,1.21,Shannon
+Am,2,8,1.4,1.26,Shannon
+Am,2,9,1.4500000000000002,1.31,Shannon
+As,5,3,0.395,0.255,ML Work
+As,5,4,0.47500000000000003,0.335,Shannon
+As,5,5,0.535,0.395,ML Work
+As,3,3,0.5529999999999999,0.413,ML Work
+As,5,6,0.6000000000000001,0.46,Shannon
+As,3,4,0.611,0.471,ML Work
+As,3,5,0.664,0.524,ML Work
+As,5,8,0.717,0.577,ML Work
+As,3,6,0.72,0.58,Shannon
+At,7,6,0.76,0.62,Shannon
+Au,5,6,0.71,0.57,Shannon
+Au,3,4,0.8200000000000001,0.68,Shannon
+Au,2,3,0.847,0.707,ML Work
+Au,3,5,0.902,0.762,ML Work
+Au,3,6,0.99,0.85,Shannon
+Au,1,2,1.0,0.86,ML Work
+Au,3,8,1.1059999999999999,0.966,ML Work
+Au,3,10,1.23,1.09,ML Work
+Au,3,12,1.3559999999999999,1.216,ML Work
+Au,1,6,1.5100000000000002,1.37,Shannon
+B,3,3,0.15000000000000002,0.01,Shannon
+B,3,4,0.25,0.11,Shannon
+B,3,5,0.328,0.188,ML Work
+B,3,6,0.41000000000000003,0.27,Shannon
+Ba,2,1,1.119,0.979,ML Work
+Ba,2,2,1.193,1.053,ML Work
+Ba,2,3,1.2679999999999998,1.128,ML Work
+Ba,2,4,1.343,1.203,ML Work
+Ba,2,5,1.4140000000000001,1.274,ML Work
+Ba,2,6,1.4900000000000002,1.35,Shannon
+Ba,2,7,1.52,1.38,Shannon
+Ba,2,8,1.56,1.42,Shannon
+Ba,2,9,1.6099999999999999,1.47,Shannon
+Ba,2,10,1.6600000000000001,1.52,Shannon
+Ba,2,11,1.71,1.57,Shannon
+Ba,2,12,1.75,1.61,Shannon
+Be,2,3,0.30000000000000004,0.16,Shannon
+Be,2,4,0.41000000000000003,0.27,Shannon
+Be,2,5,0.499,0.359,ML Work
+Be,2,6,0.5900000000000001,0.45,Shannon
+Bi,5,2,0.5589999999999999,0.419,ML Work
+Bi,5,4,0.732,0.592,ML Work
+Bi,3,1,0.754,0.614,ML Work
+Bi,5,5,0.8160000000000001,0.676,ML Work
+Bi,3,2,0.845,0.705,ML Work
+Bi,5,6,0.9,0.76,Shannon
+Bi,3,3,0.935,0.795,ML Work
+Bi,5,8,1.018,0.878,ML Work
+Bi,3,4,1.02,0.88,ML Work
+Bi,3,5,1.1,0.96,Shannon
+Bi,3,6,1.17,1.03,Shannon
+Bi,3,7,1.237,1.097,ML Work
+Bi,3,8,1.31,1.17,Shannon
+Bi,3,9,1.3599999999999999,1.22,ML Work
+Bi,3,10,1.415,1.275,ML Work
+Bi,3,11,1.4700000000000002,1.33,ML Work
+Bi,3,12,1.525,1.385,ML Work
+Bk,4,6,0.97,0.83,Shannon
+Bk,4,8,1.07,0.93,Shannon
+Bk,3,6,1.1,0.96,Shannon
+Br,7,4,0.39,0.25,Shannon
+Br,5,3,0.45,0.31,Shannon
+Br,7,6,0.53,0.39,Shannon
+Br,3,4,0.73,0.59,Shannon
+Br,5,6,0.775,0.635,ML Work
+Br,1,2,1.161,1.021,ML Work
+Br,-1,6,1.8199999999999998,1.96,Shannon
+C,3,2,0.167,0.027,ML Work
+C,4,3,0.21000000000000002,0.07,ML Work
+C,3,3,0.22400000000000003,0.084,ML Work
+C,2,1,0.245,0.105,ML Work
+C,4,4,0.29000000000000004,0.15,Shannon
+C,2,2,0.29600000000000004,0.156,ML Work
+C,4,6,0.30000000000000004,0.16,Shannon
+Ca,2,1,0.741,0.601,ML Work
+Ca,2,2,0.8250000000000001,0.685,ML Work
+Ca,2,3,0.909,0.769,ML Work
+Ca,2,4,0.99,0.85,ML Work
+Ca,2,5,1.0670000000000002,0.927,ML Work
+Ca,2,6,1.1400000000000001,1.0,Shannon
+Ca,2,7,1.2000000000000002,1.06,Shannon
+Ca,2,8,1.2600000000000002,1.12,Shannon
+Ca,2,9,1.3199999999999998,1.18,Shannon
+Ca,2,10,1.37,1.23,Shannon
+Ca,2,11,1.4260000000000002,1.286,ML Work
+Ca,2,12,1.48,1.34,Shannon
+Cd,2,2,0.726,0.586,ML Work
+Cd,2,3,0.83,0.69,ML Work
+Cd,2,4,0.92,0.78,Shannon
+Cd,2,5,1.01,0.87,Shannon
+Cd,2,6,1.0899999999999999,0.95,Shannon
+Cd,2,7,1.17,1.03,Shannon
+Cd,2,8,1.2400000000000002,1.1,Shannon
+Cd,2,9,1.291,1.151,ML Work
+Cd,2,10,1.3439999999999999,1.204,ML Work
+Cd,2,12,1.4500000000000002,1.31,Shannon
+Ce,3,2,0.912,0.772,ML Work
+Ce,4,6,1.01,0.87,Shannon
+Ce,3,4,1.0350000000000001,0.895,ML Work
+Ce,4,7,1.053,0.913,ML Work
+Ce,3,5,1.093,0.953,ML Work
+Ce,4,8,1.1099999999999999,0.97,Shannon
+Ce,3,6,1.15,1.01,Shannon
+Ce,4,9,1.1629999999999998,1.023,ML Work
+Ce,3,7,1.21,1.07,Shannon
+Ce,4,10,1.21,1.07,Shannon
+Ce,4,12,1.2799999999999998,1.14,Shannon
+Ce,3,8,1.283,1.143,Shannon
+Ce,3,9,1.3359999999999999,1.196,Shannon
+Ce,2,6,1.375,1.235,ML Work
+Ce,3,10,1.3900000000000001,1.25,Shannon
+Ce,3,11,1.4129999999999998,1.273,ML Work
+Ce,3,12,1.48,1.34,Shannon
+Cf,4,6,0.961,0.821,Shannon
+Cf,4,8,1.06,0.92,Shannon
+Cf,3,6,1.0899999999999999,0.95,Shannon
+Cl,5,2,0.192,0.052,ML Work
+Cl,7,4,0.22000000000000003,0.08,Shannon
+Cl,5,3,0.26,0.12,Shannon
+Cl,4,2,0.339,0.199,ML Work
+Cl,7,6,0.41000000000000003,0.27,Shannon
+Cl,1,1,1.083,0.943,ML Work
+Cl,1,2,1.137,0.997,ML Work
+Cl,-1,6,1.67,1.81,Shannon
+Cm,4,6,0.99,0.85,Shannon
+Cm,4,8,1.0899999999999999,0.95,Shannon
+Cm,3,6,1.1099999999999999,0.97,Shannon
+Co,3,1,0.398,0.258,ML Work
+Co,4,4,0.54,0.4,Shannon
+Co,3,3,0.55,0.41,ML Work
+Co,2,2,0.552,0.412,ML Work
+Co,4,5,0.607,0.467,ML Work
+Co,3,4,0.612,0.472,ML Work
+Co,1,2,0.627,0.487,ML Work
+Co,2,3,0.636,0.496,ML Work
+Co,3,5,0.666,0.526,ML Work
+Co,4,6,0.67,0.53,Shannon
+Co,3,6,0.685,0.545,Shannon
+Co,2,4,0.72,0.58,Shannon
+Co,2,6,0.79,0.65,Shannon
+Co,3,7,0.795,0.655,ML Work
+Co,2,5,0.81,0.67,Shannon
+Co,2,7,0.922,0.782,ML Work
+Co,2,8,1.04,0.9,Shannon
+Co,2,9,1.135,0.995,ML Work
+Cr,5,3,0.394,0.254,ML Work
+Cr,6,4,0.4,0.26,Shannon
+Cr,5,4,0.485,0.345,Shannon
+Cr,6,5,0.495,0.355,ML Work
+Cr,3,2,0.515,0.375,ML Work
+Cr,4,4,0.55,0.41,Shannon
+Cr,5,5,0.5609999999999999,0.421,ML Work
+Cr,6,6,0.5800000000000001,0.44,Shannon
+Cr,4,5,0.625,0.485,ML Work
+Cr,5,6,0.63,0.49,Shannon
+Cr,3,4,0.641,0.501,ML Work
+Cr,4,6,0.6900000000000001,0.55,Shannon
+Cr,5,8,0.71,0.57,Shannon
+Cr,2,3,0.732,0.592,ML Work
+Cr,3,6,0.755,0.615,Shannon
+Cr,2,4,0.791,0.651,ML Work
+Cr,3,7,0.829,0.689,ML Work
+Cr,2,5,0.845,0.705,ML Work
+Cr,2,6,0.87,0.73,Shannon
+Cr,2,7,0.994,0.854,ML Work
+Cr,3,9,1.004,0.864,ML Work
+Cr,3,10,1.089,0.949,ML Work
+Cr,2,8,1.0899999999999999,0.95,ML Work
+Cs,1,1,1.6,1.46,ML Work
+Cs,1,2,1.6469999999999998,1.507,ML Work
+Cs,1,3,1.6909999999999998,1.551,ML Work
+Cs,1,4,1.733,1.593,ML Work
+Cs,1,5,1.7719999999999998,1.632,ML Work
+Cs,1,6,1.81,1.67,Shannon
+Cs,1,7,1.8450000000000002,1.705,ML Work
+Cs,1,8,1.88,1.74,Shannon
+Cs,1,9,1.92,1.78,Shannon
+Cs,1,10,1.9500000000000002,1.81,Shannon
+Cs,1,11,1.9900000000000002,1.85,Shannon
+Cs,1,12,2.02,1.88,Shannon
+Cs,1,13,2.069,1.929,ML Work
+Cu,2,2,0.526,0.386,ML Work
+Cu,3,4,0.5920000000000001,0.452,ML Work
+Cu,1,2,0.6000000000000001,0.46,Shannon
+Cu,2,3,0.615,0.475,ML Work
+Cu,3,5,0.645,0.505,ML Work
+Cu,1,3,0.675,0.535,ML Work
+Cu,3,6,0.68,0.54,Shannon
+Cu,2,4,0.71,0.57,Shannon
+Cu,1,4,0.74,0.6,Shannon
+Cu,2,5,0.79,0.65,Shannon
+Cu,3,8,0.846,0.706,ML Work
+Cu,1,5,0.865,0.725,ML Work
+Cu,2,6,0.87,0.73,Shannon
+Cu,1,6,0.91,0.77,Shannon
+Cu,2,7,0.9410000000000001,0.801,ML Work
+Cu,2,8,1.021,0.881,ML Work
+Cu,1,7,1.068,0.928,ML Work
+Cu,2,9,1.1019999999999999,0.962,ML Work
+Cu,3,12,1.1480000000000001,1.008,ML Work
+Cu,1,8,1.1629999999999998,1.023,ML Work
+Cu,2,10,1.178,1.038,ML Work
+Cu,1,9,1.2530000000000001,1.113,ML Work
+Cu,2,12,1.319,1.179,ML Work
+Cu,1,10,1.338,1.198,ML Work
+Dy,3,2,0.803,0.663,ML Work
+Dy,3,3,0.866,0.726,ML Work
+Dy,3,4,0.928,0.788,ML Work
+Dy,3,5,0.989,0.849,ML Work
+Dy,3,6,1.052,0.912,Shannon
+Dy,3,7,1.1099999999999999,0.97,Shannon
+Dy,3,8,1.1669999999999998,1.027,Shannon
+Dy,2,6,1.21,1.07,Shannon
+Dy,3,9,1.2229999999999999,1.083,Shannon
+Dy,3,10,1.2690000000000001,1.129,ML Work
+Dy,2,7,1.27,1.13,Shannon
+Dy,3,12,1.327,1.187,ML Work
+Dy,2,8,1.33,1.19,Shannon
+Er,3,2,0.776,0.636,ML Work
+Er,3,3,0.84,0.7,ML Work
+Er,3,5,0.965,0.825,ML Work
+Er,3,6,1.03,0.89,Shannon
+Er,3,7,1.085,0.945,Shannon
+Er,3,8,1.1440000000000001,1.004,Shannon
+Er,3,9,1.202,1.062,Shannon
+Er,3,10,1.2429999999999999,1.103,ML Work
+Eu,3,1,0.785,0.645,ML Work
+Eu,3,2,0.849,0.709,ML Work
+Eu,3,4,0.972,0.832,ML Work
+Eu,2,1,0.982,0.842,ML Work
+Eu,3,5,1.03,0.89,ML Work
+Eu,2,2,1.049,0.909,ML Work
+Eu,3,6,1.087,0.947,Shannon
+Eu,3,7,1.15,1.01,Shannon
+Eu,3,8,1.206,1.066,Shannon
+Eu,2,5,1.2389999999999999,1.099,ML Work
+Eu,3,9,1.2600000000000002,1.12,Shannon
+Eu,2,6,1.31,1.17,Shannon
+Eu,3,10,1.3119999999999998,1.172,ML Work
+Eu,2,7,1.3399999999999999,1.2,Shannon
+Eu,3,11,1.3439999999999999,1.204,ML Work
+Eu,3,12,1.371,1.231,ML Work
+Eu,2,8,1.3900000000000001,1.25,Shannon
+Eu,2,9,1.44,1.3,Shannon
+Eu,2,10,1.4900000000000002,1.35,Shannon
+Eu,2,11,1.545,1.405,ML Work
+Eu,2,12,1.592,1.452,ML Work
+F,7,6,0.22000000000000003,0.08,Shannon
+F,-1,2,1.145,1.285,Shannon
+F,-1,3,1.1600000000000001,1.3,Shannon
+F,-1,4,1.17,1.31,Shannon
+F,-1,6,1.19,1.33,Shannon
+Fe,6,4,0.39,0.25,Shannon
+Fe,5,4,0.465,0.325,ML Work
+Fe,4,4,0.5640000000000001,0.424,ML Work
+Fe,3,3,0.5820000000000001,0.442,ML Work
+Fe,2,2,0.618,0.478,ML Work
+Fe,3,4,0.63,0.49,Shannon
+Fe,4,5,0.636,0.496,ML Work
+Fe,3,6,0.6900000000000001,0.55,Shannon
+Fe,2,3,0.6970000000000001,0.557,ML Work
+Fe,1,2,0.7020000000000001,0.562,ML Work
+Fe,3,5,0.72,0.58,Shannon
+Fe,4,6,0.725,0.585,Shannon
+Fe,2,6,0.75,0.61,Shannon
+Fe,2,4,0.77,0.63,Shannon
+Fe,2,5,0.784,0.644,ML Work
+Fe,3,7,0.806,0.666,ML Work
+Fe,3,8,0.92,0.78,Shannon
+Fe,2,7,0.924,0.784,ML Work
+Fe,2,8,1.06,0.92,Shannon
+Fe,2,9,1.166,1.026,ML Work
+Fe,2,10,1.2600000000000002,1.12,ML Work
+Fe,2,12,1.4020000000000001,1.262,ML Work
+Fr,1,6,1.94,1.8,Shannon
+Ga,3,4,0.61,0.47,Shannon
+Ga,3,5,0.6900000000000001,0.55,Shannon
+Ga,3,6,0.76,0.62,Shannon
+Ga,3,7,0.8240000000000001,0.684,ML Work
+Ga,3,8,0.89,0.75,ML Work
+Gd,3,1,0.751,0.611,ML Work
+Gd,3,2,0.8150000000000001,0.675,ML Work
+Gd,3,4,0.9430000000000001,0.803,ML Work
+Gd,3,5,1.006,0.866,ML Work
+Gd,3,6,1.0779999999999998,0.938,Shannon
+Gd,3,7,1.1400000000000001,1.0,Shannon
+Gd,3,8,1.193,1.053,Shannon
+Gd,3,9,1.2469999999999999,1.107,Shannon
+Gd,3,10,1.2879999999999998,1.148,ML Work
+Gd,2,8,1.339,1.199,ML Work
+Gd,3,12,1.346,1.206,ML Work
+Ge,4,3,0.46,0.32,ML Work
+Ge,4,4,0.53,0.39,Shannon
+Ge,4,5,0.599,0.459,ML Work
+Ge,3,4,0.607,0.467,ML Work
+Ge,4,6,0.67,0.53,Shannon
+Ge,2,3,0.677,0.537,ML Work
+Ge,4,7,0.72,0.58,ML Work
+Ge,4,8,0.776,0.636,ML Work
+Ge,2,6,0.87,0.73,Shannon
+H,1,1,-0.24,-0.38,Shannon
+H,1,2,-0.03999999999999998,-0.18,Shannon
+Hf,4,4,0.72,0.58,Shannon
+Hf,4,6,0.85,0.71,Shannon
+Hf,4,7,0.9,0.76,Shannon
+Hf,4,8,0.97,0.83,Shannon
+Hg,2,2,0.83,0.69,Shannon
+Hg,1,1,0.878,0.738,ML Work
+Hg,2,3,0.963,0.823,ML Work
+Hg,1,2,0.994,0.854,ML Work
+Hg,2,4,1.1,0.96,Shannon
+Hg,1,3,1.1099999999999999,0.97,Shannon
+Hg,2,5,1.146,1.006,ML Work
+Hg,2,6,1.1600000000000001,1.02,Shannon
+Hg,1,4,1.209,1.069,ML Work
+Hg,2,7,1.2389999999999999,1.099,ML Work
+Hg,2,8,1.2799999999999998,1.14,Shannon
+Hg,1,5,1.2879999999999998,1.148,ML Work
+Hg,1,6,1.33,1.19,Shannon
+Hg,2,9,1.3319999999999999,1.192,ML Work
+Hg,2,10,1.383,1.243,ML Work
+Hg,1,7,1.4169999999999998,1.277,ML Work
+Hg,1,8,1.48,1.34,ML Work
+Hg,2,12,1.491,1.351,ML Work
+Hg,1,9,1.5390000000000001,1.399,ML Work
+Hg,1,10,1.5939999999999999,1.454,ML Work
+Ho,3,2,0.79,0.65,ML Work
+Ho,3,3,0.853,0.713,ML Work
+Ho,3,4,0.915,0.775,ML Work
+Ho,3,5,0.977,0.837,ML Work
+Ho,3,6,1.041,0.901,Shannon
+Ho,3,7,1.099,0.959,ML Work
+Ho,3,8,1.1549999999999998,1.015,Shannon
+Ho,3,9,1.2120000000000002,1.072,Shannon
+Ho,3,10,1.2600000000000002,1.12,Shannon
+Ho,3,11,1.287,1.147,ML Work
+Ho,3,12,1.314,1.174,ML Work
+I,7,4,0.56,0.42,Shannon
+I,5,3,0.5800000000000001,0.44,Shannon
+I,7,5,0.633,0.493,ML Work
+I,7,6,0.67,0.53,Shannon
+I,5,4,0.755,0.615,ML Work
+I,7,8,0.851,0.711,ML Work
+I,5,5,0.922,0.782,ML Work
+I,5,6,1.0899999999999999,0.95,Shannon
+I,5,7,1.177,1.037,ML Work
+I,5,8,1.2530000000000001,1.113,ML Work
+I,5,9,1.3090000000000002,1.169,ML Work
+I,-1,6,2.06,2.2,Shannon
+In,3,3,0.6960000000000001,0.556,ML Work
+In,3,4,0.76,0.62,Shannon
+In,3,5,0.853,0.713,ML Work
+In,3,6,0.9400000000000001,0.8,Shannon
+In,3,7,1.0,0.86,ML Work
+In,3,8,1.06,0.92,Shannon
+In,2,6,1.1640000000000001,1.024,ML Work
+In,2,7,1.237,1.097,ML Work
+In,2,8,1.302,1.162,ML Work
+In,1,9,1.625,1.485,ML Work
+In,1,10,1.6749999999999998,1.535,ML Work
+Ir,4,4,0.621,0.481,ML Work
+Ir,6,6,0.672,0.532,ML Work
+Ir,5,6,0.71,0.57,Shannon
+Ir,4,6,0.765,0.625,Shannon
+Ir,3,6,0.8200000000000001,0.68,Shannon
+K,1,1,1.3410000000000002,1.201,ML Work
+K,1,2,1.404,1.264,ML Work
+K,1,3,1.459,1.319,ML Work
+K,1,4,1.5100000000000002,1.37,Shannon
+K,1,6,1.52,1.38,Shannon
+K,1,5,1.541,1.401,ML Work
+K,1,7,1.6,1.46,Shannon
+K,1,8,1.65,1.51,Shannon
+K,1,9,1.69,1.55,Shannon
+K,1,10,1.73,1.59,Shannon
+K,1,11,1.75,1.61,ML Work
+K,1,12,1.7799999999999998,1.64,Shannon
+K,1,13,1.8130000000000002,1.673,ML Work
+La,3,1,0.863,0.723,ML Work
+La,3,2,0.928,0.788,ML Work
+La,3,3,0.992,0.852,ML Work
+La,3,4,1.053,0.913,ML Work
+La,3,5,1.113,0.973,ML Work
+La,3,6,1.1720000000000002,1.032,Shannon
+La,3,7,1.2400000000000002,1.1,Shannon
+La,3,8,1.2999999999999998,1.16,Shannon
+La,3,9,1.3559999999999999,1.216,Shannon
+La,2,6,1.3890000000000002,1.249,ML Work
+La,3,10,1.4100000000000001,1.27,Shannon
+La,3,11,1.439,1.299,ML Work
+La,2,8,1.4849999999999999,1.345,ML Work
+La,3,12,1.5,1.36,Shannon
+La,2,9,1.537,1.397,ML Work
+La,2,10,1.5910000000000002,1.451,ML Work
+La,2,12,1.689,1.549,ML Work
+Li,1,1,0.589,0.449,ML Work
+Li,1,2,0.635,0.495,ML Work
+Li,1,3,0.683,0.543,ML Work
+Li,1,4,0.73,0.59,Shannon
+Li,1,5,0.8130000000000001,0.673,ML Work
+Li,1,6,0.9,0.76,Shannon
+Li,1,7,0.978,0.838,ML Work
+Li,1,8,1.06,0.92,Shannon
+Li,1,9,1.129,0.989,ML Work
+Li,1,10,1.194,1.054,ML Work
+Li,1,12,1.307,1.167,ML Work
+Lu,3,2,0.76,0.62,ML Work
+Lu,3,3,0.8230000000000001,0.683,ML Work
+Lu,3,5,0.9420000000000001,0.802,ML Work
+Lu,3,6,1.001,0.861,Shannon
+Lu,3,7,1.0590000000000002,0.919,ML Work
+Lu,3,8,1.117,0.977,Shannon
+Lu,3,9,1.1720000000000002,1.032,Shannon
+Lu,3,10,1.222,1.082,ML Work
+Mg,2,3,0.618,0.478,ML Work
+Mg,2,4,0.71,0.57,Shannon
+Mg,2,5,0.8,0.66,Shannon
+Mg,2,6,0.86,0.72,Shannon
+Mg,2,7,0.9480000000000001,0.808,ML Work
+Mg,2,8,1.03,0.89,Shannon
+Mg,2,9,1.097,0.957,ML Work
+Mn,7,4,0.39,0.25,Shannon
+Mn,6,4,0.395,0.255,Shannon
+Mn,5,4,0.47000000000000003,0.33,Shannon
+Mn,4,4,0.53,0.39,Shannon
+Mn,7,6,0.6000000000000001,0.46,Shannon
+Mn,4,5,0.625,0.485,ML Work
+Mn,3,4,0.66,0.52,ML Work
+Mn,2,2,0.662,0.522,ML Work
+Mn,4,6,0.67,0.53,Shannon
+Mn,3,5,0.72,0.58,Shannon
+Mn,3,6,0.72,0.58,Shannon
+Mn,2,3,0.739,0.599,ML Work
+Mn,2,4,0.8,0.66,Shannon
+Mn,2,6,0.81,0.67,Shannon
+Mn,3,7,0.83,0.69,ML Work
+Mn,2,5,0.89,0.75,Shannon
+Mn,3,8,0.924,0.784,ML Work
+Mn,2,7,1.04,0.9,Shannon
+Mn,2,8,1.1,0.96,Shannon
+Mn,2,9,1.197,1.057,ML Work
+Mn,3,12,1.241,1.101,ML Work
+Mn,2,10,1.283,1.143,ML Work
+Mn,2,12,1.42,1.28,ML Work
+Mo,5,1,0.356,0.216,ML Work
+Mo,6,2,0.368,0.228,ML Work
+Mo,6,3,0.455,0.315,ML Work
+Mo,5,3,0.518,0.378,ML Work
+Mo,6,4,0.55,0.41,Shannon
+Mo,5,4,0.6000000000000001,0.46,Shannon
+Mo,6,5,0.64,0.5,Shannon
+Mo,5,5,0.681,0.541,ML Work
+Mo,6,6,0.73,0.59,Shannon
+Mo,5,6,0.75,0.61,Shannon
+Mo,4,6,0.79,0.65,Shannon
+Mo,3,6,0.83,0.69,Shannon
+Mo,6,7,0.87,0.73,Shannon
+Mo,6,8,0.919,0.779,ML Work
+N,5,6,0.27,0.13,Shannon
+N,3,6,0.30000000000000004,0.16,Shannon
+N,-3,4,1.3199999999999998,1.46,Shannon
+Na,1,1,0.958,0.818,ML Work
+Na,1,2,1.017,0.877,ML Work
+Na,1,3,1.069,0.929,ML Work
+Na,1,4,1.13,0.99,Shannon
+Na,1,5,1.1400000000000001,1.0,Shannon
+Na,1,6,1.1600000000000001,1.02,Shannon
+Na,1,7,1.2600000000000002,1.12,Shannon
+Na,1,8,1.3199999999999998,1.18,Shannon
+Na,1,9,1.38,1.24,Shannon
+Na,1,10,1.4340000000000002,1.294,ML Work
+Na,1,11,1.484,1.344,ML Work
+Na,1,12,1.5299999999999998,1.39,Shannon
+Nb,5,4,0.62,0.48,Shannon
+Nb,4,4,0.6890000000000001,0.549,ML Work
+Nb,5,5,0.703,0.563,ML Work
+Nb,3,4,0.749,0.609,ML Work
+Nb,4,5,0.756,0.616,ML Work
+Nb,5,6,0.78,0.64,Shannon
+Nb,3,5,0.805,0.665,ML Work
+Nb,4,6,0.8200000000000001,0.68,Shannon
+Nb,5,7,0.83,0.69,Shannon
+Nb,3,6,0.86,0.72,Shannon
+Nb,5,8,0.88,0.74,Shannon
+Nb,2,4,0.895,0.755,ML Work
+Nb,4,8,0.93,0.79,Shannon
+Nb,2,5,0.956,0.816,ML Work
+Nb,2,6,1.024,0.884,ML Work
+Nd,3,1,0.828,0.688,ML Work
+Nd,3,2,0.892,0.752,ML Work
+Nd,3,3,0.954,0.814,ML Work
+Nd,3,4,1.014,0.874,ML Work
+Nd,3,5,1.072,0.932,ML Work
+Nd,3,6,1.123,0.983,Shannon
+Nd,3,7,1.189,1.049,ML Work
+Nd,3,8,1.249,1.109,Shannon
+Nd,3,9,1.303,1.163,Shannon
+Nd,3,10,1.3559999999999999,1.216,ML Work
+Nd,3,11,1.3890000000000002,1.249,ML Work
+Nd,3,12,1.4100000000000001,1.27,Shannon
+Nd,2,8,1.4300000000000002,1.29,Shannon
+Nd,2,9,1.4900000000000002,1.35,Shannon
+Nd,2,12,1.645,1.505,ML Work
+Ni,2,2,0.509,0.369,ML Work
+Ni,1,2,0.585,0.445,ML Work
+Ni,2,3,0.5900000000000001,0.45,ML Work
+Ni,3,4,0.5900000000000001,0.45,ML Work
+Ni,4,6,0.62,0.48,Shannon
+Ni,2,4,0.63,0.49,Shannon
+Ni,3,6,0.7000000000000001,0.56,Shannon
+Ni,2,5,0.77,0.63,Shannon
+Ni,2,6,0.83,0.69,Shannon
+Ni,2,7,0.926,0.786,ML Work
+Ni,2,8,1.018,0.878,ML Work
+Ni,2,9,1.1099999999999999,0.97,ML Work
+No,2,6,1.2400000000000002,1.1,Shannon
+Np,6,2,0.569,0.429,ML Work
+Np,5,2,0.653,0.513,ML Work
+Np,6,5,0.758,0.618,ML Work
+Np,5,5,0.8220000000000001,0.682,ML Work
+Np,7,6,0.85,0.71,Shannon
+Np,6,6,0.86,0.72,Shannon
+Np,5,6,0.89,0.75,Shannon
+Np,6,7,0.932,0.792,ML Work
+Np,5,7,0.962,0.822,ML Work
+Np,6,8,0.995,0.855,ML Work
+Np,4,6,1.01,0.87,Shannon
+Np,5,8,1.025,0.885,ML Work
+Np,4,8,1.12,0.98,Shannon
+Np,3,6,1.15,1.01,Shannon
+Np,2,6,1.2400000000000002,1.1,Shannon
+O,-2,2,1.21,1.35,Shannon
+O,-2,3,1.2200000000000002,1.36,Shannon
+O,-2,4,1.2399999999999998,1.38,Shannon
+O,-2,6,1.2599999999999998,1.4,Shannon
+O,-2,8,1.2799999999999998,1.42,Shannon
+Os,8,4,0.53,0.39,Shannon
+Os,7,5,0.603,0.463,ML Work
+Os,6,5,0.63,0.49,Shannon
+Os,7,6,0.665,0.525,Shannon
+Os,6,6,0.685,0.545,Shannon
+Os,5,6,0.715,0.575,Shannon
+Os,4,6,0.77,0.63,Shannon
+P,4,3,0.30100000000000005,0.161,ML Work
+P,5,4,0.31000000000000005,0.17,Shannon
+P,4,4,0.371,0.231,ML Work
+P,3,3,0.40700000000000003,0.267,ML Work
+P,5,5,0.43,0.29,Shannon
+P,5,6,0.52,0.38,Shannon
+P,3,6,0.5800000000000001,0.44,Shannon
+Pa,5,6,0.92,0.78,Shannon
+Pa,4,6,1.04,0.9,Shannon
+Pa,5,8,1.05,0.91,Shannon
+Pa,5,9,1.0899999999999999,0.95,Shannon
+Pa,4,8,1.15,1.01,Shannon
+Pa,3,6,1.1800000000000002,1.04,Shannon
+Pb,4,4,0.79,0.65,Shannon
+Pb,2,1,0.841,0.701,ML Work
+Pb,4,5,0.87,0.73,Shannon
+Pb,4,6,0.915,0.775,Shannon
+Pb,2,2,0.936,0.796,ML Work
+Pb,2,3,1.032,0.892,ML Work
+Pb,4,8,1.08,0.94,Shannon
+Pb,2,4,1.12,0.98,Shannon
+Pb,2,5,1.229,1.089,ML Work
+Pb,2,6,1.33,1.19,Shannon
+Pb,2,7,1.37,1.23,Shannon
+Pb,2,8,1.4300000000000002,1.29,Shannon
+Pb,2,9,1.4900000000000002,1.35,Shannon
+Pb,2,10,1.54,1.4,Shannon
+Pb,2,11,1.5899999999999999,1.45,Shannon
+Pb,2,12,1.63,1.49,Shannon
+Pd,2,2,0.601,0.461,ML Work
+Pd,1,2,0.73,0.59,Shannon
+Pd,4,6,0.755,0.615,Shannon
+Pd,2,4,0.78,0.64,Shannon
+Pd,3,6,0.9,0.76,Shannon
+Pd,2,6,1.0,0.86,Shannon
+Pd,2,7,1.08,0.94,ML Work
+Pd,2,8,1.1640000000000001,1.024,ML Work
+Pd,2,10,1.322,1.182,ML Work
+Pm,3,6,1.1099999999999999,0.97,Shannon
+Pm,3,8,1.233,1.093,Shannon
+Pm,3,9,1.2839999999999998,1.144,Shannon
+Po,6,6,0.81,0.67,Shannon
+Po,4,6,1.08,0.94,Shannon
+Po,4,8,1.2200000000000002,1.08,Shannon
+Pr,3,1,0.844,0.704,ML Work
+Pr,3,2,0.908,0.768,ML Work
+Pr,4,5,0.922,0.782,ML Work
+Pr,3,3,0.971,0.831,ML Work
+Pr,4,6,0.99,0.85,Shannon
+Pr,3,4,1.0310000000000001,0.891,ML Work
+Pr,4,7,1.0430000000000001,0.903,ML Work
+Pr,3,5,1.088,0.948,ML Work
+Pr,4,8,1.1,0.96,Shannon
+Pr,3,6,1.13,0.99,Shannon
+Pr,3,7,1.205,1.065,ML Work
+Pr,3,8,1.266,1.126,Shannon
+Pr,3,9,1.319,1.179,Shannon
+Pr,3,10,1.3719999999999999,1.232,ML Work
+Pr,2,6,1.3780000000000001,1.238,ML Work
+Pr,3,11,1.4060000000000001,1.266,ML Work
+Pr,3,12,1.4340000000000002,1.294,ML Work
+Pr,2,8,1.4660000000000002,1.326,ML Work
+Pr,2,12,1.665,1.525,ML Work
+Pt,2,2,0.6020000000000001,0.462,ML Work
+Pt,6,6,0.657,0.517,ML Work
+Pt,5,6,0.71,0.57,Shannon
+Pt,2,4,0.74,0.6,Shannon
+Pt,4,6,0.765,0.625,Shannon
+Pt,2,6,0.9400000000000001,0.8,Shannon
+Pt,2,7,1.0630000000000002,0.923,ML Work
+Pt,2,8,1.166,1.026,ML Work
+Pu,6,2,0.562,0.422,ML Work
+Pu,5,2,0.645,0.505,ML Work
+Pu,6,6,0.85,0.71,Shannon
+Pu,5,6,0.88,0.74,Shannon
+Pu,6,8,0.985,0.845,ML Work
+Pu,4,6,1.0,0.86,Shannon
+Pu,5,8,1.014,0.874,ML Work
+Pu,3,4,1.028,0.888,ML Work
+Pu,4,7,1.06,0.92,ML Work
+Pu,3,5,1.081,0.941,ML Work
+Pu,4,8,1.1,0.96,Shannon
+Pu,3,6,1.1400000000000001,1.0,Shannon
+Pu,3,8,1.25,1.11,ML Work
+Ra,2,8,1.62,1.48,Shannon
+Ra,2,12,1.8399999999999999,1.7,Shannon
+Rb,1,1,1.3450000000000002,1.205,ML Work
+Rb,1,2,1.416,1.276,ML Work
+Rb,1,3,1.484,1.344,ML Work
+Rb,1,4,1.548,1.408,ML Work
+Rb,1,5,1.6059999999999999,1.466,ML Work
+Rb,1,6,1.6600000000000001,1.52,Shannon
+Rb,1,7,1.7000000000000002,1.56,Shannon
+Rb,1,8,1.75,1.61,Shannon
+Rb,1,9,1.77,1.63,Shannon
+Rb,1,10,1.7999999999999998,1.66,Shannon
+Rb,1,11,1.83,1.69,Shannon
+Rb,1,12,1.8599999999999999,1.72,Shannon
+Rb,1,13,1.9129999999999998,1.773,ML Work
+Rb,1,14,1.9700000000000002,1.83,Shannon
+Re,7,4,0.52,0.38,Shannon
+Re,6,4,0.539,0.399,ML Work
+Re,5,4,0.581,0.441,ML Work
+Re,7,5,0.5960000000000001,0.456,ML Work
+Re,6,5,0.617,0.477,ML Work
+Re,4,4,0.63,0.49,ML Work
+Re,7,6,0.67,0.53,Shannon
+Re,6,6,0.6900000000000001,0.55,Shannon
+Re,5,6,0.72,0.58,Shannon
+Re,4,6,0.77,0.63,Shannon
+Re,7,8,0.807,0.667,ML Work
+Rh,5,6,0.6900000000000001,0.55,Shannon
+Rh,4,6,0.74,0.6,Shannon
+Rh,3,6,0.805,0.665,Shannon
+Rh,3,8,0.978,0.838,ML Work
+Ru,8,4,0.5,0.36,Shannon
+Ru,7,4,0.52,0.38,Shannon
+Ru,6,4,0.526,0.386,ML Work
+Ru,5,4,0.569,0.429,ML Work
+Ru,6,5,0.609,0.469,ML Work
+Ru,5,5,0.642,0.502,ML Work
+Ru,3,4,0.671,0.531,ML Work
+Ru,6,6,0.6910000000000001,0.551,ML Work
+Ru,5,6,0.705,0.565,Shannon
+Ru,4,6,0.76,0.62,Shannon
+Ru,3,6,0.8200000000000001,0.68,Shannon
+Ru,4,7,0.8250000000000001,0.685,ML Work
+Ru,4,8,0.892,0.752,ML Work
+S,5,3,0.231,0.091,ML Work
+S,6,4,0.26,0.12,Shannon
+S,4,2,0.263,0.123,ML Work
+S,4,3,0.328,0.188,ML Work
+S,6,6,0.43,0.29,Shannon
+S,3,3,0.48200000000000004,0.342,ML Work
+S,5,6,0.496,0.356,ML Work
+S,4,6,0.51,0.37,Shannon
+S,2,1,0.623,0.483,ML Work
+S,2,2,0.67,0.53,ML Work
+S,2,3,0.719,0.579,ML Work
+S,2,4,0.768,0.628,ML Work
+S,-2,6,1.7000000000000002,1.84,Shannon
+Sb,5,3,0.534,0.394,ML Work
+Sb,5,5,0.682,0.542,ML Work
+Sb,5,6,0.74,0.6,Shannon
+Sb,3,3,0.8180000000000001,0.678,ML Work
+Sb,3,4,0.9,0.76,Shannon
+Sb,3,6,0.9,0.76,Shannon
+Sb,3,5,0.9400000000000001,0.8,Shannon
+Sb,3,7,0.998,0.858,ML Work
+Sb,3,8,1.072,0.932,ML Work
+Sb,3,9,1.154,1.014,ML Work
+Sb,3,10,1.2349999999999999,1.095,ML Work
+Sc,3,2,0.569,0.429,ML Work
+Sc,3,5,0.799,0.659,ML Work
+Sc,3,6,0.885,0.745,Shannon
+Sc,3,7,0.9440000000000001,0.804,ML Work
+Sc,3,8,1.01,0.87,Shannon
+Sc,2,6,1.064,0.924,ML Work
+Sc,3,9,1.081,0.941,ML Work
+Sc,3,10,1.146,1.006,ML Work
+Se,4,1,0.265,0.125,ML Work
+Se,6,3,0.34,0.2,ML Work
+Se,4,3,0.41200000000000003,0.272,ML Work
+Se,6,4,0.42000000000000004,0.28,Shannon
+Se,6,5,0.49,0.35,ML Work
+Se,4,4,0.492,0.352,ML Work
+Se,6,6,0.56,0.42,Shannon
+Se,4,5,0.5740000000000001,0.434,ML Work
+Se,4,6,0.64,0.5,Shannon
+Se,2,1,0.659,0.519,ML Work
+Se,2,2,0.722,0.582,ML Work
+Se,4,7,0.751,0.611,ML Work
+Se,2,3,0.786,0.646,ML Work
+Se,4,8,0.843,0.703,ML Work
+Se,4,9,0.929,0.789,ML Work
+Se,2,8,1.1320000000000001,0.992,ML Work
+Se,-2,6,1.8399999999999999,1.98,Shannon
+Si,4,4,0.4,0.26,Shannon
+Si,4,5,0.47200000000000003,0.332,ML Work
+Si,4,6,0.54,0.4,Shannon
+Si,4,8,0.671,0.531,ML Work
+Sm,3,1,0.798,0.658,ML Work
+Sm,3,2,0.861,0.721,ML Work
+Sm,3,3,0.924,0.784,ML Work
+Sm,3,4,0.984,0.844,ML Work
+Sm,3,5,1.042,0.902,ML Work
+Sm,3,6,1.0979999999999999,0.958,Shannon
+Sm,3,7,1.1600000000000001,1.02,Shannon
+Sm,3,8,1.2189999999999999,1.079,Shannon
+Sm,3,9,1.2719999999999998,1.132,Shannon
+Sm,2,6,1.31,1.17,ML Work
+Sm,3,10,1.3250000000000002,1.185,ML Work
+Sm,3,11,1.358,1.218,ML Work
+Sm,2,7,1.3599999999999999,1.22,Shannon
+Sm,3,12,1.38,1.24,Shannon
+Sm,2,8,1.4100000000000001,1.27,Shannon
+Sm,2,9,1.46,1.32,Shannon
+Sn,4,4,0.6900000000000001,0.55,Shannon
+Sn,4,5,0.76,0.62,Shannon
+Sn,4,6,0.83,0.69,Shannon
+Sn,2,2,0.837,0.697,ML Work
+Sn,4,7,0.89,0.75,Shannon
+Sn,2,3,0.922,0.782,ML Work
+Sn,4,8,0.9500000000000001,0.81,Shannon
+Sn,2,4,1.002,0.862,ML Work
+Sn,2,5,1.073,0.933,ML Work
+Sn,2,6,1.139,0.999,ML Work
+Sn,2,7,1.2029999999999998,1.063,ML Work
+Sn,2,8,1.2679999999999998,1.128,ML Work
+Sn,2,9,1.335,1.195,ML Work
+Sn,2,10,1.404,1.264,ML Work
+Sr,2,1,0.9500000000000001,0.81,ML Work
+Sr,2,2,1.0310000000000001,0.891,ML Work
+Sr,2,3,1.111,0.971,ML Work
+Sr,2,4,1.186,1.046,ML Work
+Sr,2,5,1.255,1.115,ML Work
+Sr,2,6,1.3199999999999998,1.18,Shannon
+Sr,2,7,1.35,1.21,Shannon
+Sr,2,8,1.4,1.26,Shannon
+Sr,2,9,1.4500000000000002,1.31,Shannon
+Sr,2,10,1.5,1.36,Shannon
+Sr,2,11,1.541,1.401,ML Work
+Sr,2,12,1.58,1.44,Shannon
+Ta,5,4,0.618,0.478,ML Work
+Ta,5,5,0.6990000000000001,0.559,ML Work
+Ta,4,5,0.753,0.613,ML Work
+Ta,5,6,0.78,0.64,Shannon
+Ta,4,6,0.8200000000000001,0.68,Shannon
+Ta,5,7,0.83,0.69,Shannon
+Ta,3,6,0.86,0.72,Shannon
+Ta,5,8,0.88,0.74,Shannon
+Tb,3,1,0.752,0.612,ML Work
+Tb,3,2,0.8160000000000001,0.676,ML Work
+Tb,4,5,0.843,0.703,ML Work
+Tb,4,6,0.9,0.76,Shannon
+Tb,4,7,0.964,0.824,ML Work
+Tb,3,5,1.001,0.861,ML Work
+Tb,4,8,1.02,0.88,Shannon
+Tb,3,6,1.0630000000000002,0.923,Shannon
+Tb,3,7,1.12,0.98,Shannon
+Tb,3,8,1.1800000000000002,1.04,Shannon
+Tb,4,12,1.186,1.046,ML Work
+Tb,3,9,1.2349999999999999,1.095,Shannon
+Tb,3,10,1.2810000000000001,1.141,ML Work
+Tb,3,12,1.3399999999999999,1.2,ML Work
+Tc,7,4,0.51,0.37,Shannon
+Tc,7,5,0.609,0.469,ML Work
+Tc,7,6,0.7000000000000001,0.56,Shannon
+Tc,5,6,0.74,0.6,Shannon
+Tc,4,6,0.785,0.645,Shannon
+Tc,7,8,0.864,0.724,ML Work
+Te,4,2,0.5549999999999999,0.415,ML Work
+Te,6,4,0.5700000000000001,0.43,Shannon
+Te,6,5,0.638,0.498,ML Work
+Te,4,3,0.66,0.52,Shannon
+Te,6,6,0.7000000000000001,0.56,Shannon
+Te,5,5,0.79,0.65,ML Work
+Te,6,7,0.791,0.651,ML Work
+Te,4,4,0.8,0.66,Shannon
+Te,5,6,0.9,0.76,ML Work
+Te,4,5,0.9490000000000001,0.809,ML Work
+Te,4,6,1.1099999999999999,0.97,Shannon
+Te,4,7,1.149,1.009,ML Work
+Te,4,8,1.202,1.062,ML Work
+Te,4,9,1.2480000000000002,1.108,ML Work
+Te,4,10,1.2959999999999998,1.156,ML Work
+Te,-2,6,2.07,2.21,Shannon
+Th,4,4,0.937,0.797,ML Work
+Th,4,5,0.998,0.858,ML Work
+Th,4,6,1.08,0.94,Shannon
+Th,4,7,1.113,0.973,ML Work
+Th,4,8,1.19,1.05,Shannon
+Th,4,9,1.23,1.09,Shannon
+Th,4,10,1.27,1.13,Shannon
+Th,4,11,1.3199999999999998,1.18,Shannon
+Th,4,12,1.35,1.21,Shannon
+Th,3,12,1.504,1.364,ML Work
+Ti,4,1,0.323,0.183,ML Work
+Ti,4,2,0.402,0.262,ML Work
+Ti,4,3,0.48300000000000004,0.343,ML Work
+Ti,4,4,0.56,0.42,Shannon
+Ti,4,5,0.65,0.51,Shannon
+Ti,4,6,0.745,0.605,Shannon
+Ti,3,5,0.755,0.615,ML Work
+Ti,3,6,0.81,0.67,Shannon
+Ti,2,4,0.862,0.722,ML Work
+Ti,4,8,0.88,0.74,Shannon
+Ti,3,7,0.902,0.762,ML Work
+Ti,2,5,0.929,0.789,ML Work
+Ti,4,9,0.936,0.796,ML Work
+Ti,4,10,0.99,0.85,ML Work
+Ti,2,6,1.0,0.86,Shannon
+Tl,3,1,0.633,0.493,ML Work
+Tl,3,2,0.72,0.58,ML Work
+Tl,3,3,0.806,0.666,ML Work
+Tl,3,4,0.89,0.75,Shannon
+Tl,3,5,0.962,0.822,ML Work
+Tl,3,6,1.025,0.885,Shannon
+Tl,1,1,1.03,0.89,ML Work
+Tl,3,7,1.099,0.959,ML Work
+Tl,3,8,1.12,0.98,Shannon
+Tl,1,2,1.158,1.018,ML Work
+Tl,3,9,1.226,1.086,ML Work
+Tl,1,3,1.29,1.15,ML Work
+Tl,3,12,1.4009999999999998,1.261,ML Work
+Tl,1,4,1.4180000000000001,1.278,ML Work
+Tl,1,5,1.532,1.392,ML Work
+Tl,1,6,1.6400000000000001,1.5,Shannon
+Tl,1,7,1.685,1.545,ML Work
+Tl,1,8,1.73,1.59,Shannon
+Tl,1,9,1.7600000000000002,1.62,ML Work
+Tl,1,10,1.79,1.65,ML Work
+Tl,1,11,1.8199999999999998,1.68,ML Work
+Tl,1,12,1.8399999999999999,1.7,Shannon
+Tm,3,2,0.764,0.624,ML Work
+Tm,3,3,0.8270000000000001,0.687,ML Work
+Tm,3,6,1.02,0.88,Shannon
+Tm,3,7,1.076,0.936,ML Work
+Tm,3,8,1.134,0.994,Shannon
+Tm,2,6,1.17,1.03,Shannon
+Tm,3,9,1.1920000000000002,1.052,Shannon
+Tm,2,7,1.23,1.09,Shannon
+Tm,3,10,1.2309999999999999,1.091,ML Work
+Tm,2,8,1.287,1.147,ML Work
+Tm,3,12,1.29,1.15,ML Work
+Tm,2,12,1.4900000000000002,1.35,ML Work
+U,6,2,0.5900000000000001,0.45,Shannon
+U,6,3,0.624,0.484,ML Work
+U,6,4,0.66,0.52,Shannon
+U,5,2,0.664,0.524,ML Work
+U,6,5,0.769,0.629,ML Work
+U,5,5,0.834,0.694,ML Work
+U,6,6,0.87,0.73,Shannon
+U,5,6,0.9,0.76,Shannon
+U,6,7,0.9500000000000001,0.81,Shannon
+U,5,7,0.98,0.84,Shannon
+U,6,8,1.0,0.86,Shannon
+U,4,6,1.03,0.89,Shannon
+U,5,8,1.038,0.898,ML Work
+U,4,7,1.0899999999999999,0.95,Shannon
+U,4,8,1.1400000000000001,1.0,Shannon
+U,3,6,1.165,1.025,Shannon
+U,4,9,1.19,1.05,Shannon
+U,4,12,1.31,1.17,Shannon
+V,5,1,0.22300000000000003,0.083,ML Work
+V,5,2,0.31100000000000005,0.171,ML Work
+V,4,1,0.323,0.183,ML Work
+V,4,2,0.403,0.263,ML Work
+V,5,3,0.403,0.263,ML Work
+V,4,3,0.486,0.346,ML Work
+V,5,4,0.495,0.355,Shannon
+V,4,4,0.571,0.431,ML Work
+V,3,3,0.589,0.449,ML Work
+V,5,5,0.6000000000000001,0.46,Shannon
+V,3,4,0.653,0.513,ML Work
+V,4,5,0.67,0.53,Shannon
+V,5,6,0.68,0.54,Shannon
+V,3,5,0.716,0.576,ML Work
+V,4,6,0.72,0.58,Shannon
+V,5,8,0.77,0.63,ML Work
+V,3,6,0.78,0.64,Shannon
+V,4,8,0.86,0.72,Shannon
+V,2,6,0.93,0.79,Shannon
+W,6,3,0.47800000000000004,0.338,ML Work
+W,6,4,0.56,0.42,Shannon
+W,6,5,0.65,0.51,Shannon
+W,6,6,0.74,0.6,Shannon
+W,5,6,0.76,0.62,Shannon
+W,4,6,0.8,0.66,Shannon
+W,6,7,0.811,0.671,ML Work
+W,5,7,0.8250000000000001,0.685,ML Work
+W,6,8,0.877,0.737,ML Work
+Xe,8,4,0.54,0.4,Shannon
+Xe,8,6,0.62,0.48,Shannon
+Y,3,2,0.752,0.612,ML Work
+Y,3,3,0.8260000000000001,0.686,ML Work
+Y,3,4,0.899,0.759,ML Work
+Y,3,5,0.969,0.829,ML Work
+Y,3,6,1.04,0.9,Shannon
+Y,3,7,1.1,0.96,Shannon
+Y,3,8,1.1589999999999998,1.019,Shannon
+Y,2,6,1.2069999999999999,1.067,ML Work
+Y,3,9,1.2149999999999999,1.075,Shannon
+Y,3,10,1.266,1.126,ML Work
+Y,3,12,1.359,1.219,ML Work
+Yb,3,2,0.751,0.611,ML Work
+Yb,3,3,0.8150000000000001,0.675,ML Work
+Yb,3,5,0.9430000000000001,0.803,ML Work
+Yb,3,6,1.008,0.868,Shannon
+Yb,3,7,1.065,0.925,Shannon
+Yb,3,8,1.125,0.985,Shannon
+Yb,2,6,1.1600000000000001,1.02,Shannon
+Yb,3,9,1.182,1.042,Shannon
+Yb,3,10,1.2189999999999999,1.079,ML Work
+Yb,2,7,1.2200000000000002,1.08,Shannon
+Yb,3,12,1.278,1.138,ML Work
+Yb,2,8,1.2799999999999998,1.14,Shannon
+Yb,2,12,1.476,1.336,ML Work
+Zn,2,1,0.463,0.323,ML Work
+Zn,2,2,0.554,0.414,ML Work
+Zn,2,3,0.646,0.506,ML Work
+Zn,2,4,0.74,0.6,Shannon
+Zn,2,5,0.8200000000000001,0.68,Shannon
+Zn,2,6,0.88,0.74,Shannon
+Zn,2,7,0.961,0.821,ML Work
+Zn,2,8,1.04,0.9,Shannon
+Zn,2,9,1.1059999999999999,0.966,ML Work
+Zr,4,4,0.73,0.59,Shannon
+Zr,4,5,0.8,0.66,Shannon
+Zr,4,6,0.86,0.72,Shannon
+Zr,4,7,0.92,0.78,Shannon
+Zr,4,8,0.98,0.84,Shannon
+Zr,4,9,1.03,0.89,Shannon
+Zr,4,10,1.088,0.948,ML Work
```

### Comparing `SMACT-2.5.0/smact/data/solid_properties.txt` & `SMACT-2.5.1/smact/data/solid_properties.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data/solid_properties.xlsx` & `SMACT-2.5.1/smact/data/solid_properties.xlsx`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/data_loader.py` & `SMACT-2.5.1/smact/data_loader.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/distorter.py` & `SMACT-2.5.1/smact/distorter.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/dopant_prediction/doper.py` & `SMACT-2.5.1/smact/dopant_prediction/doper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,186 @@
-### This Jupyter notebook creates ntype ptype possiblie dopants for input species
-### using SMACT structure prediction
-### Working with Kieth from SCIML and Anthony
-
-###Doper ver 2
-
-# Now 'Doper' can generate possible n-type p-type dopants for multicomponent materials (i.e. Ternary, Quaternary etc).
-# Can plot the result of doping search within a single step
-# """ex) test= Doper(('Cu1+','Zn2+','Ge4+','S2-'))
-#         test.get_dopants(num_dopants = 10, plot_heatmap = True)"""
-
-
-from typing import List, Tuple
-
-from pymatgen.util import plotting
-
-import smact
-from smact.structure_prediction import mutation, utilities
-
-
-class Doper:
-    """
-    A class to search for n & p type dopants
-    Methods: get_dopants, plot_dopants
-
-    Attributes:
-        original_species: A tuple which describes the constituent species of a material. For example:
-
-            >>> test= Doper(('Cu1+','Zn2+','Ge4+','S2-'))
-            >>> test.original_species
-                ('Cu1+','Zn2+','Ge4+','S2-')
-
-    """
-
-    def __init__(self, original_species: Tuple[str, ...]):
-
-        """
-        Intialise the `Doper` class with a tuple of species
-
-        Args:
-            original_species: See :class:`~.Doper`.
-
-        """
-        self.original_species = original_species
-
-    def _get_cation_dopants(
-        self, element_objects: List[smact.Element], cations: List[str]
-    ):
-        poss_n_type_cat = []
-        poss_p_type_cat = []
-
-        for element in element_objects:
-            # [-2, -1, 0, +1, +2]
-            oxi_state = element.oxidation_states
-            el_symbol = element.symbol
-            for state in oxi_state:
-                for cation in cations:
-                    _, charge = utilities.parse_spec(cation)
-                    if state > charge:
-                        poss_n_type_cat.append(
-                            utilities.unparse_spec((el_symbol, state))
-                        )
-                    elif state < charge and state > 0:
-                        poss_p_type_cat.append(
-                            utilities.unparse_spec((el_symbol, state))
-                        )
-
-        return poss_n_type_cat, poss_p_type_cat
-
-    def _get_anion_dopants(
-        self, element_objects: List[smact.Element], anions: List[str]
-    ):
-        poss_n_type_an = []
-        poss_p_type_an = []
-
-        for element in element_objects:
-            oxi_state = element.oxidation_states
-            el_symbol = element.symbol
-            for state in oxi_state:
-                for anion in anions:
-                    _, charge = utilities.parse_spec(anion)
-                    if state > charge and state < 0:
-                        poss_n_type_an.append(
-                            utilities.unparse_spec((el_symbol, state))
-                        )
-                    elif state < charge:
-                        poss_p_type_an.append(
-                            utilities.unparse_spec((el_symbol, state))
-                        )
-        return poss_n_type_an, poss_p_type_an
-
-    def _plot_dopants(self, results: dict):
-        """
-        Uses pymatgen plotting utilities to plot the results of doping search
-        """
-        for key, val in results.items():
-            dict_results = {utilities.parse_spec(x)[0]: y for x, y in val}
-            plotting.periodic_table_heatmap(
-                elemental_data=dict_results,
-                cmap="rainbow",
-                blank_color="gainsboro",
-                edge_color="white",
-            )
-
-    def get_dopants(
-        self,
-        num_dopants: int = 5,
-        plot_heatmap: bool = False,
-    ) -> dict:
-        """
-        Args:
-            num_dopants (int): The number of suggestions to return for n- and p-type dopants.
-            plot_heatmap (bool): If True, the results of the doping search are plotted as heatmaps
-
-        Returns:
-            (dict): Dopant suggestions, given as a dictionary with keys
-            "n_type_cation", "p_type_cation", "n_type_anion", "p_type_anion".
-
-        Examples:
-            >>> test = Doper(('Ti4+','O2-'))
-            >>> print(test.get_dopants(num_dopants=2))
-                {'n-type cation substitutions': [('Ta5+', 8.790371775858281e-05),
-                ('Nb5+', 7.830035204694342e-05)],
-                'p-type cation substitutions': [('Na1+', 0.00010060400812977031),
-                ('Zn2+', 8.56373996146833e-05)],
-                'n-type anion substitutions': [('F1-', 0.01508116810515677),
-                ('Cl1-', 0.004737202729901607)],
-                'p-type anion substitutions': [('N3-', 0.0014663800608945628),
-                ('C4-', 9.31310255126729e-08)]}
-        """
-
-        cations = []
-        anions = []
-        try:
-            for ion in self.original_species:
-                _, charge = utilities.parse_spec(ion)
-                if charge > 0:
-                    cations.append(ion)
-                elif charge < 0:
-                    anions.append(ion)
-        except Exception as e:
-            print(e, "charge is not defined")
-
-        CM = mutation.CationMutator.from_json()
-
-        # call all elements
-        element_objects = list(smact.element_dictionary().values())
-
-        poss_n_type_cat, poss_p_type_cat = self._get_cation_dopants(
-            element_objects, cations
-        )
-        poss_n_type_an, poss_p_type_an = self._get_anion_dopants(
-            element_objects, anions
-        )
-
-        n_type_cat, p_type_cat, n_type_an, p_type_an = [], [], [], []
-        for cation in cations:
-            for n_specie, p_specie in zip(poss_n_type_cat, poss_p_type_cat):
-                n_type_cat.append((n_specie, CM.sub_prob(cation, n_specie)))
-                p_type_cat.append((p_specie, CM.sub_prob(cation, p_specie)))
-
-        for anion in anions:
-            for n_specie, p_specie in zip(poss_n_type_an, poss_p_type_an):
-                n_type_an.append((n_specie, CM.sub_prob(anion, n_specie)))
-                p_type_an.append((p_specie, CM.sub_prob(anion, p_specie)))
-
-        # [('B3+', 0.003), ('C4+', 0.001), (), (), ...] : list(tuple(str, float))
-        # sort by probability
-        n_type_cat.sort(key=lambda x: x[1], reverse=True)
-        p_type_cat.sort(key=lambda x: x[1], reverse=True)
-        n_type_an.sort(key=lambda x: x[1], reverse=True)
-        p_type_an.sort(key=lambda x: x[1], reverse=True)
-
-        results = {
-            "n-type cation substitutions": n_type_cat[:num_dopants],
-            "p-type cation substitutions": p_type_cat[:num_dopants],
-            "n-type anion substitutions": n_type_an[:num_dopants],
-            "p-type anion substitutions": p_type_an[:num_dopants],
-        }
-
-        # plot heatmap
-
-        if plot_heatmap:
-            self._plot_dopants(results)
-
-        # return the top (num_dopants) results for each case
-        return results
+### This Jupyter notebook creates ntype ptype possiblie dopants for input species
+### using SMACT structure prediction
+### Working with Kieth from SCIML and Anthony
+
+###Doper ver 2
+
+# Now 'Doper' can generate possible n-type p-type dopants for multicomponent materials (i.e. Ternary, Quaternary etc).
+# Can plot the result of doping search within a single step
+# """ex) test= Doper(('Cu1+','Zn2+','Ge4+','S2-'))
+#         test.get_dopants(num_dopants = 10, plot_heatmap = True)"""
+
+
+from typing import List, Tuple
+
+from pymatgen.util import plotting
+
+import smact
+from smact.structure_prediction import mutation, utilities
+
+
+class Doper:
+    """
+    A class to search for n & p type dopants
+    Methods: get_dopants, plot_dopants
+
+    Attributes:
+        original_species: A tuple which describes the constituent species of a material. For example:
+
+            >>> test= Doper(('Cu1+','Zn2+','Ge4+','S2-'))
+            >>> test.original_species
+                ('Cu1+','Zn2+','Ge4+','S2-')
+
+    """
+
+    def __init__(self, original_species: Tuple[str, ...]):
+        """
+        Intialise the `Doper` class with a tuple of species
+
+        Args:
+            original_species: See :class:`~.Doper`.
+
+        """
+        self.original_species = original_species
+
+    def _get_cation_dopants(
+        self, element_objects: List[smact.Element], cations: List[str]
+    ):
+        poss_n_type_cat = []
+        poss_p_type_cat = []
+
+        for element in element_objects:
+            # [-2, -1, 0, +1, +2]
+            oxi_state = element.oxidation_states
+            el_symbol = element.symbol
+            for state in oxi_state:
+                for cation in cations:
+                    _, charge = utilities.parse_spec(cation)
+                    if state > charge:
+                        poss_n_type_cat.append(
+                            utilities.unparse_spec((el_symbol, state))
+                        )
+                    elif state < charge and state > 0:
+                        poss_p_type_cat.append(
+                            utilities.unparse_spec((el_symbol, state))
+                        )
+
+        return poss_n_type_cat, poss_p_type_cat
+
+    def _get_anion_dopants(
+        self, element_objects: List[smact.Element], anions: List[str]
+    ):
+        poss_n_type_an = []
+        poss_p_type_an = []
+
+        for element in element_objects:
+            oxi_state = element.oxidation_states
+            el_symbol = element.symbol
+            for state in oxi_state:
+                for anion in anions:
+                    _, charge = utilities.parse_spec(anion)
+                    if state > charge and state < 0:
+                        poss_n_type_an.append(
+                            utilities.unparse_spec((el_symbol, state))
+                        )
+                    elif state < charge:
+                        poss_p_type_an.append(
+                            utilities.unparse_spec((el_symbol, state))
+                        )
+        return poss_n_type_an, poss_p_type_an
+
+    def _plot_dopants(self, results: dict):
+        """
+        Uses pymatgen plotting utilities to plot the results of doping search
+        """
+        for key, val in results.items():
+            dict_results = {utilities.parse_spec(x)[0]: y for x, y in val}
+            plotting.periodic_table_heatmap(
+                elemental_data=dict_results,
+                cmap="rainbow",
+                blank_color="gainsboro",
+                edge_color="white",
+            )
+
+    def get_dopants(
+        self,
+        num_dopants: int = 5,
+        plot_heatmap: bool = False,
+    ) -> dict:
+        """
+        Args:
+            num_dopants (int): The number of suggestions to return for n- and p-type dopants.
+            plot_heatmap (bool): If True, the results of the doping search are plotted as heatmaps
+
+        Returns:
+            (dict): Dopant suggestions, given as a dictionary with keys
+            "n_type_cation", "p_type_cation", "n_type_anion", "p_type_anion".
+
+        Examples:
+            >>> test = Doper(('Ti4+','O2-'))
+            >>> print(test.get_dopants(num_dopants=2))
+                {'n-type cation substitutions': [('Ta5+', 8.790371775858281e-05),
+                ('Nb5+', 7.830035204694342e-05)],
+                'p-type cation substitutions': [('Na1+', 0.00010060400812977031),
+                ('Zn2+', 8.56373996146833e-05)],
+                'n-type anion substitutions': [('F1-', 0.01508116810515677),
+                ('Cl1-', 0.004737202729901607)],
+                'p-type anion substitutions': [('N3-', 0.0014663800608945628),
+                ('C4-', 9.31310255126729e-08)]}
+        """
+
+        cations = []
+        anions = []
+        try:
+            for ion in self.original_species:
+                _, charge = utilities.parse_spec(ion)
+                if charge > 0:
+                    cations.append(ion)
+                elif charge < 0:
+                    anions.append(ion)
+        except Exception as e:
+            print(e, "charge is not defined")
+
+        CM = mutation.CationMutator.from_json()
+
+        # call all elements
+        element_objects = list(smact.element_dictionary().values())
+
+        poss_n_type_cat, poss_p_type_cat = self._get_cation_dopants(
+            element_objects, cations
+        )
+        poss_n_type_an, poss_p_type_an = self._get_anion_dopants(
+            element_objects, anions
+        )
+
+        n_type_cat, p_type_cat, n_type_an, p_type_an = [], [], [], []
+        for cation in cations:
+            for n_specie, p_specie in zip(poss_n_type_cat, poss_p_type_cat):
+                n_type_cat.append((n_specie, CM.sub_prob(cation, n_specie)))
+                p_type_cat.append((p_specie, CM.sub_prob(cation, p_specie)))
+
+        for anion in anions:
+            for n_specie, p_specie in zip(poss_n_type_an, poss_p_type_an):
+                n_type_an.append((n_specie, CM.sub_prob(anion, n_specie)))
+                p_type_an.append((p_specie, CM.sub_prob(anion, p_specie)))
+
+        # [('B3+', 0.003), ('C4+', 0.001), (), (), ...] : list(tuple(str, float))
+        # sort by probability
+        n_type_cat.sort(key=lambda x: x[1], reverse=True)
+        p_type_cat.sort(key=lambda x: x[1], reverse=True)
+        n_type_an.sort(key=lambda x: x[1], reverse=True)
+        p_type_an.sort(key=lambda x: x[1], reverse=True)
+
+        results = {
+            "n-type cation substitutions": n_type_cat[:num_dopants],
+            "p-type cation substitutions": p_type_cat[:num_dopants],
+            "n-type anion substitutions": n_type_an[:num_dopants],
+            "p-type anion substitutions": p_type_an[:num_dopants],
+        }
+
+        # plot heatmap
+
+        if plot_heatmap:
+            self._plot_dopants(results)
+
+        # return the top (num_dopants) results for each case
+        return results
```

### Comparing `SMACT-2.5.0/smact/lattice.py` & `SMACT-2.5.1/smact/lattice.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/lattice_parameters.py` & `SMACT-2.5.1/smact/lattice_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,15 @@
     return a, b, c, alpha, beta, gamma
 
 
 # Zn-S-Zn angle is ~109.5 degrees (from a tetrahedron). It is exactly 2*invCos(-1/3).
 # The distance of that Zn-Zn (diagonally to half the face) is (using the cosine rule) is
 # root[2(r1+r2)^2 - 2(r1+r2)^(2)cos(ZnSZn angle)].
 
+
 # B10
 def b10(shannon_radius):  # Litharge
     """The lattice parameters of Litharge
 
     Args:
         shannon_radius (list) : The radii of the a,b ions
```

### Comparing `SMACT-2.5.0/smact/oxidation_states.py` & `SMACT-2.5.1/smact/oxidation_states.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/properties.py` & `SMACT-2.5.1/smact/properties.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/screening.py` & `SMACT-2.5.1/smact/screening.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,14 @@
             Cu in +1 and +2 states)
 
     Returns: bool
     """
     if repeat_anions is False and repeat_cations is False:
         return len(symbols) == len(set(symbols))
     else:
-
         anions, cations = [], []
         for state, symbol in zip(oxidation_states, symbols):
             if state > 0:
                 cations.append(symbol)
             else:
                 anions.append(symbol)
         if not repeat_anions and len(anions) != len(set(anions)):
@@ -189,15 +188,15 @@
             compound
 
     Returns:
         bool : True if cations have higher electronegativity than
             anions, otherwise False
 
     """
-    for ((ox1, eneg1), (ox2, eneg2)) in combinations(
+    for (ox1, eneg1), (ox2, eneg2) in combinations(
         list(zip(ox_states, enegs)), 2
     ):
         if (ox1 > 0) and (ox2 < 0) and (eneg1 >= eneg2):
             return False
         elif (ox1 < 0) and (ox2 > 0) and (eneg1 <= eneg2):
             return False
         elif eneg1 is None or eneg2 is None:
@@ -228,15 +227,15 @@
             the Pauling criterion
 
     Returns:
         bool : True if cations have higher electronegativity than
             anions, otherwise False
 
     """
-    for ((ox1, eneg1), (ox2, eneg2)) in combinations(
+    for (ox1, eneg1), (ox2, eneg2) in combinations(
         list(zip(ox_states, enegs)), 2
     ):
         if (ox1 > 0) and (ox2 < 0) and ((eneg1 - eneg2) > threshold):
             return False
         elif (ox1 < 0) and (ox2 > 0) and (eneg2 - eneg1) > threshold:
             return False
     else:
@@ -306,31 +305,57 @@
 
     norm = [float(i) / sum(ML_rep) for i in ML_rep]
     return norm
 
 
 def smact_filter(
     els: Union[Tuple[Element], List[Element]],
-    threshold: int = 8,
+    threshold: Optional[int] = 8,
+    stoichs: Optional[List[List[int]]] = None,
     species_unique: bool = True,
     oxidation_states_set: str = "default",
 ) -> Union[List[Tuple[str, int, int]], List[Tuple[str, int]]]:
     """Function that applies the charge neutrality and electronegativity
     tests in one go for simple application in external scripts that
     wish to apply the general 'smact test'.
 
     Args:
         els (tuple/list): A list of smact.Element objects
         threshold (int): Threshold for stoichiometry limit, default = 8
+        stoichs (list[int]): A selection of valid stoichiometric ratios for each site.
         species_unique (bool): Whether or not to consider elements in different oxidation states as unique in the results.
         oxidation_states_set (string): A string to choose which set of oxidation states should be chosen. Options are 'default', 'icsd', 'pymatgen' and 'wiki' for the default, icsd, pymatgen structure predictor and Wikipedia (https://en.wikipedia.org/wiki/Template:List_of_oxidation_states_of_the_elements) oxidation states respectively.
     Returns:
         allowed_comps (list): Allowed compositions for that chemical system
         in the form [(elements), (oxidation states), (ratios)] if species_unique=True
         or in the form [(elements), (ratios)] if species_unique=False.
+
+    Example usage:
+        >>> from smact.screening import smact_filter
+        >>> from smact import Element
+        >>> els = (Element('Cs'), Element('Pb'), Element('I'))
+        >>> comps = smact_filter(els, threshold =5 )
+        >>> for comp in comps:
+        >>>     print(comp)
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, -4, -1), stoichiometries=(5, 1, 1))
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 1, 3))
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 2, 5))
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(2, 1, 4))
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(3, 1, 5))
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 4, -1), stoichiometries=(1, 1, 5))
+
+    Example (using stoichs):
+        >>> from smact.screening import smact_filter
+        >>> from smact import Element
+        >>> comps = smact_filter(els, stoichs = [[1],[1],[3]] )
+        >>> for comp in comps:
+        >>>     print(comp)
+        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 1, 3))
+
+
     """
 
     compositions = []
 
     # Get symbols and electronegativities
     symbols = tuple(e.symbol for e in els)
     electronegs = [e.pauling_eneg for e in els]
@@ -354,15 +379,17 @@
         warnings.warn(
             "This set of oxidation states is sourced from Wikipedia. The results from using this set could be questionable and should not be used unless you know what you are doing and have inspected the oxidation states.",
             stacklevel=2,
         )
 
     for ox_states in itertools.product(*ox_combos):
         # Test for charge balance
-        cn_e, cn_r = neutral_ratios(ox_states, threshold=threshold)
+        cn_e, cn_r = neutral_ratios(
+            ox_states, stoichs=stoichs, threshold=threshold
+        )
         # Electronegativity test
         if cn_e:
             electroneg_OK = pauling_test(ox_states, electronegs)
             if electroneg_OK:
                 for ratio in cn_r:
                     compositions.append(
                         _allowed_compositions(symbols, ox_states, ratio)
```

### Comparing `SMACT-2.5.0/smact/structure_prediction/database.py` & `SMACT-2.5.1/smact/structure_prediction/database.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/structure_prediction/mutation.py` & `SMACT-2.5.1/smact/structure_prediction/mutation.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/structure_prediction/prediction.py` & `SMACT-2.5.1/smact/structure_prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/structure_prediction/probability_models.py` & `SMACT-2.5.1/smact/structure_prediction/probability_models.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/structure_prediction/structure.py` & `SMACT-2.5.1/smact/structure_prediction/structure.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/structure_prediction/utilities.py` & `SMACT-2.5.1/smact/structure_prediction/utilities.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.0/smact/tests/test_core.py` & `SMACT-2.5.1/smact/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import smact.screening
 from smact import Species
 from smact.builder import wurtzite
 from smact.properties import band_gap_Harrison, compound_electroneg
 
 
 class TestSequenceFunctions(unittest.TestCase):
-
     # ---------------- TOP-LEVEL ----------------
 
     def test_Element_class_Pt(self):
         Pt = smact.Element("Pt")
         self.assertEqual(Pt.name, "Platinum")
         self.assertEqual(Pt.ionpot, 8.95883)
         self.assertEqual(Pt.number, 78)
@@ -335,25 +334,41 @@
         )
         self.assertEqual(
             smact.screening.ml_rep_generator([Pb, O], [1, 2]), PbO2_ml
         )
 
     def test_smact_filter(self):
         Na, Fe, Cl = (smact.Element(label) for label in ("Na", "Fe", "Cl"))
+        result = smact.screening.smact_filter([Na, Fe, Cl], threshold=2)
         self.assertEqual(
-            smact.screening.smact_filter([Na, Fe, Cl], threshold=2),
+            [(r[0], r[1], r[2]) for r in result],
             [
                 (("Na", "Fe", "Cl"), (1, -1, -1), (2, 1, 1)),
                 (("Na", "Fe", "Cl"), (1, 1, -1), (1, 1, 2)),
             ],
         )
         self.assertEqual(
             len(smact.screening.smact_filter([Na, Fe, Cl], threshold=8)), 77
         )
 
+        result = smact.screening.smact_filter(
+            [Na, Fe, Cl], stoichs=[[1], [1], [4]]
+        )
+        self.assertEqual(
+            [(r[0], r[1], r[2]) for r in result],
+            [
+                (("Na", "Fe", "Cl"), (1, 3, -1), (1, 1, 4)),
+            ],
+        )
+        stoichs = [list(range(1, 5)), list(range(1, 5)), list(range(1, 10))]
+        self.assertEqual(
+            len(smact.screening.smact_filter([Na, Fe, Cl], stoichs=stoichs)),
+            45,
+        )
+
     # ---------------- Lattice ----------------
     def test_Lattice_class(self):
         site_A = smact.lattice.Site([0, 0, 0], -1)
         site_B = smact.lattice.Site([0.5, 0.5, 0.5], [+2, +3])
         test_lattice = smact.lattice.Lattice([site_A, site_B], space_group=221)
         self.assertEqual(test_lattice.sites[0].oxidation_states, -1)
         self.assertEqual(test_lattice.sites[1].position, [0.5, 0.5, 0.5])
```

### Comparing `SMACT-2.5.0/smact/tests/test_doper.py` & `SMACT-2.5.1/smact/tests/test_doper.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import unittest
-
-import smact
-from smact.dopant_prediction import doper
-from smact.structure_prediction import mutation, utilities
-
-
-class dopant_prediction_test(unittest.TestCase):
-    def test_dopant_prediction(self):
-        num_dopants = 10
-        test_specie = ("Cu+", "Ga3+", "S2-")
-        test = doper.Doper(test_specie)
-
-        cation_max_charge = max(
-            test_specie, key=lambda x: utilities.parse_spec(x)[1]
-        )
-        anion_min_charge = min(
-            test_specie, key=lambda x: utilities.parse_spec(x)[1]
-        )
-        _, cat_charge = utilities.parse_spec(cation_max_charge)
-        _, an_charge = utilities.parse_spec(anion_min_charge)
-
-        # Assert: Length of the list and return type (dictionary: list)
-        self.assertIs(type(test.get_dopants()), dict)
-        for ls in test.get_dopants().values():
-            self.assertIs(type(ls), list)
-
-        # Assert: (cation) higher charges for n-type and lower charges for p-type
-        n_sub_list_cat = test.get_dopants().get("n-type cation substitutions")
-        p_sub_list_cat = test.get_dopants().get("p-type cation substitutions")
-        n_sub_list_an = test.get_dopants().get("n-type anion substitutions")
-        p_sub_list_an = test.get_dopants().get("p-type anion substitutions")
-        for n_atom, p_atom in zip(n_sub_list_cat, p_sub_list_cat):
-            self.assertGreater(utilities.parse_spec(n_atom[0])[1], cat_charge)
-            self.assertLess(utilities.parse_spec(p_atom[0])[1], cat_charge)
-
-        for n_atom, p_atom in zip(n_sub_list_an, p_sub_list_an):
-            self.assertGreater(utilities.parse_spec(n_atom[0])[1], an_charge)
-            self.assertLess(utilities.parse_spec(p_atom[0])[1], an_charge)
-
-
-if __name__ == "__main__":
-    TestLoader = unittest.TestLoader()
-    DoperTests = unittest.TestSuite()
-    DoperTests.addTests(
-        TestLoader.loadTestsFromTestCase(dopant_prediction_test)
-    )
-
-    runner = unittest.TextTestRunner()
-    result = runner.run(DoperTests)
+import unittest
+
+import smact
+from smact.dopant_prediction import doper
+from smact.structure_prediction import mutation, utilities
+
+
+class dopant_prediction_test(unittest.TestCase):
+    def test_dopant_prediction(self):
+        num_dopants = 10
+        test_specie = ("Cu+", "Ga3+", "S2-")
+        test = doper.Doper(test_specie)
+
+        cation_max_charge = max(
+            test_specie, key=lambda x: utilities.parse_spec(x)[1]
+        )
+        anion_min_charge = min(
+            test_specie, key=lambda x: utilities.parse_spec(x)[1]
+        )
+        _, cat_charge = utilities.parse_spec(cation_max_charge)
+        _, an_charge = utilities.parse_spec(anion_min_charge)
+
+        # Assert: Length of the list and return type (dictionary: list)
+        self.assertIs(type(test.get_dopants()), dict)
+        for ls in test.get_dopants().values():
+            self.assertIs(type(ls), list)
+
+        # Assert: (cation) higher charges for n-type and lower charges for p-type
+        n_sub_list_cat = test.get_dopants().get("n-type cation substitutions")
+        p_sub_list_cat = test.get_dopants().get("p-type cation substitutions")
+        n_sub_list_an = test.get_dopants().get("n-type anion substitutions")
+        p_sub_list_an = test.get_dopants().get("p-type anion substitutions")
+        for n_atom, p_atom in zip(n_sub_list_cat, p_sub_list_cat):
+            self.assertGreater(utilities.parse_spec(n_atom[0])[1], cat_charge)
+            self.assertLess(utilities.parse_spec(p_atom[0])[1], cat_charge)
+
+        for n_atom, p_atom in zip(n_sub_list_an, p_sub_list_an):
+            self.assertGreater(utilities.parse_spec(n_atom[0])[1], an_charge)
+            self.assertLess(utilities.parse_spec(p_atom[0])[1], an_charge)
+
+
+if __name__ == "__main__":
+    TestLoader = unittest.TestLoader()
+    DoperTests = unittest.TestSuite()
+    DoperTests.addTests(
+        TestLoader.loadTestsFromTestCase(dopant_prediction_test)
+    )
+
+    runner = unittest.TextTestRunner()
+    result = runner.run(DoperTests)
```

### Comparing `SMACT-2.5.0/smact/tests/test_structure.py` & `SMACT-2.5.1/smact/tests/test_structure.py`

 * *Files identical despite different names*

