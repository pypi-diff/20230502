# Comparing `tmp/pmutt-1.4.3.tar.gz` & `tmp/pmutt-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmutt-1.4.3.tar", last modified: Sun Mar 19 16:23:45 2023, max compression
+gzip compressed data, was "pmutt-1.4.4.tar", last modified: Tue May  2 03:28:39 2023, max compression
```

## Comparing `pmutt-1.4.3.tar` & `pmutt-1.4.4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.760013 pmutt-1.4.3/
--rw-rw-rw-   0        0        0     1082 2019-06-13 14:35:07.000000 pmutt-1.4.3/LICENSE.md
--rw-rw-rw-   0        0        0       17 2019-06-13 14:35:07.000000 pmutt-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6035 2023-03-19 16:23:45.760013 pmutt-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5485 2023-03-19 16:03:20.000000 pmutt-1.4.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.435820 pmutt-1.4.3/pmutt/
--rw-rw-rw-   0        0        0    32071 2023-03-19 16:22:25.000000 pmutt-1.4.3/pmutt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.483075 pmutt-1.4.3/pmutt/cantera/
--rw-rw-rw-   0        0        0     4338 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/cantera/__init__.py
--rw-rw-rw-   0        0        0    14184 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/cantera/phase.py
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/cantera/reaction.py
--rw-rw-rw-   0        0        0     2959 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/cantera/units.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.483075 pmutt-1.4.3/pmutt/chemkin/
--rw-rw-rw-   0        0        0     1087 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/chemkin/__init__.py
--rw-rw-rw-   0        0        0    40805 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.498731 pmutt-1.4.3/pmutt/empirical/
--rw-rw-rw-   0        0        0    23166 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/empirical/__init__.py
--rw-rw-rw-   0        0        0    86031 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/empirical/nasa.py
--rw-rw-rw-   0        0        0     9263 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/empirical/references.py
--rw-rw-rw-   0        0        0    35117 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/empirical/shomate.py
--rw-rw-rw-   0        0        0     4461 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/empirical/zacros.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.514316 pmutt-1.4.3/pmutt/eos/
--rw-rw-rw-   0        0        0     9046 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/eos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.514316 pmutt-1.4.3/pmutt/equilibrium/
--rw-rw-rw-   0        0        0       54 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/equilibrium/__init__.py
--rw-rw-rw-   0        0        0     7412 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/equilibrium/_equilibrium.py
--rw-rw-rw-   0        0        0     3452 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/examples.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.561568 pmutt-1.4.3/pmutt/io/
--rw-rw-rw-   0        0        0      662 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/io/__init__.py
--rw-rw-rw-   0        0        0     2645 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/io/cantera.py
--rw-rw-rw-   0        0        0    33834 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/io/chemkin.py
--rw-rw-rw-   0        0        0   109843 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/io/ctml_writer.py
--rw-rw-rw-   0        0        0     5692 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/io/db.py
--rw-rw-rw-   0        0        0    21207 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/io/excel.py
--rw-rw-rw-   0        0        0     5844 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/io/gaussian.py
--rw-rw-rw-   0        0        0     4692 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/io/json.py
--rw-rw-rw-   0        0        0    38155 2023-03-17 19:36:37.000000 pmutt-1.4.3/pmutt/io/omkm.py
--rw-rw-rw-   0        0        0     2132 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/io/ring.py
--rw-rw-rw-   0        0        0    14835 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/io/thermdat.py
--rw-rw-rw-   0        0        0     3093 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/io/vasp.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.561568 pmutt-1.4.3/pmutt/mixture/
--rw-rw-rw-   0        0        0     2906 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/mixture/__init__.py
--rw-rw-rw-   0        0        0     9347 2022-11-11 19:36:07.000000 pmutt-1.4.3/pmutt/mixture/cov.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.577193 pmutt-1.4.3/pmutt/omkm/
--rw-rw-rw-   0        0        0     2550 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/omkm/__init__.py
--rw-rw-rw-   0        0        0    13965 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/omkm/phase.py
--rw-rw-rw-   0        0        0    34761 2022-11-11 19:36:07.000000 pmutt-1.4.3/pmutt/omkm/reaction.py
--rw-rw-rw-   0        0        0      311 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/omkm/units.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.592816 pmutt-1.4.3/pmutt/reaction/
--rw-rw-rw-   0        0        0   120756 2022-11-11 02:30:27.000000 pmutt-1.4.3/pmutt/reaction/__init__.py
--rw-rw-rw-   0        0        0    13363 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/reaction/bep.py
--rw-rw-rw-   0        0        0    30927 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/reaction/network.py
--rw-rw-rw-   0        0        0    10567 2022-11-11 02:30:27.000000 pmutt-1.4.3/pmutt/reaction/phasediagram.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.624085 pmutt-1.4.3/pmutt/statmech/
--rw-rw-rw-   0        0        0    53576 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/statmech/__init__.py
--rw-rw-rw-   0        0        0     6215 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/statmech/elec.py
--rw-rw-rw-   0        0        0    21506 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/statmech/lsr.py
--rw-rw-rw-   0        0        0     2205 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/statmech/nucl.py
--rw-rw-rw-   0        0        0    11826 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/statmech/rot.py
--rw-rw-rw-   0        0        0     6505 2022-11-11 02:30:27.000000 pmutt-1.4.3/pmutt/statmech/trans.py
--rw-rw-rw-   0        0        0    36161 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/statmech/vib.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.655300 pmutt-1.4.3/pmutt/tests/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.659861 pmutt-1.4.3/pmutt/tests/cantera/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/cantera/__init__.py
--rw-rw-rw-   0        0        0     2343 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/tests/cantera/test_cantera.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.659861 pmutt-1.4.3/pmutt/tests/chemkin/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/chemkin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.686996 pmutt-1.4.3/pmutt/tests/empirical/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/empirical/__init__.py
--rw-rw-rw-   0        0        0    16018 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py
--rw-rw-rw-   0        0        0     4368 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py
--rw-rw-rw-   0        0        0     1365 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py
--rw-rw-rw-   0        0        0     4855 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_lsr.py
--rw-rw-rw-   0        0        0     4449 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_references.py
--rw-rw-rw-   0        0        0    21788 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_shomate.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.686996 pmutt-1.4.3/pmutt/tests/eos/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/eos/__init__.py
--rw-rw-rw-   0        0        0     2529 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/eos/test_pmutt_eos.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.718249 pmutt-1.4.3/pmutt/tests/input_output/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/input_output/__init__.py
--rw-rw-rw-   0        0        0   972790 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/input_output/test_OUTCAR
--rw-rw-rw-   0        0        0  5424027 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/input_output/test_gaussian.log
--rw-rw-rw-   0        0        0     7510 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io__thermdat.py
--rw-rw-rw-   0        0        0     4414 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io_gaussian.py
--rw-rw-rw-   0        0        0     1714 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io_vasp.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.718249 pmutt-1.4.3/pmutt/tests/mixture/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.718249 pmutt-1.4.3/pmutt/tests/omkm/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/omkm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.718249 pmutt-1.4.3/pmutt/tests/reaction/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/reaction/__init__.py
--rw-rw-rw-   0        0        0    51561 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reaction.py
--rw-rw-rw-   0        0        0    10793 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reaction_bep.py
--rw-rw-rw-   0        0        0    36667 2020-08-07 13:22:16.000000 pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reactions.py
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.749507 pmutt-1.4.3/pmutt/tests/statmech/
--rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/statmech/__init__.py
--rw-rw-rw-   0        0        0     8063 2023-01-26 19:03:21.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech.py
--rw-rw-rw-   0        0        0     3927 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_elec.py
--rw-rw-rw-   0        0        0     1385 2019-10-27 15:36:21.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_nucl.py
--rw-rw-rw-   0        0        0     4965 2022-11-11 21:22:38.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_rot.py
--rw-rw-rw-   0        0        0     4238 2022-11-11 21:20:08.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_trans.py
--rw-rw-rw-   0        0        0    11506 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_vib.py
--rw-rw-rw-   0        0        0    13434 2022-11-11 02:30:27.000000 pmutt-1.4.3/pmutt/tests/test_constants.py
--rw-rw-rw-   0        0        0    25163 2022-11-11 21:25:59.000000 pmutt-1.4.3/pmutt/tests/test_constants.xlsx
--rw-rw-rw-   0        0        0    10945 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/test_pMuTT.py
--rw-rw-rw-   0        0        0    22656 2020-03-05 17:26:34.000000 pmutt-1.4.3/pmutt/tests/test_pmutt.xlsx
-drwxrwxrwx   0        0        0        0 2023-03-19 16:23:45.459445 pmutt-1.4.3/pmutt.egg-info/
--rw-rw-rw-   0        0        0     6035 2023-03-19 16:23:45.000000 pmutt-1.4.3/pmutt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-03-19 16:23:45.000000 pmutt-1.4.3/pmutt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 16:23:45.000000 pmutt-1.4.3/pmutt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-17 19:49:43.000000 pmutt-1.4.3/pmutt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      182 2023-03-19 16:23:45.000000 pmutt-1.4.3/pmutt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-19 16:23:45.000000 pmutt-1.4.3/pmutt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 16:23:45.760013 pmutt-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-03-19 16:22:25.000000 pmutt-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.408547 pmutt-1.4.4/
+-rw-rw-rw-   0        0        0     1082 2019-06-13 14:35:07.000000 pmutt-1.4.4/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2019-06-13 14:35:07.000000 pmutt-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6035 2023-05-02 03:28:39.407469 pmutt-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5485 2023-03-19 16:03:20.000000 pmutt-1.4.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.842770 pmutt-1.4.4/pmutt/
+-rw-rw-rw-   0        0        0    32071 2023-05-02 03:27:15.000000 pmutt-1.4.4/pmutt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.890123 pmutt-1.4.4/pmutt/cantera/
+-rw-rw-rw-   0        0        0     4338 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/cantera/__init__.py
+-rw-rw-rw-   0        0        0    14184 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/cantera/phase.py
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/cantera/reaction.py
+-rw-rw-rw-   0        0        0     2959 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/cantera/units.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.890123 pmutt-1.4.4/pmutt/chemkin/
+-rw-rw-rw-   0        0        0     1087 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/chemkin/__init__.py
+-rw-rw-rw-   0        0        0    40805 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.921519 pmutt-1.4.4/pmutt/empirical/
+-rw-rw-rw-   0        0        0    23166 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/empirical/__init__.py
+-rw-rw-rw-   0        0        0    86169 2023-05-02 03:25:48.000000 pmutt-1.4.4/pmutt/empirical/nasa.py
+-rw-rw-rw-   0        0        0     9263 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/empirical/references.py
+-rw-rw-rw-   0        0        0    35117 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/empirical/shomate.py
+-rw-rw-rw-   0        0        0     4461 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/empirical/zacros.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.937106 pmutt-1.4.4/pmutt/eos/
+-rw-rw-rw-   0        0        0     9046 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/eos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.937106 pmutt-1.4.4/pmutt/equilibrium/
+-rw-rw-rw-   0        0        0       54 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/equilibrium/__init__.py
+-rw-rw-rw-   0        0        0     7412 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/equilibrium/_equilibrium.py
+-rw-rw-rw-   0        0        0     3452 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.015213 pmutt-1.4.4/pmutt/io/
+-rw-rw-rw-   0        0        0      662 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/io/__init__.py
+-rw-rw-rw-   0        0        0     2645 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/io/cantera.py
+-rw-rw-rw-   0        0        0    33834 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/io/chemkin.py
+-rw-rw-rw-   0        0        0   109843 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/io/ctml_writer.py
+-rw-rw-rw-   0        0        0     5692 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/io/db.py
+-rw-rw-rw-   0        0        0    21207 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/io/excel.py
+-rw-rw-rw-   0        0        0     5844 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/io/gaussian.py
+-rw-rw-rw-   0        0        0     4692 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/io/json.py
+-rw-rw-rw-   0        0        0    38155 2023-03-17 19:36:37.000000 pmutt-1.4.4/pmutt/io/omkm.py
+-rw-rw-rw-   0        0        0     2132 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/io/ring.py
+-rw-rw-rw-   0        0        0    14835 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/io/thermdat.py
+-rw-rw-rw-   0        0        0     3093 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.015213 pmutt-1.4.4/pmutt/mixture/
+-rw-rw-rw-   0        0        0     2906 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/mixture/__init__.py
+-rw-rw-rw-   0        0        0     9347 2022-11-11 19:36:07.000000 pmutt-1.4.4/pmutt/mixture/cov.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.062077 pmutt-1.4.4/pmutt/omkm/
+-rw-rw-rw-   0        0        0     2550 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/omkm/__init__.py
+-rw-rw-rw-   0        0        0    13965 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/omkm/phase.py
+-rw-rw-rw-   0        0        0    34761 2022-11-11 19:36:07.000000 pmutt-1.4.4/pmutt/omkm/reaction.py
+-rw-rw-rw-   0        0        0      311 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/omkm/units.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.077698 pmutt-1.4.4/pmutt/reaction/
+-rw-rw-rw-   0        0        0   120756 2022-11-11 02:30:27.000000 pmutt-1.4.4/pmutt/reaction/__init__.py
+-rw-rw-rw-   0        0        0    13363 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/reaction/bep.py
+-rw-rw-rw-   0        0        0    30927 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/reaction/network.py
+-rw-rw-rw-   0        0        0    10567 2022-11-11 02:30:27.000000 pmutt-1.4.4/pmutt/reaction/phasediagram.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.140183 pmutt-1.4.4/pmutt/statmech/
+-rw-rw-rw-   0        0        0    53576 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/statmech/__init__.py
+-rw-rw-rw-   0        0        0     6215 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/statmech/elec.py
+-rw-rw-rw-   0        0        0    21506 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/statmech/lsr.py
+-rw-rw-rw-   0        0        0     2205 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/statmech/nucl.py
+-rw-rw-rw-   0        0        0    11826 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/statmech/rot.py
+-rw-rw-rw-   0        0        0     6505 2022-11-11 02:30:27.000000 pmutt-1.4.4/pmutt/statmech/trans.py
+-rw-rw-rw-   0        0        0    36161 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/statmech/vib.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.171459 pmutt-1.4.4/pmutt/tests/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.171459 pmutt-1.4.4/pmutt/tests/cantera/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/cantera/__init__.py
+-rw-rw-rw-   0        0        0     2343 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/tests/cantera/test_cantera.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.187083 pmutt-1.4.4/pmutt/tests/chemkin/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/chemkin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.280808 pmutt-1.4.4/pmutt/tests/empirical/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/empirical/__init__.py
+-rw-rw-rw-   0        0        0    16018 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py
+-rw-rw-rw-   0        0        0     4368 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py
+-rw-rw-rw-   0        0        0     1365 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py
+-rw-rw-rw-   0        0        0     4855 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_lsr.py
+-rw-rw-rw-   0        0        0     4449 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_references.py
+-rw-rw-rw-   0        0        0    21788 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_shomate.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.280808 pmutt-1.4.4/pmutt/tests/eos/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/eos/__init__.py
+-rw-rw-rw-   0        0        0     2529 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/eos/test_pmutt_eos.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.327638 pmutt-1.4.4/pmutt/tests/input_output/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/input_output/__init__.py
+-rw-rw-rw-   0        0        0   972790 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/input_output/test_OUTCAR
+-rw-rw-rw-   0        0        0  5424027 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/input_output/test_gaussian.log
+-rw-rw-rw-   0        0        0     7510 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io__thermdat.py
+-rw-rw-rw-   0        0        0     4414 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io_gaussian.py
+-rw-rw-rw-   0        0        0     1714 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io_vasp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.327638 pmutt-1.4.4/pmutt/tests/mixture/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.327638 pmutt-1.4.4/pmutt/tests/omkm/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/omkm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.358881 pmutt-1.4.4/pmutt/tests/reaction/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/reaction/__init__.py
+-rw-rw-rw-   0        0        0    51561 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reaction.py
+-rw-rw-rw-   0        0        0    10793 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reaction_bep.py
+-rw-rw-rw-   0        0        0    36667 2020-08-07 13:22:16.000000 pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reactions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:39.390636 pmutt-1.4.4/pmutt/tests/statmech/
+-rw-rw-rw-   0        0        0        0 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/statmech/__init__.py
+-rw-rw-rw-   0        0        0     8063 2023-01-26 19:03:21.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech.py
+-rw-rw-rw-   0        0        0     3927 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_elec.py
+-rw-rw-rw-   0        0        0     1385 2019-10-27 15:36:21.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_nucl.py
+-rw-rw-rw-   0        0        0     4965 2022-11-11 21:22:38.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_rot.py
+-rw-rw-rw-   0        0        0     4238 2022-11-11 21:20:08.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_trans.py
+-rw-rw-rw-   0        0        0    11506 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_vib.py
+-rw-rw-rw-   0        0        0    13434 2022-11-11 02:30:27.000000 pmutt-1.4.4/pmutt/tests/test_constants.py
+-rw-rw-rw-   0        0        0    25163 2022-11-11 21:25:59.000000 pmutt-1.4.4/pmutt/tests/test_constants.xlsx
+-rw-rw-rw-   0        0        0    10945 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/test_pMuTT.py
+-rw-rw-rw-   0        0        0    22656 2020-03-05 17:26:34.000000 pmutt-1.4.4/pmutt/tests/test_pmutt.xlsx
+drwxrwxrwx   0        0        0        0 2023-05-02 03:28:38.858489 pmutt-1.4.4/pmutt.egg-info/
+-rw-rw-rw-   0        0        0     6035 2023-05-02 03:28:38.000000 pmutt-1.4.4/pmutt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-05-02 03:28:38.000000 pmutt-1.4.4/pmutt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 03:28:38.000000 pmutt-1.4.4/pmutt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-17 19:49:43.000000 pmutt-1.4.4/pmutt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      182 2023-05-02 03:28:38.000000 pmutt-1.4.4/pmutt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 03:28:38.000000 pmutt-1.4.4/pmutt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 03:28:39.408547 pmutt-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-05-02 03:27:15.000000 pmutt-1.4.4/setup.py
```

### Comparing `pmutt-1.4.3/LICENSE.md` & `pmutt-1.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/PKG-INFO` & `pmutt-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmutt
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python Multiscale Thermochemistry Toolbox (pmutt)
 Home-page: https://github.com/VlachosGroup/pmutt
 Author: Vlachos Research Group
 Author-email: vlachos@udel.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pmutt-1.4.3/README.rst` & `pmutt-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/__init__.py` & `pmutt-1.4.4/pmutt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ####
 #
 # setuptools likes to see a name for the package,
 # and it's best-practices to have the __version__
 # present, too:
 #
 name = 'pmutt'
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 import os
 import inspect
 import itertools
 import re
 from warnings import warn
```

### Comparing `pmutt-1.4.3/pmutt/cantera/__init__.py` & `pmutt-1.4.4/pmutt/cantera/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/cantera/phase.py` & `pmutt-1.4.4/pmutt/cantera/phase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/cantera/units.py` & `pmutt-1.4.4/pmutt/cantera/units.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/chemkin/__init__.py` & `pmutt-1.4.4/pmutt/chemkin/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/constants.py` & `pmutt-1.4.4/pmutt/constants.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/empirical/__init__.py` & `pmutt-1.4.4/pmutt/empirical/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/empirical/nasa.py` & `pmutt-1.4.4/pmutt/empirical/nasa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1756,22 +1756,24 @@
     Returns
     -------
         a6_low_out : float
             Lower a6 value for NASA polynomial
         a6_high_out : float
             Higher a6 value for NASA polynomial
     """
-    a6_low_out = (HoRT_ref - get_nasa_HoRT(a=a_low, T=T_ref)) * T_ref
-    a6_high = (HoRT_ref - get_nasa_HoRT(a=a_high, T=T_ref)) * T_ref
-
-    # Correcting for offset
-    H_low_last_T = get_nasa_HoRT(a=a_low, T=T_mid) + a6_low_out / T_mid
-    H_high_first_T = get_nasa_HoRT(a=a_high, T=T_mid) + a6_high / T_mid
-    H_offset = H_low_last_T - H_high_first_T
-    a6_high_out = T_mid * (a6_high / T_mid + H_offset)
+    if T_ref <= T_mid:
+        a6_low_out = (HoRT_ref - get_nasa_HoRT(a=a_low, T=T_ref)) * T_ref
+        a6_high_out = (get_nasa_HoRT(a=a_low, T=T_mid) +
+                       a6_low_out/T_mid - get_nasa_HoRT(a=a_high, T=T_mid))\
+            * T_mid
+    else:
+        a6_high_out = (HoRT_ref - get_nasa_HoRT(a=a_high, T=T_ref)) * T_ref
+        a6_low_out = (get_nasa_HoRT(a=a_high, T=T_mid) +
+                      a6_high_out/T_mid - get_nasa_HoRT(a=a_low, T=T_mid))\
+            * T_mid
 
     return a6_low_out, a6_high_out
 
 
 def _fit_SoR(T_ref, SoR_ref, a_low, a_high, T_mid):
     """Fit a[6] coefficient in a_low and a_high attributes given the
     dimensionless entropy
@@ -1787,22 +1789,22 @@
     Returns
     -------
         a7_low_out : float
             Lower a7 value for NASA polynomial
         a7_high_out : float
             Higher a7 value for NASA polynomial
     """
-    a7_low_out = SoR_ref - get_nasa_SoR(a=a_low, T=T_ref)
-    a7_high = SoR_ref - get_nasa_SoR(a=a_high, T=T_ref)
-
-    # Correcting for offset
-    S_low_last_T = get_nasa_SoR(a=a_low, T=T_mid) + a7_low_out
-    S_high_first_T = get_nasa_SoR(a=a_high, T=T_mid) + a7_high
-    S_offset = S_low_last_T - S_high_first_T
-    a7_high_out = a7_high + S_offset
+    if T_ref <= T_mid:
+        a7_low_out = SoR_ref - get_nasa_SoR(a=a_low, T=T_ref)
+        a7_high_out = (get_nasa_SoR(a=a_low, T=T_mid) +
+                       a7_low_out - get_nasa_SoR(a=a_high, T=T_mid))
+    else:
+        a7_high_out = SoR_ref - get_nasa_SoR(a=a_high, T=T_ref)
+        a7_low_out = (get_nasa_SoR(a=a_high, T=T_mid) +
+                      a7_high_out - get_nasa_SoR(a=a_low, T=T_mid))
 
     return a7_low_out, a7_high_out
 
 
 def _calc_T_mid_mse_nasa9(T_mid, T_low, T_high, model, n_T=50):
     """Calculates the mean squared error associated with temperature intervals
     for NASA9 polynomials
```

### Comparing `pmutt-1.4.3/pmutt/empirical/references.py` & `pmutt-1.4.4/pmutt/empirical/references.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/empirical/shomate.py` & `pmutt-1.4.4/pmutt/empirical/shomate.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/empirical/zacros.py` & `pmutt-1.4.4/pmutt/empirical/zacros.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/eos/__init__.py` & `pmutt-1.4.4/pmutt/eos/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/equilibrium/_equilibrium.py` & `pmutt-1.4.4/pmutt/equilibrium/_equilibrium.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/examples.py` & `pmutt-1.4.4/pmutt/examples.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/__init__.py` & `pmutt-1.4.4/pmutt/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/cantera.py` & `pmutt-1.4.4/pmutt/io/cantera.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/chemkin.py` & `pmutt-1.4.4/pmutt/io/chemkin.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/ctml_writer.py` & `pmutt-1.4.4/pmutt/io/ctml_writer.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/db.py` & `pmutt-1.4.4/pmutt/io/db.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/excel.py` & `pmutt-1.4.4/pmutt/io/excel.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/gaussian.py` & `pmutt-1.4.4/pmutt/io/gaussian.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/json.py` & `pmutt-1.4.4/pmutt/io/json.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/omkm.py` & `pmutt-1.4.4/pmutt/io/omkm.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/ring.py` & `pmutt-1.4.4/pmutt/io/ring.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/thermdat.py` & `pmutt-1.4.4/pmutt/io/thermdat.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/io/vasp.py` & `pmutt-1.4.4/pmutt/io/vasp.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/mixture/__init__.py` & `pmutt-1.4.4/pmutt/mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/mixture/cov.py` & `pmutt-1.4.4/pmutt/mixture/cov.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/omkm/__init__.py` & `pmutt-1.4.4/pmutt/omkm/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/omkm/phase.py` & `pmutt-1.4.4/pmutt/omkm/phase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/omkm/reaction.py` & `pmutt-1.4.4/pmutt/omkm/reaction.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/reaction/__init__.py` & `pmutt-1.4.4/pmutt/reaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/reaction/bep.py` & `pmutt-1.4.4/pmutt/reaction/bep.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/reaction/network.py` & `pmutt-1.4.4/pmutt/reaction/network.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/reaction/phasediagram.py` & `pmutt-1.4.4/pmutt/reaction/phasediagram.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/__init__.py` & `pmutt-1.4.4/pmutt/statmech/__init__.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/elec.py` & `pmutt-1.4.4/pmutt/statmech/elec.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/lsr.py` & `pmutt-1.4.4/pmutt/statmech/lsr.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/nucl.py` & `pmutt-1.4.4/pmutt/statmech/nucl.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/rot.py` & `pmutt-1.4.4/pmutt/statmech/rot.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/trans.py` & `pmutt-1.4.4/pmutt/statmech/trans.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/statmech/vib.py` & `pmutt-1.4.4/pmutt/statmech/vib.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/cantera/test_cantera.py` & `pmutt-1.4.4/pmutt/tests/cantera/test_cantera.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_Nasa.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_Nasa9.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_empiricalbase.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_lsr.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_lsr.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_references.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_references.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/empirical/test_pmutt_empirical_shomate.py` & `pmutt-1.4.4/pmutt/tests/empirical/test_pmutt_empirical_shomate.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/eos/test_pmutt_eos.py` & `pmutt-1.4.4/pmutt/tests/eos/test_pmutt_eos.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/input_output/test_OUTCAR` & `pmutt-1.4.4/pmutt/tests/input_output/test_OUTCAR`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/input_output/test_gaussian.log` & `pmutt-1.4.4/pmutt/tests/input_output/test_gaussian.log`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io__thermdat.py` & `pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io__thermdat.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io_gaussian.py` & `pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io_gaussian.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/input_output/test_pmutt_io_vasp.py` & `pmutt-1.4.4/pmutt/tests/input_output/test_pmutt_io_vasp.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reaction.py` & `pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reaction.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reaction_bep.py` & `pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reaction_bep.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/reaction/test_pmutt_reactions.py` & `pmutt-1.4.4/pmutt/tests/reaction/test_pmutt_reactions.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_elec.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_elec.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_nucl.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_nucl.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_rot.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_rot.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_trans.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_trans.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/statmech/test_pmutt_statmech_vib.py` & `pmutt-1.4.4/pmutt/tests/statmech/test_pmutt_statmech_vib.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/test_constants.py` & `pmutt-1.4.4/pmutt/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/test_constants.xlsx` & `pmutt-1.4.4/pmutt/tests/test_constants.xlsx`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/test_pMuTT.py` & `pmutt-1.4.4/pmutt/tests/test_pMuTT.py`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt/tests/test_pmutt.xlsx` & `pmutt-1.4.4/pmutt/tests/test_pmutt.xlsx`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/pmutt.egg-info/PKG-INFO` & `pmutt-1.4.4/pmutt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmutt
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python Multiscale Thermochemistry Toolbox (pmutt)
 Home-page: https://github.com/VlachosGroup/pmutt
 Author: Vlachos Research Group
 Author-email: vlachos@udel.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pmutt-1.4.3/pmutt.egg-info/SOURCES.txt` & `pmutt-1.4.4/pmutt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmutt-1.4.3/setup.py` & `pmutt-1.4.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Import the lengthy rich-text README as the package's long
 # description:
 with open('README.rst', 'r') as fh:
 	long_description = fh.read()
 
 setuptools_info = {
 	'name': 'pmutt',
-	'version': '1.4.3',
+	'version': '1.4.4',
 	'author': 'Vlachos Research Group',
 	'author_email': 'vlachos@udel.edu',
 	'description': 'Python Multiscale Thermochemistry Toolbox (pmutt)',
 	'long_description': long_description,
 	'zip_safe': False,
 	'url': 'https://github.com/VlachosGroup/pmutt',
 	'packages': setuptools.find_packages(),
```

