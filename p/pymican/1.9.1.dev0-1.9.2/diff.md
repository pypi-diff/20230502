# Comparing `tmp/pymican-1.9.1.dev0.tar.gz` & `tmp/pymican-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymican-1.9.1.dev0.tar", last modified: Mon Jun 27 06:09:21 2022, max compression
+gzip compressed data, was "pymican-1.9.2.tar", last modified: Wed Mar 29 19:01:58 2023, max compression
```

## Comparing `pymican-1.9.1.dev0.tar` & `pymican-1.9.2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.062940 pymican-1.9.1.dev0/
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.024724 pymican-1.9.1.dev0/.github/
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.028839 pymican-1.9.1.dev0/.github/workflows/
--rw-r--r--   0 sminami    (501) staff       (20)      704 2022-06-27 01:55:49.000000 pymican-1.9.1.dev0/.github/workflows/build_and_test.yml
--rw-r--r--   0 sminami    (501) staff       (20)       91 2022-06-26 22:18:46.000000 pymican-1.9.1.dev0/.gitignore
--rw-r--r--   0 sminami    (501) staff       (20)     1072 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/LICENSE
--rw-r--r--   0 sminami    (501) staff       (20)       80 2022-06-27 02:54:03.000000 pymican-1.9.1.dev0/MANIFEST.in
--rw-r--r--   0 sminami    (501) staff       (20)      300 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/Makefile
--rw-r--r--   0 sminami    (501) staff       (20)     4226 2022-06-27 06:09:21.062650 pymican-1.9.1.dev0/PKG-INFO
--rw-r--r--   0 sminami    (501) staff       (20)     3933 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/README.md
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.030644 pymican-1.9.1.dev0/pymican/
--rw-r--r--   0 sminami    (501) staff       (20)       45 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/pymican/__init__.py
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.036463 pymican-1.9.1.dev0/pymican/bin/
--rwxr-xr-x   0 sminami    (501) staff       (20)  1302384 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/pymican/bin/mican_x86_64_linux
--rw-r--r--   0 sminami    (501) staff       (20)     5983 2022-06-26 23:10:36.000000 pymican-1.9.1.dev0/pymican/main.py
--rw-r--r--   0 sminami    (501) staff       (20)     2158 2022-06-26 21:48:48.000000 pymican-1.9.1.dev0/pymican/parse_result.py
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.036151 pymican-1.9.1.dev0/pymican.egg-info/
--rw-r--r--   0 sminami    (501) staff       (20)     4226 2022-06-27 06:09:20.000000 pymican-1.9.1.dev0/pymican.egg-info/PKG-INFO
--rw-r--r--   0 sminami    (501) staff       (20)     1006 2022-06-27 06:09:20.000000 pymican-1.9.1.dev0/pymican.egg-info/SOURCES.txt
--rw-r--r--   0 sminami    (501) staff       (20)        1 2022-06-27 06:09:20.000000 pymican-1.9.1.dev0/pymican.egg-info/dependency_links.txt
--rw-r--r--   0 sminami    (501) staff       (20)       13 2022-06-27 06:09:20.000000 pymican-1.9.1.dev0/pymican.egg-info/requires.txt
--rw-r--r--   0 sminami    (501) staff       (20)        9 2022-06-27 06:09:20.000000 pymican-1.9.1.dev0/pymican.egg-info/top_level.txt
--rw-r--r--   0 sminami    (501) staff       (20)       28 2022-06-26 22:18:46.000000 pymican-1.9.1.dev0/requirements.txt
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.041112 pymican-1.9.1.dev0/scripts/
--rwxr-xr-x   0 sminami    (501) staff       (20)      131 2022-06-26 22:18:46.000000 pymican-1.9.1.dev0/scripts/mican
--rw-r--r--   0 sminami    (501) staff       (20)       38 2022-06-27 06:09:21.063044 pymican-1.9.1.dev0/setup.cfg
--rw-r--r--   0 sminami    (501) staff       (20)     1105 2022-06-27 06:09:09.000000 pymican-1.9.1.dev0/setup.py
-drwxr-xr-x   0 sminami    (501) staff       (20)        0 2022-06-27 06:09:21.062132 pymican-1.9.1.dev0/src/
--rw-r--r--   0 sminami    (501) staff       (20)     1873 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/C3score.c
--rw-r--r--   0 sminami    (501) staff       (20)     1909 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/Daliscore.c
--rw-r--r--   0 sminami    (501) staff       (20)      254 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/Makefile
--rw-r--r--   0 sminami    (501) staff       (20)     5073 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/SPscore.c
--rw-r--r--   0 sminami    (501) staff       (20)     1715 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/TMscore.c
--rw-r--r--   0 sminami    (501) staff       (20)     3584 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/TMscore_mod.c
--rw-r--r--   0 sminami    (501) staff       (20)     5607 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/assign_sse.c
--rw-r--r--   0 sminami    (501) staff       (20)     8092 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/bstft.c
--rw-r--r--   0 sminami    (501) staff       (20)     6440 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/ca_alignment.c
--rw-r--r--   0 sminami    (501) staff       (20)      563 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/calc_maxdist.c
--rw-r--r--   0 sminami    (501) staff       (20)      531 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/chain_break_check.c
--rw-r--r--   0 sminami    (501) staff       (20)     2775 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/check.c
--rw-r--r--   0 sminami    (501) staff       (20)     3287 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/clustering_align.c
--rw-r--r--   0 sminami    (501) staff       (20)      884 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/coord_definition.c
--rw-r--r--   0 sminami    (501) staff       (20)      629 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/distmat.c
--rw-r--r--   0 sminami    (501) staff       (20)     2817 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/extend_termini.c
--rw-r--r--   0 sminami    (501) staff       (20)    11405 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/fsscanf.c
--rw-r--r--   0 sminami    (501) staff       (20)     2155 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/fsscanf.h
--rw-r--r--   0 sminami    (501) staff       (20)     6015 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/getopt.c
--rw-r--r--   0 sminami    (501) staff       (20)    11676 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/global_alignment.c
--rw-r--r--   0 sminami    (501) staff       (20)      885 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/hres2trans.c
--rw-r--r--   0 sminami    (501) staff       (20)     5938 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/main.c
--rw-r--r--   0 sminami    (501) staff       (20)    20698 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/main_align.c
--rw-r--r--   0 sminami    (501) staff       (20)     6064 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/make_hash_table.c
--rw-r--r--   0 sminami    (501) staff       (20)      692 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/make_pdbdat.c
--rw-r--r--   0 sminami    (501) staff       (20)    11034 2022-06-27 02:10:22.000000 pymican-1.9.1.dev0/src/mican.h
--rw-r--r--   0 sminami    (501) staff       (20)     7120 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/output.c
--rw-r--r--   0 sminami    (501) staff       (20)     8268 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/print_data.c
--rw-r--r--   0 sminami    (501) staff       (20)     4270 2022-06-27 02:13:03.000000 pymican-1.9.1.dev0/src/print_pdb.c
--rw-r--r--   0 sminami    (501) staff       (20)      335 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/print_progress.c
--rw-r--r--   0 sminami    (501) staff       (20)     9747 2022-06-27 02:10:13.000000 pymican-1.9.1.dev0/src/read_pdb.c
--rw-r--r--   0 sminami    (501) staff       (20)     1320 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/resname2reschar.c
--rw-r--r--   0 sminami    (501) staff       (20)     1913 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/rmsd.c
--rw-r--r--   0 sminami    (501) staff       (20)     6102 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/score.c
--rw-r--r--   0 sminami    (501) staff       (20)     6268 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/search_hash.c
--rw-r--r--   0 sminami    (501) staff       (20)     1162 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/superposition.c
--rw-r--r--   0 sminami    (501) staff       (20)     9704 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/svd.c
--rw-r--r--   0 sminami    (501) staff       (20)      845 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/utils.c
--rw-r--r--   0 sminami    (501) staff       (20)     3071 2022-06-26 21:48:49.000000 pymican-1.9.1.dev0/src/xyz2vec.c
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.215135 pymican-1.9.2/
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.203800 pymican-1.9.2/.github/
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.205663 pymican-1.9.2/.github/workflows/
+-rw-r--r--   0 sminami    (503) staff       (20)      704 2023-03-29 18:46:06.000000 pymican-1.9.2/.github/workflows/build_and_test.yml
+-rw-r--r--   0 sminami    (503) staff       (20)       91 2023-03-29 18:46:06.000000 pymican-1.9.2/.gitignore
+-rw-r--r--   0 sminami    (503) staff       (20)     1072 2023-03-29 18:46:06.000000 pymican-1.9.2/LICENSE
+-rw-r--r--   0 sminami    (503) staff       (20)       80 2023-03-29 18:46:06.000000 pymican-1.9.2/MANIFEST.in
+-rw-r--r--   0 sminami    (503) staff       (20)      300 2023-03-29 18:46:06.000000 pymican-1.9.2/Makefile
+-rw-r--r--   0 sminami    (503) staff       (20)      303 2023-03-29 18:46:06.000000 pymican-1.9.2/Makefile_gcc11
+-rw-r--r--   0 sminami    (503) staff       (20)     4184 2023-03-29 19:01:58.215016 pymican-1.9.2/PKG-INFO
+-rw-r--r--   0 sminami    (503) staff       (20)     3933 2023-03-29 18:46:06.000000 pymican-1.9.2/README.md
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.206180 pymican-1.9.2/pymican/
+-rw-r--r--   0 sminami    (503) staff       (20)       45 2023-03-29 18:46:06.000000 pymican-1.9.2/pymican/__init__.py
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.206932 pymican-1.9.2/pymican/bin/
+-rwxr-xr-x   0 sminami    (503) staff       (20)  1302384 2023-03-29 18:46:06.000000 pymican-1.9.2/pymican/bin/mican_x86_64_linux
+-rw-r--r--   0 sminami    (503) staff       (20)     5980 2023-03-29 18:46:51.000000 pymican-1.9.2/pymican/main.py
+-rw-r--r--   0 sminami    (503) staff       (20)     2152 2023-03-29 18:47:11.000000 pymican-1.9.2/pymican/parse_result.py
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.206819 pymican-1.9.2/pymican.egg-info/
+-rw-r--r--   0 sminami    (503) staff       (20)     4184 2023-03-29 19:01:58.000000 pymican-1.9.2/pymican.egg-info/PKG-INFO
+-rw-r--r--   0 sminami    (503) staff       (20)     1032 2023-03-29 19:01:58.000000 pymican-1.9.2/pymican.egg-info/SOURCES.txt
+-rw-r--r--   0 sminami    (503) staff       (20)        1 2023-03-29 19:01:58.000000 pymican-1.9.2/pymican.egg-info/dependency_links.txt
+-rw-r--r--   0 sminami    (503) staff       (20)       13 2023-03-29 19:01:58.000000 pymican-1.9.2/pymican.egg-info/requires.txt
+-rw-r--r--   0 sminami    (503) staff       (20)        9 2023-03-29 19:01:58.000000 pymican-1.9.2/pymican.egg-info/top_level.txt
+-rw-r--r--   0 sminami    (503) staff       (20)       28 2023-03-29 18:46:06.000000 pymican-1.9.2/requirements.txt
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.208456 pymican-1.9.2/scripts/
+-rwxr-xr-x   0 sminami    (503) staff       (20)      131 2023-03-29 18:46:06.000000 pymican-1.9.2/scripts/mican
+-rw-r--r--   0 sminami    (503) staff       (20)       38 2023-03-29 19:01:58.215170 pymican-1.9.2/setup.cfg
+-rw-r--r--   0 sminami    (503) staff       (20)     1105 2023-03-29 18:46:06.000000 pymican-1.9.2/setup.py
+drwxr-xr-x   0 sminami    (503) staff       (20)        0 2023-03-29 19:01:58.214836 pymican-1.9.2/src/
+-rw-r--r--   0 sminami    (503) staff       (20)     1873 2023-03-29 18:46:06.000000 pymican-1.9.2/src/C3score.c
+-rw-r--r--   0 sminami    (503) staff       (20)     1926 2023-03-29 18:46:06.000000 pymican-1.9.2/src/Daliscore.c
+-rw-r--r--   0 sminami    (503) staff       (20)      254 2023-03-29 18:46:06.000000 pymican-1.9.2/src/Makefile
+-rw-r--r--   0 sminami    (503) staff       (20)     5073 2023-03-29 18:46:06.000000 pymican-1.9.2/src/SPscore.c
+-rw-r--r--   0 sminami    (503) staff       (20)     1733 2023-03-29 18:46:06.000000 pymican-1.9.2/src/TMscore.c
+-rw-r--r--   0 sminami    (503) staff       (20)     3602 2023-03-29 18:46:06.000000 pymican-1.9.2/src/TMscore_mod.c
+-rw-r--r--   0 sminami    (503) staff       (20)     5607 2023-03-29 18:46:06.000000 pymican-1.9.2/src/assign_sse.c
+-rw-r--r--   0 sminami    (503) staff       (20)     8092 2023-03-29 18:46:06.000000 pymican-1.9.2/src/bstft.c
+-rw-r--r--   0 sminami    (503) staff       (20)     6458 2023-03-29 18:46:06.000000 pymican-1.9.2/src/ca_alignment.c
+-rw-r--r--   0 sminami    (503) staff       (20)      563 2023-03-29 18:46:06.000000 pymican-1.9.2/src/calc_maxdist.c
+-rw-r--r--   0 sminami    (503) staff       (20)      531 2023-03-29 18:46:06.000000 pymican-1.9.2/src/chain_break_check.c
+-rw-r--r--   0 sminami    (503) staff       (20)     2793 2023-03-29 18:46:06.000000 pymican-1.9.2/src/check.c
+-rw-r--r--   0 sminami    (503) staff       (20)     3287 2023-03-29 18:46:06.000000 pymican-1.9.2/src/clustering_align.c
+-rw-r--r--   0 sminami    (503) staff       (20)      884 2023-03-29 18:46:06.000000 pymican-1.9.2/src/coord_definition.c
+-rw-r--r--   0 sminami    (503) staff       (20)      629 2023-03-29 18:46:06.000000 pymican-1.9.2/src/distmat.c
+-rw-r--r--   0 sminami    (503) staff       (20)     2835 2023-03-29 18:46:06.000000 pymican-1.9.2/src/extend_termini.c
+-rw-r--r--   0 sminami    (503) staff       (20)    11405 2023-03-29 18:46:06.000000 pymican-1.9.2/src/fsscanf.c
+-rw-r--r--   0 sminami    (503) staff       (20)     2155 2023-03-29 18:46:06.000000 pymican-1.9.2/src/fsscanf.h
+-rw-r--r--   0 sminami    (503) staff       (20)     6033 2023-03-29 18:46:06.000000 pymican-1.9.2/src/getopt.c
+-rw-r--r--   0 sminami    (503) staff       (20)    11694 2023-03-29 18:46:06.000000 pymican-1.9.2/src/global_alignment.c
+-rw-r--r--   0 sminami    (503) staff       (20)      885 2023-03-29 18:46:06.000000 pymican-1.9.2/src/hres2trans.c
+-rw-r--r--   0 sminami    (503) staff       (20)     6046 2023-03-29 18:46:06.000000 pymican-1.9.2/src/main.c
+-rw-r--r--   0 sminami    (503) staff       (20)       90 2023-03-29 18:46:06.000000 pymican-1.9.2/src/main.h
+-rw-r--r--   0 sminami    (503) staff       (20)    20732 2023-03-29 18:46:06.000000 pymican-1.9.2/src/main_align.c
+-rw-r--r--   0 sminami    (503) staff       (20)     6082 2023-03-29 18:46:06.000000 pymican-1.9.2/src/make_hash_table.c
+-rw-r--r--   0 sminami    (503) staff       (20)      692 2023-03-29 18:46:06.000000 pymican-1.9.2/src/make_pdbdat.c
+-rw-r--r--   0 sminami    (503) staff       (20)    11038 2023-03-29 18:46:06.000000 pymican-1.9.2/src/mican.h
+-rw-r--r--   0 sminami    (503) staff       (20)     7138 2023-03-29 18:46:06.000000 pymican-1.9.2/src/output.c
+-rw-r--r--   0 sminami    (503) staff       (20)     8286 2023-03-29 18:46:06.000000 pymican-1.9.2/src/print_data.c
+-rw-r--r--   0 sminami    (503) staff       (20)     4270 2023-03-29 18:46:06.000000 pymican-1.9.2/src/print_pdb.c
+-rw-r--r--   0 sminami    (503) staff       (20)      335 2023-03-29 18:46:06.000000 pymican-1.9.2/src/print_progress.c
+-rw-r--r--   0 sminami    (503) staff       (20)     9747 2023-03-29 18:46:06.000000 pymican-1.9.2/src/read_pdb.c
+-rw-r--r--   0 sminami    (503) staff       (20)     1320 2023-03-29 18:46:06.000000 pymican-1.9.2/src/resname2reschar.c
+-rw-r--r--   0 sminami    (503) staff       (20)     1913 2023-03-29 18:46:06.000000 pymican-1.9.2/src/rmsd.c
+-rw-r--r--   0 sminami    (503) staff       (20)     6120 2023-03-29 18:46:06.000000 pymican-1.9.2/src/score.c
+-rw-r--r--   0 sminami    (503) staff       (20)     6286 2023-03-29 18:46:06.000000 pymican-1.9.2/src/search_hash.c
+-rw-r--r--   0 sminami    (503) staff       (20)     1162 2023-03-29 18:46:06.000000 pymican-1.9.2/src/superposition.c
+-rw-r--r--   0 sminami    (503) staff       (20)     9704 2023-03-29 18:46:06.000000 pymican-1.9.2/src/svd.c
+-rw-r--r--   0 sminami    (503) staff       (20)      845 2023-03-29 18:46:06.000000 pymican-1.9.2/src/utils.c
+-rw-r--r--   0 sminami    (503) staff       (20)     3071 2023-03-29 18:46:06.000000 pymican-1.9.2/src/xyz2vec.c
```

### Comparing `pymican-1.9.1.dev0/.github/workflows/build_and_test.yml` & `pymican-1.9.2/.github/workflows/build_and_test.yml`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/LICENSE` & `pymican-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/PKG-INFO` & `pymican-1.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pymican
-Version: 1.9.1.dev0
+Version: 1.9.2
 Summary: Non-sequential protein structure alignment algorithm
 Home-page: https://github.com/ShintaroMinami/mican
 Author: Shintaro Minami
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MICAN
 Protein structure alignment program that can handle
 - M: multiple-chain complexs
 - I: inverse direction of SSEs
@@ -154,9 +152,7 @@
    % mican protein1 protein2 -r
 
  To visualize superposition:
    % mican protein1 protein2 -o sup.pdb
    % rasmol -script sup.pdb
 ```
 
-
-
```

### Comparing `pymican-1.9.1.dev0/README.md` & `pymican-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/pymican/bin/mican_x86_64_linux` & `pymican-1.9.2/pymican/bin/mican_x86_64_linux`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/pymican/main.py` & `pymican-1.9.2/pymican/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         
         Returns
         -------
         np.array
             Translated xyz coordinates
         """
         # list to np.array
-        xyz = np.array(xyz, dtype=np.float) if type(xyz) == list else xyz
+        xyz = np.array(xyz, dtype=float) if type(xyz) == list else xyz
         # save original shape
         original_shape = xyz.shape
         # add dimention 1 if ndim==1
         xyz = xyz[np.newaxis,:] if xyz.ndim == 1 else xyz
         # translate
         xyz_translated = np.dot(xyz,self.translation_rot.T) + self.translation_vec
         # return
```

### Comparing `pymican-1.9.1.dev0/pymican/parse_result.py` & `pymican-1.9.2/pymican/parse_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import numpy as np
 import pandas as pd
 
 def output2dict(mican_output:str):
     dict = {}
-    rot = np.zeros((3,3), dtype=np.float)
-    vec = np.zeros((3), dtype=np.float)
+    rot = np.zeros((3,3), dtype=float)
+    vec = np.zeros((3), dtype=float)
     align = []
     for l in mican_output.split('\n'):
         if l.startswith(' TM-score=') & l.endswith('Protein1)'):
             dict['TMscore1'], dict['coverage1'] = map(float, re.findall('=(.....)', l))
         if l.startswith(' TM-score=') & l.endswith('Protein2)'):
             dict['TMscore2'], dict['coverage2'] = map(float, re.findall('=(.....)', l))
         if l.startswith('    1    '):
```

### Comparing `pymican-1.9.1.dev0/pymican.egg-info/PKG-INFO` & `pymican-1.9.2/pymican.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pymican
-Version: 1.9.1.dev0
+Version: 1.9.2
 Summary: Non-sequential protein structure alignment algorithm
 Home-page: https://github.com/ShintaroMinami/mican
 Author: Shintaro Minami
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MICAN
 Protein structure alignment program that can handle
 - M: multiple-chain complexs
 - I: inverse direction of SSEs
@@ -154,9 +152,7 @@
    % mican protein1 protein2 -r
 
  To visualize superposition:
    % mican protein1 protein2 -o sup.pdb
    % rasmol -script sup.pdb
 ```
 
-
-
```

### Comparing `pymican-1.9.1.dev0/pymican.egg-info/SOURCES.txt` & `pymican-1.9.2/pymican.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 MANIFEST.in
 Makefile
+Makefile_gcc11
 README.md
 requirements.txt
 setup.py
 .github/workflows/build_and_test.yml
 pymican/__init__.py
 pymican/main.py
 pymican/parse_result.py
@@ -34,14 +35,15 @@
 src/extend_termini.c
 src/fsscanf.c
 src/fsscanf.h
 src/getopt.c
 src/global_alignment.c
 src/hres2trans.c
 src/main.c
+src/main.h
 src/main_align.c
 src/make_hash_table.c
 src/make_pdbdat.c
 src/mican.h
 src/output.c
 src/print_data.c
 src/print_pdb.c
```

### Comparing `pymican-1.9.1.dev0/setup.py` & `pymican-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/C3score.c` & `pymican-1.9.2/src/C3score.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/Daliscore.c` & `pymican-1.9.2/src/Daliscore.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #include "mican.h"
-
+#include "main.h"
 
 float Daliscore(int naa1, float **distmat1, float **distmat2, ALIGN *align) {
 
   int iaa, jaa;
   int iaa1, iaa2, jaa1, jaa2;
   int ialn, jaln, naln;
   int *ialn2iaa, *ialn2jaa;
```

### Comparing `pymican-1.9.1.dev0/src/SPscore.c` & `pymican-1.9.2/src/SPscore.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/TMscore.c` & `pymican-1.9.2/src/TMscore.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 float TMscore(int naa0, int naa1, RESDAT *resdat1, RESDAT *resdat2, ALIGN align) {
   int iaa, jaa;
   int ialn, naln;
   int ico;
   int i;
   float **co1;
```

### Comparing `pymican-1.9.1.dev0/src/TMscore_mod.c` & `pymican-1.9.2/src/TMscore_mod.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 float TMscore_mod(int naa0, int naa1, int naa2, RESDAT *resdat1, RESDAT *resdat2, ALIGN align,
                   int angle_switch, int local_switch) {
   int iaa, jaa;
   int ico;
   int i;
   float **co1;
```

### Comparing `pymican-1.9.1.dev0/src/assign_sse.c` & `pymican-1.9.2/src/assign_sse.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/bstft.c` & `pymican-1.9.2/src/bstft.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/ca_alignment.c` & `pymican-1.9.2/src/ca_alignment.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 int ca_alignment(int naa_q, int naa_t, RESDAT *resdat_q, RESDAT *resdat_t,
                  ALIGN align, float ***mat, float **score, float **score_r) {
   int i;
   int icoord;
   int iaa, jaa;
   float dist_2, dmax_2;
```

### Comparing `pymican-1.9.1.dev0/src/calc_maxdist.c` & `pymican-1.9.2/src/calc_maxdist.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/chain_break_check.c` & `pymican-1.9.2/src/chain_break_check.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/check.c` & `pymican-1.9.2/src/check.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 /** function for comparison of hash results **/
 PRIVATE int compare(const void *a, const void *b);
 PRIVATE int check_redundancy(ALIGN align1, ALIGN align2);
 
 void check_GHresult(int maxalign, HASH_RESULT *hres, ALIGN *align,
                     SSEDAT *ssedat_q, SSEDAT *ssedat_t) {
```

### Comparing `pymican-1.9.1.dev0/src/clustering_align.c` & `pymican-1.9.2/src/clustering_align.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/coord_definition.c` & `pymican-1.9.2/src/coord_definition.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/distmat.c` & `pymican-1.9.2/src/distmat.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/extend_termini.c` & `pymican-1.9.2/src/extend_termini.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 typedef struct {
   int iaa;
   int jaa;
   int segmode;
   float dist2;
 } TERMINI;
```

### Comparing `pymican-1.9.1.dev0/src/fsscanf.c` & `pymican-1.9.2/src/fsscanf.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/fsscanf.h` & `pymican-1.9.2/src/fsscanf.h`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/getopt.c` & `pymican-1.9.2/src/getopt.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 PRIVATE void read_opt(int argc, char *argv[], int iarg, int ich);
 PRIVATE int check_argument(int argc, char *argv[], int iarg, int ich);
 
 int getopt(int argc, char *argv[]) {
   int iarg;
   int ich;
```

### Comparing `pymican-1.9.1.dev0/src/global_alignment.c` & `pymican-1.9.2/src/global_alignment.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 #define USED -1000.0
 #define ALIGNED -2000.0
 
 PRIVATE void check_close(int naa1, int naa2, int *ncons, int **id_iaa,
                          float **mat, int mode);
 PRIVATE void takeover_mat(float **mat1, float **mat2, int ncons, int **id_iaa);
```

### Comparing `pymican-1.9.1.dev0/src/hres2trans.c` & `pymican-1.9.2/src/hres2trans.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/main.c` & `pymican-1.9.2/src/main.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 #include "mican.h"
+#include "main.h"
+
+/** Define global variables**/
+
+INPUT_DATA input;
+clock_t time_init, time_end, time_tmp;
 
 void usage(void);
 
 int main(int argc, char *argv[]) {
 
   /**  time count  **/
   time_init = clock();
```

### Comparing `pymican-1.9.1.dev0/src/main_align.c` & `pymican-1.9.2/src/main_align.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 void copy_align(int naa_q, int naa_t, ALIGN *align1, ALIGN *align2);
 
 void main_align(void) {
   int i, j, k;
   int iaa;
   int naa_q, naa_t, naa_tmp, naa_max;
@@ -80,15 +81,15 @@
     }
     if (input.TM_d0 > TM_d0_MAX) {
       input.TM_d0 = TM_d0_MAX;
     }
   }
 
   /**  naa effective (for Dali Zscore)  **/
-  input.naa_eff = sqrt(naa_q * naa_t);
+  input.naa_eff = sqrt((double)naa_q * (double)naa_t);
 
   /**  calloc RESDAT  **/
   resdat_q = (RESDAT *)calloc((size_t)(naa_q + 1), sizeof(RESDAT));
   resdat_t = (RESDAT *)calloc((size_t)(naa_t + 1), sizeof(RESDAT));
 
   /**  calloc all ATOM  **/
   allatm_q = (ALLATM *)calloc((size_t)(natom_q + 1), sizeof(ALLATM));
```

### Comparing `pymican-1.9.1.dev0/src/make_hash_table.c` & `pymican-1.9.2/src/make_hash_table.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 /*************************************/
 /**     FUNCTION  pre_make_hash     **/
 /*************************************/
 void pre_make_hash(int nsse, int nhash, HASH_TABLE ***hash, SSEDAT *ssedat) {
   int i, j, k;
   int id_x, id_y, id_z;
```

### Comparing `pymican-1.9.1.dev0/src/make_pdbdat.c` & `pymican-1.9.2/src/make_pdbdat.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/mican.h` & `pymican-1.9.2/src/mican.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef INCLUDED_mican_h_
+#define INCLUDED_mican_h_
+
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
 #include <string.h>
 #include <limits.h>
 #include <time.h>
 
@@ -165,15 +168,14 @@
   /****  output option  ****/
   int silent;
   int progress;
   /****  invisible option  ****/
   int printalign;
 } INPUT_DATA;
 
-INPUT_DATA input;
 
 typedef struct {
   int exist;
   float x;
   float y;
   float z;
   char name[4 + 1];
@@ -277,15 +279,14 @@
   float C3score;
   float TMloc_mod;
   float score_cmp;
 
   float seqID;
 } ALIGN;
 
-clock_t time_init, time_end, time_tmp;
 
 /**********************/
 /**     FUNCTION      */
 /**********************/
 
 /**  Main Controll Function  **/
 void main_align(void);
@@ -369,7 +370,9 @@
 /**  Utils  **/
 void bstft(int n, RESDAT *resdat1, RESDAT *resdat2, float *vec, float **rot);
 void wbstft(int n, RESDAT *resdat1, RESDAT *resdat2, float *vec, float **rot, float *weight);
 int svd(int m, int n, int withu, int withv, double eps, double tol, double *a,
         double *q, double *u, double *v, double *vt);
 float angle(float *a1, float *a2, float *a3, float *b1, float *b2, float *b3);
 float distance_2(float *a, float *b);
+
+#endif
```

### Comparing `pymican-1.9.1.dev0/src/output.c` & `pymican-1.9.2/src/output.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 void output(int naa_q, int naa_t, int natom_q, int natom_t, RESDAT *resdat_q,
             RESDAT *resdat_t, ALLATM *allatm_q, ALLATM *allatm_t, ALIGN *align,
             ALIGN ***align_chain, PDBDAT pdbdat_q, PDBDAT pdbdat_t) {
   int i;
   FILE *fp;
   int ichain, jchain;
```

### Comparing `pymican-1.9.1.dev0/src/print_data.c` & `pymican-1.9.2/src/print_data.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 /**  function print INPUT protein data  **/
 void printinp(int naa_q, int naa_t, PDBDAT pdbdat_q, PDBDAT pdbdat_t) {
   char filename1[STRSIZE], filename2[STRSIZE];
   int naa1, naa2, nchain1, nchain2;
   char chainuse1[STRSIZE], chainuse2[STRSIZE];
```

### Comparing `pymican-1.9.1.dev0/src/print_pdb.c` & `pymican-1.9.2/src/print_pdb.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/read_pdb.c` & `pymican-1.9.2/src/read_pdb.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/resname2reschar.c` & `pymican-1.9.2/src/resname2reschar.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/rmsd.c` & `pymican-1.9.2/src/rmsd.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/score.c` & `pymican-1.9.2/src/score.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 /** function for comparison of hash results **/
 PRIVATE int compare(const void *a, const void *b);
 
 void score_calculation(int naa_q, int naa_t, int nalign, ALIGN *align,
                        RESDAT *resdat_q, RESDAT *resdat_t) {
   int iaa;
```

### Comparing `pymican-1.9.1.dev0/src/search_hash.c` & `pymican-1.9.2/src/search_hash.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "mican.h"
+#include "main.h"
 
 PRIVATE void search(int *ialign, int nsse_q, int nsse_t, int nhash,
                     HASH_TABLE ***hash, SSEDAT *ssedat, HASH_RESULT *hres,
                     int mode);
 PRIVATE void search_list(int id_x, int id_y, int id_z, HASH_TABLE ***hash,
                          SSEDAT *ssedat, int isse, int ksse, float *para,
                          float *perp, float *coor, float *count);
```

### Comparing `pymican-1.9.1.dev0/src/superposition.c` & `pymican-1.9.2/src/superposition.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/svd.c` & `pymican-1.9.2/src/svd.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/utils.c` & `pymican-1.9.2/src/utils.c`

 * *Files identical despite different names*

### Comparing `pymican-1.9.1.dev0/src/xyz2vec.c` & `pymican-1.9.2/src/xyz2vec.c`

 * *Files identical despite different names*

