# Comparing `tmp/eminus-2.2.2.tar.gz` & `tmp/eminus-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eminus-2.2.2.tar", last modified: Fri Mar  3 15:24:31 2023, max compression
+gzip compressed data, was "eminus-2.3.0.tar", last modified: Tue May  2 11:49:15 2023, max compression
```

## Comparing `eminus-2.2.2.tar` & `eminus-2.3.0.tar`

### file list

```diff
@@ -1,224 +1,226 @@
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.821545 eminus-2.2.2/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4763 2023-03-03 15:07:18.000000 eminus-2.2.2/CHANGELOG.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.2.2/LICENSE
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       59 2023-02-21 16:32:19.000000 eminus-2.2.2/MANIFEST.in
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4729 2023-03-03 15:24:31.821545 eminus-2.2.2/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1386 2023-02-21 14:41:10.000000 eminus-2.2.2/README.md
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.805545 eminus-2.2.2/eminus/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1023 2022-11-01 10:58:37.000000 eminus-2.2.2/eminus/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      741 2023-01-05 09:58:30.000000 eminus-2.2.2/eminus/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15843 2023-03-03 14:26:33.000000 eminus-2.2.2/eminus/atoms.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2022-12-18 16:38:36.000000 eminus-2.2.2/eminus/data.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9919 2023-03-03 14:42:50.000000 eminus-2.2.2/eminus/dft.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3192 2023-02-21 13:30:26.000000 eminus-2.2.2/eminus/domains.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9795 2023-03-03 14:48:55.000000 eminus-2.2.2/eminus/energies.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.805545 eminus-2.2.2/eminus/extras/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      273 2023-01-26 09:18:14.000000 eminus-2.2.2/eminus/extras/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      621 2023-02-21 09:44:16.000000 eminus-2.2.2/eminus/extras/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5939 2023-02-21 09:43:34.000000 eminus-2.2.2/eminus/extras/fods.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2609 2023-01-26 09:18:47.000000 eminus-2.2.2/eminus/extras/libxc.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8500 2022-12-19 12:47:51.000000 eminus-2.2.2/eminus/extras/viewer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6353 2023-03-03 14:20:37.000000 eminus-2.2.2/eminus/gth.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.805545 eminus-2.2.2/eminus/io/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-01-22 12:58:23.000000 eminus-2.2.2/eminus/io/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-01-22 12:56:38.000000 eminus-2.2.2/eminus/io/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5876 2023-01-22 12:52:43.000000 eminus-2.2.2/eminus/io/cube.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3614 2023-02-01 15:30:13.000000 eminus-2.2.2/eminus/io/gth.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3613 2023-02-27 13:34:41.000000 eminus-2.2.2/eminus/io/json.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4008 2023-01-22 13:11:31.000000 eminus-2.2.2/eminus/io/pdb.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3319 2023-01-22 12:52:36.000000 eminus-2.2.2/eminus/io/xyz.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10648 2023-02-27 14:27:50.000000 eminus-2.2.2/eminus/localizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2731 2023-02-21 14:17:15.000000 eminus-2.2.2/eminus/logger.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13657 2023-03-03 14:47:51.000000 eminus-2.2.2/eminus/minimizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8596 2023-03-03 14:14:27.000000 eminus-2.2.2/eminus/operators.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4013 2023-02-21 09:54:41.000000 eminus-2.2.2/eminus/orbitals.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.817545 eminus-2.2.2/eminus/pade/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ac-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ac-q29
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ag-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ag-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ag-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Al-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Am-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Am-q35
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ar-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/As-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/At-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Au-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Au-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Au-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/B-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ba-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ba-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Be-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Be-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Bi-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Bk-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Bk-q37
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Br-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/C-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ca-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ca-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cd-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cd-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ce-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cf-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cf-q38
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cl-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cm-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cm-q36
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Co-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Co-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cr-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cr-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cs-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cs-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cu-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cu-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Cu-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Dy-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Er-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Es-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Es-q39
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Eu-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/F-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Fe-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Fe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Fm-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Fm-q40
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ga-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ga-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Gd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ge-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/H-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/He-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Hf-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Hg-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Hg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ho-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/I-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/In-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/In-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ir-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ir-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/K-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/K-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Kr-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/La-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Li-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Li-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Lr-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Lr-q43
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Lu-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Md-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Md-q41
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mg-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mn-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mn-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mo-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Mo-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/N-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Na-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Na-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Nb-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Nb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Nd-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ne-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ni-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ni-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/No-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/No-q42
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Np-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Np-q33
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/O-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Os-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Os-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/P-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pa-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pa-q31
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pb-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pd-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pm-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Po-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pr-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pt-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pt-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pu-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Pu-q34
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      316 2022-07-28 10:43:21.000000 eminus-2.2.2/eminus/pade/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Rb-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Rb-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Re-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Re-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Rh-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Rh-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Rn-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ru-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ru-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/S-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sc-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sc-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Se-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Si-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sm-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sn-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sr-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Sr-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ta-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ta-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tb-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tc-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tc-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Te-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Th-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Th-q30
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ti-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Ti-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tl-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tl-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Tm-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/U-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/U-q32
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/V-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/V-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/W-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/W-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Xe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Y-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Y-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Yb-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Zn-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Zn-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Zn-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Zr-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2022-08-05 11:50:42.000000 eminus-2.2.2/eminus/pade/Zr-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      823 2022-12-09 10:51:16.000000 eminus-2.2.2/eminus/pade/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2629 2023-02-23 09:47:06.000000 eminus-2.2.2/eminus/potentials.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    11448 2023-02-21 13:58:35.000000 eminus-2.2.2/eminus/scf.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     7514 2023-02-21 13:31:58.000000 eminus-2.2.2/eminus/tools.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3048 2022-11-01 10:58:37.000000 eminus-2.2.2/eminus/units.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5831 2023-03-03 14:51:06.000000 eminus-2.2.2/eminus/utils.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2016 2023-03-03 15:09:08.000000 eminus-2.2.2/eminus/version.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.821545 eminus-2.2.2/eminus/xc/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      494 2023-01-21 12:28:14.000000 eminus-2.2.2/eminus/xc/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      314 2023-01-25 09:06:37.000000 eminus-2.2.2/eminus/xc/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3169 2023-01-26 09:19:01.000000 eminus-2.2.2/eminus/xc/lda_c_chachiyo.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1923 2023-01-26 09:19:06.000000 eminus-2.2.2/eminus/xc/lda_c_chachiyo_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4002 2023-01-26 09:19:11.000000 eminus-2.2.2/eminus/xc/lda_c_pw.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1221 2023-01-26 09:19:47.000000 eminus-2.2.2/eminus/xc/lda_c_pw_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4267 2023-01-26 09:19:44.000000 eminus-2.2.2/eminus/xc/lda_c_vwn.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1659 2023-01-26 09:19:25.000000 eminus-2.2.2/eminus/xc/lda_x.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6141 2023-02-24 14:15:02.000000 eminus-2.2.2/eminus/xc/utils.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-03-03 15:24:31.805545 eminus-2.2.2/eminus.egg-info/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4729 2023-03-03 15:24:31.000000 eminus-2.2.2/eminus.egg-info/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4045 2023-03-03 15:24:31.000000 eminus-2.2.2/eminus.egg-info/SOURCES.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-03-03 15:24:31.000000 eminus-2.2.2/eminus.egg-info/dependency_links.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2022-09-27 12:14:58.000000 eminus-2.2.2/eminus.egg-info/not-zip-safe
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      290 2023-03-03 15:24:31.000000 eminus-2.2.2/eminus.egg-info/requires.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-03-03 15:24:31.000000 eminus-2.2.2/eminus.egg-info/top_level.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-01-27 17:55:16.000000 eminus-2.2.2/pyproject.toml
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-03-03 15:24:31.821545 eminus-2.2.2/setup.cfg
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3244 2023-02-27 13:03:24.000000 eminus-2.2.2/setup.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5289 2023-05-02 11:35:04.000000 eminus-2.3.0/CHANGELOG.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.3.0/LICENSE
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       59 2023-02-21 16:32:19.000000 eminus-2.3.0/MANIFEST.in
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3860 2023-05-02 11:49:15.304677 eminus-2.3.0/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1518 2023-04-19 09:05:34.000000 eminus-2.3.0/README.md
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      980 2023-04-24 14:35:56.000000 eminus-2.3.0/eminus/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      778 2023-04-11 09:05:31.000000 eminus-2.3.0/eminus/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15390 2023-04-21 15:03:17.000000 eminus-2.3.0/eminus/atoms.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4831 2023-04-21 14:57:11.000000 eminus-2.3.0/eminus/config.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2022-12-18 16:38:36.000000 eminus-2.3.0/eminus/data.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9949 2023-04-01 11:09:08.000000 eminus-2.3.0/eminus/dft.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3254 2023-04-18 09:14:40.000000 eminus-2.3.0/eminus/domains.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9822 2023-04-03 13:03:22.000000 eminus-2.3.0/eminus/energies.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus/extras/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-04-03 13:17:42.000000 eminus-2.3.0/eminus/extras/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-21 13:14:30.000000 eminus-2.3.0/eminus/extras/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6601 2023-04-27 09:30:47.000000 eminus-2.3.0/eminus/extras/fods.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2683 2023-04-17 18:01:40.000000 eminus-2.3.0/eminus/extras/libxc.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6343 2023-04-21 14:18:24.000000 eminus-2.3.0/eminus/extras/torch.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8499 2023-04-27 10:07:02.000000 eminus-2.3.0/eminus/extras/viewer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6353 2023-03-03 14:20:37.000000 eminus-2.3.0/eminus/gth.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.292677 eminus-2.3.0/eminus/io/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-01-22 12:58:23.000000 eminus-2.3.0/eminus/io/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-01-22 12:56:38.000000 eminus-2.3.0/eminus/io/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5761 2023-04-27 09:59:52.000000 eminus-2.3.0/eminus/io/cube.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3597 2023-05-02 11:28:01.000000 eminus-2.3.0/eminus/io/gth.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3442 2023-05-02 11:25:06.000000 eminus-2.3.0/eminus/io/json.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4052 2023-04-27 09:58:44.000000 eminus-2.3.0/eminus/io/pdb.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3240 2023-04-24 14:59:39.000000 eminus-2.3.0/eminus/io/xyz.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10633 2023-04-27 09:27:42.000000 eminus-2.3.0/eminus/localizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2700 2023-04-20 11:20:05.000000 eminus-2.3.0/eminus/logger.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13657 2023-04-01 10:00:08.000000 eminus-2.3.0/eminus/minimizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8614 2023-04-20 15:29:13.000000 eminus-2.3.0/eminus/operators.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4007 2023-04-27 09:27:59.000000 eminus-2.3.0/eminus/orbitals.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/eminus/pade/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ac-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ac-q29
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Al-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Am-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Am-q35
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ar-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/As-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/At-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/B-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ba-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ba-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Be-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Be-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bi-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bk-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bk-q37
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Br-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/C-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ca-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ca-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cd-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cd-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ce-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cf-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cf-q38
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cl-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cm-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cm-q36
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Co-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Co-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cr-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cr-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cs-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cs-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Dy-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Er-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Es-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Es-q39
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Eu-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/F-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fe-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fm-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fm-q40
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ga-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ga-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Gd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ge-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/H-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/He-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hf-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hg-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ho-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/I-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/In-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/In-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ir-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ir-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/K-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/K-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Kr-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/La-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Li-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Li-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lr-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lr-q43
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lu-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Md-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Md-q41
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mg-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mn-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mn-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mo-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mo-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/N-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Na-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Na-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nb-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nd-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ne-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ni-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ni-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/No-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/No-q42
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Np-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Np-q33
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/O-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Os-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Os-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/P-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pa-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pa-q31
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pb-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pd-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pm-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Po-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pr-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pt-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pt-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pu-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pu-q34
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      316 2022-07-28 10:43:21.000000 eminus-2.3.0/eminus/pade/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rb-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rb-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Re-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Re-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rh-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rh-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rn-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ru-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ru-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/S-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sc-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sc-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Se-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Si-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sm-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sn-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sr-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sr-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ta-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ta-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tb-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tc-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tc-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Te-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Th-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Th-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ti-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ti-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tl-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tl-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tm-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/U-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/U-q32
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/V-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/V-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/W-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/W-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Xe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Y-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Y-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Yb-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zr-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zr-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      837 2023-04-20 10:02:31.000000 eminus-2.3.0/eminus/pade/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2629 2023-04-28 12:30:26.000000 eminus-2.3.0/eminus/potentials.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    11803 2023-04-21 09:21:14.000000 eminus-2.3.0/eminus/scf.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8232 2023-04-21 13:09:12.000000 eminus-2.3.0/eminus/tools.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3048 2022-11-01 10:58:37.000000 eminus-2.3.0/eminus/units.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5521 2023-04-21 10:24:50.000000 eminus-2.3.0/eminus/utils.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1473 2023-05-02 11:35:17.000000 eminus-2.3.0/eminus/version.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/eminus/xc/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      494 2023-01-21 12:28:14.000000 eminus-2.3.0/eminus/xc/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      314 2023-01-25 09:06:37.000000 eminus-2.3.0/eminus/xc/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3169 2023-04-03 08:37:42.000000 eminus-2.3.0/eminus/xc/lda_c_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1923 2023-01-26 09:19:06.000000 eminus-2.3.0/eminus/xc/lda_c_chachiyo_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4004 2023-04-01 11:25:27.000000 eminus-2.3.0/eminus/xc/lda_c_pw.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1221 2023-01-26 09:19:47.000000 eminus-2.3.0/eminus/xc/lda_c_pw_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4269 2023-04-01 11:25:37.000000 eminus-2.3.0/eminus/xc/lda_c_vwn.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1660 2023-04-01 11:24:46.000000 eminus-2.3.0/eminus/xc/lda_x.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6165 2023-05-02 11:24:10.000000 eminus-2.3.0/eminus/xc/utils.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus.egg-info/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3860 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4085 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2022-09-27 12:14:58.000000 eminus-2.3.0/eminus.egg-info/not-zip-safe
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/requires.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/top_level.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-01-27 17:55:16.000000 eminus-2.3.0/pyproject.toml
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-05-02 11:49:15.304677 eminus-2.3.0/setup.cfg
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3436 2023-04-21 12:36:38.000000 eminus-2.3.0/setup.py
```

### Comparing `eminus-2.2.2/CHANGELOG.md` & `eminus-2.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Changelog
 =========
 
+v2.3.0 - May 02, 2023
+---------------------
+- New features
+   - Add Torch powered FFT operators as an extra
+      - Up to 20% faster calculations
+   - Add a consolidated configuration class
+      - Easier configuration and more performance infos
+   - Add a complete test suite
+      - Add CI/CD coverage reports
+   - Nix developer shell support
+- Miscellaneous
+   - Rewritten FODs guess function
+   - Simplify the FOD interface in io and viewer
+   - Fix a plethora of small bugs
+   - Update Docker image to Python 3.11
+
+----
+
 v2.2.2 - Mar 03, 2023
 ---------------------
 - New features
    - Improve performance, i.e, in operators, dotprod, and density calculations
    - Large and/or spin-polarized systems are much faster!
 - Coding style
    - Make Energies a dataclass
```

### Comparing `eminus-2.2.2/LICENSE` & `eminus-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/README.md` & `eminus-2.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![eminus logo](https://gitlab.com/wangenau/eminus/-/raw/main/docs/logo/eminus_logo.png)
 
 # eminus
 [![pypi](https://img.shields.io/pypi/v/eminus?color=1a962b)](https://pypi.org/project/eminus)
 [![language](https://img.shields.io/badge/language-Python3-green)](https://www.python.org)
 [![license](https://img.shields.io/badge/license-APACHE2-lightgrey)](https://gitlab.com/wangenau/eminus/-/blob/main/LICENSE)
+[![coverage](https://gitlab.com/wangenau/eminus/badges/main/coverage.svg)](https://gitlab.com/wangenau/eminus/-/graphs/main/charts)
 [![DOI](https://zenodo.org/badge/431079841.svg)](https://zenodo.org/badge/latestdoi/431079841)
 
 The eminus package is a plane wave density functional theory (DFT) code.
 It is built upon the [DFT++](https://arxiv.org/abs/cond-mat/9909130) pragmas, that aim to let programming languages and theory coincide.
 The goal is to create a simple code that is easy to read and easy to extend while using minimal dependencies.
 
 ## Documentation
```

### Comparing `eminus-2.2.2/eminus/README.md` & `eminus-2.3.0/eminus/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # eminus
 
 Main source code directory.
 
 | File           | Description |
 | :------------: | :---------: |
 | atoms.py       | Atoms class definition |
+| config.py      | Consolidated configuration module |
 | data.py        | Atom specific data |
 | dft.py         | DFT routines |
 | domains.py     | Domain generation |
 | energies.py    | Energy object and calculation |
 | gth.py         | GTH pseudopotential functions |
-| io.py          | Input/output functions |
 | localizer.py   | Localization routines |
 | logger.py      | Logging configuration |
 | minimizer.py   | Minimization algorithms |
 | operators.py   | Plane-wave basis-set dependent operators |
 | orbitals.py    | Orbital generation workflows |
 | potentials.py  | Miscellaneous (pseudo-)potentials |
 | scf.py         | SCF class definition |
-| units.py       | Constants and unit conversion functions |
 | tools.py       | Tools to calculate physical properties |
+| units.py       | Constants and unit conversion functions |
 | utils.py       | Linear algebra and random utilities |
 | version.py     | Package versions file |
-| xc.py          | Exchange-correlation functionals |
```

### Comparing `eminus-2.2.2/eminus/__init__.py` & `eminus-2.3.0/eminus/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 '''eminus - A plane wave density functional theory code.
 
 Minimal usage example to do a DFT calculation for helium::
 
    from eminus import Atoms, SCF
    atoms = Atoms('He', [0, 0, 0])
-   SCF(atoms)
+   SCF(atoms).run()
 '''
+from . import config
 from .atoms import Atoms
 from .dft import get_epsilon, get_psi
 from .io import (read, read_cube, read_json, read_xyz, write, write_cube, write_json, write_pdb,
                  write_xyz)
 from .logger import log
 from .scf import RSCF, SCF, USCF
 from .version import __version__, info
 
-__all__ = ['Atoms', 'get_epsilon', 'get_psi', 'info', 'log', 'read', 'read_cube', 'read_json',
-           'read_xyz', 'RSCF', 'SCF', 'USCF', 'write', 'write_cube', 'write_json', 'write_pdb',
-           'write_xyz', '__version__']
+__all__ = ['config', 'Atoms', 'get_epsilon', 'get_psi', 'info', 'log', 'read', 'read_cube',
+           'read_json', 'read_xyz', 'RSCF', 'SCF', 'USCF', 'write', 'write_cube', 'write_json',
+           'write_pdb', 'write_xyz', '__version__']
```

### Comparing `eminus-2.2.2/eminus/atoms.py` & `eminus-2.3.0/eminus/atoms.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 '''Atoms class definition.'''
 import re
 
 import numpy as np
 from scipy.fft import next_fast_len
 from scipy.linalg import det, eig, inv, norm
 
+from . import config, operators
 from .io import read_gth
 from .logger import create_logger, get_level, log
-from .operators import I, Idag, J, Jdag, K, L, Linv, O, T
 from .tools import center_of_mass, cutoff2gridspacing, inertia_tensor
 
 
 class Atoms:
     '''Atoms object that holds all system and cell parameters.
 
     Args:
@@ -30,15 +30,15 @@
 
             Examples: 10; [10, 10, 10]; (7, 8, 9),
             Default: 20 Bohr (ca. 10.5 Angstrom).
         ecut (float | None): Cut-off energy.
 
             None will disable the G-Vector truncation (needs a separate s).
             Default: 30 Hartree (ca. 816 eV).
-        Z (int | list | tuple | ndarray | None): Valence charge per atom.
+        Z (int | list | tuple | ndarray | dict | None): Valence charge per atom.
 
             The charges should not differ for same species. None will use valence charges from GTH
             files. The same charge for every atom will be assumed for single integers.
 
             Example: 1; [4, 1, 1, 1, 1],
             Default: None
         s (int | list | tuple | ndarray | None): Real-space sampling of the cell.
@@ -74,18 +74,18 @@
         verbose (int | str | None): Level of output (case insensitive).
 
             Can be one of 'CRITICAL', 'ERROR', 'WARNING', 'INFO', or 'DEBUG'.
             An integer value can be used as well, where larger numbers mean more output, starting
             from 0.
             None will use the default global logger value 'WARNING'.
 
-            Default: 'info'
+            Default: None
     '''
     def __init__(self, atom, X, a=20, ecut=30, Z=None, s=None, center=False, Nspin=2, f=None,
-                 Nstate=None, verbose='info'):
+                 Nstate=None, verbose=None):
         self.atom = atom      # Atom symbols
         self.X = X            # Atom positions
         self.a = a            # Cell/Vacuum size
         self.ecut = ecut      # Cut-off energy
         self.Z = Z            # Valence charges
         self.s = s            # Cell sampling
         self.center = center  # Center molecule in cell
@@ -97,18 +97,18 @@
         self.Natoms = None     # Number of atoms
         self.R = None          # Cell
         self.Omega = None      # Cell volume
         self.clear()
 
         # Initialize logger and update
         self.log = create_logger(self)
-        if verbose is None:
-            self.verbose = log.verbose
-        else:
+        if verbose is not None:
             self.verbose = verbose
+        else:
+            self.verbose = log.verbose
         self.initialize()
 
     def clear(self):
         '''Initialize and clear parameters that will be built out of the inputs.'''
         self.r = None          # Sample points in cell
         self.G = None          # G-vectors
         self.G2 = None         # Squared magnitudes of G-vectors
@@ -121,22 +121,23 @@
     def initialize(self):
         '''Validate inputs and update them if necessary.'''
         self._set_atom()
         self._set_charge()
         self._set_cell_size()
         self._set_positions()
         self._set_sampling()
-        self._set_states(self.Nspin)
         return self
 
     def build(self):
         '''Build all necessary parameters.'''
+        self._set_states(self.Nspin)
         M, N = self._get_index_matrices()
         self._set_cell(M)
         self._set_G(N)
+        self._set_operators()
         self.is_built = True
         return self
 
     kernel = build
 
     def recenter(self, center=None):
         '''Recenter the system inside the cell.
@@ -183,14 +184,16 @@
         return
 
     def _set_charge(self):
         '''Validate the Z input and calculate charges if necessary.'''
         # If only one charge is given, assume it is the charge for every atom
         if isinstance(self.Z, (int, np.integer)):
             self.Z = [self.Z] * self.Natoms
+        if isinstance(self.Z, dict):
+            self.Z = [self.Z[ia] for ia in self.atom]
         if isinstance(self.Z, (list, tuple)):
             self.Z = np.asarray(self.Z)
 
         # If no charge is given, use the ionic charge from the GTH files
         if self.Z is None:
             Z = []
             for ia in range(self.Natoms):
@@ -213,22 +216,22 @@
         # We need atom positions as an two-dimensional array
         self.X = np.atleast_2d(self.X)
         if isinstance(self.center, str):
             self.center = self.center.lower()
 
         # Center system such that the geometric inertia tensor will be diagonal
         # Rotate before shifting!
-        if self.center or self.center == 'rotate':
+        if self.center is True or self.center == 'rotate':
             X = self.X
             I = inertia_tensor(self.X)
             _, eigvecs = eig(I)
             self.X = (inv(eigvecs) @ self.X.T).T
 
         # Shift system such that its geometric center of mass is in the center of the cell
-        if self.center or self.center == 'shift':
+        if self.center is True or self.center == 'shift':
             X = self.X
             com = center_of_mass(X)
             self.X = X - (com - self.a / 2)
         return
 
     def _set_sampling(self):
         '''Validate the s input and calculate it if necessary.'''
@@ -288,40 +291,42 @@
         if self.f is None and self.Nstate is not None:
             self.f = 2 / self.Nspin * np.ones((self.Nspin, self.Nstate))
 
         # If the number of states is None and the occupations is a number or None, we are in trouble
         if self.Nstate is None:
             # If no occupations is given, assume 1 or 2
             if self.f is None:
-                f = 2 / self.Nspin
+                self.f = 2 / self.Nspin
             # Assume the number of states by dividing the total valence charge by an occupation of 2
             Ztot = np.sum(self.Z)
             self.Nstate = int(np.ceil(Ztot / 2))
-            self.f = f * np.ones((self.Nspin, self.Nstate))
+            self.f = self.f * np.ones((self.Nspin, self.Nstate))
             # Subtract the leftovers from the last spin state
             self.f[-1, -1] -= np.sum(self.Z) % 2
         return
 
     def _get_index_matrices(self):
         '''Build index matrices M and N to build the real and reciprocal space samplings.
 
+        The matrices are using C ordering (the last index is the fastest).
+
         Returns:
             tuple[ndarray, ndarray]: Index matrices.
         '''
         # Build index matrix M
         ms = np.arange(np.prod(self.s))
-        m1 = ms % self.s[0]
-        m2 = np.floor(ms / self.s[0]) % self.s[1]
-        m3 = np.floor(ms / (self.s[0] * self.s[1])) % self.s[2]
+        m1 = np.floor(ms / (self.s[2] * self.s[1])) % self.s[0]
+        m2 = np.floor(ms / self.s[2]) % self.s[1]
+        m3 = ms % self.s[2]
         M = np.column_stack((m1, m2, m3))
 
         # Build index matrix N
-        n1 = m1 - (m1 > self.s[0] / 2) * self.s[0]
+        n1 = m3 - (m3 > self.s[2] / 2) * self.s[2]
         n2 = m2 - (m2 > self.s[1] / 2) * self.s[1]
-        n3 = m3 - (m3 > self.s[2] / 2) * self.s[2]
+        n3 = m1 - (m1 > self.s[0] / 2) * self.s[0]
         N = np.column_stack((n1, n2, n3))
         return M, N
 
     def _set_cell(self, M):
         '''Build cell and create the respective sampling.
 
         Args:
@@ -356,14 +361,29 @@
         self.active = active
         self.G2c = G2[active]
 
         # Calculate the structure factor per atom
         self.Sf = np.exp(1j * G @ self.X.T).T
         return
 
+    def _set_operators(self):
+        '''Set operators of an Atoms class instance at runtime.'''
+        for op in ('O', 'L', 'Linv', 'K', 'T'):
+            setattr(type(self), op, getattr(operators, op))
+        fft_operators = ('I', 'J', 'Idag', 'Jdag')
+        # Use the Torch operators if desired, or the default ones otherwise
+        if config.use_torch:
+            from .extras import torch
+            for op in fft_operators:
+                setattr(type(self), op, getattr(torch, op))
+        else:
+            for op in fft_operators:
+                setattr(type(self), op, getattr(operators, op))
+        return
+
     def __repr__(self):
         '''Print the parameters stored in the Atoms object.'''
         out = 'Atom\tCharge\tPosition'
         for i in range(self.Natoms):
             out += f'\n{self.atom[i]}\t{self.Z[i]}\t' \
                    f'{self.X[i, 0]:10.5f}  {self.X[i, 1]:10.5f}  {self.X[i, 2]:10.5f}'
         return out
@@ -371,47 +391,10 @@
     @property
     def verbose(self):
         '''Verbosity level.'''
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
-        '''Verbosity setter to sync the logger with the property.'''
         self._verbose = get_level(level)
-        self.log.setLevel(self._verbose)
+        self.log.verbose = self._verbose
         return
-
-    def O(self, inp):
-        '''Overlap operator :func:`~eminus.operators.O`.'''
-        return O(self, inp)
-
-    def L(self, inp):
-        '''Laplacian operator :func:`~eminus.operators.L`.'''
-        return L(self, inp)
-
-    def Linv(self, inp):
-        '''Inverse Laplacian operator :func:`~eminus.operators.Linv`.'''
-        return Linv(self, inp)
-
-    def I(self, inp):
-        '''Transformation from reciprocal to real-space :func:`~eminus.operators.I`.'''
-        return I(self, inp)
-
-    def J(self, inp, full=True):
-        '''Transformation from real to reciprocal space :func:`~eminus.operators.J`.'''
-        return J(self, inp, full)
-
-    def Idag(self, inp, full=False):
-        '''Conj transformation from real to reciprocal space :func:`~eminus.operators.Idag`.'''
-        return Idag(self, inp, full)
-
-    def Jdag(self, inp):
-        '''Conj transformation from reciprocal to real-space :func:`~eminus.operators.Jdag`.'''
-        return Jdag(self, inp)
-
-    def K(self, inp):
-        '''Preconditioning operator :func:`~eminus.operators.K`.'''
-        return K(self, inp)
-
-    def T(self, inp, dr):
-        '''Translation operator :func:`~eminus.operators.T`.'''
-        return T(self, inp, dr)
```

### Comparing `eminus-2.2.2/eminus/data.py` & `eminus-2.3.0/eminus/data.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/dft.py` & `eminus-2.3.0/eminus/dft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 '''Main DFT functions based on the DFT++ formulation.'''
 import numpy as np
 from numpy.random import Generator, SFC64
 from scipy.linalg import eig, eigh, eigvalsh, inv, norm, sqrtm
 
 from .gth import calc_Vnonloc
-from .utils import diagprod, handle_spin_gracefully, pseudo_uniform
+from .utils import handle_spin_gracefully, pseudo_uniform
 from .xc import get_vxc
 
 
 def solve_poisson(atoms, n):
     '''Solve the Poisson equation.
 
     Reference: Comput. Phys. Commun. 128, 1.
@@ -133,22 +133,22 @@
         ndarray: Gradient.
     '''
     atoms = scf.atoms
     F = np.diag(atoms.f[spin])
     HW = H(scf, spin, W, Y, n, n_spin, phi, vxc)
     WHW = W[spin].conj().T @ HW
     # U = Wdag O(W)
-    U = W[spin].conj().T @ atoms.O(W[spin])
+    OW = atoms.O(W[spin])
+    U = W[spin].conj().T @ OW
     invU = inv(U)
     U12 = sqrtm(invU)
     # Htilde = U^-0.5 Wdag H(W) U^-0.5
     Ht = U12 @ WHW @ U12
     # grad E = H(W) - O(W) U^-1 (Wdag H(W)) (U^-0.5 F U^-0.5) + O(W) (U^-0.5 Q(Htilde F - F Htilde))
-    return (HW - (atoms.O(W[spin]) @ invU) @ WHW) @ (U12 @ F @ U12) + \
-        atoms.O(W[spin]) @ (U12 @ Q(Ht @ F - F @ Ht, U))
+    return (HW - (OW @ invU) @ WHW) @ (U12 @ F @ U12) + OW @ (U12 @ Q(Ht @ F - F @ Ht, U))
 
 
 def H(scf, spin, W, Y=None, n=None, n_spin=None, phi=None, vxc=None):
     '''Left-hand side of the eigenvalue equation.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
@@ -186,15 +186,16 @@
     Vxc = atoms.Jdag(atoms.O(atoms.J(vxc[spin])))
     # Vkin = -0.5 L(W)
     Vkin_psi = -0.5 * atoms.L(W[spin])
     # Veff = Jdag(Vion) + Jdag(O(J(vxc))) + Jdag(O(phi))
     Veff = scf.Vloc + Vxc + atoms.Jdag(atoms.O(phi))
     Vnonloc_psi = calc_Vnonloc(scf, W[spin])
     # H = Vkin + Idag(diag(Veff))I + Vnonloc
-    return Vkin_psi + atoms.Idag(diagprod(Veff, atoms.I(W[spin]))) + Vnonloc_psi
+    # Diag(a) * B can be written as a * B if a is a column vector
+    return Vkin_psi + atoms.Idag(Veff[:, None] * atoms.I(W[spin])) + Vnonloc_psi
 
 
 def Q(inp, U):
     '''Operator needed to calculate gradients with non-constant occupations.
 
     Reference: Comput. Phys. Commun. 128, 1.
```

### Comparing `eminus-2.2.2/eminus/domains.py` & `eminus-2.3.0/eminus/domains.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     except AttributeError:
         atoms = object
 
     if isinstance(length, (int, float)):
         length = length * np.ones(3)
     if centers is None:
         centers = center_of_mass(atoms.X)
+    centers = np.asanyarray(centers)
     # Handle each dimension seperately and add them together
     if centers.ndim == 1:
-        mask1 = (np.abs(centers[0] - atoms.r[:, 0]) < length[0])
-        mask2 = (np.abs(centers[1] - atoms.r[:, 1]) < length[1])
-        mask3 = (np.abs(centers[2] - atoms.r[:, 2]) < length[2])
+        mask1 = np.abs(centers[0] - atoms.r[:, 0]) < length[0]
+        mask2 = np.abs(centers[1] - atoms.r[:, 1]) < length[1]
+        mask3 = np.abs(centers[2] - atoms.r[:, 2]) < length[2]
         mask = mask1 & mask2 & mask3
     else:
         mask = np.zeros(len(atoms.r), dtype=bool)
         for center in centers:
-            mask1 = (np.abs(center[0] - atoms.r[:, 0]) < length[0])
-            mask2 = (np.abs(center[1] - atoms.r[:, 1]) < length[1])
-            mask3 = (np.abs(center[2] - atoms.r[:, 2]) < length[2])
+            mask1 = np.abs(center[0] - atoms.r[:, 0]) < length[0]
+            mask2 = np.abs(center[1] - atoms.r[:, 1]) < length[1]
+            mask3 = np.abs(center[2] - atoms.r[:, 2]) < length[2]
             mask = mask | (mask1 & mask2 & mask3)
     return mask
 
 
 def domain_isovalue(field, isovalue):
     '''Generate a mask for an isovalue real-space domain.
 
@@ -79,14 +80,15 @@
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if centers is None:
         centers = center_of_mass(atoms.X)
+    centers = np.asanyarray(centers)
     if centers.ndim == 1:
         mask = norm(centers - atoms.r, axis=1) < radius
     else:
         mask = np.zeros(len(atoms.r), dtype=bool)
         for center in centers:
             mask_tmp = norm(center - atoms.r, axis=1) < radius
             mask = mask | mask_tmp
```

### Comparing `eminus-2.2.2/eminus/energies.py` & `eminus-2.3.0/eminus/energies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python3
 '''Calculate different energy contributions.'''
-from dataclasses import dataclass, fields
+import dataclasses
 
 import numpy as np
 from scipy.linalg import inv, norm
 from scipy.special import erfc
 
 from .dft import get_n_single, solve_poisson
 from .xc import get_exc
 
 
-@dataclass
+@dataclasses.dataclass
 class Energy:
     '''Energy class to save energy contributions in one place.'''
-    Ekin: float = 0     # Kinetic energy
-    Ecoul: float = 0    # Coulomb energy
-    Exc: float = 0      # Exchange-correlation energy
-    Eloc: float = 0     # Local energy
-    Enonloc: float = 0  # Non-local energy
-    Eewald: float = 0   # Ewald energy
-    Esic: float = 0     # Self-interaction correction energy
+    Ekin: float = 0     #: Kinetic energy.
+    Ecoul: float = 0    #: Coulomb energy.
+    Exc: float = 0      #: Exchange-correlation energy.
+    Eloc: float = 0     #: Local energy.
+    Enonloc: float = 0  #: Non-local energy.
+    Eewald: float = 0   #: Ewald energy.
+    Esic: float = 0     #: Self-interaction correction energy.
 
     @property
     def Etot(self):
         '''Total energy is the sum of all energy contributions.'''
-        return sum(getattr(self, ie.name) for ie in fields(self))
+        return sum(getattr(self, ie.name) for ie in dataclasses.fields(self))
 
     def __repr__(self):
         '''Print the energies stored in the Energy object.'''
         out = ''
-        for ie in fields(self):
+        for ie in dataclasses.fields(self):
             energy = getattr(self, ie.name)
             if energy != 0:
                 out += f'{ie.name.ljust(8)}: {energy:+.9f} Eh\n'
         return f'{out}{"-" * 25}\nEtot    : {self.Etot:+.9f} Eh'
 
 
 def get_E(scf):
```

### Comparing `eminus-2.2.2/eminus/extras/__init__.py` & `eminus-2.3.0/eminus/extras/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
     pip install eminus[all]
 
 Alternativle, you can only install selected extras using the respective name:
 
 * :mod:`~eminus.extras.fods`
 * :mod:`~eminus.extras.libxc`
+* :mod:`~eminus.extras.torch`
 * :mod:`~eminus.extras.viewer`
 '''
-from .fods import get_fods, pycom, remove_core_fods, split_fods
+from .fods import get_fods, remove_core_fods, split_fods
 from .libxc import libxc_functional
 from .viewer import view, view_atoms, view_file
 
-__all__ = ['get_fods', 'libxc_functional', 'pycom', 'remove_core_fods', 'split_fods', 'view',
-           'view_atoms', 'view_file']
+__all__ = ['get_fods', 'libxc_functional', 'remove_core_fods', 'split_fods', 'view', 'view_atoms',
+           'view_file']
```

### Comparing `eminus-2.2.2/eminus/extras/fods.py` & `eminus-2.3.0/eminus/extras/fods.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,68 @@
 #!/usr/bin/env python3
 '''Fermi-orbital descriptor generation.'''
-import pathlib
-
 import numpy as np
 from scipy.linalg import norm
 
 from ..data import SYMBOL2NUMBER
 from ..logger import log
-from ..tools import center_of_mass
-from ..units import ang2bohr, bohr2ang
+from ..units import bohr2ang
+
+
+def get_localized_orbitals(mf, Nspin, loc, Nit=1000, seed=1234):
+    '''Generate localized orbitals with an additional simple stability analysis.
+
+    Same as implemented in PyFLOSIC2.
+
+    Reference: J. Chem. Phys. 153, 084104.
+
+    Args:
+        mf: PySCF SCF object.
+        Nspin (int): Number of spin states.
+        loc (str): Localization method (case insensitive).
+
+    Keyword Args:
+        Nit (int): Number of tries to get a solution with positive eigenvalues.
+        seed (int): Seed to initialize the random number generator.
+
+    Returns:
+        list: Localized occupied orbital coefficients per spin channel.
+    '''
+    rng = np.random.default_rng(seed=seed)
+    from pyscf.lo import boys, edmiston, pipek
+    loc_dict = {'ER': edmiston.EdmistonRuedenberg,
+                'FB': boys.Boys,
+                'GPM': pipek.PipekMezey,
+                'PM': pipek.PipekMezey}
+
+    loc_orb = []
+    # Localize each spin channel separately
+    for s in range(Nspin):
+        # Initialize the localizer object
+        if Nspin == 2:
+            localizer = loc_dict[loc](mf.mol, mf.mo_coeff[s][:, mf.mo_occ[s] > 0])
+        else:
+            localizer = loc_dict[loc](mf.mol, mf.mo_coeff[:, mf.mo_occ > 0])
+
+        # Set the population method in generalized PM to Becke charges
+        if loc == 'GPM':
+            localizer.pop_method = 'becke'
+
+        for _ in range(Nit):
+            tmp_orb = localizer.kernel()
+            # Calculate the eigenvalues of the Hessian
+            _, _, h_diag = localizer.gen_g_hop(u=np.eye(len(tmp_orb[0])))
+            # If there are no eigenvalues or all of them are positive break the loop
+            if len(h_diag) == 0 or np.min(h_diag) > 0:
+                break
+            # If not continue with randomly 'displaced' orbitals
+            noise = rng.normal(scale=5e-4, size=tmp_orb.shape)
+            localizer.mo_coeff = tmp_orb + noise
+        loc_orb.append(tmp_orb)
+    return loc_orb
 
 
 def get_fods(object, basis='pc-1', loc='FB', clean=True, elec_symbols=None):
     '''Generate FOD positions using the PyCOM method.
 
     Reference: J. Comput. Chem. 40, 2843.
 
@@ -25,18 +75,15 @@
         clean (bool): Remove log files.
         elec_symbols (list): Identifier for up and down FODs.
 
     Returns:
         ndarray: FOD positions.
     '''
     try:
-        from pyflosic2.atoms.atoms import Atoms
-        from pyflosic2.guess.pycom import pycom
-        from pyflosic2.parameters.flosic_parameters import parameters
-        from pyscf.gto import Mole  # PySCF is a dependency of PyFLOSIC2
+        from pyscf.gto import Mole
         from pyscf.scf import UKS, RKS
     except ImportError:
         log.exception('Necessary dependencies not found. To use this module, '
                       'install them with "pip install eminus[fods]".\n\n')
         raise
 
     try:
@@ -61,41 +108,31 @@
         spin = int(np.sum(atoms.f[0] - atoms.f[1]))
     else:
         spin = int(np.sum(atoms.Z) % 2)
 
     # Do the PySCF DFT calculation
     # Use Mole.build() over M() since the parse_arg option breaks testing with pytest
     mol = Mole(atom=atom_pyscf, basis=basis, spin=spin).build(parse_arg=False)
-    if atoms.Nspin == 2:
-        mf = UKS(mol=mol)
-    else:
+    if atoms.Nspin == 1:
         mf = RKS(mol=mol)
+    else:
+        mf = UKS(mol=mol)
     mf.verbose = 0
     mf.kernel()
 
-    # Do the PyCOM FOD generation
-    atoms_pyflosic = Atoms(atoms.atom, X, elec_symbols=elec_symbols, spin=spin)
-    if atoms.Nspin == 2:
-        p = parameters(mode='unrestricted')
-    else:
-        p = parameters(mode='restricted')
-    p.nuclei = atoms_pyflosic
-    p.basis = basis
-    p.pycom_loc = loc
-    pc = pycom(mf=mf, p=p)
-    pc.get_guess()
-
-    fod1 = ang2bohr(pc.p.fod1.positions)
-    fod2 = ang2bohr(pc.p.fod2.positions)
-    fods = [np.asarray(fod1), np.asarray(fod2)]
-
-    if clean:
-        pathlib.Path(p.log_name).unlink()
-        pathlib.Path(f'{loc}_GUESS_COM.xyz').unlink()
-    return fods
+    # Get the localized orbital coefficients
+    loc_orb = get_localized_orbitals(mf, atoms.Nspin, loc)
+    # Calculate the COMs
+    loc_com = []
+    ao = mf._numint.eval_ao(mf.mol, mf.grids.coords)
+    for s in range(atoms.Nspin):
+        phi = ao @ loc_orb[s]
+        dens = phi.conj() * phi * mf.grids.weights[:, None]
+        loc_com.append(dens.T @ mf.grids.coords)
+    return loc_com
 
 
 def split_fods(atom, X, elec_symbols=None):
     '''Split atom and FOD coordinates.
 
     Args:
         atom (list): Atom symbols.
@@ -113,29 +150,29 @@
     X_fod_up = []
     X_fod_dn = []
     # Iterate in reverted order, because we may delete elements
     for ia in range(len(X) - 1, -1, -1):
         if atom[ia] in elec_symbols:
             if atom[ia] in elec_symbols[0]:
                 X_fod_up.append(X[ia])
-            if atom[ia] in elec_symbols[1]:
+            if len(elec_symbols) > 1 and atom[ia] in elec_symbols[1]:
                 X_fod_dn.append(X[ia])
             X = np.delete(X, ia, axis=0)
             del atom[ia]
 
     X_fod = [np.asarray(X_fod_up), np.asarray(X_fod_dn)]
     return atom, X, X_fod
 
 
 def remove_core_fods(object, fods):
     '''Remove core FODs from a set of FOD coordinates.
 
     Args:
         object: Atoms or SCF object.
-        fods (ndarray): FOD positions.
+        fods (list): FOD positions.
 
     Returns:
         ndarray: Valence FOD positions.
     '''
     try:
         atoms = object.atoms
     except AttributeError:
@@ -144,51 +181,19 @@
     # If the number of valence electrons is the same as the number of FODs, do nothing
     if atoms.Nspin == 1 and len(fods[0]) * 2 == np.sum(atoms.f[0]):
         return fods
     if atoms.Nspin == 2 and len(fods[0]) == np.sum(atoms.f[0]) \
             and len(fods[1]) == np.sum(atoms.f[1]):
         return fods
 
-    for spin in range(atoms.Nspin):
+    for s in range(atoms.Nspin):
         for ia in range(atoms.Natoms):
             n_core = SYMBOL2NUMBER[atoms.atom[ia]] - atoms.Z[ia]
             # In the spin-paired case two electrons are one state
             # Since only core states are removed in pseudopotentials this value is divisible by 2
             # +1 to account for uneven amount of core FODs (e.g., for hydrogen)
             n_core = (n_core + 1) // 2
-            dist = norm(fods[spin] - atoms.X[ia], axis=1)
+            dist = norm(fods[s] - atoms.X[ia], axis=1)
             idx = np.argsort(dist)
             # Remove core FODs with the smallest distance to the core
-            fods[spin] = np.delete(fods[spin], idx[:n_core], axis=0)
+            fods[s] = np.delete(fods[s], idx[:n_core], axis=0)
     return fods
-
-
-def pycom(object, psirs):
-    '''Calculate the orbital center of masses, e.g., from localized orbitals.
-
-    Args:
-        object: Atoms or SCF object.
-        psirs (ndarray): Set of orbitals in real-space.
-
-    Returns:
-        bool: Center of masses.
-    '''
-    try:
-        atoms = object.atoms
-    except AttributeError:
-        atoms = object
-
-    coms = []
-    Ncom = psirs.shape[2]
-    for spin in range(atoms.Nspin):
-        coms_spin = np.empty((Ncom, 3))
-
-        # Square orbitals
-        psi2 = np.real(psirs[spin, :, :].conj() * psirs[spin, :, :])
-        for i in range(Ncom):
-            coms_spin[i] = center_of_mass(atoms.r, psi2[:, i])
-        coms.append(coms_spin)
-
-    # Have the same data structure as for fods
-    if atoms.Nspin == 1:
-        coms.append(np.array([]))
-    return coms
```

### Comparing `eminus-2.2.2/eminus/extras/libxc.py` & `eminus-2.3.0/eminus/extras/libxc.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Alternatively, one can use the PySCF Libxc interface with::
 
     pip install eminus[libxc]
 '''
 import numpy as np
 
+from .. import config
 from ..logger import log
 
 
 def libxc_functional(xc, n_spin, Nspin):
     '''Handle Libxc exchange-correlation functionals via pylibxc.
 
     Only LDA functionals should be used.
@@ -26,16 +27,17 @@
         n_spin (ndarray): Real-space electronic densities per spin channel.
         Nspin (int): Number of spin states.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange-correlation energy density and potential.
     '''
     try:
+        assert config.use_pylibxc
         from pylibxc import LibXCFunctional
-    except ImportError:
+    except (ImportError, AssertionError):
         return pyscf_functional(xc, n_spin, Nspin)
 
     # Libxc functionals have one integer and one string identifier
     try:
         func = LibXCFunctional(int(xc), Nspin)
     except ValueError:
         func = LibXCFunctional(xc, Nspin)
```

### Comparing `eminus-2.2.2/eminus/extras/viewer.py` & `eminus-2.3.0/eminus/extras/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,22 @@
                                  mode='markers',
                                  marker=dict(size=2 * np.pi * np.sqrt(COVALENT_RADII[ia]),
                                              color=CPK_COLORS[ia],
                                              line={'color': 'black', 'width': 2}))
         fig.add_trace(atom_data)
     if extra is not None:
         # If a list has been provided with the length of two it has to be FODs
-        if isinstance(extra, list) and len(extra) == 2:
-            if extra[0].size != 0:
+        if isinstance(extra, list):
+            if len(extra[0]) != 0:
                 extra_data = go.Scatter3d(x=extra[0][:, 0], y=extra[0][:, 1], z=extra[0][:, 2],
                                           name='up-FOD',
                                           mode='markers',
                                           marker=dict(size=np.pi, color='red'))
                 fig.add_trace(extra_data)
-            if extra[1].size != 0:
+            if len(extra) > 1 and len(extra[1]) != 0:
                 extra_data = go.Scatter3d(x=extra[1][:, 0], y=extra[1][:, 1], z=extra[1][:, 2],
                                           name='down-FOD',
                                           mode='markers',
                                           marker=dict(size=np.pi, color='green'))
                 fig.add_trace(extra_data)
         # Treat extra as normal coordinates otherwise
         else:
```

### Comparing `eminus-2.2.2/eminus/gth.py` & `eminus-2.3.0/eminus/gth.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/io/__init__.py` & `eminus-2.3.0/eminus/io/__init__.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/io/cube.py` & `eminus-2.3.0/eminus/io/cube.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # Following lines contain atom positions with the format: atom-id charge x-pos y-pos z-pos
         for line in lines[6:]:
             line_split = line.strip().split()
             # If the first value is not a (positive) integer, we have reached the field data
             if not line_split[0].isdigit():
                 break
             atom.append(NUMBER2SYMBOL[int(line_split[0])])
-            Z.append(line_split[1])
+            Z.append(float(line_split[1]))
             X.append(np.float_(line_split[2:5]))
 
     X = np.asarray(X)
     return atom, X, Z, a, s
 
 
 def write_cube(object, filename, field, fods=None, elec_symbols=None):
@@ -109,32 +109,30 @@
         # Print information about the file and program, and the file creation time.
         fp.write(f'File generated with eminus {__version__} on {time.ctime()}\n\n')
         # Number of atoms (int), and origin of the coordinate system (float)
         # The origin is normally at 0,0,0 but we could move our box, so take the minimum
         if fods is None:
             fp.write(f'{atoms.Natoms}  ')
         else:
-            fp.write(f'{atoms.Natoms + len(fods[0]) + len(fods[1])}  ')
+            fp.write(f'{atoms.Natoms + sum([len(i) for i in fods])}  ')
         fp.write('0.0  0.0  0.0\n')
         # Number of points per axis (int), and vector defining the axis (float)
         # We only have a cuboidal box, so each vector only has one non-zero component
         fp.write(f'{atoms.s[0]}  {atoms.a[0] / atoms.s[0]:.6f}  0.0  0.0\n'
                  f'{atoms.s[1]}  0.0  {atoms.a[1] / atoms.s[1]:.6f}  0.0\n'
                  f'{atoms.s[2]}  0.0  0.0  {atoms.a[2] / atoms.s[2]:.6f}\n')
         # Atomic number (int), atomic charge (float), and atom position (floats) for every atom
         for ia in range(atoms.Natoms):
             fp.write(f'{SYMBOL2NUMBER[atoms.atom[ia]]}  {atoms.Z[ia]:.3f}  '
                      f'{atoms.X[ia, 0]: .6f}  {atoms.X[ia, 1]: .6f}  {atoms.X[ia, 2]: .6f}\n')
         if fods is not None:
-            for ie in fods[0]:
-                fp.write(f'{SYMBOL2NUMBER[elec_symbols[0]]}  0.000  '
-                         f'{ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
-            for ie in fods[1]:
-                fp.write(f'{SYMBOL2NUMBER[elec_symbols[1]]}  0.000  '
-                         f'{ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
+            for s in range(len(fods)):
+                for ie in fods[s]:
+                    fp.write(f'{SYMBOL2NUMBER[elec_symbols[s]]}  0.000  '
+                             f'{ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
         # Field data (float) with scientific formatting
         # We have s[0]*s[1] chunks values with a length of s[2]
         for i in range(atoms.s[0] * atoms.s[1]):
             # Print every round of values, so we can add empty lines between them
             data_str = '%+1.6e  ' * atoms.s[2] % tuple(field[i * atoms.s[2]:(i + 1) * atoms.s[2]])
             # Print a maximum of 6 values per row
             # Max width for this formatting is 90, since 6*len('+1.00000e-000  ')=90
```

### Comparing `eminus-2.2.2/eminus/io/gth.py` & `eminus-2.3.0/eminus/io/gth.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
 def mock_gth():
     '''Create a mock dictionary with all-zeros, for atom species with no pseudopotential file.
 
     Returns:
         dict: GTH parameters (all zero).
     '''
-    psp = {}
-    psp['Zion'] = 0
-    psp['rloc'] = 0
-    psp['cloc'] = np.zeros(4)
-    psp['lmax'] = 0
-    psp['rp'] = np.zeros(4)
-    psp['Nproj_l'] = np.zeros(4, dtype=int)
-    psp['h'] = np.zeros((4, 3, 3))
-    return psp
+    return {
+        'Zion': 0,
+        'rloc': 0,
+        'cloc': np.zeros(4),
+        'lmax': 0,
+        'rp': np.zeros(4),
+        'Nproj_l': np.zeros(4, dtype=int),
+        'h': np.zeros((4, 3, 3))
+    }
```

### Comparing `eminus-2.2.2/eminus/io/json.py` & `eminus-2.3.0/eminus/io/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 '''JSON file handling.'''
 import base64
+import copy
 import json
 
 import numpy as np
 
 
 def read_json(filename):
     '''Load objects from a JSON file.
@@ -24,28 +25,29 @@
             data = base64.b64decode(dct['__ndarray__'])
             return np.frombuffer(data, dct['dtype']).reshape(dct['shape'])
 
         # Create a simple eminus objects and set all attributes afterwards
         # Explicitly call objects with verbosity since the logger is created at instantiation
         if isinstance(dct, dict) and 'atom' in dct:
             atoms = eminus.Atoms(dct['atom'], dct['X'], verbose=dct['_verbose'])
+            atoms._set_operators()
             for attr in dct:
                 if attr == 'log':
                     continue
-                setattr(atoms, attr, dct[attr])
+                setattr(atoms, attr, copy.deepcopy(dct[attr]))
             # The tuple type is not preserved when serializing, manually cast the only important one
             if isinstance(atoms.active, list):
                 atoms.active = tuple(atoms.active)
             return atoms
         if isinstance(dct, dict) and 'atoms' in dct:
             scf = eminus.SCF(dct['atoms'], verbose=dct['_verbose'])
             for attr in dct:
                 if attr == 'log':
                     continue
-                setattr(scf, attr, dct[attr])
+                setattr(scf, attr, copy.deepcopy(dct[attr]))
             return scf
         if isinstance(dct, dict) and 'Ekin' in dct:
             energies = eminus.energies.Energy()
             for attr in dct:
                 setattr(energies, attr, dct[attr])
             return energies
         return dct
@@ -71,22 +73,18 @@
         def default(self, obj):
             # ndarrays are not json serializable, encode them as base64 to save them
             if isinstance(obj, np.ndarray):
                 data = base64.b64encode(obj.copy(order='C')).decode('utf-8')
                 return {'__ndarray__': data, 'dtype': str(obj.dtype), 'shape': obj.shape}
 
             # If obj is a Atoms or SCF class dump them as a dictionary
-            if isinstance(obj, eminus.Atoms) or isinstance(obj, eminus.SCF):
+            if isinstance(obj, (eminus.Atoms, eminus.SCF, eminus.energies.Energy)):
                 # Only dumping the dict would result in a string, so do one dump and one load
                 data = json.dumps(obj.__dict__, cls=CustomEncoder)
                 return dict(json.loads(data))
-            # __slots__ classes have no __dict__, so use getattr
-            if isinstance(obj, eminus.energies.Energy):
-                data = json.dumps({slot: getattr(obj, slot) for slot in obj.__slots__})
-                return dict(json.loads(data))
             # The logger class is not serializable, just ignore it
             if isinstance(obj, eminus.logger.CustomLogger):
                 return None
             return json.JSONEncoder.default(self, obj)
 
     if not filename.endswith('.json'):
         filename += '.json'
```

### Comparing `eminus-2.2.2/eminus/io/pdb.py` & `eminus-2.3.0/eminus/io/pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,19 @@
         if 'He' in atoms.atom and atoms.Nspin == 2:
             log.warning('You need to modify "elec_symbols" to write helium with FODs in the spin-'
                         'polarized case.')
 
     atom = atoms.atom
     X = atoms.X
     if fods is not None:
-        atom += [elec_symbols[0]] * len(fods[0]) + [elec_symbols[1]] * len(fods[1])
-        if fods[0].shape[0] != 0:
+        if len(fods[0]) != 0:
+            atom = atom + [elec_symbols[0]] * len(fods[0])
             X = np.vstack((X, fods[0]))
-        if fods[1].shape[0] != 0:
+        if len(fods) > 1 and len(fods[1]) != 0:
+            atom = atom + [elec_symbols[1]] * len(fods[1])
             X = np.vstack((X, fods[1]))
 
     with open(filename, 'w') as fp:
         fp.write(create_pdb_str(atom, X, a=atoms.a))
     return
```

### Comparing `eminus-2.2.2/eminus/io/xyz.py` & `eminus-2.3.0/eminus/io/xyz.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,20 +83,19 @@
 
     with open(filename, 'w') as fp:
         # The first line contains the number of atoms.
         # If we add FOD coordinates, add them to the count.
         if fods is None:
             fp.write(f'{atoms.Natoms}\n')
         else:
-            fp.write(f'{atoms.Natoms + len(fods[0]) + len(fods[1])}\n')
+            fp.write(f'{atoms.Natoms + sum([len(i) for i in fods])}\n')
         # The second line can contains a comment.
         # Print information about the file and program, and the file creation time.
         fp.write(f'File generated with eminus {__version__} on {time.ctime()}\n')
         for ia in range(atoms.Natoms):
             fp.write(f'{atoms.atom[ia]:<2s}  {X[ia, 0]: .6f}  {X[ia, 1]: .6f}  {X[ia, 2]: .6f}\n')
         # Add FOD coordinates if desired. The atom symbol will default to X (no atom type).
         if fods is not None:
-            for ie in fods[0]:
-                fp.write(f'{elec_symbols[0]:<2s}  {ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
-            for ie in fods[1]:
-                fp.write(f'{elec_symbols[1]:<2s}  {ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
+            for s in range(len(fods)):
+                for ie in fods[s]:
+                    fp.write(f'{elec_symbols[s]:<2s}  {ie[0]: .6f}  {ie[1]: .6f}  {ie[2]: .6f}\n')
     return
```

### Comparing `eminus-2.2.2/eminus/localizer.py` & `eminus-2.3.0/eminus/localizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     '''Calculate transformation matrix to build Fermi orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
-        fods (ndarray): Fermi-orbital descriptors.
+        fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Transformation matrix R.
     '''
     # We only calculate occupied orbitals, so a zero matrix is enough
     R = np.empty((len(fods), len(fods)), dtype=complex)
 
@@ -55,15 +55,15 @@
     '''Calculate Fermi orbitals from Kohn-Sham orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
-        fods (ndarray): Fermi-orbital descriptors.
+        fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi orbitals.
     '''
     fo = np.zeros((atoms.Nspin, len(atoms.r), atoms.Nstate), dtype=complex)
 
     # Transform psi to real-space
@@ -104,15 +104,15 @@
     '''Calculate Fermi-Löwdin orbitals by orthonormalizing Fermi orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
-        fods (ndarray): Fermi-orbital descriptors.
+        fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi-Löwdin orbitals.
     '''
     fo = get_FO(atoms, psi, fods)
     flo = np.empty((atoms.Nspin, len(atoms.r), atoms.Nstate), dtype=complex)
 
@@ -207,17 +207,17 @@
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Matrices X, Y, and Z.
     '''
     dV = atoms.Omega / np.prod(atoms.s)
     # Similar to the expectation value of r, but accounting for periodicity
-    X = (psirs.conj().T * (np.exp(-1j * 2 * np.pi * atoms.r[:, 0] / atoms.a[0]))) @ psirs
-    Y = (psirs.conj().T * (np.exp(-1j * 2 * np.pi * atoms.r[:, 1] / atoms.a[1]))) @ psirs
-    Z = (psirs.conj().T * (np.exp(-1j * 2 * np.pi * atoms.r[:, 2] / atoms.a[2]))) @ psirs
+    X = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 0] / atoms.a[0])) @ psirs
+    Y = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 1] / atoms.a[1])) @ psirs
+    Z = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 2] / atoms.a[2])) @ psirs
     return X * dV, Y * dV, Z * dV
 
 
 def wannier_supercell_cost(X, Y, Z):
     '''Calculate the supercell Wannier cost.
 
     This is an equivalent criterion to the spread criterion, but not the same. This cost function
```

### Comparing `eminus-2.2.2/eminus/logger.py` & `eminus-2.3.0/eminus/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     @property
     def verbose(self):
         '''Verbosity level.'''
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
-        '''Verbosity setter to sync the logger with the property.'''
         self._verbose = get_level(level)
         self.setLevel(self._verbose)
 
 
 class CustomFormatter(logging.Formatter):
     '''Custom logger formatter.'''
     def format(self, record):
@@ -40,23 +39,39 @@
             self._style._fmt = '%(levelname)s: %(msg)s'
         else:
             # But not for infos and debug messages
             self._style._fmt = '%(msg)s'
         return super().format(record)
 
 
+# The following code is not guarded by a function because it has to be run once the logger is called
+# to set up the basic logger configuration
+
+# Create a base logger that can be used outside of classes
+logging.setLoggerClass(CustomLogger)
+log = logging.getLogger('eminus')
+
+# Basic logger setup
+formatter = CustomFormatter()
+handler = logging.StreamHandler(sys.stdout)
+handler.setFormatter(formatter)
+logging.root.addHandler(handler)
+
+
 def create_logger(object):
     '''Create a logger unique to an object.
 
     Args:
         object: Instance of a class.
     '''
     # Use ID of object to create a unique logger
     # Without this setting the verbosity in one instance would affect other instances
-    return logging.getLogger(str(id(object)))
+    local_log = logging.getLogger(str(id(object)))
+    local_log.verbose = log.verbose
+    return local_log
 
 
 def get_level(verbose):
     '''Validate logging levels.
 
     Args:
         verbose (int | str): Level of output (case insensitive).
@@ -86,22 +101,7 @@
     Returns:
         Callable: Decorator.
     '''
     def decorator(f):
         f.__name__ = newname
         return f
     return decorator
-
-
-# The following code is not guarded by a function because it has to be run once the logger is called
-# to set up the basic logger configuration
-
-# Create a base logger that can be used outside of classes
-logging.setLoggerClass(CustomLogger)
-log = logging.getLogger('eminus')
-log.verbose = 'WARNING'
-
-# Basic logger setup
-formatter = CustomFormatter()
-handler = logging.StreamHandler(sys.stdout)
-handler.setFormatter(formatter)
-logging.root.addHandler(handler)
```

### Comparing `eminus-2.2.2/eminus/minimizer.py` & `eminus-2.3.0/eminus/minimizer.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/operators.py` & `eminus-2.3.0/eminus/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 '''Basis set dependent operators for a plane wave basis.
 
 These operators act on discretized wave functions, i.e., the arrays W.
 
 These W are column vectors. This has been chosen to let theory and code coincide, e.g.,
-W^dagger W becomes W.conj().T @ W.
+W^dagger W becomes :code:`W.conj().T @ W`.
 
 The downside is that the i-th state will be accessed with W[:, i] instead of W[i].
 Choosing the i-th state makes the array 1d.
 
 These operators can act on six different options, namely
 
 1. the real-space
@@ -19,26 +19,20 @@
 6. the active reciprocal space (1d)
 
 The active space is the truncated reciprocal space by restricting it with a sphere given by ecut.
 
 Every spin dependence will be handled with handle_spin_gracefully by calling the operators for each
 spin individually.
 '''
-import os
-
 import numpy as np
 from scipy.fft import fftn, ifftn
 
+from . import config
 from .utils import handle_spin_gracefully
 
-try:
-    THREADS = int(os.environ['OMP_NUM_THREADS'])
-except KeyError:
-    THREADS = None
-
 
 # Spin handling is trivial for this operator
 def O(atoms, W):
     '''Overlap operator.
 
     This operator acts on the options 3, 4, 5, and 6.
     Reference: Comput. Phys. Commun. 128, 1.
@@ -85,15 +79,14 @@
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
     '''
-    out = np.empty_like(W, dtype=complex)
     # Ignore the division by zero for the first elements
     with np.errstate(divide='ignore', invalid='ignore'):
         if W.ndim == 1:
             # One could do some proper indexing with [1:] but indexing is slow
             out = W / (atoms.G2 * -atoms.Omega)
             out[0] = 0
         else:
@@ -122,33 +115,33 @@
 
     # If W is in the full space do nothing with W
     if len(W) == len(atoms.G2):
         Wfft = np.copy(W)
     else:
         # Fill with zeros if W is in the active space
         if W.ndim == 1:
-            Wfft = np.zeros(n, dtype=complex)
+            Wfft = np.zeros(n, dtype=W.dtype)
         else:
-            Wfft = np.zeros((n, atoms.Nstate), dtype=complex)
+            Wfft = np.zeros((n, atoms.Nstate), dtype=W.dtype)
         Wfft[atoms.active] = W
 
     # `workers` sets the number of threads the FFT operates on
     # `overwrite_x` allows writing in Wfft, but since we do not need Wfft later on, we can set this
     # for a little bit of extra performance
     # Normally, we would have to multiply by n in the end for the correct normalization, but we can
     # ignore this step when properly setting the `norm` option for a faster operation
     if W.ndim == 1:
         Wfft = Wfft.reshape(atoms.s)
-        Finv = ifftn(Wfft, workers=THREADS, overwrite_x=True, norm='forward').ravel()
+        Finv = ifftn(Wfft, workers=config.threads, overwrite_x=True, norm='forward').ravel()
     else:
         # Here we reshape the input like in the 1d case but add an extra dimension in the end,
         # holding the number of states
         Wfft = Wfft.reshape(np.append(atoms.s, atoms.Nstate))
         # Tell the function that the FFT only has to act on the first 3 axes
-        Finv = ifftn(Wfft, workers=THREADS, overwrite_x=True, norm='forward',
+        Finv = ifftn(Wfft, workers=config.threads, overwrite_x=True, norm='forward',
                      axes=(0, 1, 2)).reshape((n, atoms.Nstate))
     return Finv
 
 
 @handle_spin_gracefully
 def J(atoms, W, full=True):
     '''Forward transformation from real-space to reciprocal space.
@@ -163,26 +156,27 @@
     Keyword Args:
         full (bool): Wether to transform in the full or in the active space.
 
     Returns:
         ndarray: The operator applied on W.
     '''
     n = np.prod(atoms.s)
+    Wfft = np.copy(W)
 
     # `workers` sets the number of threads the FFT operates on
     # `overwrite_x` allows writing in Wfft, but since we do not need Wfft later on, we can set this
     # for a little bit of extra performance
     # Normally, we would have to divide by n in the end for the correct normalization, but we can
     # ignore this step when properly setting the `norm` option for a faster operation
     if W.ndim == 1:
-        Wfft = W.reshape(atoms.s)
-        F = fftn(Wfft, workers=THREADS, overwrite_x=True, norm='forward').ravel()
+        Wfft = Wfft.reshape(atoms.s)
+        F = fftn(Wfft, workers=config.threads, overwrite_x=True, norm='forward').ravel()
     else:
-        Wfft = W.reshape(np.append(atoms.s, atoms.Nstate))
-        F = fftn(Wfft, workers=THREADS, overwrite_x=True, norm='forward',
+        Wfft = Wfft.reshape(np.append(atoms.s, atoms.Nstate))
+        F = fftn(Wfft, workers=config.threads, overwrite_x=True, norm='forward',
                  axes=(0, 1, 2)).reshape((n, atoms.Nstate))
 
     # There is no way to know if J has to transform to the full or the active space
     # but normally it transforms to the full space
     if not full:
         return F[atoms.active]
     return F
@@ -262,12 +256,16 @@
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
         dr (ndarray): Real-space shift.
 
     Returns:
         ndarray: The operator applied on W.
     '''
     # Do the shift by multiplying a phase factor, given by the shift theorem
-    factor = np.exp(-1j * atoms.G[atoms.active] @ dr)
+    if len(W) == len(atoms.G2c):
+        G = atoms.G[atoms.active]
+    else:
+        G = atoms.G
+    factor = np.exp(-1j * G @ dr)
     # factor is a normal 1d row vector, reshape it so it can be applied to the column vector W
     if W.ndim == 2:
         factor = factor[:, None]
     return factor * W
```

### Comparing `eminus-2.2.2/eminus/orbitals.py` & `eminus-2.3.0/eminus/orbitals.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
-        fods (ndarray): Fermi-orbital descriptors.
+        fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi orbitals.
     '''
     # Lazy import extras
     from .extras.fods import get_fods, remove_core_fods
     atoms = scf.atoms
@@ -67,15 +67,15 @@
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
-        fods (ndarray): Fermi-orbital descriptors.
+        fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi-Löwdin orbitals.
     '''
     # Lazy import extras
     from .extras.fods import get_fods, remove_core_fods
     atoms = scf.atoms
```

### Comparing `eminus-2.2.2/eminus/pade/Ac-q11` & `eminus-2.3.0/eminus/pade/Ac-q11`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Ac-q29` & `eminus-2.3.0/eminus/pade/Ac-q29`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Am-q17` & `eminus-2.3.0/eminus/pade/Am-q17`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Am-q35` & `eminus-2.3.0/eminus/pade/Am-q35`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Bk-q19` & `eminus-2.3.0/eminus/pade/Bk-q19`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Bk-q37` & `eminus-2.3.0/eminus/pade/Bk-q37`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Cf-q20` & `eminus-2.3.0/eminus/pade/Cf-q20`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Cf-q38` & `eminus-2.3.0/eminus/pade/Cf-q38`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Cm-q18` & `eminus-2.3.0/eminus/pade/Cm-q18`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Cm-q36` & `eminus-2.3.0/eminus/pade/Cm-q36`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Es-q21` & `eminus-2.3.0/eminus/pade/Es-q21`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Es-q39` & `eminus-2.3.0/eminus/pade/Es-q39`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Fm-q22` & `eminus-2.3.0/eminus/pade/Fm-q22`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Fm-q40` & `eminus-2.3.0/eminus/pade/Fm-q40`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Lr-q25` & `eminus-2.3.0/eminus/pade/Lr-q25`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Lr-q43` & `eminus-2.3.0/eminus/pade/Lr-q43`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Md-q23` & `eminus-2.3.0/eminus/pade/Md-q23`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Md-q41` & `eminus-2.3.0/eminus/pade/Md-q41`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/No-q24` & `eminus-2.3.0/eminus/pade/No-q24`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/No-q42` & `eminus-2.3.0/eminus/pade/No-q42`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Np-q15` & `eminus-2.3.0/eminus/pade/Np-q15`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Np-q33` & `eminus-2.3.0/eminus/pade/Np-q33`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Pa-q13` & `eminus-2.3.0/eminus/pade/Pa-q13`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Pa-q31` & `eminus-2.3.0/eminus/pade/Pa-q31`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Pu-q16` & `eminus-2.3.0/eminus/pade/Pu-q16`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Pu-q34` & `eminus-2.3.0/eminus/pade/Pu-q34`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Th-q12` & `eminus-2.3.0/eminus/pade/Th-q12`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/Th-q30` & `eminus-2.3.0/eminus/pade/Th-q30`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/U-q14` & `eminus-2.3.0/eminus/pade/U-q14`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/U-q32` & `eminus-2.3.0/eminus/pade/U-q32`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/pade/__init__.py` & `eminus-2.3.0/eminus/pade/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     import urllib.request
     import zipfile
 
     psp_path = pathlib.Path(inspect.getfile(inspect.currentframe())).parent
     file = 'master.zip'
     # Download files
     url = f'https://github.com/cp2k/cp2k-data/archive/refs/heads/{file}'
-    urllib.request.urlretrieve(url, file)
+    urllib.request.urlretrieve(url, file)  # noqa: S310
     # Unpack files
     with zipfile.ZipFile(file, 'r') as fzip:
         fzip.extractall()
     # Move files
     pade_path = psp_path.joinpath('cp2k-data-master/potentials/Goedecker/cp2k/pade')
     for f in pade_path.iterdir():
         shutil.move(f, psp_path.joinpath(f.name))
```

### Comparing `eminus-2.2.2/eminus/potentials.py` & `eminus-2.3.0/eminus/potentials.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/scf.py` & `eminus-2.3.0/eminus/scf.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
             An integer value can be used as well, where larger numbers mean more output, starting
             from 0.
 
             Default: 'info'
     '''
     def __init__(self, atoms, xc='lda,vwn', pot='gth', guess='gaussian', etol=1e-7, cgform=1,
                  sic=False, min=None, verbose=None):
-        self.atoms = copy.copy(atoms)  # Atoms object
+        self.atoms = atoms             # Atoms object
         self.xc = xc.lower()           # Exchange-correlation functional
         self.pot = pot.lower()         # Used pseudopotential
-        self.guess = guess             # Initial wave functions guess
+        self.guess = guess.lower()     # Initial wave functions guess
         self.etol = etol               # Total energy convergence tolerance
         self.cgform = cgform           # Conjugate gradient form
         self.sic = sic                 # Calculate the sic energy
         self.min = min                 # Minimization methods
 
         # Set min here, better not use mutable data types in signatures
         if self.min is None:
@@ -108,26 +108,30 @@
         self.exc = None     # Exchange-correlation energy density
         self.vxc = None     # Exchange-correlation potential
         return self
 
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
         self.xc = parse_functionals(self.xc)
+        # Build the atoms object if necessary and make a copy
+        # This way the atoms object in scf is independent but we ensure that both atoms are build
         if not self.atoms.is_built:
-            self.atoms.build()
+            self.atoms = copy.copy(self.atoms.build())
+        else:
+            self.atoms = copy.copy(self.atoms)
         self._set_potential()
         self._init_W()
         self.print_precision = int(abs(np.log10(self.etol))) + 1
         return self
 
     def run(self, **kwargs):
         '''Run the self-consistent field (SCF) calculation.'''
         if self.log.level <= logging.DEBUG:
             info()
-        self.log.debug(f'--- System information ---\n{self.atoms}\n'
+        self.log.debug(f'\n--- System information ---\n{self.atoms}\n'
                        f'Spin handling: {"un" if self.atoms.Nspin == 1 else ""}polarized\n'
                        f'Number of states: {self.atoms.Nstate}\n'
                        f'Occupation per state:\n{self.atoms.f}\n'
                        f'\n--- Cell information ---\nSide lengths: {self.atoms.a} Bohr\n'
                        f'Sampling per axis: {self.atoms.s}\n'
                        f'Cut-off energy: {self.atoms.ecut} Hartree\n'
                        f'Compression: {len(self.atoms.G2) / len(self.atoms.G2c):.5f}\n'
@@ -191,30 +195,32 @@
 
     def recenter(self, center=None):
         '''Recenter the system inside the cell.
 
         Keyword Args:
             center (float | list | tuple | ndarray | None): Point to center the system around.
         '''
+        # Get the COM before centering the atoms
+        com = center_of_mass(self.atoms.X)
+
         # Run the recenter method of the atoms object
         self.atoms.recenter(center=center)
 
-        com = center_of_mass(self.atoms.X)
         if center is None:
             dr = com - self.atoms.a / 2
         else:
             center = np.asarray(center)
             dr = com - center
 
         # Shift orbitals and density
         self.W = self.atoms.T(self.W, dr=-dr)
         # Transform the density to the reciprocal space, shift, and transform back
         Jn = self.atoms.J(self.n)
         TJn = self.atoms.T(Jn, dr=-dr)
-        self.n = self.atoms.I(TJn)
+        self.n = np.real(self.atoms.I(TJn))
 
         # Recalculate the pseudopotential since it depends on the structure factor
         self._set_potential()
         # Clear intermediate results to make sure no one uses the unshifted results
         self.clear()
         return self
 
@@ -235,15 +241,15 @@
         '''Initialize wave functions.'''
         if self.guess in ('gauss', 'gaussian'):
             # Start with gaussians at atom positions
             self.W = guess_gaussian(self, complex=True)
         elif self.guess in ('rand', 'random'):
             # Start with randomized, complex basis functions with a random seed
             self.W = guess_random(self, complex=True)
-        elif self.guess in ('pseudo'):
+        elif self.guess in ('pseudo', 'pseudo_rand', 'pseudo_random'):
             # Start with pseudo-random numbers, mostly to compare with SimpleDFT
             self.W = guess_pseudo(self, seed=1234)
         else:
             self.log.error(f'No guess found for "{self.guess}"')
         return
 
     def __repr__(self):
@@ -257,37 +263,38 @@
     @property
     def verbose(self):
         '''Verbosity level.'''
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
-        '''Verbosity setter to sync the logger with the property.'''
         self._verbose = get_level(level)
-        self.log.setLevel(self._verbose)
+        self.log.verbose = self._verbose
         return
 
 
 class RSCF(SCF):
     '''SCF class for spin-paired systems.
 
     Inherited from :class:`eminus.scf.SCF`.
     '''
 
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
+        self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=1)
         super().initialize()
         return self
 
 
 class USCF(SCF):
     '''SCF class for spin-polarized systems.
 
     Inherited from :class:`eminus.scf.SCF`.
     '''
 
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
+        self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=2)
         super().initialize()
         return self
```

### Comparing `eminus-2.2.2/eminus/tools.py` & `eminus-2.3.0/eminus/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,42 @@
     '''
     if masses is None:
         masses = np.ones(len(coords))
 
     return np.sum(masses * coords.T, axis=1) / np.sum(masses)
 
 
+def orbital_center(object, psirs):
+    '''Calculate the orbital center of masses, e.g., from localized orbitals.
+
+    Args:
+        object: Atoms or SCF object.
+        psirs (ndarray): Set of orbitals in real-space.
+
+    Returns:
+        bool: Center of masses.
+    '''
+    try:
+        atoms = object.atoms
+    except AttributeError:
+        atoms = object
+
+    coms = [np.array([])] * 2
+    Ncom = psirs.shape[2]
+    for s in range(atoms.Nspin):
+        coms_spin = np.empty((Ncom, 3))
+
+        # Square orbitals
+        psi2 = np.real(psirs[s, :, :].conj() * psirs[s, :, :])
+        for i in range(Ncom):
+            coms_spin[i] = center_of_mass(atoms.r, psi2[:, i])
+        coms[s] = coms_spin
+    return coms
+
+
 def inertia_tensor(coords, masses=None):
     '''Calculate the inertia tensor for a set of coordinates and masses.
 
     Args:
         coords (ndarray): Array of real-space coordinates.
 
     Keyword Args:
```

### Comparing `eminus-2.2.2/eminus/units.py` & `eminus-2.3.0/eminus/units.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/utils.py` & `eminus-2.3.0/eminus/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,14 @@
 
 import numpy as np
 from scipy.linalg import norm
 
 from .logger import log
 
 
-def diagprod(a, B):
-    '''Efficiently calculate the expression Diag(a) * B.
-
-    Args:
-        a (ndarray): Single vector.
-        B (ndarray): Matrix.
-
-    Returns:
-        ndarray: The expressions result.
-    '''
-    # Reshape a to a column vector
-    a_col = a[:, None]
-    return a_col * B
-
-
 def dotprod(a, b):
     '''Efficiently calculate the expression a * b.
 
     Add an extra check to make sure the result is never zero since this function is used as a
     denominator in minimizers.
 
     Args:
@@ -36,18 +21,18 @@
     Returns:
         float: The expressions result
     '''
     eps = 1e-15  # 2.22e-16 is the range of float64 machine precision
     # The dot product of complex vectors looks like the expression below, but this is slow
     # res = np.real(np.trace(a.conj().T @ b))
     # We can calculate the trace faster by taking the sum of the Hadamard product
-    res = np.real(np.sum(a.conj() * b))
+    res = np.sum(a.conj() * b)
     if abs(res) < eps:
         return eps
-    return res
+    return np.real(res)
 
 
 def Ylm_real(l, m, G):
     '''Calculate real spherical harmonics from cartesian coordinates.
 
     Args:
         l (int): Angular momentum number.
@@ -74,15 +59,15 @@
 
     # Vectorized version of sin(theta)=sqrt(max(0, 1-cos_theta^2))
     sin_theta = np.sqrt(np.amax((np.zeros_like(cos_theta), 1 - cos_theta**2), axis=0))
 
     # phi=arctan(Gy/Gx)
     phi = np.arctan2(G[:, 1], G[:, 0])
     # If Gx=0: phi=pi/2*sign(Gy)
-    phi_idx = (eps > G[:, 0]) & (G[:, 0] > -eps)
+    phi_idx = np.abs(G[:, 0]) < eps
     phi[phi_idx] = np.pi / 2 * np.sign(G[phi_idx, 1])
 
     if l == 1:
         if m == -1:   # py
             return 0.5 * np.sqrt(3 / np.pi) * sin_theta * np.sin(phi)
         elif m == 0:  # pz
             return 0.5 * np.sqrt(3 / np.pi) * cos_theta
```

### Comparing `eminus-2.2.2/eminus/version.py` & `eminus-2.3.0/eminus/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,43 @@
 #!/usr/bin/env python3
 '''Package version number and version info function.'''
 import importlib
-import os
 import platform
 import sys
 
-__version__ = '2.2.2'
+__version__ = '2.3.0'
 logo = (' ___ _____ _ ___ _ _ ___ \n'
         '| -_|     | |   | | |_ -|\n'
         '|___|_|_|_|_|_|_|___|___|\n')
 
 
 def info():
     '''Print version numbers and availability of packages.'''
     dependencies = ('numpy', 'scipy')
-    extras = ('plotly', 'nglview', 'notebook', 'pyscf', 'pyflosic2')
-    dev = ('pylibxc', 'pytest', 'flake8', 'sphinx', 'furo')
+    extras = ('torch', 'pyscf', 'plotly', 'nglview')
+    dev = ('notebook', 'pylibxc', 'pytest', 'flake8', 'sphinx', 'furo')
 
     print(logo)
     print('--- Platform infos ---'
-          f'\nPlatform    : {platform.system()} {platform.machine()}'
-          f'\nRelease     : {platform.release()} {platform.version()}'
+          f'\nPlatform  : {platform.system()} {platform.machine()}'
+          f'\nRelease   : {platform.release()} {platform.version()}'
           '\n\n--- Version infos ---'
-          f'\npython      : {sys.version.split()[0]}'
-          f'\neminus      : {__version__}')
+          f'\npython    : {sys.version.split()[0]}'
+          f'\neminus    : {__version__}')
     for pkg in dependencies + extras + dev:
         try:
             module = importlib.import_module(pkg)
             try:
-                print(f'{pkg.ljust(12)}: {module.__version__}')
+                print(f'{pkg.ljust(10)}: {module.__version__}')
             except AttributeError:
                 # pylibxc does not use the standard version identifier
-                print(f'{pkg.ljust(12)}: {module.version.__version__}')
+                print(f'{pkg.ljust(10)}: {module.version.__version__}')
         except ModuleNotFoundError:
             if pkg in dependencies:
-                print(f'{pkg.ljust(12)}: Dependency not installed')
+                print(f'{pkg.ljust(10)}: Dependency not installed')
             elif pkg in extras:
-                print(f'{pkg.ljust(12)}: Extra not installed')
-
-    print('\n--- Performance infos ---')
-    try:
-        THREADS = int(os.environ['OMP_NUM_THREADS'])
-    except KeyError:
-        THREADS = 1
-        print('INFO: No OMP_NUM_THREADS environment variable was found.\n'
-              'To improve performance, add "export OMP_NUM_THREADS=THREADS" to your ".bashrc".\n'
-              'Make sure to replace "THREADS", typically with the number of cores your CPU has.')
-    finally:
-        print(f'FFT operations will run on {THREADS} thread{"s" if THREADS != 1 else ""}.')
+                print(f'{pkg.ljust(10)}: Extra not installed')
     return
 
 
 if __name__ == '__main__':
     info()
```

### Comparing `eminus-2.2.2/eminus/xc/lda_c_chachiyo.py` & `eminus-2.3.0/eminus/xc/lda_c_chachiyo.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
     '''
     a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
     b = 20.4562557
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
     rs2 = rs**2
 
     ec = a * np.log(1 + b / rs + b / rs2)
     if exc_only:
         return ec, None
 
     vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs2))
@@ -77,26 +77,26 @@
     '''
     a0 = -0.01554535   # (np.log(2) - 1) / (2 * np.pi**2)
     a1 = -0.007772675  # (np.log(2) - 1) / (4 * np.pi**2)
     b0 = 20.4562557
     b1 = 27.4203609
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
     rs2 = rs**2
 
     fzeta, dfdzeta = weight_function(zeta, exc_only=exc_only)
 
     ec0 = a0 * np.log(1 + b0 / rs + b0 / rs2)
     ec1 = a1 * np.log(1 + b1 / rs + b1 / rs2)
     ec = ec0 + (ec1 - ec0) * fzeta
     if exc_only:
         return ec, None
 
-    factor = (-1 / rs2 - 2 / rs**3)
+    factor = -1 / rs2 - 2 / rs**3
     dec0drs = a0 / (1 + b0 / rs + b0 / rs2) * b0 * factor
     dec1drs = a1 / (1 + b1 / rs + b1 / rs2) * b1 * factor
     prefactor = ec - rs / 3 * (dec0drs + (dec1drs - dec0drs) * fzeta)
 
     vcup = prefactor + (ec1 - ec0) * dfdzeta * (1 - zeta)
     vcdw = prefactor - (ec1 - ec0) * dfdzeta * (1 + zeta)
     return ec, np.array([vcup, vcdw])
```

### Comparing `eminus-2.2.2/eminus/xc/lda_c_chachiyo_mod.py` & `eminus-2.3.0/eminus/xc/lda_c_chachiyo_mod.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/xc/lda_c_pw.py` & `eminus-2.3.0/eminus/xc/lda_c_pw.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     a1 = 0.2137
     b1 = 7.5957
     b2 = 3.5876
     b3 = 1.6382
     b4 = 0.49294
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
     rs12 = np.sqrt(rs)
     rs32 = rs * rs12
     rs2 = rs**2
 
     om = 2 * a * (b1 * rs12 + b2 * rs + b3 * rs32 + b4 * rs2)
     olog = np.log(1 + 1 / om)
 
@@ -62,15 +62,15 @@
         fz0 (float): Functional parameter.
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
     '''
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
     zeta3 = zeta**3
     zeta4 = zeta3 * zeta
 
     def pw_fit(i):
         '''Calculate correlation energies by Perdew-Wang approximation interpolation.
 
         Args:
```

### Comparing `eminus-2.2.2/eminus/xc/lda_c_pw_mod.py` & `eminus-2.3.0/eminus/xc/lda_c_pw_mod.py`

 * *Files identical despite different names*

### Comparing `eminus-2.2.2/eminus/xc/lda_c_vwn.py` & `eminus-2.3.0/eminus/xc/lda_c_vwn.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     '''
     a = 0.0310907
     b = 3.72744
     c = 12.9352
     x0 = -0.10498
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
 
     q = np.sqrt(4 * c - b * b)
     f1 = 2 * b / q
     f2 = b * x0 / (x0 * x0 + b * x0 + c)
     f3 = 2 * (2 * x0 + b) / q
     rs12 = np.sqrt(rs)
     fx = rs + b * rs12 + c
@@ -61,15 +61,15 @@
     Keyword Args:
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
         tuple[ndarray, ndarray]: VWN correlation energy density and potential.
     '''
     pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
     zeta4 = zeta**4
 
     cfz = 2**(4 / 3) - 2
     iddfz0 = 9 / 8 * cfz
     trup = 1 + zeta
     trdw = 1 - zeta
     trup13 = trup**(1 / 3)
```

### Comparing `eminus-2.2.2/eminus/xc/lda_x.py` & `eminus-2.3.0/eminus/xc/lda_x.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange energy density and potential.
     '''
     pi34 = (3 / (4 * np.pi))**(1 / 3)
     f = -3 / 4 * (3 / (2 * np.pi))**(2 / 3)
-    rs = pi34 / n**(1 / 3)
+    rs = pi34 * n**(-1 / 3)
 
     ex = f / rs
     if exc_only:
         return ex, None
 
     vx = 4 / 3 * ex
     return ex, np.array([vx])
```

### Comparing `eminus-2.2.2/eminus/xc/utils.py` & `eminus-2.3.0/eminus/xc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,28 +108,28 @@
         xc = ALIAS[xc]
     except KeyError:
         pass
 
     # Parse functionals
     functionals = []
     for f in xc.split(','):
-        if 'libxc' in f or f in IMPLEMENTED.keys():
+        if 'libxc' in f or f in IMPLEMENTED:
             f_xc = f
         elif f == '':
             f_xc = 'mock_xc'
         else:
             try:
                 f_xc = XC_MAP[f]
             except KeyError:
                 log.exception(f'No functional found for "{f}"')
                 raise
         functionals.append(f_xc)
 
     # If only one or no functional has been parsed append with mock functionals
-    for i in range(2 - len(functionals)):
+    for _ in range(2 - len(functionals)):
         functionals.append('mock_xc')
     return functionals
 
 
 def get_zeta(n_spin):
     '''Calculate the relative spin polarization.
 
@@ -198,10 +198,11 @@
     'chachiyo': 'lda_c_chachiyo',
     # lda_c_chachiyo_mod
     '307': 'lda_c_chachiyo_mod',
     'chachiyo_mod': 'lda_c_chachiyo_mod'
 }
 
 ALIAS = {
-    'spw92': 'slater,pw_mod',
-    'svwn': 'slater,vwn'
+    'spw92': 'slater,pw92_mod',
+    'svwn': 'slater,vwn5',
+    'svwn5': 'slater,vwn5'
 }
```

### Comparing `eminus-2.2.2/eminus.egg-info/SOURCES.txt` & `eminus-2.3.0/eminus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 eminus/README.md
 eminus/__init__.py
 eminus/atoms.py
+eminus/config.py
 eminus/data.py
 eminus/dft.py
 eminus/domains.py
 eminus/energies.py
 eminus/gth.py
 eminus/localizer.py
 eminus/logger.py
@@ -29,14 +30,15 @@
 eminus.egg-info/not-zip-safe
 eminus.egg-info/requires.txt
 eminus.egg-info/top_level.txt
 eminus/extras/README.md
 eminus/extras/__init__.py
 eminus/extras/fods.py
 eminus/extras/libxc.py
+eminus/extras/torch.py
 eminus/extras/viewer.py
 eminus/io/README.md
 eminus/io/__init__.py
 eminus/io/cube.py
 eminus/io/gth.py
 eminus/io/json.py
 eminus/io/pdb.py
```

### Comparing `eminus-2.2.2/setup.py` & `eminus-2.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 #!/usr/bin/env python3
 '''Setup file to make eminus installable.
 
 For a full list of options see the documentation:
 https://setuptools.pypa.io/en/latest/references/keywords.html
 '''
+import re
+
 from setuptools import find_packages, setup
 
 with open('eminus/version.py', 'r') as fh:
-    version = {}
-    exec(fh.read(), version)
+    version = re.search(r"__version__ = '(.*?)'", fh.read()).group(1)
 
 with open('README.md', 'r') as readme, open('CHANGELOG.md', 'r') as changelog:
     long_description = readme.read() + '\n\n' + changelog.read().split('\n----\n')[0]
 
 extras = {
-    'fods': [
-        'pyflosic2>=2.0.0rc0'  # PyCOM FOD guessing method
-    ],
     'libxc': [
         'pyscf>=1.5.1'  # Libxc interface via PySCF
     ],
+    'torch': [
+        'torch>=1.8'  # Faster FFT operators using Torch
+    ],
     'viewer': [
         'nglview>=2.6.5',  # Molecule and isosurface viewer
         'plotly>=4'        # Grid visualization
     ]
 }
+extras['fods'] = extras['libxc']  # PyCOM FOD guessing method uses PySCF
 extras['all'] = [dep for values in extras.values() for dep in values]
 extras['dev'] = [
+    'coverage>=3.6',             # Generate coverage reports
     'flake8>=3.7',               # Style guide checker
     'flake8-docstrings>=1.4',    # Docstring style guide extension
     'flake8-import-order>=0.9',  # Import statement style guide extension
     'furo>=2022.02.14.1',        # Documentation theme
     'notebook',                  # Run and convert notebooks to HTML
     'pytest>=2.8',               # Test utilities
+    'pytest-cov>=0.6',           # Collect test coverage data
     'sphinx>=5'                  # Documentation builder
 ]
 
-
 setup(
     name='eminus',
-    version=version['__version__'],
+    version=version,
     description='A plane wave density functional theory code.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Wanja Timm Schulze',
     author_email='wangenau@protonmail.com',
     url='https://github.com/wangenau/eminus',
     packages=find_packages(),
@@ -73,15 +76,14 @@
         'Topic :: Software Development'
     ],
     license='APACHE2.0',
     install_requires=[
         'numpy>=1.17',
         'scipy>=1.6'
     ],
-    keywords=['ESP'],
     zip_safe=False,
     extras_require=extras,
     python_requires='>=3.7',
     project_urls={
         'Bug Tracker': 'https://gitlab.com/wangenau/eminus/-/issues',
         'Changelog': 'https://wangenau.gitlab.io/eminus/changelog.html',
         'Documentation': 'https://wangenau.gitlab.io/eminus',
```

