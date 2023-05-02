# Comparing `tmp/living-figures-0.1.5.tar.gz` & `tmp/living-figures-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.1.5.tar", last modified: Mon Apr 24 18:02:55 2023, max compression
+gzip compressed data, was "living-figures-0.2.0.tar", last modified: Tue May  2 16:46:19 2023, max compression
```

## Comparing `living-figures-0.1.5.tar` & `living-figures-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-24 18:01:53.000000 living-figures-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 18:01:53.000000 living-figures-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-24 18:02:55.874375 living-figures-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 18:01:53.000000 living-figures-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-24 18:01:53.000000 living-figures-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 18:01:53.000000 living-figures-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:02:55.874375 living-figures-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 18:01:53.000000 living-figures-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/pacbio_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/utilities/parse_tax_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/living_figures/bio/fom/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/ordination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/parse_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-24 18:01:53.000000 living-figures-0.1.5/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.768403 living-figures-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 16:45:17.000000 living-figures-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 16:45:17.000000 living-figures-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-02 16:46:19.768403 living-figures-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-02 16:45:17.000000 living-figures-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-02 16:45:17.000000 living-figures-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 16:45:17.000000 living-figures-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:46:19.768403 living-figures-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 16:45:17.000000 living-figures-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.760403 living-figures-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/epigenome/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27853 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/fom/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/utilities/parse_tax_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/utilities/parse_taxon_abundances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.760403 living-figures-0.2.0/src/living_figures/bio/fom/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/base_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/beta_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/differential_abundance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/ordination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.768403 living-figures-0.2.0/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.768403 living-figures-0.2.0/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/helpers/parse_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 16:45:17.000000 living-figures-0.2.0/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.764403 living-figures-0.2.0/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-02 16:46:19.000000 living-figures-0.2.0/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-02 16:46:19.000000 living-figures-0.2.0/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:46:19.000000 living-figures-0.2.0/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 16:46:19.000000 living-figures-0.2.0/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 16:46:19.000000 living-figures-0.2.0/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:19.768403 living-figures-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 16:45:17.000000 living-figures-0.2.0/tests/test_import.py
```

### Comparing `living-figures-0.1.5/LICENSE` & `living-figures-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/PKG-INFO` & `living-figures-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.5
+Version: 0.2.0
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.5/README.md` & `living-figures-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/pyproject.toml` & `living-figures-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py` & `living-figures-0.2.0/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/pacbio_file.py` & `living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/parse_rebase.py` & `living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/rebase_file.py` & `living-figures-0.2.0/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/panepibrowser.py` & `living-figures-0.2.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,22 +249,17 @@
             # Set up a new table
             df = pd.DataFrame(dict(id=all_options))
 
         # Otherwise
         else:
 
             # See if any of the options are missing
-            missing_options = [
-                option
-                for option in df.reindex(
-                    columns=['id']
-                ).dropna(
-                )['id'].drop_duplicates().tolist()
-                if option not in all_options
-            ]
+            missing_options = list(
+                set(all_options) - set(df['id'].dropna().tolist())
+            )
 
             # If no options are missing, we're done
             if len(missing_options) == 0:
                 return
 
             # Otherwise, add in new rows
             df = pd.concat([
@@ -299,14 +294,20 @@
 
         # Link to the online documentation
         docs_url = "https://living-figures.com/post/panepigenome-browser/"
         self.sidebar_container.markdown(
             f"[Pan-Epigenome Browser Documentation]({docs_url})"
         )
 
+        # Link to the online issues
+        bugs_url = "https://github.com/FredHutch/living-figures/issues"
+        self.sidebar_container.markdown(
+            f"[Report Bugs]({bugs_url})"
+        )
+
     def update_annotation_selectors(self):
 
         genomes_annot = self.get(["files", "genomes_annot"])
         if genomes_annot.shape[0] == 0:
             genomes_annot = pd.DataFrame(dict(id=[]))
         else:
             msg = "Must provide 'id' column in genome annotations"
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/__init__.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,8 @@
 from living_figures.bio.fom.widgets.microbiome.inputs import MicrobiomeAbund # noqa
 from living_figures.bio.fom.widgets.microbiome.inputs import StHashedDataFrame # noqa
 from living_figures.bio.fom.widgets.microbiome.ordination import Ordination # noqa
 from living_figures.bio.fom.widgets.microbiome.abundant_orgs import AbundantOrgs # noqa
 from living_figures.bio.fom.widgets.microbiome.alpha_diversity import AlphaDiversity # noqa
+from living_figures.bio.fom.widgets.microbiome.beta_diversity import BetaDiversity # noqa
+from living_figures.bio.fom.widgets.microbiome.differential_abundance import DifferentialAbundance # noqa
 from living_figures.bio.fom.widgets.microbiome.base_widget import BaseMicrobiomeExplorer # noqa
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from living_figures.helpers.scaling import convert_text_to_scalar
 from living_figures.helpers.sorting import sort_table
 import widgets.streamlit as wist
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
+import streamlit as st
 
 
 class AbundantOrgs(MicrobiomePlot):
 
     label = "Abundant Organisms"
 
     children = [
@@ -119,139 +120,160 @@
             ]
         ),
         wist.StResource(id="plot"),
         wist.StResource(id="plot_msg"),
         wist.StResource(id="legend_display")
     ]
 
-    def get_abundance_data(self):
-
-        # Get the plotting options
-        params = self.all_values(flatten=True)
+    @st.cache_data(max_entries=10)
+    def get_abundance_data(
+        _self,
+        tax_level: str,
+        filter_by: str,
+        n_orgs: int,
+        abund_hash
+    ):
 
         # Get the abundances, filtering to the specified taxonomic level
         # Columns are samples, rows are organisms
-        abund: pd.DataFrame = self._root().abund(
-            level=params['tax_level'],
-            filter=params['filter_by']
+        abund: pd.DataFrame = _self._root().abund(
+            level=tax_level,
+            filter=filter_by
         )
 
         if abund is None:
             return
 
         # If there are no more organisms than the specified max
-        if abund.shape[0] <= params["n_orgs"]:
+        if abund.shape[0] <= n_orgs:
             return abund
 
         # Otherwise, we need to filter down the number of organisms being shown
 
         # Compute the average abundance of each organism
         mean_abund = abund.mean(axis=1).sort_values(ascending=False)
 
-        to_keep = mean_abund.index.values[:(params["n_orgs"]-1)]
+        to_keep = mean_abund.index.values[:(n_orgs-1)]
 
         abund = pd.concat([
             abund.reindex(index=to_keep),
             pd.DataFrame(dict(
                 Other=abund.drop(index=to_keep).sum()
             )).T
         ])
 
         return abund
 
-    def get_plotting_data(self):
-        """Return the data used for plotting, using the cache when possible."""
-
-        # If the cache is populated
-        if self.get_cache(self.make_cache_key()) is not None:
-            # Return the cached data
-            return self.get_cache(self.make_cache_key())
-
-        # If the cache is not populated
+    @st.cache_data(max_entries=10)
+    def get_plotting_data(
+        _self,
+        tax_level,
+        filter_by,
+        n_orgs,
+        color_by,
+        sort_by,
+        abund_hash,
+        annot_hash
+    ):
+        """Return the data used for plotting."""
 
         # Get the abundance data to plot
-        abund_df = self.get_abundance_data()
+        abund_df = _self.get_abundance_data(
+            tax_level,
+            filter_by,
+            n_orgs,
+            abund_hash
+        )
 
         # If there is no abundance data
         if abund_df is None:
-            # Note the lack of data in the cache
-            self.set_cache(self.make_cache_key(), (None, None))
             return None, None
 
         # Get the metadata (if any was provided)
-        sample_annots: pd.DataFrame = self._root().sample_annotations()
-
-        # Get all of the parameters used for plotting
-        params = self.all_values(flatten=True)
+        sample_annots: pd.DataFrame = _self._root().sample_annotations()
 
         # If there is metadata and the user wants to display it
-        if len(params['color_by']) > 0 and sample_annots is not None:
+        if len(color_by) > 0 and sample_annots is not None:
 
             annot_df = sample_annots.reindex(
-                columns=params['color_by'],
+                columns=color_by,
                 index=abund_df.columns.values
             ).dropna()
 
             # If there are no samples with the selected metadata
             if annot_df.shape[0] == 0:
-
-                msg = "No samples available with the selected annotations"
-                self.option("plot_msg").main_empty.warning(msg)
-                self.set_cache(self.make_cache_key(), (None, None))
                 return None, None
 
             # Only keep the abundances which have annotations
             abund_df = abund_df.reindex(
                 columns=annot_df.index.values
             )
 
         else:
             annot_df = None
 
         # If the user requested to sort samples by organism abundances
-        if params['sort_by'] == "Organism Abundances":
+        if sort_by == "Organism Abundances":
 
             # Sort the abundance table
             abund_df = sort_table(abund_df)
 
         # If the user requested to sort samples by annotations
-        elif params['sort_by'] == "Selected Metadata" and annot_df is not None:
+        elif sort_by == "Selected Metadata" and annot_df is not None:
 
             # Sort the annotation table
             annot_df = annot_df.sort_values(
                 by=list(annot_df.columns.values)
             )
 
             # Order the abundances to match
             abund_df = abund_df.reindex(columns=annot_df.index.values)
 
         # Order the annotations to match the abundances
         if annot_df is not None:
             annot_df = annot_df.reindex(index=abund_df.columns.values)
 
-        self.set_cache(self.make_cache_key(), (abund_df, annot_df))
         return abund_df, annot_df
 
-    def run_self(self):
+    @st.cache_data(max_entries=10)
+    def make_fig(
+        _self,
+        tax_level,
+        filter_by,
+        n_orgs,
+        color_by,
+        sort_by,
+        annot_size,
+        plot_type,
+        title,
+        abund_hash,
+        annot_hash
+    ):
+        """Make the figure to plot"""
 
         # Get the plotting data
-        abund_df, annot_df = self.get_plotting_data()
+        abund_df, annot_df = _self.get_plotting_data(
+            tax_level,
+            filter_by,
+            n_orgs,
+            color_by,
+            sort_by,
+            abund_hash,
+            annot_hash
+        )
 
         # If there is no data
         if abund_df is None:
             # Don't make a plot
             return
 
-        # Get all of the parameters used for plotting
-        params = self.all_values(flatten=True)
-
         # Set up the size of the annotations
         annot_frac = min(
             0.5,
-            0.02 + (params["annot_size"] * float(len(params["color_by"])))
+            0.02 + (annot_size * float(len(color_by)))
         )
         row_heights = [1 - annot_frac, annot_frac]
 
         # Set up the plot area
         fig = make_subplots(
             rows=1 if annot_df is None else 2,
             cols=1,
@@ -259,36 +281,61 @@
             horizontal_spacing=0.01,
             start_cell="top-left",
             row_heights=None if annot_df is None else row_heights,
             shared_xaxes=True
         )
 
         # Plot the heatmap / stacked bars
-        fig.add_traces(self.plot_abund(abund_df), rows=1, cols=1)
+        fig.add_traces(_self.plot_abund(abund_df), rows=1, cols=1)
 
-        if params["plot_type"] == "Stacked Bars":
+        if plot_type == "Stacked Bars":
             fig.update_layout(
                 barmode='stack',
                 yaxis_title="Relative Abundance (%)"
             )
 
         # Plot the annotations
-        if len(params['color_by']) > 0 and annot_df is not None:
-            fig.add_trace(self.plot_annot(annot_df), row=2, col=1)
+        if len(color_by) > 0 and annot_df is not None:
+            fig.add_trace(_self.plot_annot(annot_df), row=2, col=1)
 
         # If there is a title
-        if params['title'] is not None and params['title'] != "None":
-            fig.update_layout(title=params['title'])
+        if title is not None and title != "None":
+            fig.update_layout(title=title)
+
+        return fig
 
-        plot_area = self._get_child("plot")
-        plot_area.main_empty.plotly_chart(
-            fig,
-            use_container_width=True
+    def run_self(self):
+
+        # Get the plotting options
+        params = self.all_values(flatten=True)
+
+        # Get the figure to plot
+        fig = self.make_fig(
+            params['tax_level'],
+            params['filter_by'],
+            params['n_orgs'],
+            params['color_by'],
+            params['sort_by'],
+            params['annot_size'],
+            params['plot_type'],
+            params['title'],
+            self._root().abund_hash(),
+            self._root().annot_hash()
         )
 
+        # If there is a figure
+        if fig is not None:
+
+            # Display it in the 'plot' child resource
+            plot_area = self._get_child("plot")
+            plot_area.main_empty.plotly_chart(
+                fig,
+                use_container_width=True
+            )
+
         # If there is a legend
         if params['legend'] is not None:
             self._get_child(
                 "legend_display"
             ).main_empty.markdown(
                 params['legend']
             )
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from scipy.stats import entropy, spearmanr, pearsonr
+from scipy.stats import entropy, spearmanr, pearsonr, f_oneway
 import streamlit as st
 from typing import Union
 from living_figures.bio.fom.widgets.microbiome.base_plots import MicrobiomePlot
 from living_figures.helpers.constants import tax_levels
 from living_figures.helpers.parse_numeric import is_numeric
 import widgets.streamlit as wist
 import pandas as pd
@@ -29,28 +29,26 @@
     """
 
     label = "Alpha Diversity"
 
     children = [
         wist.StExpander(
             id="options",
-            expanded=True,
             children=[
                 wist.StColumns(
                     id="row1",
                     children=[
                         wist.StSelectString(
-                            id='plot_type',
-                            label="Plot Type",
+                            id="metric",
+                            label="Diversity Metric",
                             options=[
-                                'Distribution',
-                                'Points',
-                                'Bars'
+                                "Shannon",
+                                "Simpson"
                             ],
-                            value='Distribution'
+                            value="Shannon"
                         ),
                         wist.StSelectString(
                             id="tax_level",
                             label="Taxonomic Level",
                             options=tax_levels,
                             value="genus"
                         )
@@ -71,22 +69,20 @@
                             options=[]
                         )
                     ]
                 ),
                 wist.StColumns(
                     id='row3',
                     children=[
-                        wist.StSelectString(
-                            id="metric",
-                            label="Diversity Metric",
-                            options=[
-                                "Shannon",
-                                "Simpson"
-                            ],
-                            value="Shannon"
+                        wist.StInteger(
+                            id="nbins",
+                            label="Number of Bins",
+                            min_value=5,
+                            max_value=100,
+                            value=20
                         ),
                         wist.StInteger(
                             label="Figure Height",
                             id="figure_height",
                             min_value=100,
                             max_value=1200,
                             step=1,
@@ -104,29 +100,30 @@
             ]
         ),
         wist.StResource(id="plot"),
         wist.StResource(id="plot_msg"),
         wist.StResource(id="legend_display")
     ]
 
+    @st.cache_data(max_entries=10)
     def get_alpha_diversity(_self, **kwargs) -> Union[None, pd.DataFrame]:
         """Return a table with the alpha diversity metrics for each sample."""
 
         # Get the abundances
         abund = _self._root().abund(
-            level=_self.val("tax_level"),
-            filter=_self.val("filter_by")
+            level=kwargs["tax_level"],
+            filter=kwargs["filter_by"]
         )
 
         # If there are no abundances
         if abund is None:
             return
 
         # Calculate the selected alpha diversity
-        metric = _self.val('metric')
+        metric = kwargs['metric']
         if metric == "Shannon":
             adiv = _self.calc_shannon(abund)
         else:
             msg = f"Unrecognized metric = '{metric}"
             assert metric == "Simpson", msg
             adiv = _self.calc_simpson(abund)
 
@@ -190,15 +187,23 @@
         self.option("plot").main_empty.plotly_chart(fig)
 
         # Print any correlation metrics
         corr_msg = self.report_corr(adiv, kwargs['metric'], kwargs['color_by'])
         if corr_msg is not None:
             self.option("plot_msg").main_empty.write(corr_msg)
 
-    # @st.cache_data
+        # If there is a legend
+        if kwargs['legend'] is not None:
+            self._get_child(
+                "legend_display"
+            ).main_empty.markdown(
+                kwargs['legend']
+            )
+
+    @st.cache_data
     def report_corr(_self, adiv, metric, color_by):
         """Print any correlation metrics."""
 
         if color_by is None or color_by == 'None':
             return
 
         stats_df = adiv.reindex(
@@ -238,67 +243,135 @@
         return adiv
 
     @st.cache_data(max_entries=10)
     def make_fig(_self, adiv, **kwargs):
         """Make the primary figure for plotting."""
 
         # Make the plot
-        if kwargs["plot_type"] == "Distribution":
-            fig = _self.plot_distribution(adiv)
-        elif kwargs["plot_type"] == "Points":
-            fig = _self.plot_points(adiv)
-        elif kwargs["plot_type"] == "Bars":
-            fig = _self.plot_bars(adiv)
-        else:
-            msg = f"Unrecognized plot type {kwargs['plot_type']}"
-            _self.option("plot_msg").main_empty.write(msg)
-            return
+        fig = _self.plot_distribution(adiv, **kwargs)
 
         if kwargs["title"] is not None and kwargs["title"] != "None":
             fig.update_layout(title=kwargs["title"])
 
         return fig
 
-    def plot_distribution(self, adiv: pd.DataFrame):
+    def plot_distribution(
+        self,
+        adiv: pd.DataFrame,
+        metric: str = None,
+        color_by: str = None,
+        nbins: int = 20,
+        **kwargs
+    ):
 
         plot_data = dict(
-            data_frame=adiv,
-            x=self.val("metric")
+            data_frame=adiv.reset_index(),
+            y=metric,
+            hover_name="index",
+            nbins=nbins
         )
         layout = dict(
-            yaxis_title="Number of Samples"
+            xaxis_title="Number of samples"
         )
 
         plot_f = px.histogram
 
         # If there is a grouping
-        color_by = self.val("color_by")
         if color_by is not None and color_by != 'None':
 
             # Only show samples which have the metadata assigned
             plot_data["data_frame"] = plot_data["data_frame"].reindex(
                 columns=[
-                    self.val("metric"),
+                    "index",
+                    metric,
                     color_by
                 ]
             ).dropna()
 
             # If the value is numeric
             if is_numeric(adiv[color_by]):
                 # Make a scatterplot
                 plot_f = px.scatter
-                # With the y-axis as the metadata
-                plot_data["y"] = color_by
-                # Label the y axis
-                layout["yaxis_title"] = color_by
+                # With the x-axis as the metadata
+                plot_data["x"] = color_by
+                # Label the x axis
+                layout["xaxis_title"] = color_by
+                # Add a marginal histogram
+                plot_data["marginal_y"] = "histogram"
+                del plot_data["nbins"]
 
             # If the value is categorical
             else:
-                # Make a facet row
-                plot_data["facet_row"] = color_by
+                # Make a facet column
+                plot_data["facet_col"] = color_by
+
+                # Add the xaxis title for all subplots
+                for i in range(
+                    plot_data["data_frame"][color_by].unique().shape[0]
+                ):
+                    axis_name = 'xaxis' if i == 0 else f'xaxis{i+1}'
+                    if axis_name not in layout:
+                        layout[axis_name] = dict()
+                    layout[axis_name]['title'] = "Number of samples"
+
+        fig = plot_f(**plot_data)
+
+        # Clean up the marginal titles
+        if color_by is not None:
+            fig.for_each_annotation(
+                lambda a: a.update(text=a.text.split("=")[-1])
+            )
+
+        # Apply the layout customizations
+        fig.update_layout(
+            **layout
+        )
+
+        return fig
+
+    def plot_points_bars(
+        self,
+        plot_f,
+        adiv: pd.DataFrame,
+        metric: str = None,
+        color_by: str = None,
+        **kwargs
+    ):
+
+        plot_data = dict(
+            data_frame=adiv.sort_values(
+                by=metric,
+                ascending=False
+            ).reset_index().rename(
+                columns=dict(index="Sample")
+            ),
+            x="Sample",
+            y=metric
+        )
+        layout = dict()
+
+        # If there is a grouping
+        if color_by is not None and color_by != 'None':
+
+            # Only show samples which have the metadata assigned
+            plot_data["data_frame"] = plot_data["data_frame"].reindex(
+                columns=[metric, color_by, "Sample"]
+            ).dropna()
+
+            # Color points
+            plot_data["color"] = color_by
+
+            # If the value is categorical
+            if not is_numeric(adiv[color_by]):
+
+                # Sort by category
+                plot_data["data_frame"] = plot_data["data_frame"].sort_values(
+                    by=[color_by, metric],
+                    ascending=[True, False]
+                )
 
         fig = plot_f(**plot_data)
         fig.update_layout(
             **layout
         )
 
         return fig
@@ -330,10 +403,21 @@
     def anova(
         self,
         adiv: pd.DataFrame,
         metric: str,
         color_by: str
     ) -> None:
 
-        print(color_by)
-        print(metric)
-        print(adiv)
+        r = f_oneway(*[
+            vals
+            for group, vals in adiv[
+                metric
+            ].groupby(
+                adiv[color_by]
+            )
+            if group is not None
+        ])
+        return " ".join([
+            "ANOVA:",
+            f"statistic={r.statistic:.2g},",
+            f"p={r.pvalue:.2g}"
+        ])
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_widget.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/base_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import streamlit as st
 from typing import List, Union
 import numpy as np
 import pandas as pd
 import widgets.streamlit as wist
 from widgets.base.exceptions import WidgetFunctionException
 from living_figures.helpers import parse_numeric
 from living_figures.helpers import is_numeric
@@ -17,27 +18,41 @@
         """
         Return the abundance table
         """
 
         # Get the abundances
         abund: pd.DataFrame = self.get(["data", "abund"])
 
+        # Get the sample annotations
+        sample_annots = self.sample_annotations()
+
+        return self._make_abund(abund, sample_annots, level, filter)
+
+    @st.cache_data
+    def _make_abund(
+        _self,
+        abund: pd.DataFrame,
+        sample_annots: pd.DataFrame,
+        level: str,
+        filter: str
+    ) -> pd.DataFrame:
+
         if abund.shape[0] == 0:
             return
 
         # If the level is not specified
         if level is None:
             # Return everything
             pass
 
         # If a level is specified
         else:
 
             # Get the taxonomic information for each row
-            index_orgs = self.get(["data", "abund"], attr="index_orgs")
+            index_orgs = _self.get(["data", "abund"], attr="index_orgs")
 
             # Filter down to the rows which are assigned at that level
             abund = abund.reindex(
                 index=index_orgs.query(
                     f"level == '{level}'"
                 ).index
             )
@@ -50,17 +65,14 @@
             abund = abund.rename(
                 index=index_orgs['name'].get
             )
 
         # If a filter was specified
         if filter is not None and filter != 'None':
 
-            # Get the sample annotations
-            sample_annots = self.sample_annotations()
-
             # Apply the filter
             query_col, query_val = filter.split(" == ", 1)
             sample_annots = sample_annots.loc[
                 sample_annots[query_col].apply(str) == query_val
             ]
             filtered_samples = set(list(sample_annots.index.values))
 
@@ -222,15 +234,17 @@
     def update_options(self) -> None:
         """Update the menu selection items based on the user inputs."""
 
         # Update the Ordination and Abundant Organism plots
         for plot_type in [
             "ordination",
             "abundant_orgs",
-            "alpha_diversity"
+            "alpha_diversity",
+            "beta_diversity",
+            "differential_abundance",
         ]:
 
             # For each of the elements of this type
             for plot_elem in self._find_child(plot_type):
 
                 # Update the 'color_by' and 'filter_by' menu options
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/inputs.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/inputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,111 @@
 from hashlib import md5
+from typing import Union
 import widgets.streamlit as wist
 import pandas as pd
-from living_figures.bio.fom.utilities import parse_tax_string
+import streamlit as st
+from living_figures.bio.fom.utilities import parse_taxon_abundances
 
 
 class MicrobiomeAbund(wist.StDataFrame):
     """Read in the abundance values of a microbiome datasets."""
 
     label = "Abundance Table"
     hash = None
     index_orgs = None
 
     children = [
         wist.StResource(id='msg')
     ]
 
+    def __init__(
+        self,
+        id="dataframe",
+        value=None,
+        label=None,
+        help: Union[str, None] = None,
+        disabled: bool = False,
+        label_visibility: str = "visible",
+        sidebar=True,
+        show_uploader=True,
+        hash=None,
+        kwargs={}
+    ):
+
+        # Instantiate the hash of the DataFrame
+        self.hash = hash
+
+        super().__init__(
+            id=id,
+            value=value,
+            label=label,
+            help=help,
+            disabled=disabled,
+            label_visibility=label_visibility,
+            sidebar=sidebar,
+            show_uploader=show_uploader,
+            kwargs=kwargs
+        )
+
     def parse_files(self, uploaded_file):
 
         # Read the file
-        self.value: pd.DataFrame = pd.read_csv(
+        df = pd.read_csv(
             uploaded_file,
             index_col=0,
             sep="\t" if "tsv" in uploaded_file.name else ",",
             compression="gzip" if uploaded_file.name.endswith(".gz") else None
         )
-        shape = self.value.shape
-        msg = f"Read {shape[0]:,} rows and {shape[1]:,} columns"
-        self._root().msg(msg)
+
+        # Parse the table of taxonomic abundances
+        self.value, self.index_orgs = self.parse_taxon_abundances(df)
 
         # Compute the hash of the data
         self.hash = md5(self.value.to_csv().encode()).hexdigest()
 
-        # Parse the index column as a taxonomic label
-        self.index_orgs = self.parse_index_orgs()
+        shape = self.value.shape
+        msg = f"Read {shape[0]:,} organisms and {shape[1]:,} samples"
+        self._root().msg(msg)
 
-    def parse_index_orgs(self):
-        """
-        Parse the taxonomic information of the index in the abundance table.
-        """
-
-        return pd.DataFrame([
-            parse_tax_string(org_str)
-            for org_str in self.value.index.values
-        ], index=self.value.index)
+    @st.cache_data(max_entries=10)
+    def parse_taxon_abundances(_self, df):
+        return parse_taxon_abundances(df)
 
 
 class StHashedDataFrame(wist.StDataFrame):
     """Read in a DataFrame and compute a hash."""
 
     hash = None
 
+    def __init__(
+        self,
+        id="dataframe",
+        value=None,
+        label=None,
+        help: Union[str, None] = None,
+        disabled: bool = False,
+        label_visibility: str = "visible",
+        sidebar=True,
+        show_uploader=True,
+        hash=None,
+        kwargs={}
+    ):
+        self.hash = hash
+        super().__init__(
+            id=id,
+            value=value,
+            label=label,
+            help=help,
+            disabled=disabled,
+            label_visibility=label_visibility,
+            kwargs=kwargs,
+            sidebar=sidebar,
+            show_uploader=show_uploader
+        )
+
     def parse_files(self, uploaded_file):
 
         # Read the file
         self.value: pd.DataFrame = pd.read_csv(
             uploaded_file,
             index_col=0,
             sep="\t" if "tsv" in uploaded_file.name else ",",
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/main.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from copy import deepcopy
 from living_figures.bio.fom.widgets.microbiome import MicrobiomeAbund
 from living_figures.bio.fom.widgets.microbiome import StHashedDataFrame
 from living_figures.bio.fom.widgets.microbiome import Ordination
 from living_figures.bio.fom.widgets.microbiome import AbundantOrgs
 from living_figures.bio.fom.widgets.microbiome import AlphaDiversity
+from living_figures.bio.fom.widgets.microbiome import BetaDiversity
+from living_figures.bio.fom.widgets.microbiome import DifferentialAbundance
 from living_figures.bio.fom.widgets.microbiome.base_widget import BaseMicrobiomeExplorer # noqa
 import widgets.streamlit as wist
 
 
 class MicrobiomeExplorer(BaseMicrobiomeExplorer):
     """
     Widget used for the analysis of microbiome data.
@@ -32,14 +34,19 @@
 
         wist.StExpander(
             id="data",
             label="Input Data",
             expanded=True,
             children=[
                 MicrobiomeAbund(id="abund"),
+                wist.StDownloadDataFrame(
+                    target="abund",
+                    label="Download Abundances",
+                    index=True
+                ),
                 StHashedDataFrame(
                     id="annots",
                     label="Sample Annotations"
                 ),
                 wist.StDownloadDataFrame(
                     target="annots",
                     label="Download Annotations"
@@ -51,15 +58,17 @@
             children=[
                 deepcopy(wist.StSelector(
                     id=f"plot_{i}",
                     disable_sidebar=True,
                     options=[
                         AbundantOrgs(id="abundant_orgs"),
                         Ordination(id="ordination"),
-                        AlphaDiversity(id="alpha_diversity")
+                        AlphaDiversity(id="alpha_diversity"),
+                        BetaDiversity(id="beta_diversity"),
+                        DifferentialAbundance(id="differential_abundance")
                     ]
                 ))
                 for i in range(20)
             ],
             value=[True] + [False for _ in range(19)]
         )
     ]
@@ -69,15 +78,18 @@
     ]
 
     extra_imports = [
         "from living_figures.helpers import parse_numeric, is_numeric",
         "import numpy as np",
         "import pandas as pd",
         "from typing import Union, Any, List",
-        "from widgets.base.exceptions import WidgetFunctionException"
+        "from widgets.base.exceptions import WidgetFunctionException",
+        "from living_figures.bio.fom.utilities import parse_taxon_abundances",
+        "from living_figures.bio.fom.widgets.microbiome.base_widget import BaseMicrobiomeExplorer", # noqa
+        "from hashlib import md5"
     ]
 
     def run_self(self):
 
         self.update_options()
 
         self.clone_button(sidebar=True)
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/ordination.py` & `living-figures-0.2.0/src/living_figures/bio/fom/widgets/microbiome/ordination.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from widgets.base.exceptions import WidgetFunctionException
 from living_figures.bio.fom.widgets.microbiome.base_plots import MicrobiomePlot
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
+import streamlit as st
 from living_figures.helpers.constants import tax_levels
 
 
 class Ordination(MicrobiomePlot):
 
     label = "Ordination (PCA/t-SNE)"
 
@@ -77,92 +78,46 @@
             ]
         ),
         wist.StResource(id="plot"),
         wist.StResource(id="ord_msg"),
         wist.StResource(id="legend_display")
     ]
 
-    def make_cache_key(self, val_str: str):
-        """Return a cache key for the plot data."""
-
-        # Get the hash of the input data
-        abund_hash: str = self._root().abund_hash()
-
-        # Set the cache key based on the input data and analysis details
-        cache_key = ":".join(map(
-            str,
-            [
-                abund_hash,
-                self.val('tax_level'),
-                self.val('ord_type'),
-                self.val('3D'),
-                self.val('filter_by'),
-                val_str
-            ]
-        ))
-
-        return cache_key
-
-    def run_ordination(self) -> Union[None, pd.DataFrame]:
+    @st.cache_data(max_entries=10)
+    def run_ordination(
+        _self,
+        tax_level,
+        filter_by,
+        ord_type,
+        abund: pd.DataFrame
+    ) -> Union[None, pd.DataFrame]:
         """Perform ordination on the abundance data."""
 
-        # Get the cache key
-        cache_key = self.make_cache_key("projection")
-
-        # If a value has been computed
-        if self.get_cache(cache_key) is not None:
-
-            # Get the value
-            proj = self.get_cache(cache_key)
-
-            # Return the value
-            if isinstance(proj, str) and proj == "None":
-                return
-            else:
-                return proj
-
-        # The projection needs to be computed
-
-        # Get the plotting options
-        params = self.all_values(flatten=True)
-
-        # Get the abundances, filtering to the specified taxonomic level
-        # Columns are samples, rows are organisms
-        abund: pd.DataFrame = self._root().abund(
-            level=params['tax_level'],
-            filter=params['filter_by']
-        )
-
         # If there are no abundances
         if abund is None:
 
             # Stop
             msg = "No abundances available for ordination"
-            self._get_child("ord_msg").main_empty.write(msg)
-            return
+            return None, None, msg
 
-        msg = f"Running {params['ord_type']} on {abund.shape[1]:,} samples"
+        msg = f"Running {ord_type} on {abund.shape[1]:,} samples"
         msg = f"{msg} using {abund.shape[0]:,}"
-        msg = f"{msg} {params['tax_level']}-level organisms"
-        if params['filter_by'] is not None and params['filter_by'] != 'None':
-            msg = msg + "  \n" + f"Filtering to {params['filter_by']}"
-        self._get_child("ord_msg").main_empty.write(msg)
-
-        if params['ord_type'] == 'PCA':
-            proj, loadings = self.run_pca(abund)
-        elif params['ord_type'] == 't-SNE':
-            proj, loadings = self.run_tsne(abund)
+        msg = f"{msg} {tax_level}-level organisms"
+        if filter_by is not None and filter_by != 'None':
+            msg = msg + "  \n" + f"Filtering to {filter_by}"
+
+        if ord_type == 'PCA':
+            proj, loadings = _self.run_pca(abund)
+        elif ord_type == 't-SNE':
+            proj, loadings = _self.run_tsne(abund)
         else:
             msg = "Ordination type not recognized"
             raise WidgetFunctionException(msg)
 
-        self.set_cache(cache_key, proj)
-        self.set_cache(self.make_cache_key("loadings"), loadings)
-
-        return self.get_cache(cache_key)
+        return proj, loadings, ""
 
     def run_pca(self, abund: pd.DataFrame):
         """Ordinate data using PCA"""
 
         pca = PCA()
         ord_mat = pca.fit_transform(abund.T)
 
@@ -210,92 +165,149 @@
             ]
         )
 
         return coords, None
 
     def run_self(self) -> None:
 
+        # Get all of the plotting parameters
+        params = self.all_values(flatten=True)
+
+        # Get the abundances, filtering to the specified taxonomic level
+        # Columns are samples, rows are organisms
+        abund: pd.DataFrame = self._root().abund(
+            level=params["tax_level"],
+            filter=params["filter_by"]
+        )
+
+        # Get the sample annotations
+        sample_annots = self._root().sample_annotations()
+
+        fig, msg = self.build_fig(
+            params["tax_level"],
+            params["filter_by"],
+            params["ord_type"],
+            abund,
+            sample_annots,
+            params["3D"],
+            params["color_by"],
+            params["title"],
+            params["pca_loadings"],
+        )
+
+        if msg is not None and len(msg) > 0:
+            self._get_child("ord_msg").main_empty.write(msg)
+        if fig is None:
+            return
+
+        # Add the plot to the display
+        self._get_child("plot").main_empty.plotly_chart(fig)
+
+        # If there is a legend
+        if params['legend'] is not None:
+            self._get_child(
+                "legend_display"
+            ).main_empty.markdown(
+                params['legend']
+            )
+
+    @st.cache_data(max_entries=10)
+    def build_fig(
+        _self,
+        tax_level,
+        filter_by,
+        ord_type,
+        abund,
+        sample_annots,
+        is_3d,
+        color_by,
+        title,
+        pca_loadings
+    ):
+
         # Get the ordinated data
-        plot_df = self.run_ordination()
+        plot_df, loadings, msg = _self.run_ordination(
+            tax_level,
+            filter_by,
+            ord_type,
+            abund
+        )
+
         if plot_df is None:
-            return
+            return None, msg
 
         # Add the metadata (if any was provided)
-        sample_annots = self._root().sample_annotations()
         if sample_annots is not None:
             plot_df = plot_df.merge(
                 sample_annots,
                 left_index=True,
                 right_index=True
             )
 
         # Get the coloring column
-        color_by = self.val("color_by")
         if color_by == 'None':
             color_by = None
 
         # Set up the data which will be used to build the plot
         plot_kwargs = dict(
-            data_frame=plot_df,
+            data_frame=plot_df.reset_index(
+            ).rename(
+                columns=dict(index="sample")
+            ),
             x=plot_df.columns.values[0],
             y=plot_df.columns.values[1],
+            hover_data=[
+                plot_df.columns.values[0],
+                plot_df.columns.values[1],
+                "sample"
+            ],
             color=color_by
         )
+        if color_by is not None:
+            plot_kwargs["hover_data"].append(color_by)
 
         # If the 3D plot was requested
-        if self.val("3D"):
+        if is_3d:
             plot_f = px.scatter_3d
             plot_kwargs['z'] = plot_df.columns.values[2]
         else:
             plot_f = px.scatter
 
         # Make a plot
         fig = plot_f(**plot_kwargs)
 
         # Add the PCA loadings, if requested
-        self.add_pca_loadings(fig, plot_df)
+        if pca_loadings:
+            _self.add_pca_loadings(
+                fig,
+                plot_df,
+                loadings,
+                is_3d
+            )
 
         # If there is a title
-        title = self.val("title")
         if title is not None and title != "None":
             fig.update_layout(title=title)
 
-        # Add the plot to the display
-        self._get_child("plot").main_empty.plotly_chart(fig)
-
-        # If there is a legend
-        legend = self.val("legend")
-        if legend is not None:
-            self._get_child(
-                "legend_display"
-            ).main_empty.markdown(legend)
-
-    def add_pca_loadings(self, fig, plot_df):
-
-        if not self.val("pca_loadings"):
-            return
-
-        # Get the key used in the cache for the loadings
-        cache_key = self.make_cache_key("loadings")
-
-        # If there is no value in the cache
-        if self.get_cache(cache_key) is None:
-            # Run the ordination to make sure that the cache
-            # is current
-            _ = self.run_ordination()
+        return fig, msg
 
-        # Get any value in the cache
-        loadings = self.get_cache(cache_key)
+    def add_pca_loadings(
+        self,
+        fig,
+        plot_df,
+        loadings,
+        is_3d
+    ):
 
         # If no value has been computed
         if loadings is None:
             return
 
         # Number of dimensions
-        ndims = 2 + self.val("3D")
+        ndims = 2 + is_3d
 
         # Just pick the number of axes used in the plot
         loadings = loadings.head(ndims)
 
         # Score the organisms based on the absolute sum of loadings
         org_score = loadings.abs().sum()
```

### Comparing `living-figures-0.1.5/src/living_figures/bio/volcano/app.py` & `living-figures-0.2.0/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.2.0/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/helpers/parse_numeric.py` & `living-figures-0.2.0/src/living_figures/helpers/parse_numeric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pandas as pd
+import streamlit as st
 
 
 def parse_numeric(df: pd.DataFrame) -> pd.DataFrame:
     """
     Convert any column to numeric which does not change the number of nulls.
     """
 
     for cname in df.columns.values:
         if is_numeric(df[cname]):
             df[cname] = df[cname].apply(pd.to_numeric, errors='coerce')
 
     return df
 
 
+@st.cache_data(max_entries=10)
 def is_numeric(r: pd.Series) -> bool:
     """Whether a column is numeric (after nulls are dropped)."""
 
     numeric_vals = r.apply(pd.to_numeric, errors='coerce')
     new_nonnull = numeric_vals.dropna().shape[0]
     return new_nonnull > 0 and new_nonnull == r.dropna().shape[0]
```

### Comparing `living-figures-0.1.5/src/living_figures/helpers/scaling.py` & `living-figures-0.2.0/src/living_figures/helpers/scaling.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures/helpers/sorting.py` & `living-figures-0.2.0/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.5/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.2.0/src/living_figures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.5
+Version: 0.2.0
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.5/src/living_figures.egg-info/SOURCES.txt` & `living-figures-0.2.0/src/living_figures.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,19 +18,22 @@
 src/living_figures/bio/epigenome/utilities/parse_rebase.py
 src/living_figures/bio/epigenome/utilities/rebase_file.py
 src/living_figures/bio/epigenome/widgets/__init__.py
 src/living_figures/bio/epigenome/widgets/panepibrowser.py
 src/living_figures/bio/fom/__init__.py
 src/living_figures/bio/fom/utilities/__init__.py
 src/living_figures/bio/fom/utilities/parse_tax_string.py
+src/living_figures/bio/fom/utilities/parse_taxon_abundances.py
 src/living_figures/bio/fom/widgets/microbiome/__init__.py
 src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
 src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py
 src/living_figures/bio/fom/widgets/microbiome/base_plots.py
 src/living_figures/bio/fom/widgets/microbiome/base_widget.py
+src/living_figures/bio/fom/widgets/microbiome/beta_diversity.py
+src/living_figures/bio/fom/widgets/microbiome/differential_abundance.py
 src/living_figures/bio/fom/widgets/microbiome/inputs.py
 src/living_figures/bio/fom/widgets/microbiome/main.py
 src/living_figures/bio/fom/widgets/microbiome/ordination.py
 src/living_figures/bio/volcano/__init__.py
 src/living_figures/bio/volcano/app.py
 src/living_figures/bio/volcano/make_test_data.py
 src/living_figures/helpers/__init__.py
```

### Comparing `living-figures-0.1.5/tests/test_import.py` & `living-figures-0.2.0/tests/test_import.py`

 * *Files identical despite different names*

