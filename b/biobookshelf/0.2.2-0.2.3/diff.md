# Comparing `tmp/biobookshelf-0.2.2.tar.gz` & `tmp/biobookshelf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobookshelf-0.2.2.tar", last modified: Tue Apr  4 13:04:38 2023, max compression
+gzip compressed data, was "biobookshelf-0.2.3.tar", last modified: Tue May  2 03:15:45 2023, max compression
```

## Comparing `biobookshelf-0.2.2.tar` & `biobookshelf-0.2.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.807491 biobookshelf-0.2.2/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.2/LICENSE
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.2/MANIFEST.in
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-04-04 13:04:38.807491 biobookshelf-0.2.2/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.2/README.md
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.411484 biobookshelf-0.2.2/biobookshelf/
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.411484 biobookshelf-0.2.2/biobookshelf/BA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       29 2022-06-12 10:31:17.000000 biobookshelf-0.2.2/biobookshelf/BA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8096 2022-08-10 14:29:21.000000 biobookshelf-0.2.2/biobookshelf/BA/bitarray_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.435484 biobookshelf-0.2.2/biobookshelf/CLI/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       36 2022-04-05 10:28:47.000000 biobookshelf-0.2.2/biobookshelf/CLI/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2889 2022-06-16 13:40:33.000000 biobookshelf-0.2.2/biobookshelf/CLI/unclassified_programs.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.471485 biobookshelf-0.2.2/biobookshelf/INT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2022-04-04 14:27:30.000000 biobookshelf-0.2.2/biobookshelf/INT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      404 2022-04-21 11:45:14.000000 biobookshelf-0.2.2/biobookshelf/INT/integer.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.503485 biobookshelf-0.2.2/biobookshelf/IT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/IT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       33 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/IT/interval_tree_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.527486 biobookshelf-0.2.2/biobookshelf/L/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/L/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       41 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/L/l_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.539486 biobookshelf-0.2.2/biobookshelf/MAP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/MAP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      638 2022-04-21 11:44:18.000000 biobookshelf-0.2.2/biobookshelf/MAP/mapping.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.563486 biobookshelf-0.2.2/biobookshelf/MP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       36 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/MP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      268 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/MP/multiprocessing_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.567487 biobookshelf-0.2.2/biobookshelf/ONT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       33 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/ONT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    52397 2023-04-04 12:40:00.000000 biobookshelf-0.2.2/biobookshelf/ONT/nanopore_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.571487 biobookshelf-0.2.2/biobookshelf/PD/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/PD/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       86 2022-04-21 11:42:53.000000 biobookshelf-0.2.2/biobookshelf/PD/pd_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.583487 biobookshelf-0.2.2/biobookshelf/PDB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/PDB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    26337 2022-04-21 11:42:43.000000 biobookshelf-0.2.2/biobookshelf/PDB/pdb.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.603487 biobookshelf-0.2.2/biobookshelf/PKG/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/PKG/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2959 2022-04-21 11:42:25.000000 biobookshelf-0.2.2/biobookshelf/PKG/package_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.619487 biobookshelf-0.2.2/biobookshelf/RNA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       21 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/RNA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14992 2022-04-30 19:37:29.000000 biobookshelf-0.2.2/biobookshelf/RNA/rnaseq.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.675489 biobookshelf-0.2.2/biobookshelf/SAM/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/SAM/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    62144 2023-01-07 10:20:40.000000 biobookshelf-0.2.2/biobookshelf/SAM/sam_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.703489 biobookshelf-0.2.2/biobookshelf/SC/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/SC/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   105156 2023-01-31 07:40:11.000000 biobookshelf-0.2.2/biobookshelf/SC/single_cell.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.723489 biobookshelf-0.2.2/biobookshelf/SEQ/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/SEQ/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    13996 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/SEQ/sequence.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.727489 biobookshelf-0.2.2/biobookshelf/STR/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       21 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/STR/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    13433 2022-06-15 15:08:10.000000 biobookshelf-0.2.2/biobookshelf/STR/string.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.751490 biobookshelf-0.2.2/biobookshelf/UniProt/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/UniProt/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      857 2022-04-21 11:39:58.000000 biobookshelf-0.2.2/biobookshelf/UniProt/uniprot.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.767490 biobookshelf-0.2.2/biobookshelf/WEB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/WEB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8224 2022-07-04 14:27:50.000000 biobookshelf-0.2.2/biobookshelf/WEB/web_application.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.795491 biobookshelf-0.2.2/biobookshelf/ZA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       25 2022-06-24 15:02:17.000000 biobookshelf-0.2.2/biobookshelf/ZA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       11 2022-06-27 07:41:03.000000 biobookshelf-0.2.2/biobookshelf/ZA/zarr_utils.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      296 2023-04-04 12:59:52.000000 biobookshelf-0.2.2/biobookshelf/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      171 2022-04-04 14:27:31.000000 biobookshelf-0.2.2/biobookshelf/__main__.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.803491 biobookshelf-0.2.2/biobookshelf/main/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.2/biobookshelf/main/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   638633 2023-04-02 09:26:39.000000 biobookshelf-0.2.2/biobookshelf/main/unclassified_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-04-04 13:04:38.411484 biobookshelf-0.2.2/biobookshelf.egg-info/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-04-04 13:04:37.000000 biobookshelf-0.2.2/biobookshelf.egg-info/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-04-04 13:04:38.000000 biobookshelf-0.2.2/biobookshelf.egg-info/SOURCES.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-04-04 13:04:37.000000 biobookshelf-0.2.2/biobookshelf.egg-info/dependency_links.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-04-04 13:04:37.000000 biobookshelf-0.2.2/biobookshelf.egg-info/entry_points.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-04-04 13:04:37.000000 biobookshelf-0.2.2/biobookshelf.egg-info/requires.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-04-04 13:04:37.000000 biobookshelf-0.2.2/biobookshelf.egg-info/top_level.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-04-04 13:04:38.807491 biobookshelf-0.2.2/setup.cfg
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-04-04 13:04:13.000000 biobookshelf-0.2.2/setup.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/LICENSE
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/MANIFEST.in
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.3/README.md
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/BA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/BA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/BA/bitarray_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/CLI/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/CLI/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3012 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/CLI/unclassified_programs.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/INT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/INT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/INT/integer.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/IT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/IT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/IT/interval_tree_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/L/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/L/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/L/l_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/MAP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MAP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MAP/mapping.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/MP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/MP/multiprocessing_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/ONT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ONT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    63568 2023-05-01 11:20:31.000000 biobookshelf-0.2.3/biobookshelf/ONT/nanopore_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PD/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PD/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PD/pd_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PDB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/PDB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29069 2023-05-01 11:20:31.000000 biobookshelf-0.2.3/biobookshelf/PDB/pdb.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf/PKG/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PKG/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3096 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/PKG/package_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/RNA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/RNA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.3/biobookshelf/RNA/rnaseq.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SAM/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/SAM/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.3/biobookshelf/SAM/sam_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SC/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/SC/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122816 2023-05-01 11:20:34.000000 biobookshelf-0.2.3/biobookshelf/SC/single_cell.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/SEQ/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/SEQ/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14816 2023-05-01 11:20:30.000000 biobookshelf-0.2.3/biobookshelf/SEQ/sequence.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/STR/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/STR/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/STR/string.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/UniProt/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/UniProt/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/UniProt/uniprot.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/WEB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.3/biobookshelf/WEB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8722 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/WEB/web_application.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/ZA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ZA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/ZA/zarr_utils.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/biobookshelf/__main__.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.430486 biobookshelf-0.2.3/biobookshelf/main/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.3/biobookshelf/main/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   711938 2023-05-01 11:21:08.000000 biobookshelf-0.2.3/biobookshelf/main/unclassified_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-02 03:15:45.426486 biobookshelf-0.2.3/biobookshelf.egg-info/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/SOURCES.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/dependency_links.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/entry_points.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/requires.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-02 03:15:45.000000 biobookshelf-0.2.3/biobookshelf.egg-info/top_level.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-02 03:15:45.434486 biobookshelf-0.2.3/setup.cfg
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-01 11:20:29.000000 biobookshelf-0.2.3/setup.py
```

### Comparing `biobookshelf-0.2.2/LICENSE` & `biobookshelf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.2/PKG-INFO` & `biobookshelf-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.2
+Version: 0.2.3
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.2/biobookshelf/BA/bitarray_utils.py` & `biobookshelf-0.2.3/biobookshelf/BA/bitarray_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,199 +1,225 @@
 from bitarray import bitarray
 import numpy as np
 
-def Find( ba, val = 1 ) :
-    ''' deprecated
-    # 2022-06-12 21:09:22 
+
+def Find(ba, val=1):
+    """deprecated
+    # 2022-06-12 21:09:22
     search the given value in the bitarray iteratively and return the start position of the occurrences
-    '''
-    len_ba = len( ba )
-    l_int_pos_occurrence = [ ]
+    """
+    len_ba = len(ba)
+    l_int_pos_occurrence = []
     int_pos_start = 0
-    while int_pos_start < len_ba :
-        int_pos_occurrence = ba.find( val, int_pos_start + 1 )
-        if int_pos_occurrence < 0 :
+    while int_pos_start < len_ba:
+        int_pos_occurrence = ba.find(val, int_pos_start + 1)
+        if int_pos_occurrence < 0:
             break
-        else :
-            l_int_pos_occurrence.append( int_pos_occurrence )
+        else:
+            l_int_pos_occurrence.append(int_pos_occurrence)
             int_pos_start = int_pos_occurrence
     return l_int_pos_occurrence
 
-def find( ba, val = 1 ) :
-    ''' # 2022-07-03 21:41:36 
+
+def find(ba, val=1):
+    """# 2022-07-03 21:41:36
     generator that returns the location of 'val' from the start of the bitarray.
     Use this function for memory-efficient iteration of position of active entries in a bitarray (np.int64 takes 64 times more memory than an entry in bitarray, which is 1 bit).
-    '''
-    len_ba = len( ba )
-    if len( ba ) == 0 : # handle empty bitarray input
+    """
+    len_ba = len(ba)
+    if len(ba) == 0:  # handle empty bitarray input
         return
     int_pos_start = 0
-    if ba[ 0 ] == val : # handle the case when the first bit is equal to 'val'
+    if ba[0] == val:  # handle the case when the first bit is equal to 'val'
         yield int_pos_start
-    while int_pos_start < len_ba :
-        int_pos_occurrence = ba.find( val, int_pos_start + 1 )
-        if int_pos_occurrence < 0 :
+    while int_pos_start < len_ba:
+        int_pos_occurrence = ba.find(val, int_pos_start + 1)
+        if int_pos_occurrence < 0:
             break
-        else :
+        else:
             yield int_pos_occurrence
             int_pos_start = int_pos_occurrence
 
+
 # def Find_Segment( ba, background = 1, flag_use_bitwise_operation = True ) :
-#     ''' # 2022-06-12 19:36:38 
+#     ''' # 2022-06-12 19:36:38
 #     find segment of a given bitarray for the given background 'background'. for example, when background = 1, find segment of 0
-    
+
 #     'flag_use_bitwise_operation' : use bitwise operation. useful when the length of bitarray is very long
 #     '''
 #     len_ba = len( ba )
-#     if flag_use_bitwise_operation : 
+#     if flag_use_bitwise_operation :
 #         ''' the implementation using bitwise operation '''
 #         mask = ( ba ^ ba >> 1 ) # find boundary of value change
 #         l_int_pos = Find( mask, 1 )
 #         flag_start_is_a_segment = ba[ 0 ] != background
 #         if flag_start_is_a_segment :
 #             l_int_pos = [ 0 ] + l_int_pos
 #         if len( l_int_pos ) % 2 != 0 :
 #             l_int_pos += [ len_ba ]
 #         return np.array( l_int_pos ).reshape( ( int( len( l_int_pos ) / 2 ), 2 ) )
 #     else :
 #         ''' the implementation using simple iteration '''
-#         int_pos = 0 
+#         int_pos = 0
 #         int_seg_start = None
 #         l_seg = [ ]
 #         while int_pos < len_ba :
 #             if int_seg_start is None and ba[ int_pos ] != background :
 #                 int_seg_start = int_pos
 #             elif int_seg_start is not None and ba[ int_pos ] == background :
 #                 l_seg.append( [ int_seg_start, int_pos ] )
 #                 int_seg_start = None
 #             int_pos += 1
 #         if int_seg_start is not None :
 #             l_seg.append( [ int_seg_start, len_ba ] )
 #         return l_seg
 
-def Find_Segment( ba, background = 1 ) :
-    ''' # 2022-06-12 19:36:38 
+
+def Find_Segment(ba, background=1):
+    """# 2022-06-12 19:36:38
     find segment of a given bitarray for the given background 'background'. for example, when background = 1, find segment of 0
-    
-    # 2022-06-22 18:36:45 
+
+    # 2022-06-22 18:36:45
     updated to a new implementation that does not require generating a copy of the bitarray.
-    '''
-    def toggle_bit( bit ) :
-        return ( bit + 1 ) % 2 # toggle the bit
-    
+    """
+
+    def toggle_bit(bit):
+        return (bit + 1) % 2  # toggle the bit
+
     # initialize
-    l_int_pos = [ ]
-    state_of_interest = toggle_bit( background ) # look for a non-background state
+    l_int_pos = []
+    state_of_interest = toggle_bit(background)  # look for a non-background state
     int_pos = 0
-    
-    while True :
-        int_pos = ba.find( state_of_interest, int_pos )
-        if int_pos < 0 :
+
+    while True:
+        int_pos = ba.find(state_of_interest, int_pos)
+        if int_pos < 0:
             break
-        l_int_pos.append( int_pos )
-        state_of_interest = toggle_bit( state_of_interest ) # toggle the state of interest
-    if len( l_int_pos ) % 2 != 0 :
-        l_int_pos.append( len( ba ) )
-    return np.array( l_int_pos ).reshape( ( int( len( l_int_pos ) / 2 ), 2 ) ) # reshape a list of int_pos to list of segments
-
-def Retrieve_Integer_Indices( ba, background = 0 ) :
-    """ deprecated (slow)
-    # 2022-06-23 08:31:45 
+        l_int_pos.append(int_pos)
+        state_of_interest = toggle_bit(
+            state_of_interest
+        )  # toggle the state of interest
+    if len(l_int_pos) % 2 != 0:
+        l_int_pos.append(len(ba))
+    return np.array(l_int_pos).reshape(
+        (int(len(l_int_pos) / 2), 2)
+    )  # reshape a list of int_pos to list of segments
+
+
+def Retrieve_Integer_Indices(ba, background=0):
+    """deprecated (slow)
+    # 2022-06-23 08:31:45
     returns a list of integer indices of non-background bits in a given bitarray 'ba'
-    
+
     'background' : a bit representing background. either 0 or 1
     """
     # compose a list of integer indices of active rows after applying filter
-    l = [ ]
-    for st, en in Find_Segment( ba, background = background ) : # retrieve active segments from bitarray filter 
-        l.extend( range( st, en ) ) # retrieve integer indices of the active rows
+    l = []
+    for st, en in Find_Segment(
+        ba, background=background
+    ):  # retrieve active segments from bitarray filter
+        l.extend(range(st, en))  # retrieve integer indices of the active rows
     return l
 
-def to_array( ba ) :
-    ''' # 2022-06-24 23:54:12 
-    return a boolean numpy array of the given bitarray '''
-    return np.frombuffer( ba.unpack( ), dtype = bool )
 
-def to_bitarray( arr_bool ) :
-    """ # 2022-06-27 15:29:56 
+def to_array(ba):
+    """# 2022-06-24 23:54:12
+    return a boolean numpy array of the given bitarray"""
+    return np.frombuffer(ba.unpack(), dtype=bool)
+
+
+def to_bitarray(arr_bool):
+    """# 2022-06-27 15:29:56
     convert numpy boolean array to bitarray
     """
-    ba = bitarray( )
-    ba.pack( arr_bool.tobytes( ) )
+    ba = bitarray()
+    ba.pack(arr_bool.tobytes())
     return ba
 
-def from_integer_indices_to_bitarray( l_int_index, length ) :
-    """ # 2022-07-01 11:21:12 
+
+def from_integer_indices_to_bitarray(l_int_index, length):
+    """# 2022-07-01 11:21:12
     convert list of integer indices to bitarray
-    
+
     'length' : length of the output bitarray object
     """
-    ba = bitarray( length )
-    ba.setall( 0 )
-    for int_index in l_int_index :
-        ba[ int_index ] = True
+    ba = bitarray(length)
+    ba.setall(0)
+    for int_index in l_int_index:
+        ba[int_index] = True
     return ba
 
-def to_integer_indices( ba ) :
-    """ # 2022-07-01 21:38:17 
+
+def to_integer_indices(ba):
+    """# 2022-07-01 21:38:17
     retrieve integer indices of the active entries of the given bitarray
-    
+
     'ba' : input bitarray object
     """
-    return np.where( to_array( ba ) )[ 0 ]
+    return np.where(to_array(ba))[0]
+
 
-def COUNTER( l_values, dict_counter = None, ignore_float = True ) : # 2020-07-29 23:49:51 
-    ''' Count values in l_values and return a dictionary containing count values. if 'dict_counter' is given, countinue counting by using the 'dict_counter'. if 'ignore_float' is True, ignore float values, including np.nan '''
-    if dict_counter is None : dict_counter = dict( )
-    if ignore_float : # if 'ignore_float' is True, ignore float values, including np.nan
-        for value in l_values :
-            if isinstance( value, float ) : continue # ignore float values
-            if value in dict_counter : dict_counter[ value ] += 1
-            else : dict_counter[ value ] = 1
-    else : # faster counting by not checking type of value
-        for value in l_values :
-            if value in dict_counter : dict_counter[ value ] += 1
-            else : dict_counter[ value ] = 1
+def COUNTER(l_values, dict_counter=None, ignore_float=True):  # 2020-07-29 23:49:51
+    """Count values in l_values and return a dictionary containing count values. if 'dict_counter' is given, countinue counting by using the 'dict_counter'. if 'ignore_float' is True, ignore float values, including np.nan"""
+    if dict_counter is None:
+        dict_counter = dict()
+    if ignore_float:  # if 'ignore_float' is True, ignore float values, including np.nan
+        for value in l_values:
+            if isinstance(value, float):
+                continue  # ignore float values
+            if value in dict_counter:
+                dict_counter[value] += 1
+            else:
+                dict_counter[value] = 1
+    else:  # faster counting by not checking type of value
+        for value in l_values:
+            if value in dict_counter:
+                dict_counter[value] += 1
+            else:
+                dict_counter[value] = 1
     return dict_counter
 
-def detect_boolean_mask( ba ) :
-    """ # 2022-08-10 23:29:06 
+
+def detect_boolean_mask(ba):
+    """# 2022-08-10 23:29:06
     detect boolean mask by looking up to 10 values
     """
     # extract the first row from the ndarray data
-    if isinstance( ba, np.ndarray ) and len( ba.shape ) > 1 :
-        for i in range( len( ba.shape ) - 1 ) :
-            ba = ba[ 0 ]
-    if not hasattr( ba, '__iter__' ) : # 'ba' should be iterable to be a boolean mask
+    if isinstance(ba, np.ndarray) and len(ba.shape) > 1:
+        for i in range(len(ba.shape) - 1):
+            ba = ba[0]
+    if not hasattr(ba, "__iter__"):  # 'ba' should be iterable to be a boolean mask
         return False
-    ba = ba[ : 10 ]
+    ba = ba[:10]
     # if the length of array of interest is <= 2 and only consists of 0, 1, consider it as an integer array, not boolean array
-    if len( ba ) <= 2 and set( COUNTER( ba[ : 10 ] ) ).issubset( { 0, 1 } ) :
+    if len(ba) <= 2 and set(COUNTER(ba[:10])).issubset({0, 1}):
         return False
-    return set( COUNTER( ba[ : 10 ] ) ).issubset( { 0, 1, True, False } )
+    return set(COUNTER(ba[:10])).issubset({0, 1, True, False})
+
 
-def convert_mask_to_bitarray( ba ) :
-    ''' # 2022-07-03 00:54:46 
+def convert_mask_to_bitarray(ba):
+    """# 2022-07-03 00:54:46
     convert boolean mask to a bitarray
-    '''
+    """
     # handle when a list type has been given (convert it to np.ndarray)
-    if isinstance( ba, list ) :
-        ba = np.array( ba, dtype = bool )
+    if isinstance(ba, list):
+        ba = np.array(ba, dtype=bool)
     # handle when a numpy ndarray has been given (convert it to bitarray)
-    if isinstance( ba, np.ndarray ) :
-        ba = to_bitarray( ba )
-    assert isinstance( ba, bitarray ) # check the return value is bitarray object
-    return ba 
+    if isinstance(ba, np.ndarray):
+        ba = to_bitarray(ba)
+    assert isinstance(ba, bitarray)  # check the return value is bitarray object
+    return ba
 
-def convert_mask_to_array( ba ) :
-    ''' # 2022-07-03 00:54:46 
+
+def convert_mask_to_array(ba):
+    """# 2022-07-03 00:54:46
     convert boolean mask to a array
-    '''
-    ''' handle non-bitarray mask types '''
+    """
+    """ handle non-bitarray mask types """
     # handle when a list type has been given (convert it to np.ndarray)
-    if isinstance( ba, list ) :
-        ba = np.array( ba, dtype = bool )
+    if isinstance(ba, list):
+        ba = np.array(ba, dtype=bool)
     # handle when a numpy ndarray has been given (convert it to np.ndarray)
-    if isinstance( ba, bitarray ) :
-        ba = to_array( ba )
-    assert isinstance( ba, np.ndarray ) # check the return value is np.ndarray object
-    return ba 
+    if isinstance(ba, bitarray):
+        ba = to_array(ba)
+    assert isinstance(ba, np.ndarray)  # check the return value is np.ndarray object
+    return ba
```

### Comparing `biobookshelf-0.2.2/biobookshelf/CLI/unclassified_programs.py` & `biobookshelf-0.2.3/biobookshelf/CLI/unclassified_programs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,91 @@
 from biobookshelf.main import *
 from biobookshelf import PKG
 
 # Command line programs
-def Recursively_stop_subprocesses( int_pid ) :
-    if int_pid < 1e3 :
-        print( 'ERROR: given PID {} has less than 4 digits. For security reasons, this program failed'.format( int_pid ) ), sys.exit( 2 ) 
-    df_processes = OS_Currently_running_processes( )
-    if int_pid in df_processes.PID.values :
-        os.system( 'kill {}'.format( int_pid ) )
-    df_subprocesses = PD_Select( df_processes, PPID = int_pid )
-    for int_pid_subprocess in df_subprocesses.PID.values :
-        Recursively_stop_subprocesses( int_pid_subprocess )
-def Stop_a_job( pid = None ) :
+def Recursively_stop_subprocesses(int_pid):
+    if int_pid < 1e3:
+        print(
+            "ERROR: given PID {} has less than 4 digits. For security reasons, this program failed".format(
+                int_pid
+            )
+        ), sys.exit(2)
+    df_processes = OS_Currently_running_processes()
+    if int_pid in df_processes.PID.values:
+        os.system("kill {}".format(int_pid))
+    df_subprocesses = PD_Select(df_processes, PPID=int_pid)
+    for int_pid_subprocess in df_subprocesses.PID.values:
+        Recursively_stop_subprocesses(int_pid_subprocess)
+
+
+def Stop_a_job(pid=None):
     """
     # 2022/04/05
     Stop a process with a given PID and all subprocess belonging to the PID.
-    
+
     'pid' : pid to recursively terminates
     """
-    flag_entry_point = PKG.Detect_Entry_Point( 'biobook' ) # detect whether an entry point was used
-    if flag_entry_point :
-        parser = argparse.ArgumentParser( description = "Stop a process with a given PID and all subprocess belonging to the PID. This program has been developed by Hyunsu An (2021/06/03)." )
-        
-        parser.add_argument( "-i", "--pid", help = "PID of a job to be terminated. (required)", type = int )
-        args = parser.parse_args( )
+    flag_entry_point = PKG.Detect_Entry_Point(
+        "biobook"
+    )  # detect whether an entry point was used
+    if flag_entry_point:
+        parser = argparse.ArgumentParser(
+            description="Stop a process with a given PID and all subprocess belonging to the PID. This program has been developed by Hyunsu An (2021/06/03)."
+        )
+
+        parser.add_argument(
+            "-i", "--pid", help="PID of a job to be terminated. (required)", type=int
+        )
+        args = parser.parse_args()
 
         # [input] parse arguments from parse_args
         int_pid = args.pid
-    
-    ''' [parse arguments] '''
-    if int_pid is None :
-        print( "required arguments are not given, exiting" )
-        if flag_entry_point :
-            sys.exit( ) 
-        else :
+
+    """ [parse arguments] """
+    if int_pid is None:
+        print("required arguments are not given, exiting")
+        if flag_entry_point:
+            sys.exit()
+        else:
             return -1
-    Recursively_stop_subprocesses( int_pid )
-    
-def Server_Status( ) :
+    Recursively_stop_subprocesses(int_pid)
+
+
+def Server_Status():
     """
     # 2022/04/05
     Print CPU and MEMORY usage of the FGL server for each program for each user.
     """
-    flag_entry_point = PKG.Detect_Entry_Point( 'biobook' ) # detect whether an entry point was used
-    if flag_entry_point :
-        parser = argparse.ArgumentParser( description = "Print CPU and MEMORY usage of the FGL server for each program for each user. This program has been developed by Hyunsu An." )
-        args = parser.parse_args( )
-    
-    df = Parse_Printed_Table( '\n'.join( os.popen( 'top -bn 1' ).read( ).split( '\n' )[ 6 : ] ) ).rename( columns = { '%CPU' : 'CPU', '%MEM' : 'MEM'  } ) # rename columns to make it compatible with pandas DataFrame
-    df = df[ ( df.CPU > 0 ) | ( df.MEM > 0 ) ] # if remove processes using '0' CPU and '0' MEM.
-    print( ' ----- Usage Total ----- \n' )
-    print( df[ [ 'CPU', 'MEM' ] ].sum( ) )
-    print( '\n\n ----- Usage by each user ----- \n' )
-    print( df[ [ 'USER', 'CPU', 'MEM' ] ].groupby( 'USER' ).sum( ).sort_values( 'MEM', ascending = False ) )
-    print( '\n\n ----- Usage by each program of each user ----- \n' )
-    print( df[ [ 'USER', 'COMMAND', 'CPU', 'MEM' ] ].groupby( [ 'USER', 'COMMAND' ] ).sum( ).sort_values( 'MEM', ascending = False ) )
-    print( )
+    flag_entry_point = PKG.Detect_Entry_Point(
+        "biobook"
+    )  # detect whether an entry point was used
+    if flag_entry_point:
+        parser = argparse.ArgumentParser(
+            description="Print CPU and MEMORY usage of the FGL server for each program for each user. This program has been developed by Hyunsu An."
+        )
+        args = parser.parse_args()
+
+    df = Parse_Printed_Table(
+        "\n".join(os.popen("top -bn 1").read().split("\n")[6:])
+    ).rename(
+        columns={"%CPU": "CPU", "%MEM": "MEM"}
+    )  # rename columns to make it compatible with pandas DataFrame
+    df = df[
+        (df.CPU > 0) | (df.MEM > 0)
+    ]  # if remove processes using '0' CPU and '0' MEM.
+    print(" ----- Usage Total ----- \n")
+    print(df[["CPU", "MEM"]].sum())
+    print("\n\n ----- Usage by each user ----- \n")
+    print(
+        df[["USER", "CPU", "MEM"]]
+        .groupby("USER")
+        .sum()
+        .sort_values("MEM", ascending=False)
+    )
+    print("\n\n ----- Usage by each program of each user ----- \n")
+    print(
+        df[["USER", "COMMAND", "CPU", "MEM"]]
+        .groupby(["USER", "COMMAND"])
+        .sum()
+        .sort_values("MEM", ascending=False)
+    )
+    print()
```

### Comparing `biobookshelf-0.2.2/biobookshelf/ONT/nanopore_functions.py` & `biobookshelf-0.2.3/biobookshelf/ONT/nanopore_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,839 +1,1516 @@
 # load internal module
 from biobookshelf.main import *
 import biobookshelf as bk
 import biobookshelf.PKG as PKG
 from typing import Union, List, Literal, Dict, Callable, Set, Iterable, Tuple
 
-def create_gene_count_from_fast5( 
-    l_path_folder_nanopore_sequencing_data : Union[ str, list ], # list of folders containing nanopore sequencing data
-    l_name_config : Union[ str, List ], # a name of config or a list of name_config 
-    l_barcoding_kit : Union[ str, List, None ], # a name of config or a list of name_config 
-    path_folder_output : str, # a path to the output folder
-    dict_name_bc_to_name_sample : Union[ dict, None ], # barcode to name_sample
-    dict_name_sample_to_organism : Union[ dict, None ], # define organism for each sample
-    dict_anno : Union[ dict, None ], # a dictionary containing annotation information for each organism
-    int_num_cpus : int = 22, # the number of cpus to use
-    flag_include_failed : bool = True, # include the failed reads into the fastq output
-    int_max_num_reads_for_drawing_size_distribution : int = 100000, # the maximum number of reads to use to draw a size distribution
-    int_max_size_for_displaying_size_distribution : int = 2000, # max molecule length to display in the histogram
-    int_num_binds_for_displaying_size_distribution : int = 200, # number of bins for drawing histogram
-) :
-    """ # 2023-04-04 20:57:35 
+
+def __create_gene_count_from_fast5__align(ins):
+    """# 2023-04-24 05:32:41
+    internal function of 'create_gene_count_from_fast5'
+    """
+    # parse input
+    (
+        path_file_fq,
+        minimap2_index,
+        path_folder_minimap2_output,
+        int_num_cpus,
+        path_file_splice_junc,
+    ) = ins
+    Minimap2_Align(
+        flag_use_split_prefix=False,
+        path_file_fastq=path_file_fq,
+        path_file_minimap2_index=minimap2_index,
+        path_folder_minimap2_output=path_folder_minimap2_output,
+        n_threads=int_num_cpus,
+        drop_unaligned=False,
+        return_bash_shellscript=False,
+        path_file_junc_bed=path_file_splice_junc,
+    )  # perform alignment
+
+
+def create_gene_count_from_fast5(
+    l_path_folder_nanopore_sequencing_data: Union[
+        str, list, None
+    ] = None,  # list of folders containing nanopore sequencing data
+    l_name_config: Union[str, List] = None,  # a name of config or a list of name_config
+    l_barcoding_kit: Union[
+        str, List, None
+    ] = None,  # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
+    path_folder_output: Union[str, None] = None,  # a path to the output folder
+    dict_name_bc_to_name_sample: Union[dict, None] = None,  # barcode to name_sample
+    dict_name_sample_to_organism: Union[
+        dict, None
+    ] = None,  # define organism for each sample
+    dict_anno: Union[
+        dict, None
+    ] = None,  # a dictionary containing annotation information for each organism
+    int_num_cpus: Union[
+        int, None
+    ] = None,  # the number of cpus to use. By default, use all the available cores
+    flag_include_failed: bool = True,  # include the failed reads into the fastq output
+    int_max_num_reads_for_drawing_size_distribution: int = 100000,  # the maximum number of reads to use to draw a size distribution
+    int_max_size_for_displaying_size_distribution: int = 2000,  # max molecule length to display in the histogram
+    int_num_bins_for_displaying_size_distribution: int = 200,  # number of bins for drawing histogram
+    flag_require_barcodes_both_ends: bool = True,  # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
+    flag_rerun_guppy=False,  # rename the the output folder (if it exists) and rerun guppy if the flag is True
+):
+    """# 2023-04-22 23:54:01
     l_path_folder_nanopore_sequencing_data : list, # list of folders containing nanopore sequencing data
-    l_name_config : Union[ str, List ], # a name of config or a list of name_config 
+    l_name_config : Union[ str, List ], # a name of config or a list of name_config
+    l_barcoding_kit : Union[ str, List, None ], # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output : str, # a path to the output folder
     dict_name_bc_to_name_sample : Union[ dict, None ], # barcode to name_sample. if not given, exit after combining fastq files.
     dict_name_sample_to_organism : Union[ dict, None ], # define organism for each sample. if not given, does not align reads to genome and transcriptomes
     dict_anno : Union[ dict, None ], # a dictionary containing annotation information for each organism. if not given, does not align reads to genome and transcriptomes
     flag_include_failed : bool = True # include the failed reads into the fastq output
     int_max_num_reads_for_drawing_size_distribution : int = 100000 # the maximum number of reads to use to draw a size distribution
     int_max_size_for_displaying_size_distribution : int = 2000 # max molecule length to display in the histogram
-    int_num_binds_for_displaying_size_distribution : int = 200 # number of bins for drawing histogram
-
+    int_num_bins_for_displaying_size_distribution : int = 200 # number of bins for drawing histogram
+    flag_require_barcodes_both_ends : bool = True, # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
     """
+    # handle default values
+    if int_num_cpus is None:
+        int_num_cpus = os.cpu_count()  # By default, use all the available cores
+
+    if (
+        path_folder_output is not None
+    ):  # if output folder has been given, initiate the output folders
+        path_folder_pipeline = path_folder_output
+        path_folder_graph = f"{path_folder_pipeline}graph/"
+        path_folder_processed_data = f"{path_folder_pipeline}processed_data/"
+        for path_folder in [
+            path_folder_pipeline,
+            path_folder_graph,
+            path_folder_processed_data,
+            f"{path_folder_pipeline}shellscript_archive/",
+        ]:
+            os.makedirs(path_folder, exist_ok=True)
+
+    if (
+        l_path_folder_nanopore_sequencing_data is not None and l_name_config is not None
+    ):  # if 'l_path_folder_nanopore_sequencing_data' and 'l_name_config' has been given, run guppy_basecaller and combine output fastq files
+        # convert to list
+        if isinstance(l_path_folder_nanopore_sequencing_data, str):
+            l_path_folder_nanopore_sequencing_data = [
+                l_path_folder_nanopore_sequencing_data
+            ]
+        int_num_samples = len(
+            l_path_folder_nanopore_sequencing_data
+        )  # retrieve the number of samples
+        if isinstance(l_name_config, str):
+            l_name_config = [l_name_config] * int_num_samples
+        if (
+            isinstance(l_barcoding_kit, str) or l_barcoding_kit is None
+        ):  # detect single entry or a list of entries
+            l_barcoding_kit = [l_barcoding_kit] * int_num_samples
+
+        # correct inputs
+        l_path_folder_nanopore_sequencing_data = list(
+            e + "/" if e[-1] != "/" else e
+            for e in l_path_folder_nanopore_sequencing_data
+        )
+        l_name_config = list(
+            e + ".cfg" if e[-4:] != ".cfg" else e for e in l_name_config
+        )
+        # match length
+
+        for path_folder_nanopore_data, name_config, id_barcoding_kit in zip(
+            l_path_folder_nanopore_sequencing_data, l_name_config, l_barcoding_kit
+        ):
+            # create folders
+            path_folder_fast5 = f"{path_folder_nanopore_data}fast5_all/"
+            path_folder_guppy_output = f"{path_folder_nanopore_data}guppy_out/"
+            for path_folder in [path_folder_fast5, path_folder_guppy_output]:
+                os.makedirs(path_folder, exist_ok=True)
+
+            # collect fast5 files
+            for path_file in (
+                glob.glob(f"{path_folder_nanopore_data}fast5_skip/*.fast5")
+                + glob.glob(f"{path_folder_nanopore_data}fast5_fail/*/*.fast5")
+                + glob.glob(f"{path_folder_nanopore_data}fast5_pass/*/*.fast5")
+            ):
+                os.rename(
+                    path_file, f"{path_folder_fast5}{path_file.rsplit( '/', 1 )[ 1 ]}"
+                )
+
+            # run guppy
+            l_args = [
+                "guppy_basecaller",
+                "-c",
+                name_config,
+                "--input_path",
+                path_folder_fast5,
+                "--save_path",
+                path_folder_guppy_output,
+                "--device",
+                "auto",
+                "--compress_fastq",
+            ]
+            if (
+                flag_require_barcodes_both_ends
+            ):  # if 'flag_require_barcodes_both_ends' is True
+                l_args += ["--require_barcodes_both_ends"]
+            if l_barcoding_kit is not None:  # if valid 'l_barcoding_kit' has been given
+                l_args += ["--barcode_kits", id_barcoding_kit]
+            print(" ".join(l_args))  # print the guppy_basecaller command
+
+            flag_output_exists = os.path.exists(
+                f"{path_folder_guppy_output}sequencing_summary.txt"
+            )  # retrieve a flag indicating that the guppy output folder already exists
+            if (
+                flag_rerun_guppy and flag_output_exists
+            ):  # if 'flag_rerun_guppy' is True and the output folder exists
+                os.rename(
+                    path_folder_guppy_output,
+                    path_folder_guppy_output[:-1] + "." + bk.UUID() + "/",
+                )  # rename the existing guppy output folder
+                os.makedirs(
+                    path_folder_guppy_output, exist_ok=True
+                )  # create the output folder anew
+                flag_output_exists = False
+            if (
+                not flag_output_exists
+            ):  # if the guppy output already exist, skip running guppy
+                subprocess.run(l_args, capture_output=False)
+
+        # if output folder has not been given, exit
+        if path_folder_output is None:
+            return
+
+        # collect fastq files
+        df_fq = pd.concat(
+            list(
+                bk.GLOB_Retrive_Strings_in_Wildcards(
+                    f"{path_folder_nanopore_data}guppy_out/*/"
+                    + ("*/" if id_barcoding_kit is not None else "")
+                    + "*.fastq.gz"
+                )
+                for path_folder_nanopore_data in l_path_folder_nanopore_sequencing_data
+            )
+        )
 
-    # convert to list
-    if isinstance( l_path_folder_nanopore_sequencing_data, str ) :
-        l_path_folder_nanopore_sequencing_data = [ l_path_folder_nanopore_sequencing_data ]
-    int_num_samples = len( l_path_folder_nanopore_sequencing_data ) # retrieve the number of samples
-    if isinstance( l_name_config, str ) :
-        l_name_config = [ l_name_config ] * int_num_samples
-    if isinstance( l_barcoding_kit, str ) :
-        l_barcoding_kit = [ l_barcoding_kit ] * int_num_samples
-
-    # correct inputs
-    l_path_folder_nanopore_sequencing_data = list( e + '/' if e[ -1 ] != '/' else e for e in l_path_folder_nanopore_sequencing_data )
-    l_name_config = list( e + '.cfg' if e[ -4 : ] != '.cfg' else e for e in l_name_config )
-    # match length
-
-    for path_folder_nanopore_data, name_config, id_barcoding_kit in zip( l_path_folder_nanopore_sequencing_data, l_name_config, l_barcoding_kit ) :
-        # create folders
-        path_folder_fast5 = f"{path_folder_nanopore_data}fast5_all/"
-        path_folder_guppy_output = f"{path_folder_nanopore_data}guppy_out/"
-        for path_folder in [ path_folder_fast5, path_folder_guppy_output ] :
-            os.makedirs( path_folder, exist_ok = True )
-
-        # collect fast5 files
-        for path_file in glob.glob( f"{path_folder_nanopore_data}fast5_skip/*.fast5" ) + glob.glob( f"{path_folder_nanopore_data}fast5_fail/*/*.fast5" ) + glob.glob( f"{path_folder_nanopore_data}fast5_pass/*/*.fast5" ) :
-            os.rename( path_file, f"{path_folder_fast5}{path_file.rsplit( '/', 1 )[ 1 ]}" )
-
-        # run guppy
-        l_args = [ 'guppy_basecaller', '-c', name_config, "--input_path", path_folder_fast5, "--save_path", path_folder_guppy_output, '--require_barcodes_both_ends', '--device', 'auto', "--barcode_kits", id_barcoding_kit, "--compress_fastq" ]
-        print( " ".join( l_args ) )
-        if not os.path.exists( f"{path_folder_guppy_output}sequencing_summary.txt" ) : # if the guppy output already exist, skip running guppy
-            subprocess.run( l_args, capture_output = False )
-
-    # collect fastq files
-    df_fq = pd.concat( list( bk.GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_nanopore_data}guppy_out/*/" + ( '*/' if id_barcoding_kit is not None else '' ) + '*.fastq.gz' ) for path_folder_nanopore_data in l_path_folder_nanopore_sequencing_data ) )
-
-    # filter fastq files
-    if not flag_include_failed :
-        df_fq = PD_Select( df_fq, wildcard_0 = 'pass' ) # use only passed reads. 
-
-    # create output folder
-    path_folder_pipeline = path_folder_output
-    path_folder_graph = f'{path_folder_pipeline}graph/'
-    path_folder_processed_data = f"{path_folder_pipeline}processed_data/"
-    for path_folder in [ path_folder_pipeline, path_folder_graph, path_folder_processed_data, f"{path_folder_pipeline}shellscript_archive/" ] :
-        os.makedirs( path_folder, exist_ok = True )
-
-    # combine fastq files
-    for name_bc in df_fq.wildcard_1.unique( ) :
-        df_fq_for_name_bc = bk.PD_Select( df_fq, wildcard_1 = name_bc )
-        bk.OS_Run( [ 'cat' ] + list( df_fq_for_name_bc.path.values ), path_file_stdout = f"{path_folder_output}{name_bc}.fastq.gz", stdout_binary = True )
-
-    # if 'dict_name_bc_to_name_sample' has not given given, stop the operations
-    if dict_name_bc_to_name_sample is None :
-        return
+        # filter fastq files
+        if not flag_include_failed:
+            df_fq = PD_Select(df_fq, wildcard_0="pass")  # use only passed reads.
+
+        # combine fastq files
+        for name_bc in df_fq.wildcard_1.unique():
+            df_fq_for_name_bc = bk.PD_Select(df_fq, wildcard_1=name_bc)
+            bk.OS_Run(
+                ["cat"] + list(df_fq_for_name_bc.path.values),
+                path_file_stdout=f"{path_folder_output}{name_bc}.fastq.gz",
+                stdout_binary=True,
+            )
 
-    # rename fastq files and remove files that are not needed.
-    for path_file_fq in glob.glob( f"{path_folder_pipeline}*.fastq.gz" ) :
-        name_file = path_file_fq.rsplit( '/', 1 )[ 1 ].rsplit( '.fastq.gz', 1 )[ 0 ]
-        if name_file in dict_name_bc_to_name_sample : # if 'name_sample' is available for the barcode, rename the file
-            name_sample = dict_name_bc_to_name_sample[ name_file ]
-            os.rename( path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz" )
-        else : # if 'name_sample' is not available for the barcode, remove the file
-            os.remove( path_file_fq )
+    # if 'dict_name_bc_to_name_sample' has given, rename fastq files and remove files that are not needed.
+    if dict_name_bc_to_name_sample is not None:
+        for path_file_fq in glob.glob(
+            f"{path_folder_pipeline}*.fastq.gz"
+        ):  # for each fastq file
+            name_file = path_file_fq.rsplit("/", 1)[1].rsplit(".fastq.gz", 1)[0]
+            if (
+                name_file in dict_name_bc_to_name_sample
+            ):  # if 'name_sample' is available for the barcode, rename the file
+                name_sample = dict_name_bc_to_name_sample[name_file]
+                os.rename(path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz")
+            else:  # if 'name_sample' is not available for the barcode, remove the file
+                os.remove(path_file_fq)
 
     # draw molecule length distribution of each sample
-    for name_sample, path_file_fq in bk.GLOB_Retrive_Strings_in_Wildcards( f'{path_folder_pipeline}*.fastq.gz' ).values :
-        df_fq = bk.FASTQ_Read( path_file_fq, int_num_reads = int_max_num_reads_for_drawing_size_distribution )
-        fig, ax = plt.subplots( 1, 1, )
+    df_fastq = bk.GLOB_Retrive_Strings_in_Wildcards(
+        f"{path_folder_pipeline}*.fastq.gz"
+    )  # retrieve the paths of input fastq files
+    int_num_samples = len(
+        df_fastq
+    )  # retrieve the number of samples based on the number of fastq files
+    for name_sample, path_file_fq in df_fastq.values:
+        df_fq = bk.FASTQ_Read(
+            path_file_fq, int_num_reads=int_max_num_reads_for_drawing_size_distribution
+        )
+        fig, ax = plt.subplots(
+            1,
+            1,
+        )
         arr_len = df_fq.seq.apply(len).values
-        arr_len = arr_len[ arr_len < int_max_size_for_displaying_size_distribution ]
-        arr_counts, arr_bins, _ = ax.hist( arr_len, bins = int_num_binds_for_displaying_size_distribution ) 
-        bk.MPL_basic_configuration( title = bk.STR.Insert_characters_every_n_characters( name_sample, 60 ) + '\nNumber of Reads', show_grid = True, x_label = 'Number of Reads' )
-        bk.MPL_SAVE( f"(Number of Reads) Length distribution of {name_sample}", folder = path_folder_graph )
-        plt.bar( arr_bins[ : -1 ], arr_counts * arr_bins[ : -1 ], width = arr_bins[ 1 ] - arr_bins[ 0 ] )
-        bk.MPL_basic_configuration( title = bk.STR.Insert_characters_every_n_characters( name_sample, 60 ) + '\nNumber of Base Pairs', show_grid = True, x_label = 'Number of Base Pairs' )
-        bk.MPL_SAVE( f"(Number of Base Pairs) Length distribution of {name_sample}", folder = path_folder_graph )
+        arr_len = arr_len[arr_len < int_max_size_for_displaying_size_distribution]
+        arr_counts, arr_bins, _ = ax.hist(
+            arr_len, bins=int_num_bins_for_displaying_size_distribution
+        )
+        bk.MPL_basic_configuration(
+            title=bk.STR.Insert_characters_every_n_characters(name_sample, 60)
+            + "\nNumber of Reads",
+            show_grid=True,
+            x_label="Number of Reads",
+        )
+        bk.MPL_SAVE(
+            f"(Number of Reads) Length distribution of {name_sample}",
+            folder=path_folder_graph,
+        )
+        plt.bar(
+            arr_bins[:-1], arr_counts * arr_bins[:-1], width=arr_bins[1] - arr_bins[0]
+        )
+        bk.MPL_basic_configuration(
+            title=bk.STR.Insert_characters_every_n_characters(name_sample, 60)
+            + "\nNumber of Base Pairs",
+            show_grid=True,
+            x_label="Number of Base Pairs",
+        )
+        bk.MPL_SAVE(
+            f"(Number of Base Pairs) Length distribution of {name_sample}",
+            folder=path_folder_graph,
+        )
 
     # if annotation is not given, exit
-    if dict_anno is None or dict_name_sample_to_organism is None :
+    if dict_anno is None or dict_name_sample_to_organism is None:
         return
 
     # create the output folder for minimap2 alignments
-    for path_folder in [ f'{path_folder_pipeline}minimap2/genome/', f'{path_folder_pipeline}minimap2/transcriptome/' ] :
-        os.makedirs( path_folder, exist_ok = True )
-
-    # align and create gene count matrix for each sample
-    dict_name_organism_to_dict_it = dict( )
-    for name_sample, path_file_fq in bk.GLOB_Retrive_Strings_in_Wildcards( f'{path_folder_pipeline}*.fastq.gz' ).values :
-        name_organism = dict_name_sample_to_organism[ name_sample ] # retrieve the name of the organism
-        dict_anno_for_sample = dict_anno[ name_organism ] # retrieve annotation for the sample
+    for path_folder in [
+        f"{path_folder_pipeline}minimap2/genome/",
+        f"{path_folder_pipeline}minimap2/transcriptome/",
+    ]:
+        os.makedirs(path_folder, exist_ok=True)
+
+    # align reads
+    import concurrent.futures
+
+    l_task = []  # initialize the list of tasks
+    int_num_cpus_for_each_alignment = min(
+        1, int(int_num_cpus / int_num_samples / 2)
+    )  # retrieve approximate number of cpus for each alignment
+    for name_sample, path_file_fq in df_fastq.values:  # for each sample
+        name_organism = dict_name_sample_to_organism[
+            name_sample
+        ]  # retrieve the name of the organism
+        dict_anno_for_sample = dict_anno[
+            name_organism
+        ]  # retrieve annotation for the sample
         # align each sample for genome and transcriptome
-        for minimap2_index, path_folder_minimap2_output in zip(
-            [ dict_anno_for_sample[ 'index_genome' ], dict_anno_for_sample[ 'index_transcriptome' ] ],
-            [ f'{path_folder_pipeline}minimap2/genome/', f'{path_folder_pipeline}minimap2/transcriptome/' ]
-        ) : 
-            Minimap2_Align( 
-                flag_use_split_prefix = False, 
-                path_file_fastq = path_file_fq, 
-                path_file_minimap2_index = minimap2_index, 
-                path_folder_minimap2_output = path_folder_minimap2_output, 
-                n_threads = int_num_cpus, 
-                drop_unaligned = False, 
-                return_bash_shellscript = False
-            )
+        l_task.extend(
+            [
+                [
+                    path_file_fq,
+                    dict_anno_for_sample["index_genome"],
+                    f"{path_folder_pipeline}minimap2/genome/",
+                    int_num_cpus_for_each_alignment,
+                    dict_anno_for_sample["splice_junc"],
+                ],  # genome
+                [
+                    path_file_fq,
+                    dict_anno_for_sample["index_transcriptome"],
+                    f"{path_folder_pipeline}minimap2/transcriptome/",
+                    int_num_cpus_for_each_alignment,
+                    None,
+                ],  # transcriptome
+            ]
+        )
+    with concurrent.futures.ProcessPoolExecutor() as executor:  # create an executer
+        for res in executor.map(
+            __create_gene_count_from_fast5__align, l_task
+        ):  # perform each task
+            pass
 
+    # analyze the BAM files and create gene count matrix for each sample
+    dict_name_organism_to_dict_it = dict()
+    for name_sample, path_file_fq in df_fastq.values:  # for each sample
         # retrieve interval tree for the gene annotations
-        if name_organism not in dict_name_organism_to_dict_it :
-            dict_name_organism_to_dict_it[ name_organism ] = bk.GTF_Interval_Tree(
-                dict_anno_for_sample[ 'gtf_ref' ],
-                feature = [ 'gene' ],
-                value = 'gene_name',
+        if name_organism not in dict_name_organism_to_dict_it:
+            dict_name_organism_to_dict_it[name_organism] = bk.GTF_Interval_Tree(
+                dict_anno_for_sample["gtf_ref"],
+                feature=["gene"],
+                value="gene_name",
             )
-        dict_it = dict_name_organism_to_dict_it[ name_organism ]
+        dict_it = dict_name_organism_to_dict_it[name_organism]
 
         # summarize fastq files
         int_read_count = 0
         int_base_pair_count = 0
-        for name_record, seq, _, qual in bk.FASTQ_Iterate( path_file_fq ) :
+        for name_record, seq, _, qual in bk.FASTQ_Iterate(path_file_fq):
             int_read_count += 1
-            int_base_pair_count += len( seq )
-        
+            int_base_pair_count += len(seq)
+
         # calculate gene count, read length, and average mapping quality from the aligned reads
-        l_l = [ ]
-        with pysam.AlignmentFile( f'{path_folder_pipeline}minimap2/genome/{name_sample}.fastq.gz.minimap2_aligned.bam' ) as samfile :
-            for r in samfile.fetch( ) :
+        l_l = []
+        with pysam.AlignmentFile(
+            f"{path_folder_pipeline}minimap2/genome/{name_sample}.fastq.gz.minimap2_aligned.bam"
+        ) as samfile:
+            for r in samfile.fetch():
                 # skip invalid reads
-                if r.seq is None :
+                if r.seq is None:
                     continue
-                if r.mapq == 0 :
+                if r.mapq == 0:
                     continue
-                if r.reference_name not in dict_it :
+                if r.reference_name not in dict_it:
                     continue
 
-                l_name_gene_for_current_read = list( i[ 2 ] for i in dict_it[ r.reference_name ][ r.reference_start : r.reference_end ] ) # retrieve a list of matching gene_names
-
-                if len( l_name_gene_for_current_read ) == 0 : # if no gene were assigned, does not count the read
+                l_name_gene_for_current_read = list(
+                    i[2]
+                    for i in dict_it[r.reference_name][
+                        r.reference_start : r.reference_end
+                    ]
+                )  # retrieve a list of matching gene_names
+
+                if (
+                    len(l_name_gene_for_current_read) == 0
+                ):  # if no gene were assigned, does not count the read
                     continue
-                elif len( l_name_gene_for_current_read ) == 1 : # if a single gene is assigned.
-                    name_gene = l_name_gene_for_current_read[ 0 ]
-                else : # if more than one gene is assigned, randomly select one of the name_gene and assign it to the read
-                    name_gene = l_name_gene_for_current_read[ math.floor( np.random.random( ) * len( l_name_gene_for_current_read ) ) ]
-                l_l.append( [
-                    name_gene,
-                    len( r.seq ),
-                    r.mapq,
-                ] ) # collect the record
+                elif (
+                    len(l_name_gene_for_current_read) == 1
+                ):  # if a single gene is assigned.
+                    name_gene = l_name_gene_for_current_read[0]
+                else:  # if more than one gene is assigned, randomly select one of the name_gene and assign it to the read
+                    name_gene = l_name_gene_for_current_read[
+                        math.floor(
+                            np.random.random() * len(l_name_gene_for_current_read)
+                        )
+                    ]
+                l_l.append(
+                    [
+                        name_gene,
+                        len(r.seq),
+                        r.mapq,
+                    ]
+                )  # collect the record
 
         # compose dataframe of reads
-        df = pd.DataFrame( l_l, columns = [ 'gene_name', 'length_of_read', 'mapping_quality' ] )
-        df[ 'gene_count' ] = 1
+        df = pd.DataFrame(
+            l_l, columns=["gene_name", "length_of_read", "mapping_quality"]
+        )
+        df["gene_count"] = 1
         # calculate unaligned read count and base count
-        int_read_count_unaligned = int_read_count - len( df )
-        int_base_pair_count_unaligned = int_base_pair_count - df.length_of_read.sum( )
+        int_read_count_unaligned = int_read_count - len(df)
+        int_base_pair_count_unaligned = int_base_pair_count - df.length_of_read.sum()
 
         # compose dataframe of genes
-        df = pd.DataFrame( {
-            'gene_count' : df[ [ 'gene_name', 'gene_count', ] ].groupby( 'gene_name' ).count( )[ 'gene_count' ], # calculate 'gene_count'
-            'average_length_of_read' : df[ [ 'gene_name', 'length_of_read', ] ].groupby( 'gene_name' ).mean( )[ 'length_of_read' ], # calculate 'average_length_of_read'
-            'average_mapping_quality' : df[ [ 'gene_name', 'mapping_quality', ] ].groupby( 'gene_name' ).mean( )[ 'mapping_quality' ], # calculate 'average_mapping_quality'
-        } )
-        df.loc[ '__unaligned_reads__' ] = [ int_read_count_unaligned, int_base_pair_count_unaligned / int_read_count_unaligned, -1 ] # add record of unaligned reads
-        df.sort_values( 'gene_count', ascending = False, inplace = True ) # sort by gene_count
+        df = pd.DataFrame(
+            {
+                "gene_count": df[
+                    [
+                        "gene_name",
+                        "gene_count",
+                    ]
+                ]
+                .groupby("gene_name")
+                .count()["gene_count"],  # calculate 'gene_count'
+                "average_length_of_read": df[
+                    [
+                        "gene_name",
+                        "length_of_read",
+                    ]
+                ]
+                .groupby("gene_name")
+                .mean()["length_of_read"],  # calculate 'average_length_of_read'
+                "average_mapping_quality": df[
+                    [
+                        "gene_name",
+                        "mapping_quality",
+                    ]
+                ]
+                .groupby("gene_name")
+                .mean()["mapping_quality"],  # calculate 'average_mapping_quality'
+            }
+        )
+        df.loc["__unaligned_reads__"] = [
+            int_read_count_unaligned,
+            int_base_pair_count_unaligned / int_read_count_unaligned,
+            -1,
+        ]  # add record of unaligned reads
+        df.sort_values(
+            "gene_count", ascending=False, inplace=True
+        )  # sort by gene_count
 
         # write result as files
-        df.to_excel( f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.xlsx" ) # output excel file
-        df.to_csv( f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.tsv.gz", sep = '\t' ) # output tsv file
-
-def Guppy_Run_and_Combine_Output( path_folder_nanopore_sequencing_data = None, flag_barcoding_was_used = False, path_folder_output_fastq = None, id_flowcell = None, id_lib_prep = None, id_barcoding_kit = None, flag_use_cpu = True, int_n_threads = 18, flag_read_splitting = False ) :
+        df.to_excel(
+            f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.xlsx"
+        )  # output excel file
+        df.to_csv(
+            f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.tsv.gz",
+            sep="\t",
+        )  # output tsv file
+
+
+def Guppy_Run_and_Combine_Output(
+    path_folder_nanopore_sequencing_data=None,
+    flag_barcoding_was_used=False,
+    path_folder_output_fastq=None,
+    id_flowcell=None,
+    id_lib_prep=None,
+    id_barcoding_kit=None,
+    flag_use_cpu=True,
+    int_n_threads=18,
+    flag_read_splitting=False,
+):
     """
-    # 2023-01-27 23:38:33 
-    Run Guppy basecaller on the nanopore sequencing datafiles in the given folder 
+    # 2023-01-27 23:38:33
+    Run Guppy basecaller on the nanopore sequencing datafiles in the given folder
     Automatically detect 'id_flowcell' and 'id_lib_prep' from the metadata saved in the folder (they can be manually set through arguments)
-    
+
     'path_folder_nanopore_sequencing_data' : Run Guppy basecaller on the nanopore sequencing datafiles in the given folder. a list of nanopore sequencing datafolders of multiple runs of the same sample (due to failed runs, etc.) can be also given
     'flag_barcoding_was_used' : flag of whether a barcoding kit was used during sequencing
     'id_flowcell' : manually set 'id_flowcell' for guppy_bascaller run.
     'id_lib_prep' : manually set 'id_lib_prep' for guppy_bascaller run.
     'id_barcoding_kit' : manually set 'id_barcoding_kit' for guppy_bascaller run.
     'flag_use_cpu' : use CPU
-    'int_n_threads' : number of CPU threads to use 
+    'int_n_threads' : number of CPU threads to use
     """
 
-    
-    flag_entry_point = PKG.Detect_Entry_Point( 'biobook' ) # detect whether an entry point was used
-    if flag_entry_point :
-        parser = argparse.ArgumentParser( description = "Run Guppy basecaller on the nanopore sequencing datafiles in the given folder . This program has been developed by Hyunsu An (2021/06/03)." )
-        parser.add_argument( 'path_folder_nanopore_sequencing_data', metavar = 'path_folder_nanopore_sequencing_data', type = str, nargs='+', help = '(Required) the nanopore sequencing data folder(s)' )
-        parser.add_argument( "-b", "--flag_barcoding_was_used", help = "Set a flag indicating a barcoding kit was used during sequencing", action = 'store_true' )
-        parser.add_argument( "-o", "--path_folder_output_fastq", help = "(optional) copy fastq files in the guppy output folder to the given directory" )
-        parser.add_argument( "-F", "--id_flowcell", help = "(optional) explicitly define the flowcell type used in sequencing. e.g. FLO-MIN106" )
-        parser.add_argument( "-L", "--id_lib_prep", help = "(optional) explicitly define the library sequencing kit used in sequencing. e.g. SQK-LSK109" )
-        parser.add_argument( "-B", "--id_barcoding_kit", help = "(optional) explicitly define the library barcoding kit used in sequencing. e.g. EXP-NBD104" )
-        parser.add_argument( "-C", "--flag_use_cpu", help = "(optional) use CPU only (use when GPU is not available)", action = 'store_true' )
-        parser.add_argument( "-S", "--flag_read_splitting", help = "(optional) perform read splitting by using the Guppy 6's optional argument", action = 'store_true' )
-        parser.add_argument( "-t", "--int_n_threads", help = "(default: 18) number of CPU threads to use", default = '18' )
-        args = parser.parse_args( )
+    flag_entry_point = PKG.Detect_Entry_Point(
+        "biobook"
+    )  # detect whether an entry point was used
+    if flag_entry_point:
+        parser = argparse.ArgumentParser(
+            description="Run Guppy basecaller on the nanopore sequencing datafiles in the given folder . This program has been developed by Hyunsu An (2021/06/03)."
+        )
+        parser.add_argument(
+            "path_folder_nanopore_sequencing_data",
+            metavar="path_folder_nanopore_sequencing_data",
+            type=str,
+            nargs="+",
+            help="(Required) the nanopore sequencing data folder(s)",
+        )
+        parser.add_argument(
+            "-b",
+            "--flag_barcoding_was_used",
+            help="Set a flag indicating a barcoding kit was used during sequencing",
+            action="store_true",
+        )
+        parser.add_argument(
+            "-o",
+            "--path_folder_output_fastq",
+            help="(optional) copy fastq files in the guppy output folder to the given directory",
+        )
+        parser.add_argument(
+            "-F",
+            "--id_flowcell",
+            help="(optional) explicitly define the flowcell type used in sequencing. e.g. FLO-MIN106",
+        )
+        parser.add_argument(
+            "-L",
+            "--id_lib_prep",
+            help="(optional) explicitly define the library sequencing kit used in sequencing. e.g. SQK-LSK109",
+        )
+        parser.add_argument(
+            "-B",
+            "--id_barcoding_kit",
+            help="(optional) explicitly define the library barcoding kit used in sequencing. e.g. EXP-NBD104",
+        )
+        parser.add_argument(
+            "-C",
+            "--flag_use_cpu",
+            help="(optional) use CPU only (use when GPU is not available)",
+            action="store_true",
+        )
+        parser.add_argument(
+            "-S",
+            "--flag_read_splitting",
+            help="(optional) perform read splitting by using the Guppy 6's optional argument",
+            action="store_true",
+        )
+        parser.add_argument(
+            "-t",
+            "--int_n_threads",
+            help="(default: 18) number of CPU threads to use",
+            default="18",
+        )
+        args = parser.parse_args()
 
         # [input] parse arguments from parse_args
         path_folder_nanopore_sequencing_data = args.path_folder_nanopore_sequencing_data
         flag_barcoding_was_used = args.flag_barcoding_was_used
         path_folder_output_fastq = args.path_folder_output_fastq
         id_flowcell = args.id_flowcell
         id_lib_prep = args.id_lib_prep
         id_barcoding_kit = args.id_barcoding_kit
         flag_use_cpu = args.flag_use_cpu
-        int_n_threads = int( args.int_n_threads )
+        int_n_threads = int(args.int_n_threads)
         flag_read_splitting = args.flag_read_splitting
-        
-    
-    ''' [parse arguments] '''
-    if path_folder_nanopore_sequencing_data is None :
-        print( "required arguments are not given, exiting" )
-        if flag_entry_point :
-            sys.exit( ) 
-        else :
+
+    """ [parse arguments] """
+    if path_folder_nanopore_sequencing_data is None:
+        print("required arguments are not given, exiting")
+        if flag_entry_point:
+            sys.exit()
+        else:
             return -1
-    
+
     # process path_folder in 'l_path_folder_nanopore_sequencing_data'
-    l_path_folder_nanopore_sequencing_data = path_folder_nanopore_sequencing_data if isinstance( path_folder_nanopore_sequencing_data, ( list ) ) else [ path_folder_nanopore_sequencing_data ] # set 'l_path_folder_nanopore_sequencing_data' according to the given 'path_folder_nanopore_sequencing_data'
-    l = [ ]
-    for path_folder in l_path_folder_nanopore_sequencing_data :
-        path_folder = os.path.abspath( path_folder )
-        if path_folder[ -1 ] != '/' : # add '/' to the end of the directory
-            path_folder += '/'
-        l.append( path_folder )
+    l_path_folder_nanopore_sequencing_data = (
+        path_folder_nanopore_sequencing_data
+        if isinstance(path_folder_nanopore_sequencing_data, (list))
+        else [path_folder_nanopore_sequencing_data]
+    )  # set 'l_path_folder_nanopore_sequencing_data' according to the given 'path_folder_nanopore_sequencing_data'
+    l = []
+    for path_folder in l_path_folder_nanopore_sequencing_data:
+        path_folder = os.path.abspath(path_folder)
+        if path_folder[-1] != "/":  # add '/' to the end of the directory
+            path_folder += "/"
+        l.append(path_folder)
     l_path_folder_nanopore_sequencing_data = l
     # process 'path_folder_output_fastq'
-    if path_folder_output_fastq is not None : # if output folder of fastq files was given
-        path_folder_output_fastq = os.path.abspath( path_folder_output_fastq )
-        if path_folder_output_fastq[ -1 ] != '/' : # add '/' to the end of the directory
-            path_folder_output_fastq += '/'
-            
-            
+    if (
+        path_folder_output_fastq is not None
+    ):  # if output folder of fastq files was given
+        path_folder_output_fastq = os.path.abspath(path_folder_output_fastq)
+        if path_folder_output_fastq[-1] != "/":  # add '/' to the end of the directory
+            path_folder_output_fastq += "/"
+
     """ run Guppy basecaller for each nanopore sequencing data folder """
-    set_path_file_fastq_gz = set( ) # a set of output fastq files
-    for path_folder_nanopore_sequencing_data in l_path_folder_nanopore_sequencing_data : 
+    set_path_file_fastq_gz = set()  # a set of output fastq files
+    for path_folder_nanopore_sequencing_data in l_path_folder_nanopore_sequencing_data:
         # [input] parse arguments
-        path_folder_nanopore_sequencing_data = os.path.abspath( path_folder_nanopore_sequencing_data )
-        if path_folder_nanopore_sequencing_data[ -1 ] != '/' : # add '/' to the end of the directory
-            path_folder_nanopore_sequencing_data += '/'
+        path_folder_nanopore_sequencing_data = os.path.abspath(
+            path_folder_nanopore_sequencing_data
+        )
+        if (
+            path_folder_nanopore_sequencing_data[-1] != "/"
+        ):  # add '/' to the end of the directory
+            path_folder_nanopore_sequencing_data += "/"
 
         # define and create a folder for all fast5 files
-        path_folder_fast5 = path_folder_nanopore_sequencing_data + 'fast5/'
-        if not os.path.exists( path_folder_fast5 ) : # if the folder already exists, skip moving fast5 files to a single folder (when fast-bascalling option has not been turned on, fast5 folder is present)
-            os.makedirs( path_folder_fast5, exist_ok = True )
+        path_folder_fast5 = path_folder_nanopore_sequencing_data + "fast5/"
+        if not os.path.exists(
+            path_folder_fast5
+        ):  # if the folder already exists, skip moving fast5 files to a single folder (when fast-bascalling option has not been turned on, fast5 folder is present)
+            os.makedirs(path_folder_fast5, exist_ok=True)
             # move all fast5 files into one folder
-            l_path_file = glob.glob( f"{path_folder_nanopore_sequencing_data}*/*fast5" ) + glob.glob( f"{path_folder_nanopore_sequencing_data}*/*/*fast5" ) # retrieve fast5 files
-            for path_file in l_path_file : # no barcoding
-                shutil.copyfile( path_file, path_folder_fast5 + path_file.rsplit( '/', 1 )[ 1 ] )
+            l_path_file = glob.glob(
+                f"{path_folder_nanopore_sequencing_data}*/*fast5"
+            ) + glob.glob(
+                f"{path_folder_nanopore_sequencing_data}*/*/*fast5"
+            )  # retrieve fast5 files
+            for path_file in l_path_file:  # no barcoding
+                shutil.copyfile(
+                    path_file, path_folder_fast5 + path_file.rsplit("/", 1)[1]
+                )
         # retrieve flowcell type and library preperation method using summary file inside the directory
 
-        if id_flowcell is None or id_lib_prep is None :
-            l = glob.glob( f"{path_folder_nanopore_sequencing_data}final_summary_*.txt" )
-            if len( l ) > 0 : 
-                with open( l[ 0 ] ) as file :
-                    content = file.read( ).strip( )
-                    l_line = content.split( '\n' )
-                if 'FLO-MIN114' in content : # 10.4.1 moter speed option
-                    _, id_flowcell, id_lib_prep, str_moter_speed = list( line.split( 'protocol=' )[ 1 ].split( ':' ) for line in l_line if 'protocol=' == line[ : len( 'protocol=' ) ] )[ 0 ] # retrieve flowcell type and library preperation method using summary file inside the directory
-                else :
-                    _, id_flowcell, id_lib_prep = list( line.split( 'protocol=' )[ 1 ].split( ':' ) for line in l_line if 'protocol=' == line[ : len( 'protocol=' ) ] )[ 0 ] # retrieve flowcell type and library preperation method using summary file inside the directory
-            
-            if id_flowcell is None or id_lib_prep is None :
-                l = glob.glob( f"{path_folder_nanopore_sequencing_data}report_*.md" ) # retry
-                if len( l ) > 0 : 
-                    with open( l[ 0 ] ) as file :
-                        l_line = file.read( ).strip( ).split( '\n' )
-                    _, id_flowcell, id_lib_prep = list( e.replace( '",', '' ) for e in list( line.split( '"exp_script_name":' )[ 1 ].split( ':' ) for line in l_line if '"exp_script_name":' in line )[ 0 ] ) # retrieve flowcell type and library preperation method using summary file inside the directory
-                else :
-                    print( "[Guppy_Run_and_Combine_Output] appropriate 'id_flowcell' and/or 'id_lib_prep' were not found, exiting" )
-                    return -1 
-        ''' run guppy basecaller and write output as a text file '''
+        if id_flowcell is None or id_lib_prep is None:
+            l = glob.glob(f"{path_folder_nanopore_sequencing_data}final_summary_*.txt")
+            if len(l) > 0:
+                with open(l[0]) as file:
+                    content = file.read().strip()
+                    l_line = content.split("\n")
+                if "FLO-MIN114" in content:  # 10.4.1 moter speed option
+                    _, id_flowcell, id_lib_prep, str_moter_speed = list(
+                        line.split("protocol=")[1].split(":")
+                        for line in l_line
+                        if "protocol=" == line[: len("protocol=")]
+                    )[
+                        0
+                    ]  # retrieve flowcell type and library preperation method using summary file inside the directory
+                else:
+                    _, id_flowcell, id_lib_prep = list(
+                        line.split("protocol=")[1].split(":")
+                        for line in l_line
+                        if "protocol=" == line[: len("protocol=")]
+                    )[
+                        0
+                    ]  # retrieve flowcell type and library preperation method using summary file inside the directory
+
+            if id_flowcell is None or id_lib_prep is None:
+                l = glob.glob(
+                    f"{path_folder_nanopore_sequencing_data}report_*.md"
+                )  # retry
+                if len(l) > 0:
+                    with open(l[0]) as file:
+                        l_line = file.read().strip().split("\n")
+                    _, id_flowcell, id_lib_prep = list(
+                        e.replace('",', "")
+                        for e in list(
+                            line.split('"exp_script_name":')[1].split(":")
+                            for line in l_line
+                            if '"exp_script_name":' in line
+                        )[0]
+                    )  # retrieve flowcell type and library preperation method using summary file inside the directory
+                else:
+                    print(
+                        "[Guppy_Run_and_Combine_Output] appropriate 'id_flowcell' and/or 'id_lib_prep' were not found, exiting"
+                    )
+                    return -1
+        """ run guppy basecaller and write output as a text file """
         path_folder_guppy_output = f"{path_folder_nanopore_sequencing_data}guppy_out/"
-        if not os.path.exists( path_folder_guppy_output ) :
+        if not os.path.exists(path_folder_guppy_output):
             # compose guppy basecaller arguments
-            l_args = [ 'guppy_basecaller' ] 
-            if not flag_use_cpu : # use GPU if it exists
-                l_args += [ '--device', 'auto' ]
-            if flag_read_splitting :
-                l_args += [ '--do_read_splitting' ] 
-            l_args += [ '--cpu_threads_per_caller', str( int_n_threads ) ]
-
-            if id_lib_prep == 'SQK-RBK096' : # change 'id_lib_prep' to guppy-compatible id
-                id_lib_prep = 'SQK-RBK110-96'
-            if flag_barcoding_was_used :
-                ''' automatically set barcoding_kit '''
-                if id_barcoding_kit is None :
-                    id_barcoding_kit = "EXP-NBD104 EXP-NBD114" if 'LSK' in id_lib_prep else id_lib_prep
-                print( ' '.join( l_args + [ "--flowcell", id_flowcell, "--kit", id_lib_prep, "--barcode_kits", id_barcoding_kit, "--compress_fastq", "--input_path", path_folder_fast5, "--save_path", path_folder_guppy_output ] ) )  
-                run_guppy = subprocess.run( l_args + [ "--flowcell", id_flowcell, "--kit", id_lib_prep, "--barcode_kits", id_barcoding_kit, "--compress_fastq", "--input_path", path_folder_fast5, "--save_path", path_folder_guppy_output ], capture_output = True )
-            else :
-                run_guppy = subprocess.run( l_args + [ "--flowcell", id_flowcell, "--kit", id_lib_prep, "--compress_fastq", "--input_path", path_folder_fast5, "--save_path", path_folder_guppy_output ], capture_output = True )
-            with open( path_folder_nanopore_sequencing_data + 'guppy_basecaller.out', 'w' ) as file :
-                file.write( run_guppy.stdout.decode( ) )
-        
-        ''' combine fastq.gz output files of guppy_basecaller output '''
-        if flag_barcoding_was_used :
-            for path_folder_barcode in glob.glob( path_folder_guppy_output + 'pass/*/' ) + glob.glob( path_folder_guppy_output + 'fail/*/' ) :
-                name_barcode = path_folder_barcode.rsplit( '/', 2 )[ 1 ] # retrieve barcode name from the path
-                path_file_fastq_gz = f"{path_folder_guppy_output}{name_barcode}.fastq.gz"
-                OS_FILE_Combine_Files_in_order( list( glob.glob( f"{path_folder_guppy_output}*/{name_barcode}/*" + '*fastq.gz' ) ), path_file_fastq_gz, flag_bgzip_output = False ) # combine fastq files
-                set_path_file_fastq_gz.add( path_file_fastq_gz )
-        else :
+            l_args = ["guppy_basecaller"]
+            if not flag_use_cpu:  # use GPU if it exists
+                l_args += ["--device", "auto"]
+            if flag_read_splitting:
+                l_args += ["--do_read_splitting"]
+            l_args += ["--cpu_threads_per_caller", str(int_n_threads)]
+
+            if (
+                id_lib_prep == "SQK-RBK096"
+            ):  # change 'id_lib_prep' to guppy-compatible id
+                id_lib_prep = "SQK-RBK110-96"
+            if flag_barcoding_was_used:
+                """automatically set barcoding_kit"""
+                if id_barcoding_kit is None:
+                    id_barcoding_kit = (
+                        "EXP-NBD104 EXP-NBD114" if "LSK" in id_lib_prep else id_lib_prep
+                    )
+                print(
+                    " ".join(
+                        l_args
+                        + [
+                            "--flowcell",
+                            id_flowcell,
+                            "--kit",
+                            id_lib_prep,
+                            "--barcode_kits",
+                            id_barcoding_kit,
+                            "--compress_fastq",
+                            "--input_path",
+                            path_folder_fast5,
+                            "--save_path",
+                            path_folder_guppy_output,
+                        ]
+                    )
+                )
+                run_guppy = subprocess.run(
+                    l_args
+                    + [
+                        "--flowcell",
+                        id_flowcell,
+                        "--kit",
+                        id_lib_prep,
+                        "--barcode_kits",
+                        id_barcoding_kit,
+                        "--compress_fastq",
+                        "--input_path",
+                        path_folder_fast5,
+                        "--save_path",
+                        path_folder_guppy_output,
+                    ],
+                    capture_output=True,
+                )
+            else:
+                run_guppy = subprocess.run(
+                    l_args
+                    + [
+                        "--flowcell",
+                        id_flowcell,
+                        "--kit",
+                        id_lib_prep,
+                        "--compress_fastq",
+                        "--input_path",
+                        path_folder_fast5,
+                        "--save_path",
+                        path_folder_guppy_output,
+                    ],
+                    capture_output=True,
+                )
+            with open(
+                path_folder_nanopore_sequencing_data + "guppy_basecaller.out", "w"
+            ) as file:
+                file.write(run_guppy.stdout.decode())
+
+        """ combine fastq.gz output files of guppy_basecaller output """
+        if flag_barcoding_was_used:
+            for path_folder_barcode in glob.glob(
+                path_folder_guppy_output + "pass/*/"
+            ) + glob.glob(path_folder_guppy_output + "fail/*/"):
+                name_barcode = path_folder_barcode.rsplit("/", 2)[
+                    1
+                ]  # retrieve barcode name from the path
+                path_file_fastq_gz = (
+                    f"{path_folder_guppy_output}{name_barcode}.fastq.gz"
+                )
+                OS_FILE_Combine_Files_in_order(
+                    list(
+                        glob.glob(
+                            f"{path_folder_guppy_output}*/{name_barcode}/*"
+                            + "*fastq.gz"
+                        )
+                    ),
+                    path_file_fastq_gz,
+                    flag_bgzip_output=False,
+                )  # combine fastq files
+                set_path_file_fastq_gz.add(path_file_fastq_gz)
+        else:
             path_file_fastq_gz = f"{path_folder_guppy_output}guppy_basecalled.fastq.gz"
-            OS_FILE_Combine_Files_in_order( list( glob.glob( path_folder_guppy_output + '*fastq.gz' ) ), path_file_fastq_gz, flag_bgzip_output = False ) # combine fastq files
-            set_path_file_fastq_gz.add( path_file_fastq_gz )
-    ''' copy and combine output fastq files to the output directory '''
-    if path_folder_output_fastq is not None : # if output folder of fastq files was given
-        # group 'path_file_fastq_gz' based on 'name_file' 
-        
-        dict_name_file_to_dir = dict( )
-        for d in set_path_file_fastq_gz :
-            name_file = d.rsplit( '/', 1 )[ 1 ] 
-            if name_file not in dict_name_file_to_dir :
-                dict_name_file_to_dir[ name_file ] = [ ]
-            dict_name_file_to_dir[ name_file ].append( d )
-        
-        for name_file in dict_name_file_to_dir : # for each output 'name_file' (barcodes), combine and copy the file to the given output folder
-            l_path_file = dict_name_file_to_dir[ name_file ] # retrieve list of file path of the current barcode
-            if len( l_path_file ) == 1 : # when only single file exist for the current barcode , simply copy the file to the output 
-                OS_Run( [ 'cp', l_path_file[ 0 ], f"{path_folder_output_fastq}{name_file}" ] )
-            else : # combine files 
-                OS_FILE_Combine_Files_in_order( l_path_file, f"{path_folder_output_fastq}{name_file}", flag_bgzip_output = False ) # 
-        
-def Minimap2_Align( path_file_fastq, path_file_minimap2_index = '/node210data/shared/ensembl/Mus_musculus/index/minimap2/Mus_musculus.GRCm38.dna.primary_assembly.k_14.idx', path_folder_minimap2_output = None, n_threads = 20, verbose = True, drop_unaligned = False, return_bash_shellscript = False, n_threads_for_sort = 1, flag_use_split_prefix : bool = False ) :
-    """ 
-    # 2022-09-24 19:15:33 
-    align given fastq file of nanopore reads using minimap2 and write an output as a bam file 
+            OS_FILE_Combine_Files_in_order(
+                list(glob.glob(path_folder_guppy_output + "*fastq.gz")),
+                path_file_fastq_gz,
+                flag_bgzip_output=False,
+            )  # combine fastq files
+            set_path_file_fastq_gz.add(path_file_fastq_gz)
+    """ copy and combine output fastq files to the output directory """
+    if (
+        path_folder_output_fastq is not None
+    ):  # if output folder of fastq files was given
+        # group 'path_file_fastq_gz' based on 'name_file'
+
+        dict_name_file_to_dir = dict()
+        for d in set_path_file_fastq_gz:
+            name_file = d.rsplit("/", 1)[1]
+            if name_file not in dict_name_file_to_dir:
+                dict_name_file_to_dir[name_file] = []
+            dict_name_file_to_dir[name_file].append(d)
+
+        for (
+            name_file
+        ) in (
+            dict_name_file_to_dir
+        ):  # for each output 'name_file' (barcodes), combine and copy the file to the given output folder
+            l_path_file = dict_name_file_to_dir[
+                name_file
+            ]  # retrieve list of file path of the current barcode
+            if (
+                len(l_path_file) == 1
+            ):  # when only single file exist for the current barcode , simply copy the file to the output
+                OS_Run(["cp", l_path_file[0], f"{path_folder_output_fastq}{name_file}"])
+            else:  # combine files
+                OS_FILE_Combine_Files_in_order(
+                    l_path_file,
+                    f"{path_folder_output_fastq}{name_file}",
+                    flag_bgzip_output=False,
+                )  #
+
+
+def Minimap2_Align(
+    path_file_fastq,
+    path_file_minimap2_index="/node210data/shared/ensembl/Mus_musculus/index/minimap2/Mus_musculus.GRCm38.dna.primary_assembly.k_14.idx",
+    path_folder_minimap2_output=None,
+    n_threads=20,
+    verbose=True,
+    drop_unaligned=False,
+    return_bash_shellscript=False,
+    n_threads_for_sort=10,
+    flag_use_split_prefix: bool = False,
+    path_file_junc_bed: Union[
+        None, str
+    ] = None,  # if given, the bed file will be used for prioritizing known splice sites.
+    path_file_gtf: Union[
+        None, str
+    ] = None,  # path to gene and exon annotation files, required if 'path_file_junc_bed' is given but the file does not exist
+):
+    """
+    # 2023-04-23 01:18:58
+    align given fastq file of nanopore reads using minimap2 and write an output as a bam file
     'path_file_fastq' : input fastq or fasta file (gzipped or uncompressed file is accepted)
     'path_file_minimap2_index' : minimap2 index file
     'path_folder_minimap2_output' : minimap2 output folder
     'drop_unaligned' : a flag indicating whether reads not aligned to the reference ('SAM flag == 4') are included in the output bam file
     'return_bash_shellscript' : return shellscript instead of running minimap2 using the subprocess module
     'flag_use_split_prefix' = False # for large index, split-prefix should be used
     """
-    path_folder_fastq, name_file_fastq = path_file_fastq.rsplit( '/', 1 )
-    if path_folder_minimap2_output is None : # default output folder is a subdirectory of the folder containing the input fastq file
-        path_folder_minimap2_output = f'{path_folder_fastq}/minimap2/'
-    if path_folder_minimap2_output[ -1 ] != '/' : # add '/' at the end of the output directory if it does not exist
-        path_folder_minimap2_output += '/'
-    os.makedirs( path_folder_minimap2_output, exist_ok = True ) # create folder if it does not exist
-
-    path_file_sam = f"{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.sam"
-    path_file_bam = f"{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.bam"
-    
-    l_bash_shellscript = [ ]
-    
-    ''' perform minimap2 alignment '''
-    l_arg = [ 'minimap2', '-t', str( int( n_threads ) ), '-ax', 'splice', "-o", path_file_sam ] 
-    
+    path_folder_fastq, name_file_fastq = path_file_fastq.rsplit("/", 1)
+    if (
+        path_folder_minimap2_output is None
+    ):  # default output folder is a subdirectory of the folder containing the input fastq file
+        path_folder_minimap2_output = f"{path_folder_fastq}/minimap2/"
+    if (
+        path_folder_minimap2_output[-1] != "/"
+    ):  # add '/' at the end of the output directory if it does not exist
+        path_folder_minimap2_output += "/"
+    os.makedirs(
+        path_folder_minimap2_output, exist_ok=True
+    )  # create folder if it does not exist
+
+    path_file_sam = (
+        f"{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.sam"
+    )
+    path_file_bam = (
+        f"{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.bam"
+    )
+
+    l_bash_shellscript = []
+
+    """ perform minimap2 alignment """
+    l_arg = [
+        "minimap2",
+        "-t",
+        str(int(n_threads)),
+        "-ax",
+        "splice",
+        "-o",
+        path_file_sam,
+    ]
+
     # for large index, split-prefix should be used
-    if flag_use_split_prefix :
-        l_arg += [ f'--split-prefix={path_folder_minimap2_output}{UUID( )}' ]
-    
-    if drop_unaligned :
-        l_arg += [ '--sam-hit-only' ]
-    l_arg += [ path_file_minimap2_index, path_file_fastq ]
-    if return_bash_shellscript : # perform minimap2 alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-    else :
-        run = subprocess.run( l_arg, capture_output = True )
-        with open( f'{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.out', 'w' ) as file :
-            file.write( run.stdout.decode( ) )
-        if verbose :
-            print( 'minimap2 completed' )
-            
-    ''' sort output SAM file '''
-    l_arg = [ 'samtools', 'sort', '-@', str( int( min( n_threads_for_sort, 10 ) ) ), '-O', "BAM", '-o', path_file_bam, path_file_sam ]
-    if return_bash_shellscript : # perform minimap2 alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-        l_bash_shellscript.append( ' '.join( [ 'rm', '-f', path_file_sam ] ) )
-    else :     
-        run = subprocess.run( l_arg, capture_output = False )
-        os.remove( path_file_sam ) # remove sam file
-        
-    ''' index resulting BAM file '''
-    l_arg = [ 'samtools', 'index', path_file_bam ]
-    if return_bash_shellscript : # perform minimap2 alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-    else :   
-        run = subprocess.run( l_arg, capture_output = False )
-        if verbose :
-            print( 'samtools bam file compressing and indexing completed' )
-    
-    if return_bash_shellscript : # retrun bash shell scripts
-        return ' && '.join( l_bash_shellscript )
-    
-def Minimap2_Index( path_file_fasta, path_file_minimap2_index = None, verbose = False ) :
-    """ 
-    # 2021-03-24 00:44:51 
+    if flag_use_split_prefix:
+        l_arg += [f"--split-prefix={path_folder_minimap2_output}{UUID( )}"]
+
+    if path_file_junc_bed is not None:
+        if (
+            not os.path.exists(path_file_junc_bed) and path_file_gtf is not None
+        ):  # if the bed file does not exist, create the bed file using paftools.js, packaged with the minimap2 executable
+            l_args_for_creating_junc_bed = ["paftools.js", "gff2bed", path_file_gtf]
+            if (
+                return_bash_shellscript
+            ):  # perform minimap2 alignment using subprocess module
+                l_bash_shellscript.append(
+                    " ".join(l_args_for_creating_junc_bed + [">", path_file_junc_bed])
+                )
+            else:
+                bk.OS_Run(
+                    l_args_for_creating_junc_bed,
+                    path_file_stdout=path_file_junc_bed,
+                    stdout_binary=False,
+                )
+        if os.path.exists(path_file_junc_bed):
+            l_arg += ["--junc-bed", path_file_junc_bed]
+
+    if drop_unaligned:
+        l_arg += ["--sam-hit-only"]
+    l_arg += [path_file_minimap2_index, path_file_fastq]
+    if return_bash_shellscript:  # perform minimap2 alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+    else:
+        run = subprocess.run(l_arg, capture_output=True)
+        with open(
+            f"{path_folder_minimap2_output}{name_file_fastq}.minimap2_aligned.out", "w"
+        ) as file:
+            file.write(run.stdout.decode())
+        if verbose:
+            print("minimap2 completed")
+
+    """ sort output SAM file """
+    l_arg = [
+        "samtools",
+        "sort",
+        "-@",
+        str(int(min(n_threads_for_sort, 10))),
+        "-O",
+        "BAM",
+        "-o",
+        path_file_bam,
+        path_file_sam,
+    ]
+    if return_bash_shellscript:  # perform minimap2 alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+        l_bash_shellscript.append(" ".join(["rm", "-f", path_file_sam]))
+    else:
+        run = subprocess.run(l_arg, capture_output=False)
+        os.remove(path_file_sam)  # remove sam file
+
+    """ index resulting BAM file """
+    l_arg = ["samtools", "index", path_file_bam]
+    if return_bash_shellscript:  # perform minimap2 alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+    else:
+        run = subprocess.run(l_arg, capture_output=False)
+        if verbose:
+            print("samtools bam file compressing and indexing completed")
+
+    if return_bash_shellscript:  # retrun bash shell scripts
+        return " && ".join(l_bash_shellscript)
+
+
+def Minimap2_Index(path_file_fasta, path_file_minimap2_index=None, verbose=False):
+    """
+    # 2021-03-24 00:44:51
     index given fasta file for nanopore reads alignment
     'path_file_fasta' : input reference fasta file
     'path_file_minimap2_index' : minimap2 index file
     """
-    path_folder_fastq, name_file_fasta = path_file_fasta.rsplit( '/', 1 )
-    if path_file_minimap2_index is None : # set the default directory of the minimap index 
-        path_file_minimap2_index = f'{path_folder_fastq}/index/minimap2/{name_file_fasta}.ont.mmi'
-    path_folder_minimap2_index, name_file_index = path_file_minimap2_index.rsplit( '/', 1 )
-    path_folder_minimap2_index += '/'
-    os.makedirs( path_folder_minimap2_index, exist_ok = True ) # create folder if it does not exist
-    if os.path.exists( path_file_minimap2_index ) : # exit if an index file already exists
-        return 
+    path_folder_fastq, name_file_fasta = path_file_fasta.rsplit("/", 1)
+    if (
+        path_file_minimap2_index is None
+    ):  # set the default directory of the minimap index
+        path_file_minimap2_index = (
+            f"{path_folder_fastq}/index/minimap2/{name_file_fasta}.ont.mmi"
+        )
+    path_folder_minimap2_index, name_file_index = path_file_minimap2_index.rsplit(
+        "/", 1
+    )
+    path_folder_minimap2_index += "/"
+    os.makedirs(
+        path_folder_minimap2_index, exist_ok=True
+    )  # create folder if it does not exist
+    if os.path.exists(path_file_minimap2_index):  # exit if an index file already exists
+        return
     # build minimap2 index
-    run = subprocess.run( [ 'minimap2', '-x', 'map-ont', '-d', path_file_minimap2_index, path_file_fasta ], capture_output = True )
-    
-    with open( f'{path_folder_minimap2_index}{name_file_index}.minimap2_index.out', 'w' ) as file :
-        file.write( run.stdout.decode( ) )
-    if verbose :
-        print( 'minimap2 indexing completed' )
-        
-        
-def Desalt_Index( path_file_fasta, path_folder_desalt_index = None, verbose = False ) :
-    """ 
-    # 2021-08-02 11:26:56 
+    run = subprocess.run(
+        ["minimap2", "-x", "map-ont", "-d", path_file_minimap2_index, path_file_fasta],
+        capture_output=True,
+    )
+
+    with open(
+        f"{path_folder_minimap2_index}{name_file_index}.minimap2_index.out", "w"
+    ) as file:
+        file.write(run.stdout.decode())
+    if verbose:
+        print("minimap2 indexing completed")
+
+
+def Desalt_Index(path_file_fasta, path_folder_desalt_index=None, verbose=False):
+    """
+    # 2021-08-02 11:26:56
     index given fasta file for nanopore reads alignment using deSALT
     'path_file_fasta' : input reference fasta file
     'path_folder_desalt_index' : a folder where the index will be saved.
     """
-    path_folder_fastq, name_file_fasta = path_file_fasta.rsplit( '/', 1 )
-    if path_folder_desalt_index is None : # set the default directory of the minimap index 
-        os.makedirs( f'{path_folder_fastq}/index/desalt/', exist_ok = True )
-        path_folder_desalt_index = f'{path_folder_fastq}/index/desalt/{name_file_fasta}.desalt.idx/'
+    path_folder_fastq, name_file_fasta = path_file_fasta.rsplit("/", 1)
+    if (
+        path_folder_desalt_index is None
+    ):  # set the default directory of the minimap index
+        os.makedirs(f"{path_folder_fastq}/index/desalt/", exist_ok=True)
+        path_folder_desalt_index = (
+            f"{path_folder_fastq}/index/desalt/{name_file_fasta}.desalt.idx/"
+        )
     # build desalt index
-    run = subprocess.run( [ 'deSALT', 'index', path_file_fasta, path_folder_desalt_index ], capture_output = True )
-    with open( f"{path_folder_desalt_index.rsplit( '/', 1 )[ 0 ]}.desalt_index.out", 'w' ) as file :
-        file.write( run.stdout.decode( ) )
-    if verbose :
-        print( f'deSALT indexing of {path_file_fasta} completed' )
-        
-def Desalt_Align( path_file_fastq, path_folder_desalt_index = None, path_folder_desalt_output = None, arg_read_type = 'ont2d', path_file_gtf = None, n_threads = 20, verbose = True, return_bash_shellscript = False ) :
-    """ 
-    # 2021-06-14 23:19:19 
-    align given fastq file of nanopore reads using deSALT and write an output as a bam file 
+    run = subprocess.run(
+        ["deSALT", "index", path_file_fasta, path_folder_desalt_index],
+        capture_output=True,
+    )
+    with open(
+        f"{path_folder_desalt_index.rsplit( '/', 1 )[ 0 ]}.desalt_index.out", "w"
+    ) as file:
+        file.write(run.stdout.decode())
+    if verbose:
+        print(f"deSALT indexing of {path_file_fasta} completed")
+
+
+def Desalt_Align(
+    path_file_fastq,
+    path_folder_desalt_index=None,
+    path_folder_desalt_output=None,
+    arg_read_type="ont2d",
+    path_file_gtf=None,
+    n_threads=20,
+    verbose=True,
+    return_bash_shellscript=False,
+):
+    """
+    # 2021-06-14 23:19:19
+    align given fastq file of nanopore reads using deSALT and write an output as a bam file
     'path_file_fastq' : input fastq or fasta file (gzipped or uncompressed file is accepted)
     'path_folder_desalt_index' : desalt index file
     'path_folder_desalt_output' : desalt output folder
-    'arg_read_type' : parameter sets for each read type. available parameter sets are the following: 
+    'arg_read_type' : parameter sets for each read type. available parameter sets are the following:
                                    'ccs' (PacBio SMRT CCS reads): error rate 1%
                                    'clr' (PacBio SMRT CLR reads): error rate 15%
                                    'ont1d' (Oxford Nanopore 1D reads): error rate > 20%
                                    'ont2d' (Oxford Nanopore 2D reads): error rate > 12%
     'path_file_gtf' : directory of reference transcriptome annotations (for more accurate alignment)
     'return_bash_shellscript' : return shellscript instead of running desalt using the subprocess module
     """
-    path_folder_fastq, name_file_fastq = path_file_fastq.rsplit( '/', 1 )
-    if path_folder_desalt_output is None : # default output folder is a subdirectory of the folder containing the input fastq file
-        path_folder_desalt_output = f'{path_folder_fastq}/desalt/'
-    if path_folder_desalt_output[ -1 ] != '/' : # add '/' at the end of the output directory if it does not exist
-        path_folder_desalt_output += '/'
-    os.makedirs( path_folder_desalt_output, exist_ok = True ) # create folder if it does not exist
+    path_folder_fastq, name_file_fastq = path_file_fastq.rsplit("/", 1)
+    if (
+        path_folder_desalt_output is None
+    ):  # default output folder is a subdirectory of the folder containing the input fastq file
+        path_folder_desalt_output = f"{path_folder_fastq}/desalt/"
+    if (
+        path_folder_desalt_output[-1] != "/"
+    ):  # add '/' at the end of the output directory if it does not exist
+        path_folder_desalt_output += "/"
+    os.makedirs(
+        path_folder_desalt_output, exist_ok=True
+    )  # create folder if it does not exist
 
     path_file_sam = f"{path_folder_desalt_output}{name_file_fastq}.desalt_aligned.sam"
     path_file_bam = f"{path_folder_desalt_output}{name_file_fastq}.desalt_aligned.bam"
-    
-    l_bash_shellscript = [ ]
-    
-    ''' perform desalt alignment '''
-    l_arg = [ 'deSALT', 'aln', '-t', str( int( n_threads ) ), '-x', arg_read_type, "-o", path_file_sam ] 
-    if path_file_gtf is not None :
-        path_file_gtf_info = f"{path_file_gtf}.desalt.info" # directory of a processed gtf file
+
+    l_bash_shellscript = []
+
+    """ perform desalt alignment """
+    l_arg = [
+        "deSALT",
+        "aln",
+        "-t",
+        str(int(n_threads)),
+        "-x",
+        arg_read_type,
+        "-o",
+        path_file_sam,
+    ]
+    if path_file_gtf is not None:
+        path_file_gtf_info = (
+            f"{path_file_gtf}.desalt.info"  # directory of a processed gtf file
+        )
         # process a given gtf file into deSALT GTF info
-        if not os.path.exists( path_file_gtf_info ) :
-            run = subprocess.run( [ 'Annotation_Load.py', path_file_gtf, path_file_gtf_info ], capture_output = True )
-            with open( f'{path_file_gtf}.desalt_annotation_load.out', 'w' ) as file :
-                file.write( run.stdout.decode( ) )
-        l_arg += [ '-G', path_file_gtf ]
-    l_arg += [ path_folder_desalt_index, path_file_fastq ]
-    if return_bash_shellscript : # perform desalt alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-    else :
-        run = subprocess.run( l_arg, capture_output = True )
-        with open( f'{path_folder_desalt_output}{name_file_fastq}.desalt_aligned.out', 'w' ) as file :
-            file.write( run.stdout.decode( ) )
-        if verbose :
-            print( 'desalt completed' )
-            
-    ''' sort output SAM file '''
-    l_arg = [ 'samtools', 'sort', '-@', str( int( min( n_threads, 10 ) ) ), '-O', "BAM", '-o', path_file_bam, path_file_sam ]
-    if return_bash_shellscript : # perform desalt alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-        l_bash_shellscript.append( ' '.join( [ 'rm', '-f', path_file_sam ] ) )
-    else :     
-        run = subprocess.run( l_arg, capture_output = False )
-        os.remove( path_file_sam ) # remove sam file
-        
-    ''' index resulting BAM file '''
-    l_arg = [ 'samtools', 'index', path_file_bam ]
-    if return_bash_shellscript : # perform desalt alignment using subprocess module
-        l_bash_shellscript.append( ' '.join( l_arg ) )
-    else :   
-        run = subprocess.run( l_arg, capture_output = False )
-        if verbose :
-            print( 'samtools bam file compressing and indexing completed' )
-    
-    if return_bash_shellscript : # retrun bash shell scripts
-        return ' && '.join( l_bash_shellscript )
-        
-def FeatureCounts( path_file_annotation, path_file_output, * l_path_file_input, str_type_attribute = 'gene_id', verbose = False, return_dataframe = True ) :
-    """ 
-    # 2021-03-07 18:44:04 
+        if not os.path.exists(path_file_gtf_info):
+            run = subprocess.run(
+                ["Annotation_Load.py", path_file_gtf, path_file_gtf_info],
+                capture_output=True,
+            )
+            with open(f"{path_file_gtf}.desalt_annotation_load.out", "w") as file:
+                file.write(run.stdout.decode())
+        l_arg += ["-G", path_file_gtf]
+    l_arg += [path_folder_desalt_index, path_file_fastq]
+    if return_bash_shellscript:  # perform desalt alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+    else:
+        run = subprocess.run(l_arg, capture_output=True)
+        with open(
+            f"{path_folder_desalt_output}{name_file_fastq}.desalt_aligned.out", "w"
+        ) as file:
+            file.write(run.stdout.decode())
+        if verbose:
+            print("desalt completed")
+
+    """ sort output SAM file """
+    l_arg = [
+        "samtools",
+        "sort",
+        "-@",
+        str(int(min(n_threads, 10))),
+        "-O",
+        "BAM",
+        "-o",
+        path_file_bam,
+        path_file_sam,
+    ]
+    if return_bash_shellscript:  # perform desalt alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+        l_bash_shellscript.append(" ".join(["rm", "-f", path_file_sam]))
+    else:
+        run = subprocess.run(l_arg, capture_output=False)
+        os.remove(path_file_sam)  # remove sam file
+
+    """ index resulting BAM file """
+    l_arg = ["samtools", "index", path_file_bam]
+    if return_bash_shellscript:  # perform desalt alignment using subprocess module
+        l_bash_shellscript.append(" ".join(l_arg))
+    else:
+        run = subprocess.run(l_arg, capture_output=False)
+        if verbose:
+            print("samtools bam file compressing and indexing completed")
+
+    if return_bash_shellscript:  # retrun bash shell scripts
+        return " && ".join(l_bash_shellscript)
+
+
+def FeatureCounts(
+    path_file_annotation,
+    path_file_output,
+    *l_path_file_input,
+    str_type_attribute="gene_id",
+    verbose=False,
+    return_dataframe=True,
+):
+    """
+    # 2021-03-07 18:44:04
     count aligned reads using featureCounts
     'str_type_attribute' : see featureCounts help messages
     'return_dataframe' : return a dataframe containing the featureCounts output
     """
-    path_folder_output, name_file_output = path_file_output.rsplit( '/', 1 )
-    path_folder_output += '/'
-    os.makedirs( path_folder_output, exist_ok = True ) # create folder if it does not exist
-    
-    run = subprocess.run( [ 'featureCounts', '-L', '-a', path_file_annotation, '-o', path_file_output, '-g', str_type_attribute ] + list( l_path_file_input ), capture_output = True )
-    with open( f'{path_file_output}.featureCounts.out', 'w' ) as file :
-        file.write( run.stdout.decode( ) )
-    if verbose :
-        print( 'featureCounts completed' )
-    if return_dataframe : # return a dataframe containing the featureCounts output
-        df = pd.read_csv( path_file_output, sep = '\t', low_memory = False, skiprows = [ 0 ] )
+    path_folder_output, name_file_output = path_file_output.rsplit("/", 1)
+    path_folder_output += "/"
+    os.makedirs(path_folder_output, exist_ok=True)  # create folder if it does not exist
+
+    run = subprocess.run(
+        [
+            "featureCounts",
+            "-L",
+            "-a",
+            path_file_annotation,
+            "-o",
+            path_file_output,
+            "-g",
+            str_type_attribute,
+        ]
+        + list(l_path_file_input),
+        capture_output=True,
+    )
+    with open(f"{path_file_output}.featureCounts.out", "w") as file:
+        file.write(run.stdout.decode())
+    if verbose:
+        print("featureCounts completed")
+    if return_dataframe:  # return a dataframe containing the featureCounts output
+        df = pd.read_csv(path_file_output, sep="\t", low_memory=False, skiprows=[0])
         return df
 
-def Gene_Read_Count( path_file_bam, dict_it_gene, thres_mapq = 60 ) :
-    """ 
-    Count number of reads uniquely aligned to each gene 
-    
+
+def Gene_Read_Count(path_file_bam, dict_it_gene, thres_mapq=60):
+    """
+    Count number of reads uniquely aligned to each gene
+
     'path_file_bam' : BAM file containing aligned nanopore reads
     'dict_it_gene' : dictionary of interval trees from a GTF file containing gene annotations of the reference genome to which the nanopore reads have been aligned (returned by 'GTF_Interval_Tree')
     'thres_mapq' : threshold for mapping quality
-    
+
     return a dataframe
     """
 
     # retrieve aligned length of nanopore read for each gene
-    dict_count = dict( )
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        for r in samfile.fetch( ) :
-            if r.reference_name not in dict_it_gene : # skip read aligned to segment that does not contain genes
-                continue
-            if r.mapq < thres_mapq : # skip read whose mapq is below 'thres_mapq'
-                continue
-            if r.seq is None : # skip multi-mapped reads (minimap2 skip sequence information for multi-mapped reads)
-                continue
-            set_overlap = dict_it_gene[ r.reference_name ].overlap( r.reference_start, r.reference_end )
-            if len( set_overlap ) == 0 : # skip if the read has not been aligned to any genes
-                continue
-            name_gene = list( set_overlap )[ 0 ][ 2 ][ 0 ]
-            if name_gene not in dict_count :
-                dict_count[ name_gene ] = 0
-            dict_count[ name_gene ] += 1
+    dict_count = dict()
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        for r in samfile.fetch():
+            if (
+                r.reference_name not in dict_it_gene
+            ):  # skip read aligned to segment that does not contain genes
+                continue
+            if r.mapq < thres_mapq:  # skip read whose mapq is below 'thres_mapq'
+                continue
+            if (
+                r.seq is None
+            ):  # skip multi-mapped reads (minimap2 skip sequence information for multi-mapped reads)
+                continue
+            set_overlap = dict_it_gene[r.reference_name].overlap(
+                r.reference_start, r.reference_end
+            )
+            if (
+                len(set_overlap) == 0
+            ):  # skip if the read has not been aligned to any genes
+                continue
+            name_gene = list(set_overlap)[0][2][0]
+            if name_gene not in dict_count:
+                dict_count[name_gene] = 0
+            dict_count[name_gene] += 1
     return dict_count
-    
+
     # summarize read length distribution for each gene
-    l_l = [ ]
-    for name_gene in dict_length :
-        arr = np.array( dict_length[ name_gene ], dtype = int )
-        l_l.append( [ name_gene, len( arr ), np.mean( arr ), np.std( arr ) ] )
-    df_gene_read_length_summary = pd.DataFrame( l_l, columns = [ 'name_gene', 'n_reads', 'mean_read_length', 'std_read_length' ] )
+    l_l = []
+    for name_gene in dict_length:
+        arr = np.array(dict_length[name_gene], dtype=int)
+        l_l.append([name_gene, len(arr), np.mean(arr), np.std(arr)])
+    df_gene_read_length_summary = pd.DataFrame(
+        l_l, columns=["name_gene", "n_reads", "mean_read_length", "std_read_length"]
+    )
     return df_gene_read_length_summary
-    
-def Gene_Read_Length( path_file_bam, path_file_gtf, return_list_of_read_length = False, thres_mapq = 30 ) :
-    """ 
-    # 2021-04-23 19:19:33 
+
+
+def Gene_Read_Length(
+    path_file_bam, path_file_gtf, return_list_of_read_length=False, thres_mapq=30
+):
+    """
+    # 2021-04-23 19:19:33
     'path_file_bam' : BAM file containing aligned nanopore reads
     'path_file_gtf' : GTF file containing gene annotations of the reference genome to which the nanopore reads have been aligned
     'return_list_of_read_length' : return a dictionary containing list of read length for each name_gene
     'thres_mapq' : threshold for mapping quality
-    
-    return a dataframe summarizing aligned read length distribution for each gene   
+
+    return a dataframe summarizing aligned read length distribution for each gene
     """
     # read gtf file and build interval tree
-    df_gtf = GTF_Read( path_file_gtf, parse_attr = True )
-    df_gtf_gene = PD_Select( df_gtf, feature = 'gene' )
-    dict_it = dict( )
-    for gene_name, seqname, start, end in df_gtf_gene[ [ 'gene_name', 'seqname', 'start', 'end' ] ].values :
-        if seqname not in dict_it :
-            dict_it[ seqname ] = intervaltree.IntervalTree( )
-        dict_it[ seqname ].addi( start, end, [ gene_name ] )
+    df_gtf = GTF_Read(path_file_gtf, parse_attr=True)
+    df_gtf_gene = PD_Select(df_gtf, feature="gene")
+    dict_it = dict()
+    for gene_name, seqname, start, end in df_gtf_gene[
+        ["gene_name", "seqname", "start", "end"]
+    ].values:
+        if seqname not in dict_it:
+            dict_it[seqname] = intervaltree.IntervalTree()
+        dict_it[seqname].addi(start, end, [gene_name])
 
     # retrieve aligned length of nanopore read for each gene
-    dict_length = dict( )
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        for r in samfile.fetch( ) :
-            if r.reference_name not in dict_it : # skip read aligned to segment that does not contain genes
-                continue
-            if r.mapq < thres_mapq : # skip read whose mapq is below 'thres_mapq'
-                continue
-            set_overlap = dict_it[ r.reference_name ].overlap( r.reference_start, r.reference_end )
-            if len( set_overlap ) == 0 :
-                continue
-            name_gene = list( set_overlap )[ 0 ][ 2 ][ 0 ]
-            if name_gene not in dict_length :
-                dict_length[ name_gene ] = [ ]
-            dict_length[ name_gene ].append( r.qlen )
-    if return_list_of_read_length : # if 'return_list_of_read_length' is set to True, return a dictionary containing list of read length for each name_gene 
+    dict_length = dict()
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        for r in samfile.fetch():
+            if (
+                r.reference_name not in dict_it
+            ):  # skip read aligned to segment that does not contain genes
+                continue
+            if r.mapq < thres_mapq:  # skip read whose mapq is below 'thres_mapq'
+                continue
+            set_overlap = dict_it[r.reference_name].overlap(
+                r.reference_start, r.reference_end
+            )
+            if len(set_overlap) == 0:
+                continue
+            name_gene = list(set_overlap)[0][2][0]
+            if name_gene not in dict_length:
+                dict_length[name_gene] = []
+            dict_length[name_gene].append(r.qlen)
+    if (
+        return_list_of_read_length
+    ):  # if 'return_list_of_read_length' is set to True, return a dictionary containing list of read length for each name_gene
         return dict_length
-    
+
     # summarize read length distribution for each gene
-    l_l = [ ]
-    for name_gene in dict_length :
-        arr = np.array( dict_length[ name_gene ], dtype = int )
-        l_l.append( [ name_gene, len( arr ), np.mean( arr ), np.std( arr ) ] )
-    df_gene_read_length_summary = pd.DataFrame( l_l, columns = [ 'name_gene', 'n_reads', 'mean_read_length', 'std_read_length' ] )
+    l_l = []
+    for name_gene in dict_length:
+        arr = np.array(dict_length[name_gene], dtype=int)
+        l_l.append([name_gene, len(arr), np.mean(arr), np.std(arr)])
+    df_gene_read_length_summary = pd.DataFrame(
+        l_l, columns=["name_gene", "n_reads", "mean_read_length", "std_read_length"]
+    )
     return df_gene_read_length_summary
 
-def Gene_10X_Adaptor( path_file_bam, path_file_gtf, thres_mapq = 60, float_error_rate = 0.15 ) :
-    """ 
-    # 2021-04-27 11:30:13 
+
+def Gene_10X_Adaptor(
+    path_file_bam, path_file_gtf, thres_mapq=60, float_error_rate=0.15
+):
+    """
+    # 2021-04-27 11:30:13
     'path_file_bam' : BAM file containing aligned nanopore reads
     'path_file_gtf' : GTF file containing gene annotations of the reference genome to which the nanopore reads have been aligned
     'thres_mapq' : threshold for mapping quality
     'float_error_rate' : error rate for searching 10X adaptor sequences
-    
+
     return a dataframe containing adaptor counts for each gene
     """
     # read gtf file and build interval tree
-    df_gtf = GTF_Read( path_file_gtf, parse_attr = True )
-    df_gtf_gene = PD_Select( df_gtf, feature = 'gene' )
-    dict_it = dict( )
-    for gene_name, seqname, start, end in df_gtf_gene[ [ 'gene_name', 'seqname', 'start', 'end' ] ].values :
-        if seqname not in dict_it :
-            dict_it[ seqname ] = intervaltree.IntervalTree( )
-        dict_it[ seqname ].addi( start, end, [ gene_name ] )
+    df_gtf = GTF_Read(path_file_gtf, parse_attr=True)
+    df_gtf_gene = PD_Select(df_gtf, feature="gene")
+    dict_it = dict()
+    for gene_name, seqname, start, end in df_gtf_gene[
+        ["gene_name", "seqname", "start", "end"]
+    ].values:
+        if seqname not in dict_it:
+            dict_it[seqname] = intervaltree.IntervalTree()
+        dict_it[seqname].addi(start, end, [gene_name])
 
     # adaptor sequences for counting adaptor sequences from the soft-clipped sequences at the ends
     str_seq_tso = "AAGCAGTGGTATCAACGCAGAGTACAT"
     str_seq_r1 = "CTACACGACGCTCTTCCGATCT"
-    str_seq_tso_rc = NGS_SEQ_Reverse_Complement( "AAGCAGTGGTATCAACGCAGAGTACAT" )
-    str_seq_r1_rc = NGS_SEQ_Reverse_Complement( "CTACACGACGCTCTTCCGATCT" )
+    str_seq_tso_rc = NGS_SEQ_Reverse_Complement("AAGCAGTGGTATCAACGCAGAGTACAT")
+    str_seq_r1_rc = NGS_SEQ_Reverse_Complement("CTACACGACGCTCTTCCGATCT")
 
-    dict_adaptor = dict( )
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        for r in samfile.fetch( ) :
-            if r.reference_name not in dict_it : # skip read aligned to segment that does not contain genes
+    dict_adaptor = dict()
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        for r in samfile.fetch():
+            if (
+                r.reference_name not in dict_it
+            ):  # skip read aligned to segment that does not contain genes
                 continue
-            if r.mapq < thres_mapq : # skip read whose mapq is below 'thres_mapq'
+            if r.mapq < thres_mapq:  # skip read whose mapq is below 'thres_mapq'
                 continue
-            if r.seq is None : # skip multi-mapped reads (minimap2 skip sequence information for multi-mapped reads)
+            if (
+                r.seq is None
+            ):  # skip multi-mapped reads (minimap2 skip sequence information for multi-mapped reads)
                 continue
-            set_overlap = dict_it[ r.reference_name ].overlap( r.reference_start, r.reference_end )
-            if len( set_overlap ) == 0 : # skip if no gene was assigned to the read 
+            set_overlap = dict_it[r.reference_name].overlap(
+                r.reference_start, r.reference_end
+            )
+            if len(set_overlap) == 0:  # skip if no gene was assigned to the read
                 continue
-            name_gene = list( set_overlap )[ 0 ][ 2 ][ 0 ] # retrieve name of the gene that the read was assigned
+            name_gene = list(set_overlap)[0][2][
+                0
+            ]  # retrieve name of the gene that the read was assigned
 
             # retrieve soft-clipped sequences from the ends of the read
-            l_cigar = list( NGS_CIGAR_Iterate_a_CIGAR_String( r.cigarstring ) ) # retrieve tuples of a cigar string
-            l_seq = [ ] 
-            if l_cigar[ 0 ][ 1 ] == 'S' :
-                l_seq.append( r.seq[ : l_cigar[ 0 ][ 0 ] ] )
-            if l_cigar[ -1 ][ 1 ] == 'S' :
-                l_seq.append( r.seq[ - l_cigar[ -1 ][ 0 ] : ] )
+            l_cigar = list(
+                NGS_CIGAR_Iterate_a_CIGAR_String(r.cigarstring)
+            )  # retrieve tuples of a cigar string
+            l_seq = []
+            if l_cigar[0][1] == "S":
+                l_seq.append(r.seq[: l_cigar[0][0]])
+            if l_cigar[-1][1] == "S":
+                l_seq.append(r.seq[-l_cigar[-1][0] :])
             # count adaptors at the soft-clipped sequences at the ends
             n_tso_count, n_r1_count = 0, 0
-            for seq_adaptor in [ str_seq_tso, str_seq_tso_rc ] :
-                for seq in l_seq :
-                    if STR.Search_Subsequence( seq, seq_adaptor, error_rate = float_error_rate )[ 'matched_subsequence' ] is not None : # increase the count if the adaptor is found in the soft-clipped bsequence
+            for seq_adaptor in [str_seq_tso, str_seq_tso_rc]:
+                for seq in l_seq:
+                    if (
+                        STR.Search_Subsequence(
+                            seq, seq_adaptor, error_rate=float_error_rate
+                        )["matched_subsequence"]
+                        is not None
+                    ):  # increase the count if the adaptor is found in the soft-clipped bsequence
                         n_tso_count += 1
-            for seq_adaptor in [ str_seq_r1, str_seq_r1_rc ] :
-                for seq in l_seq :
-                    if STR.Search_Subsequence( seq, seq_adaptor, error_rate = float_error_rate )[ 'matched_subsequence' ] is not None :
+            for seq_adaptor in [str_seq_r1, str_seq_r1_rc]:
+                for seq in l_seq:
+                    if (
+                        STR.Search_Subsequence(
+                            seq, seq_adaptor, error_rate=float_error_rate
+                        )["matched_subsequence"]
+                        is not None
+                    ):
                         n_r1_count += 1
 
             # count each adaptor_type (classification of reads based on adaptor counts) for each gene
-            if name_gene not in dict_adaptor :
-                dict_adaptor[ name_gene ] = dict( )
-            name_adaptor_type = f'tso_{n_tso_count}__r1_{n_r1_count}'
-            if name_adaptor_type not in dict_adaptor[ name_gene ] :
-                dict_adaptor[ name_gene ][ name_adaptor_type ] = 0
-            dict_adaptor[ name_gene ][ name_adaptor_type ] += 1
-    
+            if name_gene not in dict_adaptor:
+                dict_adaptor[name_gene] = dict()
+            name_adaptor_type = f"tso_{n_tso_count}__r1_{n_r1_count}"
+            if name_adaptor_type not in dict_adaptor[name_gene]:
+                dict_adaptor[name_gene][name_adaptor_type] = 0
+            dict_adaptor[name_gene][name_adaptor_type] += 1
+
     # compose a dataframe
-    df = pd.DataFrame( dict_adaptor ).T
-    df.fillna( 0, inplace = True )
-    df[ 'total_count' ] = df.sum( axis = 1 )
-    df.sort_values( 'total_count', ascending = False, inplace = True )
-    df.index.name = 'name_gene'
+    df = pd.DataFrame(dict_adaptor).T
+    df.fillna(0, inplace=True)
+    df["total_count"] = df.sum(axis=1)
+    df.sort_values("total_count", ascending=False, inplace=True)
+    df.index.name = "name_gene"
     return df
 
 
-def Check_plasmid_with_nanopore_sequencing( path_file_fasta_ref = None, path_file_fastq = None, path_folder_output = 'default', n_threads = 10, flag_correct_reference = False, flag_perform_assembly = False ) :
+def Check_plasmid_with_nanopore_sequencing(
+    path_file_fasta_ref=None,
+    path_file_fastq=None,
+    path_folder_output="default",
+    n_threads=10,
+    flag_correct_reference=False,
+    flag_perform_assembly=False,
+):
     """
-    # 2021-06-03 21:52:00 
-    Correct plasmid sequence using nanopore sequencing 
-    
+    # 2021-06-03 21:52:00
+    Correct plasmid sequence using nanopore sequencing
+
     'path_file_fastq' : (Required) directory of a fasta file containing the reference sequence. (e.g. a fasta sequence from AddGene)
     'path_folder_output' : (Default: subdirectory of the folder containing the given fastq file) directory of output folder
     'n_threads' : number of threads to run the pipeline
-    
+
     """
     # 'flag_correct_reference' : manually set 'id_barcoding_kit' for guppy_bascaller run.
-    
-    flag_entry_point = PKG.Detect_Entry_Point( 'biobook' ) # detect whether an entry point was used
-    if flag_entry_point :
-        parser = argparse.ArgumentParser( description = "Analyze nanopore sequencing data of a plasmid. This program has been developed by Hyunsu An (2021/06/03)." )
-        parser.add_argument( "-r", "--path_file_fasta_ref", help = "(Required) directory of a fasta file containing the reference sequence. (e.g. a fasta sequence from AddGene)" )
-        parser.add_argument( "-i", "--path_file_fastq", help = "(Required) directory of a fastq file from a nanopore sequencing" )
-        parser.add_argument( "-o", "--path_folder_output", help = "(Default: subdirectory of the folder containing the given fastq file) directory of output folder", default = 'default' )
-        parser.add_argument( "-t", "--threads", help = "(Default: 10) Number of threads to use in the current compute node.", default = '10' )
-        parser.add_argument( "-a", "--flag_perform_assembly", help = "(Default: False) Perform assembly using Flye", action = 'store_true' )
 
-        args = parser.parse_args( )
+    flag_entry_point = PKG.Detect_Entry_Point(
+        "biobook"
+    )  # detect whether an entry point was used
+    if flag_entry_point:
+        parser = argparse.ArgumentParser(
+            description="Analyze nanopore sequencing data of a plasmid. This program has been developed by Hyunsu An (2021/06/03)."
+        )
+        parser.add_argument(
+            "-r",
+            "--path_file_fasta_ref",
+            help="(Required) directory of a fasta file containing the reference sequence. (e.g. a fasta sequence from AddGene)",
+        )
+        parser.add_argument(
+            "-i",
+            "--path_file_fastq",
+            help="(Required) directory of a fastq file from a nanopore sequencing",
+        )
+        parser.add_argument(
+            "-o",
+            "--path_folder_output",
+            help="(Default: subdirectory of the folder containing the given fastq file) directory of output folder",
+            default="default",
+        )
+        parser.add_argument(
+            "-t",
+            "--threads",
+            help="(Default: 10) Number of threads to use in the current compute node.",
+            default="10",
+        )
+        parser.add_argument(
+            "-a",
+            "--flag_perform_assembly",
+            help="(Default: False) Perform assembly using Flye",
+            action="store_true",
+        )
+
+        args = parser.parse_args()
         # [input] parse arguments from parse_args
         path_file_fasta_ref = args.path_file_fasta_ref
         path_file_fastq = args.path_file_fastq
         path_folder_output = args.path_folder_output
         flag_perform_assembly = args.flag_perform_assembly
         # flag_correct_reference = args.flag_correct_reference
-        n_threads = int( args.threads )
-    
-    
-    ''' [parse arguments] '''
-    if path_file_fastq is None or path_file_fastq is None  :
-        print( "required arguments are not given, exiting" )
-        if flag_entry_point :
-            sys.exit( ) 
-        else :
+        n_threads = int(args.threads)
+
+    """ [parse arguments] """
+    if path_file_fastq is None or path_file_fastq is None:
+        print("required arguments are not given, exiting")
+        if flag_entry_point:
+            sys.exit()
+        else:
             return -1
-        
 
-    # [process input] output folder 
+    # [process input] output folder
     # retrieve absolute paths
-    path_file_fasta_ref = os.path.abspath( path_file_fasta_ref )
-    path_file_fastq = os.path.abspath( path_file_fastq )
-    # set default output folder 
-    if path_folder_output == 'default' : 
-        path_folder, name_file = path_file_fastq.rsplit( '/', 1 )
-        path_folder += '/'
-        if name_file.rsplit( '.', 1 )[ 1 ].lower( ) == 'gz' :
-            name_file = name_file.rsplit( '.', 1 )[ 0 ]
-        name_file = name_file.rsplit( '.', 1 )[ 0 ]
+    path_file_fasta_ref = os.path.abspath(path_file_fasta_ref)
+    path_file_fastq = os.path.abspath(path_file_fastq)
+    # set default output folder
+    if path_folder_output == "default":
+        path_folder, name_file = path_file_fastq.rsplit("/", 1)
+        path_folder += "/"
+        if name_file.rsplit(".", 1)[1].lower() == "gz":
+            name_file = name_file.rsplit(".", 1)[0]
+        name_file = name_file.rsplit(".", 1)[0]
         path_folder_output = f"{path_folder}{name_file}/"
-    path_folder_output = os.path.abspath( path_folder_output )
-    if path_folder_output[ -1 ] != '/' : # add '/' at the end of the output folder
-        path_folder_output += '/'
-    if os.path.exists( path_folder_output ) : # if output folder already exists, exit
-        print( 'output folder already exists, exiting' )
-        if flag_entry_point :
-            sys.exit( ) 
-        else :
+    path_folder_output = os.path.abspath(path_folder_output)
+    if path_folder_output[-1] != "/":  # add '/' at the end of the output folder
+        path_folder_output += "/"
+    if os.path.exists(path_folder_output):  # if output folder already exists, exit
+        print("output folder already exists, exiting")
+        if flag_entry_point:
+            sys.exit()
+        else:
             return -1
-    else : # create an output folder
-        os.makedirs( path_folder_output )
-            
+    else:  # create an output folder
+        os.makedirs(path_folder_output)
+
     """ analyze plasmid sequence """
     path_file_index_ref = f"{path_folder_output}index.ont.mmi"
-    Minimap2_Index( path_file_fasta_ref, path_file_index_ref )
+    Minimap2_Index(path_file_fasta_ref, path_file_index_ref)
     path_folder_minimap2_output = f"{path_folder_output}minimap2/"
-    Minimap2_Align( path_file_fastq, path_file_minimap2_index = path_file_index_ref, path_folder_minimap2_output = path_folder_minimap2_output, n_threads = n_threads )
-
-    dict_fasta = FASTA_Read( path_file_fasta_ref )
-    str_fasta_ref = dict_fasta[ list( dict_fasta )[ 0 ] ].upper( ) # read genome sequence of the reference (first sequence of the reference fasta file)
-    shutil.copyfile( path_file_fasta_ref, f"{path_folder_minimap2_output}{path_file_fasta_ref.rsplit( '/', 1 )[ 1 ]}" ) # copy reference sequence file to minimap2 output file (convenient minimap visualization
+    Minimap2_Align(
+        path_file_fastq,
+        path_file_minimap2_index=path_file_index_ref,
+        path_folder_minimap2_output=path_folder_minimap2_output,
+        n_threads=n_threads,
+    )
+
+    dict_fasta = FASTA_Read(path_file_fasta_ref)
+    str_fasta_ref = dict_fasta[
+        list(dict_fasta)[0]
+    ].upper()  # read genome sequence of the reference (first sequence of the reference fasta file)
+    shutil.copyfile(
+        path_file_fasta_ref,
+        f"{path_folder_minimap2_output}{path_file_fasta_ref.rsplit( '/', 1 )[ 1 ]}",
+    )  # copy reference sequence file to minimap2 output file (convenient minimap visualization
 
     # count number of each base for each position of the reference genome
     str_list_of_bases = "ATGC-"
-    dict_base_to_index = dict( ( ( str_base, i ) for i, str_base in enumerate( str_list_of_bases ) ) )
-    arr_count_base = np.zeros( ( 5, len( str_fasta_ref ) ) )
-
-    l = [ ]
-    with pysam.AlignmentFile( glob.glob( f"{path_folder_minimap2_output}*.bam" )[ 0 ], 'rb' ) as samfile :
-        for r in samfile.fetch( ) :
-            for pos_read, pos_ref in r.aligned_pairs :
-                if pos_ref is not None and r.seq is not None : # ignore insertion mutation type # ignore secondary alignment (where sequence is None)
-                    arr_count_base[ dict_base_to_index[ '-' if pos_read is None else r.seq[ pos_read ] ] ][ pos_ref ] += 1 # detect deletion by checking aligned positions of a read
+    dict_base_to_index = dict(
+        ((str_base, i) for i, str_base in enumerate(str_list_of_bases))
+    )
+    arr_count_base = np.zeros((5, len(str_fasta_ref)))
+
+    l = []
+    with pysam.AlignmentFile(
+        glob.glob(f"{path_folder_minimap2_output}*.bam")[0], "rb"
+    ) as samfile:
+        for r in samfile.fetch():
+            for pos_read, pos_ref in r.aligned_pairs:
+                if (
+                    pos_ref is not None and r.seq is not None
+                ):  # ignore insertion mutation type # ignore secondary alignment (where sequence is None)
+                    arr_count_base[
+                        dict_base_to_index["-" if pos_read is None else r.seq[pos_read]]
+                    ][
+                        pos_ref
+                    ] += 1  # detect deletion by checking aligned positions of a read
 
     # summerize results
-    arr_coverage = arr_count_base.sum( axis = 0 )
-    arr_coverage[ arr_coverage == 0 ] = -1 # mask positions with zero coverage
-    df_summary = pd.DataFrame( arr_count_base / arr_coverage, index = list( str_list_of_bases ), columns = np.arange( 1, len( str_fasta_ref ) + 1 ) ) # 1-based coordinates
-    df_summary.loc[ 'coverage' ] = arr_count_base.sum( axis = 0 )
-    str_fasta_consensus = ''.join( list( str_list_of_bases[ arr_freq.argmax( ) ] if arr_freq.sum( ) > 0.1 else '*' for arr_freq in ( arr_count_base / arr_coverage ).T ) ) # if arr_frequency contains only zero values (no coverage), put '*' in the sequence
-    df_summary.loc[ 'consensus_sequence' ] = list( str_fasta_consensus )
-    df_summary.loc[ 'reference_sequence' ] = list( str_fasta_ref )
-    l = [ ]
+    arr_coverage = arr_count_base.sum(axis=0)
+    arr_coverage[arr_coverage == 0] = -1  # mask positions with zero coverage
+    df_summary = pd.DataFrame(
+        arr_count_base / arr_coverage,
+        index=list(str_list_of_bases),
+        columns=np.arange(1, len(str_fasta_ref) + 1),
+    )  # 1-based coordinates
+    df_summary.loc["coverage"] = arr_count_base.sum(axis=0)
+    str_fasta_consensus = "".join(
+        list(
+            str_list_of_bases[arr_freq.argmax()] if arr_freq.sum() > 0.1 else "*"
+            for arr_freq in (arr_count_base / arr_coverage).T
+        )
+    )  # if arr_frequency contains only zero values (no coverage), put '*' in the sequence
+    df_summary.loc["consensus_sequence"] = list(str_fasta_consensus)
+    df_summary.loc["reference_sequence"] = list(str_fasta_ref)
+    l = []
     # classify mutations
-    for base_consensus, base_ref in zip( df_summary.loc[ 'consensus_sequence' ].values, df_summary.loc[ 'reference_sequence' ].values ) :
-        str_mut_type = '.' # default mut_type
-        if base_consensus == base_ref :
+    for base_consensus, base_ref in zip(
+        df_summary.loc["consensus_sequence"].values,
+        df_summary.loc["reference_sequence"].values,
+    ):
+        str_mut_type = "."  # default mut_type
+        if base_consensus == base_ref:
             pass
-        elif base_consensus == '-' :
-            str_mut_type = 'deletion'
-        elif base_ref == 'N' :
+        elif base_consensus == "-":
+            str_mut_type = "deletion"
+        elif base_ref == "N":
             pass
-        elif base_consensus == '*' :
-            str_mut_type = 'unknown'
-        else :
-            str_mut_type = 'substitution'
-        l.append( str_mut_type )
-    df_summary.loc[ 'mutation_type' ] = l
-    df_summary.to_excel( f"{path_folder_output}summary__base_frequency.xlsx" )
+        elif base_consensus == "*":
+            str_mut_type = "unknown"
+        else:
+            str_mut_type = "substitution"
+        l.append(str_mut_type)
+    df_summary.loc["mutation_type"] = l
+    df_summary.to_excel(f"{path_folder_output}summary__base_frequency.xlsx")
 
     # detect substitutions and extract a flanking sequence for each substitution
-    df_substitution = df_summary.T[ df_summary.T.mutation_type == 'substitution' ]
-    df_substitution.index.name = 'location_of_mutation'
-    df_substitution.reset_index( inplace = True )
-
-    len_flanking_base = 5 # number of bases flanking a mutation
-    l_l = list( )
-    for index in df_substitution.location_of_mutation.values - 1 : # 0-based coordinates
-        sl = slice( index - len_flanking_base, index + len_flanking_base + 1 )
-        l_l.append( [ str_fasta_consensus[ sl ], str_fasta_ref[ sl ] ] )
-    df_substitution = df_substitution.join( pd.DataFrame( l_l, columns = [ 'flanking_sequence_consensus', 'flanking_sequence_reference' ] ) )
-    df_substitution.to_excel( f"{path_folder_output}summary__substitution.xlsx" )
-    
-    if flag_perform_assembly : # perform assembly if the flag is on
+    df_substitution = df_summary.T[df_summary.T.mutation_type == "substitution"]
+    df_substitution.index.name = "location_of_mutation"
+    df_substitution.reset_index(inplace=True)
+
+    len_flanking_base = 5  # number of bases flanking a mutation
+    l_l = list()
+    for index in df_substitution.location_of_mutation.values - 1:  # 0-based coordinates
+        sl = slice(index - len_flanking_base, index + len_flanking_base + 1)
+        l_l.append([str_fasta_consensus[sl], str_fasta_ref[sl]])
+    df_substitution = df_substitution.join(
+        pd.DataFrame(
+            l_l, columns=["flanking_sequence_consensus", "flanking_sequence_reference"]
+        )
+    )
+    df_substitution.to_excel(f"{path_folder_output}summary__substitution.xlsx")
+
+    if flag_perform_assembly:  # perform assembly if the flag is on
         pass
-        
-    
-    
-    
-
```

### Comparing `biobookshelf-0.2.2/biobookshelf/PDB/pdb.py` & `biobookshelf-0.2.3/biobookshelf/PDB/pdb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,105 @@
 import numpy as np
 import pandas as pd
-from io import StringIO 
-import collections # for external function
+from io import StringIO
+import collections  # for external function
 from copy import deepcopy
 
 # import internal functions
-def PD_Select( df, deselect = False, ** dict_select ) :
-    ''' Select and filter rows of df according to the given dict_select. If 'deselect' is set to True, deselect rows according to the given dict_select  Usage example : PANDAS_Select( df_meta_imid_ubi, dict(  Data_Type = [ 'Proteome', 'Ubi_Profiling' ], Value_Type = 'log2fc' ) ) '''
-    for col, query in dict_select.items( ) :
-        if type( df ) is pd.Series :
-            data_values = df.index.values if col == 'index' else df.values # select values or indices of a given pd.Series
-        elif type( df ) is pd.DataFrame : 
-            if col not in df.columns.values and col != 'index' :
-                print( "'{}' does not exist in columns of a given DataFrame".format( col ) )
+def PD_Select(df, deselect=False, **dict_select):
+    """Select and filter rows of df according to the given dict_select. If 'deselect' is set to True, deselect rows according to the given dict_select  Usage example : PANDAS_Select( df_meta_imid_ubi, dict(  Data_Type = [ 'Proteome', 'Ubi_Profiling' ], Value_Type = 'log2fc' ) )"""
+    for col, query in dict_select.items():
+        if type(df) is pd.Series:
+            data_values = (
+                df.index.values if col == "index" else df.values
+            )  # select values or indices of a given pd.Series
+        elif type(df) is pd.DataFrame:
+            if col not in df.columns.values and col != "index":
+                print("'{}' does not exist in columns of a given DataFrame".format(col))
                 continue
-            data_values = df.index.values if col == 'index' else df[ col ].values
-        else :
-            print( '[INVALID INPUT]: Inputs should be DataFrame or Series' )
+            data_values = df.index.values if col == "index" else df[col].values
+        else:
+            print("[INVALID INPUT]: Inputs should be DataFrame or Series")
             return -1
-        if isinstance( query, ( list, tuple, np.ndarray, set ) ) : # if data to be selected is iterable
-            query = set( query ) if isinstance( query, ( list, tuple, np.ndarray ) ) else query  # convert query into set
-            df = df[ list( False if data_value in query else True for data_value in data_values ) ] if deselect else df[ list( True if data_value in query else False for data_value in data_values ) ]
-        else :
-            df = df[ data_values != query ] if deselect else df[ data_values == query ]
+        if isinstance(
+            query, (list, tuple, np.ndarray, set)
+        ):  # if data to be selected is iterable
+            query = (
+                set(query) if isinstance(query, (list, tuple, np.ndarray)) else query
+            )  # convert query into set
+            df = (
+                df[
+                    list(
+                        False if data_value in query else True
+                        for data_value in data_values
+                    )
+                ]
+                if deselect
+                else df[
+                    list(
+                        True if data_value in query else False
+                        for data_value in data_values
+                    )
+                ]
+            )
+        else:
+            df = df[data_values != query] if deselect else df[data_values == query]
     return df
 
-def LIST_COUNT( iterable, return_series = True, duplicate_filter = 2, dropna = True, sort_series_by_values = True, convert_tuple_to_string = False ) :
-    ''' 
+
+def LIST_COUNT(
+    iterable,
+    return_series=True,
+    duplicate_filter=2,
+    dropna=True,
+    sort_series_by_values=True,
+    convert_tuple_to_string=False,
+):
+    """
     # 20210224
-    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more. '''
-    if dropna and isinstance( iterable, pd.Series ) : iterable = iterable.dropna( ) # if dropna is set to 'True', dropn NaN values before counting
-    if isinstance( next( iterable.__iter__( ) ), ( np.ndarray, list ) ) : iterable = list( map( tuple, iterable ) ) # if value is non-hashable list of numpy array, convert a value to a hashable format, tuple
-    dict_counted = COUNTER( iterable )
-    if convert_tuple_to_string : # if 'convert_tuple_to_string' is True and values in a given list are tuples, convert tuples into string
-        dict_counted__tuple_converted_to_string = dict( )
-        for key in dict_counted :
-            value = dict_counted[ key ]
-            if isinstance( key, ( tuple ) ) : dict_counted__tuple_converted_to_string[ ( '{}, ' * len( key ) )[ : -2 ].format( * key ) ] = value # convert tuple into string concatanated with ', '
-            else : dict_counted__tuple_converted_to_string[ key ] = value
+    return a dictionary where key = each element in a given list, value = counts of the element in the list. if 'duplicate_filter' is not None, return entries that are duplicated 'duplicate_filter' times or more."""
+    if dropna and isinstance(iterable, pd.Series):
+        iterable = (
+            iterable.dropna()
+        )  # if dropna is set to 'True', dropn NaN values before counting
+    if isinstance(next(iterable.__iter__()), (np.ndarray, list)):
+        iterable = list(
+            map(tuple, iterable)
+        )  # if value is non-hashable list of numpy array, convert a value to a hashable format, tuple
+    dict_counted = COUNTER(iterable)
+    if (
+        convert_tuple_to_string
+    ):  # if 'convert_tuple_to_string' is True and values in a given list are tuples, convert tuples into string
+        dict_counted__tuple_converted_to_string = dict()
+        for key in dict_counted:
+            value = dict_counted[key]
+            if isinstance(key, (tuple)):
+                dict_counted__tuple_converted_to_string[
+                    ("{}, " * len(key))[:-2].format(*key)
+                ] = value  # convert tuple into string concatanated with ', '
+            else:
+                dict_counted__tuple_converted_to_string[key] = value
         dict_counted = dict_counted__tuple_converted_to_string
-    if return_series :
-        s_counted = pd.Series( dict_counted )
-        if duplicate_filter is not None : s_counted = s_counted[ s_counted >= duplicate_filter ]
-        if sort_series_by_values : s_counted = s_counted.sort_values( ascending = False )
+    if return_series:
+        s_counted = pd.Series(dict_counted)
+        if duplicate_filter is not None:
+            s_counted = s_counted[s_counted >= duplicate_filter]
+        if sort_series_by_values:
+            s_counted = s_counted.sort_values(ascending=False)
         return s_counted
-    else : return dict_counted
+    else:
+        return dict_counted
+
 
 # In[7]:
 
 
-df_meta_pdb_format = pd.read_csv( StringIO( '''Columns	Data	Justification	Data Type
+df_meta_pdb_format = pd.read_csv(
+    StringIO(
+        """Columns	Data	Justification	Data Type
 1-6	ATOM_or_HETATM	.	character
 7-11	Atom_serial_number	right	integer
 13-16	Atom_name	left*	character
 17	Alternate_location_indicator		character
 18-20	Residue_name	right	character
 22	Chain_identifier		character
 23-26	Residue_sequence_number	right	integer
@@ -61,21 +107,26 @@
 31-38	X_orthogonal_Å_coordinate	right	real (8.3)
 39-46	Y_orthogonal_Å_coordinate	right	real (8.3)
 47-54	Z_orthogonal_Å_coordinate	right	real (8.3)
 55-60	Occupancy	right	real (6.2)
 61-66	Temperature_factor	right	real (6.2)
 73-76	Segment_identifier	left	character
 77-78	Element_symbol	right	character
-79-80	Charge	.	character''' ), sep = '\t' )
+79-80	Charge	.	character"""
+    ),
+    sep="\t",
+)
 
 
 # In[3]:
 
 
-df_amino_acids = pd.read_csv( StringIO( '''Amino_acid	Letter_code__3	Letter_code__1	Class	Polarity	Charge__at_pH_7_4	Hydropathy_index	Molar_absorptivity__Wavelength__λmax__nm_	Molar_absorptivity__Coefficient__ε__mM_1·cm_1_	Molecular_mass	Abundance_in_proteins___Percent___129_	Standard_genetic_coding__IUPAC_notation	MaxASA__Tien_et_al__2013__theor__	MaxASA__Tien_et_al__2013__emp__	MaxASA__Miller_et_al__1987	MaxASA__Rose_et_al__1985
+df_amino_acids = pd.read_csv(
+    StringIO(
+        """Amino_acid	Letter_code__3	Letter_code__1	Class	Polarity	Charge__at_pH_7_4	Hydropathy_index	Molar_absorptivity__Wavelength__λmax__nm_	Molar_absorptivity__Coefficient__ε__mM_1·cm_1_	Molecular_mass	Abundance_in_proteins___Percent___129_	Standard_genetic_coding__IUPAC_notation	MaxASA__Tien_et_al__2013__theor__	MaxASA__Tien_et_al__2013__emp__	MaxASA__Miller_et_al__1987	MaxASA__Rose_et_al__1985
 Alanine	Ala	A	Aliphatic	Nonpolar	Neutral	1.8			89.094	8.76	GCN	129.0	121.0	113.0	118.1
 Arginine	Arg	R	Basic	Basic polar	Positive	−4.5			174.203	5.78	MGR, CGY (coding codons can also be expressed by: CGN, AGR)	274.0	265.0	241.0	256.0
 Asparagine	Asn	N	Amide	Polar	Neutral	−3.5			132.119	3.93	AAY	195.0	187.0	158.0	165.5
 Aspartate	Asp	D	Acid	Acidic polar	Negative	−3.5			133.10399999999998	5.49	GAY	193.0	187.0	151.0	158.7
 Cysteine	Cys	C	Sulfuric	Nonpolar	Neutral	2.5	250	0.3	121.154	1.38	UGY	167.0	148.0	140.0	146.1
 Glutamate	Glu	E	Acid	Acidic polar	Negative	−3.5			147.131	6.32	GAR	223.0	214.0	183.0	186.2
 Glutamine	Gln	Q	Amide	Polar	Neutral	−3.5			146.14600000000002	3.9	CAR	225.0	214.0	189.0	193.2
@@ -87,15 +138,18 @@
 Methionine	Met	M	Sulfuric	Nonpolar	Neutral	1.9			149.208	2.32	AUG	224.0	203.0	204.0	203.4
 Phenylalanine	Phe	F	Aromatic	Nonpolar	Neutral	2.8	257, 206, 188	0.2, 9.3, 60.0	165.192	3.87	UUY	240.0	228.0	218.0	222.8
 Proline	Pro	P	Cyclic	Nonpolar	Neutral	−1.6			115.132	5.02	CCN	159.0	154.0	143.0	146.8
 Serine	Ser	S	Hydroxylic	Polar	Neutral	−0.8			105.09299999999999	7.14	UCN, AGY	155.0	143.0	122.0	129.8
 Threonine	Thr	T	Hydroxylic	Polar	Neutral	−0.7			119.119	5.53	ACN	172.0	163.0	146.0	152.5
 Tryptophan	Trp	W	Aromatic	Nonpolar	Neutral	−0.9	280, 219	5.6, 47.0	204.22799999999998	1.25	UGG	285.0	264.0	259.0	266.3
 Tyrosine	Tyr	Y	Aromatic	Polar	Neutral	−1.3	274, 222, 193	1.4, 8.0, 48.0	181.19099999999997	2.91	UAY	263.0	255.0	229.0	236.8
-Valine	Val	V	Aliphatic	Nonpolar	Neutral	4.2			117.148	6.73	GUN	174.0	165.0	160.0	164.5''' ), sep = '\t' )
+Valine	Val	V	Aliphatic	Nonpolar	Neutral	4.2			117.148	6.73	GUN	174.0	165.0	160.0	164.5"""
+    ),
+    sep="\t",
+)
 
 
 # In[4]:
 
 
 df_amino_acids
 
@@ -105,264 +159,487 @@
 
 """def Parse_ATOM_or_HETATM_line( line ) :
     '''  parse a given line (should be ATOM or HETATM records) and return parsed data values as a numpy array (dtype = object)  '''
     try :
         arr_values = np.array( [ line[ 0 : 6 ].strip( ), int( line[ 6 : 11 ].strip( ) ), line[ 12 : 16 ].strip( ), line[ 16 ].strip( ), line[ 17 : 20 ].strip( ), line[ 21 ].strip( ), int( line[ 22 : 26 ].strip( ) ), line[ 26 ].strip( ), float( line[ 30 : 38 ].strip( ) ), float( line[ 39 : 46 ].strip( ) ), float( line[ 46 : 54 ].strip( ) ), float( line[ 54 : 60 ].strip( ) ), float( line[ 60 : 66 ].strip( ) ), line[ 72 : 76 ].strip( ), line[ 76 : 78 ].strip( ), line[ 78 : 80 ].strip( ) ], dtype = object )
     except : # for ZDOCK result (contain four wrongly placed columns containing real values)
         arr_values = np.array( [ line[ 0 : 6 ].strip( ), int( line[ 6 : 11 ].strip( ) ), line[ 12 : 16 ].strip( ), line[ 16 ].strip( ), line[ 17 : 20 ].strip( ), line[ 21 ].strip( ), int( line[ 22 : 26 ].strip( ) ), line[ 26 ].strip( ), float( line[ 30 : 38 ].strip( ) ), float( line[ 39 : 46 ].strip( ) ), float( line[ 46 : 54 ].strip( ) ), line[ 54 : 60 ].strip( ), line[ 60 : 66 ].strip( ), line[ 72 : 76 ].strip( ), line[ 76 : 78 ].strip( ), line[ 78 : 80 ].strip( ) ], dtype = object )
-    return arr_values""" # 20191104
+    return arr_values"""  # 20191104
 """def Compose_ATOM_or_HETATM_line( arr_values ) :
     '''  compose a ATOM or HETATM line from the output of 'Parse_ATOM_or_HETATM_line' (it is essentially a reverse operation of 'Parse_ATOM_or_HETATM_line') '''
-    return "{:<6s}{:>5d} {:<4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}      {:<3s}{:>3s}{:2s}".format( * arr_values )""" # 20191104
+    return "{:<6s}{:>5d} {:<4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}      {:<3s}{:>3s}{:2s}".format( * arr_values )"""  # 20191104
 
 
 # In[4]:
 
 
-def Parse_ATOM_or_HETATM_line( line ) :
-    '''  # 2021-04-27 11:12:31 
-    parse a given line (should be ATOM or HETATM records) and return parsed data values as a numpy array (dtype = object) Parse only until xyz coordinates (because later columns are somewhat variable across different docking servers)  '''
+def Parse_ATOM_or_HETATM_line(line):
+    """# 2021-04-27 11:12:31
+    parse a given line (should be ATOM or HETATM records) and return parsed data values as a numpy array (dtype = object) Parse only until xyz coordinates (because later columns are somewhat variable across different docking servers)"""
     # parse optional fields based on the length of the entry
-    value = '' if len( line ) < 60 else line[ 54 : 60 ].strip( )
-    float_occupancy = np.nan if len( value ) == 0 else float( value )
-    value = '' if len( line ) < 66 else line[ 60 : 66 ].strip( )
-    float_temperature_factor = np.nan if len( value ) == 0 else float( value )
-    str_id_segment = '' if len( line ) < 76 else line[ 72 : 76 ].strip( )
-    str_symbol_element = '' if len( line ) < 78 else line[ 76 : 78 ].strip( )
-    str_change = '' if len( line ) < 80 else line[ 78 : 80 ].strip( )
+    value = "" if len(line) < 60 else line[54:60].strip()
+    float_occupancy = np.nan if len(value) == 0 else float(value)
+    value = "" if len(line) < 66 else line[60:66].strip()
+    float_temperature_factor = np.nan if len(value) == 0 else float(value)
+    str_id_segment = "" if len(line) < 76 else line[72:76].strip()
+    str_symbol_element = "" if len(line) < 78 else line[76:78].strip()
+    str_change = "" if len(line) < 80 else line[78:80].strip()
     # parse required fields
-    arr = np.array( [ line[ 0 : 6 ].strip( ), None if "*" in line[ 6 : 11 ] else int( line[ 6 : 11 ].strip( ) ), line[ 12 : 16 ].strip( ), line[ 16 ].strip( ), line[ 17 : 20 ].strip( ), line[ 21 ].strip( ), int( line[ 22 : 26 ].strip( ) ), line[ 26 ].strip( ), float( line[ 30 : 38 ].strip( ) ), float( line[ 39 : 46 ].strip( ) ), float( line[ 46 : 54 ].strip( ) ), float_occupancy, float_temperature_factor, str_id_segment, str_symbol_element, str_change ], dtype = object )
+    arr = np.array(
+        [
+            line[0:6].strip(),
+            None if "*" in line[6:11] else int(line[6:11].strip()),
+            line[12:16].strip(),
+            line[16].strip(),
+            line[17:20].strip(),
+            line[21].strip(),
+            int(line[22:26].strip()),
+            line[26].strip(),
+            float(line[30:38].strip()),
+            float(line[39:46].strip()),
+            float(line[46:54].strip()),
+            float_occupancy,
+            float_temperature_factor,
+            str_id_segment,
+            str_symbol_element,
+            str_change,
+        ],
+        dtype=object,
+    )
     # atom_number might contain non-integer characters ('*****') when the atom_number is > 99999 (e.g. pdb files from 'SWISS-MODEL repositories')
     return arr
 
 
 # In[11]:
 
 
-def Compose_ATOM_or_HETATM_line( arr_values ) :
-    '''  # 2020-12-14 00:08:19 
-    compose a ATOM or HETATM line from the output of 'Parse_ATOM_or_HETATM_line' (it is essentially a reverse operation of 'Parse_ATOM_or_HETATM_line') '''
-    arr_values = deepcopy( arr_values )
-    if len( df_meta_pdb_format ) > len( df_meta_pdb_format ) :
-        arr_values = arr_values[ : len( df_meta_pdb_format ) ]
-    arr_values[ 11 ] = "      " if isinstance( arr_values[ 11 ], ( str ) ) or np.isnan( arr_values[ 11 ] ) else "{:>6.2f}".format( arr_values[ 11 ] )
-    arr_values[ 12 ] = "      " if isinstance( arr_values[ 12 ], ( str ) ) or np.isnan( arr_values[ 12 ] ) else "{:>6.2f}".format( arr_values[ 12 ] )
-    
-    atom_name = arr_values[ 2 ]
-    if atom_name[ 0 ] in "ONCHSP" and len( atom_name ) < 4 : # based on description 'Atom names start with element symbols right-justified in columns 13-14 as permitted by the length of the name'
-        return "{:<6s}{:>5d}  {:<3s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6s}{:>6s}      {:<4s}{:>2s}{:<2s}".format( * arr_values )
-    else :
-        return "{:<6s}{:>5d} {:<4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6s}{:>6s}      {:<4s}{:>2s}{:<2s}".format( * arr_values )
+def Compose_ATOM_or_HETATM_line(arr_values):
+    """# 2020-12-14 00:08:19
+    compose a ATOM or HETATM line from the output of 'Parse_ATOM_or_HETATM_line' (it is essentially a reverse operation of 'Parse_ATOM_or_HETATM_line')"""
+    arr_values = deepcopy(arr_values)
+    if len(df_meta_pdb_format) > len(df_meta_pdb_format):
+        arr_values = arr_values[: len(df_meta_pdb_format)]
+    arr_values[11] = (
+        "      "
+        if isinstance(arr_values[11], (str)) or np.isnan(arr_values[11])
+        else "{:>6.2f}".format(arr_values[11])
+    )
+    arr_values[12] = (
+        "      "
+        if isinstance(arr_values[12], (str)) or np.isnan(arr_values[12])
+        else "{:>6.2f}".format(arr_values[12])
+    )
+
+    atom_name = arr_values[2]
+    if (
+        atom_name[0] in "ONCHSP" and len(atom_name) < 4
+    ):  # based on description 'Atom names start with element symbols right-justified in columns 13-14 as permitted by the length of the name'
+        return "{:<6s}{:>5d}  {:<3s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6s}{:>6s}      {:<4s}{:>2s}{:<2s}".format(
+            *arr_values
+        )
+    else:
+        return "{:<6s}{:>5d} {:<4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6s}{:>6s}      {:<4s}{:>2s}{:<2s}".format(
+            *arr_values
+        )
 
 
 # In[ ]:
 
 
-def Read_Single_Module( path_file, enable_automatic_correction = False, verbose = False ) : # 2020-07-07 15:59:00 
-    '''   # 2021-04-27 11:25:12 
-    Read PDB file with a single module (one chain A and one chain B, etc), and return dataframes of ATOM and HETATM records. If missing chain identifiers are detected, reassign chain identifiers based on chain transitions inferred by residue_numbers  '''
-    if '/' in path_file : 
-        with open( path_file, 'r' ) as file :
-            l_lines = file.read( ).split( '\n' )
-    else : # if a given 'path_file' is not a directory (does not contain '/') read 'path_file' as a string
-        l_lines = path_file.split( '\n' )
-    l_lines = list( line for line in l_lines if 'HEADER' not in line and 'REMARK' not in line ) # remove header or remarks from the data
-    n_terminations = len( list( line for line in l_lines if 'TER' in line[ : 3 ] ) ) # count the number of terminations
+def Read_Single_Module(
+    path_file, enable_automatic_correction=False, verbose=False
+):  # 2020-07-07 15:59:00
+    """# 2021-04-27 11:25:12
+    Read PDB file with a single module (one chain A and one chain B, etc), and return dataframes of ATOM and HETATM records. If missing chain identifiers are detected, reassign chain identifiers based on chain transitions inferred by residue_numbers"""
+    if "/" in path_file:
+        with open(path_file, "r") as file:
+            l_lines = file.read().split("\n")
+    else:  # if a given 'path_file' is not a directory (does not contain '/') read 'path_file' as a string
+        l_lines = path_file.split("\n")
+    l_lines = list(
+        line for line in l_lines if "HEADER" not in line and "REMARK" not in line
+    )  # remove header or remarks from the data
+    n_terminations = len(
+        list(line for line in l_lines if "TER" in line[:3])
+    )  # count the number of terminations
     # parse all lines containing ATOM or HETATM records
-    l_arr = [ ]
-    for line in l_lines :
-        if 'ATOM' in line[ : 6 ] or 'HETATM' in line[ : 6 ] : # parse all lines containing ATOM or HETATM records
-            arr = Parse_ATOM_or_HETATM_line( line )
-            if arr[ 1 ] is None : # if atom_number contain invalid number 
-                arr[ 1 ] = l_arr[ -1 ][ 1 ] + 1 # set atom_number as previous_atom_number + 1
-            l_arr.append( arr )
-    if verbose : print( "{} lines of ATOM or HETATM and {} terminations are found".format( str( len( l_arr ) ), n_terminations ) )
-    df = pd.DataFrame( np.vstack( l_arr ), columns = df_meta_pdb_format.Data.values ).sort_values( [ 'Chain_identifier', 'Residue_sequence_number', 'Atom_serial_number' ], ignore_index = True )  # build dataframes of ATOM and HETATM records (except the five last data columns)
-    arr_index_chain_transition = np.where( np.diff( df.Residue_sequence_number.values ) < 0 )[ 0 ] # retrive array of row indices where chain transiton exist (where new chain starts) (values in arr_index_chain_transition indicates locations of new chain starts)
-    n_chains_in_pdb, n_chains_inferred = len( df.Chain_identifier.unique( ) ), len( arr_index_chain_transition ) + 1
-    if n_chains_in_pdb < n_chains_inferred and enable_automatic_correction : # detect error in chain identifier assignment and try to correct it
-        if verbose : print( "[Read_Single_Module] [ERROR:Chain Identifier Missing] {} chains were found in PDB files, but the redisue number trend says there are {} chain. Chain Identifiers will be re-assigned".format( str( n_chains_in_pdb ), str( n_chains_inferred ) ) )
-        arr_chain_identifier = np.full( len( df ), 'A' )
-        l_index_chain_transition = [ 0 ] + list( arr_index_chain_transition + 1 ) + [ len( df ) ]
-        for index, str_new_chain_identifier in zip( np.arange( n_chains_inferred ), 'ABCDEFGHIJKLMNOPQRSTUVWXYZ' ) :
-            arr_chain_identifier[ l_index_chain_transition[ index ] : l_index_chain_transition[ index + 1 ] ] = str_new_chain_identifier
+    l_arr = []
+    for line in l_lines:
+        if (
+            "ATOM" in line[:6] or "HETATM" in line[:6]
+        ):  # parse all lines containing ATOM or HETATM records
+            arr = Parse_ATOM_or_HETATM_line(line)
+            if arr[1] is None:  # if atom_number contain invalid number
+                arr[1] = l_arr[-1][1] + 1  # set atom_number as previous_atom_number + 1
+            l_arr.append(arr)
+    if verbose:
+        print(
+            "{} lines of ATOM or HETATM and {} terminations are found".format(
+                str(len(l_arr)), n_terminations
+            )
+        )
+    df = pd.DataFrame(
+        np.vstack(l_arr), columns=df_meta_pdb_format.Data.values
+    ).sort_values(
+        ["Chain_identifier", "Residue_sequence_number", "Atom_serial_number"],
+        ignore_index=True,
+    )  # build dataframes of ATOM and HETATM records (except the five last data columns)
+    arr_index_chain_transition = np.where(
+        np.diff(df.Residue_sequence_number.values) < 0
+    )[
+        0
+    ]  # retrive array of row indices where chain transiton exist (where new chain starts) (values in arr_index_chain_transition indicates locations of new chain starts)
+    n_chains_in_pdb, n_chains_inferred = (
+        len(df.Chain_identifier.unique()),
+        len(arr_index_chain_transition) + 1,
+    )
+    if (
+        n_chains_in_pdb < n_chains_inferred and enable_automatic_correction
+    ):  # detect error in chain identifier assignment and try to correct it
+        if verbose:
+            print(
+                "[Read_Single_Module] [ERROR:Chain Identifier Missing] {} chains were found in PDB files, but the redisue number trend says there are {} chain. Chain Identifiers will be re-assigned".format(
+                    str(n_chains_in_pdb), str(n_chains_inferred)
+                )
+            )
+        arr_chain_identifier = np.full(len(df), "A")
+        l_index_chain_transition = (
+            [0] + list(arr_index_chain_transition + 1) + [len(df)]
+        )
+        for index, str_new_chain_identifier in zip(
+            np.arange(n_chains_inferred), "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+        ):
+            arr_chain_identifier[
+                l_index_chain_transition[index] : l_index_chain_transition[index + 1]
+            ] = str_new_chain_identifier
         df.Chain_identifier = arr_chain_identifier
     return df
 
 
 # In[ ]:
 
 
-def Read_Multiple_Models( path_file ) : # 2020-11-27 16:27:07 
-    """ read pdb file of 'path_file' containing multiple models (CABS-Dock output 'clus' and 'replica' files) and return l_df """
-    l_df, l_l = list( ), list( )
-    with open( path_file ) as file : 
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 : break
-            if line[ : 5 ] == 'MODEL' :
-                name_model = line.strip( ).split( )[ 1 ]
-                l_l = list( )
-            elif 'HEADER' not in line and 'REMARK' not in line and ( 'ATOM' in line or 'HETATM' in line ) : # if current line contains ATOM or HETATM records
-                l_l.append( Parse_ATOM_or_HETATM_line( line ) )
-            elif line[ : 6 ] == 'ENDMDL' :
-                df = pd.DataFrame( l_l, columns = df_meta_pdb_format.Data.values ).sort_values( [ 'Chain_identifier', 'Residue_sequence_number', 'Atom_serial_number' ], ignore_index = True )
-                df[ 'MODEL' ] = name_model # assign id_model
-                l_l = list( )
-                l_df.append( df )
+def Read_Multiple_Models(path_file):  # 2020-11-27 16:27:07
+    """read pdb file of 'path_file' containing multiple models (CABS-Dock output 'clus' and 'replica' files) and return l_df"""
+    l_df, l_l = list(), list()
+    with open(path_file) as file:
+        while True:
+            line = file.readline()
+            if len(line) == 0:
+                break
+            if line[:5] == "MODEL":
+                name_model = line.strip().split()[1]
+                l_l = list()
+            elif (
+                "HEADER" not in line
+                and "REMARK" not in line
+                and ("ATOM" in line or "HETATM" in line)
+            ):  # if current line contains ATOM or HETATM records
+                l_l.append(Parse_ATOM_or_HETATM_line(line))
+            elif line[:6] == "ENDMDL":
+                df = pd.DataFrame(
+                    l_l, columns=df_meta_pdb_format.Data.values
+                ).sort_values(
+                    [
+                        "Chain_identifier",
+                        "Residue_sequence_number",
+                        "Atom_serial_number",
+                    ],
+                    ignore_index=True,
+                )
+                df["MODEL"] = name_model  # assign id_model
+                l_l = list()
+                l_df.append(df)
     return l_df
 
 
 # In[ ]:
 
 
-def Split_Multiple_Models( path_file, path_folder_output = None ) : # 2020-11-30 03:07:27 
-    """ read pdb file of 'path_file' containing multiple models (CABS-Dock output 'clus' and 'replica' files) and split the file into individual models without parsing and composing data values.
-    'path_folder_output' : output directory of split files. by default, it is where the pdb file is located """
-    path_folder, name_file = path_file.rsplit( '/', 1 )
-    if path_folder_output is None : path_folder_output = path_folder # set default folder
-    path_prefix_output = path_folder_output + name_file.rsplit( '.', 1 )[ 0 ]
-    flag_writing = False # flag for writing
-    with open( path_file ) as file : 
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 : break
-            if line[ : 5 ] == 'MODEL' :
-                name_model = line.strip( ).split( )[ 1 ]
-                newfile = open( path_prefix_output + '.model_{name_model}.pdb'.format( name_model = name_model ), 'w' )
+def Split_Multiple_Models(path_file, path_folder_output=None):  # 2020-11-30 03:07:27
+    """read pdb file of 'path_file' containing multiple models (CABS-Dock output 'clus' and 'replica' files) and split the file into individual models without parsing and composing data values.
+    'path_folder_output' : output directory of split files. by default, it is where the pdb file is located"""
+    path_folder, name_file = path_file.rsplit("/", 1)
+    if path_folder_output is None:
+        path_folder_output = path_folder  # set default folder
+    path_prefix_output = path_folder_output + name_file.rsplit(".", 1)[0]
+    flag_writing = False  # flag for writing
+    with open(path_file) as file:
+        while True:
+            line = file.readline()
+            if len(line) == 0:
+                break
+            if line[:5] == "MODEL":
+                name_model = line.strip().split()[1]
+                newfile = open(
+                    path_prefix_output
+                    + ".model_{name_model}.pdb".format(name_model=name_model),
+                    "w",
+                )
                 flag_writing = True
-                newfile.write( line )
-            elif 'HEADER' not in line and 'REMARK' not in line and ( 'ATOM' in line or 'HETATM' in line ) and flag_writing : # if current line contains ATOM or HETATM records and currently a file is opened for writing
-                newfile.write( line )
-            elif line[ : 6 ] == 'ENDMDL' :
-                newfile.close( )
+                newfile.write(line)
+            elif (
+                "HEADER" not in line
+                and "REMARK" not in line
+                and ("ATOM" in line or "HETATM" in line)
+                and flag_writing
+            ):  # if current line contains ATOM or HETATM records and currently a file is opened for writing
+                newfile.write(line)
+            elif line[:6] == "ENDMDL":
+                newfile.close()
                 flag_writing = False
 
 
 # In[4]:
 
 
-def Write_Single_Module( df, path_file, verbose = False ) : # 2020-07-07 15:59:03 
-    '''   Add a 'TER' record automatically at the end of each chain, and write values in a given PDB dataframe (output of 'Read_Single_Module' function) as a PDB text file in the given directory 'path_file'.  '''
-    df = df.sort_values( [ 'Chain_identifier', 'Residue_sequence_number', 'Atom_name' ] ) # sort df before adding 'TER' records after the end of each chain and save the PDB dataframe as a PDB text file 
-    df.Atom_serial_number = np.arange( 1, len( df ) + 1 ) # renumber 'Atom_serial_number'
-    l_line = list( map( Compose_ATOM_or_HETATM_line, df.values ) ) # convert values in dataframe to string according to PDB text format.
-    l_index_chain_transition = [ 0 ] + list( np.where( np.diff( df.Residue_sequence_number.values ) < 0 )[ 0 ] + 1 ) + [ len( df ) ] # retrive array of row indices where where new chain starts
-    n_ter = len( l_index_chain_transition ) - 1
-    if verbose : print( "{} chains detected. 'TER' record will be added".format( n_ter ) )
-    l_line_with_ter = list( ) # add 'TER' records
-    for index in np.arange( n_ter ) :
-        l_line_with_ter.extend( l_line[ l_index_chain_transition[ index ] : l_index_chain_transition[ index + 1 ] ] + [ 'TER' ] )
-    if '.pdb' not in path_file.lower( ) : path_file += '.pdb' # add pdb file extension if it does not exist in the given directory to the file to be written
-    with open( path_file, 'w' ) as file : file.write( '\n'.join( l_line_with_ter ) + '\nEND\n' )
+def Write_Single_Module(df, path_file, verbose=False):  # 2020-07-07 15:59:03
+    """Add a 'TER' record automatically at the end of each chain, and write values in a given PDB dataframe (output of 'Read_Single_Module' function) as a PDB text file in the given directory 'path_file'."""
+    df = df.sort_values(
+        ["Chain_identifier", "Residue_sequence_number", "Atom_name"]
+    )  # sort df before adding 'TER' records after the end of each chain and save the PDB dataframe as a PDB text file
+    df.Atom_serial_number = np.arange(1, len(df) + 1)  # renumber 'Atom_serial_number'
+    l_line = list(
+        map(Compose_ATOM_or_HETATM_line, df.values)
+    )  # convert values in dataframe to string according to PDB text format.
+    l_index_chain_transition = (
+        [0]
+        + list(np.where(np.diff(df.Residue_sequence_number.values) < 0)[0] + 1)
+        + [len(df)]
+    )  # retrive array of row indices where where new chain starts
+    n_ter = len(l_index_chain_transition) - 1
+    if verbose:
+        print("{} chains detected. 'TER' record will be added".format(n_ter))
+    l_line_with_ter = list()  # add 'TER' records
+    for index in np.arange(n_ter):
+        l_line_with_ter.extend(
+            l_line[
+                l_index_chain_transition[index] : l_index_chain_transition[index + 1]
+            ]
+            + ["TER"]
+        )
+    if ".pdb" not in path_file.lower():
+        path_file += ".pdb"  # add pdb file extension if it does not exist in the given directory to the file to be written
+    with open(path_file, "w") as file:
+        file.write("\n".join(l_line_with_ter) + "\nEND\n")
 
 
 # In[ ]:
 
 
-def Retrive_Signatures_of_atoms( df, l_col = [ 'Atom_name', 'Residue_name', 'Chain_identifier', 'Residue_sequence_number' ] ) :
-    '''  Input : output dataframe of 'Read_Single_Module'. Output : a set of signatures of atoms (tuple of values contained in the given array of columns, default = [ 'Atom_name', 'Residue_name', 'Chain_identifier', 'Residue_sequence_number' ] )  '''
-    arr_atoms = df[ l_col ].values
-    s_duplicated_signatures = L.Count( list( tuple( arr_values ) for arr_values in arr_atoms ) )
-    if len( s_duplicated_signatures ) > 0 :
-        print( '{} duplicated signatures of atom were found'.format( str( len( s_duplicated_signatures ) ) ) )
-    return set( tuple( arr_values ) for arr_values in arr_atoms )
+def Retrive_Signatures_of_atoms(
+    df,
+    l_col=["Atom_name", "Residue_name", "Chain_identifier", "Residue_sequence_number"],
+):
+    """Input : output dataframe of 'Read_Single_Module'. Output : a set of signatures of atoms (tuple of values contained in the given array of columns, default = [ 'Atom_name', 'Residue_name', 'Chain_identifier', 'Residue_sequence_number' ] )"""
+    arr_atoms = df[l_col].values
+    s_duplicated_signatures = L.Count(
+        list(tuple(arr_values) for arr_values in arr_atoms)
+    )
+    if len(s_duplicated_signatures) > 0:
+        print(
+            "{} duplicated signatures of atom were found".format(
+                str(len(s_duplicated_signatures))
+            )
+        )
+    return set(tuple(arr_values) for arr_values in arr_atoms)
 
 
 # In[ ]:
 
 
-def Identify_Protein_and_Assign_Chain_identifier( df, ** dict_identifiable_chains ) :
-    '''  Input : output dataframe of 'Read_Single_Module' as 'df' and keyworded arguments for desired chain identifier for each identifiable protein (example input: A = { 'start' : { 'ILE' : 47 }, 323 : 'CYS', 326 : 'CYS', 391 : 'CYS', 394 : 'CYS' } )
-    Output : output dataframe of 'Read_Single_Module', but with modified chain identifiers for each identified proteins  '''
-    l_df_a_chain = list( )
-    for char_chain_identifier in df.Chain_identifier.unique( ) : # resolve merged multiper proteins (for example ACAT1 dimer)
-        df_a_chain = PD.Select( df, Chain_identifier = char_chain_identifier )
-        arr_residue_num = df_a_chain.Residue_sequence_number.unique( )
-        n_residues = len( arr_residue_num )
-        if n_residues == 391 * 2 : # for HawkDock ACAT1 dimer (their residue numbers are renumbered and needed to be separated)
-            print( '[Identify_Protein_and_Assign_Chain_identifier] ACAT1 Dimer Splited' )
-            df_a_chain.loc[ df_a_chain.Residue_sequence_number > 391, 'Chain_identifier' ] = 'Splited'
-        l_df_a_chain.append( df_a_chain )
-    df = pd.concat( l_df_a_chain )
-    l_df_a_chain = list( )
-    for char_chain_identifier in df.Chain_identifier.unique( ) :    
-        df_a_chain = PD.Select( df, Chain_identifier = char_chain_identifier )
-        for char_desired_chain_identifier, dict_sequence_signature in dict_identifiable_chains.items( ) :
-            dict_sequence_signature = deepcopy( dict_sequence_signature )
-            str_start_residue, int_start_residue_num = list( dict_sequence_signature.pop( 'start' ).items( ) )[ 0 ] # retrive given start residue number and name for the unique chain profile ('dict_sequence_signature') 
-            int_min_residue_num = df_a_chain.Residue_sequence_number.min( )
-            if int_min_residue_num != int_start_residue_num and PD.Select( df_a_chain, Residue_sequence_number = int_min_residue_num ).Residue_name.values[ 0 ] == str_start_residue : # if the starting residue names are the same but the starting residue numbers are different, re-number residue numbers of the chain
-                print( "\t[Identify_Protein_and_Assign_Chain_identifier] [NOTE] the given start residue name and start residue name in the chain is the same while start residue numbers are different, and residue numbers will be re-numbered" )
-                df_a_chain.Residue_sequence_number = df_a_chain.Residue_sequence_number + ( int_start_residue_num - int_min_residue_num )
-            if np.sum( list( PD.Select( df_a_chain, Residue_sequence_number = int_residue_number ).Residue_name.values[ 0 ] != str_residue_name if len( PD.Select( df_a_chain, Residue_sequence_number = int_residue_number ) ) > 0 else True for int_residue_number, str_residue_name in dict_sequence_signature.items( ) ) ) == 0 :
+def Identify_Protein_and_Assign_Chain_identifier(df, **dict_identifiable_chains):
+    """Input : output dataframe of 'Read_Single_Module' as 'df' and keyworded arguments for desired chain identifier for each identifiable protein (example input: A = { 'start' : { 'ILE' : 47 }, 323 : 'CYS', 326 : 'CYS', 391 : 'CYS', 394 : 'CYS' } )
+    Output : output dataframe of 'Read_Single_Module', but with modified chain identifiers for each identified proteins"""
+    l_df_a_chain = list()
+    for (
+        char_chain_identifier
+    ) in (
+        df.Chain_identifier.unique()
+    ):  # resolve merged multiper proteins (for example ACAT1 dimer)
+        df_a_chain = PD.Select(df, Chain_identifier=char_chain_identifier)
+        arr_residue_num = df_a_chain.Residue_sequence_number.unique()
+        n_residues = len(arr_residue_num)
+        if (
+            n_residues == 391 * 2
+        ):  # for HawkDock ACAT1 dimer (their residue numbers are renumbered and needed to be separated)
+            print("[Identify_Protein_and_Assign_Chain_identifier] ACAT1 Dimer Splited")
+            df_a_chain.loc[
+                df_a_chain.Residue_sequence_number > 391, "Chain_identifier"
+            ] = "Splited"
+        l_df_a_chain.append(df_a_chain)
+    df = pd.concat(l_df_a_chain)
+    l_df_a_chain = list()
+    for char_chain_identifier in df.Chain_identifier.unique():
+        df_a_chain = PD.Select(df, Chain_identifier=char_chain_identifier)
+        for (
+            char_desired_chain_identifier,
+            dict_sequence_signature,
+        ) in dict_identifiable_chains.items():
+            dict_sequence_signature = deepcopy(dict_sequence_signature)
+            str_start_residue, int_start_residue_num = list(
+                dict_sequence_signature.pop("start").items()
+            )[
+                0
+            ]  # retrive given start residue number and name for the unique chain profile ('dict_sequence_signature')
+            int_min_residue_num = df_a_chain.Residue_sequence_number.min()
+            if (
+                int_min_residue_num != int_start_residue_num
+                and PD.Select(
+                    df_a_chain, Residue_sequence_number=int_min_residue_num
+                ).Residue_name.values[0]
+                == str_start_residue
+            ):  # if the starting residue names are the same but the starting residue numbers are different, re-number residue numbers of the chain
+                print(
+                    "\t[Identify_Protein_and_Assign_Chain_identifier] [NOTE] the given start residue name and start residue name in the chain is the same while start residue numbers are different, and residue numbers will be re-numbered"
+                )
+                df_a_chain.Residue_sequence_number = (
+                    df_a_chain.Residue_sequence_number
+                    + (int_start_residue_num - int_min_residue_num)
+                )
+            if (
+                np.sum(
+                    list(
+                        PD.Select(
+                            df_a_chain, Residue_sequence_number=int_residue_number
+                        ).Residue_name.values[0]
+                        != str_residue_name
+                        if len(
+                            PD.Select(
+                                df_a_chain, Residue_sequence_number=int_residue_number
+                            )
+                        )
+                        > 0
+                        else True
+                        for int_residue_number, str_residue_name in dict_sequence_signature.items()
+                    )
+                )
+                == 0
+            ):
                 df_a_chain.Chain_identifier = char_desired_chain_identifier
-                l_df_a_chain.append( df_a_chain )
-                dict_identifiable_chains.pop( char_desired_chain_identifier )
+                l_df_a_chain.append(df_a_chain)
+                dict_identifiable_chains.pop(char_desired_chain_identifier)
                 break
-    return pd.concat( l_df_a_chain )
+    return pd.concat(l_df_a_chain)
 
 
 # In[ ]:
 
 
-def Clean_Minimal( path_file_pdb, path_file_pdb_clean, l_chain_id = None, remove_hetatm = True ) : # 2020-11-30 01:57:22 
-    ''' Clean a pdb (from RCSB PDB) in a minimal fashion
+def Clean_Minimal(
+    path_file_pdb, path_file_pdb_clean, l_chain_id=None, remove_hetatm=True
+):  # 2020-11-30 01:57:22
+    """Clean a pdb (from RCSB PDB) in a minimal fashion
     'l_chain_id' : list of chain_ids to retain. by default, retain all chain_ids
-    'remove_hetatm' : remove hetatm lines '''
-    if l_chain_id is not None : set_chain_id = set( l_chain_id )
-    with open( path_file_pdb_clean, 'w' ) as newfile :
-        with open( path_file_pdb ) as file :
-            while True :
-                line = file.readline( )
-                if len( line ) == 0 : break
-                if remove_hetatm :
-                    if line[ : 6 ] == 'HETATM' : continue
-                if l_chain_id is not None :
-                    if line[ 21 ] not in set_chain_id : continue
-                newfile.write( line )
+    'remove_hetatm' : remove hetatm lines"""
+    if l_chain_id is not None:
+        set_chain_id = set(l_chain_id)
+    with open(path_file_pdb_clean, "w") as newfile:
+        with open(path_file_pdb) as file:
+            while True:
+                line = file.readline()
+                if len(line) == 0:
+                    break
+                if remove_hetatm:
+                    if line[:6] == "HETATM":
+                        continue
+                if l_chain_id is not None:
+                    if line[21] not in set_chain_id:
+                        continue
+                newfile.write(line)
 
 
 # In[ ]:
 
 
-def Dissociate( df, * l_l_chains, float_distance_for_dissociation = 1000 ) :
-    '''  # 2020-12-21 23:02:46 
+def Dissociate(df, *l_l_chains, float_distance_for_dissociation=1000):
+    """# 2020-12-21 23:02:46
     Move apart the parts defined by a list of lists of chain_ids 'l_l_chains' by 'float_distance_for_dissociation' from the center of the system.
     float_distance_for_dissociation = 1000 # distance used for dissociation of each 'part'
-    '''
-    l_col_coord = [ 'X_orthogonal_Å_coordinate', 'Y_orthogonal_Å_coordinate', 'Z_orthogonal_Å_coordinate' ]
-    df = deepcopy( df )
-    
-    coord_center = df[ l_col_coord ].values.mean( axis = 0 ) # retrieve coordinates of center (average coordinates of all atoms)
-    l_df = list( )
-    for l_chains in l_l_chains :
-        df_part = PD.Select( df, Chain_identifier = l_chains ) # subset pdb with the current list of chain_ids
-        coord_center_part = df_part[ l_col_coord ].values.mean( axis = 0 ) # retrieve coordinates of center of the current part (average coordinates of all atoms)
+    """
+    l_col_coord = [
+        "X_orthogonal_Å_coordinate",
+        "Y_orthogonal_Å_coordinate",
+        "Z_orthogonal_Å_coordinate",
+    ]
+    df = deepcopy(df)
+
+    coord_center = df[l_col_coord].values.mean(
+        axis=0
+    )  # retrieve coordinates of center (average coordinates of all atoms)
+    l_df = list()
+    for l_chains in l_l_chains:
+        df_part = PD.Select(
+            df, Chain_identifier=l_chains
+        )  # subset pdb with the current list of chain_ids
+        coord_center_part = df_part[l_col_coord].values.mean(
+            axis=0
+        )  # retrieve coordinates of center of the current part (average coordinates of all atoms)
         vector_center_part_from_center_system = coord_center_part - coord_center
-        unit_vector_center_part_from_center_system = vector_center_part_from_center_system / sum( vector_center_part_from_center_system ** 2 ) ** 0.5 # retrieve unit vector of the centor of the part relative to the center of the system
-        vector_move = unit_vector_center_part_from_center_system * float_distance_for_dissociation
-        df_part.loc[ :, l_col_coord ] = df_part[ l_col_coord ].values + vector_move # move the part by the unit vector times 'float_distance_for_dissociation'
-        l_df.append( df_part )
-    df_moved = pd.concat( l_df ) # combine moved parts
+        unit_vector_center_part_from_center_system = (
+            vector_center_part_from_center_system
+            / sum(vector_center_part_from_center_system**2) ** 0.5
+        )  # retrieve unit vector of the centor of the part relative to the center of the system
+        vector_move = (
+            unit_vector_center_part_from_center_system * float_distance_for_dissociation
+        )
+        df_part.loc[:, l_col_coord] = (
+            df_part[l_col_coord].values + vector_move
+        )  # move the part by the unit vector times 'float_distance_for_dissociation'
+        l_df.append(df_part)
+    df_moved = pd.concat(l_df)  # combine moved parts
     return df_moved
 
 
 # # Specific Functions
 
 # In[ ]:
 
 
-def CRBN_Modify_Residue_Name( df ) :
-    '''   Modify PDB file containing CRBN so that its Zn coordinating site can be appropriatly simulated. If PDB records were already modified, modify them back to standard residue names.   '''
-    df = deepcopy( df )
-    df = df[ df.Atom_name != 'ZN' ] # remove previous Zn from the structure before processing
-    arr_mask_crbn = df.Chain_identifier.values == 'A'
+def CRBN_Modify_Residue_Name(df):
+    """Modify PDB file containing CRBN so that its Zn coordinating site can be appropriatly simulated. If PDB records were already modified, modify them back to standard residue names."""
+    df = deepcopy(df)
+    df = df[
+        df.Atom_name != "ZN"
+    ]  # remove previous Zn from the structure before processing
+    arr_mask_crbn = df.Chain_identifier.values == "A"
     arr_residue_num = df.Residue_sequence_number.values
-    if len( PD.Select( df, Residue_name = 'CYZ' ) ) == 0 : # if a given PDB dataframe's CRBN's residues were already modified.
-        df.loc[ arr_mask_crbn & ( ( arr_residue_num == 323 ) | ( arr_residue_num == 326 ) | ( arr_residue_num == 391 ) ), 'Residue_name' ] = 'CY1'
-        df.loc[ arr_mask_crbn & ( arr_residue_num == 394 ), 'Residue_name' ] = 'CYZ'
-        df.loc[ -1 ] = np.array( [ 'ATOM', 3280, 'ZN', '', 'CYZ', 'A', 394, '' ] + list( PD.Select( df, Residue_name = [ 'CY1', 'CYZ' ], Atom_name = 'SG' )[ [ 'X_orthogonal_Å_coordinate', 'Y_orthogonal_Å_coordinate', 'Z_orthogonal_Å_coordinate' ] ].mean( axis = 0 ) ), dtype = object ) # add discarded Zn ion in the PDB dataframe (average of xyz coordinats of SG of the four cysteines)
-    else :
-        df.loc[ arr_mask_crbn & ( ( arr_residue_num == 323 ) | ( arr_residue_num == 326 ) | ( arr_residue_num == 391 ) | ( arr_residue_num == 394 ) ), 'Residue_name' ] = 'CYS'
-    return df.sort_values( [ 'Chain_identifier', 'Residue_sequence_number', 'Atom_name' ] ).reset_index( drop = True )
-
+    if (
+        len(PD.Select(df, Residue_name="CYZ")) == 0
+    ):  # if a given PDB dataframe's CRBN's residues were already modified.
+        df.loc[
+            arr_mask_crbn
+            & (
+                (arr_residue_num == 323)
+                | (arr_residue_num == 326)
+                | (arr_residue_num == 391)
+            ),
+            "Residue_name",
+        ] = "CY1"
+        df.loc[arr_mask_crbn & (arr_residue_num == 394), "Residue_name"] = "CYZ"
+        df.loc[-1] = np.array(
+            ["ATOM", 3280, "ZN", "", "CYZ", "A", 394, ""]
+            + list(
+                PD.Select(df, Residue_name=["CY1", "CYZ"], Atom_name="SG")[
+                    [
+                        "X_orthogonal_Å_coordinate",
+                        "Y_orthogonal_Å_coordinate",
+                        "Z_orthogonal_Å_coordinate",
+                    ]
+                ].mean(axis=0)
+            ),
+            dtype=object,
+        )  # add discarded Zn ion in the PDB dataframe (average of xyz coordinats of SG of the four cysteines)
+    else:
+        df.loc[
+            arr_mask_crbn
+            & (
+                (arr_residue_num == 323)
+                | (arr_residue_num == 326)
+                | (arr_residue_num == 391)
+                | (arr_residue_num == 394)
+            ),
+            "Residue_name",
+        ] = "CYS"
+    return df.sort_values(
+        ["Chain_identifier", "Residue_sequence_number", "Atom_name"]
+    ).reset_index(drop=True)
```

### Comparing `biobookshelf-0.2.2/biobookshelf/PKG/package_util.py` & `biobookshelf-0.2.3/biobookshelf/PKG/package_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,72 @@
 from biobookshelf.main import *
 
-def Download_Data( path_file, path_remote, name_package ) :
+
+def Download_Data(path_file, path_remote, name_package):
     """
     Download large datafile of a PyPI package from a remote directory. If the file already exists, skip downloading and exit the funciton.
     download given file (relative directory within a package) from the remote directory (usually a Github directory, with sufficient number of data packs for Git-LFS pulls) to a current package
     """
-    path_file_download_flag = pkg_resources.resource_filename( name_package, f'{path_file}.download_completed.flag' )
-    if not os.path.exists( path_file_download_flag ) :
-        OS_Download( f'{path_remote}{path_file}', pkg_resources.resource_filename( name_package, path_file ) )
-        with open( path_file_download_flag, 'w' ) as file :
-            file.write( 'download completed at ' + TIME_GET_timestamp( ) )
-        print( f"data file {path_file} of the package {name_package} has been downloaded." )
-        
-def Gunzip_Data( path_file, name_package ) :
+    path_file_download_flag = pkg_resources.resource_filename(
+        name_package, f"{path_file}.download_completed.flag"
+    )
+    if not os.path.exists(path_file_download_flag):
+        OS_Download(
+            f"{path_remote}{path_file}",
+            pkg_resources.resource_filename(name_package, path_file),
+        )
+        with open(path_file_download_flag, "w") as file:
+            file.write("download completed at " + TIME_GET_timestamp())
+        print(
+            f"data file {path_file} of the package {name_package} has been downloaded."
+        )
+
+
+def Gunzip_Data(path_file, name_package):
     """
     Unzip large datafiles of a PyPI package often downloaded from a remote directory. If the gunzipped file already exists, skip unzipping and exit the funciton.
     """
-    if path_file.count( '.' ) == 0 or path_file.rsplit( '.', 1 )[ 1 ].lower( ) != 'gz' : # check whether given file is a gzipped file
-        print( f"[Gunzip_Data] given file {path_file} seems to be not a gzipped file, exiting" )
+    if (
+        path_file.count(".") == 0 or path_file.rsplit(".", 1)[1].lower() != "gz"
+    ):  # check whether given file is a gzipped file
+        print(
+            f"[Gunzip_Data] given file {path_file} seems to be not a gzipped file, exiting"
+        )
         return -1
-    path_file_download_flag = pkg_resources.resource_filename( name_package, f'{path_file}.gunzip_completed.flag' )
-    if not os.path.exists( path_file_download_flag ) : # if gunzip has not been done or not completed 
-        
-        path_file_zipped = pkg_resources.resource_filename( name_package, path_file ) # absolute directory of gzipped file
-        path_file_unzipped = path_file_zipped.rsplit( '.', 1 )[ 0 ] # retrieve directory of an unzipped file
-        if os.path.exists( path_file_unzipped ) : # if incomplete unzipped file exists, remove the file
-            os.remove( path_file_unzipped )
-        OS_Run( [ 'gunzip', path_file_zipped ] )
-        with open( path_file_download_flag, 'w' ) as file :
-            file.write( 'gunzip completed at ' + TIME_GET_timestamp( ) )
-        print( f"data file {path_file} of the package {name_package} has been gunzipped." )
-        
-def Detect_Entry_Point( name_entry_point ) :
-    '''  # 2021-06-04 11:05:34 
+    path_file_download_flag = pkg_resources.resource_filename(
+        name_package, f"{path_file}.gunzip_completed.flag"
+    )
+    if not os.path.exists(
+        path_file_download_flag
+    ):  # if gunzip has not been done or not completed
+
+        path_file_zipped = pkg_resources.resource_filename(
+            name_package, path_file
+        )  # absolute directory of gzipped file
+        path_file_unzipped = path_file_zipped.rsplit(".", 1)[
+            0
+        ]  # retrieve directory of an unzipped file
+        if os.path.exists(
+            path_file_unzipped
+        ):  # if incomplete unzipped file exists, remove the file
+            os.remove(path_file_unzipped)
+        OS_Run(["gunzip", path_file_zipped])
+        with open(path_file_download_flag, "w") as file:
+            file.write("gunzip completed at " + TIME_GET_timestamp())
+        print(
+            f"data file {path_file} of the package {name_package} has been gunzipped."
+        )
+
+
+def Detect_Entry_Point(name_entry_point):
+    """# 2021-06-04 11:05:34
     check whether an entry point with the given name of entry point has been used when running the current application
     return True if the given entry point was used and return False if not.
-    '''
+    """
     # retrieve the name of a current executable
-    str_name_program = sys.argv[ 0 ] 
-    if '/' in str_name_program :
-        str_name_program = str_name_program.rsplit( '/', 1 )[ 1 ]
-    flag_usage_from_command_line_interface = str_name_program[ : len( name_entry_point ) ] == name_entry_point
+    str_name_program = sys.argv[0]
+    if "/" in str_name_program:
+        str_name_program = str_name_program.rsplit("/", 1)[1]
+    flag_usage_from_command_line_interface = (
+        str_name_program[: len(name_entry_point)] == name_entry_point
+    )
     return flag_usage_from_command_line_interface
-
```

### Comparing `biobookshelf-0.2.2/biobookshelf/SAM/sam_util.py` & `biobookshelf-0.2.3/biobookshelf/SAM/sam_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,590 +1,834 @@
 from biobookshelf.main import *
 import biobookshelf.SEQ as SEQ
 
-def combine_bam( path_file_bam_output, * l_bam_file, int_max_num_files = 900, flag_remove_file = False, int_num_threads = 12 ) :
-    """ # 2022-07-21 14:49:08 CML & HSA 
+
+def combine_bam(
+    path_file_bam_output,
+    *l_bam_file,
+    int_max_num_files=900,
+    flag_remove_file=False,
+    int_num_threads=12,
+):
+    """# 2022-07-21 14:49:08 CML & HSA
     abstraction: hide the detail implementation to users.
 
     'path_file_bam_output' : path to output file. if the output file already exists, this throw an error
     'l_bam_file' : list of bam files that will be merged
     'int_max_num_files' : maximum number of files that can be opened in a process (typicaly 1024 in linux)
     'flag_remove_file' : if True, input files will be removed.
     'int_num_threads' : the number of threads to merge input bam files. one thread will be used to distribute works (so int_num_threads - 1 threads will be actually used for sorting)
     """
-    int_num_files = len( l_bam_file )
-    int_num_of_recursive_merging = int( np.ceil( math.log( int_num_files, int_max_num_files ) ) ) # retrieve the minmum number of recursive merging
+    int_num_files = len(l_bam_file)
+    int_num_of_recursive_merging = int(
+        np.ceil(math.log(int_num_files, int_max_num_files))
+    )  # retrieve the minmum number of recursive merging
+
+    path_folder_output = (
+        path_file_bam_output.rsplit("/", 1)[0] + "/"
+    )  # retrieve output folder where the output file will reside
+    path_folder_temp = f"{path_folder_output}temp_{UUID( )}/"
 
-    path_folder_output = path_file_bam_output.rsplit( '/', 1 )[ 0 ] + '/' # retrieve output folder where the output file will reside
-    path_folder_temp = f'{path_folder_output}temp_{UUID( )}/'
-    
     # create folders
-    for path_folder in [ path_folder_output, path_folder_temp ] :
-        os.makedirs( path_folder, exist_ok = True ) # create temp folder
+    for path_folder in [path_folder_output, path_folder_temp]:
+        os.makedirs(path_folder, exist_ok=True)  # create temp folder
 
     # merge files until all files are merged in to a single file
-    while len( l_bam_file ) > 1 : # while loop is active when there is files to be merged
-        int_num_files = len( l_bam_file )  # retreive number of bam files
-        l_file_size = list( os.stat( path_file ).st_size for path_file in l_bam_file ) # retrieve file size of input bam files
+    while len(l_bam_file) > 1:  # while loop is active when there is files to be merged
+        int_num_files = len(l_bam_file)  # retreive number of bam files
+        l_file_size = list(
+            os.stat(path_file).st_size for path_file in l_bam_file
+        )  # retrieve file size of input bam files
 
-        str_uuid_current_merge_step = UUID( ) # identifier for the current merge step
+        str_uuid_current_merge_step = UUID()  # identifier for the current merge step
 
         # retrieve number of output bam files
-        if int_num_files < int_max_num_files :
+        if int_num_files < int_max_num_files:
             int_num_output_bam_file = 1
-        else :
-            int_num_output_bam_file = int( np.ceil( int_num_files / int_max_num_files ) ) 
+        else:
+            int_num_output_bam_file = int(np.ceil(int_num_files / int_max_num_files))
 
-        def batch_generator(  ) :
-            l_batch = LIST_Split( l_bam_file, n_split = int_num_output_bam_file, flag_contiguous_chunk = True, arr_weight_for_load_balancing = l_file_size )
-            for batch in l_batch :
+        def batch_generator():
+            l_batch = LIST_Split(
+                l_bam_file,
+                n_split=int_num_output_bam_file,
+                flag_contiguous_chunk=True,
+                arr_weight_for_load_balancing=l_file_size,
+            )
+            for batch in l_batch:
                 yield batch
-        def process_batch( batch, pipe_sender = None ) :
-            l_file_bam_to_be_merged_into_a_single_bam_file = batch 
-            path_file_bam_combined_for_a_batch = f"{path_folder_temp}{str_uuid_current_merge_step}.{UUID( )}.bam"
-            print( len( l_file_bam_to_be_merged_into_a_single_bam_file ), 'files will be merged into', path_file_bam_combined_for_a_batch )
-            pysam.merge( '--no-PG', path_file_bam_combined_for_a_batch, * l_file_bam_to_be_merged_into_a_single_bam_file )
-            pysam.index( path_file_bam_combined_for_a_batch )
-            pipe_sender.send( 'completed' ) # tell the distributor that the work is done! 
 
-        Multiprocessing_Batch( batch_generator(  ), process_batch, int_num_threads = max( 2, int_num_threads ) )
+        def process_batch(batch, pipe_sender=None):
+            l_file_bam_to_be_merged_into_a_single_bam_file = batch
+            path_file_bam_combined_for_a_batch = (
+                f"{path_folder_temp}{str_uuid_current_merge_step}.{UUID( )}.bam"
+            )
+            print(
+                len(l_file_bam_to_be_merged_into_a_single_bam_file),
+                "files will be merged into",
+                path_file_bam_combined_for_a_batch,
+            )
+            pysam.merge(
+                "--no-PG",
+                path_file_bam_combined_for_a_batch,
+                *l_file_bam_to_be_merged_into_a_single_bam_file,
+            )
+            pysam.index(path_file_bam_combined_for_a_batch)
+            pipe_sender.send("completed")  # tell the distributor that the work is done!
+
+        Multiprocessing_Batch(
+            batch_generator(), process_batch, int_num_threads=max(2, int_num_threads)
+        )
 
         # remove temporary or input files
-        if flag_remove_file :
-            for path_file in l_bam_file :
-                os.remove( path_file )
-                os.remove( path_file + '.bai' ) # delete index files, too
+        if flag_remove_file:
+            for path_file in l_bam_file:
+                os.remove(path_file)
+                os.remove(path_file + ".bai")  # delete index files, too
                 pass
-        flag_remove_file = True # remove temporary files
+        flag_remove_file = True  # remove temporary files
 
-        l_bam_file = glob.glob( f"{path_folder_temp}{str_uuid_current_merge_step}.*.bam" ) # retrieve input bam files for the next round
+        l_bam_file = glob.glob(
+            f"{path_folder_temp}{str_uuid_current_merge_step}.*.bam"
+        )  # retrieve input bam files for the next round
 
     # rename combined output file
-    os.rename( l_bam_file[ 0 ], path_file_bam_output )
-    os.rename( l_bam_file[ 0 ] + '.bai', path_file_bam_output + '.bai' )
+    os.rename(l_bam_file[0], path_file_bam_output)
+    os.rename(l_bam_file[0] + ".bai", path_file_bam_output + ".bai")
 
     # delete temporary folder
-    shutil.rmtree( path_folder_temp )
+    shutil.rmtree(path_folder_temp)
+
 
-def Cigartuple_Convert( r_mappy = None, seq_mappy = None, cigartuple_pysam = None ) :
-    """ # 2021-11-25 13:36:51 
+def Cigartuple_Convert(r_mappy=None, seq_mappy=None, cigartuple_pysam=None):
+    """# 2021-11-25 13:36:51
     convert cigartuple from mappy to that of pysam and vice versa
     The output format will be fixed to list of tuples (pysam format)
     for mappy cigartuple -> pysam cigartuple, since the mappy does not include soft-clipping or hard clipping operations in its cigartuples, the hit record along with mappy sequence is required to return a complete cigartuples object (the clipped regions will be considered as soft-clipped regions)
     """
     # define interger representation of the CIGAR operations used in BAM files
     int_cigarop_S = 4
     int_cigarop_H = 5
-    
-    l_cigartuple = [ ]
-    if r_mappy is not None and seq_mappy is not None :
-        ''' mappy cigartuple -> pysam cigartuple '''
+
+    l_cigartuple = []
+    if r_mappy is not None and seq_mappy is not None:
+        """mappy cigartuple -> pysam cigartuple"""
         r = r_mappy
-        len_seq = len( seq_mappy )
-        
-        ''' handle soft clipping at the front (front in the '+' strand) '''
-        if r.strand > 0 and r.q_st > 0 : # if sequence was aligned to '+' strand 
-            l_cigartuple.append( ( int_cigarop_S, r.q_st ) )
-        elif r.strand < 0 and r.q_en < len_seq :
-            l_cigartuple.append( ( int_cigarop_S, len_seq - r.q_en ) )
-            
-        for int_n_base_pairs, int_cigarop in r.cigar :
-            l_cigartuple.append( ( int_cigarop, int_n_base_pairs ) )
-            
-        ''' handle soft clipping at the end (end in the '+' strand) '''
-        if r.strand > 0 and r.q_en < len_seq : # if sequence was aligned to '+' strand 
-            l_cigartuple.append( ( int_cigarop_S, len_seq - r.q_en ) )
-        elif r.strand < 0 and r.q_st > 0 :
-            l_cigartuple.append( ( int_cigarop_S, r.q_st ) )
-            
-    elif cigartuple_pysam is not None :
-        ''' pysam cigartuple -> mappy cigartuple '''
-        for int_cigarop, int_n_base_pairs in cigartuple_pysam :
-            l_cigartuple.append( ( int_n_base_pairs, int_cigarop ) )
+        len_seq = len(seq_mappy)
+
+        """ handle soft clipping at the front (front in the '+' strand) """
+        if r.strand > 0 and r.q_st > 0:  # if sequence was aligned to '+' strand
+            l_cigartuple.append((int_cigarop_S, r.q_st))
+        elif r.strand < 0 and r.q_en < len_seq:
+            l_cigartuple.append((int_cigarop_S, len_seq - r.q_en))
+
+        for int_n_base_pairs, int_cigarop in r.cigar:
+            l_cigartuple.append((int_cigarop, int_n_base_pairs))
+
+        """ handle soft clipping at the end (end in the '+' strand) """
+        if r.strand > 0 and r.q_en < len_seq:  # if sequence was aligned to '+' strand
+            l_cigartuple.append((int_cigarop_S, len_seq - r.q_en))
+        elif r.strand < 0 and r.q_st > 0:
+            l_cigartuple.append((int_cigarop_S, r.q_st))
+
+    elif cigartuple_pysam is not None:
+        """pysam cigartuple -> mappy cigartuple"""
+        for int_cigarop, int_n_base_pairs in cigartuple_pysam:
+            l_cigartuple.append((int_n_base_pairs, int_cigarop))
     return l_cigartuple
 
-def Generate_Base_and_Qual( r ) :
-    """ # 2021-08-27 22:09:31 
-    a generator function yielding the base and quality of every matched/mismatched positions of a given pysam read record 
-    """
-    pos_read, pos_ref = 0, 0 # current position in the extracted reference sequence and the current read
-    int_oper_M, int_oper_I, int_oper_D, int_oper_N, int_oper_S, int_oper_H, int_oper_P, int_oper_equal, int_oper_X = list( range( 9 ) )
-    for int_oper, n_bases in r.cigartuples :
-        if int_oper == int_oper_M : 
-            for _ in range( n_bases ) :
-                str_base_read, str_qual_read = r.seq[ pos_read ], r.query_qualities[ pos_read ]
+
+def Generate_Base_and_Qual(r):
+    """# 2021-08-27 22:09:31
+    a generator function yielding the base and quality of every matched/mismatched positions of a given pysam read record
+    """
+    pos_read, pos_ref = (
+        0,
+        0,
+    )  # current position in the extracted reference sequence and the current read
+    (
+        int_oper_M,
+        int_oper_I,
+        int_oper_D,
+        int_oper_N,
+        int_oper_S,
+        int_oper_H,
+        int_oper_P,
+        int_oper_equal,
+        int_oper_X,
+    ) = list(range(9))
+    for int_oper, n_bases in r.cigartuples:
+        if int_oper == int_oper_M:
+            for _ in range(n_bases):
+                str_base_read, str_qual_read = (
+                    r.seq[pos_read],
+                    r.query_qualities[pos_read],
+                )
                 yield r.reference_start + pos_ref, str_base_read, str_qual_read
                 pos_ref += 1
                 pos_read += 1
-        elif int_oper == int_oper_N :
+        elif int_oper == int_oper_N:
             pos_ref += n_bases
-        elif int_oper == int_oper_S :
+        elif int_oper == int_oper_S:
             pos_read += n_bases
-        elif int_oper == int_oper_I :
+        elif int_oper == int_oper_I:
             pos_read += n_bases
-        elif int_oper == int_oper_D :
+        elif int_oper == int_oper_D:
             pos_ref += n_bases
-        elif int_oper == int_oper_H :
+        elif int_oper == int_oper_H:
             pass
-        elif int_oper == int_oper_P :
+        elif int_oper == int_oper_P:
             pass
-        elif int_oper == int_oper_equal :
-            str_base_read, str_qual_read = r.seq[ pos_read ], r.query_qualities[ pos_read ]
+        elif int_oper == int_oper_equal:
+            str_base_read, str_qual_read = r.seq[pos_read], r.query_qualities[pos_read]
             yield r.reference_start + pos_ref, str_base_read, str_qual_read
             pos_ref += n_bases
             pos_read += n_bases
-        elif int_oper == int_oper_X :
-            for _ in range( n_bases ) :
-                str_base_read, str_qual_read = r.seq[ pos_read ], r.query_qualities[ pos_read ]
+        elif int_oper == int_oper_X:
+            for _ in range(n_bases):
+                str_base_read, str_qual_read = (
+                    r.seq[pos_read],
+                    r.query_qualities[pos_read],
+                )
                 yield r.reference_start + pos_ref, str_base_read, str_qual_read
                 pos_ref += 1
-                pos_read += 1           
-                
-def Retrive_List_of_Mapped_Segments( cigartuples, pos_start, return_1_based_coordinate = False, flag_pos_start_0_based_coord = True, flag_return_splice_junction = False, flag_is_cigartuples_from_mappy = False ) :
-    ''' # 2022-01-28 01:51:16 
+                pos_read += 1
+
+
+def Retrive_List_of_Mapped_Segments(
+    cigartuples,
+    pos_start,
+    return_1_based_coordinate=False,
+    flag_pos_start_0_based_coord=True,
+    flag_return_splice_junction=False,
+    flag_is_cigartuples_from_mappy=False,
+):
+    """# 2022-01-28 01:51:16
     return l_seq and int_total_aligned_length for given cigartuples (returned by pysam cigartuples) and 'pos_start' (0-based coordinates, assuming pos_start is 0-based coordinate)
     'return_1_based_coordinate' : return 1-based coordinate, assuming 'pos_start' is 0-based coordinate (pysam returns 0-based coordinate)
     'flag_return_splice_junction' : additionally return list of splice junction tuples
     'flag_is_cigartuples_from_mappy' : if cigartuples are from mappy.Alignment, set this flag to True
-    '''
-    l_seg, start, int_aligned_length, int_total_aligned_length = list( ), pos_start, 0, 0
-    if return_1_based_coordinate and flag_pos_start_0_based_coord : # 0-based > 1-based
+    """
+    l_seg, start, int_aligned_length, int_total_aligned_length = list(), pos_start, 0, 0
+    if return_1_based_coordinate and flag_pos_start_0_based_coord:  # 0-based > 1-based
         start -= 1
-    for operation, length in cigartuples :
-        if flag_is_cigartuples_from_mappy : # if flag_is_cigartuples_from_mappy, swap the two values
+    for operation, length in cigartuples:
+        if (
+            flag_is_cigartuples_from_mappy
+        ):  # if flag_is_cigartuples_from_mappy, swap the two values
             temp = operation
             operation = length
             length = temp
-        if operation in { 0, 2, 7, 8 } : # 'MD=X'
+        if operation in {0, 2, 7, 8}:  # 'MD=X'
             int_aligned_length += length
-        elif operation == 3 : # 'N' if splice junction appears, split the region and make a record
-            l_seg.append( ( start, ( start + int_aligned_length - 1 ) if return_1_based_coordinate else ( start + int_aligned_length ) ) ) # set the end position
-            start = start + int_aligned_length + length # set the next start position
-            int_total_aligned_length += int_aligned_length # update total aligned length
+        elif (
+            operation == 3
+        ):  # 'N' if splice junction appears, split the region and make a record
+            l_seg.append(
+                (
+                    start,
+                    (start + int_aligned_length - 1)
+                    if return_1_based_coordinate
+                    else (start + int_aligned_length),
+                )
+            )  # set the end position
+            start = start + int_aligned_length + length  # set the next start position
+            int_total_aligned_length += (
+                int_aligned_length  # update total aligned length
+            )
             int_aligned_length = 0
-    if int_aligned_length > 0 : 
-        l_seg.append( ( start, ( start + int_aligned_length - 1 ) if return_1_based_coordinate else ( start + int_aligned_length ) ) )
+    if int_aligned_length > 0:
+        l_seg.append(
+            (
+                start,
+                (start + int_aligned_length - 1)
+                if return_1_based_coordinate
+                else (start + int_aligned_length),
+            )
+        )
         int_total_aligned_length += int_aligned_length
-    if flag_return_splice_junction :
+    if flag_return_splice_junction:
         # collect splice junction tuples from l_seg
-        l_sj = [ ]
-        for i in range( len( l_seg ) - 1 ) :
-            l_sj.append( ( l_seg[ i ][ 1 ], l_seg[ i + 1 ][ 0 ] ) )
+        l_sj = []
+        for i in range(len(l_seg) - 1):
+            l_sj.append((l_seg[i][1], l_seg[i + 1][0]))
         return l_seg, int_total_aligned_length, l_sj
-    else :
+    else:
         return l_seg, int_total_aligned_length
-    
-def Alignment_Record_from_Mappy_to_String( hit, r_fastq ) :
-    """ # 2021-10-27 15:19:48  
+
+
+def Alignment_Record_from_Mappy_to_String(hit, r_fastq):
+    """# 2021-10-27 15:19:48
     For single-end read only
-    
+
     'hit': mappy.Alignment object returned by mappy.Aligner.map function
     'r_fastq' : list of qname, seq, _, qual containing a single fastq record whose sequence has been queried using mappy
     """
     # set cigar operation values
     int_cigarop_S = 4
     int_cigarop_H = 5
-    
+
     # parse fastq record
-    header, seq, _, qual = r_fastq 
-    qname = header[ 1 : ].split( ' ', 1 )[ 0 ] # retrieve qname
-    
-    flag_is_reverse_complemented = hit.strand != 1 
-    int_flag = ( not hit.is_primary ) * 256 + ( flag_is_reverse_complemented ) * 16 # compose flag integer
-    
+    header, seq, _, qual = r_fastq
+    qname = header[1:].split(" ", 1)[0]  # retrieve qname
+
+    flag_is_reverse_complemented = hit.strand != 1
+    int_flag = (not hit.is_primary) * 256 + (
+        flag_is_reverse_complemented
+    ) * 16  # compose flag integer
+
     # retrieve seq and qual in the right orientation
-    seq_in_sam_record = SEQ.Reverse_Complement( seq ) if flag_is_reverse_complemented else seq
-    qual_in_sam_record = qual[ : : -1 ] if flag_is_reverse_complemented else qual
-    
+    seq_in_sam_record = (
+        SEQ.Reverse_Complement(seq) if flag_is_reverse_complemented else seq
+    )
+    qual_in_sam_record = qual[::-1] if flag_is_reverse_complemented else qual
+
     # remove hard clipped portion of read (front)
-    int_len_op, int_type_op = hit.cigar[ 0 ]
-    if int_type_op == int_cigarop_H :
-        seq_in_sam_record = seq_in_sam_record[ int_len_op : ]
-        qual_in_sam_record = qual_in_sam_record[ int_len_op : ]
+    int_len_op, int_type_op = hit.cigar[0]
+    if int_type_op == int_cigarop_H:
+        seq_in_sam_record = seq_in_sam_record[int_len_op:]
+        qual_in_sam_record = qual_in_sam_record[int_len_op:]
     # remove hard clipped portion of read (rear)
-    int_len_op, int_type_op = hit.cigar[ -1 ]
-    if int_type_op == int_cigarop_H :
-        seq_in_sam_record = seq_in_sam_record[ : - int_len_op ]
-        qual_in_sam_record = qual_in_sam_record[ : - int_len_op ]
-        
-    str_sam_record = '\t'.join( [ qname, str( int_flag ), hit.ctg, str( hit.r_st + 1 ), str( hit.mapq ), hit.cigar_str, '*', '0', '0', seq_in_sam_record, qual_in_sam_record ] ) # 0>1-based coordinates
+    int_len_op, int_type_op = hit.cigar[-1]
+    if int_type_op == int_cigarop_H:
+        seq_in_sam_record = seq_in_sam_record[:-int_len_op]
+        qual_in_sam_record = qual_in_sam_record[:-int_len_op]
+
+    str_sam_record = "\t".join(
+        [
+            qname,
+            str(int_flag),
+            hit.ctg,
+            str(hit.r_st + 1),
+            str(hit.mapq),
+            hit.cigar_str,
+            "*",
+            "0",
+            "0",
+            seq_in_sam_record,
+            qual_in_sam_record,
+        ]
+    )  # 0>1-based coordinates
     return str_sam_record
 
+
 """
 Build a list of bookmarks for multithreading (simultaneous access of BAM files) 
 """
-def Bookmark( path_file_bam, n_threads, int_min_mapq_unique_mapped, int_n_bases_padding_around_interval = 10, verbose = False, l_dict_it = [ ], flag_ignore_record_with_flag_secondary_alignment = True, flag_ignore_record_with_flag_optical_or_pcr_duplicate = True, flag_genome_without_chr_prefix_was_used_for_l_dict_it = True ) :
-    """  # 2021-11-10 23:35:29 
+
+
+def Bookmark(
+    path_file_bam,
+    n_threads,
+    int_min_mapq_unique_mapped,
+    int_n_bases_padding_around_interval=10,
+    verbose=False,
+    l_dict_it=[],
+    flag_ignore_record_with_flag_secondary_alignment=True,
+    flag_ignore_record_with_flag_optical_or_pcr_duplicate=True,
+    flag_genome_without_chr_prefix_was_used_for_l_dict_it=True,
+):
+    """# 2021-11-10 23:35:29
     iterate the given BAM file twice to create a bookmark to mark the start and end of each chunk for simultaneous access of the BAM file
     WARNING: there might be a little overlap of reads analyzed by each process since the chunk boundary is marked with ( qname, flag, refname, refstart ). If the two SAM records with the same ( qname, flag, refname, refstart ), the reads between the two 'identical' SAM records might be analyzed twice by two processes analyzing the two chunk sharing the boundary (however, it is unlikely that this will happens in a typical BAM file).
 
     'path_file_bam' : indexed (with .bai file) BAM file to be create bookmarks for access by multiple processes
-    'n_threads' : number of threads (or number of bookmarks to create) to access a single BAM file 
-    'l_dict_it' : a list of dictionaries of interval trees (pip intervaltree package) containing intervals (genes and repeat annotations, etc.). When boundaries between chunk overlaps with the given intervals, it will be adjusted so that the boundary is at least 'int_n_bases_padding_around_interval' base pair away from the interval. 
+    'n_threads' : number of threads (or number of bookmarks to create) to access a single BAM file
+    'l_dict_it' : a list of dictionaries of interval trees (pip intervaltree package) containing intervals (genes and repeat annotations, etc.). When boundaries between chunk overlaps with the given intervals, it will be adjusted so that the boundary is at least 'int_n_bases_padding_around_interval' base pair away from the interval.
         This functionality will allow analyzing all reads aligned to a single interval in the 'dict_it' to be analyzed in a single thread, thus abolishing the need to combine results from all threads to produce interval-level output, thus simplifying  downstream analysis. if chromosome name contains 'chr' prefix, please set 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' to False
     'flag_genome_without_chr_prefix_was_used_for_l_dict_it' : (default = True) Please set this flag to False if the chromosome names of the given 'l_dict_it' annotations have a 'chr' prefix.
 
     returns
     df_bookmark, l_int_n_sam_records_per_chunk
     """
-    if isinstance( l_dict_it, dict ) : # if a single dict_it is given, wrap the dict_it inside a list
-        l_dict_it = [ l_dict_it ]
-
-    ''' retrieve sequence length of reference sequence from the BAM header '''
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        dict_header = samfile.header.to_dict( )
-    dict_seqname_to_len_seq = pd.DataFrame( dict_header[ 'SQ' ] ).set_index( 'SN' ).LN.to_dict( )
+    if isinstance(
+        l_dict_it, dict
+    ):  # if a single dict_it is given, wrap the dict_it inside a list
+        l_dict_it = [l_dict_it]
+
+    """ retrieve sequence length of reference sequence from the BAM header """
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        dict_header = samfile.header.to_dict()
+    dict_seqname_to_len_seq = (
+        pd.DataFrame(dict_header["SQ"]).set_index("SN").LN.to_dict()
+    )
 
     """ define internal functions """
-    def __chromosome_name_remove_chr__( str_name_chrom ) :
-        ''' remove 'chr' prefix from the chromosome name '''
-        if 'chr' == str_name_chrom[ : 3 ] :
-            return str_name_chrom[ 3 : ]
-        else :
+
+    def __chromosome_name_remove_chr__(str_name_chrom):
+        """remove 'chr' prefix from the chromosome name"""
+        if "chr" == str_name_chrom[:3]:
+            return str_name_chrom[3:]
+        else:
             return str_name_chrom
 
     """ Compose list of bookmarks for iterating input BAM file using multiple threads """
-    l_col = [ 'id_refname_start', 'int_refstart_start', 'int_index_chunk_start', 'id_refname_end', 'int_refstart_end', 'int_index_chunk_end' ]
+    l_col = [
+        "id_refname_start",
+        "int_refstart_start",
+        "int_index_chunk_start",
+        "id_refname_end",
+        "int_refstart_end",
+        "int_index_chunk_end",
+    ]
     # when number of threads > 1, retrieve bookmarks for multiprocessing
-    if n_threads > 1 : 
-        ''' retrieve the total number of SAM records '''
+    if n_threads > 1:
+        """retrieve the total number of SAM records"""
         # iterate the entire BAM file to retrieve the total number of SAM records
         int_n_total_sam_records = 0
-        with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-            for r in samfile.fetch( ) :
-                ''' filter alignments based on mapq and flag '''
-                if r.mapq < int_min_mapq_unique_mapped : # skip read whose mapq is below 'int_min_mapq_unique_mapped'
+        with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+            for r in samfile.fetch():
+                """filter alignments based on mapq and flag"""
+                if (
+                    r.mapq < int_min_mapq_unique_mapped
+                ):  # skip read whose mapq is below 'int_min_mapq_unique_mapped'
                     continue
                 # ignore records with flag indicating secondary alignment
-                if flag_ignore_record_with_flag_secondary_alignment and ( r.flag & ( 1 << 8 ) ) :
+                if flag_ignore_record_with_flag_secondary_alignment and (
+                    r.flag & (1 << 8)
+                ):
                     continue
                 # ignore records with flag indicating the alignment is optical pcr duplicates
-                if flag_ignore_record_with_flag_optical_or_pcr_duplicate and ( r.flag & ( 1 << 10 ) ) :
+                if flag_ignore_record_with_flag_optical_or_pcr_duplicate and (
+                    r.flag & (1 << 10)
+                ):
                     continue
-                ''' count the number of valid alignment records '''
+                """ count the number of valid alignment records """
                 int_n_total_sam_records += 1
 
         """ retrieve the positions and the id_reads at the start and stop points ('bookmark') for multiprocessing """
-        ''' retrieve bookmarks to mark the start and ends of contigs for each chunnk '''
+        """ retrieve bookmarks to mark the start and ends of contigs for each chunnk """
         # calculate the number of reads for each chunk
-        l_int_n_sam_records_per_chunk = INT.Split( int_n_total_sam_records, n_threads )
+        l_int_n_sam_records_per_chunk = INT.Split(int_n_total_sam_records, n_threads)
 
-        l_bookmark = [ ] # empty bookmark
+        l_bookmark = []  # empty bookmark
         flag_has_bookmark_been_initialized = False
-        int_start_possible_boundary = None # start position of the possible boundary # will be set to non-None value when the desired number of records in the current chunk has been reached its target and the boundary is being set or being adjusted
+        int_start_possible_boundary = None  # start position of the possible boundary # will be set to non-None value when the desired number of records in the current chunk has been reached its target and the boundary is being set or being adjusted
         int_n_sam_record_count = 0
         int_index_chunk = 0
-        id_refname_current = None # default reference name
+        id_refname_current = None  # default reference name
 
-        l_int_actual_n_sam_records_per_chunk = [ ] # actual number of sam records per chunk for the created bookmarks
+        l_int_actual_n_sam_records_per_chunk = (
+            []
+        )  # actual number of sam records per chunk for the created bookmarks
         # iterate the entire BAM file to retrieve the total number of SAM records
-        with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-            for r in samfile.fetch( ) :
-                ''' filter alignments based on mapq and flag '''
-                if r.mapq < int_min_mapq_unique_mapped : # skip read whose mapq is below 'int_min_mapq_unique_mapped'
+        with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+            for r in samfile.fetch():
+                """filter alignments based on mapq and flag"""
+                if (
+                    r.mapq < int_min_mapq_unique_mapped
+                ):  # skip read whose mapq is below 'int_min_mapq_unique_mapped'
                     continue
                 # ignore records with flag indicating secondary alignment
-                if flag_ignore_record_with_flag_secondary_alignment and ( r.flag & ( 1 << 8 ) ) :
+                if flag_ignore_record_with_flag_secondary_alignment and (
+                    r.flag & (1 << 8)
+                ):
                     continue
                 # ignore records with flag indicating the alignment is optical pcr duplicates
-                if flag_ignore_record_with_flag_optical_or_pcr_duplicate and ( r.flag & ( 1 << 10 ) ) :
+                if flag_ignore_record_with_flag_optical_or_pcr_duplicate and (
+                    r.flag & (1 << 10)
+                ):
                     continue
 
                 # retrieve SAM record info.
-                refname = r.reference_name 
+                refname = r.reference_name
                 refstart = r.reference_start
                 refend = r.reference_end
                 qname = r.qname
                 flag = r.flag
 
                 # initialize the bookmarks
-                if not flag_has_bookmark_been_initialized :
-                    l_bookmark.append( [ refname, refstart, 0 ] ) # initialize bookmark by assigning the first sam record to the index_chunk 0
+                if not flag_has_bookmark_been_initialized:
+                    l_bookmark.append(
+                        [refname, refstart, 0]
+                    )  # initialize bookmark by assigning the first sam record to the index_chunk 0
                     id_refname_current = refname
                     flag_has_bookmark_been_initialized = True
                     continue
 
                 int_n_sam_record_count += 1
 
                 """ mark the change of contig by adding bookmarks """
-                ''' if the next chromosome has been reached while for searching for next gene boundary, the boundary is considered passed, and the new chunk will be initiated.'''
-                if id_refname_current != refname :
-                    if verbose :
-                        print( f'chromosome changed from {id_refname_current} to {refname} at chunk_{int_index_chunk}:{int_n_sam_record_count}' )
+                """ if the next chromosome has been reached while for searching for next gene boundary, the boundary is considered passed, and the new chunk will be initiated."""
+                if id_refname_current != refname:
+                    if verbose:
+                        print(
+                            f"chromosome changed from {id_refname_current} to {refname} at chunk_{int_index_chunk}:{int_n_sam_record_count}"
+                        )
                     id_refname_current = refname
-                    ''' handle the case when contig changes while the chunk boundary is being searched '''
-                    if int_start_possible_boundary is not None : 
+                    """ handle the case when contig changes while the chunk boundary is being searched """
+                    if int_start_possible_boundary is not None:
                         # retrieve stats about the current chunk and initializes the next chunk
                         int_start_possible_boundary = None
-                        l_int_actual_n_sam_records_per_chunk.append( int_n_sam_record_count - 1 )
-                        if verbose :
-                            print( f'new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)' )
+                        l_int_actual_n_sam_records_per_chunk.append(
+                            int_n_sam_record_count - 1
+                        )
+                        if verbose:
+                            print(
+                                f"new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)"
+                            )
                         int_index_chunk += 1
                         int_n_sam_record_count = 1
-                    bookmark = [ refname, 0, int_index_chunk ]
-                    l_bookmark.append( bookmark ) # add bookmarks twice
-                    l_bookmark.append( bookmark )
+                    bookmark = [refname, 0, int_index_chunk]
+                    l_bookmark.append(bookmark)  # add bookmarks twice
+                    l_bookmark.append(bookmark)
 
                 """
                 Search boundaries 
                 """
                 # initialize the next chunk if the 'int_n_sam_record_count' reached the assigned number of sam records for the current chunk (process)
-                if int_n_sam_record_count > l_int_n_sam_records_per_chunk[ int_index_chunk ] :
-                    ''' set default boundary (current position + 1) '''
-                    if int_start_possible_boundary is None :
+                if (
+                    int_n_sam_record_count
+                    > l_int_n_sam_records_per_chunk[int_index_chunk]
+                ):
+                    """set default boundary (current position + 1)"""
+                    if int_start_possible_boundary is None:
                         int_start_possible_boundary = refstart + 1
-                    ''' iterate until reaching the possible chunk boundary '''
-                    if int_start_possible_boundary is not None :
-                        if refstart < int_start_possible_boundary : # if the next possible boundary has not been reached 
+                    """ iterate until reaching the possible chunk boundary """
+                    if int_start_possible_boundary is not None:
+                        if (
+                            refstart < int_start_possible_boundary
+                        ):  # if the next possible boundary has not been reached
                             continue
 
                     """
                     Possible boundary has been reached
                     """
-                    ''' check whether the current position overlaps with intervals in the given list of dictionaries of interval trees, and set the next possible boundary based on the overlapped intervals '''
-                    l_adjusted_boundary_based_on_overlapped_interval = [ ]
+                    """ check whether the current position overlaps with intervals in the given list of dictionaries of interval trees, and set the next possible boundary based on the overlapped intervals """
+                    l_adjusted_boundary_based_on_overlapped_interval = []
                     # search overlapped intervals
-                    int_len_seq_current_contig = dict_seqname_to_len_seq[ refname ] # retrieve the length of the current contig
-                    refname_for_l_dict_it = __chromosome_name_remove_chr__( refname ) if flag_genome_without_chr_prefix_was_used_for_l_dict_it else refname # handle if BAM file's genome chromosome name convention and 'l_dict_it' annotations' chromosome name convention is different # retrieve refname without 'chr' prefix if 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' is True
-
-                    for dict_it in l_dict_it :
-                        if refname_for_l_dict_it in dict_it :
-                            for start, end, anno_name in dict_it[ refname_for_l_dict_it ][ refstart ] :
-                                l_adjusted_boundary_based_on_overlapped_interval.append( min( end + int_n_bases_padding_around_interval, int_len_seq_current_contig - 1 ) ) # maximum boundary is the end position of the contig
-                                if verbose :
-                                    print( f"for chunk {int_index_chunk}, the possible boundary currently overlaps with {refname_for_l_dict_it}:{start}-{end}|{anno_name}" )
+                    int_len_seq_current_contig = dict_seqname_to_len_seq[
+                        refname
+                    ]  # retrieve the length of the current contig
+                    refname_for_l_dict_it = (
+                        __chromosome_name_remove_chr__(refname)
+                        if flag_genome_without_chr_prefix_was_used_for_l_dict_it
+                        else refname
+                    )  # handle if BAM file's genome chromosome name convention and 'l_dict_it' annotations' chromosome name convention is different # retrieve refname without 'chr' prefix if 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' is True
+
+                    for dict_it in l_dict_it:
+                        if refname_for_l_dict_it in dict_it:
+                            for start, end, anno_name in dict_it[refname_for_l_dict_it][
+                                refstart
+                            ]:
+                                l_adjusted_boundary_based_on_overlapped_interval.append(
+                                    min(
+                                        end + int_n_bases_padding_around_interval,
+                                        int_len_seq_current_contig - 1,
+                                    )
+                                )  # maximum boundary is the end position of the contig
+                                if verbose:
+                                    print(
+                                        f"for chunk {int_index_chunk}, the possible boundary currently overlaps with {refname_for_l_dict_it}:{start}-{end}|{anno_name}"
+                                    )
                     # if there is any overlaps with the intervals, start adjusting boundaries
-                    if len( l_adjusted_boundary_based_on_overlapped_interval ) != 0 :
-                        int_start_possible_boundary_previous = int_start_possible_boundary
+                    if len(l_adjusted_boundary_based_on_overlapped_interval) != 0:
+                        int_start_possible_boundary_previous = (
+                            int_start_possible_boundary
+                        )
                         # set the next possible boundary
-                        int_start_possible_boundary = max( l_adjusted_boundary_based_on_overlapped_interval ) # use the farthest interval ends when setting the next potential boundary 
-                        if verbose :
-                            print( f'for chunk {int_index_chunk}, the possible boundary will change from {refname_for_l_dict_it}:{int_start_possible_boundary_previous} to {refname_for_l_dict_it}:{int_start_possible_boundary} ({int_start_possible_boundary - refstart}bp shift) when int_n_sam_record_count = {int_n_sam_record_count}' )
+                        int_start_possible_boundary = max(
+                            l_adjusted_boundary_based_on_overlapped_interval
+                        )  # use the farthest interval ends when setting the next potential boundary
+                        if verbose:
+                            print(
+                                f"for chunk {int_index_chunk}, the possible boundary will change from {refname_for_l_dict_it}:{int_start_possible_boundary_previous} to {refname_for_l_dict_it}:{int_start_possible_boundary} ({int_start_possible_boundary - refstart}bp shift) when int_n_sam_record_count = {int_n_sam_record_count}"
+                            )
                         continue
 
                     """
                     Finalize boundary
                     """
-                    ''' if the current position does not overlap with any intervals, set the current position as the boundary between chunks '''
-                    int_start_possible_boundary = None # set 'int_start_possible_boundary' to indicate boundary is not being searched
-                    l_int_actual_n_sam_records_per_chunk.append( int_n_sam_record_count - 1 )
-                    if verbose :
-                        print( f'new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)' )
+                    """ if the current position does not overlap with any intervals, set the current position as the boundary between chunks """
+                    int_start_possible_boundary = None  # set 'int_start_possible_boundary' to indicate boundary is not being searched
+                    l_int_actual_n_sam_records_per_chunk.append(
+                        int_n_sam_record_count - 1
+                    )
+                    if verbose:
+                        print(
+                            f"new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)"
+                        )
                     # initialized the next chunk
                     int_n_sam_record_count = 1
                     int_index_chunk += 1
                     # add a bookmark of the current position to mark the start of the new chunk
-                    bookmark = [ refname, refstart, int_index_chunk ]
-                    l_bookmark.append( bookmark )
-                    l_bookmark.append( bookmark )
-
-        l_int_actual_n_sam_records_per_chunk.append( int_n_sam_record_count )
-        l_bookmark.append( [ '', -1, int_index_chunk ] )
-        l_bookmark = np.array( l_bookmark, dtype = object ).reshape( int( len( l_bookmark ) / 2 ), 6 ) # reshape bookmark so that each record contains bookmark of the start point and end points
-        df_bookmark = pd.DataFrame( l_bookmark, columns = l_col )
-    else :
-        df_bookmark = pd.DataFrame( [ [ 'single_thread' ] * 6 ], columns = l_col )
+                    bookmark = [refname, refstart, int_index_chunk]
+                    l_bookmark.append(bookmark)
+                    l_bookmark.append(bookmark)
+
+        l_int_actual_n_sam_records_per_chunk.append(int_n_sam_record_count)
+        l_bookmark.append(["", -1, int_index_chunk])
+        l_bookmark = np.array(l_bookmark, dtype=object).reshape(
+            int(len(l_bookmark) / 2), 6
+        )  # reshape bookmark so that each record contains bookmark of the start point and end points
+        df_bookmark = pd.DataFrame(l_bookmark, columns=l_col)
+    else:
+        df_bookmark = pd.DataFrame([["single_thread"] * 6], columns=l_col)
     return df_bookmark, l_int_actual_n_sam_records_per_chunk
 
-def Bookmark_Generator( path_file_bam, int_min_mapq_unique_mapped, int_num_sam_records_for_each_chunk = 1000000, int_n_bases_padding_around_interval = 10, verbose = False, l_dict_it = [ ], flag_ignore_record_with_flag_secondary_alignment = True, flag_ignore_record_with_flag_optical_or_pcr_duplicate = True, flag_genome_without_chr_prefix_was_used_for_l_dict_it = True ) :
-    """  # 2022-01-17 21:50:42 
+
+def Bookmark_Generator(
+    path_file_bam,
+    int_min_mapq_unique_mapped,
+    int_num_sam_records_for_each_chunk=1000000,
+    int_n_bases_padding_around_interval=10,
+    verbose=False,
+    l_dict_it=[],
+    flag_ignore_record_with_flag_secondary_alignment=True,
+    flag_ignore_record_with_flag_optical_or_pcr_duplicate=True,
+    flag_genome_without_chr_prefix_was_used_for_l_dict_it=True,
+):
+    """# 2022-01-17 21:50:42
     iterate the given BAM file twice to create a bookmark to mark the start and end of each chunk for simultaneous access of the BAM file.
     yield a single bookmark at a time
     WARNING: there might be a little overlap of reads analyzed by each process since the chunk boundary is marked with ( qname, flag, refname, refstart ). If the two SAM records with the same ( qname, flag, refname, refstart ), the reads between the two 'identical' SAM records might be analyzed twice by two processes analyzing the two chunk sharing the boundary (however, it is unlikely that this will happens in a typical BAM file).
 
     'path_file_bam' : indexed (with .bai file) BAM file to be create bookmarks for access by multiple processes
-    'int_num_sam_records_for_each_chunk' : a guidance to the number of sam records contained in each chunk 
-    'l_dict_it' : a list of dictionaries of interval trees (pip intervaltree package) containing intervals (genes and repeat annotations, etc.). When boundaries between chunk overlaps with the given intervals, it will be adjusted so that the boundary is at least 'int_n_bases_padding_around_interval' base pair away from the interval. 
+    'int_num_sam_records_for_each_chunk' : a guidance to the number of sam records contained in each chunk
+    'l_dict_it' : a list of dictionaries of interval trees (pip intervaltree package) containing intervals (genes and repeat annotations, etc.). When boundaries between chunk overlaps with the given intervals, it will be adjusted so that the boundary is at least 'int_n_bases_padding_around_interval' base pair away from the interval.
         This functionality will allow analyzing all reads aligned to a single interval in the 'dict_it' to be analyzed in a single thread, thus abolishing the need to combine results from all threads to produce interval-level output, thus simplifying  downstream analysis. if chromosome name contains 'chr' prefix, please set 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' to False
     'flag_genome_without_chr_prefix_was_used_for_l_dict_it' : (default = True) Please set this flag to False if the chromosome names of the given 'l_dict_it' annotations have a 'chr' prefix.
 
     returns
     bookmark, n_sam_records
     bookmark's columns : l_col = [ 'id_refname_start', 'int_refstart_start', 'int_index_chunk_start', 'id_refname_end', 'int_refstart_end', 'int_index_chunk_end' ]
     """
-    if isinstance( l_dict_it, dict ) : # if a single dict_it is given, wrap the dict_it inside a list
-        l_dict_it = [ l_dict_it ]
-
-    ''' retrieve sequence length of reference sequence used in the input BAM file from the BAM header '''
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        dict_header = samfile.header.to_dict( )
-    dict_seqname_to_len_seq = pd.DataFrame( dict_header[ 'SQ' ] ).set_index( 'SN' ).LN.to_dict( )
+    if isinstance(
+        l_dict_it, dict
+    ):  # if a single dict_it is given, wrap the dict_it inside a list
+        l_dict_it = [l_dict_it]
+
+    """ retrieve sequence length of reference sequence used in the input BAM file from the BAM header """
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        dict_header = samfile.header.to_dict()
+    dict_seqname_to_len_seq = (
+        pd.DataFrame(dict_header["SQ"]).set_index("SN").LN.to_dict()
+    )
 
     """ define internal functions """
-    def __chromosome_name_remove_chr__( str_name_chrom ) :
-        ''' remove 'chr' prefix from the chromosome name '''
-        if 'chr' == str_name_chrom[ : 3 ] :
-            return str_name_chrom[ 3 : ]
-        else :
+
+    def __chromosome_name_remove_chr__(str_name_chrom):
+        """remove 'chr' prefix from the chromosome name"""
+        if "chr" == str_name_chrom[:3]:
+            return str_name_chrom[3:]
+        else:
             return str_name_chrom
 
-    def __l_bookmark_to_df_bookmark__( l_bookmark ) :
-        ''' convert l_bookmark to df_bookmark for a single chunk '''
-        l_col = [ 'id_refname_start', 'int_refstart_start', 'int_index_chunk_start', 'id_refname_end', 'int_refstart_end', 'int_index_chunk_end' ]
-        l_bookmark = np.array( l_bookmark, dtype = object ).reshape( int( len( l_bookmark ) / 2 ), 6 ) # reshape bookmark so that each record contains bookmark of the start point and end points
-        df_bookmark = pd.DataFrame( l_bookmark, columns = l_col )
+    def __l_bookmark_to_df_bookmark__(l_bookmark):
+        """convert l_bookmark to df_bookmark for a single chunk"""
+        l_col = [
+            "id_refname_start",
+            "int_refstart_start",
+            "int_index_chunk_start",
+            "id_refname_end",
+            "int_refstart_end",
+            "int_index_chunk_end",
+        ]
+        l_bookmark = np.array(l_bookmark, dtype=object).reshape(
+            int(len(l_bookmark) / 2), 6
+        )  # reshape bookmark so that each record contains bookmark of the start point and end points
+        df_bookmark = pd.DataFrame(l_bookmark, columns=l_col)
         return df_bookmark
 
     """ Compose list of bookmarks for iterating input BAM file using multiple threads """
     """ retrieve the positions and the id_reads at the start and stop points ('bookmark') for multiprocessing """
-    ''' retrieve bookmarks to mark the start and ends of contigs for each chunnk '''
-    l_bookmark = [ ] # empty bookmark
+    """ retrieve bookmarks to mark the start and ends of contigs for each chunnk """
+    l_bookmark = []  # empty bookmark
     flag_has_bookmark_been_initialized = False
-    int_start_possible_boundary = None # start position of the possible boundary # will be set to non-None value when the desired number of records in the current chunk has been reached its target and the boundary is being set or being adjusted
+    int_start_possible_boundary = None  # start position of the possible boundary # will be set to non-None value when the desired number of records in the current chunk has been reached its target and the boundary is being set or being adjusted
     int_n_sam_record_count = 0
     int_index_chunk = 0
-    id_refname_current = None # default reference name
+    id_refname_current = None  # default reference name
 
     # iterate the entire BAM file to retrieve the total number of SAM records
-    with pysam.AlignmentFile( path_file_bam, 'rb' ) as samfile :
-        for r in samfile.fetch( ) :
-            ''' filter alignments based on mapq and flag '''
-            if r.mapq < int_min_mapq_unique_mapped : # skip read whose mapq is below 'int_min_mapq_unique_mapped'
+    with pysam.AlignmentFile(path_file_bam, "rb") as samfile:
+        for r in samfile.fetch():
+            """filter alignments based on mapq and flag"""
+            if (
+                r.mapq < int_min_mapq_unique_mapped
+            ):  # skip read whose mapq is below 'int_min_mapq_unique_mapped'
                 continue
             # ignore records with flag indicating secondary alignment
-            if flag_ignore_record_with_flag_secondary_alignment and ( r.flag & ( 1 << 8 ) ) :
+            if flag_ignore_record_with_flag_secondary_alignment and (r.flag & (1 << 8)):
                 continue
             # ignore records with flag indicating the alignment is optical pcr duplicates
-            if flag_ignore_record_with_flag_optical_or_pcr_duplicate and ( r.flag & ( 1 << 10 ) ) :
+            if flag_ignore_record_with_flag_optical_or_pcr_duplicate and (
+                r.flag & (1 << 10)
+            ):
                 continue
 
             # retrieve SAM record info.
-            refname = r.reference_name 
+            refname = r.reference_name
             refstart = r.reference_start
             refend = r.reference_end
             qname = r.qname
             flag = r.flag
 
             # initialize the bookmarks
-            if not flag_has_bookmark_been_initialized :
-                l_bookmark.append( [ refname, refstart, 0 ] ) # initialize bookmark by assigning the first sam record to the index_chunk 0
+            if not flag_has_bookmark_been_initialized:
+                l_bookmark.append(
+                    [refname, refstart, 0]
+                )  # initialize bookmark by assigning the first sam record to the index_chunk 0
                 id_refname_current = refname
                 flag_has_bookmark_been_initialized = True
                 continue
 
             int_n_sam_record_count += 1
 
             """ mark the change of contig by adding bookmarks """
-            ''' if the next chromosome has been reached while for searching for next gene boundary, the boundary is considered passed, and the new chunk will be initiated.'''
-            if id_refname_current != refname :
-                if verbose :
-                    print( f'chromosome changed from {id_refname_current} to {refname} at chunk_{int_index_chunk}:{int_n_sam_record_count}' )
+            """ if the next chromosome has been reached while for searching for next gene boundary, the boundary is considered passed, and the new chunk will be initiated."""
+            if id_refname_current != refname:
+                if verbose:
+                    print(
+                        f"chromosome changed from {id_refname_current} to {refname} at chunk_{int_index_chunk}:{int_n_sam_record_count}"
+                    )
                 id_refname_current = refname
-                ''' handle the case when contig changes while the chunk boundary is being searched '''
-                if int_start_possible_boundary is not None : 
+                """ handle the case when contig changes while the chunk boundary is being searched """
+                if int_start_possible_boundary is not None:
                     # retrieve stats about the current chunk and initializes the next chunk
                     int_start_possible_boundary = None
                     int_actual_n_sam_records_per_chunk = int_n_sam_record_count - 1
-                    if verbose :
-                        print( f'new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)' )
+                    if verbose:
+                        print(
+                            f"new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)"
+                        )
                     int_index_chunk += 1
                     int_n_sam_record_count = 1
-                    bookmark = [ refname, 0, int_index_chunk ]
-                    l_bookmark.append( bookmark ) 
-                    ''' yield current bookmark and initialize the next bookmark '''
-                    yield __l_bookmark_to_df_bookmark__( l_bookmark ), int_actual_n_sam_records_per_chunk
-                    l_bookmark = [ ]
-                    l_bookmark.append( bookmark )
-                else :
-                    bookmark = [ refname, 0, int_index_chunk ]
-                    l_bookmark.append( bookmark ) 
-                    l_bookmark.append( bookmark )
+                    bookmark = [refname, 0, int_index_chunk]
+                    l_bookmark.append(bookmark)
+                    """ yield current bookmark and initialize the next bookmark """
+                    yield __l_bookmark_to_df_bookmark__(
+                        l_bookmark
+                    ), int_actual_n_sam_records_per_chunk
+                    l_bookmark = []
+                    l_bookmark.append(bookmark)
+                else:
+                    bookmark = [refname, 0, int_index_chunk]
+                    l_bookmark.append(bookmark)
+                    l_bookmark.append(bookmark)
 
             """
             Search boundaries 
             """
             # initialize the next chunk if the 'int_n_sam_record_count' reached the assigned number of sam records for the current chunk (process)
-            if int_n_sam_record_count > int_num_sam_records_for_each_chunk :
-                ''' set default boundary (current position + 1) '''
-                if int_start_possible_boundary is None :
+            if int_n_sam_record_count > int_num_sam_records_for_each_chunk:
+                """set default boundary (current position + 1)"""
+                if int_start_possible_boundary is None:
                     int_start_possible_boundary = refstart + 1
-                ''' iterate until reaching the possible chunk boundary '''
-                if int_start_possible_boundary is not None :
-                    if refstart < int_start_possible_boundary : # if the next possible boundary has not been reached 
+                """ iterate until reaching the possible chunk boundary """
+                if int_start_possible_boundary is not None:
+                    if (
+                        refstart < int_start_possible_boundary
+                    ):  # if the next possible boundary has not been reached
                         continue
 
                 """
                 Possible boundary has been reached
                 """
-                ''' check whether the current position overlaps with intervals in the given list of dictionaries of interval trees, and set the next possible boundary based on the overlapped intervals '''
-                l_adjusted_boundary_based_on_overlapped_interval = [ ]
+                """ check whether the current position overlaps with intervals in the given list of dictionaries of interval trees, and set the next possible boundary based on the overlapped intervals """
+                l_adjusted_boundary_based_on_overlapped_interval = []
                 # search overlapped intervals
-                int_len_seq_current_contig = dict_seqname_to_len_seq[ refname ] # retrieve the length of the current contig
-                refname_for_l_dict_it = __chromosome_name_remove_chr__( refname ) if flag_genome_without_chr_prefix_was_used_for_l_dict_it else refname # handle if BAM file's genome chromosome name convention and 'l_dict_it' annotations' chromosome name convention is different # retrieve refname without 'chr' prefix if 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' is True
-
-                for dict_it in l_dict_it :
-                    if refname_for_l_dict_it in dict_it :
-                        for start, end, anno_name in dict_it[ refname_for_l_dict_it ][ refstart ] :
-                            l_adjusted_boundary_based_on_overlapped_interval.append( min( end + int_n_bases_padding_around_interval, int_len_seq_current_contig - 1 ) ) # maximum boundary is the end position of the contig
-                            if verbose :
-                                print( f"for chunk {int_index_chunk}, the possible boundary currently overlaps with {refname_for_l_dict_it}:{start}-{end}|{anno_name}" )
+                int_len_seq_current_contig = dict_seqname_to_len_seq[
+                    refname
+                ]  # retrieve the length of the current contig
+                refname_for_l_dict_it = (
+                    __chromosome_name_remove_chr__(refname)
+                    if flag_genome_without_chr_prefix_was_used_for_l_dict_it
+                    else refname
+                )  # handle if BAM file's genome chromosome name convention and 'l_dict_it' annotations' chromosome name convention is different # retrieve refname without 'chr' prefix if 'flag_genome_without_chr_prefix_was_used_for_l_dict_it' is True
+
+                for dict_it in l_dict_it:
+                    if refname_for_l_dict_it in dict_it:
+                        for start, end, anno_name in dict_it[refname_for_l_dict_it][
+                            refstart
+                        ]:
+                            l_adjusted_boundary_based_on_overlapped_interval.append(
+                                min(
+                                    end + int_n_bases_padding_around_interval,
+                                    int_len_seq_current_contig - 1,
+                                )
+                            )  # maximum boundary is the end position of the contig
+                            if verbose:
+                                print(
+                                    f"for chunk {int_index_chunk}, the possible boundary currently overlaps with {refname_for_l_dict_it}:{start}-{end}|{anno_name}"
+                                )
                 # if there is any overlaps with the intervals, start adjusting boundaries
-                if len( l_adjusted_boundary_based_on_overlapped_interval ) != 0 :
+                if len(l_adjusted_boundary_based_on_overlapped_interval) != 0:
                     int_start_possible_boundary_previous = int_start_possible_boundary
                     # set the next possible boundary
-                    int_start_possible_boundary = max( l_adjusted_boundary_based_on_overlapped_interval ) # use the farthest interval ends when setting the next potential boundary 
-                    if verbose :
-                        print( f'for chunk {int_index_chunk}, the possible boundary will change from {refname_for_l_dict_it}:{int_start_possible_boundary_previous} to {refname_for_l_dict_it}:{int_start_possible_boundary} ({int_start_possible_boundary - refstart}bp shift) when int_n_sam_record_count = {int_n_sam_record_count}' )
+                    int_start_possible_boundary = max(
+                        l_adjusted_boundary_based_on_overlapped_interval
+                    )  # use the farthest interval ends when setting the next potential boundary
+                    if verbose:
+                        print(
+                            f"for chunk {int_index_chunk}, the possible boundary will change from {refname_for_l_dict_it}:{int_start_possible_boundary_previous} to {refname_for_l_dict_it}:{int_start_possible_boundary} ({int_start_possible_boundary - refstart}bp shift) when int_n_sam_record_count = {int_n_sam_record_count}"
+                        )
                     continue
 
                 """
                 Finalize boundary
                 """
-                ''' if the current position does not overlap with any intervals, set the current position as the boundary between chunks '''
-                int_start_possible_boundary = None # set 'int_start_possible_boundary' to indicate boundary is not being searched
+                """ if the current position does not overlap with any intervals, set the current position as the boundary between chunks """
+                int_start_possible_boundary = None  # set 'int_start_possible_boundary' to indicate boundary is not being searched
                 int_actual_n_sam_records_per_chunk = int_n_sam_record_count - 1
-                if verbose :
-                    print( f'new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)' )
+                if verbose:
+                    print(
+                        f"new chunk initiated (chunk {int_index_chunk + 1}) (chunk {int_index_chunk} has {int_n_sam_record_count} number of reads)"
+                    )
                 # initialized the next chunk
                 int_n_sam_record_count = 1
                 int_index_chunk += 1
                 # add a bookmark of the current position to mark the start of the new chunk
-                bookmark = [ refname, refstart, int_index_chunk ]
-                l_bookmark.append( bookmark )
-                ''' yield current bookmark and initialize the next bookmark '''
-                yield __l_bookmark_to_df_bookmark__( l_bookmark ), int_actual_n_sam_records_per_chunk
-                l_bookmark = [ ]
-                l_bookmark.append( bookmark )
-    ''' yield final bookmark '''
-    l_bookmark.append( [ '', -1, int_index_chunk ] )
-    yield __l_bookmark_to_df_bookmark__( l_bookmark ), int_n_sam_record_count # yield the bookmark for the final chunk
-
-def Call_Variant( 
-    r, 
-    dict_fasta_genome, 
-    function_for_processing_reference_name = None
-) :
-    ''' # 2023-01-07 18:58:43 
+                bookmark = [refname, refstart, int_index_chunk]
+                l_bookmark.append(bookmark)
+                """ yield current bookmark and initialize the next bookmark """
+                yield __l_bookmark_to_df_bookmark__(
+                    l_bookmark
+                ), int_actual_n_sam_records_per_chunk
+                l_bookmark = []
+                l_bookmark.append(bookmark)
+    """ yield final bookmark """
+    l_bookmark.append(["", -1, int_index_chunk])
+    yield __l_bookmark_to_df_bookmark__(
+        l_bookmark
+    ), int_n_sam_record_count  # yield the bookmark for the final chunk
+
+
+def Call_Variant(r, dict_fasta_genome, function_for_processing_reference_name=None):
+    """# 2023-01-07 18:58:43
     perform vcf-style variant calling of a single aligned read (pysam read object) using a given genome
     return a list of mutations and corrected read sequence
-    
+
     'r' : AlignedSegment object returned by pysam
     'dict_fasta_genome' : dictionary of genome sequences
     'function_for_processing_reference_name' : a function that can be applied to reference name to make reference_name used in r consistent with those used in 'dict_fasta_genome' and the id_mut that will be returned by the current function. (e.g. a function that can remove 'chr' prefix from the reference name, if chromosome name without the 'chr' prefix is being used)
 
     --- returns ---
     'l_mut' : list of variants with the following nomenclature
     {refname}:{refpos}:{ref}>{alt}, where refpos, ref, alt follows nomenclature of VCF file
-    '''
-    pos_read, pos_ref = 0, 0 # current position in the extracted reference sequence and the current read
-    
+    """
+    pos_read, pos_ref = (
+        0,
+        0,
+    )  # current position in the extracted reference sequence and the current read
+
     # parse a sam record
     arr_qual = r.query_qualities
     seq = r.seq
     ref_name = r.reference_name
-    if function_for_processing_reference_name is not None :
-        ref_name = function_for_processing_reference_name( ref_name )
+    if function_for_processing_reference_name is not None:
+        ref_name = function_for_processing_reference_name(ref_name)
     ref_start = r.reference_start
     cigartuples = r.cigartuples
     alen = r.alen
-    
+
     # retrieve a part of the reference sequence where the current read was aligned
-    seq_ref = dict_fasta_genome[ ref_name ][ ref_start : ref_start + alen ] 
-    
-    l_mut = [ ]
+    seq_ref = dict_fasta_genome[ref_name][ref_start : ref_start + alen]
+
+    l_mut = []
 
     """
     # define interger representation of the CIGAR operations used in BAM files
     
     M 0 alignment match (can be a sequence match or mismatch)
     I 1 insertion to the reference
     D 2 deletion from the reference
@@ -601,87 +845,112 @@
     int_cigarop_N = 3
     int_cigarop_S = 4
     int_cigarop_H = 5
     int_cigarop_P = 6
     int_cigarop_equal = 7
     int_cigarop_X = 8
 
-    ns = dict( ) # create a namespace
+    ns = dict()  # create a namespace
     # initialilze the namespace
-    ns[ 'pos_ref_variant_start' ] = None # 0-based coordinate of the start of the alternative allele on the reference
-    ns[ 'pos_ref_variant_end' ] = None # 0-based coordinate of the end of the alternative allele on the reference
-    ns[ 'alt' ] = ''
-    def __update_alt( pos_ref : int, len_bases_ref : int = 0, bases_alt : str = '' ) :
-        """ # 2023-01-07 17:51:14 
-        """
+    ns[
+        "pos_ref_variant_start"
+    ] = None  # 0-based coordinate of the start of the alternative allele on the reference
+    ns[
+        "pos_ref_variant_end"
+    ] = None  # 0-based coordinate of the end of the alternative allele on the reference
+    ns["alt"] = ""
+
+    def __update_alt(pos_ref: int, len_bases_ref: int = 0, bases_alt: str = ""):
+        """# 2023-01-07 17:51:14"""
         # initialize variant
-        if ns[ 'pos_ref_variant_start' ] is None :
-            ns[ 'pos_ref_variant_start' ] = pos_ref
-            ns[ 'pos_ref_variant_end' ] = pos_ref
-            ns[ 'alt' ] = ''
-        ns[ 'pos_ref_variant_end' ] += len_bases_ref
-        ns[ 'alt' ] += bases_alt
-    def __flush_alt( ) :
-        """ # 2023-01-07 17:24:20 
+        if ns["pos_ref_variant_start"] is None:
+            ns["pos_ref_variant_start"] = pos_ref
+            ns["pos_ref_variant_end"] = pos_ref
+            ns["alt"] = ""
+        ns["pos_ref_variant_end"] += len_bases_ref
+        ns["alt"] += bases_alt
+
+    def __flush_alt():
+        """# 2023-01-07 17:24:20
         flush variant allele
         """
-        if ns[ 'pos_ref_variant_start' ] is not None :
-            if len( ns[ 'alt' ] ) == 0 or ns[ 'pos_ref_variant_end' ] == ns[ 'pos_ref_variant_start' ] : # for simple insertion/deletion variants, add a single base pair of the reference before insertion or deletion to record the variant
-                ns[ 'pos_ref_variant_start' ] -= 1
-                ns[ 'alt' ] = seq_ref[ ns[ 'pos_ref_variant_start' ] ] + ns[ 'alt' ]
-            l_mut.append( f"{ref_name}:{ref_start + 1 + ns[ 'pos_ref_variant_start' ]}:{seq_ref[ ns[ 'pos_ref_variant_start' ] : ns[ 'pos_ref_variant_end' ] ]}>{ns[ 'alt' ]}" ) # append the variant
-            ns[ 'pos_ref_variant_start' ] = None
-            ns[ 'pos_ref_variant_end' ] = None
-            ns[ 'alt' ] = ''
-    for int_oper, n_bases in cigartuples :
-        if int_oper == int_cigarop_M :
-            for _ in range( n_bases ) :
-                str_base_read, str_base_ref, str_qual_read = seq[ pos_read ], seq_ref[ pos_ref ], arr_qual[ pos_read ]
-                if str_base_read == str_base_ref :
-                    __flush_alt( ) # flush a variant
-                else :
-                    __update_alt( pos_ref, len_bases_ref = 1, bases_alt = str_base_read )
+        if ns["pos_ref_variant_start"] is not None:
+            if (
+                len(ns["alt"]) == 0
+                or ns["pos_ref_variant_end"] == ns["pos_ref_variant_start"]
+            ):  # for simple insertion/deletion variants, add a single base pair of the reference before insertion or deletion to record the variant
+                ns["pos_ref_variant_start"] -= 1
+                ns["alt"] = seq_ref[ns["pos_ref_variant_start"]] + ns["alt"]
+            l_mut.append(
+                f"{ref_name}:{ref_start + 1 + ns[ 'pos_ref_variant_start' ]}:{seq_ref[ ns[ 'pos_ref_variant_start' ] : ns[ 'pos_ref_variant_end' ] ]}>{ns[ 'alt' ]}"
+            )  # append the variant
+            ns["pos_ref_variant_start"] = None
+            ns["pos_ref_variant_end"] = None
+            ns["alt"] = ""
+
+    for int_oper, n_bases in cigartuples:
+        if int_oper == int_cigarop_M:
+            for _ in range(n_bases):
+                str_base_read, str_base_ref, str_qual_read = (
+                    seq[pos_read],
+                    seq_ref[pos_ref],
+                    arr_qual[pos_read],
+                )
+                if str_base_read == str_base_ref:
+                    __flush_alt()  # flush a variant
+                else:
+                    __update_alt(pos_ref, len_bases_ref=1, bases_alt=str_base_read)
                 pos_ref += 1
                 pos_read += 1
-        elif int_oper == int_cigarop_N :
-            __flush_alt( ) # flush a variant
+        elif int_oper == int_cigarop_N:
+            __flush_alt()  # flush a variant
             pos_ref += n_bases
-        elif int_oper == int_cigarop_S :
-            __flush_alt( ) # flush a variant
+        elif int_oper == int_cigarop_S:
+            __flush_alt()  # flush a variant
             pos_read += n_bases
-        elif int_oper == int_cigarop_I :
-            __update_alt( pos_ref, bases_alt = seq[ pos_read : pos_read + n_bases ] )
+        elif int_oper == int_cigarop_I:
+            __update_alt(pos_ref, bases_alt=seq[pos_read : pos_read + n_bases])
             pos_read += n_bases
-        elif int_oper == int_cigarop_D :
-            __update_alt( pos_ref, len_bases_ref = n_bases )
+        elif int_oper == int_cigarop_D:
+            __update_alt(pos_ref, len_bases_ref=n_bases)
             pos_ref += n_bases
-        elif int_oper == int_cigarop_H :
-            __flush_alt( ) # flush a variant
+        elif int_oper == int_cigarop_H:
+            __flush_alt()  # flush a variant
             pass
-        elif int_oper == int_cigarop_P :
-            __flush_alt( ) # flush a variant
+        elif int_oper == int_cigarop_P:
+            __flush_alt()  # flush a variant
             pass
-        elif int_oper == int_cigarop_equal :
-            __flush_alt( ) # flush a variant
+        elif int_oper == int_cigarop_equal:
+            __flush_alt()  # flush a variant
             pos_ref += n_bases
             pos_read += n_bases
-        elif int_oper == int_cigarop_X :
-            for _ in range( n_bases ) :
-                str_base_read, str_qual_read = seq[ pos_read ], arr_qual[ pos_read ]
-                __update_alt( pos_ref, 1, str_base_read )
+        elif int_oper == int_cigarop_X:
+            for _ in range(n_bases):
+                str_base_read, str_qual_read = seq[pos_read], arr_qual[pos_read]
+                __update_alt(pos_ref, 1, str_base_read)
                 pos_ref += 1
                 pos_read += 1
-    __flush_alt( ) # flush a variant
+    __flush_alt()  # flush a variant
     return l_mut
-    
-def Retrieve_Variant( r, dict_fasta_genome, set_mut_filtered = None, return_corrected_read_sequence = False, flag_ignore_indel = False, flag_return_as_string = True, flag_return_matched = False, function_for_processing_reference_name = None ) :
-    ''' # 2022-01-15 00:37:28 
+
+
+def Retrieve_Variant(
+    r,
+    dict_fasta_genome,
+    set_mut_filtered=None,
+    return_corrected_read_sequence=False,
+    flag_ignore_indel=False,
+    flag_return_as_string=True,
+    flag_return_matched=False,
+    function_for_processing_reference_name=None,
+):
+    """# 2022-01-15 00:37:28
     perform variant calling of a single aligned read (pysam read object) using a given genome
     return a list of mutations and corrected read sequence
-    
+
     'r' : AlignedSegment object returned by pysam
     'dict_fasta_genome' : dictionary of genome sequences
     'set_mut_filtered' : only consider mutations in the given 'set_mut_filtered'. only valid when 'return_corrected_read_sequence' = True
     'return_corrected_read_sequence' : return aligned read sequence after hard-clipping and filtering variants using 'set_mut_filtered'
     'flag_ignore_indel' : ignore insertion and deletion mutation calls
     'flag_return_as_string' : return a called mutation as a string in the following format: f"{reference_name}:{start}_{cigar_operation}_{mutation}". If set to False, return the called mutation as a tuple (reference_name, start, int_operation, mutation, quality)
     'flag_return_matched' : return 'id_mut' even when there is no mutation. the 'int_operation' for matched base is int_cigarop_M
@@ -693,31 +962,34 @@
     {refname}:{refpos}_{refbase}>{mutbase}
 
     # insertion:
     {refname}:{refpos_after_the_insertion}_ins_{inserted_bases}
 
     # deletion:
     {refname}:{refpos_of_the_first_base_of_the_deletion}_del_{number_of_deleted_bases}
-    '''
-    pos_read, pos_ref = 0, 0 # current position in the extracted reference sequence and the current read
-    
+    """
+    pos_read, pos_ref = (
+        0,
+        0,
+    )  # current position in the extracted reference sequence and the current read
+
     # parse a sam record
     arr_qual = r.query_qualities
     seq = r.seq
     ref_name = r.reference_name
-    if function_for_processing_reference_name is not None :
-        ref_name = function_for_processing_reference_name( ref_name )
+    if function_for_processing_reference_name is not None:
+        ref_name = function_for_processing_reference_name(ref_name)
     ref_start = r.reference_start
     cigartuples = r.cigartuples
     alen = r.alen
-    
+
     # retrieve a part of the reference sequence where the current read was aligned
-    seq_ref = dict_fasta_genome[ ref_name ][ ref_start : ref_start + alen ] 
-    
-    l_mut = [ ]
+    seq_ref = dict_fasta_genome[ref_name][ref_start : ref_start + alen]
+
+    l_mut = []
 
     """
     # define interger representation of the CIGAR operations used in BAM files
     
     M 0 alignment match (can be a sequence match or mismatch)
     I 1 insertion to the reference
     D 2 deletion from the reference
@@ -734,255 +1006,493 @@
     int_cigarop_N = 3
     int_cigarop_S = 4
     int_cigarop_H = 5
     int_cigarop_P = 6
     int_cigarop_equal = 7
     int_cigarop_X = 8
 
-    if return_corrected_read_sequence : # correction mode
-        str_seq_corrected_read = '' # corrected read sequence after hard clipping and filtering variants
-        for int_oper, n_bases in cigartuples :
-            if int_oper == int_cigarop_M :
-                for _ in range( n_bases ) :
-                    str_base_read, str_base_ref, str_qual_read = seq[ pos_read ], seq_ref[ pos_ref ], arr_qual[ pos_read ]
-                    str_base_read_corrected = str_base_ref # default corrected read base = ref
-                    if str_base_read != str_base_ref :
-                        id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'X', str_base_read, str_qual_read ) # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
-                        if set_mut_filtered is None or id_mut in set_mut_filtered :
-                            l_mut.append( id_mut )
+    if return_corrected_read_sequence:  # correction mode
+        str_seq_corrected_read = (
+            ""  # corrected read sequence after hard clipping and filtering variants
+        )
+        for int_oper, n_bases in cigartuples:
+            if int_oper == int_cigarop_M:
+                for _ in range(n_bases):
+                    str_base_read, str_base_ref, str_qual_read = (
+                        seq[pos_read],
+                        seq_ref[pos_ref],
+                        arr_qual[pos_read],
+                    )
+                    str_base_read_corrected = (
+                        str_base_ref  # default corrected read base = ref
+                    )
+                    if str_base_read != str_base_ref:
+                        id_mut = (
+                            f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}"
+                            if flag_return_as_string
+                            else (
+                                ref_name,
+                                ref_start + pos_ref,
+                                "X",
+                                str_base_read,
+                                str_qual_read,
+                            )
+                        )  # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
+                        if set_mut_filtered is None or id_mut in set_mut_filtered:
+                            l_mut.append(id_mut)
                             str_base_read_corrected = str_base_read
-                    elif flag_return_matched :
-                        id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'M', str_base_read, str_qual_read ) # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
-                        l_mut.append( id_mut )
-                    str_seq_corrected_read += str_base_read_corrected # add corrected read 
+                    elif flag_return_matched:
+                        id_mut = (
+                            f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}"
+                            if flag_return_as_string
+                            else (
+                                ref_name,
+                                ref_start + pos_ref,
+                                "M",
+                                str_base_read,
+                                str_qual_read,
+                            )
+                        )  # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
+                        l_mut.append(id_mut)
+                    str_seq_corrected_read += (
+                        str_base_read_corrected  # add corrected read
+                    )
                     pos_ref += 1
                     pos_read += 1
-            elif int_oper == int_cigarop_N :
+            elif int_oper == int_cigarop_N:
                 pos_ref += n_bases
-            elif int_oper == int_cigarop_S :
+            elif int_oper == int_cigarop_S:
                 pos_read += n_bases
-            elif int_oper == int_cigarop_I :
-                id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_ins_{seq[ pos_read : pos_read + n_bases ]}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'I', seq[ pos_read : pos_read + n_bases ], arr_qual[ pos_read : pos_read + n_bases ] ) # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
-                if not flag_ignore_indel and ( set_mut_filtered is None or id_mut in set_mut_filtered ) :
-                    l_mut.append( id_mut ) 
-                    str_seq_corrected_read += seq[ pos_read : pos_read + n_bases ] # add inserted sequence (if insertion is valid)
+            elif int_oper == int_cigarop_I:
+                id_mut = (
+                    f"{ref_name}:{ref_start + 1 + pos_ref}_ins_{seq[ pos_read : pos_read + n_bases ]}"
+                    if flag_return_as_string
+                    else (
+                        ref_name,
+                        ref_start + pos_ref,
+                        "I",
+                        seq[pos_read : pos_read + n_bases],
+                        arr_qual[pos_read : pos_read + n_bases],
+                    )
+                )  # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
+                if not flag_ignore_indel and (
+                    set_mut_filtered is None or id_mut in set_mut_filtered
+                ):
+                    l_mut.append(id_mut)
+                    str_seq_corrected_read += seq[
+                        pos_read : pos_read + n_bases
+                    ]  # add inserted sequence (if insertion is valid)
                 pos_read += n_bases
-            elif int_oper == int_cigarop_D :
-                id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_del_{n_bases}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'D', n_bases, None ) # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
-                if not flag_ignore_indel and ( set_mut_filtered is None or id_mut in set_mut_filtered ) :
-                    l_mut.append( id_mut ) 
-                else :
-                    str_seq_corrected_read += seq_ref[ pos_ref : pos_ref + n_bases ] # add deleted reference sequence (if deletion is invalid)
+            elif int_oper == int_cigarop_D:
+                id_mut = (
+                    f"{ref_name}:{ref_start + 1 + pos_ref}_del_{n_bases}"
+                    if flag_return_as_string
+                    else (ref_name, ref_start + pos_ref, "D", n_bases, None)
+                )  # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
+                if not flag_ignore_indel and (
+                    set_mut_filtered is None or id_mut in set_mut_filtered
+                ):
+                    l_mut.append(id_mut)
+                else:
+                    str_seq_corrected_read += seq_ref[
+                        pos_ref : pos_ref + n_bases
+                    ]  # add deleted reference sequence (if deletion is invalid)
                 pos_ref += n_bases
-            elif int_oper == int_cigarop_H :
+            elif int_oper == int_cigarop_H:
                 pass
-            elif int_oper == int_cigarop_P :
+            elif int_oper == int_cigarop_P:
                 pass
-            elif int_oper == int_cigarop_equal :
-                if flag_return_matched :
-                    str_base_read, str_qual_read = seq[ pos_read ], arr_qual[ pos_read ]
-                    id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'M', str_base_read, str_qual_read ) # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
-                    l_mut.append( id_mut )
-                str_seq_corrected_read += seq[ pos_read : pos_read + n_bases ] # add read sequences
+            elif int_oper == int_cigarop_equal:
+                if flag_return_matched:
+                    str_base_read, str_qual_read = seq[pos_read], arr_qual[pos_read]
+                    id_mut = (
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}"
+                        if flag_return_as_string
+                        else (
+                            ref_name,
+                            ref_start + pos_ref,
+                            "M",
+                            str_base_read,
+                            str_qual_read,
+                        )
+                    )  # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
+                    l_mut.append(id_mut)
+                str_seq_corrected_read += seq[
+                    pos_read : pos_read + n_bases
+                ]  # add read sequences
                 pos_ref += n_bases
                 pos_read += n_bases
-            elif int_oper == int_cigarop_X :
-                for _ in range( n_bases ) :
-                    str_base_read, str_base_ref, str_qual_read = seq[ pos_read ], seq_ref[ pos_ref ], arr_qual[ pos_read ]
-                    str_base_read_corrected = str_base_ref # default corrected read base = ref
-                    id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'X', str_base_read, str_qual_read ) # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
-                    if set_mut_filtered is None or id_mut in set_mut_filtered :
-                        l_mut.append( id_mut ) 
+            elif int_oper == int_cigarop_X:
+                for _ in range(n_bases):
+                    str_base_read, str_base_ref, str_qual_read = (
+                        seq[pos_read],
+                        seq_ref[pos_ref],
+                        arr_qual[pos_read],
+                    )
+                    str_base_read_corrected = (
+                        str_base_ref  # default corrected read base = ref
+                    )
+                    id_mut = (
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}"
+                        if flag_return_as_string
+                        else (
+                            ref_name,
+                            ref_start + pos_ref,
+                            "X",
+                            str_base_read,
+                            str_qual_read,
+                        )
+                    )  # compose id_mut, 0-based coordinate to 1-based coordinate when returning id_mut as a string
+                    if set_mut_filtered is None or id_mut in set_mut_filtered:
+                        l_mut.append(id_mut)
                         str_base_read_corrected = str_base_read
-                    str_seq_corrected_read += str_base_read_corrected # add corrected read 
+                    str_seq_corrected_read += (
+                        str_base_read_corrected  # add corrected read
+                    )
                     pos_ref += 1
                     pos_read += 1
         return l_mut, str_seq_corrected_read
-    else : # normal mutation calling mode
-        for int_oper, n_bases in cigartuples :
-            if int_oper == int_cigarop_M :
-                for _ in range( n_bases ) :
-                    str_base_read, str_base_ref, str_qual_read = seq[ pos_read ], seq_ref[ pos_ref ], arr_qual[ pos_read ]
-                    if str_base_read != str_base_ref :
-                        l_mut.append( f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'X', str_base_read, str_qual_read ) ) # 0-based coordinate to 1-based coordinate when returning id_mut as a string
-                    elif flag_return_matched :
-                        l_mut.append( f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'M', str_base_read, str_qual_read ) ) # 0-based coordinate to 1-based coordinate when returning id_mut as a string
+    else:  # normal mutation calling mode
+        for int_oper, n_bases in cigartuples:
+            if int_oper == int_cigarop_M:
+                for _ in range(n_bases):
+                    str_base_read, str_base_ref, str_qual_read = (
+                        seq[pos_read],
+                        seq_ref[pos_ref],
+                        arr_qual[pos_read],
+                    )
+                    if str_base_read != str_base_ref:
+                        l_mut.append(
+                            f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}"
+                            if flag_return_as_string
+                            else (
+                                ref_name,
+                                ref_start + pos_ref,
+                                "X",
+                                str_base_read,
+                                str_qual_read,
+                            )
+                        )  # 0-based coordinate to 1-based coordinate when returning id_mut as a string
+                    elif flag_return_matched:
+                        l_mut.append(
+                            f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}"
+                            if flag_return_as_string
+                            else (
+                                ref_name,
+                                ref_start + pos_ref,
+                                "M",
+                                str_base_read,
+                                str_qual_read,
+                            )
+                        )  # 0-based coordinate to 1-based coordinate when returning id_mut as a string
                     pos_ref += 1
                     pos_read += 1
-            elif int_oper == int_cigarop_N :
+            elif int_oper == int_cigarop_N:
                 pos_ref += n_bases
-            elif int_oper == int_cigarop_S :
+            elif int_oper == int_cigarop_S:
                 pos_read += n_bases
-            elif int_oper == int_cigarop_I :
-                if not flag_ignore_indel :
-                    l_mut.append( f"{ref_name}:{ref_start + 1 + pos_ref}_ins_{seq[ pos_read : pos_read + n_bases ]}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'I', seq[ pos_read : pos_read + n_bases ], arr_qual[ pos_read : pos_read + n_bases ] ) ) # 0-based coordinate to 1-based coordinate when returning id_mut as a string
+            elif int_oper == int_cigarop_I:
+                if not flag_ignore_indel:
+                    l_mut.append(
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_ins_{seq[ pos_read : pos_read + n_bases ]}"
+                        if flag_return_as_string
+                        else (
+                            ref_name,
+                            ref_start + pos_ref,
+                            "I",
+                            seq[pos_read : pos_read + n_bases],
+                            arr_qual[pos_read : pos_read + n_bases],
+                        )
+                    )  # 0-based coordinate to 1-based coordinate when returning id_mut as a string
                 pos_read += n_bases
-            elif int_oper == int_cigarop_D :
-                if not flag_ignore_indel :
-                    l_mut.append( f"{ref_name}:{ref_start + 1 + pos_ref}_del_{n_bases}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'D', n_bases, None ) ) # 0-based coordinate to 1-based coordinate when returning id_mut as a string
+            elif int_oper == int_cigarop_D:
+                if not flag_ignore_indel:
+                    l_mut.append(
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_del_{n_bases}"
+                        if flag_return_as_string
+                        else (ref_name, ref_start + pos_ref, "D", n_bases, None)
+                    )  # 0-based coordinate to 1-based coordinate when returning id_mut as a string
                 pos_ref += n_bases
-            elif int_oper == int_cigarop_H :
+            elif int_oper == int_cigarop_H:
                 pass
-            elif int_oper == int_cigarop_P :
+            elif int_oper == int_cigarop_P:
                 pass
-            elif int_oper == int_cigarop_equal :
-                if flag_return_matched :
-                    str_base_read, str_qual_read = seq[ pos_read ], arr_qual[ pos_read ]
-                    id_mut = f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'M', str_base_read, str_qual_read ) # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
-                    l_mut.append( id_mut )
+            elif int_oper == int_cigarop_equal:
+                if flag_return_matched:
+                    str_base_read, str_qual_read = seq[pos_read], arr_qual[pos_read]
+                    id_mut = (
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_read}"
+                        if flag_return_as_string
+                        else (
+                            ref_name,
+                            ref_start + pos_ref,
+                            "M",
+                            str_base_read,
+                            str_qual_read,
+                        )
+                    )  # compose id_mut, convert 0-based coordinate to 1-based coordinate when calling a mutation as a string
+                    l_mut.append(id_mut)
                 pos_ref += n_bases
                 pos_read += n_bases
-            elif int_oper == int_cigarop_X :
-                for _ in range( n_bases ) :
-                    str_base_read, str_qual_read = seq[ pos_read ], arr_qual[ pos_read ]
-                    l_mut.append( f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}" if flag_return_as_string else ( ref_name, ref_start + pos_ref, 'X', str_base_read, str_qual_read ) ) # 0-based coordinate to 1-based coordinate when returning id_mut as a string
+            elif int_oper == int_cigarop_X:
+                for _ in range(n_bases):
+                    str_base_read, str_qual_read = seq[pos_read], arr_qual[pos_read]
+                    l_mut.append(
+                        f"{ref_name}:{ref_start + 1 + pos_ref}_{str_base_ref}>{str_base_read}"
+                        if flag_return_as_string
+                        else (
+                            ref_name,
+                            ref_start + pos_ref,
+                            "X",
+                            str_base_read,
+                            str_qual_read,
+                        )
+                    )  # 0-based coordinate to 1-based coordinate when returning id_mut as a string
                     pos_ref += 1
                     pos_read += 1
         return l_mut
 
-def Get_dict_pysam_alignmentheader_from_dict_seqname_to_len_seq( dict_seqname_to_len_seq ) :
-    ''' # 2022-06-10 17:55:59 
+
+def Get_dict_pysam_alignmentheader_from_dict_seqname_to_len_seq(
+    dict_seqname_to_len_seq,
+):
+    """# 2022-06-10 17:55:59
     compose a dictionary that can be used to build an alignment header from 'dict_seqname_to_len_seq'
-    '''
-    dict_header = dict( )
-    dict_header[ 'HD' ] = { 'VN': '1.6', 'SO': 'coordinate' }
-    dict_header[ 'SQ' ] = list( { 'SN': seqname, 'LN': dict_seqname_to_len_seq[ seqname ] } for seqname in dict_seqname_to_len_seq )
+    """
+    dict_header = dict()
+    dict_header["HD"] = {"VN": "1.6", "SO": "coordinate"}
+    dict_header["SQ"] = list(
+        {"SN": seqname, "LN": dict_seqname_to_len_seq[seqname]}
+        for seqname in dict_seqname_to_len_seq
+    )
     return dict_header
 
-def Convert_mappy_alignment_to_pysam_aligned_segment( qname, seq, qual, mappy_alignment, samfile_header, start = None, flag_mark_as_supplementary_alignment = False ) :
-    ''' # 2022-06-16 00:04:36 
+
+def Convert_mappy_alignment_to_pysam_aligned_segment(
+    qname,
+    seq,
+    qual,
+    mappy_alignment,
+    samfile_header,
+    start=None,
+    flag_mark_as_supplementary_alignment=False,
+):
+    """# 2022-06-16 00:04:36
     convert 'mappy_alignment' (mappy.Alignment record) to pysam.AlignedSegment object
-    
+
     'flag_mark_as_supplementary_alignment' : mark the alignment record for supplementary alignment. for mappy, unlike minimap2 output, supplementary alignment is not marked by default (https://github.com/lh3/minimap2/issues/342). The first alignment can be considered primary, and all other alignment can be marked as supplementary.
     'start' : if a subset sequence of the 'query' sequence was searched using mappy, set this argument as the 0-based coordinate of the start of the subsequence
-    '''
-    len_seq = len( seq )
+    """
+    len_seq = len(seq)
     # set default arguments
-    if start is None :
+    if start is None:
         start = 0
 
-    flag = 0 # initialize flag
-    if not mappy_alignment.is_primary :
+    flag = 0  # initialize flag
+    if not mappy_alignment.is_primary:
         flag ^= 1 << 8
-    if flag_mark_as_supplementary_alignment :
+    if flag_mark_as_supplementary_alignment:
         flag ^= 1 << 11
-    if mappy_alignment.strand == -1 : # mark reverse complemented reads
+    if mappy_alignment.strand == -1:  # mark reverse complemented reads
         flag ^= 1 << 4
         flag_reverse_complemented = True
         # reverse complement reads
-        seq = SEQ.Reverse_Complement( seq )
-        qual = qual[ : : -1 ]
+        seq = SEQ.Reverse_Complement(seq)
+        qual = qual[::-1]
         # retrieve numbers of soft-clipped bases
-        int_num_soft_clipped_bases_left, int_num_soft_clipped_bases_right = len_seq - mappy_alignment.q_en - start, mappy_alignment.q_st + start
-    else :
+        int_num_soft_clipped_bases_left, int_num_soft_clipped_bases_right = (
+            len_seq - mappy_alignment.q_en - start,
+            mappy_alignment.q_st + start,
+        )
+    else:
         # retrieve numbers of soft-clipped bases
-        int_num_soft_clipped_bases_left, int_num_soft_clipped_bases_right = mappy_alignment.q_st + start, len_seq - mappy_alignment.q_en - start
-        
-        
-    # retrieve a modify cigar string
-    cigar_str = ( str( int_num_soft_clipped_bases_left ) + 'S' if int_num_soft_clipped_bases_left > 0 else '' ) + mappy_alignment.cigar_str + ( str( int_num_soft_clipped_bases_right ) + 'S' if int_num_soft_clipped_bases_right else '' )
+        int_num_soft_clipped_bases_left, int_num_soft_clipped_bases_right = (
+            mappy_alignment.q_st + start,
+            len_seq - mappy_alignment.q_en - start,
+        )
 
-    l_sam = [ qname, flag, mappy_alignment.ctg, mappy_alignment.r_st + 1, mappy_alignment.mapq, cigar_str, '*', 0, 0, seq, qual ] # compose a basic sam record using list
+    # retrieve a modify cigar string
+    cigar_str = (
+        (
+            str(int_num_soft_clipped_bases_left) + "S"
+            if int_num_soft_clipped_bases_left > 0
+            else ""
+        )
+        + mappy_alignment.cigar_str
+        + (
+            str(int_num_soft_clipped_bases_right) + "S"
+            if int_num_soft_clipped_bases_right
+            else ""
+        )
+    )
+
+    l_sam = [
+        qname,
+        flag,
+        mappy_alignment.ctg,
+        mappy_alignment.r_st + 1,
+        mappy_alignment.mapq,
+        cigar_str,
+        "*",
+        0,
+        0,
+        seq,
+        qual,
+    ]  # compose a basic sam record using list
     # add tag
-    for name_attr, type_val in zip( [ 'NM', 'MD', 'cs' ], [ 'i', 'A', 'A' ] ) :
-        val = getattr( mappy_alignment, name_attr )
-        if val != '' : # if the current tag contains a valid value
-            l_sam.append( ''.join( [ name_attr, ':', type_val, ':', str( val ) ] ) ) # add a SAM tag
+    for name_attr, type_val in zip(["NM", "MD", "cs"], ["i", "A", "A"]):
+        val = getattr(mappy_alignment, name_attr)
+        if val != "":  # if the current tag contains a valid value
+            l_sam.append(
+                "".join([name_attr, ":", type_val, ":", str(val)])
+            )  # add a SAM tag
     # add transcript strand tag
-    if hasattr( mappy_alignment, 'trans_strand' ) :
-        l_sam.append( 'ts:A:' + { -1 : '-', 0 : '.', 1 : '+' }[ mappy_alignment.trans_strand ] ) # add a SAM tag
-    
-    return pysam.AlignedSegment.fromstring( '\t'.join( map( str, l_sam ) ), samfile_header ) # return pysam AlignedSegment object
+    if hasattr(mappy_alignment, "trans_strand"):
+        l_sam.append(
+            "ts:A:" + {-1: "-", 0: ".", 1: "+"}[mappy_alignment.trans_strand]
+        )  # add a SAM tag
+
+    return pysam.AlignedSegment.fromstring(
+        "\t".join(map(str, l_sam)), samfile_header
+    )  # return pysam AlignedSegment object
+
 
-def Visualize_alignment( r, am = None, seq_ref_aligned = None, flag_display = True ) :
-    ''' # 2022-06-12 16:01:22 
-    'am' : minimap2 index used for alignment 
+def Visualize_alignment(r, am=None, seq_ref_aligned=None, flag_display=True):
+    """# 2022-06-12 16:01:22
+    'am' : minimap2 index used for alignment
     'r' : pysam.AlignedSegment record
     'seq_ref_aligned' : if 'am' is not given, use this sequence as the aligned portion of the reference sequence
     'flag_display' : display the aligned record if True. return two strings, 'str_aligned_seq_ref' and 'str_aligned_seq_query' if False
-    '''
+    """
     # retrieve aligned portion of reference and query sequences
-    if am is not None :
-        seq_ref = am.seq( r.reference_name, r.reference_start, r.reference_end )
-    else :
+    if am is not None:
+        seq_ref = am.seq(r.reference_name, r.reference_start, r.reference_end)
+    else:
         seq_ref = seq_ref_aligned
     seq_query = r.seq
 
     # initialize
-    l_aligned_seq_ref = [ ]
-    l_aligned_seq_query = [ ]
+    l_aligned_seq_ref = []
+    l_aligned_seq_query = []
 
     pos_ref, pos_query = 0, 0
 
-    l_mask_consumes_query = [ True, True, False, False, True, False, False, True, True ]
-    l_mask_consumes_ref = [ True, False, True, True, False, False, False, True, True ]
-    l_flag_record_alignment = [ True, True, True, False, False, False, False, True, True ]
-    l_fill_value = [ '', '-', '-', f'__splicing__', '__soft_clipping__', '', '', '', '' ]
-    for int_cigarop, int_num_bases in r.cigartuples :
-        flag_consumes_query = l_mask_consumes_query[ int_cigarop ]
-        flag_consumes_ref = l_mask_consumes_ref[ int_cigarop ]
-        flag_record_alignment = l_flag_record_alignment[ int_cigarop ]
-        str_fill_value = l_fill_value[ int_cigarop ]
+    l_mask_consumes_query = [True, True, False, False, True, False, False, True, True]
+    l_mask_consumes_ref = [True, False, True, True, False, False, False, True, True]
+    l_flag_record_alignment = [True, True, True, False, False, False, False, True, True]
+    l_fill_value = ["", "-", "-", f"__splicing__", "__soft_clipping__", "", "", "", ""]
+    for int_cigarop, int_num_bases in r.cigartuples:
+        flag_consumes_query = l_mask_consumes_query[int_cigarop]
+        flag_consumes_ref = l_mask_consumes_ref[int_cigarop]
+        flag_record_alignment = l_flag_record_alignment[int_cigarop]
+        str_fill_value = l_fill_value[int_cigarop]
 
         # annotate alignment
-        if flag_record_alignment :
-            if flag_consumes_ref :
-                l_aligned_seq_ref.append( seq_ref[ pos_ref : pos_ref + int_num_bases ] )
-            else :
-                l_aligned_seq_ref.append( str_fill_value * int_num_bases )
-            if flag_consumes_query :
-                l_aligned_seq_query.append( seq_query[ pos_query : pos_query + int_num_bases ] )
-            else :
-                l_aligned_seq_query.append( str_fill_value * int_num_bases )
-        elif len( str_fill_value ) > 0 :
-            l_aligned_seq_ref.append( str_fill_value )
-            l_aligned_seq_query.append( str_fill_value )
+        if flag_record_alignment:
+            if flag_consumes_ref:
+                l_aligned_seq_ref.append(seq_ref[pos_ref : pos_ref + int_num_bases])
+            else:
+                l_aligned_seq_ref.append(str_fill_value * int_num_bases)
+            if flag_consumes_query:
+                l_aligned_seq_query.append(
+                    seq_query[pos_query : pos_query + int_num_bases]
+                )
+            else:
+                l_aligned_seq_query.append(str_fill_value * int_num_bases)
+        elif len(str_fill_value) > 0:
+            l_aligned_seq_ref.append(str_fill_value)
+            l_aligned_seq_query.append(str_fill_value)
 
         # update coordinate
-        if flag_consumes_query :
+        if flag_consumes_query:
             pos_query += int_num_bases
-        if flag_consumes_ref :
+        if flag_consumes_ref:
             pos_ref += int_num_bases
-    
+
     # compose visual representation of the alignment
-    str_aligned_seq_ref = ''.join( l_aligned_seq_ref )
-    str_aligned_seq_query = ''.join( l_aligned_seq_query )
-    
-    if flag_display :
+    str_aligned_seq_ref = "".join(l_aligned_seq_ref)
+    str_aligned_seq_query = "".join(l_aligned_seq_query)
+
+    if flag_display:
         from IPython.display import display, HTML
+
         # display a long text strings with overflow
-        display(HTML("<div style='overflow: scroll; width: 100%; min-width: 1px; font-family:consolas; white-space: nowrap; display: block;'>" +
-                    str_aligned_seq_ref + '<br>' + str_aligned_seq_query +
-                     "</div>"))
-        
-    else :
+        display(
+            HTML(
+                "<div style='overflow: scroll; width: 100%; min-width: 1px; font-family:consolas; white-space: nowrap; display: block;'>"
+                + str_aligned_seq_ref
+                + "<br>"
+                + str_aligned_seq_query
+                + "</div>"
+            )
+        )
+
+    else:
         return str_aligned_seq_ref, str_aligned_seq_query
 
-def Plot_alignment( l_r, figsize = ( 10, 1 ), len_head = 100, verbose = True, min_dx_abs = 1e-2, color = 'random' ) :
-    """ # 2022-06-12 19:06:43 
+
+def Plot_alignment(
+    l_r, figsize=(10, 1), len_head=100, verbose=True, min_dx_abs=1e-2, color="random"
+):
+    """# 2022-06-12 19:06:43
     plot a given list of pysam.AlignedSegment records of a single read aligned against the same reference.
-    
+
     'len_head' : the length of the arrow head
     'min_dx_abs' : the min absolute length of arrow stem
     """
-    qname = l_r[ 0 ].qname
-    fig, ax = plt.subplots( 1, 2, figsize = figsize )
-    for i, r in enumerate( l_r ) :
-        # retrieve a random color 
-        c = Get_random_hex_color( ) if color == 'random' else color
-        
+    qname = l_r[0].qname
+    fig, ax = plt.subplots(1, 2, figsize=figsize)
+    for i, r in enumerate(l_r):
+        # retrieve a random color
+        c = Get_random_hex_color() if color == "random" else color
+
         # draw an alignment on the reference
         y = i
-        ax[ 0 ].arrow( x = r.query_alignment_start if not r.is_reverse > 0 else len( r.seq ) - r.query_alignment_end, y = y, dx = max( r.query_alignment_end - r.query_alignment_start, min_dx_abs ), dy = 0, head_width = 1, head_length = len_head, fc = c, ec = 'k', length_includes_head = True ) # direction of the arrow on the query is always + direction!
-        
+        ax[0].arrow(
+            x=r.query_alignment_start
+            if not r.is_reverse > 0
+            else len(r.seq) - r.query_alignment_end,
+            y=y,
+            dx=max(r.query_alignment_end - r.query_alignment_start, min_dx_abs),
+            dy=0,
+            head_width=1,
+            head_length=len_head,
+            fc=c,
+            ec="k",
+            length_includes_head=True,
+        )  # direction of the arrow on the query is always + direction!
+
         # draw an alignment on the reference
-        
-        for ref_start, ref_end in Retrive_List_of_Mapped_Segments( r.cigartuples, r.reference_start )[ 0 ] :
+
+        for ref_start, ref_end in Retrive_List_of_Mapped_Segments(
+            r.cigartuples, r.reference_start
+        )[0]:
             dx_ref = ref_end - ref_start if not r.is_reverse else ref_start - ref_end
-            if dx_ref == 0 :
-                dx_ref = min_dx_abs if r.is_reverse else - min_dx_abs
-            ax[ 1 ].arrow( x = ref_start if not r.is_reverse else ref_end, y = y, dx = dx_ref, dy = 0, head_width = 1, head_length = len_head, fc = c, ec = 'k', length_includes_head = True )
-        if verbose :
-            print( r.flag, qname, r.mapq, r.query_alignment_start, r.query_alignment_end, r.reference_start, r.reference_end, r.is_reverse, Retrive_List_of_Mapped_Segments( r.cigar, r.reference_start, flag_is_cigartuples_from_mappy = False ) )
-    ax[ 0 ].set_title( f'query aligned regions for\n{qname}' )
-    ax[ 1 ].set_title( f'reference aligned regions for\n{qname}' )
-    
+            if dx_ref == 0:
+                dx_ref = min_dx_abs if r.is_reverse else -min_dx_abs
+            ax[1].arrow(
+                x=ref_start if not r.is_reverse else ref_end,
+                y=y,
+                dx=dx_ref,
+                dy=0,
+                head_width=1,
+                head_length=len_head,
+                fc=c,
+                ec="k",
+                length_includes_head=True,
+            )
+        if verbose:
+            print(
+                r.flag,
+                qname,
+                r.mapq,
+                r.query_alignment_start,
+                r.query_alignment_end,
+                r.reference_start,
+                r.reference_end,
+                r.is_reverse,
+                Retrive_List_of_Mapped_Segments(
+                    r.cigar, r.reference_start, flag_is_cigartuples_from_mappy=False
+                ),
+            )
+    ax[0].set_title(f"query aligned regions for\n{qname}")
+    ax[1].set_title(f"reference aligned regions for\n{qname}")
```

### Comparing `biobookshelf-0.2.2/biobookshelf/SC/single_cell.py` & `biobookshelf-0.2.3/biobookshelf/SC/single_cell.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1381 +1,2690 @@
 from biobookshelf.main import *
 from biobookshelf import MAP
+
 pd.options.mode.chained_assignment = None  # default='warn' # to disable worining
 import scanpy
 
-''' previosuly written for biobookshelf '''
-def CB_Parse_list_of_id_cell( l_id_cell, dropna = True ) :
-    ''' # 2022-03-25 16:35:23 
+from typing import Union, List, Literal, Dict, Callable, Set, Iterable, Tuple
+import os
+import pandas as pd
+import numpy as np
+import multiprocessing as mp
+import math
+import logging
+from copy import deepcopy
+import pickle
+import time
+import glob
+import gzip  # to handle gzip file
+import shutil  # for copying file
+import base64  # for converting binary to text data (web application)
+import json  # to read and write JSON file
+import matplotlib.pyplot as plt
+import scipy.sparse
+import io
+import concurrent.futures  # for multiprocessing
+
+""" previosuly written for biobookshelf """
+
+
+def CB_Parse_list_of_id_cell(l_id_cell, dropna=True):
+    """# 2022-03-25 16:35:23
     parse a given list of id_cells into a dataframe using 'SC.CB_detect_cell_barcode_from_id_cell' function
-    'dropna' : drop id_cells that does not contains cell barcodes 
-    '''
-    df = pd.DataFrame( list( [ e ] + list( CB_detect_cell_barcode_from_id_cell( e ) ) for e in l_id_cell ), columns = [ 'id_cell', 'CB', 'id_sample_from_id_cell' ] ).set_index( 'id_cell' )
+    'dropna' : drop id_cells that does not contains cell barcodes
+    """
+    df = pd.DataFrame(
+        list([e] + list(CB_detect_cell_barcode_from_id_cell(e)) for e in l_id_cell),
+        columns=["id_cell", "CB", "id_sample_from_id_cell"],
+    ).set_index("id_cell")
     return df
-def CB_Build_dict_id_sample_to_set_cb( l_id_cell ) :
-    ''' # 2022-03-28 22:24:30 
-    Build a set of cell barcode for each id_sample from the given list of id_cells 
-    '''
-    df = CB_Parse_list_of_id_cell( l_id_cell )
-    dict_id_sample_to_set_cb = dict( )
-    for cb, id_sample in df.values :
-        if id_sample not in dict_id_sample_to_set_cb :
-            dict_id_sample_to_set_cb[ id_sample ] = set( )
-        dict_id_sample_to_set_cb[ id_sample ].add( cb )
+
+
+def CB_Build_dict_id_sample_to_set_cb(l_id_cell):
+    """# 2022-03-28 22:24:30
+    Build a set of cell barcode for each id_sample from the given list of id_cells
+    """
+    df = CB_Parse_list_of_id_cell(l_id_cell)
+    dict_id_sample_to_set_cb = dict()
+    for cb, id_sample in df.values:
+        if id_sample not in dict_id_sample_to_set_cb:
+            dict_id_sample_to_set_cb[id_sample] = set()
+        dict_id_sample_to_set_cb[id_sample].add(cb)
     return dict_id_sample_to_set_cb
-def CB_Match_Batch( l_id_cell_1, l_id_cell_2, flag_calculate_proportion_using_l_id_cell_2 = True ) :
-    ''' # 2022-03-28 23:10:43 
+
+
+def CB_Match_Batch(
+    l_id_cell_1, l_id_cell_2, flag_calculate_proportion_using_l_id_cell_2=True
+):
+    """# 2022-03-28 23:10:43
     Find matching batches between two given lists of id_cells by finding the batches sharing the largest number of cell barcodes
-    
-    'l_id_cell_1' : first list of id_cells 
-    'l_id_cell_2' : second list of id_cells
+
+    'l_id_cell_1' : first list of id_cells (e.g. unannotated barcodes)
+    'l_id_cell_2' : second list of id_cells (e.g. annotated barcodes)
     'flag_calculate_proportion_using_l_id_cell_2' : if True, finding matching batches using the shared proportion calculated using the cell barcodes from 'l_id_cell_2'. if False, proportion of the matching barcodes will be calculated using the cell barcodes from 'l_id_cell_1'
-    
+
     return:
     df_id_cell_matched, df_sample_matched
-    '''
-    # retrieve set of cell barcodes 
-    df_id_cell_1 = CB_Parse_list_of_id_cell( l_id_cell_1 )
-    df_id_cell_2 = CB_Parse_list_of_id_cell( l_id_cell_2 )
-    dict_id_sample_to_set_cb_1 = CB_Build_dict_id_sample_to_set_cb( l_id_cell_1 )
-    dict_id_sample_to_set_cb_2 = CB_Build_dict_id_sample_to_set_cb( l_id_cell_2 )
+    """
+    # retrieve set of cell barcodes
+    df_id_cell_1 = CB_Parse_list_of_id_cell(l_id_cell_1)
+    df_id_cell_2 = CB_Parse_list_of_id_cell(l_id_cell_2)
+    dict_id_sample_to_set_cb_1 = CB_Build_dict_id_sample_to_set_cb(l_id_cell_1)
+    dict_id_sample_to_set_cb_2 = CB_Build_dict_id_sample_to_set_cb(l_id_cell_2)
 
     # Find matching id_samples of the two given list of id_cells
     # calculate the proportion of matching cell barcodes between each pair of samples from the two given list of id_cells
-    l_l = [ ]
-    for id_sample_1 in dict_id_sample_to_set_cb_1 :
-        for id_sample_2 in dict_id_sample_to_set_cb_2 :
-            set_cb_1 = dict_id_sample_to_set_cb_1[ id_sample_1 ]
-            set_cb_2 = dict_id_sample_to_set_cb_2[ id_sample_2 ]
-            float_prop_matching_cb = len( set_cb_1.intersection( set_cb_2 ) ) / ( len( set_cb_2 ) if flag_calculate_proportion_using_l_id_cell_2 else len( set_cb_1 ) )
-            l_l.append( [ id_sample_1, id_sample_2, float_prop_matching_cb ] )
-    df = pd.DataFrame( l_l, columns = [ 'id_sample_1', 'id_sample_2', 'float_prop_matching_cb' ] ) # search result
-    df_sample_matched = df.sort_values( 'float_prop_matching_cb', ascending = False ).drop_duplicates( 'id_sample_2', keep = 'first' ).drop_duplicates( 'id_sample_1', keep = 'first' ) # retrieve the best matches between samples so that a unique mapping exists for every sample
+    l_l = []
+    for id_sample_1 in dict_id_sample_to_set_cb_1:
+        for id_sample_2 in dict_id_sample_to_set_cb_2:
+            set_cb_1 = dict_id_sample_to_set_cb_1[id_sample_1]
+            set_cb_2 = dict_id_sample_to_set_cb_2[id_sample_2]
+            float_prop_matching_cb = len(set_cb_1.intersection(set_cb_2)) / (
+                len(set_cb_2)
+                if flag_calculate_proportion_using_l_id_cell_2
+                else len(set_cb_1)
+            )
+            l_l.append([id_sample_1, id_sample_2, float_prop_matching_cb])
+    df = pd.DataFrame(
+        l_l, columns=["id_sample_1", "id_sample_2", "float_prop_matching_cb"]
+    )  # search result
+    df_sample_matched = (
+        df.sort_values("float_prop_matching_cb", ascending=False)
+        .drop_duplicates("id_sample_2", keep="first")
+        .drop_duplicates("id_sample_1", keep="first")
+    )  # retrieve the best matches between samples so that a unique mapping exists for every sample
 
     # Find matching id_cells of given two list of id_cells
-    df_id_cell_1.reset_index( inplace = True, drop = False )
-    df_id_cell_2.reset_index( inplace = True, drop = False )
-    df_id_cell_1.rename( columns = { 'id_sample_from_id_cell' : 'id_sample_from_id_cell_1' }, inplace = True )
-    df_id_cell_2.rename( columns = { 'id_sample_from_id_cell' : 'id_sample_from_id_cell_2' }, inplace = True )
-    df_id_cell_1[ 'id_sample_from_id_cell_2' ] = df_id_cell_1.id_sample_from_id_cell_1.apply( MAP.Map( df_sample_matched.set_index( 'id_sample_1' ).id_sample_2.to_dict( ) ).a2b )
-    df_id_cell_1.dropna( subset = [ 'id_sample_from_id_cell_2' ], inplace = True ) # ignore cells without matching id_sample from the '2' batch
-    df_id_cell_1.set_index( [ 'CB', 'id_sample_from_id_cell_2' ], inplace = True )
-    df_id_cell_matched = df_id_cell_1.join( df_id_cell_2[ ~ pd.isnull( df_id_cell_2.id_sample_from_id_cell_2 ) ].set_index( [ 'CB', 'id_sample_from_id_cell_2' ] ), lsuffix = '_1', rsuffix = '_2' ) # match id_cells from two given list of id_cells
-    df_id_cell_matched.reset_index( drop = False, inplace = True )
-    df_id_cell_matched = df_id_cell_matched[ [ 'id_cell_1', 'id_cell_2', 'CB', 'id_sample_from_id_cell_1', 'id_sample_from_id_cell_2' ] ] # reorder columns
-    
+    df_id_cell_1.reset_index(inplace=True, drop=False)
+    df_id_cell_2.reset_index(inplace=True, drop=False)
+    df_id_cell_1.rename(
+        columns={"id_sample_from_id_cell": "id_sample_from_id_cell_1"}, inplace=True
+    )
+    df_id_cell_2.rename(
+        columns={"id_sample_from_id_cell": "id_sample_from_id_cell_2"}, inplace=True
+    )
+    df_id_cell_1[
+        "id_sample_from_id_cell_2"
+    ] = df_id_cell_1.id_sample_from_id_cell_1.apply(
+        bk.Map(df_sample_matched.set_index("id_sample_1").id_sample_2.to_dict()).a2b
+    )
+    df_id_cell_1.dropna(
+        subset=["id_sample_from_id_cell_2"], inplace=True
+    )  # ignore cells without matching id_sample from the '2' batch
+    df_id_cell_1.set_index(["CB", "id_sample_from_id_cell_2"], inplace=True)
+    df_id_cell_matched = df_id_cell_1.join(
+        df_id_cell_2[~pd.isnull(df_id_cell_2.id_sample_from_id_cell_2)].set_index(
+            ["CB", "id_sample_from_id_cell_2"]
+        ),
+        lsuffix="_1",
+        rsuffix="_2",
+    )  # match id_cells from two given list of id_cells
+    df_id_cell_matched.reset_index(drop=False, inplace=True)
+    df_id_cell_matched = df_id_cell_matched[
+        [
+            "id_cell_1",
+            "id_cell_2",
+            "CB",
+            "id_sample_from_id_cell_1",
+            "id_sample_from_id_cell_2",
+        ]
+    ]  # reorder columns
+
     return df_id_cell_matched, df_sample_matched
-def SCANPY_Detect_cell_barcode_from_cell_id( adata ) :
-    ''' # 2022-03-24 20:35:22 
+
+
+def SCANPY_Detect_cell_barcode_from_cell_id(adata):
+    """# 2022-03-24 20:35:22
     Detect cell barcodes from id_cell (index of adata.obs), and add new two columns to the adata.obs [ 'CB', 'id_sample_from_id_cell' ]
-    '''
-    adata.obs = adata.obs.join( pd.DataFrame( list( [ e ] + list( CB_detect_cell_barcode_from_id_cell( e ) ) for e in adata.obs.index.values ), columns = [ 'id_cell', 'CB', 'id_sample_from_id_cell' ] ).set_index( 'id_cell' ) )
-def SCANPY_Retrieve_Markers_as_DataFrame( adata ) :
-    ''' # 2022-02-15 14:40:02 
-    receive scanpy anndata and return a dataframe contianing marker genes 
-    
-    --- return --- 
-    df_marker : a dataframe contianing marker genes 
-    '''
-    l_df = [ ]
-    for index_clus, name_clus in enumerate( adata.uns["rank_genes_groups"]['names'].dtype.names ) : 
-        df = pd.DataFrame( dict( ( name_col, adata.uns["rank_genes_groups"][ name_col ][ name_clus ] ) for name_col in ['logfoldchanges', 'names', 'pvals', 'pvals_adj', 'scores' ] ) )
-        df[ "name_clus" ] = name_clus 
-        df[ "index_clus" ] = index_clus
-        l_df.append( df )
-    df_marker = pd.concat( l_df )
+    """
+    adata.obs = adata.obs.join(
+        pd.DataFrame(
+            list(
+                [e] + list(CB_detect_cell_barcode_from_id_cell(e))
+                for e in adata.obs.index.values
+            ),
+            columns=["id_cell", "CB", "id_sample_from_id_cell"],
+        ).set_index("id_cell")
+    )
+
+
+def SCANPY_Retrieve_Markers_as_DataFrame(adata):
+    """# 2022-02-15 14:40:02
+    receive scanpy anndata and return a dataframe contianing marker genes
+
+    --- return ---
+    df_marker : a dataframe contianing marker genes
+    """
+    l_df = []
+    for index_clus, name_clus in enumerate(
+        adata.uns["rank_genes_groups"]["names"].dtype.names
+    ):
+        df = pd.DataFrame(
+            dict(
+                (name_col, adata.uns["rank_genes_groups"][name_col][name_clus])
+                for name_col in [
+                    "logfoldchanges",
+                    "names",
+                    "pvals",
+                    "pvals_adj",
+                    "scores",
+                ]
+            )
+        )
+        df["name_clus"] = name_clus
+        df["index_clus"] = index_clus
+        l_df.append(df)
+    df_marker = pd.concat(l_df)
     return df_marker
-def CB_detect_cell_barcode_from_id_cell( id_cell, int_number_atgc_in_cell_barcode = 16 ) :
-    ''' # 2022-02-21 00:03:34 
-    retrieve cell_barcode from id_cell 
-    'int_number_atgc_in_cell_barcode' : number of ATGC characters in the cell barcode
-    '''
+
+
+def CB_detect_cell_barcode_from_id_cell(
+    id_cell, int_min_number_atgc_in_cell_barcode=16
+):
+    """# 2023-04-02 14:10:46
+    retrieve cell_barcode from id_cell
+    'int_min_number_atgc_in_cell_barcode' : number of ATGC characters in the cell barcode
+    """
     int_count_atgc = 0
     int_start_appearance_of_atgc = None
-    set_atgc = set( "ATGC" )
-    
-    def __retrieve_cell_barcode_and_id_channel_from_id_cell__( id_cell, int_start_appearance_of_atgc, int_number_atgc_in_cell_barcode ) :
-        ''' __retrieve_cell_barcode_and_id_channel_from_id_cell__ '''
+    set_atgc = set("ATGC")
+
+    def __retrieve_cell_barcode_and_id_channel_from_id_cell__(
+        id_cell, int_start_appearance_of_atgc, int_count_atgc
+    ):
+        """__retrieve_cell_barcode_and_id_channel_from_id_cell__"""
         int_cb_start = int_start_appearance_of_atgc
-        int_cb_end = int_start_appearance_of_atgc + int_number_atgc_in_cell_barcode
-        return [ id_cell[ int_cb_start : int_cb_end ], id_cell[ : int_cb_start ] + '|' + id_cell[ int_cb_end : ] ] # return cell_barcode, id_channel
-        
-    for index_c, c in enumerate( id_cell.upper( ) ) : # case-insensitive detection of cell-barcodes
-        if c in set_atgc :
+        int_cb_end = int_start_appearance_of_atgc + int_count_atgc
+        return [
+            id_cell[int_cb_start:int_cb_end],
+            id_cell[:int_cb_start] + "|" + id_cell[int_cb_end:],
+        ]  # return cell_barcode, id_channel
+
+    for index_c, c in enumerate(
+        id_cell.upper()
+    ):  # case-insensitive detection of cell-barcodes
+        if c in set_atgc:
             if int_start_appearance_of_atgc is None:
                 int_start_appearance_of_atgc = index_c
             int_count_atgc += 1
-        else :
-            ''' identify cell barcode and return the cell barcode '''
+        else:
+            """identify cell barcode and return the cell barcode"""
             if int_start_appearance_of_atgc is not None:
-                if int_count_atgc == int_number_atgc_in_cell_barcode :
-                    return __retrieve_cell_barcode_and_id_channel_from_id_cell__( id_cell, int_start_appearance_of_atgc, int_number_atgc_in_cell_barcode )
+                if int_count_atgc >= int_min_number_atgc_in_cell_barcode:
+                    return __retrieve_cell_barcode_and_id_channel_from_id_cell__(
+                        id_cell, int_start_appearance_of_atgc, int_count_atgc
+                    )
             # initialize the next search
-            int_count_atgc = 0 
+            int_count_atgc = 0
             int_start_appearance_of_atgc = None
-    ''' identify cell barcode and return the cell barcode '''
+    """ identify cell barcode and return the cell barcode """
     if int_start_appearance_of_atgc is not None:
-        if int_count_atgc == int_number_atgc_in_cell_barcode :
-            return __retrieve_cell_barcode_and_id_channel_from_id_cell__( id_cell, int_start_appearance_of_atgc, int_number_atgc_in_cell_barcode )
-    ''' return None when cell_barcode was not found '''
-    return [ None, None ]
+        if int_count_atgc >= int_min_number_atgc_in_cell_barcode:
+            return __retrieve_cell_barcode_and_id_channel_from_id_cell__(
+                id_cell, int_start_appearance_of_atgc, int_count_atgc
+            )
+    """ return None when cell_barcode was not found """
+    return [None, None]
+
 
-def Read_10X( path_folder_mtx_10x, verbose = False ) :
-    ''' # 2021-11-24 13:00:13 
+def Read_10X(path_folder_mtx_10x, verbose=False):
+    """# 2021-11-24 13:00:13
     read 10x count matrix
     'path_folder_mtx_10x' : a folder containing files for 10x count matrix
     return df_mtx, df_feature
-    '''
+    """
     # handle inputs
-    if path_folder_mtx_10x[ -1 ] != '/' :
-        path_folder_mtx_10x += '/'
-    
+    if path_folder_mtx_10x[-1] != "/":
+        path_folder_mtx_10x += "/"
+
     # define input file directories
-    path_file_bc = f'{path_folder_mtx_10x}barcodes.tsv.gz'
-    path_file_feature = f'{path_folder_mtx_10x}features.tsv.gz'
-    path_file_mtx = f'{path_folder_mtx_10x}matrix.mtx.gz'
+    path_file_bc = f"{path_folder_mtx_10x}barcodes.tsv.gz"
+    path_file_feature = f"{path_folder_mtx_10x}features.tsv.gz"
+    path_file_mtx = f"{path_folder_mtx_10x}matrix.mtx.gz"
 
     # check whether all required files are present
-    if sum( list( not os.path.exists( path_folder ) for path_folder in [ path_file_bc, path_file_feature, path_file_mtx ] ) ) :
-        if verbose :
-            print( f'required file(s) is not present at {path_folder_mtx_10x}' )
+    if sum(
+        list(
+            not filesystem_operations("exists", path_folder)
+            for path_folder in [path_file_bc, path_file_feature, path_file_mtx]
+        )
+    ):
+        if verbose:
+            logger.info(f"required file(s) is not present at {path_folder_mtx_10x}")
 
     # read mtx file as a tabular format
-    df_mtx = pd.read_csv( path_file_mtx, sep = ' ', comment = '%' )
-    df_mtx.columns = [ 'id_row', 'id_column', 'read_count' ]
+    df_mtx = pd.read_csv(path_file_mtx, sep=" ", comment="%")
+    df_mtx.columns = ["id_row", "id_column", "read_count"]
 
     # read barcode and feature information
-    df_bc = pd.read_csv( path_file_bc, sep = '\t', header = None )
-    df_bc.columns = [ 'barcode' ]
-    df_feature = pd.read_csv( path_file_feature, sep = '\t', header = None )
-    df_feature.columns = [ 'id_feature', 'feature', 'feature_type' ]
+    df_bc = pd.read_csv(path_file_bc, sep="\t", header=None)
+    df_bc.columns = ["barcode"]
+    df_feature = pd.read_csv(path_file_feature, sep="\t", header=None)
+    df_feature.columns = ["id_feature", "feature", "feature_type"]
 
     # mapping using 1 based coordinates (0->1 based coordinate )
-    df_mtx[ 'barcode' ] = df_mtx.id_column.apply( MAP.Map( DICTIONARY_Build_from_arr( df_bc.barcode.values, index_start = 1 ) ).a2b ) # mapping using 1 based coordinates (0->1 based coordinate )
-    df_mtx[ 'id_feature' ] = df_mtx.id_row.apply( MAP.Map( DICTIONARY_Build_from_arr( df_feature.id_feature.values, index_start = 1 ) ).a2b ) 
-    df_mtx.drop( columns = [ 'id_row', 'id_column' ], inplace = True ) # drop unnecessary columns
-    
+    df_mtx["barcode"] = df_mtx.id_column.apply(
+        bk.Map(bk.DICTIONARY_Build_from_arr(df_bc.barcode.values, index_start=1)).a2b
+    )  # mapping using 1 based coordinates (0->1 based coordinate )
+    df_mtx["id_feature"] = df_mtx.id_row.apply(
+        bk.Map(
+            bk.DICTIONARY_Build_from_arr(df_feature.id_feature.values, index_start=1)
+        ).a2b
+    )
+    df_mtx.drop(
+        columns=["id_row", "id_column"], inplace=True
+    )  # drop unnecessary columns
+
     return df_mtx, df_feature
-def Write_10X( df_mtx, df_feature, path_folder_output_mtx_10x ) :
-    """ # 2021-11-24 12:57:30 
+
+
+def Write_10X(df_mtx, df_feature, path_folder_output_mtx_10x):
+    """# 2021-11-24 12:57:30
     'df_feature' should contains the following column names : [ 'id_feature', 'feature', 'feature_type' ]
     'df_mtx' should contains the following column names : [ 'id_feature', 'barcode', 'read_count' ]
     'path_folder_output_mtx_10x' : an output folder directory where the mtx_10x files will be written
 
     """
-    df_mtx = deepcopy( df_mtx ) # create a copy of df_mtx before modification
+    import scipy.io
+
+    df_mtx = deepcopy(df_mtx)  # create a copy of df_mtx before modification
 
     # create an output folder
-    os.makedirs( path_folder_output_mtx_10x, exist_ok = True )
+    filesystem_operations("mkdir", path_folder_output_mtx_10x, exist_ok=True)
 
-    ''' save barcode file '''
+    """ save barcode file """
     # retrieve list of barcodes
-    arr_barcode = LIST_COUNT( df_mtx.barcode, duplicate_filter = None ).index.values
-    pd.DataFrame( arr_barcode ).to_csv( f"{path_folder_output_mtx_10x}barcodes.tsv.gz", sep = '\t', index = False, header = False ) 
+    arr_barcode = bk.LIST_COUNT(df_mtx.barcode, duplicate_filter=None).index.values
+    pd.DataFrame(arr_barcode).to_csv(
+        f"{path_folder_output_mtx_10x}barcodes.tsv.gz",
+        sep="\t",
+        index=False,
+        header=False,
+    )
 
-    ''' save feature file '''
+    """ save feature file """
     # compose a feature dataframe
-    df_feature[ [ 'id_feature', 'feature', 'feature_type' ] ].to_csv( f"{path_folder_output_mtx_10x}features.tsv.gz", sep = '\t', index = False, header = False ) # save as a file
+    df_feature[["id_feature", "feature", "feature_type"]].to_csv(
+        f"{path_folder_output_mtx_10x}features.tsv.gz",
+        sep="\t",
+        index=False,
+        header=False,
+    )  # save as a file
     # retrieve list of features
     arr_id_feature = df_feature.id_feature.values
 
-    ''' save matrix file '''
+    """ save matrix file """
     # convert feature and barcode to integer indices
-    df_mtx.id_feature = df_mtx.id_feature.apply( MAP.Map( DICTIONARY_Build_from_arr( arr_id_feature, order_index_entry = False ) ).a2b ) # 0-based coordinates
-    df_mtx.barcode = df_mtx.barcode.apply( MAP.Map( DICTIONARY_Build_from_arr( arr_barcode, order_index_entry = False ) ).a2b ) # 0-based coordinates
+    df_mtx.id_feature = df_mtx.id_feature.apply(
+        bk.Map(
+            bk.DICTIONARY_Build_from_arr(arr_id_feature, order_index_entry=False)
+        ).a2b
+    )  # 0-based coordinates
+    df_mtx.barcode = df_mtx.barcode.apply(
+        bk.Map(bk.DICTIONARY_Build_from_arr(arr_barcode, order_index_entry=False)).a2b
+    )  # 0-based coordinates
     # save count matrix as a gzipped matrix market format
-    row, col, data = df_mtx[ [ 'id_feature', 'barcode', 'read_count' ] ].values.T
-    sm = scipy.sparse.coo_matrix( ( data, ( row, col ) ), shape = ( len( arr_id_feature ), len( arr_barcode ) ) )
-    scipy.io.mmwrite( f"{path_folder_output_mtx_10x}matrix", sm )
+    row, col, data = df_mtx[["id_feature", "barcode", "read_count"]].values.T
+    sm = scipy.sparse.coo_matrix(
+        (data, (row, col)), shape=(len(arr_id_feature), len(arr_barcode))
+    )
+    scipy.io.mmwrite(f"{path_folder_output_mtx_10x}matrix", sm)
     # remove previous output file to overwrite the file
     path_file_mtx_output = f"{path_folder_output_mtx_10x}matrix.mtx.gz"
-    if os.path.exists( path_file_mtx_output ) :
-        os.remove( path_file_mtx_output )
-    OS_Run( [ 'gzip', f"{path_folder_output_mtx_10x}matrix.mtx" ] ) # gzip the mtx file
-def __function_for_adjusting_thresholds_for_filtering_empty_droplets__( path_folder_mtx_10x_output, min_counts, min_features, min_cells ) :
-    ''' # 2022-02-23 14:26:07 
+    if filesystem_operations("exists", path_file_mtx_output):
+        filesystem_operations("rm", path_file_mtx_output)
+    bk.OS_Run(["gzip", f"{path_folder_output_mtx_10x}matrix.mtx"])  # gzip the mtx file
+
+
+def AnnData_Convert_to_10X_MTX(
+    adata,
+    path_folder_mtx_output,
+    dict_var_rename: dict = {"feature_types": "feature_type", "gene_ids": "id_feature"},
+    dtype_value=np.int64,
+):
+    """# 2022-12-14 02:14:31
+    write AnnData count matrix as a 10X matrix object
+
+    'dict_var_rename' : a dictionary for renaming columns of adata.var columns
+    """
+    import scipy.io
+
+    # compose df_var
+    df_feature = adata.var
+    df_feature.rename(columns=dict_var_rename, inplace=True)
+
+    # create an output folder
+    filesystem_operations("mkdir", path_folder_mtx_output, exist_ok=True)
+
+    """ save barcode file """
+    # retrieve list of barcodes
+    arr_barcode = adata.obs.index.values
+    pd.DataFrame(arr_barcode).to_csv(
+        f"{path_folder_mtx_output}barcodes.tsv.gz", sep="\t", index=False, header=False
+    )
+
+    """ save feature file """
+    # compose a feature dataframe
+    df_feature[["id_feature", "feature", "feature_type"]].to_csv(
+        f"{path_folder_mtx_output}features.tsv.gz", sep="\t", index=False, header=False
+    )  # save as a file
+    # retrieve list of features
+    arr_id_feature = df_feature.id_feature.values
+
+    """ save matrix file """
+    # save count matrix as a gzipped matrix market format
+    arr_int_barcode, arr_int_id_feature, arr_read_count = scipy.sparse.find(adata.X)
+    # convert dtype of the values
+    if dtype_value is not None:
+        arr_read_count = arr_read_count.astype(dtype_value)
+    # compose a sparse matrix
+    sm = scipy.sparse.coo_matrix(
+        (arr_read_count, (arr_int_id_feature, arr_int_barcode)),
+        shape=(len(arr_id_feature), len(arr_barcode)),
+    )
+    scipy.io.mmwrite(f"{path_folder_mtx_output}matrix", sm)
+    # remove previous output file to overwrite the file
+    path_file_mtx_output = f"{path_folder_mtx_output}matrix.mtx.gz"
+    if filesystem_operations("exists", path_file_mtx_output):
+        filesystem_operations("rm", path_file_mtx_output)
+    bk.OS_Run(["gzip", f"{path_folder_mtx_output}matrix.mtx"])  # gzip the mtx file
+
+
+def __function_for_adjusting_thresholds_for_filtering_empty_droplets__(
+    path_folder_mtx_10x_output, min_counts, min_features, min_cells
+):
+    """# 2022-02-23 14:26:07
     This function is intended for the use in 'MTX_10X_Filter' function for filtering cells from the 10X dataset (before chromium X, 10,000 cells per channel)
-    
-    Assuming a typical number of droplets in a experiment is 100,000, adjust 'min_counts' to reduce the number of filtered cells below 'int_max_num_cells' 
-    '''
-    s_count = pd.read_csv( f"{path_folder_mtx_10x_output}dict_id_column_to_count.before_filtering.tsv.gz", sep = '\t', header = None, index_col = 0 )[ 1 ].sort_values( ascending = False ).iloc[ : 100000 ]
-    
-    int_max_num_cells = 20000 # maximum number of allowed cells
+
+    Assuming a typical number of droplets in a experiment is 100,000, adjust 'min_counts' to reduce the number of filtered cells below 'int_max_num_cells'
+    """
+    s_count = (
+        pd.read_csv(
+            f"{path_folder_mtx_10x_output}dict_id_column_to_count.before_filtering.tsv.gz",
+            sep="\t",
+            header=None,
+            index_col=0,
+        )[1]
+        .sort_values(ascending=False)
+        .iloc[:100000]
+    )
+
+    int_max_num_cells = 20000  # maximum number of allowed cells
     min_counts_maximum = 2000
-    def function_for_increasing_min_counts( min_counts ) :
+
+    def function_for_increasing_min_counts(min_counts):
         return min_counts * 2
-    while True :
-        ''' increase threshold if the number of filtered cells is larger than 'int_max_num_cells' '''
-        if len( s_count[ s_count > min_counts ] ) > int_max_num_cells and min_counts < min_counts_maximum :
-            min_counts = function_for_increasing_min_counts( min_counts )
-        else :
+
+    while True:
+        """increase threshold if the number of filtered cells is larger than 'int_max_num_cells'"""
+        if (
+            len(s_count[s_count > min_counts]) > int_max_num_cells
+            and min_counts < min_counts_maximum
+        ):
+            min_counts = function_for_increasing_min_counts(min_counts)
+        else:
             break
     return min_counts, min_features, min_cells
-def MTX_10X_Split( path_folder_mtx_10x_output, int_max_num_entries_for_chunk = 10000000, flag_split_mtx = True, flag_split_mtx_again = False ) :
-    ''' # 2022-04-28 01:16:35 
-    split input mtx file into multiple files and write a flag file indicating the splitting has been completed. 
+
+
+def MTX_10X_Split(
+    path_folder_mtx_10x_output,
+    int_max_num_entries_for_chunk=10000000,
+    flag_split_mtx=True,
+    flag_split_mtx_again=False,
+):
+    """# 2022-04-28 01:16:35
+    split input mtx file into multiple files and write a flag file indicating the splitting has been completed.
     return the list of split mtx files
-    
+
     'flag_split_mtx' : if 'flag_split_mtx' is True, split input mtx file into multiple files. if False, does not split the input matrix, and just return the list containing a single path pointing to the input matrix. This flag exists for the compatibility with single-thread operations
     'flag_split_mtx_again' : split the input matrix again even if it has beem already split. It will remove previously split files.
-    '''
+    """
     # 'flag_split_mtx' : if False, does not split the input matrix, and just return the list containing a single path pointing to the input matrix
-    if not flag_split_mtx :
-        return [ f"{path_folder_mtx_10x_output}matrix.mtx.gz" ]
-    
-    ''' if 'flag_split_mtx_again' flag is True, remove previously split files '''
+    if not flag_split_mtx:
+        return [f"{path_folder_mtx_10x_output}matrix.mtx.gz"]
+
+    """ if 'flag_split_mtx_again' flag is True, remove previously split files """
     path_file_flag = f"{path_folder_mtx_10x_output}matrix.mtx.gz.split.flag"
-    if flag_split_mtx_again :
-        os.remove( path_file_flag ) # remove the flag
+    if flag_split_mtx_again:
+        filesystem_operations("rm", path_file_flag)  # remove the flag
         # remove previously split files
-        for path_file in glob.glob( f'{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz' ) :
-            os.remove( path_file )
-
-    ''' split input matrix file '''
-    if not os.path.exists( path_file_flag ) : # check whether the flag exists
+        for path_file in filesystem_operations(
+            "glob", f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz"
+        ):
+            filesystem_operations("rm", path_file)
+
+    """ split input matrix file """
+    if not filesystem_operations(
+        "exists", path_file_flag
+    ):  # check whether the flag exists
         index_mtx_10x = 0
-        newfile = gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", 'wb' )
-        l_path_file_mtx_10x = [ f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz" ]
+        newfile = gzip.open(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", "wb"
+        )
+        l_path_file_mtx_10x = [
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz"
+        ]
         int_num_entries_written_for_the_current_chunk = 0
-        with gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz", 'rb' ) as file :
-            while True :
-                line = file.readline( ) # binary string
-                if len( line ) == 0 :
-                    newfile.close( ) # close the output file
+        with gzip.open(f"{path_folder_mtx_10x_output}matrix.mtx.gz", "rb") as file:
+            while True:
+                line = file.readline()  # binary string
+                if len(line) == 0:
+                    newfile.close()  # close the output file
                     break
-                ''' write the line to the current chunk and update the number of entries written for the current chunk '''
-                newfile.write( line )
+                """ write the line to the current chunk and update the number of entries written for the current chunk """
+                newfile.write(line)
                 int_num_entries_written_for_the_current_chunk += 1
-                ''' initialize the next chunk if a sufficient number of entries were written '''
-                if int_num_entries_written_for_the_current_chunk >= int_max_num_entries_for_chunk :
-                    newfile.close( ) # close the output file
+                """ initialize the next chunk if a sufficient number of entries were written """
+                if (
+                    int_num_entries_written_for_the_current_chunk
+                    >= int_max_num_entries_for_chunk
+                ):
+                    newfile.close()  # close the output file
                     # initialize the next chunk
                     index_mtx_10x += 1
                     int_num_entries_written_for_the_current_chunk = 0
-                    newfile = gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", 'wb' )
-                    l_path_file_mtx_10x.append( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz" )
-        with open( path_file_flag, 'w' ) as file :
-            file.write( 'completed' )
-    else :
-        ''' retrieve the list of split mtx files '''
-        df = GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz" )
-        df.wildcard_0 = df.wildcard_0.astype( int )
-        df.sort_values( 'wildcard_0', ascending = True, inplace = True )
+                    newfile = gzip.open(
+                        f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz",
+                        "wb",
+                    )
+                    l_path_file_mtx_10x.append(
+                        f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz"
+                    )
+        with open(path_file_flag, "w") as file:
+            file.write("completed")
+    else:
+        """retrieve the list of split mtx files"""
+        df = bk.GLOB_Retrive_Strings_in_Wildcards(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz"
+        )
+        df.wildcard_0 = df.wildcard_0.astype(int)
+        df.sort_values("wildcard_0", ascending=True, inplace=True)
         l_path_file_mtx_10x = df.path.values
     return l_path_file_mtx_10x
-dict_id_feature_to_index_feature = dict( )
-def __MTX_10X_Combine__renumber_feature_mtx_10x__( path_file_input, path_folder_mtx_10x_output ) :
-    ''' # deprecated
+
+
+dict_id_feature_to_index_feature = dict()
+
+
+def __MTX_10X_Combine__renumber_feature_mtx_10x__(
+    path_file_input, path_folder_mtx_10x_output
+):
+    """# deprecated
     internal function for MTX_10X_Combine
-    # 2022-02-22 00:38:33 
-    '''
-#     dict_id_feature_to_index_feature = PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_feature_to_index_feature.pickle' ) # retrieve id_feature to index_feature mapping 
-    for path_folder_mtx_10x, int_total_n_barcodes_of_previously_written_matrices, index_mtx_10x in pd.read_csv( path_file_input, sep = '\t' ).values :
+    # 2022-02-22 00:38:33
+    """
+    #     dict_id_feature_to_index_feature = bk.PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_feature_to_index_feature.pickle' ) # retrieve id_feature to index_feature mapping
+    for (
+        path_folder_mtx_10x,
+        int_total_n_barcodes_of_previously_written_matrices,
+        index_mtx_10x,
+    ) in pd.read_csv(path_file_input, sep="\t").values:
         # directly write matrix.mtx.gz file without header
-        with gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", 'wb' ) as newfile :
-            arr_id_feature = pd.read_csv( f'{path_folder_mtx_10x}features.tsv.gz', sep = '\t', header = None ).values[ :, 0 ] # retrieve a list of id_feature for the current dataset
-            with gzip.open( f'{path_folder_mtx_10x}matrix.mtx.gz', 'rb' ) as file : # retrieve a list of features
-                line = file.readline( ).decode( ) # read the first line
+        with gzip.open(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", "wb"
+        ) as newfile:
+            arr_id_feature = pd.read_csv(
+                f"{path_folder_mtx_10x}features.tsv.gz", sep="\t", header=None
+            ).values[
+                :, 0
+            ]  # retrieve a list of id_feature for the current dataset
+            with gzip.open(
+                f"{path_folder_mtx_10x}matrix.mtx.gz", "rb"
+            ) as file:  # retrieve a list of features
+                line = file.readline().decode()  # read the first line
                 # if the first line of the file contains a comment line, read all comment lines and a description line following the comments.
-                if line[ 0 ] == '%' :
+                if len(line) > 0 and line[0] == "%":
                     # read comment and the description line
-                    while True :
-                        if line[ 0 ] != '%' :
+                    while True:
+                        if line[0] != "%":
                             break
-                        line = file.readline( ).decode( ) # read the next line
-                    line = file.readline( ).decode( ) # discard the description line and read the next line
+                        line = file.readline().decode()  # read the next line
+                    line = (
+                        file.readline().decode()
+                    )  # discard the description line and read the next line
                 # process entries
-                while True :
-                    if len( line ) == 0 :
+                while True:
+                    if len(line) == 0:
                         break
-                    index_row, index_col, int_value = tuple( map( int, line.strip( ).split( ) ) ) # parse each entry of the current matrix 
-                    newfile.write( ( ' '.join( tuple( map( str, [ dict_id_feature_to_index_feature[ arr_id_feature[ index_row - 1 ] ], index_col + int_total_n_barcodes_of_previously_written_matrices, int_value ] ) ) ) + '\n' ).encode( ) ) # translate indices of the current matrix to that of the combined matrix            
-                    line = file.readline( ).decode( ) # read the next line
-def Read_SPLiT_Seq( path_folder_mtx ) :
-    ''' # 2022-04-22 07:10:50 
-    Read SPLiT-Seq pipeline output 
+                    index_row, index_col, int_value = tuple(
+                        map(int, line.strip().split())
+                    )  # parse each entry of the current matrix
+                    newfile.write(
+                        (
+                            " ".join(
+                                tuple(
+                                    map(
+                                        str,
+                                        [
+                                            dict_id_feature_to_index_feature[
+                                                arr_id_feature[index_row - 1]
+                                            ],
+                                            index_col
+                                            + int_total_n_barcodes_of_previously_written_matrices,
+                                            int_value,
+                                        ],
+                                    )
+                                )
+                            )
+                            + "\n"
+                        ).encode()
+                    )  # translate indices of the current matrix to that of the combined matrix
+                    line = file.readline().decode()  # read the next line
+
+
+def Read_SPLiT_Seq(path_folder_mtx):
+    """# 2022-04-22 07:10:50
+    Read SPLiT-Seq pipeline output
     return:
     df_feature, df_mtx
-    '''
-    path_file_bc = f'{path_folder_mtx}cell_metadata.csv'
-    path_file_feature = f'{path_folder_mtx}genes.csv'
-    path_file_mtx = f'{path_folder_mtx}DGE.mtx'
+    """
+    path_file_bc = f"{path_folder_mtx}cell_metadata.csv"
+    path_file_feature = f"{path_folder_mtx}genes.csv"
+    path_file_mtx = f"{path_folder_mtx}DGE.mtx"
 
     # read mtx file as a tabular format
-    df_mtx = pd.read_csv( path_file_mtx, sep = ' ', comment = '%' )
-    df_mtx.columns = [ 'id_row', 'id_column', 'read_count' ]
+    df_mtx = pd.read_csv(path_file_mtx, sep=" ", comment="%")
+    df_mtx.columns = ["id_row", "id_column", "read_count"]
 
     # read barcode and feature information
-    df_bc = pd.read_csv( path_file_bc )[ [ 'cell_barcode' ] ]
-    df_bc.columns = [ 'barcode' ]
-    df_feature = pd.read_csv( path_file_feature, index_col = 0 )
-    df_feature.columns = [ 'id_feature', 'feature', 'genome' ]
+    df_bc = pd.read_csv(path_file_bc)[["cell_barcode"]]
+    df_bc.columns = ["barcode"]
+    df_feature = pd.read_csv(path_file_feature, index_col=0)
+    df_feature.columns = ["id_feature", "feature", "genome"]
 
     # mapping using 1 based coordinates (0->1 based coordinate )
-    df_mtx[ 'barcode' ] = df_mtx.id_row.apply( MAP.Map( DICTIONARY_Build_from_arr( df_bc.barcode.values, index_start = 1 ) ).a2b ) # mapping using 1 based coordinates (0->1 based coordinate )
-    df_mtx[ 'id_feature' ] = df_mtx.id_column.apply( MAP.Map( DICTIONARY_Build_from_arr( df_feature.id_feature.values, index_start = 1 ) ).a2b ) 
-    df_mtx.drop( columns = [ 'id_row', 'id_column' ], inplace = True ) # drop unnecessary columns
+    df_mtx["barcode"] = df_mtx.id_row.apply(
+        bk.Map(bk.DICTIONARY_Build_from_arr(df_bc.barcode.values, index_start=1)).a2b
+    )  # mapping using 1 based coordinates (0->1 based coordinate )
+    df_mtx["id_feature"] = df_mtx.id_column.apply(
+        bk.Map(
+            bk.DICTIONARY_Build_from_arr(df_feature.id_feature.values, index_start=1)
+        ).a2b
+    )
+    df_mtx.drop(
+        columns=["id_row", "id_column"], inplace=True
+    )  # drop unnecessary columns
     return df_feature, df_mtx
-def MTX_10X_Barcode_add_prefix_or_suffix( path_file_barcodes_input, path_file_barcodes_output = None, barcode_prefix = '', barcode_suffix = '' ) :
-    ''' # 2022-05-13 17:54:13 
+
+
+def MTX_10X_Barcode_add_prefix_or_suffix(
+    path_file_barcodes_input,
+    path_file_barcodes_output=None,
+    barcode_prefix="",
+    barcode_suffix="",
+):
+    """# 2022-05-13 17:54:13
     Add prefix or suffix to the 'barcode' of a given 'barcodes.tsv.gz' file
     'path_file_barcodes_output' : default: None. by default, the input 'path_file_barcodes_input' file will be overwritten with the modified barcodes
-    '''
-    flag_replace_input_file = path_file_barcodes_output is None # retrieve a flag indicating the replacement of original input file with modified input file
-    if flag_replace_input_file :
-        path_file_barcodes_output = f'{path_file_barcodes_input}.writing.tsv.gz' # set a temporary output file 
-    newfile = gzip.open( path_file_barcodes_output, 'wb' ) # open an output file
-    with gzip.open( path_file_barcodes_input, 'rb' ) as file :
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 :
+    """
+    flag_replace_input_file = (
+        path_file_barcodes_output is None
+    )  # retrieve a flag indicating the replacement of original input file with modified input file
+    if flag_replace_input_file:
+        path_file_barcodes_output = (
+            f"{path_file_barcodes_input}.writing.tsv.gz"  # set a temporary output file
+        )
+    newfile = gzip.open(path_file_barcodes_output, "wb")  # open an output file
+    with gzip.open(path_file_barcodes_input, "rb") as file:
+        while True:
+            line = file.readline()
+            if len(line) == 0:
                 break
-            barcode = line.decode( ).strip( ) # parse a barcode
-            barcode_new = barcode_prefix + barcode + barcode_suffix # compose new barcode
-            newfile.write( ( barcode_new + '\n' ).encode( ) ) # write a new barcode
-    newfile.close( ) # close the output file
+            barcode = line.decode().strip()  # parse a barcode
+            barcode_new = (
+                barcode_prefix + barcode + barcode_suffix
+            )  # compose new barcode
+            newfile.write((barcode_new + "\n").encode())  # write a new barcode
+    newfile.close()  # close the output file
     # if the output file path was not given, replace the original file with modified file
-    if flag_replace_input_file :
-        os.remove( path_file_barcodes_input )
-        os.rename( path_file_barcodes_output, path_file_barcodes_input )
-def MTX_10X_Feature_add_prefix_or_suffix( path_file_features_input, path_file_features_output = None, id_feature_prefix = '', id_feature_suffix = '', name_feature_prefix = '', name_feature_suffix = '' ) :
-    ''' # 2022-05-13 17:54:17 
+    if flag_replace_input_file:
+        filesystem_operations("rm", path_file_barcodes_input)
+        filesystem_operations("mv", path_file_barcodes_output, path_file_barcodes_input)
+
+
+def MTX_10X_Feature_add_prefix_or_suffix(
+    path_file_features_input,
+    path_file_features_output=None,
+    id_feature_prefix="",
+    id_feature_suffix="",
+    name_feature_prefix="",
+    name_feature_suffix="",
+):
+    """# 2022-05-13 17:54:17
     Add prefix or suffix to the id_feature and name_feature of a given 'features.tsv.gz' file
     'path_file_features_output' : default: None. by default, the input 'path_file_features_input' file will be overwritten with the modified features
-    '''
-    flag_replace_input_file = path_file_features_output is None # retrieve a flag indicating the replacement of original input file with modified input file
-    if flag_replace_input_file :
-        path_file_features_output = f'{path_file_features_input}.writing.tsv.gz' # set a temporary output file 
-    newfile = gzip.open( path_file_features_output, 'wb' ) # open an output file
-    with gzip.open( path_file_features_input, 'rb' ) as file :
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 :
+    """
+    flag_replace_input_file = (
+        path_file_features_output is None
+    )  # retrieve a flag indicating the replacement of original input file with modified input file
+    if flag_replace_input_file:
+        path_file_features_output = (
+            f"{path_file_features_input}.writing.tsv.gz"  # set a temporary output file
+        )
+    newfile = gzip.open(path_file_features_output, "wb")  # open an output file
+    with gzip.open(path_file_features_input, "rb") as file:
+        while True:
+            line = file.readline()
+            if len(line) == 0:
                 break
-            id_feature, name_feature, type_feature = line.decode( ).strip( ).split( '\t' ) # parse a feature
-            id_feature_new = id_feature_prefix + id_feature + id_feature_suffix # compose new id_feature
-            name_feature_new = name_feature_prefix + name_feature + name_feature_suffix # compose new name_feature
-            newfile.write( ( '\t'.join( [ id_feature_new, name_feature_new, type_feature ] ) + '\n' ).encode( ) ) # write a new feature
-    newfile.close( ) # close the output file
+            id_feature, name_feature, type_feature = (
+                line.decode().strip().split("\t")
+            )  # parse a feature
+            id_feature_new = (
+                id_feature_prefix + id_feature + id_feature_suffix
+            )  # compose new id_feature
+            name_feature_new = (
+                name_feature_prefix + name_feature + name_feature_suffix
+            )  # compose new name_feature
+            newfile.write(
+                (
+                    "\t".join([id_feature_new, name_feature_new, type_feature]) + "\n"
+                ).encode()
+            )  # write a new feature
+    newfile.close()  # close the output file
     # if the output file path was not given, replace the original file with modified file
-    if flag_replace_input_file :
-        os.remove( path_file_features_input )
-        os.rename( path_file_features_output, path_file_features_input )
-def __MTX_10X_Combine__renumber_barcode_or_feature_index_mtx_10x__( path_file_input, path_folder_mtx_10x_output, flag_renumber_feature_index ) :
-    '''
+    if flag_replace_input_file:
+        filesystem_operations("rm", path_file_features_input)
+        filesystem_operations("mv", path_file_features_output, path_file_features_input)
+
+
+def __MTX_10X_Combine__renumber_barcode_or_feature_index_mtx_10x__(
+    path_file_input, path_folder_mtx_10x_output, flag_renumber_feature_index
+):
+    """
     internal function for MTX_10X_Combine
-    # 2022-04-21 12:10:53 
-    
+    # 2022-04-21 12:10:53
+
     'flag_renumber_feature_index' : if True, assumes barcodes are not shared between matrices and renumber features only. If False, assumes features are not shared between matrices and renumber barcodes only.
-    '''
+    """
     global dict_id_entry_to_index_entry
-    for path_folder_mtx_10x, int_total_n_entries_of_previously_written_matrices, index_mtx_10x in pd.read_csv( path_file_input, sep = '\t' ).values :
+    for (
+        path_folder_mtx_10x,
+        int_total_n_entries_of_previously_written_matrices,
+        index_mtx_10x,
+    ) in pd.read_csv(path_file_input, sep="\t").values:
         # directly write matrix.mtx.gz file without header
-        with gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", 'wb' ) as newfile :
-            arr_id_entry = pd.read_csv( f"{path_folder_mtx_10x}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz", sep = '\t', header = None ).values[ :, 0 ] # retrieve a list of id_feature for the current dataset
-            with gzip.open( f'{path_folder_mtx_10x}matrix.mtx.gz', 'rb' ) as file : # retrieve a list of features
-                line = file.readline( ).decode( ) # read the first line
+        with gzip.open(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", "wb"
+        ) as newfile:
+            arr_id_entry = pd.read_csv(
+                f"{path_folder_mtx_10x}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz",
+                sep="\t",
+                header=None,
+            ).values[
+                :, 0
+            ]  # retrieve a list of id_feature for the current dataset
+            with gzip.open(
+                f"{path_folder_mtx_10x}matrix.mtx.gz", "rb"
+            ) as file:  # retrieve a list of features
+                line = file.readline().decode()  # read the first line
                 # if the first line of the file contains a comment line, read all comment lines and a description line following the comments.
-                if line[ 0 ] == '%' :
+                if len(line) > 0 and line[0] == "%":
                     # read comment and the description line
-                    while True :
-                        if line[ 0 ] != '%' :
+                    while True:
+                        if line[0] != "%":
                             break
-                        line = file.readline( ).decode( ) # read the next line
-                    line = file.readline( ).decode( ) # discard the description line and read the next line
+                        line = file.readline().decode()  # read the next line
+                    line = (
+                        file.readline().decode()
+                    )  # discard the description line and read the next line
                 # process entries
-                while True :
-                    if len( line ) == 0 :
+                while True:
+                    if len(line) == 0:
                         break
-                    index_row, index_col, int_value = tuple( map( int, line.strip( ).split( ) ) ) # parse each entry of the current matrix 
-                    
-                    newfile.write( ( ' '.join( tuple( map( str, ( [ dict_id_entry_to_index_entry[ arr_id_entry[ index_row - 1 ] ], index_col + int_total_n_entries_of_previously_written_matrices ] if flag_renumber_feature_index else [ index_row + int_total_n_entries_of_previously_written_matrices, dict_id_entry_to_index_entry[ arr_id_entry[ index_col - 1 ] ] ] ) + [ int_value ] ) ) ) + '\n' ).encode( ) ) # translate indices of the current matrix to that of the combined matrix            
-                    line = file.readline( ).decode( ) # read the next line
-def MTX_10X_Combine( path_folder_mtx_10x_output, * l_path_folder_mtx_10x_input, int_num_threads = 15, flag_split_mtx = True, flag_split_mtx_again = False, int_max_num_entries_for_chunk = 10000000, flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs = None, flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs = None, verbose = False ) :
-    '''
-    # 2022-05-16 11:39:24 
+                    index_row, index_col, int_value = tuple(
+                        map(int, map(float, line.strip().split()))
+                    )  # parse each entry of the current matrix
+
+                    newfile.write(
+                        (
+                            " ".join(
+                                tuple(
+                                    map(
+                                        str,
+                                        (
+                                            [
+                                                dict_id_entry_to_index_entry[
+                                                    arr_id_entry[index_row - 1]
+                                                ],
+                                                index_col
+                                                + int_total_n_entries_of_previously_written_matrices,
+                                            ]
+                                            if flag_renumber_feature_index
+                                            else [
+                                                index_row
+                                                + int_total_n_entries_of_previously_written_matrices,
+                                                dict_id_entry_to_index_entry[
+                                                    arr_id_entry[index_col - 1]
+                                                ],
+                                            ]
+                                        )
+                                        + [int_value],
+                                    )
+                                )
+                            )
+                            + "\n"
+                        ).encode()
+                    )  # translate indices of the current matrix to that of the combined matrix
+                    line = file.readline().decode()  # read the next line
+
+
+def MTX_10X_Combine(
+    path_folder_mtx_10x_output,
+    *l_path_folder_mtx_10x_input,
+    int_num_threads=15,
+    flag_split_mtx=True,
+    flag_split_mtx_again=False,
+    int_max_num_entries_for_chunk=10000000,
+    flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs=None,
+    flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs=None,
+    verbose=False,
+):
+    """
+    # 2022-12-14 18:47:04
     Combine 10X count matrix files from the given list of folders and write combined output files to the given output folder 'path_folder_mtx_10x_output'
     If there are no shared cells between matrix files, a low-memory mode will be used. The output files will be simply combined since no count summing operation is needed. Only feature matrix will be loaded and updated in the memory.
-    'id_feature' should be unique across all features
-    
+    'id_feature' should be unique across all features. if id_feature is not unique, features with duplicated id_features will lead to combining of the features into a single feature (with combined counts/values).
+
     'int_num_threads' : number of threads to use when combining datasets. multiple threads will be utilized only when datasets does not share cells and thus can be safely concatanated.
     'flag_split_mtx' : split the resulting mtx file so that the contents in the output mtx file can be processed in parallel without ungzipping the mtx.gz file and spliting the file.
-    'flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs' : a flag for entering low-memory mode when there is no shared cells between given input matrices. By default (when None is given), matrices will be examined and the flag will be set automatically by the program. To reduce running time and memory, this flag can be manually set by users. Explicitly setting this flag will dramatically reduce the memory consumption. 
-    'flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs' : a flag for entering low-memory mode when there is no shared features between given input matrices. By default (when None is given), matrices will be examined and the flag will be set automatically by the program. To reduce running time and memory, this flag can be manually set by users. Explicitly setting this flag will dramatically reduce the memory consumption. 
-    '''
-    
+    'flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs' : a flag for entering low-memory mode when there is no shared cells between given input matrices. By default (when None is given), matrices will be examined and the flag will be set automatically by the program. To reduce running time and memory, this flag can be manually set by users. Explicitly setting this flag will dramatically reduce the memory consumption.
+    'flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs' : a flag for entering low-memory mode when there is no shared features between given input matrices. By default (when None is given), matrices will be examined and the flag will be set automatically by the program. To reduce running time and memory, this flag can be manually set by users. Explicitly setting this flag will dramatically reduce the memory consumption.
+    """
+
     # create an output folder
-    os.makedirs( path_folder_mtx_10x_output, exist_ok = True ) 
+    filesystem_operations("mkdir", path_folder_mtx_10x_output, exist_ok=True)
 
-    if not flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs and flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs is None :
-        """ retrieve cell barcodes of all 10X matrices and check whether cell barcodes are not shared between matrices """
-        int_total_n_barcodes_of_previously_written_matrices = 0 # follow the number of barcodes that are previously written
-        l_int_total_n_barcodes_of_previously_written_matrices = [ ] # calculate the number of barcodes of the previous dataset in the combined mtx.
-        set_barcode = set( ) # update a set of unique barcodes
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            arr_barcode = pd.read_csv( f'{path_folder_mtx_10x}barcodes.tsv.gz', sep = '\t', header = None ).squeeze( "columns" ).values # retrieve a list of features
-            set_barcode.update( arr_barcode ) # update a set of barcodes
-            l_int_total_n_barcodes_of_previously_written_matrices.append( int_total_n_barcodes_of_previously_written_matrices )
-            int_total_n_barcodes_of_previously_written_matrices += len( arr_barcode ) # update the number of barcodes 
-        ''' check whether there are shared cell barcodes between matrices and set a flag for entering a low-memory mode '''
-        flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs = len( set_barcode ) == int_total_n_barcodes_of_previously_written_matrices # update flag
-    elif flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs :
-        """ retrieve cell barcodes of all 10X matrices and check whether cell barcodes are not shared between matrices """
-        int_total_n_barcodes_of_previously_written_matrices = 0 # follow the number of barcodes that are previously written
-        l_int_total_n_barcodes_of_previously_written_matrices = [ ] # calculate the number of barcodes of the previous dataset in the combined mtx.
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            l_int_total_n_barcodes_of_previously_written_matrices.append( int_total_n_barcodes_of_previously_written_matrices )
-            int_total_n_barcodes_of_previously_written_matrices += len( pd.read_csv( f'{path_folder_mtx_10x}barcodes.tsv.gz', sep = '\t', header = None ) ) # retrieve a list of barcodes and # update the number of barcodes 
-    
-    if not flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs and flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs is None :
-        """ retrieve features of all 10X matrices and check whether features are not shared between matrices """
-        int_total_n_features_of_previously_written_matrices = 0 # follow the number of features that are previously written
-        l_int_total_n_features_of_previously_written_matrices = [ ] # calculate the number of features of the previous dataset in the combined mtx.
-        set_feature = set( ) # update a set of unique features
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            arr_feature = pd.read_csv( f'{path_folder_mtx_10x}features.tsv.gz', sep = '\t', header = None, usecols = [ 0 ] ).squeeze( "columns" ).values # retrieve a list of features
-            set_feature.update( arr_feature ) # update a set of features
-            l_int_total_n_features_of_previously_written_matrices.append( int_total_n_features_of_previously_written_matrices )
-            int_total_n_features_of_previously_written_matrices += len( arr_feature ) # update the number of features 
-        ''' check whether there are shared features between matrices and set a flag for entering a low-memory mode '''
-        flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs = len( set_feature ) == int_total_n_features_of_previously_written_matrices # update flag
-    elif flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs :
-        """ retrieve features of all 10X matrices and check whether features are not shared between matrices """
-        int_total_n_features_of_previously_written_matrices = 0 # follow the number of features that are previously written
-        l_int_total_n_features_of_previously_written_matrices = [ ] # calculate the number of features of the previous dataset in the combined mtx.
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            l_int_total_n_features_of_previously_written_matrices.append( int_total_n_features_of_previously_written_matrices )
-            int_total_n_features_of_previously_written_matrices += len( pd.read_csv( f'{path_folder_mtx_10x}features.tsv.gz', sep = '\t', header = None, usecols = [ 0 ] ) ) # retrieve a list of features and update the number of features 
-        
-
-    flag_low_memory_mode = flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs or flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs # retrieve flag for low-memory mode
-    if flag_low_memory_mode :
-        """ low-memory mode """
-        flag_renumber_feature_index = flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs # retrieve a flag for renumbering features
-        if verbose :
-            print( f"entering low-memory mode, re-numbering {'features' if flag_renumber_feature_index else 'barcodes'} index because {'barcodes' if flag_renumber_feature_index else 'features'} are not shared across the matrices." )
-        
-        """ write a combined barcodes/features.tsv.gz - that are not shared between matrices """
-        OS_FILE_Combine_Files_in_order( list( f"{path_folder_mtx_10x}{'barcodes' if flag_renumber_feature_index else 'features'}.tsv.gz" for path_folder_mtx_10x in l_path_folder_mtx_10x_input ), f"{path_folder_mtx_10x_output}{'barcodes' if flag_renumber_feature_index else 'features'}.tsv.gz", overwrite_existing_file = True )
+    if (
+        not flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs
+        and flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs is None
+    ):
+        """retrieve cell barcodes of all 10X matrices and check whether cell barcodes are not shared between matrices"""
+        int_total_n_barcodes_of_previously_written_matrices = (
+            0  # follow the number of barcodes that are previously written
+        )
+        l_int_total_n_barcodes_of_previously_written_matrices = (
+            []
+        )  # calculate the number of barcodes of the previous dataset in the combined mtx.
+        set_barcode = set()  # update a set of unique barcodes
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            arr_barcode = (
+                pd.read_csv(
+                    f"{path_folder_mtx_10x}barcodes.tsv.gz", sep="\t", header=None
+                )
+                .squeeze("columns")
+                .values
+            )  # retrieve a list of features
+            set_barcode.update(arr_barcode)  # update a set of barcodes
+            l_int_total_n_barcodes_of_previously_written_matrices.append(
+                int_total_n_barcodes_of_previously_written_matrices
+            )
+            int_total_n_barcodes_of_previously_written_matrices += len(
+                arr_barcode
+            )  # update the number of barcodes
+        """ check whether there are shared cell barcodes between matrices and set a flag for entering a low-memory mode """
+        flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs = (
+            len(set_barcode) == int_total_n_barcodes_of_previously_written_matrices
+        )  # update flag
+    elif flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs:
+        """retrieve cell barcodes of all 10X matrices and check whether cell barcodes are not shared between matrices"""
+        int_total_n_barcodes_of_previously_written_matrices = (
+            0  # follow the number of barcodes that are previously written
+        )
+        l_int_total_n_barcodes_of_previously_written_matrices = (
+            []
+        )  # calculate the number of barcodes of the previous dataset in the combined mtx.
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            l_int_total_n_barcodes_of_previously_written_matrices.append(
+                int_total_n_barcodes_of_previously_written_matrices
+            )
+            int_total_n_barcodes_of_previously_written_matrices += len(
+                pd.read_csv(
+                    f"{path_folder_mtx_10x}barcodes.tsv.gz", sep="\t", header=None
+                )
+            )  # retrieve a list of barcodes and # update the number of barcodes
+
+    if (
+        not flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs
+        and flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs is None
+    ):
+        """retrieve features of all 10X matrices and check whether features are not shared between matrices"""
+        int_total_n_features_of_previously_written_matrices = (
+            0  # follow the number of features that are previously written
+        )
+        l_int_total_n_features_of_previously_written_matrices = (
+            []
+        )  # calculate the number of features of the previous dataset in the combined mtx.
+        set_feature = set()  # update a set of unique features
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            arr_feature = (
+                pd.read_csv(
+                    f"{path_folder_mtx_10x}features.tsv.gz",
+                    sep="\t",
+                    header=None,
+                    usecols=[0],
+                )
+                .squeeze("columns")
+                .values
+            )  # retrieve a list of features
+            set_feature.update(arr_feature)  # update a set of features
+            l_int_total_n_features_of_previously_written_matrices.append(
+                int_total_n_features_of_previously_written_matrices
+            )
+            int_total_n_features_of_previously_written_matrices += len(
+                arr_feature
+            )  # update the number of features
+        """ check whether there are shared features between matrices and set a flag for entering a low-memory mode """
+        flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs = (
+            len(set_feature) == int_total_n_features_of_previously_written_matrices
+        )  # update flag
+    elif flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs:
+        """retrieve features of all 10X matrices and check whether features are not shared between matrices"""
+        int_total_n_features_of_previously_written_matrices = (
+            0  # follow the number of features that are previously written
+        )
+        l_int_total_n_features_of_previously_written_matrices = (
+            []
+        )  # calculate the number of features of the previous dataset in the combined mtx.
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            l_int_total_n_features_of_previously_written_matrices.append(
+                int_total_n_features_of_previously_written_matrices
+            )
+            int_total_n_features_of_previously_written_matrices += len(
+                pd.read_csv(
+                    f"{path_folder_mtx_10x}features.tsv.gz",
+                    sep="\t",
+                    header=None,
+                    usecols=[0],
+                )
+            )  # retrieve a list of features and update the number of features
+
+    flag_low_memory_mode = (
+        flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs
+        or flag_low_memory_mode_because_there_is_no_shared_feature_between_mtxs
+    )  # retrieve flag for low-memory mode
+    if flag_low_memory_mode:
+        """low-memory mode"""
+        flag_renumber_feature_index = flag_low_memory_mode_because_there_is_no_shared_cell_between_mtxs  # retrieve a flag for renumbering features
+        if verbose:
+            logger.info(
+                f"entering low-memory mode, re-numbering {'features' if flag_renumber_feature_index else 'barcodes'} index because {'barcodes' if flag_renumber_feature_index else 'features'} are not shared across the matrices."
+            )
 
-        ''' collect a set of unique entries and a list of entries for each 10X matrix '''
-        set_t_entry = set( ) # update a set unique id_entry (either id_cell or id_entry)
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            set_t_entry.update( list( map( tuple, pd.read_csv( f"{path_folder_mtx_10x}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz", sep = '\t', header = None ).values ) ) ) # update a set of feature tuples
+        """ write a combined barcodes/features.tsv.gz - that are not shared between matrices """
+        bk.OS_Run(
+            ["cat"]
+            + list(
+                f"{path_folder_mtx_10x}{'barcodes' if flag_renumber_feature_index else 'features'}.tsv.gz"
+                for path_folder_mtx_10x in l_path_folder_mtx_10x_input
+            ),
+            path_file_stdout=f"{path_folder_mtx_10x_output}{'barcodes' if flag_renumber_feature_index else 'features'}.tsv.gz",
+            stdout_binary=True,
+            return_output=False,
+        )  # combine the files in order
+
+        """ collect a set of unique entries and a list of entries for each 10X matrix """
+        set_t_entry = set()  # update a set unique id_entry (either id_cell or id_entry)
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            set_t_entry.update(
+                list(
+                    map(
+                        tuple,
+                        pd.read_csv(
+                            f"{path_folder_mtx_10x}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz",
+                            sep="\t",
+                            header=None,
+                        ).values,
+                    )
+                )
+            )  # update a set of feature tuples
 
         """ write a combined features/barcodes.tsv.gz - that are shared between matrices """
-        l_t_entry = list( set_t_entry ) # convert set to list
-        with gzip.open( f"{path_folder_mtx_10x_output}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz", 'wb' ) as newfile :
-            for t_entry in l_t_entry :
-                newfile.write( ( '\t'.join( t_entry ) + '\n' ).encode( ) )
+        l_t_entry = list(set_t_entry)  # convert set to list
+        with gzip.open(
+            f"{path_folder_mtx_10x_output}{'features' if flag_renumber_feature_index else 'barcodes'}.tsv.gz",
+            "wb",
+        ) as newfile:
+            for t_entry in l_t_entry:
+                newfile.write(("\t".join(t_entry) + "\n").encode())
 
         """ build a mapping of id_entry to index_entry, which will be consistent across datasets - for features/barcodes that are shared between matrices """
-        global dict_id_entry_to_index_entry # use global variable for multiprocessing
-        dict_id_entry_to_index_entry = dict( ( t_entry[ 0 ], index_entry + 1 ) for index_entry, t_entry in enumerate( l_t_entry ) ) # 0>1 based index
-        PICKLE_Write( f'{path_folder_mtx_10x_output}dict_id_entry_to_index_entry.pickle', dict_id_entry_to_index_entry ) # save id_feature to index_feature mapping as a pickle file
-
-        ''' collect the number of records for each 10X matrix '''
-        int_total_n_records = 0 
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            with gzip.open( f'{path_folder_mtx_10x}matrix.mtx.gz', 'rb' ) as file : # retrieve a list of features
-                file.readline( ), file.readline( )
-                int_total_n_records += int( file.readline( ).decode( ).strip( ).split( )[ 2 ] ) # update the total number of entries
+        global dict_id_entry_to_index_entry  # use global variable for multiprocessing
+        dict_id_entry_to_index_entry = dict(
+            (t_entry[0], index_entry + 1)
+            for index_entry, t_entry in enumerate(l_t_entry)
+        )  # 0>1 based index
+        bk.PICKLE_Write(
+            f"{path_folder_mtx_10x_output}dict_id_entry_to_index_entry.pickle",
+            dict_id_entry_to_index_entry,
+        )  # save id_feature to index_feature mapping as a pickle file
+
+        """ collect the number of records for each 10X matrix """
+        int_total_n_records = 0
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            with gzip.open(
+                f"{path_folder_mtx_10x}matrix.mtx.gz", "rt"
+            ) as file:  # retrieve a list of features
+                line = file.readline()
+                while line[0] == "%":
+                    line = file.readline()
+                int_total_n_records += int(
+                    line.strip().split()[2]
+                )  # update the total number of entries
 
         """ write a part of a combined matrix.mtx.gz for each dataset using multiple processes """
         # compose inputs for multiprocessing
-        df_input = pd.DataFrame( { 'path_folder_input_mtx_10x' : l_path_folder_mtx_10x_input, 'int_total_n_barcodes_of_previously_written_matrices' : ( l_int_total_n_barcodes_of_previously_written_matrices if flag_renumber_feature_index else l_int_total_n_features_of_previously_written_matrices ), 'index_mtx_10x' : np.arange( len( l_int_total_n_barcodes_of_previously_written_matrices ) if flag_renumber_feature_index else len( l_int_total_n_features_of_previously_written_matrices ) ) } )
-        Multiprocessing( df_input, __MTX_10X_Combine__renumber_barcode_or_feature_index_mtx_10x__, int_num_threads, global_arguments = [ path_folder_mtx_10x_output, flag_renumber_feature_index ] )
-#         os.remove( f'{path_folder_mtx_10x_output}dict_id_entry_to_index_entry.pickle' ) # remove pickle file
-        
+        df_input = pd.DataFrame(
+            {
+                "path_folder_input_mtx_10x": l_path_folder_mtx_10x_input,
+                "int_total_n_barcodes_of_previously_written_matrices": (
+                    l_int_total_n_barcodes_of_previously_written_matrices
+                    if flag_renumber_feature_index
+                    else l_int_total_n_features_of_previously_written_matrices
+                ),
+                "index_mtx_10x": np.arange(
+                    len(l_int_total_n_barcodes_of_previously_written_matrices)
+                    if flag_renumber_feature_index
+                    else len(l_int_total_n_features_of_previously_written_matrices)
+                ),
+            }
+        )
+        bk.Multiprocessing(
+            df_input,
+            __MTX_10X_Combine__renumber_barcode_or_feature_index_mtx_10x__,
+            int_num_threads,
+            global_arguments=[path_folder_mtx_10x_output, flag_renumber_feature_index],
+        )
+        #         filesystem_operations( 'rm', f'{path_folder_mtx_10x_output}dict_id_entry_to_index_entry.pickle' ) # remove pickle file
+
         """ combine parts and add the MTX file header to compose a combined mtx file """
-        df_file = GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz" )
-        df_file.wildcard_0 = df_file.wildcard_0.astype( int )
-        df_file.sort_values( 'wildcard_0', inplace = True )
-        # if 'flag_split_mtx' is True, does not delete the split mtx files
-        OS_FILE_Combine_Files_in_order( df_file.path.values, f"{path_folder_mtx_10x_output}matrix.mtx.gz", delete_input_files = not flag_split_mtx, header = f"%%MatrixMarket matrix coordinate integer general\n%\n{len( l_t_entry ) if flag_renumber_feature_index else int_total_n_features_of_previously_written_matrices} {int_total_n_barcodes_of_previously_written_matrices if flag_renumber_feature_index else len( l_t_entry )} {int_total_n_records}\n" ) # combine the output mtx files in the given order
+        df_file = bk.GLOB_Retrive_Strings_in_Wildcards(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz"
+        )
+        df_file.wildcard_0 = df_file.wildcard_0.astype(int)
+        df_file.sort_values("wildcard_0", inplace=True)
+
+        # write header
+        path_file_header = f"{path_folder_mtx_10x_output}matrix.mtx.header.txt.gz"
+        with gzip.open(path_file_header, "wt") as newfile:
+            newfile.write(
+                f"%%MatrixMarket matrix coordinate integer general\n%\n{len( l_t_entry ) if flag_renumber_feature_index else int_total_n_features_of_previously_written_matrices} {int_total_n_barcodes_of_previously_written_matrices if flag_renumber_feature_index else len( l_t_entry )} {int_total_n_records}\n"
+            )
+        bk.OS_Run(
+            ["cat", path_file_header] + list(df_file.path.values),
+            path_file_stdout=f"{path_folder_mtx_10x_output}matrix.mtx.gz",
+            stdout_binary=True,
+            return_output=False,
+        )  # combine the output mtx files in the order
+
+        if not flag_split_mtx:
+            # delete temporary files if 'flag_split_mtx' is False
+            for path_file in df_file.path.values:
+                os.remove(path_file)
+
         # write a flag indicating that the current output directory contains split mtx files
-        with open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.split.flag", 'w' ) as file :
-            file.write( 'completed' )
-        
-    else :
-        ''' normal operation mode perfoming count merging operations '''
-        l_df_mtx, l_df_feature = [ ], [ ]
-        for path_folder_mtx_10x in l_path_folder_mtx_10x_input :
-            df_mtx, df_feature = Read_10X( path_folder_mtx_10x )
-            l_df_mtx.append( df_mtx ), l_df_feature.append( df_feature )
+        with open(f"{path_folder_mtx_10x_output}matrix.mtx.gz.split.flag", "w") as file:
+            file.write("completed")
+    else:
+        """normal operation mode perfoming count merging operations"""
+        l_df_mtx, l_df_feature = [], []
+        for path_folder_mtx_10x in l_path_folder_mtx_10x_input:
+            df_mtx, df_feature = Read_10X(path_folder_mtx_10x)
+            l_df_mtx.append(df_mtx), l_df_feature.append(df_feature)
 
         # combine mtx
-        df_mtx = pd.concat( l_df_mtx )
-        df_mtx = df_mtx.groupby( [ 'barcode', 'id_feature' ] ).sum( )
-        df_mtx.reset_index( drop = False, inplace = True )
+        df_mtx = pd.concat(l_df_mtx)
+        df_mtx = df_mtx.groupby(["barcode", "id_feature"]).sum()
+        df_mtx.reset_index(drop=False, inplace=True)
 
         # combine features
-        df_feature = pd.concat( l_df_feature )
-        df_feature.drop_duplicates( inplace = True )
+        df_feature = pd.concat(l_df_feature)
+        df_feature.drop_duplicates(inplace=True)
+
+        Write_10X(df_mtx, df_feature, path_folder_mtx_10x_output)
 
-        Write_10X( df_mtx, df_feature, path_folder_mtx_10x_output )
-        
         # split a matrix file into multiple files
-        MTX_10X_Split( path_folder_mtx_10x_output, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk )
-def __Combine_Dictionaries__( path_folder_mtx_10x_input, name_dict ) :
-    """ # 2022-03-06 00:06:23 
+        MTX_10X_Split(
+            path_folder_mtx_10x_output,
+            int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+        )
+
+
+def __Combine_Dictionaries__(path_folder_mtx_10x_input, name_dict):
+    """# 2022-03-06 00:06:23
     combined dictionaries processed from individual files
     """
-    if os.path.exists( f'{path_folder_mtx_10x_input}{name_dict}.tsv.gz' ) :
-        ''' if an output file already exists, read the file and return the combined dictionary '''
-        dict_combined = pd.read_csv( f'{path_folder_mtx_10x_input}{name_dict}.tsv.gz', sep = '\t', header = None, index_col = 0 ).iloc[ :, 0 ].to_dict( )
-    else :
-        ''' combine summarized results '''
-        l_path_file = glob.glob( f"{path_folder_mtx_10x_input}{name_dict}.*" )
-        try :
-            counter = collections.Counter( pd.read_csv( l_path_file[ 0 ], sep = '\t', header = None, index_col = 0 ).iloc[ :, 0 ].to_dict( ) ) # initialize counter object with the dictionary from the first file
-        except pd.errors.EmptyDataError :
-            counter = collections.Counter( ) # when an error (possibly because the file is empty) occur, use an empty counter
-        for path_file in l_path_file[ 1 : ] :
+    import collections
+
+    if filesystem_operations(
+        "exists", f"{path_folder_mtx_10x_input}{name_dict}.tsv.gz"
+    ):
+        """if an output file already exists, read the file and return the combined dictionary"""
+        dict_combined = (
+            pd.read_csv(
+                f"{path_folder_mtx_10x_input}{name_dict}.tsv.gz",
+                sep="\t",
+                header=None,
+                index_col=0,
+            )
+            .iloc[:, 0]
+            .to_dict()
+        )
+    else:
+        """combine summarized results"""
+        l_path_file = filesystem_operations(
+            "glob", f"{path_folder_mtx_10x_input}{name_dict}.*"
+        )
+        try:
+            counter = collections.Counter(
+                pd.read_csv(l_path_file[0], sep="\t", header=None, index_col=0)
+                .iloc[:, 0]
+                .to_dict()
+            )  # initialize counter object with the dictionary from the first file
+        except pd.errors.EmptyDataError:
+            counter = (
+                collections.Counter()
+            )  # when an error (possibly because the file is empty) occur, use an empty counter
+        for path_file in l_path_file[1:]:
             # when an error (possibly because the file is empty) occur, skip updating the counter
-            try :
-                counter = counter + collections.Counter( pd.read_csv( path_file, sep = '\t', header = None, index_col = 0 ).iloc[ :, 0 ].to_dict( ) ) # update counter object using the dictionary from each file
-            except pd.errors.EmptyDataError :
+            try:
+                counter = counter + collections.Counter(
+                    pd.read_csv(path_file, sep="\t", header=None, index_col=0)
+                    .iloc[:, 0]
+                    .to_dict()
+                )  # update counter object using the dictionary from each file
+            except pd.errors.EmptyDataError:
                 pass
-        dict_combined = dict( counter ) # retrieve a combined dictionary
-        '''remove temporary files '''
-        for path_file in l_path_file :
-            os.remove( path_file )
-        ''' save dictionary as a file '''
-        pd.Series( dict_combined ).to_csv( f'{path_folder_mtx_10x_input}{name_dict}.tsv.gz', sep = '\t', header = None )
-    return dict_combined # returns a combined dictionary
-def __MTX_10X_Summarize_Counts__summarize_counts_for_each_mtx_10x__( path_file_input, path_folder_mtx_10x_input ) :
-    '''
+        dict_combined = dict(counter)  # retrieve a combined dictionary
+        """remove temporary files """
+        for path_file in l_path_file:
+            filesystem_operations("rm", path_file)
+        """ save dictionary as a file """
+        pd.Series(dict_combined).to_csv(
+            f"{path_folder_mtx_10x_input}{name_dict}.tsv.gz", sep="\t", header=None
+        )
+    return dict_combined  # returns a combined dictionary
+
+
+def __MTX_10X_Summarize_Counts__summarize_counts_for_each_mtx_10x__(
+    path_file_input, path_folder_mtx_10x_input
+):
+    """
     internal function for MTX_10X_Summarize_Count
-    # 2022-04-28 04:26:57 
-    '''
-    ''' survey the metrics '''
-    ''' for each split mtx file, count number of umi and n_feature for each cells or the number of cells for each feature '''
-    ''' initialize the dictionaries that will be handled by the current function '''
-    dict_id_column_to_count = dict( )
-    dict_id_column_to_n_features = dict( )
-    dict_id_row_to_count = dict( )
-    dict_id_row_to_n_cells = dict( )
-    dict_id_row_to_log_transformed_count = dict( )
-    
-    global dict_name_set_feature_to_set_id_row # use global read-only object
-    dict_name_set_feature_to_dict_id_column_to_count = dict( ( name_set_feature, dict( ) ) for name_set_feature in dict_name_set_feature_to_set_id_row ) # initialize 'dict_name_set_feature_to_dict_id_column_to_count'
-    for path_file_input_mtx in pd.read_csv( path_file_input, sep = '\t', header = None ).values.ravel( ) :
-        with gzip.open( path_file_input_mtx, 'rb' ) as file :
-            ''' read the first line '''
-            line = file.readline( ).decode( ) 
-            ''' if the first line of the file contains a comment line, read all comment lines and a description line following the comments. '''
-            if line[ 0 ] == '%' :
+    # 2022-04-28 04:26:57
+    """
+    """ survey the metrics """
+    """ for each split mtx file, count number of umi and n_feature for each cells or the number of cells for each feature """
+    """ initialize the dictionaries that will be handled by the current function """
+    dict_id_column_to_count = dict()
+    dict_id_column_to_n_features = dict()
+    dict_id_row_to_count = dict()
+    dict_id_row_to_n_cells = dict()
+    dict_id_row_to_log_transformed_count = dict()
+
+    global dict_name_set_feature_to_set_id_row  # use global read-only object
+    dict_name_set_feature_to_dict_id_column_to_count = dict(
+        (name_set_feature, dict())
+        for name_set_feature in dict_name_set_feature_to_set_id_row
+    )  # initialize 'dict_name_set_feature_to_dict_id_column_to_count'
+    for path_file_input_mtx in pd.read_csv(
+        path_file_input, sep="\t", header=None
+    ).values.ravel():
+        with gzip.open(path_file_input_mtx, "rb") as file:
+            """read the first line"""
+            line = file.readline().decode()
+            """ if the first line of the file contains a comment line, read all comment lines and a description line following the comments. """
+            if len(line) > 0 and line[0] == "%":
                 # read comment and the description line
-                while True :
-                    if line[ 0 ] != '%' :
+                while True:
+                    if line[0] != "%":
                         break
-                    line = file.readline( ).decode( ) # read the next line
+                    line = file.readline().decode()  # read the next line
                 # process the description line
-                int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
-                line = file.readline( ).decode( ) # read the next line
-            ''' process entries'''
-            while True :
-                if len( line ) == 0 :
+                int_num_rows, int_num_columns, int_num_entries = tuple(
+                    int(e) for e in line.strip().split()
+                )  # retrieve the number of rows, number of columns and number of entries
+                line = file.readline().decode()  # read the next line
+            """ process entries"""
+            while True:
+                if len(line) == 0:
                     break
-                ''' parse a record, and update metrics '''
-                id_row, id_column, int_value = tuple( int( e ) for e in line.strip( ).split( ) ) # parse a record of a matrix-market format file
-                ''' 1-based > 0-based coordinates '''
+                """ parse a record, and update metrics """
+                id_row, id_column, int_value = tuple(
+                    int(float(e)) for e in line.strip().split()
+                )  # parse a record of a matrix-market format file
+                """ 1-based > 0-based coordinates """
                 id_row -= 1
                 id_column -= 1
-                ''' update umi count for each cell '''
-                if id_column not in dict_id_column_to_count :
-                    dict_id_column_to_count[ id_column ] = 0
-                dict_id_column_to_count[ id_column ] += int_value
-                ''' update umi count of specific set of features for each cell '''
-                for name_set_feature in dict_name_set_feature_to_dict_id_column_to_count :
-                    if id_row in dict_name_set_feature_to_set_id_row[ name_set_feature ] :
-                        if id_column not in dict_name_set_feature_to_dict_id_column_to_count[ name_set_feature ] :
-                            dict_name_set_feature_to_dict_id_column_to_count[ name_set_feature ][ id_column ] = 0
-                        dict_name_set_feature_to_dict_id_column_to_count[ name_set_feature ][ id_column ] += int_value
-                ''' update n_features for each cell '''
-                if id_column not in dict_id_column_to_n_features :
-                    dict_id_column_to_n_features[ id_column ] = 0
-                dict_id_column_to_n_features[ id_column ] += 1
-                ''' update umi count for each feature '''
-                if id_row not in dict_id_row_to_count :
-                    dict_id_row_to_count[ id_row ] = 0
-                dict_id_row_to_count[ id_row ] += int_value
-                ''' update n_cells for each feature '''
-                if id_row not in dict_id_row_to_n_cells :
-                    dict_id_row_to_n_cells[ id_row ] = 0
-                dict_id_row_to_n_cells[ id_row ] += 1
-                ''' update log transformed counts, calculated by 'X_new = log_10(X_old + 1)', for each feature '''
-                if id_row not in dict_id_row_to_log_transformed_count :
-                    dict_id_row_to_log_transformed_count[ id_row ] = 0
-                dict_id_row_to_log_transformed_count[ id_row ] += math.log10( int_value + 1 )
-                
-                ''' read the next line '''
-                line = file.readline( ).decode( ) # binary > uncompressed string # read the next line
-    
+                """ update umi count for each cell """
+                if id_column not in dict_id_column_to_count:
+                    dict_id_column_to_count[id_column] = 0
+                dict_id_column_to_count[id_column] += int_value
+                """ update umi count of specific set of features for each cell """
+                for (
+                    name_set_feature
+                ) in dict_name_set_feature_to_dict_id_column_to_count:
+                    if id_row in dict_name_set_feature_to_set_id_row[name_set_feature]:
+                        if (
+                            id_column
+                            not in dict_name_set_feature_to_dict_id_column_to_count[
+                                name_set_feature
+                            ]
+                        ):
+                            dict_name_set_feature_to_dict_id_column_to_count[
+                                name_set_feature
+                            ][id_column] = 0
+                        dict_name_set_feature_to_dict_id_column_to_count[
+                            name_set_feature
+                        ][id_column] += int_value
+                """ update n_features for each cell """
+                if id_column not in dict_id_column_to_n_features:
+                    dict_id_column_to_n_features[id_column] = 0
+                dict_id_column_to_n_features[id_column] += 1
+                """ update umi count for each feature """
+                if id_row not in dict_id_row_to_count:
+                    dict_id_row_to_count[id_row] = 0
+                dict_id_row_to_count[id_row] += int_value
+                """ update n_cells for each feature """
+                if id_row not in dict_id_row_to_n_cells:
+                    dict_id_row_to_n_cells[id_row] = 0
+                dict_id_row_to_n_cells[id_row] += 1
+                """ update log transformed counts, calculated by 'X_new = log_10(X_old + 1)', for each feature """
+                if id_row not in dict_id_row_to_log_transformed_count:
+                    dict_id_row_to_log_transformed_count[id_row] = 0
+                dict_id_row_to_log_transformed_count[id_row] += math.log10(
+                    int_value + 1
+                )
+
+                """ read the next line """
+                line = (
+                    file.readline().decode()
+                )  # binary > uncompressed string # read the next line
+
     # save collected count as tsv files
-    str_uuid_process = UUID( ) # retrieve uuid of the current process
-    pd.Series( dict_id_column_to_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_column_to_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_column_to_n_features ).to_csv( f'{path_folder_mtx_10x_input}dict_id_column_to_n_features.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_n_cells ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_n_cells.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_log_transformed_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_log_transformed_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    
+    str_uuid_process = bk.UUID()  # retrieve uuid of the current process
+    pd.Series(dict_id_column_to_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_column_to_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_column_to_n_features).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_column_to_n_features.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_n_cells).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_n_cells.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_log_transformed_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_log_transformed_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+
     # save collected counts as tsv files for 'dict_name_set_feature_to_dict_id_column_to_count'
-    for name_set_feature in dict_name_set_feature_to_dict_id_column_to_count :
-        pd.Series( dict_name_set_feature_to_dict_id_column_to_count[ name_set_feature ] ).to_csv( f'{path_folder_mtx_10x_input}{name_set_feature}.dict_id_column_to_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-def MTX_10X_Summarize_Counts( path_folder_mtx_10x_input, verbose = False, int_num_threads = 15, flag_split_mtx = True, int_max_num_entries_for_chunk = 10000000, dict_name_set_feature_to_l_id_feature = dict( ), flag_split_mtx_again = False ) :
-    """ # 2022-04-28 06:53:45 
-    Summarize 
-    (1) UMI and Feature counts for each cell, 
+    for name_set_feature in dict_name_set_feature_to_dict_id_column_to_count:
+        pd.Series(
+            dict_name_set_feature_to_dict_id_column_to_count[name_set_feature]
+        ).to_csv(
+            f"{path_folder_mtx_10x_input}{name_set_feature}.dict_id_column_to_count.{str_uuid_process}.tsv.gz",
+            sep="\t",
+            header=None,
+        )
+
+
+def MTX_10X_Summarize_Counts(
+    path_folder_mtx_10x_input,
+    verbose=False,
+    int_num_threads=15,
+    flag_split_mtx=True,
+    int_max_num_entries_for_chunk=10000000,
+    dict_name_set_feature_to_l_id_feature=dict(),
+    flag_split_mtx_again=False,
+):
+    """# 2022-04-28 06:53:45
+    Summarize
+    (1) UMI and Feature counts for each cell,
     (2) UMI and Cell counts for each feature, and
     (3) log10-transformed values of UMI counts (X_new = log_10(X_old + 1)) for each feature
     (4) UMI counts for the optionally given lists of features for each cell
     and save these metrics as TSV files
 
     Inputs:
     'dict_name_set_feature_to_l_id_feature' : (Default: None)
-                                            a dictionary with 'name_set_features' as key and a list of id_feature as value for each set of id_features. 
-                                            If None is given, only the basic metrics will be summarized. 
+                                            a dictionary with 'name_set_features' as key and a list of id_feature as value for each set of id_features.
+                                            If None is given, only the basic metrics will be summarized.
                                             'name_set_features' should be compatible as a Linux file system (should not contain '/' and other special characters, such as newlines).
                                             (for Scarab short_read outputs)
                                             If 'atac' is given, 'promoter_and_gene_body', 'promoter' features will be summarized.
                                             If 'multiome' is given, total 'atac' counts will be summarized separately in addition to 'atac' mode
 
     Returns:
     a dictionary containing the following and other additional dictionaries: dict_id_column_to_count, dict_id_column_to_n_features, dict_id_row_to_count, dict_id_row_to_n_cells, dict_id_row_to_log_transformed_count
     """
 
-    ''' the name of the dictionaries handled by this function (basic) '''
-    l_name_dict = [ 'dict_id_column_to_count', 'dict_id_column_to_n_features', 'dict_id_row_to_count', 'dict_id_row_to_n_cells', 'dict_id_row_to_log_transformed_count' ]
-
-    ''' handle inputs '''
-    if path_folder_mtx_10x_input[ -1 ] != '/' :
-        path_folder_mtx_10x_input += '/'
+    """ the name of the dictionaries handled by this function (basic) """
+    l_name_dict = [
+        "dict_id_column_to_count",
+        "dict_id_column_to_n_features",
+        "dict_id_row_to_count",
+        "dict_id_row_to_n_cells",
+        "dict_id_row_to_log_transformed_count",
+    ]
+
+    """ handle inputs """
+    if path_folder_mtx_10x_input[-1] != "/":
+        path_folder_mtx_10x_input += "/"
 
     # define flag and check whether the flag exists
     path_file_flag = f"{path_folder_mtx_10x_input}counts_summarized.flag"
-    if not os.path.exists( path_file_flag ) :
+    if not filesystem_operations("exists", path_file_flag):
         # define input file directories
-        path_file_input_bc = f'{path_folder_mtx_10x_input}barcodes.tsv.gz'
-        path_file_input_feature = f'{path_folder_mtx_10x_input}features.tsv.gz'
-        path_file_input_mtx = f'{path_folder_mtx_10x_input}matrix.mtx.gz'
+        path_file_input_bc = f"{path_folder_mtx_10x_input}barcodes.tsv.gz"
+        path_file_input_feature = f"{path_folder_mtx_10x_input}features.tsv.gz"
+        path_file_input_mtx = f"{path_folder_mtx_10x_input}matrix.mtx.gz"
 
         # check whether all required files are present
-        if sum( list( not os.path.exists( path_folder ) for path_folder in [ path_file_input_bc, path_file_input_feature, path_file_input_mtx ] ) ) :
-            if verbose :
-                print( f'required file(s) is not present at {path_folder_mtx_10x}' )
+        if sum(
+            list(
+                not filesystem_operations("exists", path_folder)
+                for path_folder in [
+                    path_file_input_bc,
+                    path_file_input_feature,
+                    path_file_input_mtx,
+                ]
+            )
+        ):
+            if verbose:
+                logger.info(f"required file(s) is not present at {path_folder_mtx_10x}")
+
+        """ split input mtx file into multiple files """
+        l_path_file_mtx_10x = MTX_10X_Split(
+            path_folder_mtx_10x_input,
+            int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+            flag_split_mtx=flag_split_mtx,
+            flag_split_mtx_again=flag_split_mtx_again,
+        )
 
-        ''' split input mtx file into multiple files '''
-        l_path_file_mtx_10x = MTX_10X_Split( path_folder_mtx_10x_input, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk, flag_split_mtx = flag_split_mtx, flag_split_mtx_again = flag_split_mtx_again )
-
-        ''' prepare 'dict_name_set_feature_to_set_id_row' for summarizing total counts for given sets of features '''
+        """ prepare 'dict_name_set_feature_to_set_id_row' for summarizing total counts for given sets of features """
         global dict_name_set_feature_to_set_id_row
-        dict_name_set_feature_to_set_id_row = dict( ) # initialize 'dict_name_set_feature_to_set_id_row'
-        if dict_name_set_feature_to_l_id_feature is not None :
-            arr_id_feature = pd.read_csv( path_file_input_feature, sep = '\t', usecols = [ 0 ], header = None ).values.ravel( ) # retrieve array of id_features
-            dict_id_feature_to_id_row = dict( ( e, i ) for i, e in enumerate( arr_id_feature ) ) # retrieve id_feature -> id_row mapping
-
-            ''' handle presets for 'dict_name_set_feature_to_l_id_feature' '''
-            if isinstance( dict_name_set_feature_to_l_id_feature, str ) :    
-                str_preset = dict_name_set_feature_to_l_id_feature # retrieve preset
-                dict_name_set_feature_to_l_id_feature = dict( ) # initialize the dictionary
-                if str_preset in [ 'multiome', 'atac' ] :
-                    if str_preset == 'multiome' :
-                        arr_id_feature_atac = Search_list_of_strings_with_multiple_query( arr_id_feature, '|mode=atac' )
-                        dict_name_set_feature_to_l_id_feature[ 'atac_all' ] = arr_id_feature_atac
-                    elif str_preset == 'atac' :
+        dict_name_set_feature_to_set_id_row = (
+            dict()
+        )  # initialize 'dict_name_set_feature_to_set_id_row'
+        if dict_name_set_feature_to_l_id_feature is not None:
+            arr_id_feature = pd.read_csv(
+                path_file_input_feature, sep="\t", usecols=[0], header=None
+            ).values.ravel()  # retrieve array of id_features
+            dict_id_feature_to_id_row = dict(
+                (e, i) for i, e in enumerate(arr_id_feature)
+            )  # retrieve id_feature -> id_row mapping
+
+            """ handle presets for 'dict_name_set_feature_to_l_id_feature' """
+            if isinstance(dict_name_set_feature_to_l_id_feature, str):
+                str_preset = dict_name_set_feature_to_l_id_feature  # retrieve preset
+                dict_name_set_feature_to_l_id_feature = (
+                    dict()
+                )  # initialize the dictionary
+                if str_preset in ["multiome", "atac"]:
+                    if str_preset == "multiome":
+                        arr_id_feature_atac = (
+                            bk.Search_list_of_strings_with_multiple_query(
+                                arr_id_feature, "|mode=atac"
+                            )
+                        )
+                        dict_name_set_feature_to_l_id_feature[
+                            "atac_all"
+                        ] = arr_id_feature_atac
+                    elif str_preset == "atac":
                         arr_id_feature_atac = arr_id_feature
                     # add sets of promoter and gene_body features
-                    arr_id_feature_atac_promoter_and_gene_body = Search_list_of_strings_with_multiple_query( arr_id_feature_atac, '-genomic_region|', '-repeatmasker_ucsc|', '-regulatory_element|' )
-                    arr_id_feature_atac_promoter = Search_list_of_strings_with_multiple_query( arr_id_feature_atac_promoter_and_gene_body, 'promoter|' )
-                    dict_name_set_feature_to_l_id_feature[ 'atac_promoter_and_gene_body' ] = arr_id_feature_atac_promoter_and_gene_body    
-                    dict_name_set_feature_to_l_id_feature[ 'atac_promoter' ] = arr_id_feature_atac_promoter
+                    arr_id_feature_atac_promoter_and_gene_body = (
+                        bk.Search_list_of_strings_with_multiple_query(
+                            arr_id_feature_atac,
+                            "-genomic_region|",
+                            "-repeatmasker_ucsc|",
+                            "-regulatory_element|",
+                        )
+                    )
+                    arr_id_feature_atac_promoter = (
+                        bk.Search_list_of_strings_with_multiple_query(
+                            arr_id_feature_atac_promoter_and_gene_body, "promoter|"
+                        )
+                    )
+                    dict_name_set_feature_to_l_id_feature[
+                        "atac_promoter_and_gene_body"
+                    ] = arr_id_feature_atac_promoter_and_gene_body
+                    dict_name_set_feature_to_l_id_feature[
+                        "atac_promoter"
+                    ] = arr_id_feature_atac_promoter
 
             # make sure that 'name_set_feature' does not contains characters incompatible with linux file path
-            for name_set_feature in dict_name_set_feature_to_l_id_feature :
-                assert not( '/' in name_set_feature or '\n' in name_set_feature )
-
-            dict_name_set_feature_to_set_id_row = dict( ( name_set_feature, set( dict_id_feature_to_id_row[ id_feature ] for id_feature in dict_name_set_feature_to_l_id_feature[ name_set_feature ] ) ) for name_set_feature in dict_name_set_feature_to_l_id_feature )
-            # PICKLE_Write( f"{path_folder_mtx_10x_input}dict_name_set_feature_to_set_id_row.binary.pickle", dict_name_set_feature_to_set_id_row ) # write the dictionary as a pickle
+            for name_set_feature in dict_name_set_feature_to_l_id_feature:
+                assert not ("/" in name_set_feature or "\n" in name_set_feature)
 
-        ''' summarize each split mtx file '''
-        Multiprocessing( l_path_file_mtx_10x, __MTX_10X_Summarize_Counts__summarize_counts_for_each_mtx_10x__, n_threads = int_num_threads, global_arguments = [ path_folder_mtx_10x_input ] )
+            dict_name_set_feature_to_set_id_row = dict(
+                (
+                    name_set_feature,
+                    set(
+                        dict_id_feature_to_id_row[id_feature]
+                        for id_feature in dict_name_set_feature_to_l_id_feature[
+                            name_set_feature
+                        ]
+                    ),
+                )
+                for name_set_feature in dict_name_set_feature_to_l_id_feature
+            )
+            # bk.PICKLE_Write( f"{path_folder_mtx_10x_input}dict_name_set_feature_to_set_id_row.binary.pickle", dict_name_set_feature_to_set_id_row ) # write the dictionary as a pickle
+
+        """ summarize each split mtx file """
+        bk.Multiprocessing(
+            l_path_file_mtx_10x,
+            __MTX_10X_Summarize_Counts__summarize_counts_for_each_mtx_10x__,
+            n_threads=int_num_threads,
+            global_arguments=[path_folder_mtx_10x_input],
+        )
 
-        ''' combine summarized results '''
+        """ combine summarized results """
         # update the list of the names of dictionaries
-        l_name_dict += list( f"{name_set_feature}.dict_id_column_to_count" for name_set_feature in GLOB_Retrive_Strings_in_Wildcards( f'{path_folder_mtx_10x_input}*.dict_id_column_to_count.*.tsv.gz' ).wildcard_0.unique( ) ) 
-
-        dict_dict = dict( )
-        for name_dict in l_name_dict :
-            dict_dict[ name_dict ] = __Combine_Dictionaries__( path_folder_mtx_10x_input, name_dict )
+        l_name_dict += list(
+            f"{name_set_feature}.dict_id_column_to_count"
+            for name_set_feature in bk.GLOB_Retrive_Strings_in_Wildcards(
+                f"{path_folder_mtx_10x_input}*.dict_id_column_to_count.*.tsv.gz"
+            ).wildcard_0.unique()
+        )
+
+        dict_dict = dict()
+        for name_dict in l_name_dict:
+            dict_dict[name_dict] = __Combine_Dictionaries__(
+                path_folder_mtx_10x_input, name_dict
+            )
         # write the flag
-        with open( path_file_flag, 'w' ) as newfile :
-            newfile.write( 'completed at ' + TIME_GET_timestamp( True ) )
-    else :
-        ''' read summarized results '''
+        with open(path_file_flag, "w") as newfile:
+            newfile.write("completed at " + bk.TIME_GET_timestamp(True))
+    else:
+        """read summarized results"""
         # update the list of the names of dictionaries
-        l_name_dict += list( f"{name_set_feature}.dict_id_column_to_count" for name_set_feature in GLOB_Retrive_Strings_in_Wildcards( f'{path_folder_mtx_10x_input}*.dict_id_column_to_count.tsv.gz' ).wildcard_0.unique( ) ) 
-
-        dict_dict = dict( )
-        for name_dict in l_name_dict :
-            try :
-                dict_dict[ name_dict ] = pd.read_csv( f'{path_folder_mtx_10x_input}{name_dict}.tsv.gz', sep = '\t', header = None, index_col = 0 ).iloc[ :, 0 ].to_dict( )
-            except pd.errors.EmptyDataError : # handle when the current dictionary is empty
-                dict_dict[ name_dict ] = dict( )
+        l_name_dict += list(
+            f"{name_set_feature}.dict_id_column_to_count"
+            for name_set_feature in bk.GLOB_Retrive_Strings_in_Wildcards(
+                f"{path_folder_mtx_10x_input}*.dict_id_column_to_count.tsv.gz"
+            ).wildcard_0.unique()
+        )
+
+        dict_dict = dict()
+        for name_dict in l_name_dict:
+            try:
+                dict_dict[name_dict] = (
+                    pd.read_csv(
+                        f"{path_folder_mtx_10x_input}{name_dict}.tsv.gz",
+                        sep="\t",
+                        header=None,
+                        index_col=0,
+                    )
+                    .iloc[:, 0]
+                    .to_dict()
+                )
+            except pd.errors.EmptyDataError:  # handle when the current dictionary is empty
+                dict_dict[name_dict] = dict()
 
     # return summarized metrics
     return dict_dict
-def MTX_10X_Retrieve_number_of_rows_columns_and_records( path_folder_mtx_10x_input ) :
-    """ # 2022-03-05 19:58:32 
-    Retrieve the number of rows, columns, and entries from the matrix with the matrix market format 
-    
+
+
+def MTX_10X_Retrieve_number_of_rows_columns_and_records(path_folder_mtx_10x_input):
+    """# 2022-03-05 19:58:32
+    Retrieve the number of rows, columns, and entries from the matrix with the matrix market format
+
+    'path_folder_mtx_10x_input' : a folder mtx file resides or path to mtx file
+
     Returns:
     int_num_rows, int_num_columns, int_num_entries
     """
-    ''' handle inputs '''
-    if path_folder_mtx_10x_input[ -1 ] != '/' :
-        path_folder_mtx_10x_input += '/'
+    """ handle inputs """
+    if (
+        path_folder_mtx_10x_input[-3:].lower() == ".gz"
+    ):  # when a path to mtx file was given
+        path_file_input_mtx = path_folder_mtx_10x_input
+    else:  # when a folder where mtx file resides was given
+        if path_folder_mtx_10x_input[-1] != "/":
+            path_folder_mtx_10x_input += "/"
+
+        # define input file directories
+        path_file_input_mtx = f"{path_folder_mtx_10x_input}matrix.mtx.gz"
+
+        # check whether all required files are present
+        if sum(
+            list(
+                not filesystem_operations("exists", path_folder)
+                for path_folder in [path_file_input_mtx]
+            )
+        ):
+            return None
 
-    # define input file directories
-    path_file_input_mtx = f'{path_folder_mtx_10x_input}matrix.mtx.gz'
-    
-    # check whether all required files are present
-    if sum( list( not os.path.exists( path_folder ) for path_folder in [ path_file_input_mtx ] ) ) :
-        if verbose :
-            print( f'required file(s) is not present at {path_folder_mtx_10x}' )
-    
     # read the input matrix
-    with gzip.open( path_file_input_mtx, 'rb' ) as file :
-        ''' read the first line '''
-        line = file.readline( ).decode( ).strip( )
-        ''' if the first line of the file contains a comment line, read all comment lines and a description line following the comments. '''
-        if line[ 0 ] == '%' :
+    with gzip.open(path_file_input_mtx, "rb") as file:
+        """read the first line"""
+        line = file.readline().decode().strip()
+        """ if the first line of the file contains a comment line, read all comment lines and a description line following the comments. """
+        if len(line) > 0 and line[0] == "%":
             # read comment and the description line
-            while True :
-                if line[ 0 ] != '%' :
+            while True:
+                if line[0] != "%":
                     break
-                line = file.readline( ).decode( ).strip( ) # read the next line
+                line = file.readline().decode().strip()  # read the next line
             # process the description line
-            int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
-        else :
-            ''' the first line does not contain a comment, assumes it contains a description line '''
-            int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
+            int_num_rows, int_num_columns, int_num_entries = tuple(
+                int(e) for e in line.strip().split()
+            )  # retrieve the number of rows, number of columns and number of entries
+        else:
+            """the first line does not contain a comment, assumes it contains a description line"""
+            int_num_rows, int_num_columns, int_num_entries = tuple(
+                int(e) for e in line.strip().split()
+            )  # retrieve the number of rows, number of columns and number of entries
     return int_num_rows, int_num_columns, int_num_entries
-dict_id_column_to_count, dict_id_row_to_avg_count, dict_id_row_to_avg_log_transformed_count, dict_id_row_to_avg_normalized_count, dict_id_row_to_avg_log_transformed_normalized_count = dict( ), dict( ), dict( ), dict( ), dict( ) # global variables # total UMI counts for each cell, average feature counts for each feature
-def __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__first_pass__( path_file_input, path_folder_mtx_10x_input, int_target_sum ) :
-    ''' # 2022-03-06 01:21:07 
+
+
+(
+    dict_id_column_to_count,
+    dict_id_row_to_avg_count,
+    dict_id_row_to_avg_log_transformed_count,
+    dict_id_row_to_avg_normalized_count,
+    dict_id_row_to_avg_log_transformed_normalized_count,
+) = (
+    dict(),
+    dict(),
+    dict(),
+    dict(),
+    dict(),
+)  # global variables # total UMI counts for each cell, average feature counts for each feature
+
+
+def __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__first_pass__(
+    path_file_input, path_folder_mtx_10x_input, int_target_sum
+):
+    """# 2022-03-06 01:21:07
     internal function for MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr
-    '''
-    global dict_id_column_to_count, dict_id_row_to_avg_count, dict_id_row_to_avg_log_transformed_count # use data in read-only global variables 
-    ''' initialize the dictionaries that will be handled by the current function '''
-    dict_id_row_to_deviation_from_mean_count = dict( )
-    dict_id_row_to_deviation_from_mean_log_transformed_count = dict( )
-    dict_id_row_to_normalized_count = dict( )
-    dict_id_row_to_log_transformed_normalized_count = dict( )
-    
-    for path_file_input_mtx in pd.read_csv( path_file_input, sep = '\t', header = None ).values.ravel( ) :
-        with gzip.open( path_file_input_mtx, 'rb' ) as file :
-            ''' read the first line '''
-            line = file.readline( ).decode( ) 
-            ''' if the first line of the file contains a comment line, read all comment lines and a description line following the comments. '''
-            if line[ 0 ] == '%' :
+    """
+    global dict_id_column_to_count, dict_id_row_to_avg_count, dict_id_row_to_avg_log_transformed_count  # use data in read-only global variables
+    """ initialize the dictionaries that will be handled by the current function """
+    dict_id_row_to_deviation_from_mean_count = dict()
+    dict_id_row_to_deviation_from_mean_log_transformed_count = dict()
+    dict_id_row_to_normalized_count = dict()
+    dict_id_row_to_log_transformed_normalized_count = dict()
+
+    for path_file_input_mtx in pd.read_csv(
+        path_file_input, sep="\t", header=None
+    ).values.ravel():
+        with gzip.open(path_file_input_mtx, "rb") as file:
+            """read the first line"""
+            line = file.readline().decode()
+            """ if the first line of the file contains a comment line, read all comment lines and a description line following the comments. """
+            if len(line) > 0 and line[0] == "%":
                 # read comment and the description line
-                while True :
-                    if line[ 0 ] != '%' :
+                while True:
+                    if line[0] != "%":
                         break
-                    line = file.readline( ).decode( ) # read the next line
+                    line = file.readline().decode()  # read the next line
                 # process the description line
-                int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
-                line = file.readline( ).decode( ) # read the next line
-            ''' process entries'''
-            while True :
-                if len( line ) == 0 :
+                int_num_rows, int_num_columns, int_num_entries = tuple(
+                    int(e) for e in line.strip().split()
+                )  # retrieve the number of rows, number of columns and number of entries
+                line = file.readline().decode()  # read the next line
+            """ process entries"""
+            while True:
+                if len(line) == 0:
                     break
-                ''' parse a record, and update metrics '''
-                id_row, id_column, int_value = tuple( int( e ) for e in line.strip( ).split( ) ) # parse a record of a matrix-market format file
-                ''' 1-based > 0-based coordinates '''
+                """ parse a record, and update metrics """
+                id_row, id_column, int_value = tuple(
+                    int(e) for e in line.strip().split()
+                )  # parse a record of a matrix-market format file
+                """ 1-based > 0-based coordinates """
                 id_row -= 1
                 id_column -= 1
-                
-                ''' update deviation from mean umi count for count of each feature '''
-                if id_row not in dict_id_row_to_deviation_from_mean_count :
-                    dict_id_row_to_deviation_from_mean_count[ id_row ] = 0
-                dict_id_row_to_deviation_from_mean_count[ id_row ] += ( int_value - dict_id_row_to_avg_count[ id_row ] ) ** 2
-                ''' update deviation from mean log transformed umi count for log_transformed count of each feature '''
-                if id_row not in dict_id_row_to_deviation_from_mean_log_transformed_count :
-                    dict_id_row_to_deviation_from_mean_log_transformed_count[ id_row ] = 0
-                dict_id_row_to_deviation_from_mean_log_transformed_count[ id_row ] += ( math.log10( int_value + 1 ) - dict_id_row_to_avg_log_transformed_count[ id_row ] ) ** 2
-                ''' calculate normalized target sum '''
-                int_value_normalized = int_value / dict_id_column_to_count[ id_column ] * int_target_sum 
-                ''' update normalized counts, calculated by 'X_new = X_old / total_umi * int_target_sum', for each feature '''
-                if id_row not in dict_id_row_to_normalized_count :
-                    dict_id_row_to_normalized_count[ id_row ] = 0
-                dict_id_row_to_normalized_count[ id_row ] += int_value_normalized
-                ''' update log transformed normalized counts, calculated by 'X_new = log_10(X_old / total_umi * int_target_sum + 1)', for each feature '''
-                if id_row not in dict_id_row_to_log_transformed_normalized_count :
-                    dict_id_row_to_log_transformed_normalized_count[ id_row ] = 0
-                dict_id_row_to_log_transformed_normalized_count[ id_row ] += math.log10( int_value_normalized + 1 ) 
-                
-                line = file.readline( ).decode( ) # binary > uncompressed string # read the next line
-    
+
+                """ update deviation from mean umi count for count of each feature """
+                if id_row not in dict_id_row_to_deviation_from_mean_count:
+                    dict_id_row_to_deviation_from_mean_count[id_row] = 0
+                dict_id_row_to_deviation_from_mean_count[id_row] += (
+                    int_value - dict_id_row_to_avg_count[id_row]
+                ) ** 2
+                """ update deviation from mean log transformed umi count for log_transformed count of each feature """
+                if (
+                    id_row
+                    not in dict_id_row_to_deviation_from_mean_log_transformed_count
+                ):
+                    dict_id_row_to_deviation_from_mean_log_transformed_count[id_row] = 0
+                dict_id_row_to_deviation_from_mean_log_transformed_count[id_row] += (
+                    math.log10(int_value + 1)
+                    - dict_id_row_to_avg_log_transformed_count[id_row]
+                ) ** 2
+                """ calculate normalized target sum """
+                int_value_normalized = (
+                    int_value / dict_id_column_to_count[id_column] * int_target_sum
+                )
+                """ update normalized counts, calculated by 'X_new = X_old / total_umi * int_target_sum', for each feature """
+                if id_row not in dict_id_row_to_normalized_count:
+                    dict_id_row_to_normalized_count[id_row] = 0
+                dict_id_row_to_normalized_count[id_row] += int_value_normalized
+                """ update log transformed normalized counts, calculated by 'X_new = log_10(X_old / total_umi * int_target_sum + 1)', for each feature """
+                if id_row not in dict_id_row_to_log_transformed_normalized_count:
+                    dict_id_row_to_log_transformed_normalized_count[id_row] = 0
+                dict_id_row_to_log_transformed_normalized_count[id_row] += math.log10(
+                    int_value_normalized + 1
+                )
+
+                line = (
+                    file.readline().decode()
+                )  # binary > uncompressed string # read the next line
+
     # save collected count as tsv files
-    str_uuid_process = UUID( ) # retrieve uuid of the current process
-    pd.Series( dict_id_row_to_deviation_from_mean_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_deviation_from_mean_log_transformed_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_log_transformed_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_normalized_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_normalized_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_log_transformed_normalized_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_log_transformed_normalized_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-def __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__second_pass__( path_file_input, path_folder_mtx_10x_input, int_target_sum ) :
-    ''' # 2022-03-06 01:21:14 
+    str_uuid_process = bk.UUID()  # retrieve uuid of the current process
+    pd.Series(dict_id_row_to_deviation_from_mean_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_deviation_from_mean_log_transformed_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_log_transformed_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_normalized_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_normalized_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(dict_id_row_to_log_transformed_normalized_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_log_transformed_normalized_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+
+
+def __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__second_pass__(
+    path_file_input, path_folder_mtx_10x_input, int_target_sum
+):
+    """# 2022-03-06 01:21:14
     internal function for MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr
-    '''
-    global dict_id_column_to_count, dict_id_row_to_avg_normalized_count, dict_id_row_to_avg_log_transformed_normalized_count # use data in read-only global variables 
-    ''' initialize the dictionaries that will be handled by the current function '''
-    dict_id_row_to_deviation_from_mean_normalized_count = dict( )
-    dict_id_row_to_deviation_from_mean_log_transformed_normalized_count = dict( )
-    
-    for path_file_input_mtx in pd.read_csv( path_file_input, sep = '\t', header = None ).values.ravel( ) :
-        with gzip.open( path_file_input_mtx, 'rb' ) as file :
-            ''' read the first line '''
-            line = file.readline( ).decode( ) 
-            ''' if the first line of the file contains a comment line, read all comment lines and a description line following the comments. '''
-            if line[ 0 ] == '%' :
+    """
+    global dict_id_column_to_count, dict_id_row_to_avg_normalized_count, dict_id_row_to_avg_log_transformed_normalized_count  # use data in read-only global variables
+    """ initialize the dictionaries that will be handled by the current function """
+    dict_id_row_to_deviation_from_mean_normalized_count = dict()
+    dict_id_row_to_deviation_from_mean_log_transformed_normalized_count = dict()
+
+    for path_file_input_mtx in pd.read_csv(
+        path_file_input, sep="\t", header=None
+    ).values.ravel():
+        with gzip.open(path_file_input_mtx, "rb") as file:
+            """read the first line"""
+            line = file.readline().decode()
+            """ if the first line of the file contains a comment line, read all comment lines and a description line following the comments. """
+            if len(line) > 0 and line[0] == "%":
                 # read comment and the description line
-                while True :
-                    if line[ 0 ] != '%' :
+                while True:
+                    if line[0] != "%":
                         break
-                    line = file.readline( ).decode( ) # read the next line
+                    line = file.readline().decode()  # read the next line
                 # process the description line
-                int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
-                line = file.readline( ).decode( ) # read the next line
-            ''' process entries'''
-            while True :
-                if len( line ) == 0 :
+                int_num_rows, int_num_columns, int_num_entries = tuple(
+                    int(e) for e in line.strip().split()
+                )  # retrieve the number of rows, number of columns and number of entries
+                line = file.readline().decode()  # read the next line
+            """ process entries"""
+            while True:
+                if len(line) == 0:
                     break
-                ''' parse a record, and update metrics '''
-                id_row, id_column, int_value = tuple( int( e ) for e in line.strip( ).split( ) ) # parse a record of a matrix-market format file
-                ''' 1-based > 0-based coordinates '''
+                """ parse a record, and update metrics """
+                id_row, id_column, int_value = tuple(
+                    int(e) for e in line.strip().split()
+                )  # parse a record of a matrix-market format file
+                """ 1-based > 0-based coordinates """
                 id_row -= 1
                 id_column -= 1
-                
-                ''' calculate normalized target sum '''
-                int_value_normalized = int_value / dict_id_column_to_count[ id_column ] * int_target_sum 
-                ''' update deviation from mean normalized umi counts, calculated by 'X_new = X_old / total_umi * int_target_sum', for each feature '''
-                if id_row not in dict_id_row_to_deviation_from_mean_normalized_count :
-                    dict_id_row_to_deviation_from_mean_normalized_count[ id_row ] = 0
-                dict_id_row_to_deviation_from_mean_normalized_count[ id_row ] += ( int_value_normalized - dict_id_row_to_avg_normalized_count[ id_row ] ) ** 2
-                ''' update deviation from mean log transformed normalized umi counts, calculated by 'X_new = log_10(X_old / total_umi * int_target_sum + 1)', for each feature '''
-                if id_row not in dict_id_row_to_deviation_from_mean_log_transformed_normalized_count :
-                    dict_id_row_to_deviation_from_mean_log_transformed_normalized_count[ id_row ] = 0
-                dict_id_row_to_deviation_from_mean_log_transformed_normalized_count[ id_row ] += ( math.log10( int_value_normalized + 1 ) - dict_id_row_to_avg_log_transformed_normalized_count[ id_row ] ) ** 2
-                
-                line = file.readline( ).decode( ) # binary > uncompressed string # read the next line
-    
+
+                """ calculate normalized target sum """
+                int_value_normalized = (
+                    int_value / dict_id_column_to_count[id_column] * int_target_sum
+                )
+                """ update deviation from mean normalized umi counts, calculated by 'X_new = X_old / total_umi * int_target_sum', for each feature """
+                if id_row not in dict_id_row_to_deviation_from_mean_normalized_count:
+                    dict_id_row_to_deviation_from_mean_normalized_count[id_row] = 0
+                dict_id_row_to_deviation_from_mean_normalized_count[id_row] += (
+                    int_value_normalized - dict_id_row_to_avg_normalized_count[id_row]
+                ) ** 2
+                """ update deviation from mean log transformed normalized umi counts, calculated by 'X_new = log_10(X_old / total_umi * int_target_sum + 1)', for each feature """
+                if (
+                    id_row
+                    not in dict_id_row_to_deviation_from_mean_log_transformed_normalized_count
+                ):
+                    dict_id_row_to_deviation_from_mean_log_transformed_normalized_count[
+                        id_row
+                    ] = 0
+                dict_id_row_to_deviation_from_mean_log_transformed_normalized_count[
+                    id_row
+                ] += (
+                    math.log10(int_value_normalized + 1)
+                    - dict_id_row_to_avg_log_transformed_normalized_count[id_row]
+                ) ** 2
+
+                line = (
+                    file.readline().decode()
+                )  # binary > uncompressed string # read the next line
+
     # save collected count as tsv files
-    str_uuid_process = UUID( ) # retrieve uuid of the current process
-    pd.Series( dict_id_row_to_deviation_from_mean_normalized_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_normalized_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-    pd.Series( dict_id_row_to_deviation_from_mean_log_transformed_normalized_count ).to_csv( f'{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_log_transformed_normalized_count.{str_uuid_process}.tsv.gz', sep = '\t', header = None )
-def MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr( path_folder_mtx_10x_input, int_target_sum = 10000, verbose = False, int_num_threads = 15, flag_split_mtx = True, int_max_num_entries_for_chunk = 10000000 ) :
-    """ # 2022-02-23 22:54:35 
+    str_uuid_process = bk.UUID()  # retrieve uuid of the current process
+    pd.Series(dict_id_row_to_deviation_from_mean_normalized_count).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_normalized_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+    pd.Series(
+        dict_id_row_to_deviation_from_mean_log_transformed_normalized_count
+    ).to_csv(
+        f"{path_folder_mtx_10x_input}dict_id_row_to_deviation_from_mean_log_transformed_normalized_count.{str_uuid_process}.tsv.gz",
+        sep="\t",
+        header=None,
+    )
+
+
+def MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr(
+    path_folder_mtx_10x_input,
+    int_target_sum=10000,
+    verbose=False,
+    int_num_threads=15,
+    flag_split_mtx=True,
+    int_max_num_entries_for_chunk=10000000,
+):
+    """# 2022-02-23 22:54:35
     Calculate average log transformed normalized expr
     (1) UMI and Feature counts for cells, and
     (2) Cell counts for features,
     and save these metrics as TSV files
-    
+
     Arguments:
     'int_target_sum' : the target count for the total UMI count for each cell. The counts will normalized to meet the target sum.
-    
+
     Returns:
     dict_id_column_to_count, dict_id_column_to_n_features, dict_id_row_to_count, dict_id_row_to_n_cells, dict_id_row_to_log_transformed_count
     """
 
-    ''' handle inputs '''
-    if path_folder_mtx_10x_input[ -1 ] != '/' :
-        path_folder_mtx_10x_input += '/'
+    """ handle inputs """
+    if path_folder_mtx_10x_input[-1] != "/":
+        path_folder_mtx_10x_input += "/"
 
     # define flag and check whether the flag exists
     path_file_flag = f"{path_folder_mtx_10x_input}avg_expr_normalized_summarized.int_target_sum__{int_target_sum}.flag"
-    if not os.path.exists( path_file_flag ) :
+    if not filesystem_operations("exists", path_file_flag):
         # define input file directories
-        path_file_input_bc = f'{path_folder_mtx_10x_input}barcodes.tsv.gz'
-        path_file_input_feature = f'{path_folder_mtx_10x_input}features.tsv.gz'
-        path_file_input_mtx = f'{path_folder_mtx_10x_input}matrix.mtx.gz'
+        path_file_input_bc = f"{path_folder_mtx_10x_input}barcodes.tsv.gz"
+        path_file_input_feature = f"{path_folder_mtx_10x_input}features.tsv.gz"
+        path_file_input_mtx = f"{path_folder_mtx_10x_input}matrix.mtx.gz"
 
         # check whether all required files are present
-        if sum( list( not os.path.exists( path_folder ) for path_folder in [ path_file_input_bc, path_file_input_feature, path_file_input_mtx ] ) ) :
-            if verbose :
-                print( f'required file(s) is not present at {path_folder_mtx_10x}' )
-
-        ''' split input mtx file into multiple files '''
-        l_path_file_mtx_10x = MTX_10X_Split( path_folder_mtx_10x_input, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk, flag_split_mtx = flag_split_mtx )
-
-        ''' retrieve number of cells, features, and entries from the matrix file '''
-        int_num_cells, int_num_features, int_num_entries = MTX_10X_Retrieve_number_of_rows_columns_and_records( path_folder_mtx_10x_input )
-        
-        ''' summarizes counts '''
-        global dict_id_column_to_count, dict_id_row_to_avg_count, dict_id_row_to_avg_log_transformed_count, dict_id_row_to_avg_normalized_count, dict_id_row_to_avg_log_transformed_normalized_count # use global variable
-        dict_data = MTX_10X_Summarize_Counts( path_folder_mtx_10x_input, verbose = verbose, int_num_threads = int_num_threads, flag_split_mtx = flag_split_mtx, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk )
-        dict_id_column_to_count, dict_id_column_to_n_features, dict_id_row_to_count, dict_id_row_to_n_cells, dict_id_row_to_log_transformed_count = dict_data[ 'dict_id_column_to_count' ], dict_data[ 'dict_id_column_to_n_features' ], dict_data[ 'dict_id_row_to_count' ], dict_data[ 'dict_id_row_to_n_cells' ], dict_data[ 'dict_id_row_to_log_transformed_count' ] # parse 'dict_data'
+        if sum(
+            list(
+                not filesystem_operations("exists", path_folder)
+                for path_folder in [
+                    path_file_input_bc,
+                    path_file_input_feature,
+                    path_file_input_mtx,
+                ]
+            )
+        ):
+            if verbose:
+                logger.info(f"required file(s) is not present at {path_folder_mtx_10x}")
+
+        """ split input mtx file into multiple files """
+        l_path_file_mtx_10x = MTX_10X_Split(
+            path_folder_mtx_10x_input,
+            int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+            flag_split_mtx=flag_split_mtx,
+        )
+
+        """ retrieve number of cells, features, and entries from the matrix file """
+        (
+            int_num_cells,
+            int_num_features,
+            int_num_entries,
+        ) = MTX_10X_Retrieve_number_of_rows_columns_and_records(
+            path_folder_mtx_10x_input
+        )
+
+        """ summarizes counts """
+        global dict_id_column_to_count, dict_id_row_to_avg_count, dict_id_row_to_avg_log_transformed_count, dict_id_row_to_avg_normalized_count, dict_id_row_to_avg_log_transformed_normalized_count  # use global variable
+        dict_data = MTX_10X_Summarize_Counts(
+            path_folder_mtx_10x_input,
+            verbose=verbose,
+            int_num_threads=int_num_threads,
+            flag_split_mtx=flag_split_mtx,
+            int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+        )
+        (
+            dict_id_column_to_count,
+            dict_id_column_to_n_features,
+            dict_id_row_to_count,
+            dict_id_row_to_n_cells,
+            dict_id_row_to_log_transformed_count,
+        ) = (
+            dict_data["dict_id_column_to_count"],
+            dict_data["dict_id_column_to_n_features"],
+            dict_data["dict_id_row_to_count"],
+            dict_data["dict_id_row_to_n_cells"],
+            dict_data["dict_id_row_to_log_transformed_count"],
+        )  # parse 'dict_data'
 
         """ first pass """
         # calculate mean counts
-        dict_id_row_to_avg_count = ( pd.Series( dict_id_row_to_count ) / int_num_cells ).to_dict( ) # calculate average expression of each feature
-        dict_id_row_to_avg_log_transformed_count = ( pd.Series( dict_id_row_to_log_transformed_count ) / int_num_cells ).to_dict( ) # calculate average log-transformed expression of each feature
-        
-        ''' calculated average log2 transformed normalized expr for each split mtx file '''
-        Multiprocessing( l_path_file_mtx_10x, __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__first_pass__, n_threads = int_num_threads, global_arguments = [ path_folder_mtx_10x_input, int_target_sum ] )
-
-        l_name_dict_first_pass = [ 'dict_id_row_to_deviation_from_mean_count', 'dict_id_row_to_deviation_from_mean_log_transformed_count', 'dict_id_row_to_normalized_count', 'dict_id_row_to_log_transformed_normalized_count' ]
-        
-        ''' combine summarized results '''
-        dict_dict = dict( )
-        for name_dict in l_name_dict_first_pass :
-            dict_dict[ name_dict ] = __Combine_Dictionaries__( path_folder_mtx_10x_input, name_dict )
-            
+        dict_id_row_to_avg_count = (
+            pd.Series(dict_id_row_to_count) / int_num_cells
+        ).to_dict()  # calculate average expression of each feature
+        dict_id_row_to_avg_log_transformed_count = (
+            pd.Series(dict_id_row_to_log_transformed_count) / int_num_cells
+        ).to_dict()  # calculate average log-transformed expression of each feature
+
+        """ calculated average log2 transformed normalized expr for each split mtx file """
+        bk.Multiprocessing(
+            l_path_file_mtx_10x,
+            __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__first_pass__,
+            n_threads=int_num_threads,
+            global_arguments=[path_folder_mtx_10x_input, int_target_sum],
+        )
+
+        l_name_dict_first_pass = [
+            "dict_id_row_to_deviation_from_mean_count",
+            "dict_id_row_to_deviation_from_mean_log_transformed_count",
+            "dict_id_row_to_normalized_count",
+            "dict_id_row_to_log_transformed_normalized_count",
+        ]
+
+        """ combine summarized results """
+        dict_dict = dict()
+        for name_dict in l_name_dict_first_pass:
+            dict_dict[name_dict] = __Combine_Dictionaries__(
+                path_folder_mtx_10x_input, name_dict
+            )
+
         """ second pass """
         # calculate mean counts
-        dict_id_row_to_avg_normalized_count = ( pd.Series( dict_dict[ 'dict_id_row_to_normalized_count' ] ) / int_num_cells ).to_dict( ) # calculate average expression of each feature
-        dict_id_row_to_avg_log_transformed_normalized_count = ( pd.Series( dict_dict[ 'dict_id_row_to_log_transformed_normalized_count' ] ) / int_num_cells ).to_dict( ) # calculate average log-transformed expression of each feature
-        
-        ''' calculated average log2 transformed normalized expr for each split mtx file '''
-        Multiprocessing( l_path_file_mtx_10x, __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__second_pass__, n_threads = int_num_threads, global_arguments = [ path_folder_mtx_10x_input, int_target_sum ] )
-
-        l_name_dict_second_pass = [ 'dict_id_row_to_deviation_from_mean_normalized_count', 'dict_id_row_to_deviation_from_mean_log_transformed_normalized_count' ]
-        
-        ''' combine summarized results '''
-        for name_dict in l_name_dict_second_pass :
-            dict_dict[ name_dict ] = __Combine_Dictionaries__( path_folder_mtx_10x_input, name_dict )
-            
-        ''' compose a dataframe containing the summary about the features '''
-        df_summary = pd.DataFrame( { 
-            'n_cells' : pd.Series( dict_id_row_to_n_cells ),
-            'variance_of_count' : pd.Series( dict_dict[ 'dict_id_row_to_deviation_from_mean_count' ] ) / ( int_num_cells - 1 ),
-            'variance_of_log_transformed_count' : pd.Series( dict_dict[ 'dict_id_row_to_deviation_from_mean_log_transformed_count' ] ) / ( int_num_cells - 1 ),
-            'variance_of_normalized_count' : pd.Series( dict_dict[ 'dict_id_row_to_deviation_from_mean_normalized_count' ] ) / ( int_num_cells - 1 ),
-            'variance_of_log_transformed_normalized_count' : pd.Series( dict_dict[ 'dict_id_row_to_deviation_from_mean_log_transformed_normalized_count' ] ) / ( int_num_cells - 1 ),
-            'mean_count' : pd.Series( dict_id_row_to_avg_count ),
-            'mean_log_transformed_count' : pd.Series( dict_id_row_to_avg_log_transformed_count ),
-            'mean_normalized_count' : pd.Series( dict_id_row_to_avg_normalized_count ),
-            'mean_log_transformed_normalized_count' : pd.Series( dict_id_row_to_avg_log_transformed_normalized_count ),
-        } )
+        dict_id_row_to_avg_normalized_count = (
+            pd.Series(dict_dict["dict_id_row_to_normalized_count"]) / int_num_cells
+        ).to_dict()  # calculate average expression of each feature
+        dict_id_row_to_avg_log_transformed_normalized_count = (
+            pd.Series(dict_dict["dict_id_row_to_log_transformed_normalized_count"])
+            / int_num_cells
+        ).to_dict()  # calculate average log-transformed expression of each feature
+
+        """ calculated average log2 transformed normalized expr for each split mtx file """
+        bk.Multiprocessing(
+            l_path_file_mtx_10x,
+            __MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr__second_pass__,
+            n_threads=int_num_threads,
+            global_arguments=[path_folder_mtx_10x_input, int_target_sum],
+        )
+
+        l_name_dict_second_pass = [
+            "dict_id_row_to_deviation_from_mean_normalized_count",
+            "dict_id_row_to_deviation_from_mean_log_transformed_normalized_count",
+        ]
+
+        """ combine summarized results """
+        for name_dict in l_name_dict_second_pass:
+            dict_dict[name_dict] = __Combine_Dictionaries__(
+                path_folder_mtx_10x_input, name_dict
+            )
+
+        """ compose a dataframe containing the summary about the features """
+        df_summary = pd.DataFrame(
+            {
+                "n_cells": pd.Series(dict_id_row_to_n_cells),
+                "variance_of_count": pd.Series(
+                    dict_dict["dict_id_row_to_deviation_from_mean_count"]
+                )
+                / (int_num_cells - 1),
+                "variance_of_log_transformed_count": pd.Series(
+                    dict_dict[
+                        "dict_id_row_to_deviation_from_mean_log_transformed_count"
+                    ]
+                )
+                / (int_num_cells - 1),
+                "variance_of_normalized_count": pd.Series(
+                    dict_dict["dict_id_row_to_deviation_from_mean_normalized_count"]
+                )
+                / (int_num_cells - 1),
+                "variance_of_log_transformed_normalized_count": pd.Series(
+                    dict_dict[
+                        "dict_id_row_to_deviation_from_mean_log_transformed_normalized_count"
+                    ]
+                )
+                / (int_num_cells - 1),
+                "mean_count": pd.Series(dict_id_row_to_avg_count),
+                "mean_log_transformed_count": pd.Series(
+                    dict_id_row_to_avg_log_transformed_count
+                ),
+                "mean_normalized_count": pd.Series(dict_id_row_to_avg_normalized_count),
+                "mean_log_transformed_normalized_count": pd.Series(
+                    dict_id_row_to_avg_log_transformed_normalized_count
+                ),
+            }
+        )
         # read a dataframe containing features
-        df_feature = pd.read_csv( path_file_input_feature, sep = '\t', header = None )
-        df_feature.columns = [ 'id_feature', 'feature', 'feature_type' ]
-        
-        df_summary = df_summary.join( df_feature, how = 'left' ) # add df_feature to the df_summary
-        df_summary.index.name = 'id_row' 
-        df_summary.reset_index( drop = False, inplace = True ) # retrieve id_row as a column
-        df_summary.to_csv( f'{path_folder_mtx_10x_input}statistical_summary_of_features.int_target_sum__{int_target_sum}.tsv.gz', sep = '\t', index = False ) # save statistical summary as a text file
-        
+        df_feature = pd.read_csv(path_file_input_feature, sep="\t", header=None)
+        df_feature.columns = ["id_feature", "feature", "feature_type"]
+
+        df_summary = df_summary.join(
+            df_feature, how="left"
+        )  # add df_feature to the df_summary
+        df_summary.index.name = "id_row"
+        df_summary.reset_index(drop=False, inplace=True)  # retrieve id_row as a column
+        df_summary.to_csv(
+            f"{path_folder_mtx_10x_input}statistical_summary_of_features.int_target_sum__{int_target_sum}.tsv.gz",
+            sep="\t",
+            index=False,
+        )  # save statistical summary as a text file
+
         # write the flag
-        with open( path_file_flag, 'w' ) as newfile :
-            newfile.write( 'completed at ' + TIME_GET_timestamp( True ) )
-    else :
-        ''' if 'MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr' function has been already run on the current folder, read the previously saved result, and return the summary dataframe '''
-        df_summary = pd.read_csv( f'{path_folder_mtx_10x_input}statistical_summary_of_features.int_target_sum__{int_target_sum}.tsv.gz', sep = '\t' ) # save statistical summary as a text file
+        with open(path_file_flag, "w") as newfile:
+            newfile.write("completed at " + bk.TIME_GET_timestamp(True))
+    else:
+        """if 'MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr' function has been already run on the current folder, read the previously saved result, and return the summary dataframe"""
+        df_summary = pd.read_csv(
+            f"{path_folder_mtx_10x_input}statistical_summary_of_features.int_target_sum__{int_target_sum}.tsv.gz",
+            sep="\t",
+        )  # save statistical summary as a text file
     return df_summary
-dict_id_column_previous_to_id_column_current, dict_id_row_previous_to_id_row_current = dict( ), dict( )
-def __MTX_10X_Filter__filter_mtx_10x__( path_file_input, path_folder_mtx_10x_output ) :
-    """ # 2022-02-22 02:06:03 
+
+
+dict_id_column_previous_to_id_column_current, dict_id_row_previous_to_id_row_current = (
+    dict(),
+    dict(),
+)
+
+
+def __MTX_10X_Filter__filter_mtx_10x__(path_file_input, path_folder_mtx_10x_output):
+    """# 2022-02-22 02:06:03
     __MTX_10X_Filter__filter_mtx_10x__
-    
+
     Returns:
     int_n_entries = total number of entries written by the current process after filtering
     """
-    int_n_entries = 0 # total number of entries written by the current process after filtering
-#     dict_id_column_previous_to_id_column_current = PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_column_previous_to_id_column_current.pickle' ) # retrieve id_feature to index_feature mapping 
-#     dict_id_row_previous_to_id_row_current = PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_row_previous_to_id_row_current.pickle' ) # retrieve id_feature to index_feature mapping 
+    int_n_entries = (
+        0  # total number of entries written by the current process after filtering
+    )
+    #     dict_id_column_previous_to_id_column_current = bk.PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_column_previous_to_id_column_current.pickle' ) # retrieve id_feature to index_feature mapping
+    #     dict_id_row_previous_to_id_row_current = bk.PICKLE_Read( f'{path_folder_mtx_10x_output}dict_id_row_previous_to_id_row_current.pickle' ) # retrieve id_feature to index_feature mapping
     """ write a filtered matrix.mtx.gz for each split mtx file """
-    for path_file_mtx_10x, index_mtx_10x in pd.read_csv( path_file_input, sep = '\t' ).values :
+    for path_file_mtx_10x, index_mtx_10x in pd.read_csv(
+        path_file_input, sep="\t"
+    ).values:
         # directly write matrix.mtx.gz file without using an external dependency
-        with gzip.open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", 'wb' ) as newfile :
-            with gzip.open( path_file_mtx_10x, 'rb' ) as file : 
-                ''' read the first line '''
-                line = file.readline( ).decode( ) 
-                ''' if the first line of the file contains a comment line, read all comment lines and a description line following the comments. '''
-                if line[ 0 ] == '%' :
+        with gzip.open(
+            f"{path_folder_mtx_10x_output}matrix.mtx.gz.{index_mtx_10x}.gz", "wb"
+        ) as newfile:
+            with gzip.open(path_file_mtx_10x, "rb") as file:
+                """read the first line"""
+                line = file.readline().decode()
+                """ if the first line of the file contains a comment line, read all comment lines and a description line following the comments. """
+                if len(line) > 0 and line[0] == "%":
                     # read comment and the description line
-                    while True :
-                        if line[ 0 ] != '%' :
+                    while True:
+                        if line[0] != "%":
                             break
-                        line = file.readline( ).decode( ) # read the next line
+                        line = file.readline().decode()  # read the next line
                     # process the description line
-                    int_num_rows, int_num_columns, int_num_entries = tuple( int( e ) for e in line.strip( ).split( ) ) # retrieve the number of rows, number of columns and number of entries
-                    line = file.readline( ).decode( ) # read the next line
-                ''' process entries'''
-                while True :
-                    if len( line ) == 0 :
+                    int_num_rows, int_num_columns, int_num_entries = tuple(
+                        int(e) for e in line.strip().split()
+                    )  # retrieve the number of rows, number of columns and number of entries
+                    line = file.readline().decode()  # read the next line
+                """ process entries"""
+                while True:
+                    if len(line) == 0:
                         break
-                    id_row, id_column, int_value = tuple( map( int, line.strip( ).split( ) ) ) # parse each entry of the current matrix 
-                    ''' 1-based > 0-based coordinates '''
+                    id_row, id_column, int_value = tuple(
+                        int(float(e)) for e in line.strip().split()
+                    )  # parse each entry of the current matrix
+                    """ 1-based > 0-based coordinates """
                     id_row -= 1
                     id_column -= 1
-                    ''' write a record to the new matrix file only when both id_row and id_column belongs to filtered id_rows and id_columns '''
-                    if id_row in dict_id_row_previous_to_id_row_current and id_column in dict_id_column_previous_to_id_column_current :
-                        newfile.write( ( ' '.join( tuple( map( str, [ dict_id_row_previous_to_id_row_current[ id_row ] + 1, dict_id_column_previous_to_id_column_current[ id_column ] + 1, int_value ] ) ) ) + '\n' ).encode( ) ) # map id_row and id_column of the previous matrix to those of the filtered matrix (new matrix) # 0-based > 1-based coordinates
-                        int_n_entries += 1 # update the total number of entries written by the current process
-                    line = file.readline( ).decode( ) # read the next line
-    return int_n_entries # returns the total number of entries written by the current process
-def MTX_10X_Filter( path_folder_mtx_10x_input, path_folder_mtx_10x_output, min_counts = None, min_features = None, min_cells = None, l_features = None, l_cells = None, verbose = False, function_for_adjusting_thresholds = None, int_num_threads = 15, flag_split_mtx = True, int_max_num_entries_for_chunk = 10000000 ) :
-    ''' # 2022-02-22 01:39:45  hyunsu-an
+                    """ write a record to the new matrix file only when both id_row and id_column belongs to filtered id_rows and id_columns """
+                    if (
+                        id_row in dict_id_row_previous_to_id_row_current
+                        and id_column in dict_id_column_previous_to_id_column_current
+                    ):
+                        newfile.write(
+                            (
+                                " ".join(
+                                    tuple(
+                                        map(
+                                            str,
+                                            [
+                                                dict_id_row_previous_to_id_row_current[
+                                                    id_row
+                                                ]
+                                                + 1,
+                                                dict_id_column_previous_to_id_column_current[
+                                                    id_column
+                                                ]
+                                                + 1,
+                                                int_value,
+                                            ],
+                                        )
+                                    )
+                                )
+                                + "\n"
+                            ).encode()
+                        )  # map id_row and id_column of the previous matrix to those of the filtered matrix (new matrix) # 0-based > 1-based coordinates
+                        int_n_entries += 1  # update the total number of entries written by the current process
+                    line = file.readline().decode()  # read the next line
+    return int_n_entries  # returns the total number of entries written by the current process
+
+
+def MTX_10X_Filter(
+    path_folder_mtx_10x_input,
+    path_folder_mtx_10x_output,
+    min_counts=None,
+    min_features=None,
+    min_cells=None,
+    l_features=None,
+    l_cells=None,
+    verbose=False,
+    function_for_adjusting_thresholds=None,
+    int_num_threads=15,
+    flag_split_mtx=True,
+    int_max_num_entries_for_chunk=10000000,
+):
+    """# 2022-08-20 10:23:28
+    # hyunsu-an
     read 10x count matrix and filter matrix based on several thresholds
     'path_folder_mtx_10x_input' : a folder containing files for the input 10x count matrix
     'path_folder_mtx_10x_output' : a folder containing files for the input 10x count matrix
 
     Only the threshold arguments for either cells ( 'min_counts', 'min_features' ) or features ( 'min_cells' ) can be given at a time.
 
     'min_counts' : the minimum number of total counts for a cell to be included in the output matrix
     'min_features' : the minimum number of features for a cell to be included in the output matrix
     'min_cells' : the minimum number of cells for a feature to be included in the output matrix
     'l_features' : a list of features (values in the first column of 'features.tsv.gz') to include. All other features will be excluded from the output matrix. (default: None) If None is given, include all features in the output matrix.
     'l_cells' : a list of cells (values in the first column of 'barcodes.tsv.gz') to include. All other cells will be excluded from the output matrix. (default: None) If None is given, include all cells in the output matrix.
     'int_num_threads' : when 'int_num_threads' is 1, does not use the multiprocessing  module for parallel processing
-    'function_for_adjusting_thresholds' : a function for adjusting thresholds based on the summarized metrics. Useful when the exact threshold for removing empty droplets are variable across the samples. the function should receive arguments and return values in the following structure: 
+    'function_for_adjusting_thresholds' : a function for adjusting thresholds based on the summarized metrics. Useful when the exact threshold for removing empty droplets are variable across the samples. the function should receive arguments and return values in the following structure:
                                         min_counts_new, min_features_new, min_cells_new = function_for_adjusting_thresholds( path_folder_mtx_10x_output, min_counts, min_features, min_cells )
-    '''
+    """
 
-    ''' handle inputs '''
-    if path_folder_mtx_10x_input[ -1 ] != '/' :
-        path_folder_mtx_10x_input += '/'
-    if path_folder_mtx_10x_output[ -1 ] != '/' :
-        path_folder_mtx_10x_output += '/'
-    if ( ( min_counts is not None ) or ( min_features is not None ) ) and ( min_cells is not None ) : # check whether thresholds for both cells and features were given (thresdholds for either cells or features can be given at a time)
-        if verbose :
-            print( '[MTX_10X_Filter] (error) no threshold is given or more thresholds for both cells and features are given. (Thresdholds for either cells or features can be given at a time.)' )
+    """ handle inputs """
+    if path_folder_mtx_10x_input[-1] != "/":
+        path_folder_mtx_10x_input += "/"
+    if path_folder_mtx_10x_output[-1] != "/":
+        path_folder_mtx_10x_output += "/"
+    if ((min_counts is not None) or (min_features is not None)) and (
+        min_cells is not None
+    ):  # check whether thresholds for both cells and features were given (thresdholds for either cells or features can be given at a time)
+        if verbose:
+            logger.info(
+                "[MTX_10X_Filter] (error) no threshold is given or more thresholds for both cells and features are given. (Thresdholds for either cells or features can be given at a time.)"
+            )
         return -1
     # create an output folder
-    os.makedirs( path_folder_mtx_10x_output, exist_ok = True )
+    filesystem_operations("mkdir", path_folder_mtx_10x_output, exist_ok=True)
 
     # define input file directories
-    path_file_input_bc = f'{path_folder_mtx_10x_input}barcodes.tsv.gz'
-    path_file_input_feature = f'{path_folder_mtx_10x_input}features.tsv.gz'
-    path_file_input_mtx = f'{path_folder_mtx_10x_input}matrix.mtx.gz'
+    path_file_input_bc = f"{path_folder_mtx_10x_input}barcodes.tsv.gz"
+    path_file_input_feature = f"{path_folder_mtx_10x_input}features.tsv.gz"
+    path_file_input_mtx = f"{path_folder_mtx_10x_input}matrix.mtx.gz"
 
     # check whether all required files are present
-    if sum( list( not os.path.exists( path_folder ) for path_folder in [ path_file_input_bc, path_file_input_feature, path_file_input_mtx ] ) ) :
-        if verbose :
-            print( f'required file(s) is not present at {path_folder_mtx_10x}' )
-
-    ''' read barcode and feature information '''
-    df_bc = pd.read_csv( path_file_input_bc, sep = '\t', header = None )
-    df_bc.columns = [ 'barcode' ]
-    df_feature = pd.read_csv( path_file_input_feature, sep = '\t', header = None )
-    df_feature.columns = [ 'id_feature', 'feature', 'feature_type' ]
-
-    ''' split input mtx file into multiple files '''
-    l_path_file_mtx_10x = MTX_10X_Split( path_folder_mtx_10x_input, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk, flag_split_mtx = flag_split_mtx )
-    
-    ''' summarizes counts '''
-    dict_data = MTX_10X_Summarize_Counts( path_folder_mtx_10x_input, verbose = verbose, int_num_threads = int_num_threads, flag_split_mtx = flag_split_mtx, int_max_num_entries_for_chunk = int_max_num_entries_for_chunk )
-    dict_id_column_to_count, dict_id_column_to_n_features, dict_id_row_to_count, dict_id_row_to_n_cells, dict_id_row_to_log_transformed_count = dict_data[ 'dict_id_column_to_count' ], dict_data[ 'dict_id_column_to_n_features' ], dict_data[ 'dict_id_row_to_count' ], dict_data[ 'dict_id_row_to_n_cells' ], dict_data[ 'dict_id_row_to_log_transformed_count' ] # parse 'dict_data'
-    
-    ''' adjust thresholds based on the summarized metrices (if a function has been given) '''
-    if function_for_adjusting_thresholds is not None :
-        min_counts, min_features, min_cells = function_for_adjusting_thresholds( path_folder_mtx_10x_input, min_counts, min_features, min_cells )
-    
-    ''' filter row or column that do not satisfy the given thresholds '''
-    if min_counts is not None :
-        dict_id_column_to_count = dict( ( k, dict_id_column_to_count[ k ] ) for k in dict_id_column_to_count if dict_id_column_to_count[ k ] >= min_counts ) 
-    if min_features is not None :
-        dict_id_column_to_n_features = dict( ( k, dict_id_column_to_n_features[ k ] ) for k in dict_id_column_to_n_features if dict_id_column_to_n_features[ k ] >= min_features )
-    if min_cells is not None :
-        dict_id_row_to_n_cells = dict( ( k, dict_id_row_to_n_cells[ k ] ) for k in dict_id_row_to_n_cells if dict_id_row_to_n_cells[ k ] >= min_cells )
-
-    ''' retrieve id_row and id_column that satisfy the given thresholds '''    
-    set_id_column = set( dict_id_column_to_count ).intersection( set( dict_id_column_to_n_features ) )
-    set_id_row = set( dict_id_row_to_n_cells )
-    
-    ''' exclude cells and features not present in the input lists (if the lists were given)  '''
-    if l_cells is not None :        
-        dict_barcode_to_id_column = dict( ( barcode, id_column ) for id_column, barcode in enumerate( df_bc.barcode.values ) )
-        set_id_column = set_id_column.intersection( set( dict_barcode_to_id_column[ barcode ] for barcode in set( l_cells ) if barcode in dict_barcode_to_id_column ) )
+    if sum(
+        list(
+            not filesystem_operations("exists", path_folder)
+            for path_folder in [
+                path_file_input_bc,
+                path_file_input_feature,
+                path_file_input_mtx,
+            ]
+        )
+    ):
+        if verbose:
+            logger.info(f"required file(s) is not present at {path_folder_mtx_10x}")
+
+    """ read barcode and feature information """
+    df_bc = pd.read_csv(path_file_input_bc, sep="\t", header=None)
+    df_bc.columns = ["barcode"]
+    df_feature = pd.read_csv(path_file_input_feature, sep="\t", header=None)
+    df_feature.columns = ["id_feature", "feature", "feature_type"]
+
+    """ split input mtx file into multiple files """
+    l_path_file_mtx_10x = MTX_10X_Split(
+        path_folder_mtx_10x_input,
+        int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+        flag_split_mtx=flag_split_mtx,
+    )
+
+    """ summarizes counts """
+    dict_data = MTX_10X_Summarize_Counts(
+        path_folder_mtx_10x_input,
+        verbose=verbose,
+        int_num_threads=int_num_threads,
+        flag_split_mtx=flag_split_mtx,
+        int_max_num_entries_for_chunk=int_max_num_entries_for_chunk,
+    )
+    (
+        dict_id_column_to_count,
+        dict_id_column_to_n_features,
+        dict_id_row_to_count,
+        dict_id_row_to_n_cells,
+        dict_id_row_to_log_transformed_count,
+    ) = (
+        dict_data["dict_id_column_to_count"],
+        dict_data["dict_id_column_to_n_features"],
+        dict_data["dict_id_row_to_count"],
+        dict_data["dict_id_row_to_n_cells"],
+        dict_data["dict_id_row_to_log_transformed_count"],
+    )  # parse 'dict_data'
+
+    """ adjust thresholds based on the summarized metrices (if a function has been given) """
+    if function_for_adjusting_thresholds is not None:
+        min_counts, min_features, min_cells = function_for_adjusting_thresholds(
+            path_folder_mtx_10x_input, min_counts, min_features, min_cells
+        )
+
+    """ filter row or column that do not satisfy the given thresholds """
+    if min_counts is not None:
+        dict_id_column_to_count = dict(
+            (k, dict_id_column_to_count[k])
+            for k in dict_id_column_to_count
+            if dict_id_column_to_count[k] >= min_counts
+        )
+    if min_features is not None:
+        dict_id_column_to_n_features = dict(
+            (k, dict_id_column_to_n_features[k])
+            for k in dict_id_column_to_n_features
+            if dict_id_column_to_n_features[k] >= min_features
+        )
+    if min_cells is not None:
+        dict_id_row_to_n_cells = dict(
+            (k, dict_id_row_to_n_cells[k])
+            for k in dict_id_row_to_n_cells
+            if dict_id_row_to_n_cells[k] >= min_cells
+        )
+
+    """ retrieve id_row and id_column that satisfy the given thresholds """
+    set_id_column = set(dict_id_column_to_count).intersection(
+        set(dict_id_column_to_n_features)
+    )
+    set_id_row = set(dict_id_row_to_n_cells)
+
+    """ exclude cells and features not present in the input lists (if the lists were given)  """
+    if l_cells is not None:
+        dict_barcode_to_id_column = dict(
+            (barcode, id_column)
+            for id_column, barcode in enumerate(df_bc.barcode.values)
+        )
+        set_id_column = set_id_column.intersection(
+            set(
+                dict_barcode_to_id_column[barcode]
+                for barcode in set(l_cells)
+                if barcode in dict_barcode_to_id_column
+            )
+        )
         del dict_barcode_to_id_column
-    if l_features is not None :
-        dict_id_feature_to_id_row = dict( ( id_feature, id_row ) for id_row, id_feature in enumerate( df_feature.id_feature.values ) )
-        set_id_row = set_id_row.intersection( set( dict_id_feature_to_id_row[ id_feature ] for id_feature in set( l_features ) if id_feature in dict_id_feature_to_id_row ) )
+    if l_features is not None:
+        dict_id_feature_to_id_row = dict(
+            (id_feature, id_row)
+            for id_row, id_feature in enumerate(df_feature.id_feature.values)
+        )
+        set_id_row = set_id_row.intersection(
+            set(
+                dict_id_feature_to_id_row[id_feature]
+                for id_feature in set(l_features)
+                if id_feature in dict_id_feature_to_id_row
+            )
+        )
         del dict_id_feature_to_id_row
 
-    ''' report the number of cells or features that will be filtered out '''
-    if verbose :
-        int_n_bc_filtered = len( df_bc ) - len( set_id_column )
-        if int_n_bc_filtered > 0 :
-            print( f"{int_n_bc_filtered}/{len( df_bc )} barcodes will be filtered out" )
-        int_n_feature_filtered = len( df_feature ) - len( set_id_row )
-        if int_n_feature_filtered > 0 :
-            print( f"{int_n_feature_filtered}/{len( df_feature )} features will be filtered out" )
+    """ report the number of cells or features that will be filtered out """
+    if verbose:
+        int_n_bc_filtered = len(df_bc) - len(set_id_column)
+        if int_n_bc_filtered > 0:
+            logger.info(
+                f"{int_n_bc_filtered}/{len( df_bc )} barcodes will be filtered out"
+            )
+        int_n_feature_filtered = len(df_feature) - len(set_id_row)
+        if int_n_feature_filtered > 0:
+            logger.info(
+                f"{int_n_feature_filtered}/{len( df_feature )} features will be filtered out"
+            )
 
     """ retrieve a mapping between previous id_column to current id_column """
-    global dict_id_column_previous_to_id_column_current, dict_id_row_previous_to_id_row_current # use global variables for multiprocessing
-    df_bc = df_bc.loc[ list( set_id_column ) ]
-    df_bc.index.name = 'id_column_previous'
-    df_bc.reset_index( drop = False, inplace = True )
-    df_bc[ 'id_column_current' ] = np.arange( len( df_bc ) )
-    dict_id_column_previous_to_id_column_current = df_bc.set_index( 'id_column_previous' ).id_column_current.to_dict( ) 
-    PICKLE_Write( f'{path_folder_mtx_10x_output}dict_id_column_previous_to_id_column_current.pickle', dict_id_column_previous_to_id_column_current ) # save id_feature to index_feature mapping 
+    global dict_id_column_previous_to_id_column_current, dict_id_row_previous_to_id_row_current  # use global variables for multiprocessing
+    df_bc = df_bc.loc[list(set_id_column)]
+    df_bc.index.name = "id_column_previous"
+    df_bc.reset_index(drop=False, inplace=True)
+    df_bc["id_column_current"] = np.arange(len(df_bc))
+    dict_id_column_previous_to_id_column_current = df_bc.set_index(
+        "id_column_previous"
+    ).id_column_current.to_dict()
+    bk.PICKLE_Write(
+        f"{path_folder_mtx_10x_output}dict_id_column_previous_to_id_column_current.pickle",
+        dict_id_column_previous_to_id_column_current,
+    )  # save id_feature to index_feature mapping
     """ retrieve a mapping between previous id_row to current id_row """
-    df_feature = df_feature.loc[ list( set_id_row ) ]
-    df_feature.index.name = 'id_row_previous'
-    df_feature.reset_index( drop = False, inplace = True )
-    df_feature[ 'id_row_current' ] = np.arange( len( df_feature ) )
-    dict_id_row_previous_to_id_row_current = df_feature.set_index( 'id_row_previous' ).id_row_current.to_dict( ) 
-    PICKLE_Write( f'{path_folder_mtx_10x_output}dict_id_row_previous_to_id_row_current.pickle', dict_id_row_previous_to_id_row_current ) # save id_feature to index_feature mapping 
-
-    ''' save barcode file '''
-    df_bc.to_csv( f"{path_folder_mtx_10x_output}barcodes.tsv.gz", columns = [ 'barcode' ], sep = '\t', index = False, header = False ) 
-
-    ''' save feature file '''
-    df_feature[ [ 'id_feature', 'feature', 'feature_type' ] ].to_csv( f"{path_folder_mtx_10x_output}features.tsv.gz", sep = '\t', index = False, header = False ) # save as a file
+    df_feature = df_feature.loc[list(set_id_row)]
+    df_feature.index.name = "id_row_previous"
+    df_feature.reset_index(drop=False, inplace=True)
+    df_feature["id_row_current"] = np.arange(len(df_feature))
+    dict_id_row_previous_to_id_row_current = df_feature.set_index(
+        "id_row_previous"
+    ).id_row_current.to_dict()
+    bk.PICKLE_Write(
+        f"{path_folder_mtx_10x_output}dict_id_row_previous_to_id_row_current.pickle",
+        dict_id_row_previous_to_id_row_current,
+    )  # save id_feature to index_feature mapping
+
+    """ save barcode file """
+    df_bc.to_csv(
+        f"{path_folder_mtx_10x_output}barcodes.tsv.gz",
+        columns=["barcode"],
+        sep="\t",
+        index=False,
+        header=False,
+    )
+    del df_bc
+
+    """ save feature file """
+    df_feature[["id_feature", "feature", "feature_type"]].to_csv(
+        f"{path_folder_mtx_10x_output}features.tsv.gz",
+        sep="\t",
+        index=False,
+        header=False,
+    )  # save as a file
+    del df_feature
 
     """ write a filtered matrix.mtx.gz for each split mtx file using multiple processes and retrieve the total number of entries written by each process """
     # compose inputs for multiprocessing
-    df_input = pd.DataFrame( { 'path_file_mtx_10x' : l_path_file_mtx_10x, 'index_mtx_10x' : np.arange( len( l_path_file_mtx_10x ) ) } )
-    l_int_n_entries = Multiprocessing( df_input, __MTX_10X_Filter__filter_mtx_10x__, int_num_threads, global_arguments = [ path_folder_mtx_10x_output ] ) 
+    df_input = pd.DataFrame(
+        {
+            "path_file_mtx_10x": l_path_file_mtx_10x,
+            "index_mtx_10x": np.arange(len(l_path_file_mtx_10x)),
+        }
+    )
+    l_int_n_entries = bk.Multiprocessing(
+        df_input,
+        __MTX_10X_Filter__filter_mtx_10x__,
+        int_num_threads,
+        global_arguments=[path_folder_mtx_10x_output],
+    )
     # retrieve the total number of entries
-    int_total_n_entries = sum( l_int_n_entries )
-    
+    int_total_n_entries = sum(l_int_n_entries)
+
     """ combine parts and add the MTX file header to compose a combined mtx file """
-    df_file = GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz" )
-    df_file.wildcard_0 = df_file.wildcard_0.astype( int )
-    df_file.sort_values( 'wildcard_0', inplace = True )
-    OS_FILE_Combine_Files_in_order( df_file.path.values, f"{path_folder_mtx_10x_output}matrix.mtx.gz", delete_input_files = not flag_split_mtx, header = f"%%MatrixMarket matrix coordinate integer general\n%\n{len( dict_id_row_previous_to_id_row_current )} {len( dict_id_column_previous_to_id_column_current )} {int_total_n_entries}\n" ) # combine the output mtx files in the order # does not delete temporary files if 'flag_split_mtx' is True
-    
+    df_file = bk.GLOB_Retrive_Strings_in_Wildcards(
+        f"{path_folder_mtx_10x_output}matrix.mtx.gz.*.gz"
+    )
+    df_file.wildcard_0 = df_file.wildcard_0.astype(int)
+    df_file.sort_values("wildcard_0", inplace=True)
+
+    # write header
+    path_file_header = f"{path_folder_mtx_10x_output}matrix.mtx.header.txt.gz"
+    with gzip.open(path_file_header, "wb") as newfile:
+        newfile.write(
+            f"%%MatrixMarket matrix coordinate integer general\n%\n{len( dict_id_row_previous_to_id_row_current )} {len( dict_id_column_previous_to_id_column_current )} {int_total_n_entries}\n".encode()
+        )
+    bk.OS_Run(
+        ["cat", path_file_header] + list(df_file.path.values),
+        path_file_stdout=f"{path_folder_mtx_10x_output}matrix.mtx.gz",
+        stdout_binary=True,
+        return_output=False,
+    )  # combine the output mtx files in the order # does not delete temporary files if 'flag_split_mtx' is True
+
     # write a flag indicating that the current output directory contains split mtx files
-    with open( f"{path_folder_mtx_10x_output}matrix.mtx.gz.split.flag", 'w' ) as file :
-        file.write( 'completed' )
-def MTX_10X_Identify_Highly_Variable_Features( path_folder_mtx_10x_input, int_target_sum = 10000, verbose = False, int_num_threads = 15, flag_split_mtx = True, int_max_num_entries_for_chunk = 10000000 ) :
-    ''' # 2022-03-16 17:18:44 
+    with open(f"{path_folder_mtx_10x_output}matrix.mtx.gz.split.flag", "w") as file:
+        file.write("completed")
+
+
+def MTX_10X_Identify_Highly_Variable_Features(
+    path_folder_mtx_10x_input,
+    int_target_sum=10000,
+    verbose=False,
+    int_num_threads=15,
+    flag_split_mtx=True,
+    int_max_num_entries_for_chunk=10000000,
+):
+    """# 2022-03-16 17:18:44
     calculate variance from log-transformed normalized counts using 'MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr' and rank features based on how each feature is variable compared to other features with similar means.
-    Specifically, polynomial of degree 2 will be fitted to variance-mean relationship graph in order to captures the relationship between variance and mean. 
-    
+    Specifically, polynomial of degree 2 will be fitted to variance-mean relationship graph in order to captures the relationship between variance and mean.
+
     'name_col_for_mean', 'name_col_for_variance' : name of columns of 'df_summary' returned by 'MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr' that will be used to infer highly variable features. By defaults, mean and variance of log-transformed normalized counts will be used.
-    '''
-    
+    """
+
     # calculate variance and means and load the result
-    df_summary = MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr( path_folder_mtx_10x_input, int_target_sum = int_target_sum, int_num_threads = int_num_threads, verbose = verbose, flag_split_mtx = flag_split_mtx )
-    
+    df_summary = MTX_10X_Calculate_Average_Log10_Transformed_Normalized_Expr(
+        path_folder_mtx_10x_input,
+        int_target_sum=int_target_sum,
+        int_num_threads=int_num_threads,
+        verbose=verbose,
+        flag_split_mtx=flag_split_mtx,
+    )
+
     # calculate scores for identifying highly variable features for the selected set of count data types: [ 'log_transformed_normalized_count', 'log_transformed_count' ]
-    for name_type in [ 'log_transformed_normalized_count', 'log_transformed_count' ] :
-        name_col_for_mean, name_col_for_variance = f'mean_{name_type}', f'variance_of_{name_type}'
+    for name_type in ["log_transformed_normalized_count", "log_transformed_count"]:
+        name_col_for_mean, name_col_for_variance = (
+            f"mean_{name_type}",
+            f"variance_of_{name_type}",
+        )
         # retrieve the relationship between mean and variance
-        arr_mean = df_summary[ name_col_for_mean ].values
-        arr_var = df_summary[ name_col_for_variance ].values
-        mean_var_relationship_fit = np.polynomial.polynomial.Polynomial.fit( arr_mean, arr_var, 2 )
+        arr_mean = df_summary[name_col_for_mean].values
+        arr_var = df_summary[name_col_for_variance].values
+        mean_var_relationship_fit = np.polynomial.polynomial.Polynomial.fit(
+            arr_mean, arr_var, 2
+        )
 
         # calculate the deviation from the estimated variance from the mean
-        arr_ratio_of_variance_to_expected_variance_from_mean = np.zeros( len( df_summary ) )
-        arr_diff_of_variance_to_expected_variance_from_mean = np.zeros( len( df_summary ) )
-        for i in range( len( df_summary ) ) : # iterate list of means of the features
-            var, mean = arr_var[ i ], arr_mean[ i ] # retrieve var and mean
-            var_expected = mean_var_relationship_fit( mean ) # calculate expected variance from the mean
-            if var_expected == 0 : # handle the case when the current expected variance is zero 
-                arr_ratio_of_variance_to_expected_variance_from_mean[ i ] = 1
-                arr_diff_of_variance_to_expected_variance_from_mean[ i ] = 0
-            else :
-                arr_ratio_of_variance_to_expected_variance_from_mean[ i ] = var / var_expected
-                arr_diff_of_variance_to_expected_variance_from_mean[ i ] = var - var_expected
-
-        df_summary[ f'float_ratio_of_variance_to_expected_variance_from_mean_from_{name_type}' ] = arr_ratio_of_variance_to_expected_variance_from_mean
-        df_summary[ f'float_diff_of_variance_to_expected_variance_from_mean_{name_type}' ] = arr_diff_of_variance_to_expected_variance_from_mean
+        arr_ratio_of_variance_to_expected_variance_from_mean = np.zeros(len(df_summary))
+        arr_diff_of_variance_to_expected_variance_from_mean = np.zeros(len(df_summary))
+        for i in range(len(df_summary)):  # iterate list of means of the features
+            var, mean = arr_var[i], arr_mean[i]  # retrieve var and mean
+            var_expected = mean_var_relationship_fit(
+                mean
+            )  # calculate expected variance from the mean
+            if (
+                var_expected == 0
+            ):  # handle the case when the current expected variance is zero
+                arr_ratio_of_variance_to_expected_variance_from_mean[i] = 1
+                arr_diff_of_variance_to_expected_variance_from_mean[i] = 0
+            else:
+                arr_ratio_of_variance_to_expected_variance_from_mean[i] = (
+                    var / var_expected
+                )
+                arr_diff_of_variance_to_expected_variance_from_mean[i] = (
+                    var - var_expected
+                )
+
+        df_summary[
+            f"float_ratio_of_variance_to_expected_variance_from_mean_from_{name_type}"
+        ] = arr_ratio_of_variance_to_expected_variance_from_mean
+        df_summary[
+            f"float_diff_of_variance_to_expected_variance_from_mean_{name_type}"
+        ] = arr_diff_of_variance_to_expected_variance_from_mean
 
         # calculate the product of the ratio and difference of variance to expected variance for scoring and sorting highly variable features
-        df_summary[ f'float_score_highly_variable_feature_from_{name_type}' ] = df_summary[ f'float_ratio_of_variance_to_expected_variance_from_mean_from_{name_type}' ] * df_summary[ f'float_diff_of_variance_to_expected_variance_from_mean_{name_type}' ]
-
-    df_summary[ 'float_score_highly_variable_feature' ] = list( np.prod( arr_val ) if sum( np.sign( arr_val ) < 0 ) == 0 else 0 for arr_val in df_summary[ [ 'float_score_highly_variable_feature_from_log_transformed_normalized_count', 'float_score_highly_variable_feature_from_log_transformed_count' ] ].values )
+        df_summary[f"float_score_highly_variable_feature_from_{name_type}"] = (
+            df_summary[
+                f"float_ratio_of_variance_to_expected_variance_from_mean_from_{name_type}"
+            ]
+            * df_summary[
+                f"float_diff_of_variance_to_expected_variance_from_mean_{name_type}"
+            ]
+        )
+
+    df_summary["float_score_highly_variable_feature"] = list(
+        np.prod(arr_val) if sum(np.sign(arr_val) < 0) == 0 else 0
+        for arr_val in df_summary[
+            [
+                "float_score_highly_variable_feature_from_log_transformed_normalized_count",
+                "float_score_highly_variable_feature_from_log_transformed_count",
+            ]
+        ].values
+    )
     return df_summary
 
-''' newly written functions '''
-def is_binary_stream( f ) :
-    ''' # 2022-05-01 01:57:10 
-    check whether a given stream is a binary stream '''
-    if hasattr( f, 'mode' ) : # if given stream is file
-        return 'b' in f.mode
-    else :
-        return isinstance( f, ( io.RawIOBase, io.BufferedIOBase ) ) 
-def __Get_path_essential_files__( path_folder_mtx_10x_input ) :
-    ''' # 2022-04-30 16:28:15 
+
+""" functions that were added later """
+
+
+def is_binary_stream(f):
+    """# 2022-05-01 01:57:10
+    check whether a given stream is a binary stream"""
+    if hasattr(f, "mode"):  # if given stream is file
+        return "b" in f.mode
+    else:
+        return isinstance(f, (io.RawIOBase, io.BufferedIOBase))
+
+
+def __Get_path_essential_files__(path_folder_mtx_10x_input):
+    """# 2022-04-30 16:28:15
     get paths of essential files for the given matrix folder ('path_folder_mtx_10x_input', currently only supports 10X-GEX-formated output matrix)
-    '''
+    """
     # define input file paths
-    path_file_input_bc = f'{path_folder_mtx_10x_input}barcodes.tsv.gz'
-    path_file_input_feature = f'{path_folder_mtx_10x_input}features.tsv.gz'
-    path_file_input_mtx = f'{path_folder_mtx_10x_input}matrix.mtx.gz'
+    path_file_input_bc = f"{path_folder_mtx_10x_input}barcodes.tsv.gz"
+    path_file_input_feature = f"{path_folder_mtx_10x_input}features.tsv.gz"
+    path_file_input_mtx = f"{path_folder_mtx_10x_input}matrix.mtx.gz"
     # check whether input files exist
-    for path_file in [ path_file_input_bc, path_file_input_feature, path_file_input_mtx ] :
-        if not os.path.exists( path_file ) :
-            raise OSError( f'{path_file} does not exist' )
-    return path_file_input_bc, path_file_input_feature, path_file_input_mtx 
-def Merge_Sort_Files( file_output, * l_iterator_decorated_file_input ) :
-    """ # 2022-05-01 02:23:09 
+    for path_file in [path_file_input_bc, path_file_input_feature, path_file_input_mtx]:
+        if not os.path.exists(path_file):
+            raise OSError(f"{path_file} does not exist")
+    return path_file_input_bc, path_file_input_feature, path_file_input_mtx
+
+
+def Merge_Sort_Files(file_output, *l_iterator_decorated_file_input):
+    """# 2022-05-01 02:23:09
     Merge sort input files (should be sorted) without loading the complete contents on memory.
     'path_file_output' : output file handle/stream
     'l_iterator_decorated_file_input' : a list of iterators based on input file handles (or streams). each iterator should yield the following tuple: (key_for_sorting, content_that_will_be_written_in_the_output_file). This function does not check whether the datatype of the 'content_that_will_be_written_in_the_output_file' matches that of 'path_file_output'
     """
     # handle invalid case
-    if len( l_iterator_decorated_file_input ) == 0 :
-        return - 1
+    if len(l_iterator_decorated_file_input) == 0:
+        return -1
     # perform merge sorting
-    for r in heapq.merge( * l_iterator_decorated_file_input ) :
-        file_output.write( r[ 1 ] ) # assumes the 'iterator_decorated_file_input' returns appropriate datatype (either bytes or string) for the output file
-def __Merge_Sort_MTX_10X__( path_file_output, * l_path_file_input, flag_ramtx_sorted_by_id_feature = True, flag_delete_input_file_upon_completion = False ) :
-    """ # 2022-05-01 02:25:07 
-    merge sort mtx files 
+    for r in heapq.merge(*l_iterator_decorated_file_input):
+        file_output.write(
+            r[1]
+        )  # assumes the 'iterator_decorated_file_input' returns appropriate datatype (either bytes or string) for the output file
+
+
+def __Merge_Sort_MTX_10X__(
+    path_file_output,
+    *l_path_file_input,
+    flag_ramtx_sorted_by_id_feature=True,
+    flag_delete_input_file_upon_completion=False,
+):
+    """# 2022-05-01 02:25:07
+    merge sort mtx files
     'path_file_output' and 'l_path_file_input'  : either file path or file handles
-    
+
     'flag_ramtx_sorted_by_id_feature' : if True, sort by 'id_feature'. if False, sort by 'id_cell'
     """
     # process arguments for input files
-    if isinstance( l_path_file_input[ 0 ], str ) : # if paths are given as input files
-        flag_input_binary = l_path_file_input[ 0 ].rsplit( '.', 1 )[ 1 ].lower( ) == 'gz' # automatically detect gzipped input file # determined gzipped status by only looking at the first file
-        l_file_input = list( gzip.open( path_file, 'rb' ) if flag_input_binary else open( path_file, 'r' ) for path_file in l_path_file_input )
-    else :
-        flag_input_binary = is_binary_stream( l_file_input[ 0 ] ) # detect binary stream 
+    if isinstance(l_path_file_input[0], str):  # if paths are given as input files
+        flag_input_binary = (
+            l_path_file_input[0].rsplit(".", 1)[1].lower() == "gz"
+        )  # automatically detect gzipped input file # determined gzipped status by only looking at the first file
+        l_file_input = list(
+            gzip.open(path_file, "rb") if flag_input_binary else open(path_file, "r")
+            for path_file in l_path_file_input
+        )
+    else:
+        flag_input_binary = is_binary_stream(l_file_input[0])  # detect binary stream
         l_file_input = l_path_file_input
     # process argument for output file
-    if isinstance( path_file_output, str ) : # if path was given as an output file
+    if isinstance(path_file_output, str):  # if path was given as an output file
         flag_output_is_file = True
-        flag_output_binary = path_file_output.rsplit( '.', 1 )[ 1 ].lower( ) == 'gz' # automatically detect gzipped input file # determined gzipped status by only looking at the first file
-        file_output = gzip.open( path_file_output, 'wb' ) if flag_output_binary else open( path_file_output, 'w' )
-    else :
+        flag_output_binary = (
+            path_file_output.rsplit(".", 1)[1].lower() == "gz"
+        )  # automatically detect gzipped input file # determined gzipped status by only looking at the first file
+        file_output = (
+            gzip.open(path_file_output, "wb")
+            if flag_output_binary
+            else open(path_file_output, "w")
+        )
+    else:
         flag_output_is_file = False
-        flag_output_binary = is_binary_stream( path_file_output ) # detect binary stream 
+        flag_output_binary = is_binary_stream(path_file_output)  # detect binary stream
         file_output = path_file_output
     # define a function for decorating mtx record
-    def __decorate_mtx_file__( file ) :
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 :
+    def __decorate_mtx_file__(file):
+        while True:
+            line = file.readline()
+            if len(line) == 0:
                 break
-            ''' parse a mtx record '''
-            line_decoded = line.decode( ) if flag_input_binary else line
-            index_row, index_column, float_value = ( line_decoded ).strip( ).split( ) # parse a record of a matrix-market format file
-            index_row, index_column, float_value = int( index_row ), int( index_column ), float( float_value ) # 0-based coordinates
-            yield index_row if flag_ramtx_sorted_by_id_feature else index_column, ( line if flag_input_binary else line.encode( ) ) if flag_output_binary else line_decoded
-    
-    Merge_Sort_Files( file_output, * list( __decorate_mtx_file__( file ) for file in l_file_input ) ) # perform merge sorting
-    
+            """ parse a mtx record """
+            line_decoded = line.decode() if flag_input_binary else line
+            index_row, index_column, float_value = (
+                (line_decoded).strip().split()
+            )  # parse a record of a matrix-market format file
+            index_row, index_column, float_value = (
+                int(index_row),
+                int(index_column),
+                float(float_value),
+            )  # 0-based coordinates
+            yield index_row if flag_ramtx_sorted_by_id_feature else index_column, (
+                line if flag_input_binary else line.encode()
+            ) if flag_output_binary else line_decoded
+
+    Merge_Sort_Files(
+        file_output, *list(__decorate_mtx_file__(file) for file in l_file_input)
+    )  # perform merge sorting
+
     # if the output file is stream, does not close the stream # only close the output if the output file was an actual file
-    if flag_output_is_file :
-        file_output.close( )
-    
-    ''' delete input files once merge sort is completed if 'flag_delete_input_file_upon_completion' is True '''
-    if flag_delete_input_file_upon_completion and isinstance( l_path_file_input[ 0 ], str ) : # if paths are given as input files
-        for path_file in l_path_file_input :
-            os.remove( path_file )
-def __Merge_Sort_and_Index_MTX_10X__( path_file_output, * l_path_file_input, flag_ramtx_sorted_by_id_feature = True, flag_delete_input_file_upon_completion = False ) :
-    """ # 2022-05-01 02:25:07 
+    if flag_output_is_file:
+        file_output.close()
+
+    """ delete input files once merge sort is completed if 'flag_delete_input_file_upon_completion' is True """
+    if flag_delete_input_file_upon_completion and isinstance(
+        l_path_file_input[0], str
+    ):  # if paths are given as input files
+        for path_file in l_path_file_input:
+            os.remove(path_file)
+
+
+def __Merge_Sort_and_Index_MTX_10X__(
+    path_file_output,
+    *l_path_file_input,
+    flag_ramtx_sorted_by_id_feature=True,
+    flag_delete_input_file_upon_completion=False,
+):
+    """# 2022-05-01 02:25:07
     merge sort mtx files into a single mtx uncompressed file and index entries in the combined mtx file while writing the file
     'path_file_output' : should be a file path, file handle (or stream) for non-binary (text) output
-    'l_path_file_input' 
-    
+    'l_path_file_input'
+
     'flag_ramtx_sorted_by_id_feature' : if True, sort by 'id_feature'. if False, sort by 'id_cell'
     """
     # process arguments for input files
-    if isinstance( l_path_file_input[ 0 ], str ) : # if paths are given as input files
-        flag_input_binary = l_path_file_input[ 0 ].rsplit( '.', 1 )[ 1 ].lower( ) == 'gz' # automatically detect gzipped input file # determined gzipped status by only looking at the first file
-        l_file_input = list( gzip.open( path_file, 'rb' ) if flag_input_binary else open( path_file, 'r' ) for path_file in l_path_file_input )
-    else :
-        flag_input_binary = is_binary_stream( l_file_input[ 0 ] ) # detect binary stream 
+    if isinstance(l_path_file_input[0], str):  # if paths are given as input files
+        flag_input_binary = (
+            l_path_file_input[0].rsplit(".", 1)[1].lower() == "gz"
+        )  # automatically detect gzipped input file # determined gzipped status by only looking at the first file
+        l_file_input = list(
+            gzip.open(path_file, "rb") if flag_input_binary else open(path_file, "r")
+            for path_file in l_path_file_input
+        )
+    else:
+        flag_input_binary = is_binary_stream(l_file_input[0])  # detect binary stream
         l_file_input = l_path_file_input
     # process argument for output file
-    if isinstance( path_file_output, str ) : # if path was given as an output file
+    if isinstance(path_file_output, str):  # if path was given as an output file
         flag_output_is_file = True
-        flag_output_binary = path_file_output.rsplit( '.', 1 )[ 1 ].lower( ) == 'gz' # automatically detect gzipped input file # determined gzipped status by only looking at the first file
-        file_output = gzip.open( path_file_output, 'wb' ) if flag_output_binary else open( path_file_output, 'w' )
-    else :
+        flag_output_binary = (
+            path_file_output.rsplit(".", 1)[1].lower() == "gz"
+        )  # automatically detect gzipped input file # determined gzipped status by only looking at the first file
+        file_output = (
+            gzip.open(path_file_output, "wb")
+            if flag_output_binary
+            else open(path_file_output, "w")
+        )
+    else:
         flag_output_is_file = False
-        flag_output_binary = is_binary_stream( path_file_output ) # detect binary stream 
+        flag_output_binary = is_binary_stream(path_file_output)  # detect binary stream
         file_output = path_file_output
-        
-    if flag_output_binary : # the output file should be non-binary stream/file
-        raise OSError( 'the output file should be non-binary stream/file' )
+
+    if flag_output_binary:  # the output file should be non-binary stream/file
+        raise OSError("the output file should be non-binary stream/file")
 
     # define and open index output file
     path_file_index_output = f"{path_file_output}.idx.tsv.gz"
-    file_index_output = gzip.open( path_file_index_output, 'wb' )
-    file_index_output.write( ( '\t'.join( [ 'index_entry', 'int_pos_start', 'int_pos_end' ] ) + '\n' ).encode( ) ) # write the header of the index file
-        
+    file_index_output = gzip.open(path_file_index_output, "wb")
+    file_index_output.write(
+        ("\t".join(["index_entry", "int_pos_start", "int_pos_end"]) + "\n").encode()
+    )  # write the header of the index file
+
     # define a function for decorating mtx record
-    def __decorate_mtx_file__( file ) :
-        while True :
-            line = file.readline( )
-            if len( line ) == 0 :
+    def __decorate_mtx_file__(file):
+        while True:
+            line = file.readline()
+            if len(line) == 0:
                 break
-            ''' parse a mtx record '''
-            line_decoded = line.decode( ) if flag_input_binary else line
-            index_row, index_column, float_value = ( line_decoded ).strip( ).split( ) # parse a record of a matrix-market format file
-            index_row, index_column, float_value = int( index_row ), int( index_column ), float( float_value ) # 0-based coordinates
-            yield index_row if flag_ramtx_sorted_by_id_feature else index_column, ( line if flag_input_binary else line.encode( ) ) if flag_output_binary else line_decoded
+            """ parse a mtx record """
+            line_decoded = line.decode() if flag_input_binary else line
+            index_row, index_column, float_value = (
+                (line_decoded).strip().split()
+            )  # parse a record of a matrix-market format file
+            index_row, index_column, float_value = (
+                int(index_row),
+                int(index_column),
+                float(float_value),
+            )  # 0-based coordinates
+            yield index_row if flag_ramtx_sorted_by_id_feature else index_column, (
+                line if flag_input_binary else line.encode()
+            ) if flag_output_binary else line_decoded
 
     # perform merge sorting
     index_entry_currently_being_written = -1
     int_num_character_written_for_index_entry_currently_being_written = 0
     int_total_num_character_written = 0
-    for r in heapq.merge( * list( __decorate_mtx_file__( file ) for file in l_file_input ) ) :
-        if index_entry_currently_being_written != r[ 0 ] : # if current index_entry is different from the previous one, which mark the change of sorted blocks (a block has the same id_entry), record the data for the previous block and initialze data for the next block 
-            if index_entry_currently_being_written > 0 : # check whether 'index_entry_currently_being_written' is valid (ignore 'dummy' or default value that was used for initialization)
-                file_index_output.write( ( '\t'.join( map( str, [ index_entry_currently_being_written, int_total_num_character_written, int_total_num_character_written + int_num_character_written_for_index_entry_currently_being_written ] ) ) + '\n' ).encode( ) ) # write information required for indexing
-            int_total_num_character_written += int_num_character_written_for_index_entry_currently_being_written # update 'int_total_num_character_written'
+    for r in heapq.merge(*list(__decorate_mtx_file__(file) for file in l_file_input)):
+        if (
+            index_entry_currently_being_written != r[0]
+        ):  # if current index_entry is different from the previous one, which mark the change of sorted blocks (a block has the same id_entry), record the data for the previous block and initialze data for the next block
+            if (
+                index_entry_currently_being_written > 0
+            ):  # check whether 'index_entry_currently_being_written' is valid (ignore 'dummy' or default value that was used for initialization)
+                file_index_output.write(
+                    (
+                        "\t".join(
+                            map(
+                                str,
+                                [
+                                    index_entry_currently_being_written,
+                                    int_total_num_character_written,
+                                    int_total_num_character_written
+                                    + int_num_character_written_for_index_entry_currently_being_written,
+                                ],
+                            )
+                        )
+                        + "\n"
+                    ).encode()
+                )  # write information required for indexing
+            int_total_num_character_written += int_num_character_written_for_index_entry_currently_being_written  # update 'int_total_num_character_written'
             # initialize data for index of the next 'index_entry'
-            index_entry_currently_being_written = r[ 0 ] # update current index_entry
-            int_num_character_written_for_index_entry_currently_being_written = 0 # reset the count of characters (which is equal to the number of bytes for any mtx records, because they only contains numeric characters)
-        int_num_character_written_for_index_entry_currently_being_written += file_output.write( r[ 1 ] ) # assumes the 'iterator_decorated_file_input' returns appropriate datatype (either bytes or string) for the output file # count the number of characters written for the current index_row
-    
+            index_entry_currently_being_written = r[0]  # update current index_entry
+            int_num_character_written_for_index_entry_currently_being_written = 0  # reset the count of characters (which is equal to the number of bytes for any mtx records, because they only contains numeric characters)
+        int_num_character_written_for_index_entry_currently_being_written += file_output.write(
+            r[1]
+        )  # assumes the 'iterator_decorated_file_input' returns appropriate datatype (either bytes or string) for the output file # count the number of characters written for the current index_row
+
     # write the record for the last block
-    file_index_output.write( ( '\t'.join( map( str, [ index_entry_currently_being_written, int_total_num_character_written, int_total_num_character_written + int_num_character_written_for_index_entry_currently_being_written ] ) ) + '\n' ).encode( ) ) # write information required for indexing
+    file_index_output.write(
+        (
+            "\t".join(
+                map(
+                    str,
+                    [
+                        index_entry_currently_being_written,
+                        int_total_num_character_written,
+                        int_total_num_character_written
+                        + int_num_character_written_for_index_entry_currently_being_written,
+                    ],
+                )
+            )
+            + "\n"
+        ).encode()
+    )  # write information required for indexing
     # close index file
-    file_index_output.close( )
+    file_index_output.close()
     # if the output file is stream, does not close the stream # only close the output if the output file was an actual file
-    if flag_output_is_file :
-        file_output.close( )
-    
-    ''' delete input files once merge sort is completed if 'flag_delete_input_file_upon_completion' is True '''
-    if flag_delete_input_file_upon_completion and isinstance( l_path_file_input[ 0 ], str ) : # if paths are given as input files
-        for path_file in l_path_file_input :
-            os.remove( path_file )
-
-''' methods for handling 10X matrix objects '''
-def Convert_df_count_to_MTX_10X( path_file_df_count, path_folder_mtx_10x_output, chunksize = 500000, flag_debugging = False, inplace = False ) :
-    ''' # 2022-06-02 01:43:01 
+    if flag_output_is_file:
+        file_output.close()
+
+    """ delete input files once merge sort is completed if 'flag_delete_input_file_upon_completion' is True """
+    if flag_delete_input_file_upon_completion and isinstance(
+        l_path_file_input[0], str
+    ):  # if paths are given as input files
+        for path_file in l_path_file_input:
+            os.remove(path_file)
+
+
+""" methods for handling 10X matrix objects """
+
+
+def Convert_df_count_to_MTX_10X(
+    path_file_df_count,
+    path_folder_mtx_10x_output,
+    chunksize=500000,
+    flag_debugging=False,
+    inplace=False,
+):
+    """# 2022-06-02 01:43:01
     convert df_count (scarab output) to 10X MTX (matrix market) format in a memory-efficient manner.
-    
+
     'path_file_df_count' : file path to 'df_count'
-    '''
+    """
     # create a temporary output folder
-    path_folder_temp = f'{path_folder_mtx_10x_output}temp_{UUID( )}/' 
-    os.makedirs( path_folder_temp, exist_ok = True ) 
+    path_folder_temp = f"{path_folder_mtx_10x_output}temp_{UUID( )}/"
+    os.makedirs(path_folder_temp, exist_ok=True)
 
     # retrieve unique feature/barcode information from df_count
-    DF_Deduplicate_without_loading_in_memory( path_file_df_count, f'{path_folder_temp}_features.tsv.gz', l_col_for_identifying_duplicates = [ 'feature', 'id_feature' ], str_delimiter = '\t' )
-    int_num_lines = DF_Deduplicate_without_loading_in_memory( path_file_df_count, f'{path_folder_temp}_barcodes.tsv.gz', l_col_for_identifying_duplicates = [ 'barcode' ], str_delimiter = '\t' ) # collect the number of records
+    DF_Deduplicate_without_loading_in_memory(
+        path_file_df_count,
+        f"{path_folder_temp}_features.tsv.gz",
+        l_col_for_identifying_duplicates=["feature", "id_feature"],
+        str_delimiter="\t",
+    )
+    int_num_lines = DF_Deduplicate_without_loading_in_memory(
+        path_file_df_count,
+        f"{path_folder_temp}_barcodes.tsv.gz",
+        l_col_for_identifying_duplicates=["barcode"],
+        str_delimiter="\t",
+    )  # collect the number of records
 
     # read features and barcode information
-    df_barcode = pd.read_csv( f'{path_folder_temp}_barcodes.tsv.gz', sep = '\t', usecols = [ 'barcode' ] )
-    df_feature = pd.read_csv( f'{path_folder_temp}_features.tsv.gz', sep = '\t', usecols = [ 'feature', 'id_feature' ] )
-    df_feature = df_feature.loc[ :, [ 'id_feature', 'feature' ] ]
-    df_feature[ '10X_type' ] = 'Gene Expression'
+    df_barcode = pd.read_csv(
+        f"{path_folder_temp}_barcodes.tsv.gz", sep="\t", usecols=["barcode"]
+    )
+    df_feature = pd.read_csv(
+        f"{path_folder_temp}_features.tsv.gz",
+        sep="\t",
+        usecols=["feature", "id_feature"],
+    )
+    df_feature = df_feature.loc[:, ["id_feature", "feature"]]
+    df_feature["10X_type"] = "Gene Expression"
     # save feature/cell metadata
-    df_barcode.to_csv( f'{path_folder_temp}barcodes.tsv.gz', sep = '\t', index = False, header = False )
-    df_feature.to_csv( f'{path_folder_temp}features.tsv.gz', sep = '\t', index = False, header = False )
+    df_barcode.to_csv(
+        f"{path_folder_temp}barcodes.tsv.gz", sep="\t", index=False, header=False
+    )
+    df_feature.to_csv(
+        f"{path_folder_temp}features.tsv.gz", sep="\t", index=False, header=False
+    )
 
     # retrieve barcode/feature to integer representation of barcode/feature mapping
-    dict_to_int_barcode = dict( ( e, i + 1 ) for i, e in enumerate( df_barcode.iloc[ :, 0 ].values ) )
-    dict_to_int_feature = dict( ( e, i + 1 ) for i, e in enumerate( df_feature.iloc[ :, 0 ].values ) )
-
-    int_num_features, int_num_barcodes, int_num_records = len( df_feature ), len( df_barcode ), int_num_lines # retrieve metadata of the output matrix
-    del df_feature, df_barcode # delete objects
+    dict_to_int_barcode = dict(
+        (e, i + 1) for i, e in enumerate(df_barcode.iloc[:, 0].values)
+    )
+    dict_to_int_feature = dict(
+        (e, i + 1) for i, e in enumerate(df_feature.iloc[:, 0].values)
+    )
+
+    int_num_features, int_num_barcodes, int_num_records = (
+        len(df_feature),
+        len(df_barcode),
+        int_num_lines,
+    )  # retrieve metadata of the output matrix
+    del df_feature, df_barcode  # delete objects
 
     # write mtx file
-    with gzip.open( f'{path_folder_temp}matrix.mtx.gz', 'wb' ) as newfile :
-        newfile.write( f"""%%MatrixMarket matrix coordinate integer general\n%\n{int_num_features} {int_num_barcodes} {int_num_records}\n""".encode( ) )
+    with gzip.open(f"{path_folder_temp}matrix.mtx.gz", "wb") as newfile:
+        newfile.write(
+            f"""%%MatrixMarket matrix coordinate integer general\n%\n{int_num_features} {int_num_barcodes} {int_num_records}\n""".encode()
+        )
         # iterate through each chunk
-        for df_chunk in pd.read_csv( path_file_df_count, iterator = True, header = 0, chunksize = chunksize, sep = '\t', usecols = [ 'id_feature', 'barcode', 'read_count' ] ) :
-            df_chunk = df_chunk[ [ 'id_feature', 'barcode', 'read_count' ] ] # reorder columns
-            df_chunk[ 'id_feature' ] = df_chunk.id_feature.apply( MAP.Map( dict_to_int_feature ).a2b )
-            df_chunk[ 'barcode' ] = df_chunk.barcode.apply( MAP.Map( dict_to_int_barcode ).a2b )
-            df_chunk.to_csv( newfile, sep = ' ', header = None, index = False )
+        for df_chunk in pd.read_csv(
+            path_file_df_count,
+            iterator=True,
+            header=0,
+            chunksize=chunksize,
+            sep="\t",
+            usecols=["id_feature", "barcode", "read_count"],
+        ):
+            df_chunk = df_chunk[
+                ["id_feature", "barcode", "read_count"]
+            ]  # reorder columns
+            df_chunk["id_feature"] = df_chunk.id_feature.apply(
+                MAP.Map(dict_to_int_feature).a2b
+            )
+            df_chunk["barcode"] = df_chunk.barcode.apply(
+                MAP.Map(dict_to_int_barcode).a2b
+            )
+            df_chunk.to_csv(newfile, sep=" ", header=None, index=False)
 
     # export result files
-    for name_file in [ 'features.tsv.gz', 'barcodes.tsv.gz', 'matrix.mtx.gz' ] :
-        os.rename( f"{path_folder_temp}{name_file}", f"{path_folder_mtx_10x_output}{name_file}" )
+    for name_file in ["features.tsv.gz", "barcodes.tsv.gz", "matrix.mtx.gz"]:
+        os.rename(
+            f"{path_folder_temp}{name_file}", f"{path_folder_mtx_10x_output}{name_file}"
+        )
     # delete temporary folder
-    shutil.rmtree( path_folder_temp )
-            
+    shutil.rmtree(path_folder_temp)
```

### Comparing `biobookshelf-0.2.2/biobookshelf/STR/string.py` & `biobookshelf-0.2.3/biobookshelf/STR/string.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,255 +6,393 @@
 import biobookshelf.BA as BA
 
 # In[ ]:
 
 
 setting__n_characters__Insert_characters_every_n_characters = 20
 
-def Insert_characters_every_n_characters( a_string, n_characters = None, insert_characters = '\n' ) : 
-    """   Insert new line characters in the sequences every 'n_characters' characters   """
-    n_characters = setting__n_characters__Insert_characters_every_n_characters if n_characters is None else n_characters
-    return insert_characters.join( list( a_string[ n_characters * index_line : n_characters * ( index_line + 1 ) ] for index_line in np.arange( int( ( len( a_string ) - 1 ) / n_characters ) + 1 ) ) ) # Since there should not be additional no new additional character at the end for the sequences with 60 amino acid, ( len( seq ) - 1 ) / 60 will be used
 
+def Insert_characters_every_n_characters(
+    a_string, n_characters=None, insert_characters="\n"
+):
+    """Insert new line characters in the sequences every 'n_characters' characters"""
+    n_characters = (
+        setting__n_characters__Insert_characters_every_n_characters
+        if n_characters is None
+        else n_characters
+    )
+    return insert_characters.join(
+        list(
+            a_string[n_characters * index_line : n_characters * (index_line + 1)]
+            for index_line in np.arange(int((len(a_string) - 1) / n_characters) + 1)
+        )
+    )  # Since there should not be additional no new additional character at the end for the sequences with 60 amino acid, ( len( seq ) - 1 ) / 60 will be used
 
-def Replace_a_character_at_an_index( text, index, replacement ):
-    return text[ : index ] + replacement + text[ index + 1 : ]
+
+def Replace_a_character_at_an_index(text, index, replacement):
+    return text[:index] + replacement + text[index + 1 :]
 
 
 # In[ ]:
 
 
 setting__n_characters__replace_a_character_every_n_characters = 11
 
-def Replace_a_character_every_n_characters( a_string, n_characters = None, replacement_characters = '' ) : 
-    """   Insert new line characters in the sequences every 'n_characters' characters   """
-    n_characters = setting__n_characters__replace_a_character_every_n_characters if n_characters is None else n_characters
-    return replacement_characters.join( list( a_string[ n_characters * index_line : n_characters * ( index_line + 1 ) - 1 ] for index_line in np.arange( int( ( len( a_string ) - 1 ) / n_characters ) + 1 ) ) ) # Since there should not be additional no new additional character at the end for the sequences with 60 amino acid, ( len( seq ) - 1 ) / 60 will be used
+
+def Replace_a_character_every_n_characters(
+    a_string, n_characters=None, replacement_characters=""
+):
+    """Insert new line characters in the sequences every 'n_characters' characters"""
+    n_characters = (
+        setting__n_characters__replace_a_character_every_n_characters
+        if n_characters is None
+        else n_characters
+    )
+    return replacement_characters.join(
+        list(
+            a_string[n_characters * index_line : n_characters * (index_line + 1) - 1]
+            for index_line in np.arange(int((len(a_string) - 1) / n_characters) + 1)
+        )
+    )  # Since there should not be additional no new additional character at the end for the sequences with 60 amino acid, ( len( seq ) - 1 ) / 60 will be used
 
 
 # In[ ]:
 
 
-def Find_all( a_str, sub ) :
-    ''' Find all positions of a substring 'sub' in a given string 'a_str' '''
+def Find_all(a_str, sub):
+    """Find all positions of a substring 'sub' in a given string 'a_str'"""
     start = 0
-    l_positions = list( )
+    l_positions = list()
     while True:
-        start = a_str.find( sub, start )
-        if start == -1 : break
-        l_positions.append( start )
-        start += len( sub ) # use start += 1 to find overlapping matches
+        start = a_str.find(sub, start)
+        if start == -1:
+            break
+        l_positions.append(start)
+        start += len(sub)  # use start += 1 to find overlapping matches
     return l_positions
 
 
 # In[ ]:
 
 
-def Generate_substring_indexes( substring, string ) :
-    """ Generate indices of where substring begins in string
+def Generate_substring_indexes(substring, string):
+    """Generate indices of where substring begins in string
     >>> list(find_substring('me', "The cat says meow, meow"))
-    [13, 19]    """
+    [13, 19]"""
     last_found = -1  # Begin at -1 so the next position to search from is 0
     while True:
         # Find next index of substring, by starting after its last known position
-        last_found = string.find( substring, last_found + 1 )
-        if last_found == -1:  
+        last_found = string.find(substring, last_found + 1)
+        if last_found == -1:
             break  # All occurrences have been found
         yield last_found
 
 
 # In[ ]:
 
 
-def Locate_substring_last_index( substring, string ) :
-    """ return an index for the last substring in a string  """
+def Locate_substring_last_index(substring, string):
+    """return an index for the last substring in a string"""
     last_found = -1  # Begin at -1 so the next position to search from is 0
     while True:
         # Find next index of substring, by starting after its last known position
-        index = string.find( substring, last_found + 1)
-        if index == -1:  
+        index = string.find(substring, last_found + 1)
+        if index == -1:
             return last_found
-        else :
+        else:
             last_found = index
 
 
 # In[4]:
 
 
-def To_python_compatible_str( a_string, dict_replacement = { '%' : '_Percent_', '+' : '_Plus_', '-' : '_Minus_', '&' : '_and_', '=' : '_Equal_' } ) :
-    ''' convert a string into python-compatible string. '''
-    l_incompatible_character = [ ' ', '?', '(', ')', '&', '%', '/', ',', ':', '.', '-', '+', '[', ']', '#', '=', '\n', '"', '\\', '|', '?', '*' ]
-    for incompatible_character in l_incompatible_character : 
-        a_string = a_string.replace( incompatible_character, dict_replacement.get( incompatible_character, '_' ) )
+def To_python_compatible_str(
+    a_string,
+    dict_replacement={
+        "%": "_Percent_",
+        "+": "_Plus_",
+        "-": "_Minus_",
+        "&": "_and_",
+        "=": "_Equal_",
+    },
+):
+    """convert a string into python-compatible string."""
+    l_incompatible_character = [
+        " ",
+        "?",
+        "(",
+        ")",
+        "&",
+        "%",
+        "/",
+        ",",
+        ":",
+        ".",
+        "-",
+        "+",
+        "[",
+        "]",
+        "#",
+        "=",
+        "\n",
+        '"',
+        "\\",
+        "|",
+        "?",
+        "*",
+    ]
+    for incompatible_character in l_incompatible_character:
+        a_string = a_string.replace(
+            incompatible_character, dict_replacement.get(incompatible_character, "_")
+        )
     return a_string
 
 
 # In[ ]:
 
 
-def To_path_compatible_str( a_string ) :
-    '''
+def To_path_compatible_str(a_string):
+    """
         replace following characters to '_' so that a given string will be compatible for Window file system :
     : (colon)    " (double quote)    / (forward slash)    \ (backslash)    | (vertical bar or pipe)    ? (question mark)    * (asterisk)
         Also, replace new line character into '_'
-    '''
-    return a_string.replace( '\n', '_' ).replace( ':', '_' ).replace( '"', '_' ).replace( '/', '_' ).replace( '\\', '_' ).replace( '|', '_' ).replace( '?', '_' ).replace( '*', '_' ).replace( ' ', '_' ).replace( ';', '_' )
+    """
+    return (
+        a_string.replace("\n", "_")
+        .replace(":", "_")
+        .replace('"', "_")
+        .replace("/", "_")
+        .replace("\\", "_")
+        .replace("|", "_")
+        .replace("?", "_")
+        .replace("*", "_")
+        .replace(" ", "_")
+        .replace(";", "_")
+    )
 
 
 # In[ ]:
 
 
-def Read_Field_Locations( str_field_locations, character_indicating_fields = '-', character_indicating_non_fields = ' ' ) :
-    ''' return start and end position of masks annotating field locations of a given strings '''
-    int_position = 0 
-    l_l_annotation_start_end = list( )
-    while True :
-        str_field_locations_start = str_field_locations[ int_position : ]
-        if '-' in str_field_locations_start : int_annotation_start = str_field_locations_start.find( character_indicating_fields ) + int_position # retrive field annotation start position
-        else : break # finish the loop if there is no annotation left
-        str_field_locations_end = str_field_locations[ int_annotation_start : ]
-        int_annotation_end = str_field_locations_end.find( character_indicating_non_fields ) + int_annotation_start if ' ' in str_field_locations_end else len( str_field_locations ) # retrive field annotation end position
-        l_l_annotation_start_end.append( [ int_annotation_start, int_annotation_end ] )
+def Read_Field_Locations(
+    str_field_locations,
+    character_indicating_fields="-",
+    character_indicating_non_fields=" ",
+):
+    """return start and end position of masks annotating field locations of a given strings"""
+    int_position = 0
+    l_l_annotation_start_end = list()
+    while True:
+        str_field_locations_start = str_field_locations[int_position:]
+        if "-" in str_field_locations_start:
+            int_annotation_start = (
+                str_field_locations_start.find(character_indicating_fields)
+                + int_position
+            )  # retrive field annotation start position
+        else:
+            break  # finish the loop if there is no annotation left
+        str_field_locations_end = str_field_locations[int_annotation_start:]
+        int_annotation_end = (
+            str_field_locations_end.find(character_indicating_non_fields)
+            + int_annotation_start
+            if " " in str_field_locations_end
+            else len(str_field_locations)
+        )  # retrive field annotation end position
+        l_l_annotation_start_end.append([int_annotation_start, int_annotation_end])
         int_position = int_annotation_end
     return l_l_annotation_start_end
 
 
 # In[2]:
 
 
-def Search_Subsequence( str_seq, str_subseq, error_rate = 0.1, index_start_window = None, index_end_window = None ) :
-    ''' # 2021-02-04 18:12:04 
+def Search_Subsequence(
+    str_seq, str_subseq, error_rate=0.1, index_start_window=None, index_end_window=None
+):
+    """# 2021-02-04 18:12:04
     search a sequence with a given subsequence and return the integer index after the subsequence (for example, when subsequence presents from 10-19, return 20)
     'error_rate' : maximum allowed error_rate (including substitutions, insertions and deletions)
-    'index_start_window' : 
-    '''
+    'index_start_window' :
+    """
     # set default values
     str_matched_subsequence = None
-    index_start_subsequence = -1 # 0-based coordinates
-    index_end_subsequence = -1 # 0-based coordinates
+    index_start_subsequence = -1  # 0-based coordinates
+    index_end_subsequence = -1  # 0-based coordinates
     int_num_errors = -1
     # search all positions of a given sequence by default
-    len_seq = len( str_seq )
-    if index_start_window is None :
+    len_seq = len(str_seq)
+    if index_start_window is None:
         index_start_window = 0
-    if index_end_window is None :
+    if index_end_window is None:
         index_end_window = len_seq
     # handle negative indices (indices from the end of the sequence)
-    if index_start_window < 0 :
+    if index_start_window < 0:
         index_start_window = len_seq + index_start_window
-    if index_end_window < 0 :
+    if index_end_window < 0:
         index_end_window = len_seq + index_end_window
-    str_seq = str_seq[ index_start_window : index_end_window ]
-    if str_subseq in str_seq :
-        str_matched_subsequence = str_subseq # return the index after the subsequence
-        index_start_subsequence = index_start_window + str_seq.find( str_subseq )
-        index_end_subsequence = index_start_subsequence + len( str_subseq )
+    str_seq = str_seq[index_start_window:index_end_window]
+    if str_subseq in str_seq:
+        str_matched_subsequence = str_subseq  # return the index after the subsequence
+        index_start_subsequence = index_start_window + str_seq.find(str_subseq)
+        index_end_subsequence = index_start_subsequence + len(str_subseq)
         int_num_errors = 0
-    else :
-        int_max_num_allowed_errors = int( len( str_subseq ) * error_rate ) # set maximum number of errors
-        for int_num_allowed_errors in range( 1, int_max_num_allowed_errors + 1 ) :
-            l_match = regex.findall( f"({str_subseq}){{e<={int_num_allowed_errors}}}", str_seq )
-            if len( l_match ) > 0 :
-                str_matched_subsequence = l_match[ 0 ];
-                index_start_subsequence = index_start_window + str_seq.find( str_matched_subsequence )
-                index_end_subsequence = index_start_subsequence + len( str_matched_subsequence )
+    else:
+        int_max_num_allowed_errors = int(
+            len(str_subseq) * error_rate
+        )  # set maximum number of errors
+        for int_num_allowed_errors in range(1, int_max_num_allowed_errors + 1):
+            l_match = regex.findall(
+                f"({str_subseq}){{e<={int_num_allowed_errors}}}", str_seq
+            )
+            if len(l_match) > 0:
+                str_matched_subsequence = l_match[0]
+                index_start_subsequence = index_start_window + str_seq.find(
+                    str_matched_subsequence
+                )
+                index_end_subsequence = index_start_subsequence + len(
+                    str_matched_subsequence
+                )
                 int_num_errors = int_num_allowed_errors
                 break
 
-    return { "index_start_subsequence" : index_start_subsequence, "index_end_subsequence" : index_end_subsequence, "matched_subsequence" : str_matched_subsequence, "num_errors" : int_num_errors } # return dictionary containing the index after the subsequence
-
-def Search_Subsequences( str_seq, str_subseq, error_rate = 0.1, index_start_window = None, index_end_window = None, int_min_num_errors = 0 ) :
-    ''' # 2022-06-15 23:48:25 
+    return {
+        "index_start_subsequence": index_start_subsequence,
+        "index_end_subsequence": index_end_subsequence,
+        "matched_subsequence": str_matched_subsequence,
+        "num_errors": int_num_errors,
+    }  # return dictionary containing the index after the subsequence
+
+
+def Search_Subsequences(
+    str_seq,
+    str_subseq,
+    error_rate=0.1,
+    index_start_window=None,
+    index_end_window=None,
+    int_min_num_errors=0,
+):
+    """# 2022-06-15 23:48:25
     perform an exhuastive search of a sequence with a given subsequence and return the integer index after the subsequence (for example, when subsequence presents from 10-19, return 20)
     ignore overlapping matches. if one region was matched with the subsequence, the subsequent search will be done in the sequences excluding the region
-    
+
     'error_rate' : maximum allowed error_rate (including substitutions, insertions and deletions)
     'index_start_window', 'index_end_window' : start and end position of the region to search the subsequence
-    
+
     'int_min_num_errors' : an internal argument. the minimum number of errors for the search. used in the recursive calling of this function internally.
-    '''
-    l_sr = [ ] # initialize search results
-    def _initialize_search_result_( ) :
+    """
+    l_sr = []  # initialize search results
+
+    def _initialize_search_result_():
         # set default values
-        return { 'index_start_subsequence' : None, 'index_end_subsequence' : -1, 'matched_subsequence' : -1, 'num_errors' : -1 } # 0-based coordinates
+        return {
+            "index_start_subsequence": None,
+            "index_end_subsequence": -1,
+            "matched_subsequence": -1,
+            "num_errors": -1,
+        }  # 0-based coordinates
+
+    def _add_search_results_of_a_subsequence_(str_subseq, int_num_errors):
+        len_subseq = len(str_subseq)
+        for index_found in Find_all(str_seq_of_a_given_window, str_subseq):
+            ba[
+                index_found : index_found + len_subseq
+            ] = 1  # set the mask to mark the region matched with the subsequence
+            sr = _initialize_search_result_()
+            sr[
+                "matched_subsequence"
+            ] = str_subseq  # return the index after the subsequence
+            sr["index_start_subsequence"] = index_start_window + index_found
+            sr["index_end_subsequence"] = sr["index_start_subsequence"] + len_subseq
+            sr["num_errors"] = int_num_errors
+            l_sr.append(sr)
 
-    def _add_search_results_of_a_subsequence_( str_subseq, int_num_errors ) :
-        len_subseq = len( str_subseq )
-        for index_found in Find_all( str_seq_of_a_given_window, str_subseq ) :
-            ba[ index_found : index_found + len_subseq ] = 1 # set the mask to mark the region matched with the subsequence
-            sr = _initialize_search_result_( )
-            sr[ 'matched_subsequence' ] = str_subseq # return the index after the subsequence
-            sr[ 'index_start_subsequence' ] = index_start_window + index_found
-            sr[ 'index_end_subsequence' ] = sr[ 'index_start_subsequence' ] + len_subseq
-            sr[ 'num_errors' ] = int_num_errors
-            l_sr.append( sr )
-            
-    ''' indexing '''
+    """ indexing """
     # search all positions of a given sequence by default
-    len_seq = len( str_seq )
-    if index_start_window is None :
+    len_seq = len(str_seq)
+    if index_start_window is None:
         index_start_window = 0
-    if index_end_window is None :
+    if index_end_window is None:
         index_end_window = len_seq
     # handle negative indices (indices from the end of the sequence)
-    if index_start_window < 0 :
+    if index_start_window < 0:
         index_start_window = len_seq + index_start_window
-    if index_end_window < 0 :
+    if index_end_window < 0:
         index_end_window = len_seq + index_end_window
     # retrieve a sequence of the given window
-    str_seq_of_a_given_window = str_seq[ index_start_window : index_end_window ]
-    
-    ''' handle premature exit condition '''
-    if len( str_seq_of_a_given_window ) < len( str_subseq ) - int_min_num_errors : # if the searched region is smaller than the query sequence (considering errors), exit without performing the search
+    str_seq_of_a_given_window = str_seq[index_start_window:index_end_window]
+
+    """ handle premature exit condition """
+    if (
+        len(str_seq_of_a_given_window) < len(str_subseq) - int_min_num_errors
+    ):  # if the searched region is smaller than the query sequence (considering errors), exit without performing the search
         return l_sr
-    
-    ''' initialize bitarray mask '''
-    # 'ba' : an internal argument. a bitarray object of 'str_seq_of_a_given_window', marking the regions were matched subsequences were found (marked by 1). these region will be ignored 
-    ba = bitarray( len( str_seq_of_a_given_window ) )
-    ba.setall( 0 ) 
-    
-    ''' performing search for 'int_num_allowed_errors' '''
-    int_max_num_allowed_errors = int( len( str_subseq ) * error_rate ) # retrieve maximum number of allowed errors
-    if int_min_num_errors == 0 :
-        _add_search_results_of_a_subsequence_( str_subseq, 0 )
-    elif int_min_num_errors <= int_max_num_allowed_errors :
-        for str_matched_subsequence in regex.findall( f"({str_subseq}){{e<={int_min_num_errors}}}", str_seq_of_a_given_window ) :
-            _add_search_results_of_a_subsequence_( str_matched_subsequence, int_min_num_errors )
-        
-    if int_min_num_errors < int_max_num_allowed_errors : # recursive calls only when terminating condition (int_min_num_errors == int_max_num_allowed_errors) is not met 
-        for start_next_window, end_next_window in BA.Find_Segment( ba, background = 1 ) : # ignore matched regions in the subsequent searches
-            l_sr.extend( Search_Subsequences( str_seq, str_subseq, error_rate = error_rate, index_start_window = index_start_window + start_next_window, index_end_window = index_start_window + end_next_window, int_min_num_errors = int_min_num_errors + 1 ) ) # perform recursive search for the larger number of errors and collect the result
-    return l_sr # return the search result
+
+    """ initialize bitarray mask """
+    # 'ba' : an internal argument. a bitarray object of 'str_seq_of_a_given_window', marking the regions were matched subsequences were found (marked by 1). these region will be ignored
+    ba = bitarray(len(str_seq_of_a_given_window))
+    ba.setall(0)
+
+    """ performing search for 'int_num_allowed_errors' """
+    int_max_num_allowed_errors = int(
+        len(str_subseq) * error_rate
+    )  # retrieve maximum number of allowed errors
+    if int_min_num_errors == 0:
+        _add_search_results_of_a_subsequence_(str_subseq, 0)
+    elif int_min_num_errors <= int_max_num_allowed_errors:
+        for str_matched_subsequence in regex.findall(
+            f"({str_subseq}){{e<={int_min_num_errors}}}", str_seq_of_a_given_window
+        ):
+            _add_search_results_of_a_subsequence_(
+                str_matched_subsequence, int_min_num_errors
+            )
+
+    if (
+        int_min_num_errors < int_max_num_allowed_errors
+    ):  # recursive calls only when terminating condition (int_min_num_errors == int_max_num_allowed_errors) is not met
+        for start_next_window, end_next_window in BA.Find_Segment(
+            ba, background=1
+        ):  # ignore matched regions in the subsequent searches
+            l_sr.extend(
+                Search_Subsequences(
+                    str_seq,
+                    str_subseq,
+                    error_rate=error_rate,
+                    index_start_window=index_start_window + start_next_window,
+                    index_end_window=index_start_window + end_next_window,
+                    int_min_num_errors=int_min_num_errors + 1,
+                )
+            )  # perform recursive search for the larger number of errors and collect the result
+    return l_sr  # return the search result
+
 
 # In[ ]:
 
 
-def Find_stretch_of_a_character( a_str, a_char, int_len_threshold = 1 ) :
+def Find_stretch_of_a_character(a_str, a_char, int_len_threshold=1):
     """
     Find locations of stretches of a character
     'int_len_threshold' : a number of characters in a stretch to be classified as a 'stretch'
     return a list of [ index_start, index_end, length_of_stretch ] of identified stretches
     """
     # set default values
-    flag_stretch_started = False 
+    flag_stretch_started = False
     index_start = None
     index = 0
-    l_l = list( )
-    for current_char in a_str :
-        if flag_stretch_started :
-            if current_char != a_char : # when stretch has been started and has ended
+    l_l = list()
+    for current_char in a_str:
+        if flag_stretch_started:
+            if current_char != a_char:  # when stretch has been started and has ended
                 flag_stretch_started = False
                 len_stretch = index - index_start
-                if len_stretch >= int_len_threshold :
-                    l_l.append( [ index_start, index, len_stretch ] )
+                if len_stretch >= int_len_threshold:
+                    l_l.append([index_start, index, len_stretch])
                 index_start = None
-        else :
-            if current_char == a_char : # when stretch has just started
+        else:
+            if current_char == a_char:  # when stretch has just started
                 flag_stretch_started = True
                 index_start = index
         index += 1
-    if index_start is not None : # if stretch of a character ends with the given string
+    if index_start is not None:  # if stretch of a character ends with the given string
         len_stretch = index - index_start
-        if len_stretch >= int_len_threshold :
-            l_l.append( [ index_start, index, len_stretch ] )
+        if len_stretch >= int_len_threshold:
+            l_l.append([index_start, index, len_stretch])
     return l_l
-
```

### Comparing `biobookshelf-0.2.2/biobookshelf/UniProt/uniprot.py` & `biobookshelf-0.2.3/biobookshelf/UniProt/uniprot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from biobookshelf.main import *
 
-def FASTA_Parse_UniProt_Header( line ) :
-    """ # 2021-04-06 11:51:13 
+
+def FASTA_Parse_UniProt_Header(line):
+    """# 2021-04-06 11:51:13
     Parse uniprot header and return a dictionary containing field name and field values
     """
-    if line[ 0 ] == '>' : # remove '>' character in front of the line if presents
-        line = line[ 1 : ]
-    l_split = list( r.replace( '_|_', ' = ' ) for r in line.strip( ).replace( ' = ', '_|_' ).split( '=' ) ) # some OS name contain ' = ' characters. mask ' = ' before spliting with '='. 
-    l = [ ]
-    for r in l_split[ : -1 ] :
-        l.extend( r.rsplit( ' ', 1 ) )
-    arr_r = np.array( [ 'UniProt_FASTA_Name' ] + l + l_split[ -1 : ], dtype = object )
-    dict_field = dict( ( name_field, val ) for name_field, val in arr_r.reshape( ( int( len( arr_r ) / 2 ), 2 ) ) )
-    dict_field[ 'header' ] = line # add original line
-    return dict_field
+    if line[0] == ">":  # remove '>' character in front of the line if presents
+        line = line[1:]
+    l_split = list(
+        r.replace("_|_", " = ") for r in line.strip().replace(" = ", "_|_").split("=")
+    )  # some OS name contain ' = ' characters. mask ' = ' before spliting with '='.
+    l = []
+    for r in l_split[:-1]:
+        l.extend(r.rsplit(" ", 1))
+    arr_r = np.array(["UniProt_FASTA_Name"] + l + l_split[-1:], dtype=object)
+    dict_field = dict(
+        (name_field, val) for name_field, val in arr_r.reshape((int(len(arr_r) / 2), 2))
+    )
+    dict_field["header"] = line  # add original line
+    return dict_field
```

### Comparing `biobookshelf-0.2.2/biobookshelf/WEB/web_application.py` & `biobookshelf-0.2.3/biobookshelf/WEB/web_application.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,219 @@
 from biobookshelf.main import *
 
-def Round_Float( df, l_col_scientific_notations, l_col_typical_notation, n_significant_digits_scientific_notation = 3, n_significant_digits_typical_notation = 3, inplace = False ) :
-    ''' # 2021-07-19 17:38:40 
-    round float with a given number of significant digits and convert floating point numbers to strings '''
-    if not inplace :
-        df = deepcopy( df )
-    str_format_scientific_notation = "{:." + str( int( n_significant_digits_scientific_notation ) ) + "e}"
-    str_format_typical_notation = '{:.' + str( int( n_significant_digits_typical_notation ) ) + 'f}'
-    for col in l_col_scientific_notations :
-        df[ col ] = list( '' if np.isnan( value ) else str_format_scientific_notation.format( value ) for value in df[ col ].values )
-    for col in l_col_typical_notation :
-        df[ col ] = list( '' if np.isnan( value ) else str_format_typical_notation.format( value ) for value in df[ col ].values )
+
+def Round_Float(
+    df,
+    l_col_scientific_notations,
+    l_col_typical_notation,
+    n_significant_digits_scientific_notation=3,
+    n_significant_digits_typical_notation=3,
+    inplace=False,
+):
+    """# 2021-07-19 17:38:40
+    round float with a given number of significant digits and convert floating point numbers to strings"""
+    if not inplace:
+        df = deepcopy(df)
+    str_format_scientific_notation = (
+        "{:." + str(int(n_significant_digits_scientific_notation)) + "e}"
+    )
+    str_format_typical_notation = (
+        "{:." + str(int(n_significant_digits_typical_notation)) + "f}"
+    )
+    for col in l_col_scientific_notations:
+        df[col] = list(
+            "" if np.isnan(value) else str_format_scientific_notation.format(value)
+            for value in df[col].values
+        )
+    for col in l_col_typical_notation:
+        df[col] = list(
+            "" if np.isnan(value) else str_format_typical_notation.format(value)
+            for value in df[col].values
+        )
     return df
 
-def Index_and_Base64_Encode( df_to_be_indexed, l_col_index, path_prefix_output, path_folder_temp = '/tmp/', flag_delete_temp_folder = True ) :
-    """ # 2022-01-24 13:08:12 
+
+def Index_and_Base64_Encode(
+    df_to_be_indexed,
+    l_col_index,
+    path_prefix_output,
+    path_folder_temp="/tmp/",
+    flag_delete_temp_folder=True,
+):
+    """# 2022-01-24 13:08:12
     'df_to_be_indexed' : dataframe to be exported to base64 encoded file and indexed with values in 'l_col_index'
     'l_col_index' : list of columns for indexing 'df_to_be_indexed'
     'path_prefix_output' : directory prefix for an indexed base64 encoded file and a base64 encoded index file
     'path_folder_temp' : directory where a temporary folder will be created and removed
-    'flag_delete_temp_folder' : flag indicating whether the temporary folder should be removed 
+    'flag_delete_temp_folder' : flag indicating whether the temporary folder should be removed
     """
 
     # retrieve path_folder_wd
-    path_folder_temp = os.path.abspath( path_folder_temp )
-    if path_folder_temp[ -1 ] != '/' :
-        path_folder_temp += '/'
-    str_uuid = UUID( )
+    path_folder_temp = os.path.abspath(path_folder_temp)
+    if path_folder_temp[-1] != "/":
+        path_folder_temp += "/"
+    str_uuid = UUID()
     path_folder_temp = f"{path_folder_temp}{str_uuid}/"
-    os.makedirs( path_folder_temp, exist_ok = True )
+    os.makedirs(path_folder_temp, exist_ok=True)
 
-    df_to_be_indexed = deepcopy( df_to_be_indexed )
+    df_to_be_indexed = deepcopy(df_to_be_indexed)
     # retrieve unique indices from values in the 'l_col_index'
-    l_index = LIST_COUNT( df_to_be_indexed[ l_col_index ].values, duplicate_filter = None, sort_series_by_values = True ).index.values # sort by number of counts so that the most frequent access is close to the start of the file
+    l_index = LIST_COUNT(
+        df_to_be_indexed[l_col_index].values,
+        duplicate_filter=None,
+        sort_series_by_values=True,
+    ).index.values  # sort by number of counts so that the most frequent access is close to the start of the file
+
+    df_to_be_indexed.set_index(l_col_index, inplace=True)
+    df_to_be_indexed.sort_index(inplace=True)  # sort by index for faster indexing
 
-    df_to_be_indexed.set_index( l_col_index, inplace = True )
-    df_to_be_indexed.sort_index( inplace = True ) # sort by index for faster indexing
-    
     # base64 encode each individual file
-    for int_index, t_index in enumerate( l_index ) :
-        df = df_to_be_indexed.loc[ t_index ]
-        df.reset_index( drop = False, inplace = True )
+    for int_index, t_index in enumerate(l_index):
+        df = df_to_be_indexed.loc[t_index]
+        df.reset_index(drop=False, inplace=True)
         path_prefix_file = f"{path_folder_temp}{int_index}"
-        df.T.to_csv( f"{path_prefix_file}.tsv.gz", sep = '\t', index = True, header = None ) # save transposed array (each 'row' is column, and the first element in each 'row' is the column name)
-        Base64_Encode( f"{path_prefix_file}.tsv.gz", f"{path_prefix_file}.tsv.gz.base64.txt", header = ' ' )
+        df.T.to_csv(
+            f"{path_prefix_file}.tsv.gz", sep="\t", index=True, header=None
+        )  # save transposed array (each 'row' is column, and the first element in each 'row' is the column name)
+        Base64_Encode(
+            f"{path_prefix_file}.tsv.gz",
+            f"{path_prefix_file}.tsv.gz.base64.txt",
+            header=" ",
+        )
 
     # retrieve file size of base64 encoded chucks
-    df_file_base64 = GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_temp}*.tsv.gz.base64.txt", retrieve_file_size = True )
-    df_file_base64.wildcard_0 = df_file_base64.wildcard_0.astype( int ) # retrieve integer index
-    df_file_base64.sort_values( 'wildcard_0', inplace = True ) # sort by gene_name
+    df_file_base64 = GLOB_Retrive_Strings_in_Wildcards(
+        f"{path_folder_temp}*.tsv.gz.base64.txt", retrieve_file_size=True
+    )
+    df_file_base64.wildcard_0 = df_file_base64.wildcard_0.astype(
+        int
+    )  # retrieve integer index
+    df_file_base64.sort_values("wildcard_0", inplace=True)  # sort by gene_name
 
     # concatanate base64 encoded files in the specified order
-    OS_FILE_Combine_Files_in_order( df_file_base64.path.values, f"{path_prefix_output}.tsv.gz.base64.concatanated.txt", overwrite_existing_file = True )
+    OS_FILE_Combine_Files_in_order(
+        df_file_base64.path.values,
+        f"{path_prefix_output}.tsv.gz.base64.concatanated.txt",
+        overwrite_existing_file=True,
+    )
 
     # write an index file describing the byte positions of each gene_symbol in the concatanated file
     int_byte_accumulated = 0
-    l_l = [ ]
-    flag_multiindex = len( l_col_index ) > 1 # retrieve flag indicating whether a multi-index was used.
-    for int_index, size_in_bytes in df_file_base64[ [ 'wildcard_0', 'size_in_bytes' ] ].values :
-        l_l.append( list( l_index[ int_index ] ) + [ int_byte_accumulated, int_byte_accumulated + size_in_bytes ] ) # index_byte uses 0-based coordinates
-        int_byte_accumulated += size_in_bytes # update accumulated number of bytes
-    df_index_byte = pd.DataFrame( l_l, columns = l_col_index + [ 'index_byte_start', 'index_byte_end' ] )
-
-    df_index_byte.T.to_csv( f"{path_folder_temp}index.tsv.gz", sep = '\t', index = True, header = False )
-    Base64_Encode( f"{path_folder_temp}index.tsv.gz", f"{path_prefix_output}.index.tsv.gz.base64.txt" ) # convert binary file into text using base64 encoding
+    l_l = []
+    flag_multiindex = (
+        len(l_col_index) > 1
+    )  # retrieve flag indicating whether a multi-index was used.
+    for int_index, size_in_bytes in df_file_base64[
+        ["wildcard_0", "size_in_bytes"]
+    ].values:
+        l_l.append(
+            list(l_index[int_index])
+            + [int_byte_accumulated, int_byte_accumulated + size_in_bytes]
+        )  # index_byte uses 0-based coordinates
+        int_byte_accumulated += size_in_bytes  # update accumulated number of bytes
+    df_index_byte = pd.DataFrame(
+        l_l, columns=l_col_index + ["index_byte_start", "index_byte_end"]
+    )
+
+    df_index_byte.T.to_csv(
+        f"{path_folder_temp}index.tsv.gz", sep="\t", index=True, header=False
+    )
+    Base64_Encode(
+        f"{path_folder_temp}index.tsv.gz",
+        f"{path_prefix_output}.index.tsv.gz.base64.txt",
+    )  # convert binary file into text using base64 encoding
 
-    if flag_delete_temp_folder :
+    if flag_delete_temp_folder:
         # remove temporary folder
-        shutil.rmtree( path_folder_temp )
-        
-def Index_Chunks_and_Base64_Encode( df_to_be_chunked_and_indexed, int_num_rows_for_each_chunk, path_prefix_output, flag_include_header = False, path_folder_temp = '/tmp/', flag_delete_temp_folder = True ) :
-    """ # 2022-06-20 10:53:13 
+        shutil.rmtree(path_folder_temp)
+
+
+def Index_Chunks_and_Base64_Encode(
+    df_to_be_chunked_and_indexed,
+    int_num_rows_for_each_chunk,
+    path_prefix_output,
+    flag_include_header=False,
+    path_folder_temp="/tmp/",
+    flag_delete_temp_folder=True,
+):
+    """# 2022-06-20 10:53:13
     'df_to_be_chunked_and_indexed' : dataframe to be exported to base64 encoded file and indexed with values in 'l_col_index'
     'l_col_index' : list of columns for indexing 'df_to_be_chunked_and_indexed'
     'path_prefix_output' : directory prefix for an indexed base64 encoded file and a base64 encoded index file
     'flag_include_header' : include header in the output file
     'path_folder_temp' : directory where a temporary folder will be created and removed
-    'flag_delete_temp_folder' : flag indicating whether the temporary folder should be removed 
+    'flag_delete_temp_folder' : flag indicating whether the temporary folder should be removed
     """
 
     # retrieve path_folder_wd
-    path_folder_temp = os.path.abspath( path_folder_temp )
-    if path_folder_temp[ -1 ] != '/' :
-        path_folder_temp += '/'
-    str_uuid = UUID( )
+    path_folder_temp = os.path.abspath(path_folder_temp)
+    if path_folder_temp[-1] != "/":
+        path_folder_temp += "/"
+    str_uuid = UUID()
     path_folder_temp = f"{path_folder_temp}{str_uuid}/"
-    os.makedirs( path_folder_temp, exist_ok = True )
+    os.makedirs(path_folder_temp, exist_ok=True)
 
-    df_to_be_chunked_and_indexed = deepcopy( df_to_be_chunked_and_indexed )
-    int_num_rows = len( df_to_be_chunked_and_indexed )
+    df_to_be_chunked_and_indexed = deepcopy(df_to_be_chunked_and_indexed)
+    int_num_rows = len(df_to_be_chunked_and_indexed)
 
     # calculate the number of chunk
-    int_num_chunk = int( np.ceil( int_num_rows / int_num_rows_for_each_chunk ) )
+    int_num_chunk = int(np.ceil(int_num_rows / int_num_rows_for_each_chunk))
     # base64 encode each individual file
-    for int_index in range( int_num_chunk ) :
-        df = df_to_be_chunked_and_indexed.iloc[ int_index * int_num_rows_for_each_chunk : ( int_index + 1 ) * int_num_rows_for_each_chunk ]
+    for int_index in range(int_num_chunk):
+        df = df_to_be_chunked_and_indexed.iloc[
+            int_index
+            * int_num_rows_for_each_chunk : (int_index + 1)
+            * int_num_rows_for_each_chunk
+        ]
         path_prefix_file = f"{path_folder_temp}{int_index}"
-        df.T.to_csv( f"{path_prefix_file}.tsv.gz", sep = '\t', index = flag_include_header, header = None ) # save transposed array (each 'row' is column, and the first element in each 'row' is the column name) # to aid parsing in browser side
-        Base64_Encode( f"{path_prefix_file}.tsv.gz", f"{path_prefix_file}.tsv.gz.base64.txt", header = ' ' ) # the additional ' ' space is to help separate file contents when using range queries
+        df.T.to_csv(
+            f"{path_prefix_file}.tsv.gz",
+            sep="\t",
+            index=flag_include_header,
+            header=None,
+        )  # save transposed array (each 'row' is column, and the first element in each 'row' is the column name) # to aid parsing in browser side
+        Base64_Encode(
+            f"{path_prefix_file}.tsv.gz",
+            f"{path_prefix_file}.tsv.gz.base64.txt",
+            header=" ",
+        )  # the additional ' ' space is to help separate file contents when using range queries
 
     # retrieve file size of base64 encoded chucks
-    df_file_base64 = GLOB_Retrive_Strings_in_Wildcards( f"{path_folder_temp}*.tsv.gz.base64.txt", retrieve_file_size = True )
-    df_file_base64.wildcard_0 = df_file_base64.wildcard_0.astype( int ) # retrieve integer index
-    df_file_base64.sort_values( 'wildcard_0', inplace = True ) # sort by gene_name
+    df_file_base64 = GLOB_Retrive_Strings_in_Wildcards(
+        f"{path_folder_temp}*.tsv.gz.base64.txt", retrieve_file_size=True
+    )
+    df_file_base64.wildcard_0 = df_file_base64.wildcard_0.astype(
+        int
+    )  # retrieve integer index
+    df_file_base64.sort_values("wildcard_0", inplace=True)  # sort by gene_name
 
     # concatanate base64 encoded files in the specified order
-    OS_Run( [ 'cat' ] + list( df_file_base64.path.values ), path_file_stdout = f"{path_prefix_output}.tsv.gz.base64.concatenated.txt" )
+    OS_Run(
+        ["cat"] + list(df_file_base64.path.values),
+        path_file_stdout=f"{path_prefix_output}.tsv.gz.base64.concatenated.txt",
+    )
 
     # write an index file describing the byte positions of each gene_symbol in the concatanated file
     int_byte_accumulated = 0
-    l_l = [ ]
-    for int_index, size_in_bytes in df_file_base64[ [ 'wildcard_0', 'size_in_bytes' ] ].values :
-        l_l.append( [ int_index, int_byte_accumulated, int_byte_accumulated + size_in_bytes ] ) # index each chunk # index_byte uses 0-based coordinates
-        int_byte_accumulated += size_in_bytes # update accumulated number of bytes
-    df_index_byte = pd.DataFrame( l_l, columns = [ 'index_chunk', 'index_byte_start', 'index_byte_end' ] )
-
-    df_index_byte.T.to_csv( f"{path_folder_temp}index.tsv.gz", sep = '\t', index = True, header = False )
-    Base64_Encode( f"{path_folder_temp}index.tsv.gz", f"{path_prefix_output}.index.tsv.gz.base64.txt" ) # convert binary file into text using base64 encoding
+    l_l = []
+    for int_index, size_in_bytes in df_file_base64[
+        ["wildcard_0", "size_in_bytes"]
+    ].values:
+        l_l.append(
+            [int_index, int_byte_accumulated, int_byte_accumulated + size_in_bytes]
+        )  # index each chunk # index_byte uses 0-based coordinates
+        int_byte_accumulated += size_in_bytes  # update accumulated number of bytes
+    df_index_byte = pd.DataFrame(
+        l_l, columns=["index_chunk", "index_byte_start", "index_byte_end"]
+    )
+
+    df_index_byte.T.to_csv(
+        f"{path_folder_temp}index.tsv.gz", sep="\t", index=True, header=False
+    )
+    Base64_Encode(
+        f"{path_folder_temp}index.tsv.gz",
+        f"{path_prefix_output}.index.tsv.gz.base64.txt",
+    )  # convert binary file into text using base64 encoding
 
-    if flag_delete_temp_folder :
+    if flag_delete_temp_folder:
         # remove temporary folder
-        shutil.rmtree( path_folder_temp )
+        shutil.rmtree(path_folder_temp)
```

### Comparing `biobookshelf-0.2.2/biobookshelf.egg-info/PKG-INFO` & `biobookshelf-0.2.3/biobookshelf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.2
+Version: 0.2.3
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.2/biobookshelf.egg-info/SOURCES.txt` & `biobookshelf-0.2.3/biobookshelf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.2/setup.py` & `biobookshelf-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,59 +7,59 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
-    name='biobookshelf',
-    version='0.2.2',
+    name="biobookshelf",
+    version="0.2.3",
     author="Hyunsu An",
     author_email="ahs2202@gm.gist.ac.kr",
     description="a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ahs2202/biobookshelf",
     license="GPLv3",
-    packages=find_packages(include=['biobookshelf', 'biobookshelf.*']),
+    packages=find_packages(include=["biobookshelf", "biobookshelf.*"]),
     include_package_data=True,
     install_requires=[
-        'ipython>=7.19.0',
-        'plotly>=4.11.0',
-        'plotnine>=0.10.1',
-        'pandas>=1.1.4',
-        'numpy>=1.18.5',
-        'pysam>=0.16.0.1',
-        'scanpy>=1.6.0',
-        'intervaltree>=3.1.0',
-        'umap-learn>=0.4.6',
-        'regex>=2020.10.15',
-        'scipy>=1.4.1',
-        'matplotlib>=3.3.2',
-        'leidenalg>=0.8.3',
-        'numba>=0.52.0',
-        'scikit-learn>=1.0.2',
-        'seaborn>=0.11.1',
-        'statsmodels>=0.12.1',
-        'bitarray>=1.6.1',
-        'xmltodict>=0.12.0',
-        'beautifulsoup4>=4.9.3',
+        "ipython>=7.19.0",
+        "plotly>=4.11.0",
+        "plotnine>=0.10.1",
+        "pandas>=1.1.4",
+        "numpy>=1.18.5",
+        "pysam>=0.16.0.1",
+        "scanpy>=1.6.0",
+        "intervaltree>=3.1.0",
+        "umap-learn>=0.4.6",
+        "regex>=2020.10.15",
+        "scipy>=1.4.1",
+        "matplotlib>=3.3.2",
+        "leidenalg>=0.8.3",
+        "numba>=0.52.0",
+        "scikit-learn>=1.0.2",
+        "seaborn>=0.11.1",
+        "statsmodels>=0.12.1",
+        "bitarray>=1.6.1",
+        "xmltodict>=0.12.0",
+        "beautifulsoup4>=4.9.3",
         "parse>=1.18.0",
         "UpSetPlot>=0.4.1",
         "seqfold>=0.7.7",
-        'mappy>=2.21',
-        'primer3-py>=0.6.1',
-        'biopython>=1.79',
-        'edlib>=1.3.9',
-        'h5py>=2.1.0',
-        'psutil>=5.7.0',
-        'zarr>=2.11.0',
+        "mappy>=2.21",
+        "primer3-py>=0.6.1",
+        "biopython>=1.79",
+        "edlib>=1.3.9",
+        "h5py>=2.1.0",
+        "psutil>=5.7.0",
+        "zarr>=2.11.0",
     ],
     entry_points={
         "console_scripts": [
             "biobook-check_plasmid_with_nanopore_sequencing=biobookshelf.ONT.nanopore_functions:Check_plasmid_with_nanopore_sequencing",
             "biobook-run_guppy_and_combine_output=biobookshelf.ONT.nanopore_functions:Guppy_Run_and_Combine_Output",
-            'biobook-Server_Status=biobookshelf.CLI.unclassified_programs:Server_Status',
-            'biobook-Stop_a_job=biobookshelf.CLI.unclassified_programs:Stop_a_job',
+            "biobook-Server_Status=biobookshelf.CLI.unclassified_programs:Server_Status",
+            "biobook-Stop_a_job=biobookshelf.CLI.unclassified_programs:Stop_a_job",
         ]
     },
 )
```

