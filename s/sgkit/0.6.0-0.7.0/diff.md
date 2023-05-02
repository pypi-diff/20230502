# Comparing `tmp/sgkit-0.6.0.tar.gz` & `tmp/sgkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgkit-0.6.0.tar", last modified: Wed Feb  1 13:18:35 2023, max compression
+gzip compressed data, was "sgkit-0.7.0.tar", last modified: Tue May  2 11:10:44 2023, max compression
```

## Comparing `sgkit-0.6.0.tar` & `sgkit-0.7.0.tar`

### file list

```diff
@@ -1,110 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-01 13:18:22.000000 sgkit-0.6.0/.cirun.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-01 13:18:22.000000 sgkit-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-01 13:18:22.000000 sgkit-0.6.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-01 13:18:22.000000 sgkit-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-01 13:18:22.000000 sgkit-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-01 13:18:35.969822 sgkit-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-01 13:18:22.000000 sgkit-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.961822 sgkit-0.6.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:22.000000 sgkit-0.6.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-02-01 13:18:22.000000 sgkit-0.6.0/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-01 13:18:22.000000 sgkit-0.6.0/benchmarks/benchmarks_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-01 13:18:22.000000 sgkit-0.6.0/benchmarks/benchmarks_vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.961822 sgkit-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    32468 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/data-structures-xarray.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/docsearch.sbt.css
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/docsearch.sbt.js
--rw-r--r--   0 runner    (1001) docker     (123)    54048 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/mydask.png
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/numfocus_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    40680 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/order.png
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/sgkit_blue_trnsprnt.png
--rw-r--r--   0 runner    (1001) docker     (123)    33737 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/sgkit_trnsprnt.png
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/_static/switcher.json
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  1335792 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/examples/gwas_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/examples/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/how_do_i.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/docs/news/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/news/introducing_sgkit.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/news.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18321 2023-02-01 13:18:22.000000 sgkit-0.6.0/docs/vcf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-01 13:18:22.000000 sgkit-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-01 13:18:22.000000 sgkit-0.6.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-01 13:18:22.000000 sgkit-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-02-01 13:18:35.973822 sgkit-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-01 13:18:22.000000 sgkit-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/sgkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/accelerate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/distance/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/distance/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/io/bgen/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/bgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22661 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/bgen/bgen_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/io/plink/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/plink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/plink/plink_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/io/vcf/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/csi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/tbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/vcf_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/vcf_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/vcf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcf/vcf_writer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/io/vcfzarr_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.969822 sgkit-0.6.0/sgkit/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/association.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/genee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/genee_momentchi2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/grm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/hwe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/ibs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/ld.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/pc_relate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    73355 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)    35393 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/popgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    36357 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/regenie.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/stats/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35255 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-02-01 13:18:22.000000 sgkit-0.6.0/sgkit/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 13:18:35.965822 sgkit-0.6.0/sgkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 13:18:35.000000 sgkit-0.6.0/sgkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.208659 sgkit-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-02 11:10:31.000000 sgkit-0.7.0/.cirun.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 11:10:31.000000 sgkit-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 11:10:31.000000 sgkit-0.7.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:10:31.000000 sgkit-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 11:10:31.000000 sgkit-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 11:10:44.208659 sgkit-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 11:10:31.000000 sgkit-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.188658 sgkit-0.7.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:31.000000 sgkit-0.7.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-02 11:10:31.000000 sgkit-0.7.0/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 11:10:31.000000 sgkit-0.7.0/benchmarks/benchmarks_plink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-02 11:10:31.000000 sgkit-0.7.0/benchmarks/benchmarks_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-02 11:10:31.000000 sgkit-0.7.0/benchmarks/benchmarks_vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.192658 sgkit-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.192658 sgkit-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    32468 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/data-structures-xarray.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/docsearch.sbt.css
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/docsearch.sbt.js
+-rw-r--r--   0 runner    (1001) docker     (123)    54048 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/mydask.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/numfocus_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40680 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/order.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/sgkit_blue_trnsprnt.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33737 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/sgkit_trnsprnt.png
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/_static/switcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.196658 sgkit-0.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  1335792 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/examples/gwas_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/examples/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.196658 sgkit-0.7.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/how_do_i.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.196658 sgkit-0.7.0/docs/news/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/news/introducing_sgkit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18321 2023-05-02 11:10:31.000000 sgkit-0.7.0/docs/vcf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 11:10:31.000000 sgkit-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-02 11:10:31.000000 sgkit-0.7.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 11:10:31.000000 sgkit-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-02 11:10:44.220659 sgkit-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 11:10:31.000000 sgkit-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.196658 sgkit-0.7.0/sgkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/accelerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/display_numba_fns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.200658 sgkit-0.7.0/sgkit/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/distance/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/distance/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.200658 sgkit-0.7.0/sgkit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.200658 sgkit-0.7.0/sgkit/io/bgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/bgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/bgen/bgen_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.200658 sgkit-0.7.0/sgkit/io/plink/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/plink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/plink/plink_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/plink/plink_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.204659 sgkit-0.7.0/sgkit/io/vcf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/csi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/tbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/vcf_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55890 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/vcf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/vcf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcf/vcf_writer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/io/vcfzarr_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.208659 sgkit-0.7.0/sgkit/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35606 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/aggregation_numba_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/cohort_numba_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/conversion_numba_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/genee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/genee_momentchi2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/grm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/hwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/ibs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/ld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/pc_relate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72858 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30669 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/popgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/popgen_numba_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36357 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/regenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/stats/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37725 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21177 2023-05-02 11:10:31.000000 sgkit-0.7.0/sgkit/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:10:44.200658 sgkit-0.7.0/sgkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 11:10:43.000000 sgkit-0.7.0/sgkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-02 11:10:44.000000 sgkit-0.7.0/sgkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:10:43.000000 sgkit-0.7.0/sgkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:10:43.000000 sgkit-0.7.0/sgkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 11:10:43.000000 sgkit-0.7.0/sgkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 11:10:43.000000 sgkit-0.7.0/sgkit.egg-info/top_level.txt
```

### Comparing `sgkit-0.6.0/.cirun.yml` & `sgkit-0.7.0/.cirun.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # Cheapest GPU on GCP
     gpu: nvidia-tesla-t4
     # Cheapest VM on GCP, with GPU attachable
     instance_type: n1-standard-1
     # Custom image with NVIDIA drivers installed on Ubuntu-20.4
     # to reduce provision time
     # Format => project_name:image_name
-    machine_image: sgkit-dev:cirun-nvidia
+    machine_image: sgkit-dev:cirun-nvidia-v2
     region:
       - us-central1-a
       - us-central1-b
       - us-central1-c
       - us-central1-f
       - us-east1-c
       - us-east1-d
```

### Comparing `sgkit-0.6.0/LICENSE` & `sgkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/PKG-INFO` & `sgkit-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgkit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Statistical genetics toolkit
 Home-page: https://github.com/pystatgen/sgkit
 Author: sgkit Developers
 Author-email: project@pystatgen.org
 License: Apache
 Description: 
         **sgkit** is an open source project for analyzing and manipulating genetic
```

### Comparing `sgkit-0.6.0/README.md` & `sgkit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/benchmarks/asv.conf.json` & `sgkit-0.7.0/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/benchmarks/benchmarks_stats.py` & `sgkit-0.7.0/benchmarks/benchmarks_stats.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/benchmarks/benchmarks_vcf.py` & `sgkit-0.7.0/benchmarks/benchmarks_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from sgkit.io.vcf.vcf_reader import vcf_to_zarr, zarr_array_sizes
 from sgkit.io.vcf.vcf_writer import zarr_to_vcf
 
 
 class VcfSpeedSuite:
     def setup(self) -> None:
-
         asv_env_dir = os.environ["ASV_ENV_DIR"]
         path = Path(
             asv_env_dir,
             "project/sgkit/tests/io/vcf/data/1000G.phase3.broad.withGenotypes.chr20.10100000.vcf.gz",
         )
         tmp_path = Path(tempfile.mkdtemp())
         self.input_vcf = tmp_path.joinpath("1000G.in.vcf").as_posix()
@@ -78,28 +77,26 @@
 
 def _to_mb_per_s(bytes, duration):
     return bytes / (1_000_000 * duration)
 
 
 class VcfCompressionSuite:
     def setup(self) -> None:
-
         asv_env_dir = os.environ["ASV_ENV_DIR"]
         self.input_vcf = Path(
             asv_env_dir,
             "project/sgkit/tests/io/vcf/data/1kg_target_chr20_38_imputed_chr20_500000.vcf.bgz",
         )
 
         tmp_path = Path(tempfile.mkdtemp())
         self.output_zarr = tmp_path.joinpath("1000G.out.zarr")
 
     # use track_* asv methods since we want to measure compression size not time
 
     def track_zarr_compression_size(self) -> None:
-
         encoding = {
             "variant_AF": {
                 "filters": [
                     FixedScaleOffset(offset=0, scale=10000, dtype="f4", astype="u2")
                 ],
             },
             "call_DS": {
```

### Comparing `sgkit-0.6.0/docs/Makefile` & `sgkit-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/data-structures-xarray.jpg` & `sgkit-0.7.0/docs/_static/data-structures-xarray.jpg`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/mydask.png` & `sgkit-0.7.0/docs/_static/mydask.png`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/numfocus_logo.png` & `sgkit-0.7.0/docs/_static/numfocus_logo.png`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/order.png` & `sgkit-0.7.0/docs/_static/order.png`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/sgkit_blue_trnsprnt.png` & `sgkit-0.7.0/docs/_static/sgkit_blue_trnsprnt.png`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/sgkit_trnsprnt.png` & `sgkit-0.7.0/docs/_static/sgkit_trnsprnt.png`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/_static/switcher.json` & `sgkit-0.7.0/docs/_static/switcher.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'2': "{'name': '0.5.0'}",*

 * * 'insert': "[(1, OrderedDict([('name', '0.6.0 (stable)'), ('version', '0.6.0'), ('url', "*

 * *           "'https://pystatgen.github.io/sgkit/0.6.0/')]))]"}*

```diff
@@ -1,14 +1,19 @@
 [
     {
         "url": "https://pystatgen.github.io/sgkit/latest/",
         "version": "latest"
     },
     {
-        "name": "0.5.0 (stable)",
+        "name": "0.6.0 (stable)",
+        "url": "https://pystatgen.github.io/sgkit/0.6.0/",
+        "version": "0.6.0"
+    },
+    {
+        "name": "0.5.0",
         "url": "https://pystatgen.github.io/sgkit/0.5.0/",
         "version": "0.5.0"
     },
     {
         "url": "https://pystatgen.github.io/sgkit/0.4.0/",
         "version": "0.4.0"
     },
```

### Comparing `sgkit-0.6.0/docs/about.rst` & `sgkit-0.7.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/api.rst` & `sgkit-0.7.0/docs/api.rst`

 * *Files 15% similar despite different names*

```diff
@@ -23,34 +23,39 @@
 PLINK
 -----
 
 .. currentmodule:: sgkit.io.plink
 .. autosummary::
    :toctree: generated/
 
+   plink_to_zarr
    read_plink
+   write_plink
+   zarr_to_plink
 
 VCF (reading)
 -------------
 
 .. currentmodule:: sgkit.io.vcf
 .. autosummary::
    :toctree: generated/
 
+   read_vcf
    vcf_to_zarr
 
 For more low-level control:
 
 .. currentmodule:: sgkit.io.vcf
 .. autosummary::
    :toctree: generated/
 
    partition_into_regions
    vcf_to_zarrs
    concat_zarrs
+   zarr_array_sizes
 
 For converting from `scikit-allel's VCF Zarr representation <https://scikit-allel.readthedocs.io/en/stable/io.html#allel.vcf_to_zarr>`_ to sgkit's Zarr representation:
 
 .. currentmodule:: sgkit
 .. autosummary::
    :toctree: generated/
 
@@ -94,14 +99,16 @@
    diversity
    Fst
    Garud_H
    genee
    genomic_relationship
    gwas_linear_regression
    hardy_weinberg_test
+   hybrid_inverse_relationship
+   hybrid_relationship
    identity_by_state
    individual_heterozygosity
    ld_matrix
    ld_prune
    maximal_independent_set
    observed_heterozygosity
    pbs
@@ -117,20 +124,22 @@
 
 Utilities
 =========
 
 .. autosummary::
    :toctree: generated/
 
+   convert_call_to_index
    convert_probability_to_call
    display_genotypes
    filter_partial_calls
    infer_call_ploidy
    infer_sample_ploidy
    infer_variant_ploidy
+   invert_relationship_matrix
    parent_indices
    simulate_genotype_call_dataset
    window_by_genome
    window_by_interval
    window_by_position
    window_by_variant
 
@@ -152,14 +161,16 @@
     variables.call_genotype_complete_mask_spec
     variables.call_genotype_spec
     variables.call_genotype_mask_spec
     variables.call_genotype_fill_spec
     variables.call_genotype_phased_spec
     variables.call_genotype_probability_spec
     variables.call_genotype_probability_mask_spec
+    variables.call_genotype_index_spec
+    variables.call_genotype_index_mask_spec
     variables.call_heterozygosity_spec
     variables.call_ploidy_spec
     variables.cohort_allele_count_spec
     variables.cohort_allele_frequency_spec
     variables.covariates_spec
     variables.interval_contig_name_spec
     variables.interval_start_spec
@@ -188,18 +199,22 @@
     variables.stat_divergence_spec
     variables.stat_diversity_spec
     variables.stat_Fst_spec
     variables.stat_Garud_h1_spec
     variables.stat_Garud_h12_spec
     variables.stat_Garud_h123_spec
     variables.stat_Garud_h2_h1_spec
+    variables.stat_genomic_kinship_spec
     variables.stat_genomic_relationship_spec
     variables.stat_Hamilton_Kerr_lambda_spec
     variables.stat_Hamilton_Kerr_tau_spec
+    variables.stat_hybrid_relationship_spec
+    variables.stat_hybrid_inverse_relationship_spec
     variables.stat_identity_by_state_spec
+    variables.stat_inverse_relationship_spec
     variables.stat_observed_heterozygosity_spec
     variables.stat_pbs_spec
     variables.stat_pedigree_inbreeding_spec
     variables.stat_pedigree_inverse_kinship_spec
     variables.stat_pedigree_inverse_relationship_spec
     variables.stat_pedigree_kinship_spec
     variables.stat_pedigree_relationship_spec
```

### Comparing `sgkit-0.6.0/docs/conf.py` & `sgkit-0.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 # https://pydata-sphinx-theme.readthedocs.io/en/latest/user_guide/configuring.html
 html_theme_options = {
     "github_url": "https://github.com/pystatgen/sgkit",
     "logo": {
         "image_light": "sgkit_trnsprnt.png",
         "image_dark": "sgkit_blue_trnsprnt.png",
     },
+    # https://github.com/pydata/pydata-sphinx-theme/issues/1220
+    "icon_links": [],
     "navbar_end": ["version-switcher", "theme-switcher", "navbar-icon-links"],
     "switcher": {
         "json_url": "_static/switcher.json",
         "version_match": version,
     },
 }
```

### Comparing `sgkit-0.6.0/docs/contributing.rst` & `sgkit-0.7.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/examples/gwas_tutorial.ipynb` & `sgkit-0.7.0/docs/examples/gwas_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/extensions/typed_returns.py` & `sgkit-0.7.0/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/getting_started.rst` & `sgkit-0.7.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/how_do_i.rst` & `sgkit-0.7.0/docs/how_do_i.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/index.rst` & `sgkit-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/news/introducing_sgkit.md` & `sgkit-0.7.0/docs/news/introducing_sgkit.md`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/docs/vcf.rst` & `sgkit-0.7.0/docs/vcf.rst`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/setup.cfg` & `sgkit-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/__init__.py` & `sgkit-0.7.0/sgkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,22 @@
     infer_call_ploidy,
     infer_sample_ploidy,
     infer_variant_ploidy,
     sample_stats,
     variant_stats,
 )
 from .stats.association import gwas_linear_regression, regenie_loco_regression
-from .stats.conversion import convert_probability_to_call
+from .stats.conversion import convert_call_to_index, convert_probability_to_call
 from .stats.genee import genee
-from .stats.grm import genomic_relationship
+from .stats.grm import (
+    genomic_relationship,
+    hybrid_inverse_relationship,
+    hybrid_relationship,
+    invert_relationship_matrix,
+)
 from .stats.hwe import hardy_weinberg_test
 from .stats.ibs import Weir_Goudet_beta, identity_by_state
 from .stats.ld import ld_matrix, ld_prune, maximal_independent_set
 from .stats.pc_relate import pc_relate
 from .stats.pca import pca
 from .stats.pedigree import (
     parent_indices,
@@ -69,14 +74,15 @@
     "DIM_ALLELE",
     "DIM_PLOIDY",
     "DIM_SAMPLE",
     "DIM_VARIANT",
     "call_allele_frequencies",
     "create_genotype_call_dataset",
     "cohort_allele_frequencies",
+    "convert_call_to_index",
     "convert_probability_to_call",
     "count_variant_alleles",
     "count_call_alleles",
     "count_cohort_alleles",
     "count_variant_genotypes",
     "create_genotype_dosage_dataset",
     "display_genotypes",
@@ -84,19 +90,22 @@
     "genee",
     "genomic_relationship",
     "gwas_linear_regression",
     "read_scikit_allel_vcfzarr",
     "regenie",
     "regenie_loco_regression",
     "hardy_weinberg_test",
+    "hybrid_relationship",
+    "hybrid_inverse_relationship",
     "identity_by_state",
     "individual_heterozygosity",
     "infer_call_ploidy",
     "infer_sample_ploidy",
     "infer_variant_ploidy",
+    "invert_relationship_matrix",
     "ld_matrix",
     "ld_prune",
     "maximal_independent_set",
     "parent_indices",
     "pedigree_inbreeding",
     "pedigree_inverse_kinship",
     "pedigree_kinship",
```

### Comparing `sgkit-0.6.0/sgkit/accelerate.py` & `sgkit-0.7.0/sgkit/accelerate.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/cohorts.py` & `sgkit-0.7.0/sgkit/cohorts.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/display.py` & `sgkit-0.7.0/sgkit/display.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Any, Hashable, Mapping, Tuple
 
+import numpy as np
 import pandas as pd
 import xarray as xr
 
+from sgkit.typing import ArrayLike
+
 
 class GenotypeDisplay:
     """
     A printable object to display genotype information.
     """
 
     def __init__(
@@ -52,14 +55,50 @@
                 return self.df._repr_html_().replace(
                     "</div>",
                     f"<p>{self.shape[0]} rows x {self.shape[1]} columns</p></div>",
                 )
             return self.df._repr_html_()
 
 
+def genotype_as_bytes(
+    genotype: ArrayLike,
+    phased: ArrayLike,
+    max_allele_chars: int = 2,
+) -> ArrayLike:
+    """Convert integer encoded genotype calls to (unphased)
+    VCF style byte strings.
+
+    Parameters
+    ----------
+    genotype
+        Genotype call.
+    phased
+        Boolean indicating if genotype is phased.
+    max_allele_chars
+        Maximum number of chars required for any allele.
+        This should include signed sentinel values.
+
+    Returns
+    -------
+    genotype_string
+        Genotype encoded as byte string.
+    """
+    from .display_numba_fns import _format_genotype_bytes
+
+    ploidy = genotype.shape[-1]
+    b = genotype.astype("|S{}".format(max_allele_chars))
+    b.dtype = np.uint8
+    n_num = b.shape[-1]
+    n_char = n_num + ploidy - 1
+    dummy = np.empty(n_char, np.uint8)
+    c = _format_genotype_bytes(b, ploidy, phased, dummy)
+    c.dtype = "|S{}".format(n_char)
+    return np.squeeze(c)
+
+
 def truncate(ds: xr.Dataset, max_sizes: Mapping[Hashable, int]) -> xr.Dataset:
     """Truncate a dataset along two dimensions into a form suitable for display.
 
     Truncation involves taking four rectangles from each corner of the dataset array
     (or arrays) and combining them into a smaller dataset array (or arrays).
 
     Parameters
@@ -77,60 +116,26 @@
 
     Warnings
     --------
     A maximum size of `n` may result in the array having size `n + 2` (and not `n`).
     The reason for this is so that pandas can be used to display the array as a table,
     and correctly truncate rows or columns (shown as ellipses ...).
     """
-
-    if len(max_sizes) != 2:
-        raise ValueError("Truncation is only supported for two dimensions")
-
-    dims = list(max_sizes.keys())
-    max_dim = max_sizes[dims[0]], max_sizes[dims[1]]
-    n_dim = ds.sizes[dims[0]], ds.sizes[dims[1]]
-
-    if n_dim[0] <= max_dim[0] + 2 and n_dim[1] <= max_dim[1] + 2:
-        # No truncation required
-        return ds
-
-    if n_dim[0] <= max_dim[0] + 1:
-        # Truncate dim1 only
-        m_dim = n_dim[0], max_dim[1] // 2 + 1
-        rows = [[(0, 0), (0, m_dim[1])]]
-    elif n_dim[1] <= max_dim[1] + 1:
-        # Truncate dim0 only
-        m_dim = max_dim[0] // 2 + 1, n_dim[1]
-        rows = [[(0, 0)], [(m_dim[0], 0)]]
-    else:
-        # Truncate both dimensions
-        m_dim = max_dim[0] // 2 + 1, max_dim[1] // 2 + 1
-        rows = [[(0, 0), (0, m_dim[1])], [(m_dim[0], 0), (m_dim[0], m_dim[1])]]
-
-    limits = {dims[0]: m_dim[0], dims[1]: m_dim[1]}
-    slices = {k: slice(v) for k, v in limits.items()}
-    ds_abbr: xr.Dataset = xr.combine_nested(
-        [
-            [
-                # Roll all of these simultaneously along with any indexes/coords
-                # and then clip them using the same slice for each corner
-                ds.roll(dict(zip(limits, roll)), roll_coords=True).isel(  # type: ignore[misc]
-                    **slices  # type: ignore[arg-type]
-                )
-                for roll in row
-            ]
-            for row in rows
-        ],
-        concat_dim=limits.keys(),  # type: ignore[arg-type]
-    )
-
-    assert ds_abbr.sizes[dims[0]] <= max_dim[0] + 2
-    assert ds_abbr.sizes[dims[1]] <= max_dim[1] + 2
-
-    return ds_abbr
+    sel = dict()
+    for dim, size in max_sizes.items():
+        if ds.dims[dim] <= size:
+            # No truncation required
+            pass
+        else:
+            n_head = size // 2 + size % 2 + 1  # + 1 for ellipses
+            n_tail = -size // 2
+            head = ds[dim][0:n_head]
+            tail = ds[dim][n_tail:]
+            sel[dim] = np.append(head, tail)
+    return ds.sel(sel)
 
 
 def set_index_if_unique(ds: xr.Dataset, dim: str, index: str) -> xr.Dataset:
     ds_with_index = ds.set_index({dim: index})
     idx = ds_with_index.get_index(dim)
     if len(idx) != len(idx.unique()):
         # index is not unique so don't use it
@@ -163,50 +168,44 @@
         The maximum number of samples (columns) to display. If there are
         more samples than this then the table is truncated.
 
     Returns
     -------
     A printable object to display genotype information.
     """
-
-    # Create a copy to avoid clobbering original indexes
-    ds_calls = ds.copy()
-
-    # Set indexes only if not already set (allows users to have different row/col labels)
-    # and if setting them produces a unique index
+    # create a truncated dataset with required variables
+    variables = ["call_genotype", "sample_id"]
+    if "call_genotype_phased" in ds:
+        variables.append("call_genotype_phased")
+    if "variant_id" in ds:
+        variables.append("variant_id")
+    else:
+        variables.append("variant_position")
+    ds_calls = ds[variables]
+    ds_calls = truncate(
+        ds_calls, max_sizes={"variants": max_variants, "samples": max_samples}
+    )
     if isinstance(ds_calls.get_index("samples"), pd.RangeIndex):
         ds_calls = set_index_if_unique(ds_calls, "samples", "sample_id")
     if isinstance(ds_calls.get_index("variants"), pd.RangeIndex):
         variant_index = "variant_id" if "variant_id" in ds_calls else "variant_position"
         ds_calls = set_index_if_unique(ds_calls, "variants", variant_index)
-
-    # Restrict to genotype call variables
+    # convert call genotypes to strings
+    calls = ds_calls["call_genotype"].values
+    max_chars = max(2, len(str(ds.dims["alleles"] - 1)))
     if "call_genotype_phased" in ds_calls:
-        ds_calls = ds_calls[
-            ["call_genotype", "call_genotype_mask", "call_genotype_phased"]
-        ]
+        phased = ds_calls["call_genotype_phased"].values
     else:
-        ds_calls = ds_calls[["call_genotype", "call_genotype_mask"]]
-
-    # Truncate the dataset then convert to a dataframe
-    ds_abbr = truncate(
-        ds_calls, max_sizes={"variants": max_variants, "samples": max_samples}
-    )
-    df = ds_abbr.to_dataframe().unstack(level="ploidy")
-
-    # Convert each genotype to a string representation
-    def calls_to_str(r: pd.DataFrame) -> str:
-        gt = r["call_genotype"].astype(str)
-        gt_mask = r["call_genotype_mask"].astype(bool)
-        gt[gt_mask] = "."
-        if "call_genotype_phased" in r and r["call_genotype_phased"][0]:
-            return "|".join(gt)
-        return "/".join(gt)
-
-    df = df.apply(calls_to_str, axis=1).unstack("samples")
-
+        phased = False
+    strings = genotype_as_bytes(calls, phased, max_chars).astype("U")
+    # wrap them in a dataframe
+    df = pd.DataFrame(strings)
+    df.columns = ds_calls["samples"].values
+    df.columns.name = "samples"
+    df.index = ds_calls["variants"].values
+    df.index.name = "variants"
     return GenotypeDisplay(
         df,
         (ds.sizes["variants"], ds.sizes["samples"]),
         max_variants,
         max_samples,
     )
```

### Comparing `sgkit-0.6.0/sgkit/distance/api.py` & `sgkit-0.7.0/sgkit/distance/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 
 import dask.array as da
 import numpy as np
 from typing_extensions import Literal
 
-from sgkit.distance import metrics
 from sgkit.typing import ArrayLike
 
 MetricTypes = Literal["euclidean", "correlation"]
 DeviceTypes = Literal["cpu", "gpu"]
 
 
 def pairwise_distance(
@@ -94,14 +93,16 @@
 
     >>> x = np.array([[6, 4, 1,], [4, 5, 2], [9, 7, 3]])
     >>> pairwise_distance(x, metric='correlation').compute()
     array([[-4.44089210e-16,  2.62956526e-01,  2.82353505e-03],
            [ 2.62956526e-01,  0.00000000e+00,  2.14285714e-01],
            [ 2.82353505e-03,  2.14285714e-01,  0.00000000e+00]])
     """
+    from sgkit.distance import metrics  # defer numba compilation
+
     valid_devices = DeviceTypes.__args__  # type: ignore[attr-defined]
     if device not in valid_devices:
         raise ValueError(
             f"Invalid Device, expected one of {valid_devices}, got: {device}"
         )
     try:
         map_func_name = f"{metric}_map_{device}"
```

### Comparing `sgkit-0.6.0/sgkit/distance/metrics.py` & `sgkit-0.7.0/sgkit/distance/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,21 @@
 
     # In future when we have an average GPU with ability to have
     # more number of threads per block, we can increase this to that value
     # or parameterise this from the pairwise function or get the maximum
     # possible value for a given compute capability.
 
     threads_per_block = (32, 32)
+    # Minimum grid size is 128 (12*12 = 144)
+    # Ref: https://github.com/numba/numba/blob/008077553b558bd183668ecd581d4d0bc54bd32c/numba/cuda/dispatcher.py#L534
+    default_blocks_per_grid = (12, 12)
+
     blocks_per_grid = (
-        math.ceil(out.shape[0] / threads_per_block[0]),
-        math.ceil(out.shape[1] / threads_per_block[1]),
+        max(default_blocks_per_grid[0], math.ceil(out.shape[0] / threads_per_block[0])),
+        max(default_blocks_per_grid[1], math.ceil(out.shape[1] / threads_per_block[1])),
     )
 
     metric_kernel[blocks_per_grid, threads_per_block](d_a, d_b, d_out)
     # copy the output array back to the host system
     d_out_host = d_out.copy_to_host()
     return d_out_host
```

### Comparing `sgkit-0.6.0/sgkit/io/bgen/bgen_reader.py` & `sgkit-0.7.0/sgkit/io/bgen/bgen_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         ("a2", "S"),
         ("offset", "int64"),
     ]
 )
 
 
 class BgenReader:
-
     name = "bgen_reader"
 
     def __init__(
         self,
         path: PathType,
         metafile_path: Optional[PathType] = None,
         dtype: DType = "float32",
```

### Comparing `sgkit-0.6.0/sgkit/io/dataset.py` & `sgkit-0.7.0/sgkit/io/dataset.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/plink/plink_reader.py` & `sgkit-0.7.0/sgkit/io/plink/plink_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """PLINK 1.9 reader implementation"""
 from pathlib import Path
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Dict, List, MutableMapping, Optional, Tuple, Union
 
 import dask.array as da
 import dask.dataframe as dd
 import numpy as np
 from bed_reader import open_bed
 from dask.dataframe import DataFrame
 from xarray import Dataset
 
-from sgkit import create_genotype_call_dataset
+from sgkit import create_genotype_call_dataset, save_dataset
 from sgkit.io.utils import dataframe_to_dict
 from sgkit.model import DIM_SAMPLE
 from sgkit.typing import ArrayLike, NDArray
 from sgkit.utils import encode_array
 
 PathType = Union[str, Path]
 
@@ -35,14 +35,17 @@
     ("pos", "int32", "int32"),
     ("a1", str, "S"),
     ("a2", str, "S"),
 ]
 BIM_DF_DTYPE = dict([(f[0], f[1]) for f in BIM_FIELDS])
 BIM_ARRAY_DTYPE = dict([(f[0], f[2]) for f in BIM_FIELDS])
 
+INT_MISSING = -1
+STR_MISSING = "."
+
 
 class BedReader(object):
     def __init__(
         self,
         path: PathType,
         shape: Tuple[int, int],
         dtype: Any = np.int8,
@@ -77,16 +80,16 @@
         # Missing values are represented as -127 with int8 dtype,
         # see: https://fastlmm.github.io/bed-reader
         arr = self.bed.read(index=(idx[1], idx[0]), dtype=np.int8, order="F").T
         # NOTE: bed-reader can return float32 and float64, too, so this copy could be avoided
         #       (missing would then be NaN)
         arr = arr.astype(self.dtype)
         # Add a ploidy dimension, so allele counts of 0, 1, 2 correspond to 00, 10, 11
-        call0 = np.where(arr < 0, -1, np.where(arr == 0, 0, 1))
-        call1 = np.where(arr < 0, -1, np.where(arr == 2, 1, 0))
+        call0 = np.where(arr < 0, INT_MISSING, np.where(arr == 0, 0, 1))
+        call1 = np.where(arr < 0, INT_MISSING, np.where(arr == 2, 1, 0))
         arr = np.stack([call0, call1], axis=-1)
         # Apply final slice to 3D result
         return arr[:, :, idx[-1]]
 
     def close(self) -> None:
         # This is not actually crucial since a Bed instance with no
         # in-memory bim/map/fam data is essentially just a file pointer
@@ -100,18 +103,20 @@
     names = [f[0] for f in FAM_FIELDS]
     df = dd.read_csv(str(path), sep=sep, names=names, dtype=FAM_DF_DTYPE)
 
     def coerce_code(v: dd.Series, codes: List[int]) -> dd.Series:
         # Set non-ints and unexpected codes to missing (-1)
         v = dd.to_numeric(v, errors="coerce")
         v = v.where(v.isin(codes), np.nan)
-        return v.fillna(-1).astype("int8")
+        return v.fillna(INT_MISSING).astype("int8")
 
-    df["paternal_id"] = df["paternal_id"].where(df["paternal_id"] != "0", None)
-    df["maternal_id"] = df["maternal_id"].where(df["maternal_id"] != "0", None)
+    # replace fam "0" with sgkit missing values (".")
+    df["family_id"] = df["family_id"].where(df["family_id"] != "0", STR_MISSING)
+    df["paternal_id"] = df["paternal_id"].where(df["paternal_id"] != "0", STR_MISSING)
+    df["maternal_id"] = df["maternal_id"].where(df["maternal_id"] != "0", STR_MISSING)
     df["sex"] = coerce_code(df["sex"], [1, 2])
     df["phenotype"] = coerce_code(df["phenotype"], [1, 2])
 
     return df
 
 
 def read_bim(path: PathType, sep: str = "\t") -> DataFrame:
@@ -204,24 +209,26 @@
     - :data:`sgkit.variables.variant_allele_spec` (variants)
     - :data:`sgkit.variables.sample_id_spec` (samples)
     - :data:`sgkit.variables.call_genotype_spec` (variants, samples, ploidy)
     - :data:`sgkit.variables.call_genotype_mask_spec` (variants, samples, ploidy)
 
     The following pedigree-specific fields are also included:
 
-    - ``sample_family_id``: Family identifier commonly referred to as FID
-    - ``sample_id``: Within-family identifier for sample
-    - ``sample_paternal_id``: Within-family identifier for father of sample
-    - ``sample_maternal_id``: Within-family identifier for mother of sample
+    - ``sample_family_id``: Family identifier commonly referred to as FID,
+        "." for missing
+    - ``sample_member_id`` and ``sample_id``: Within-family identifier for sample
+    - ``sample_paternal_id``: Within-family identifier for father of sample,
+        "." for missing
+    - ``sample_maternal_id``: Within-family identifier for mother of sample,
+        "." for missing
     - ``sample_sex``: Sex code equal to 1 for male, 2 for female, and -1
         for missing
     - ``sample_phenotype``: Phenotype code equal to 1 for control, 2 for case,
         and -1 for missing
 
-
     See https://www.cog-genomics.org/plink/1.9/formats#fam for more details.
 
     Raises
     ------
     ValueError
         If `path` and one of `bed_path`, `bim_path` or `fam_path` are provided.
     """
@@ -291,10 +298,93 @@
         variant_allele=variant_allele,
         sample_id=sample_id,
         call_genotype=call_genotype,
         variant_id=variant_id,
     )
 
     # Assign PLINK-specific pedigree fields
-    return ds.assign(
-        {f"sample_{f}": (DIM_SAMPLE, arr_fam[f]) for f in arr_fam if f != "member_id"}
+    return ds.assign({f"sample_{f}": (DIM_SAMPLE, arr_fam[f]) for f in arr_fam})
+
+
+def plink_to_zarr(
+    *,
+    path: Optional[PathType] = None,
+    bed_path: Optional[PathType] = None,
+    bim_path: Optional[PathType] = None,
+    fam_path: Optional[PathType] = None,
+    output: Union[PathType, MutableMapping[str, bytes]],
+    chunks: Union[str, int, tuple] = "auto",
+    fam_sep: str = " ",
+    bim_sep: str = "\t",
+    bim_int_contig: bool = False,
+    lock: bool = False,
+    persist: bool = True,
+    storage_options: Optional[Dict[str, str]] = None,
+) -> None:
+    """Convert a PLINK file to a Zarr on-disk store.
+
+    A convenience for :func:`read_plink` followed by :func:`sgkit.save_dataset`.
+
+    Refer to :func:`read_plink` for details and limitations.
+
+    Parameters
+    ----------
+    path
+        Path to PLINK file set.
+        This should not include a suffix, i.e. if the files are
+        at `data.{bed,fam,bim}` then only 'data' should be
+        provided (suffixes are added internally).
+        Either this path must be provided or all 3 of
+        `bed_path`, `bim_path` and `fam_path`.
+    bed_path
+        Path to PLINK bed file.
+        This should be a full path including the `.bed` extension
+        and cannot be specified in conjunction with `path`.
+    bim_path
+        Path to PLINK bim file.
+        This should be a full path including the `.bim` extension
+        and cannot be specified in conjunction with `path`.
+    fam_path
+        Path to PLINK fam file.
+        This should be a full path including the `.fam` extension
+        and cannot be specified in conjunction with `path`.
+    output
+        Zarr store or path to directory in file system.
+    chunks
+        Chunk size for genotype (i.e. `.bed`) data, by default "auto"
+    fam_sep
+        Delimiter for `.fam` file, by default " "
+    bim_sep
+        Delimiter for `.bim` file, by default "\t"
+    bim_int_contig
+        Whether or not the contig/chromosome name in the `.bim`
+        file should be interpreted as an integer, by default False.
+        If False, then the `variant/contig` field in the resulting
+        dataset will contain the indexes of corresponding strings
+        encountered in the first `.bim` field.
+    lock
+        Whether or not to synchronize concurrent reads of `.bed`
+        file blocks, by default False. This is passed through to
+        [dask.array.from_array](https://docs.dask.org/en/latest/array-api.html#dask.array.from_array).
+    persist
+        Whether or not to persist `.fam` and `.bim` information in
+        memory, by default True. This is an important performance
+        consideration as the plain text files for this data will
+        be read multiple times when False. This can lead to load
+        times that are upwards of 10x slower.
+    storage_options
+        Any additional parameters for the storage backend (see ``fsspec.open``).
+    """
+
+    ds = read_plink(
+        path=path,
+        bed_path=bed_path,
+        bim_path=bim_path,
+        fam_path=fam_path,
+        chunks=chunks,
+        fam_sep=fam_sep,
+        bim_sep=bim_sep,
+        bim_int_contig=bim_int_contig,
+        lock=lock,
+        persist=persist,
     )
+    save_dataset(ds, output, storage_options=storage_options)
```

### Comparing `sgkit-0.6.0/sgkit/io/utils.py` & `sgkit-0.7.0/sgkit/io/utils.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/vcf/csi.py` & `sgkit-0.7.0/sgkit/io/vcf/csi.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/vcf/tbi.py` & `sgkit-0.7.0/sgkit/io/vcf/tbi.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/vcf/utils.py` & `sgkit-0.7.0/sgkit/io/vcf/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
 @contextmanager
 def temporary_directory(
     suffix: Optional[str] = None,
     prefix: Optional[str] = None,
     dir: Optional[PathType] = None,
     storage_options: Optional[Dict[str, str]] = None,
+    retain_temp_files: Optional[bool] = None,
 ) -> Iterator[str]:
     """Create a temporary directory in a fsspec filesystem.
 
     Parameters
     ----------
     suffix : Optional[str], optional
         If not None, the name of the temporary directory will end with that suffix.
@@ -140,15 +141,17 @@
         If not None, the name of the temporary directory will start with that prefix.
     dir : Optional[PathType], optional
         If not None, the temporary directory will be created in that directory, otherwise
         the local filesystem directory returned by `tempfile.gettempdir()` will be used.
         The directory may be specified as any fsspec URL.
     storage_options : Optional[Dict[str, str]], optional
         Any additional parameters for the storage backend (see `fsspec.open`).
-
+    retain_temp_files : Optional[bool], optional
+        If True, the temporary directory will not be removed on exiting the context manager.
+        Defaults to None, which means the directory will be removed.
     Yields
     -------
     Generator[str, None, None]
         A context manager yielding the fsspec URL to the created directory.
     """
 
     # Fill in defaults
@@ -164,15 +167,16 @@
     # Construct a random directory name
     tempdir = build_url(dir, prefix + str(uuid.uuid4()) + suffix)
     try:
         fs.mkdir(tempdir)
         yield tempdir
     finally:
         # Remove the temporary directory on exiting the context manager
-        fs.rm(tempdir, recursive=True)
+        if not retain_temp_files:
+            fs.rm(tempdir, recursive=True)
 
 
 def get_default_vcf_encoding(ds, chunk_length, chunk_width, compressor):
     # Enforce uniform chunks in the variants dimension
     # Also chunk in the samples direction
     def get_chunk_size(dim: Hashable, size: int) -> int:
         if dim == "variants":
```

### Comparing `sgkit-0.6.0/sgkit/io/vcf/vcf_partition.py` & `sgkit-0.7.0/sgkit/io/vcf/vcf_partition.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/vcf/vcf_reader.py` & `sgkit-0.7.0/sgkit/io/vcf/vcf_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 import functools
 import itertools
 import re
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Dict, Iterator, MutableMapping, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    MutableMapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import dask
 import fsspec
 import numpy as np
 import xarray as xr
 import zarr
 from cyvcf2 import VCF, Variant
 
 from sgkit import variables
+from sgkit.io.dataset import load_dataset
 from sgkit.io.utils import (
     CHAR_FILL,
     CHAR_MISSING,
     FLOAT32_FILL,
     FLOAT32_MISSING,
     INT_FILL,
     INT_MISSING,
@@ -35,14 +46,15 @@
     url_filename,
 )
 from sgkit.io.vcfzarr_reader import (
     concat_zarrs_optimized,
     vcf_number_to_dimension_and_size,
 )
 from sgkit.model import (
+    DIM_CONTIG,
     DIM_FILTER,
     DIM_PLOIDY,
     DIM_SAMPLE,
     DIM_VARIANT,
     create_genotype_call_dataset,
 )
 from sgkit.typing import ArrayLike, DType, PathType
@@ -412,16 +424,18 @@
     ploidy: int = 2,
     mixed_ploidy: bool = False,
     truncate_calls: bool = False,
     max_alt_alleles: int = DEFAULT_MAX_ALT_ALLELES,
     fields: Optional[Sequence[str]] = None,
     exclude_fields: Optional[Sequence[str]] = None,
     field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
+    read_chunk_length: Optional[int] = None,
 ) -> None:
-
+    if read_chunk_length is None:
+        read_chunk_length = chunk_length
     with open_vcf(input) as vcf:
         sample_id = np.array(vcf.samples, dtype="O")
         n_allele = max_alt_alleles + 1
 
         variant_contig_names = vcf.seqnames
 
         filters = [
@@ -433,52 +447,55 @@
         if "PASS" in filters:
             filters.remove("PASS")
             filters.insert(0, "PASS")
 
         # Remember max lengths of variable-length strings
         max_alt_alleles_seen = 0
 
-        # Iterate through variants in batches of chunk_length
+        # Iterate through variants in batches of read_chunk_length
 
         if region is None:
             variants = vcf
         else:
             variants = vcf(region)
 
         variant_contig_dtype = smallest_numpy_int_dtype(len(variant_contig_names))
-        variant_contig = np.empty(chunk_length, dtype=variant_contig_dtype)
-        variant_position = np.empty(chunk_length, dtype="i4")
+        variant_contig = np.empty(read_chunk_length, dtype=variant_contig_dtype)
+        variant_position = np.empty(read_chunk_length, dtype="i4")
 
         fields = fields or ["FORMAT/GT"]  # default to GT as the only extra field
         fields = _normalize_fields(vcf, fields)
         exclude_fields = exclude_fields or []
         exclude_fields = _normalize_fields(vcf, exclude_fields)
         fields = [f for f in fields if f not in exclude_fields]
         field_defs = field_defs or {}
         field_handlers = [
             VcfFieldHandler.for_field(
                 vcf,
                 field,
-                chunk_length,
+                read_chunk_length,
                 ploidy,
                 mixed_ploidy,
                 truncate_calls,
                 max_alt_alleles,
                 field_defs.get(field, {}),
             )
             for field in fields
         ]
 
         first_variants_chunk = True
-        for variants_chunk in chunks(region_filter(variants, region), chunk_length):
-
+        for variants_chunk in chunks(
+            region_filter(variants, region), read_chunk_length
+        ):
             variant_ids = []
             variant_alleles = []
-            variant_quality = np.empty(chunk_length, dtype="f4")
-            variant_filter = np.full((chunk_length, len(filters)), False, dtype="bool")
+            variant_quality = np.empty(read_chunk_length, dtype="f4")
+            variant_filter = np.full(
+                (read_chunk_length, len(filters)), False, dtype="bool"
+            )
 
             i = -1  # initialize in case of empty variants_chunk
             for i, variant in enumerate(variants_chunk):
                 variant_id = variant.ID if variant.ID is not None else "."
                 variant_ids.append(variant_id)
                 try:
                     variant_contig[i] = variant_contig_names.index(variant.CHROM)
@@ -503,16 +520,16 @@
                     for f in variant.FILTERS:
                         variant_filter[i][filters.index(f)] = True
                 except ValueError:
                     raise ValueError(f"Filter '{f}' is not defined in the header.")
                 for field_handler in field_handlers:
                     field_handler.add_variant(i, variant)
 
-            # Truncate np arrays (if last chunk is smaller than chunk_length)
-            if i + 1 < chunk_length:
+            # Truncate np arrays (if last chunk is smaller than read_chunk_length)
+            if i + 1 < read_chunk_length:
                 variant_contig = variant_contig[: i + 1]
                 variant_position = variant_position[: i + 1]
                 variant_quality = variant_quality[: i + 1]
                 variant_filter = variant_filter[: i + 1]
 
                 for field_handler in field_handlers:
                     field_handler.truncate_array(i + 1)
@@ -535,18 +552,20 @@
             ds["variant_id_mask"] = (
                 [DIM_VARIANT],
                 variant_id_mask,
             )
             ds["variant_quality"] = ([DIM_VARIANT], variant_quality)
             ds["variant_filter"] = ([DIM_VARIANT, DIM_FILTER], variant_filter)
             ds.attrs["filters"] = filters
-            ds.attrs["vcf_zarr_version"] = "0.1"
+            ds["filter_id"] = ([DIM_FILTER], np.array(filters, dtype="O"))
+            ds.attrs["vcf_zarr_version"] = "0.2"
             ds.attrs["vcf_header"] = vcf.raw_header
             try:
                 ds.attrs["contig_lengths"] = vcf.seqlens
+                ds["contig_length"] = ([DIM_CONTIG], np.array(vcf.seqlens))
             except AttributeError:
                 pass
 
             for field_handler in field_handlers:
                 field_handler.update_dataset(ds)
             ds.attrs["max_alt_alleles_seen"] = max_alt_alleles_seen
 
@@ -604,24 +623,28 @@
     ploidy: int = 2,
     mixed_ploidy: bool = False,
     truncate_calls: bool = False,
     max_alt_alleles: int = DEFAULT_MAX_ALT_ALLELES,
     fields: Optional[Sequence[str]] = None,
     exclude_fields: Optional[Sequence[str]] = None,
     field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
+    read_chunk_length: Optional[int] = None,
+    retain_temp_files: Optional[bool] = None,
 ) -> None:
     """Convert specified regions of one or more VCF files to zarr files, then concat, rechunk, write to zarr"""
 
     if temp_chunk_length is None:
         temp_chunk_length = chunk_length
 
     with temporary_directory(
-        prefix="vcf_to_zarr_", dir=tempdir, storage_options=tempdir_storage_options
+        prefix="vcf_to_zarr_",
+        dir=tempdir,
+        storage_options=tempdir_storage_options,
+        retain_temp_files=retain_temp_files,
     ) as tmpdir:
-
         paths = vcf_to_zarrs(
             input,
             tmpdir,
             regions,
             temp_chunk_length,
             chunk_width,
             compressor,
@@ -630,20 +653,22 @@
             ploidy=ploidy,
             mixed_ploidy=mixed_ploidy,
             truncate_calls=truncate_calls,
             max_alt_alleles=max_alt_alleles,
             fields=fields,
             exclude_fields=exclude_fields,
             field_defs=field_defs,
+            read_chunk_length=read_chunk_length,
         )
 
         concat_zarrs(
             paths,
             output,
             storage_options=tempdir_storage_options,
+            chunk_length=chunk_length,
         )
 
 
 def vcf_to_zarrs(
     input: Union[PathType, Sequence[PathType]],
     output: PathType,
     regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]],
@@ -655,14 +680,15 @@
     ploidy: int = 2,
     mixed_ploidy: bool = False,
     truncate_calls: bool = False,
     max_alt_alleles: int = DEFAULT_MAX_ALT_ALLELES,
     fields: Optional[Sequence[str]] = None,
     exclude_fields: Optional[Sequence[str]] = None,
     field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
+    read_chunk_length: Optional[int] = None,
 ) -> Sequence[str]:
     """Convert VCF files to multiple Zarr on-disk stores, one per region.
 
     Parameters
     ----------
     input
         A path (or paths) to the input BCF or VCF file (or files). VCF files should
@@ -717,59 +743,50 @@
         integer larger than 1. For example,
         ``{"INFO/AC": {"Number": "A"}, "FORMAT/HQ": {"dimension": "haplotypes"}}``
         overrides the ``INFO/AC`` field to be Number ``A`` (useful if the VCF defines it as
         having variable length with ``.``), and names the final dimension of the ``HQ`` array
         (which is defined as Number 2 in the VCF header) as ``haplotypes``.
         (Note that Number ``A`` is the number of alternate alleles, see section 1.4.2 of the
         VCF spec https://samtools.github.io/hts-specs/VCFv4.3.pdf.)
+    read_chunk_length
+        Length (number of variants) of chunks to read from the VCF file at a time. Use this
+        option to reduce memory usage by using a value lower than ``chunk_length`` with a small
+        cost in extra run time. The increase in runtime becomes higher as the ratio of
+        ``read_chunk_length`` to ``chunk_length`` decreases. Defaults to ``None``, which
+        means that a value equal to ``chunk_length`` is used. The memory usage of the
+        conversion process is proportional to ``read_chunk_length*n_samples*(1+n_ploidy)``
+        so this option is mainly useful for very large numbers of samples and/or where a
+        large ``chunk_size`` is desirable to reduce the number of dask tasks needed in
+        downstream analysis.
 
     Returns
     -------
     A list of URLs to the Zarr outputs.
     """
 
     output_storage_options = output_storage_options or {}
 
-    if isinstance(input, str) or isinstance(input, Path):
-        # Single input
-        inputs: Sequence[PathType] = [input]
-        assert regions is not None  # this would just be sequential case
-        input_regions: Sequence[Optional[Sequence[str]]] = [regions]  # type: ignore
-    else:
-        # Multiple inputs
-        inputs = input
-        if regions is None:
-            input_regions = [None] * len(inputs)
-        else:
-            if len(regions) == 0 or isinstance(regions[0], str):
-                raise ValueError(
-                    f"For multiple inputs, multiple input regions must be a sequence of sequence of strings: {regions}"
-                )
-            input_regions = regions
-
-    assert len(inputs) == len(input_regions)
-
     tasks = []
     parts = []
-    for i, input in enumerate(inputs):
+    for input, input_region_list in zip_input_and_regions(input, regions):
         filename = url_filename(str(input))
-        input_region_list = input_regions[i]
         if input_region_list is None:
             # single partition case: make a list so the loop below works
             input_region_list = [None]  # type: ignore
         for r, region in enumerate(input_region_list):
             part_url = build_url(str(output), f"{filename}/part-{r}.zarr")
             output_part = fsspec.get_mapper(part_url, **output_storage_options)
             parts.append(part_url)
             task = dask.delayed(vcf_to_zarr_sequential)(
                 input,
                 output=output_part,
                 region=region,
                 chunk_length=chunk_length,
                 chunk_width=chunk_width,
+                read_chunk_length=read_chunk_length,
                 compressor=compressor,
                 encoding=encoding,
                 ploidy=ploidy,
                 mixed_ploidy=mixed_ploidy,
                 truncate_calls=truncate_calls,
                 max_alt_alleles=max_alt_alleles,
                 fields=fields,
@@ -782,43 +799,49 @@
 
 
 def concat_zarrs(
     urls: Sequence[str],
     output: Union[PathType, MutableMapping[str, bytes]],
     *,
     storage_options: Optional[Dict[str, str]] = None,
+    chunk_length: Optional[int] = None,
 ) -> None:
     """Concatenate multiple Zarr stores into a single Zarr store.
 
     The Zarr stores are concatenated and rechunked to produce a single combined store.
 
     Parameters
     ----------
     urls
         A list of URLs to the Zarr stores to combine, typically the return value of
         :func:`vcf_to_zarrs`.
     output
         Zarr store or path to directory in file system.
     storage_options
         Any additional parameters for the storage backend (see ``fsspec.open``).
+    chunk_length
+       The length of the variant dimension chunks in the output Zarr store. If not specified,
+       the chunk length of the first input Zarr store is used.
     """
 
     vars_to_rechunk = []
     vars_to_copy = []
     storage_options = storage_options or {}
     ds = xr.open_zarr(  # type: ignore[no-untyped-call]
         fsspec.get_mapper(urls[0], **storage_options), concat_characters=False
     )
-    for (var, arr) in ds.data_vars.items():
+    for var, arr in ds.data_vars.items():
         if arr.dims[0] == "variants":
             vars_to_rechunk.append(var)
         else:
             vars_to_copy.append(var)
 
-    concat_zarrs_optimized(urls, output, vars_to_rechunk, vars_to_copy)
+    concat_zarrs_optimized(
+        urls, output, vars_to_rechunk, vars_to_copy, chunk_length=chunk_length
+    )
 
 
 def vcf_to_zarr(
     input: Union[PathType, Sequence[PathType]],
     output: Union[PathType, MutableMapping[str, bytes]],
     *,
     target_part_size: Union[None, int, str] = "auto",
@@ -833,14 +856,16 @@
     ploidy: int = 2,
     mixed_ploidy: bool = False,
     truncate_calls: bool = False,
     max_alt_alleles: int = DEFAULT_MAX_ALT_ALLELES,
     fields: Optional[Sequence[str]] = None,
     exclude_fields: Optional[Sequence[str]] = None,
     field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
+    read_chunk_length: Optional[int] = None,
+    retain_temp_files: Optional[bool] = None,
 ) -> None:
     """Convert VCF files to a single Zarr on-disk store.
 
     By default, the conversion is carried out in parallel, by writing the output for each
     part to a separate, intermediate Zarr store in ``tempdir``. Then, in a second step
     the intermediate outputs are concatenated and rechunked into the final output Zarr
     store in ``output``.
@@ -920,100 +945,294 @@
         integer larger than 1. For example,
         ``{"INFO/AC": {"Number": "A"}, "FORMAT/HQ": {"dimension": "haplotypes"}}``
         overrides the ``INFO/AC`` field to be Number ``A`` (useful if the VCF defines it as
         having variable length with ``.``), and names the final dimension of the ``HQ`` array
         (which is defined as Number 2 in the VCF header) as ``haplotypes``.
         (Note that Number ``A`` is the number of alternate alleles, see section 1.4.2 of the
         VCF spec https://samtools.github.io/hts-specs/VCFv4.3.pdf.)
+    read_chunk_length
+        Length (number of variants) of chunks to read from the VCF file at a time. Use this
+        option to reduce memory usage by using a value lower than ``chunk_length`` with a small
+        cost in extra run time. The increase in runtime becomes higher as the ratio of
+        ``read_chunk_length`` to  Defaults to ``None``, which means that a value equal
+        to ``chunk_length`` is used. The memory usage of the conversion process is
+        proportional to ``read_chunk_length*n_samples*(1+n_ploidy)`` so this option is
+        mainly useful for very large numbers of samples and/or where a large ``chunk_size``
+        is desirable to reduce the number of dask tasks needed in downstream analysis.
+    retain_temp_files
+        If True, intermediate files are retained after the final output is written. Defaults
+        to deleting intermediate files. Intermediate files are deleted in a single process,
+        so for large VCF files this can be slow.
     """
 
     if temp_chunk_length is not None:
         if chunk_length % temp_chunk_length != 0:
             raise ValueError(
                 f"Temporary chunk length in variant dimension ({temp_chunk_length}) "
                 f"must evenly divide target chunk length {chunk_length}"
             )
-    if regions is None and target_part_size is not None:
-        if target_part_size == "auto":
-            target_part_size = "20MB"
-        if isinstance(input, str) or isinstance(input, Path):
-            regions = partition_into_regions(input, target_part_size=target_part_size)
-        else:
-            # Multiple inputs
-            inputs = input
-            regions = [
-                partition_into_regions(input, target_part_size=target_part_size)
-                for input in inputs
-            ]
 
-    if (isinstance(input, str) or isinstance(input, Path)) and (
-        regions is None or isinstance(regions, str)
-    ):
-        convert_func = vcf_to_zarr_sequential
-    else:
-        convert_func = functools.partial(
-            vcf_to_zarr_parallel,
-            temp_chunk_length=temp_chunk_length,
-            tempdir=tempdir,
-            tempdir_storage_options=tempdir_storage_options,
-        )
-    convert_func(
-        input,  # type: ignore
-        output,
-        regions,  # type: ignore
+    # all arguments except input and region/regions
+    sequential_function = functools.partial(
+        vcf_to_zarr_sequential,
+        output=output,
         chunk_length=chunk_length,
         chunk_width=chunk_width,
+        read_chunk_length=read_chunk_length,
         compressor=compressor,
         encoding=encoding,
         ploidy=ploidy,
         mixed_ploidy=mixed_ploidy,
         truncate_calls=truncate_calls,
         max_alt_alleles=max_alt_alleles,
         fields=fields,
         exclude_fields=exclude_fields,
         field_defs=field_defs,
     )
+    parallel_function = functools.partial(
+        vcf_to_zarr_parallel,
+        output=output,
+        chunk_length=chunk_length,
+        chunk_width=chunk_width,
+        read_chunk_length=read_chunk_length,
+        compressor=compressor,
+        encoding=encoding,
+        ploidy=ploidy,
+        mixed_ploidy=mixed_ploidy,
+        truncate_calls=truncate_calls,
+        max_alt_alleles=max_alt_alleles,
+        fields=fields,
+        exclude_fields=exclude_fields,
+        field_defs=field_defs,
+        temp_chunk_length=temp_chunk_length,
+        tempdir=tempdir,
+        tempdir_storage_options=tempdir_storage_options,
+        retain_temp_files=retain_temp_files,
+    )
+    process_vcfs(
+        input,
+        sequential_function,
+        parallel_function,
+        regions=regions,
+        target_part_size=target_part_size,
+    )
 
     # Issue a warning if max_alt_alleles caused data to be dropped
     ds = zarr.open(output)
     max_alt_alleles_seen = ds.attrs["max_alt_alleles_seen"]
     if max_alt_alleles_seen > max_alt_alleles:
         warnings.warn(
             f"Some alternate alleles were dropped, since actual max value {max_alt_alleles_seen} exceeded max_alt_alleles setting of {max_alt_alleles}.",
             MaxAltAllelesExceededWarning,
         )
 
 
+def read_vcf(
+    input: Union[PathType, Sequence[PathType]],
+    *,
+    target_part_size: Union[None, int, str] = "auto",
+    regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]] = None,
+    chunk_length: int = 10_000,
+    chunk_width: int = 1_000,
+    compressor: Optional[Any] = DEFAULT_COMPRESSOR,
+    encoding: Optional[Any] = None,
+    temp_chunk_length: Optional[int] = None,
+    tempdir: Optional[PathType] = None,
+    tempdir_storage_options: Optional[Dict[str, str]] = None,
+    ploidy: int = 2,
+    mixed_ploidy: bool = False,
+    truncate_calls: bool = False,
+    max_alt_alleles: int = DEFAULT_MAX_ALT_ALLELES,
+    fields: Optional[Sequence[str]] = None,
+    exclude_fields: Optional[Sequence[str]] = None,
+    field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
+) -> xr.Dataset:
+    """Read VCF dataset.
+
+    A convenience for :func:`vcf_to_zarr` followed by :func:`sgkit.load_dataset`.
+    Note that the output Zarr store in ``tempdir`` is not deleted after this function
+    returns, so must be deleted manually by the user.
+
+    Refer to :func:`vcf_to_zarr` for details and limitations.
+
+    Parameters
+    ----------
+    input
+        A path (or paths) to the input BCF or VCF file (or files). VCF files should
+        be compressed and have a ``.tbi`` or ``.csi`` index file. BCF files should
+        have a ``.csi`` index file.
+    target_part_size
+        The desired size, in bytes, of each (compressed) part of the input to be
+        processed in parallel. Defaults to ``"auto"``, which will pick a good size
+        (currently 20MB). A value of None means that the input will be processed
+        sequentially. The setting will be ignored if ``regions`` is also specified.
+    regions
+        Genomic region or regions to extract variants for. For multiple inputs, multiple
+        input regions are specified as a sequence of values which may be None, or a
+        sequence of region strings. Takes priority over ``target_part_size`` if both
+        are not None.
+    chunk_length
+        Length (number of variants) of chunks in which data are stored, by default 10,000.
+    chunk_width
+        Width (number of samples) to use when storing chunks in output, by default 1,000.
+    compressor
+        Zarr compressor, by default Blosc + zstd with compression level 7 and auto-shuffle.
+        No compression is used when set as None.
+    encoding
+        Variable-specific encodings for xarray, specified as a nested dictionary with
+        variable names as keys and dictionaries of variable specific encodings as values.
+        Can be used to override Zarr compressor and filters on a per-variable basis,
+        e.g., ``{"call_genotype": {"compressor": Blosc("zstd", 9)}}``.
+    temp_chunk_length
+        Length (number of variants) of chunks for temporary intermediate files. Set this
+        to be smaller than ``chunk_length`` to avoid memory errors when loading files with
+        very large numbers of samples. Must be evenly divisible into ``chunk_length``.
+        Defaults to ``chunk_length`` if not set.
+    tempdir
+        Temporary directory where intermediate files are stored. The default None means
+        use the system default temporary directory.
+    tempdir_storage_options:
+        Any additional parameters for the storage backend for tempdir (see ``fsspec.open``).
+    ploidy
+        The (maximum) ploidy of genotypes in the VCF file.
+    mixed_ploidy
+        If True, genotype calls with fewer alleles than the specified ploidy will be padded
+        with the fill (non-allele) sentinel value of -2. If false, calls with fewer alleles than
+        the specified ploidy will be treated as incomplete and will be padded with the
+        missing-allele sentinel value of -1.
+    truncate_calls
+        If True, genotype calls with more alleles than the specified (maximum) ploidy value
+        will be truncated to size ploidy. If false, calls with more alleles than the
+        specified ploidy will raise an exception.
+    max_alt_alleles
+        The (maximum) number of alternate alleles in the VCF file. Any records with more than
+        this number of alternate alleles will have the extra alleles dropped (the `variant_allele`
+        variable will be truncated). Any call genotype fields with the extra alleles will
+        be changed to the missing-allele sentinel value of -1.
+    fields
+        Extra fields to extract data for. A list of strings, with ``INFO`` or ``FORMAT`` prefixes.
+        Wildcards are permitted too, for example: ``["INFO/*", "FORMAT/DP"]``.
+    field_defs
+        Per-field information that overrides the field definitions in the VCF header, or
+        provides extra information needed in the dataset representation. Definitions
+        are a represented as a dictionary whose keys are the field names, and values are
+        dictionaries with any of the following keys: ``Number``, ``Type``, ``Description``,
+        ``dimension``. The first three correspond to VCF header values, and ``dimension`` is
+        the name of the final dimension in the array for the case where ``Number`` is a fixed
+        integer larger than 1. For example,
+        ``{"INFO/AC": {"Number": "A"}, "FORMAT/HQ": {"dimension": "haplotypes"}}``
+        overrides the ``INFO/AC`` field to be Number ``A`` (useful if the VCF defines it as
+        having variable length with ``.``), and names the final dimension of the ``HQ`` array
+        (which is defined as Number 2 in the VCF header) as ``haplotypes``.
+        (Note that Number ``A`` is the number of alternate alleles, see section 1.4.2 of the
+        VCF spec https://samtools.github.io/hts-specs/VCFv4.3.pdf.)
+
+    """
+
+    # Need to retain zarr file backing the returned dataset
+    with temporary_directory(
+        prefix="read_vcf_",
+        suffix=".zarr",
+        dir=tempdir,
+        storage_options=tempdir_storage_options,
+        retain_temp_files=True,
+    ) as output:
+        vcf_to_zarr(
+            input,
+            output,
+            target_part_size=target_part_size,
+            regions=regions,
+            chunk_length=chunk_length,
+            chunk_width=chunk_width,
+            compressor=compressor,
+            encoding=encoding,
+            temp_chunk_length=temp_chunk_length,
+            tempdir=tempdir,
+            tempdir_storage_options=tempdir_storage_options,
+            ploidy=ploidy,
+            mixed_ploidy=mixed_ploidy,
+            truncate_calls=truncate_calls,
+            max_alt_alleles=max_alt_alleles,
+            fields=fields,
+            exclude_fields=exclude_fields,
+            field_defs=field_defs,
+        )
+        return load_dataset(output)
+
+
 def count_variants(path: PathType, region: Optional[str] = None) -> int:
     """Count the number of variants in a VCF file."""
     with open_vcf(path) as vcf:
         if region is not None:
             vcf = vcf(region)
         return sum(1 for _ in region_filter(vcf, region))
 
 
-def zarr_array_sizes(input: PathType) -> Dict[str, Any]:
-    """Make a pass through a VCF/BCF file to determine sizes for storage in Zarr."""
+def zarr_array_sizes(
+    input: Union[PathType, Sequence[PathType]],
+    *,
+    regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]] = None,
+    target_part_size: Union[None, int, str] = "auto",
+) -> Dict[str, Any]:
+    """Make a pass through a VCF/BCF file to determine sizes for storage in Zarr.
 
-    with open_vcf(input) as vcf:
+    By default, the input is processed in parts in parallel. However, if the input
+    is a single file, ``target_part_size`` is None, and ``regions`` is None,
+    then the operation will be carried out sequentially.
 
+    Parameters
+    ----------
+    input
+        A path (or paths) to the input BCF or VCF file (or files). VCF files should
+        be compressed and have a ``.tbi`` or ``.csi`` index file. BCF files should
+        have a ``.csi`` index file.
+    target_part_size
+        The desired size, in bytes, of each (compressed) part of the input to be
+        processed in parallel. Defaults to ``"auto"``, which will pick a good size
+        (currently 20MB). A value of None means that the input will be processed
+        sequentially. The setting will be ignored if ``regions`` is also specified.
+    regions
+        Genomic region or regions to extract variants for. For multiple inputs, multiple
+        input regions are specified as a sequence of values which may be None, or a
+        sequence of region strings. Takes priority over ``target_part_size`` if both
+        are not None.
+    """
+
+    return process_vcfs(
+        input,
+        zarr_array_sizes_sequential,
+        zarr_array_sizes_parallel,
+        regions=regions,
+        target_part_size=target_part_size,
+    )
+
+
+def zarr_array_sizes_sequential(
+    input: PathType, region: Optional[str] = None
+) -> Dict[str, Any]:
+    with open_vcf(input) as vcf:
         ploidy = -1
         alt_alleles = 0
 
         info = _get_vcf_field_defs(vcf, "INFO")
         info_field_defs = {
             key: {"Number": 1} for key in info.keys() if info[key]["Number"] == "."
         }
 
         format = _get_vcf_field_defs(vcf, "FORMAT")
         format_field_defs = {
             key: {"Number": 1} for key in format.keys() if format[key]["Number"] == "."
         }
 
-        for variant in vcf:
+        if region is None:
+            variants = vcf
+        else:
+            variants = vcf(region)
+
+        for variant in region_filter(variants, region):
             for key, val in info_field_defs.items():
                 field_val = variant.INFO.get(key)
                 if field_val is not None:
                     try:
                         val["Number"] = max(val["Number"], len(field_val))
                     except TypeError:
                         pass  # single value
@@ -1026,15 +1245,17 @@
                         val["Number"] = max(val["Number"], m)
                     else:
                         val["Number"] = max(val["Number"], field_val.shape[-1])
 
             try:
                 if variant.genotype is not None:
                     ploidy = max(ploidy, variant.genotype.ploidy)
-            except Exception:  # cyvcf2 raises an Exception "couldn't get genotypes for variant"
+            except (
+                Exception
+            ):  # cyvcf2 raises an Exception "couldn't get genotypes for variant"
                 pass  # no genotype information
             alt_alleles = max(alt_alleles, len(variant.ALT))
 
         field_defs = {}
         for key, val in info_field_defs.items():
             field_defs[f"INFO/{key}"] = val
         for key, val in format_field_defs.items():
@@ -1042,7 +1263,103 @@
 
         kwargs: Dict[str, Any] = {"max_alt_alleles": alt_alleles}
         if len(field_defs) > 0:
             kwargs["field_defs"] = field_defs
         if ploidy > -1:
             kwargs["ploidy"] = ploidy
         return kwargs
+
+
+def zarr_array_sizes_parallel(
+    input: Union[PathType, Sequence[PathType]],
+    regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]],
+) -> Dict[str, Any]:
+    tasks = []
+    for input, input_region_list in zip_input_and_regions(input, regions):
+        if input_region_list is None:
+            # single partition case: make a list so the loop below works
+            input_region_list = [None]  # type: ignore
+        for region in input_region_list:
+            task = dask.delayed(zarr_array_sizes_sequential)(
+                input,
+                region=region,
+            )
+            tasks.append(task)
+    all_kwargs = dask.compute(*tasks)
+    return merge_zarr_array_sizes(all_kwargs)
+
+
+def merge_zarr_array_sizes(all_kwargs: Sequence[Dict[str, Any]]):
+    """Merge a sequence of size kwargs using the largest size found in any of them."""
+
+    max_alt_alleles = max([kwargs["max_alt_alleles"] for kwargs in all_kwargs])
+    ploidy = max([kwargs.get("ploidy", -1) for kwargs in all_kwargs])
+
+    field_defs = {}
+    if len(all_kwargs) > 0 and "field_defs" in all_kwargs[0]:
+        for key in all_kwargs[0]["field_defs"].keys():
+            number = max([kwargs["field_defs"][key]["Number"] for kwargs in all_kwargs])
+            field_defs[key] = {"Number": number}
+
+    kwargs: Dict[str, Any] = {"max_alt_alleles": max_alt_alleles}
+    if len(field_defs) > 0:
+        kwargs["field_defs"] = field_defs
+    if ploidy > -1:
+        kwargs["ploidy"] = ploidy
+    return kwargs
+
+
+def process_vcfs(
+    input: Union[PathType, Sequence[PathType]],
+    sequential_function: Callable,
+    parallel_function: Callable,
+    *,
+    regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]] = None,
+    target_part_size: Union[None, int, str] = "auto",
+) -> Any:
+    """A helper function to process VCFs in region chunks, using a sequential function
+    for single file and single region input, and a parallel function otherwise."""
+    if regions is None and target_part_size is not None:
+        if target_part_size == "auto":
+            target_part_size = "20MB"
+        if isinstance(input, str) or isinstance(input, Path):
+            regions = partition_into_regions(input, target_part_size=target_part_size)
+        else:
+            # Multiple inputs
+            inputs = input
+            regions = [
+                partition_into_regions(input, target_part_size=target_part_size)
+                for input in inputs
+            ]
+
+    if (isinstance(input, str) or isinstance(input, Path)) and (
+        regions is None or isinstance(regions, str)
+    ):
+        return sequential_function(input=input, region=regions)
+    else:
+        return parallel_function(input=input, regions=regions)
+
+
+def zip_input_and_regions(
+    input: Union[PathType, Sequence[PathType]],
+    regions: Union[None, Sequence[str], Sequence[Optional[Sequence[str]]]],
+) -> Any:
+    if isinstance(input, str) or isinstance(input, Path):
+        # Single input
+        inputs: Sequence[PathType] = [input]
+        assert regions is not None  # this would just be sequential case
+        input_regions: Sequence[Optional[Sequence[str]]] = [regions]  # type: ignore
+    else:
+        # Multiple inputs
+        inputs = input
+        if regions is None:
+            input_regions = [None] * len(inputs)
+        else:
+            if len(regions) == 0 or isinstance(regions[0], str):
+                raise ValueError(
+                    f"For multiple inputs, multiple input regions must be a sequence of sequence of strings: {regions}"
+                )
+            input_regions = regions
+
+    assert len(inputs) == len(input_regions)
+
+    return zip(inputs, input_regions)
```

### Comparing `sgkit-0.6.0/sgkit/io/vcf/vcf_writer_utils.py` & `sgkit-0.7.0/sgkit/io/vcf/vcf_writer_utils.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/io/vcfzarr_reader.py` & `sgkit-0.7.0/sgkit/io/vcfzarr_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             prefix="vcfzarr_to_zarr_", suffix=".zarr", dir=tempdir
         ) as tmpdir:
             zarr_files = []
             for i, contig in enumerate(contigs):
                 # convert contig group to zarr and save in tmpdir
                 ds = _vcfzarr_to_dataset(vcfzarr[contig], contig, variant_contig_names)
                 if i == 0:
-                    for (var, arr) in ds.data_vars.items():
+                    for var, arr in ds.data_vars.items():
                         if arr.dims[0] == "variants":
                             vars_to_rechunk.append(var)
                         else:
                             vars_to_copy.append(var)
 
                 contig_zarr_file = Path(tmpdir) / contig
                 ds.to_zarr(contig_zarr_file)
@@ -172,15 +172,14 @@
 def _vcfzarr_to_dataset(
     vcfzarr: zarr.Array,
     contig: Optional[str] = None,
     variant_contig_names: Optional[List[str]] = None,
     fix_strings: bool = True,
     field_defs: Optional[Dict[str, Dict[str, Any]]] = None,
 ) -> xr.Dataset:
-
     variant_position = da.from_zarr(vcfzarr["variants/POS"])
 
     if contig is None:
         # Get the contigs from variants/CHROM
         variants_chrom = da.from_zarr(vcfzarr["variants/CHROM"]).astype(str)
         variant_contig, variant_contig_names = encode_array(variants_chrom.compute())
         variant_contig_dtype = smallest_numpy_int_dtype(len(variant_contig_names))
@@ -254,15 +253,15 @@
         field_def = field_defs.get(field, {})
         _add_field_to_dataset(
             category, key, vcfzarr_key, variable_name, dims, field_def, vcfzarr, ds
         )
 
     # Fix string types to include length
     if fix_strings:
-        for (var, arr) in ds.data_vars.items():
+        for var, arr in ds.data_vars.items():
             kind = arr.dtype.kind
             if kind in ["O", "U", "S"]:
                 # Compute fixed-length string dtype for array
                 if kind == "O" or var in ("variant_id", "variant_allele"):
                     kind = "S"
                 max_len = max_str_len(arr).values  # type: ignore
                 dt = f"{kind}{max_len}"
@@ -321,14 +320,15 @@
 
 def concat_zarrs_optimized(
     zarr_files: Sequence[str],
     output: Union[PathType, MutableMapping[str, bytes]],
     vars_to_rechunk: List[Hashable],
     vars_to_copy: List[Hashable],
     fix_strings: bool = False,
+    chunk_length: Optional[int] = None,
 ) -> None:
     if isinstance(output, Path):
         output = str(output)
 
     zarr_groups = [zarr.open_group(f) for f in zarr_files]
 
     first_zarr_group = zarr_groups[0]
@@ -336,22 +336,26 @@
     # create the top-level group
     zarr.open_group(output, mode="w")
 
     # copy variables that are to be rechunked
     # NOTE: that this uses _to_zarr function defined here that is needed to avoid
     # race conditions between writing the array contents and its metadata
     # see https://github.com/pystatgen/sgkit/pull/486
-    delayed = []  # do all the rechunking operations in one computation
     for var in vars_to_rechunk:
         dtype = None
         if fix_strings and var in {"variant_id", "variant_allele"}:
             max_len = _get_max_len(zarr_groups, f"max_length_{var}")
             dtype = f"S{max_len}"
+        assert first_zarr_group[var].attrs["_ARRAY_DIMENSIONS"][0] == "variants"
+        target_chunks = None
+        if chunk_length is not None:
+            target_chunks = list(first_zarr_group[var].chunks)
+            target_chunks[0] = chunk_length
         arr = concatenate_and_rechunk(
-            [group[var] for group in zarr_groups], dtype=dtype
+            [group[var] for group in zarr_groups], dtype=dtype, chunks=target_chunks
         )
 
         _to_zarr_kwargs = dict(
             compressor=first_zarr_group[var].compressor,
             filters=first_zarr_group[var].filters,
             fill_value=None,
         )
@@ -370,16 +374,15 @@
             output,
             component=var,
             overwrite=True,
             compute=False,
             attrs=first_zarr_group[var].attrs.asdict(),
             **_to_zarr_kwargs,
         )
-        d = _fuse_delayed(d)  # type: ignore[no-untyped-call]
-        delayed.append(d)
+        da.compute(_fuse_delayed(d))  # type: ignore[no-untyped-call]
 
     # copy variables that are not rechunked (e.g. sample_id)
     for var in vars_to_copy:
         arr = da.from_zarr(zarr_files[0], component=var)
         _to_zarr_kwargs = dict(
             compressor=first_zarr_group[var].compressor,
             filters=first_zarr_group[var].filters,
@@ -400,22 +403,18 @@
             output,
             component=var,
             overwrite=True,
             compute=False,
             attrs=first_zarr_group[var].attrs.asdict(),
             **_to_zarr_kwargs,
         )
-        d = _fuse_delayed(d)  # type: ignore[no-untyped-call]
-        delayed.append(d)
-
-    da.compute(*delayed)
+        da.compute(_fuse_delayed(d))  # type: ignore[no-untyped-call]
 
     # copy unchanged variables and top-level metadata
     with zarr.open_group(output) as output_zarr:
-
         # copy top-level attributes
         group_attrs = dict(first_zarr_group.attrs)
         if "max_alt_alleles_seen" in group_attrs:
             max_alt_alleles_seen = _get_max_len(zarr_groups, "max_alt_alleles_seen")
             group_attrs["max_alt_alleles_seen"] = max_alt_alleles_seen
         output_zarr.attrs.update(group_attrs)
 
@@ -460,14 +459,17 @@
     storage_options = storage_options or {}
     if isinstance(url, str):
         mapper = get_mapper(url, **storage_options)
     else:
         # assume the object passed is already a mapper
         mapper = url  # pragma: no cover
     chunks = [c[0] for c in arr.chunks]
+    # Zarr errors if we specify chunks of length 0 (#1068)
+    if sum(chunks) == 0:
+        chunks = None
     z = _zarr_create_with_attrs(  # type: ignore[no-untyped-call]
         shape=arr.shape,
         chunks=chunks,
         dtype=arr.dtype,
         store=mapper,
         path=component,
         overwrite=overwrite,
@@ -521,9 +523,9 @@
             dim_name = f"{category}_{key}_dim"
             warnings.warn(
                 f"A new dimension named {dim_name} was created. To change this name re-run specifying `field_defs`.",
                 DimensionNameForFixedFormatFieldWarning,
             )
             return (dim_name, int(vcf_number))
     raise ValueError(
-        f"{category} field '{key}' is defined as Number '{vcf_number}', which is not supported."
+        f"{category} field '{key}' is defined as Number '{vcf_number}', which is not supported. Consider specifying `field_defs` to provide a concrete size for this field."
     )
```

### Comparing `sgkit-0.6.0/sgkit/model.py` & `sgkit-0.7.0/sgkit/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import warnings
 from typing import Any, Dict, Hashable, List, Optional
 
 import numpy as np
 import xarray as xr
 
 import sgkit as sg
 
 from .typing import ArrayLike
 from .utils import create_dataset
 
+DIM_CONTIG = "contigs"
 DIM_VARIANT = "variants"
 DIM_SAMPLE = "samples"
 DIM_PLOIDY = "ploidy"
 DIM_ALLELE = "alleles"
 DIM_GENOTYPE = "genotypes"
 DIM_FILTER = "filters"
 
@@ -57,14 +59,15 @@
         The unique identifier of the variant.
 
     Returns
     -------
     The dataset of genotype calls.
     """
     data_vars: Dict[Hashable, Any] = {
+        "contig_id": ([DIM_CONTIG], np.array(variant_contig_names, dtype=str)),
         "variant_contig": ([DIM_VARIANT], variant_contig),
         "variant_position": ([DIM_VARIANT], variant_position),
         "variant_allele": ([DIM_VARIANT, DIM_ALLELE], variant_allele),
         "sample_id": ([DIM_SAMPLE], sample_id),
     }
     if call_genotype is not None:
         data_vars["call_genotype"] = (
@@ -135,14 +138,15 @@
 
     Returns
     -------
     The dataset of genotype calls.
 
     """
     data_vars: Dict[Hashable, Any] = {
+        "contig_id": ([DIM_CONTIG], np.array(variant_contig_names, dtype=str)),
         "variant_contig": ([DIM_VARIANT], variant_contig),
         "variant_position": ([DIM_VARIANT], variant_position),
         "variant_allele": ([DIM_VARIANT, DIM_ALLELE], variant_allele),
         "sample_id": ([DIM_SAMPLE], sample_id),
         "call_dosage": ([DIM_VARIANT, DIM_SAMPLE], call_dosage),
         "call_dosage_mask": ([DIM_VARIANT, DIM_SAMPLE], np.isnan(call_dosage)),
         "call_genotype_probability": (
@@ -152,9 +156,46 @@
         "call_genotype_probability_mask": (
             [DIM_VARIANT, DIM_SAMPLE, DIM_GENOTYPE],
             np.isnan(call_genotype_probability),
         ),
     }
     if variant_id is not None:
         data_vars["variant_id"] = ([DIM_VARIANT], variant_id)
-    attrs: Dict[Hashable, Any] = {"contigs": variant_contig_names}
+    attrs: Dict[Hashable, Any] = {
+        "contigs": variant_contig_names,
+        "source": f"sgkit-{sg.__version__}",
+    }
     return create_dataset(data_vars=data_vars, attrs=attrs)
+
+
+def num_contigs(ds: xr.Dataset) -> ArrayLike:
+    """Return the number of contigs in a dataset."""
+    if DIM_CONTIG in ds.dims:
+        return ds.dims[DIM_CONTIG]
+    else:
+        return len(ds.attrs["contigs"])
+
+
+def get_contigs(ds: xr.Dataset) -> ArrayLike:
+    """Return the contigs in a dataset."""
+    if "contig_id" in ds:
+        return ds["contig_id"].values
+    else:
+        warnings.warn(
+            "The 'contigs' VCF Zarr group attribute is deprecated and should be converted to a 'contig_id' array.",
+            DeprecationWarning,
+        )
+        return np.array(ds.attrs["contigs"], dtype="S")
+
+
+def get_filters(ds: xr.Dataset) -> Optional[ArrayLike]:
+    """Return the filters in a dataset."""
+    if "filter_id" in ds:
+        return ds["filter_id"].values
+    elif "filters" in ds.attrs:
+        warnings.warn(
+            "The 'filters' VCF Zarr group attribute is deprecated and should be converted to a 'filter_id' array.",
+            DeprecationWarning,
+        )
+        return np.array(ds.attrs["filters"], dtype="S")
+    else:
+        return None
```

### Comparing `sgkit-0.6.0/sgkit/stats/aggregation.py` & `sgkit-0.7.0/sgkit/stats/aggregation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,27 @@
-import math
 from typing import Any, Dict, Hashable
 
 import dask.array as da
 import numpy as np
 import xarray as xr
 from typing_extensions import Literal
 from xarray import Dataset
 
 from sgkit import variables
-from sgkit.accelerate import numba_guvectorize, numba_jit
-from sgkit.stats.utils import cohort_sum
-from sgkit.typing import ArrayLike
+from sgkit.display import genotype_as_bytes
 from sgkit.utils import (
     conditional_merge_datasets,
     create_dataset,
     define_variable_if_absent,
     smallest_numpy_int_dtype,
 )
 
 Dimension = Literal["samples", "variants"]
 
 
-@numba_guvectorize(  # type: ignore
-    [
-        "void(int8[:], uint8[:], uint8[:])",
-        "void(int16[:], uint8[:], uint8[:])",
-        "void(int32[:], uint8[:], uint8[:])",
-        "void(int64[:], uint8[:], uint8[:])",
-    ],
-    "(k),(n)->(n)",
-)
-def count_alleles(
-    g: ArrayLike, _: ArrayLike, out: ArrayLike
-) -> None:  # pragma: no cover
-    """Generalized U-function for computing per sample allele counts.
-
-    Parameters
-    ----------
-    g
-        Genotype call of shape (ploidy,) containing alleles encoded as
-        type `int` with values < 0 indicating a missing allele.
-    _
-        Dummy variable of type `uint8` and shape (alleles,) used to
-        define the number of unique alleles to be counted in the
-        return value.
-
-    Returns
-    -------
-    ac : ndarray
-        Allele counts with shape (alleles,) and values corresponding to
-        the number of non-missing occurrences of each allele.
-
-    """
-    out[:] = 0
-    n_allele = len(g)
-    for i in range(n_allele):
-        a = g[i]
-        if a >= 0:
-            out[a] += 1
-
-
 def count_call_alleles(
     ds: Dataset,
     *,
     call_genotype: Hashable = variables.call_genotype,
     merge: bool = True,
 ) -> Dataset:
     """Compute per sample allele counts from genotype calls.
@@ -110,14 +68,16 @@
     <BLANKLINE>
            [[1, 1],
             [1, 1]],
     <BLANKLINE>
            [[2, 0],
             [2, 0]]], dtype=uint8)
     """
+    from .aggregation_numba_fns import count_alleles
+
     variables.validate(ds, {call_genotype: variables.call_genotype_spec})
     n_alleles = ds.dims["alleles"]
     G = da.asarray(ds[call_genotype])
     shape = (G.chunks[0], G.chunks[1], n_alleles)
     # use numpy array to avoid dask task dependencies between chunks
     N = np.empty(n_alleles, dtype=np.uint8)
     new_ds = create_dataset(
@@ -256,14 +216,16 @@
     <BLANKLINE>
             [[1, 3],
             [1, 3]],
     <BLANKLINE>
             [[3, 1],
             [1, 3]]], dtype=uint64)
     """
+    from .cohort_numba_fns import cohort_sum
+
     ds = define_variable_if_absent(
         ds, variables.call_allele_count, call_allele_count, count_call_alleles
     )
     variables.validate(ds, {call_allele_count: variables.call_allele_count_spec})
     # ensure cohorts is a numpy array to minimize dask task
     # dependencies between chunks in other dimensions
     AC, SC = da.asarray(ds[call_allele_count]), ds[sample_cohort].values
@@ -283,112 +245,14 @@
     odim = _swap(dim)[:-1]
     n_called = (~ds[call_genotype_mask].any(dim="ploidy")).sum(dim=dim)
     return create_dataset(
         {f"{odim}_n_called": n_called, f"{odim}_call_rate": n_called / ds.dims[dim]}
     )
 
 
-@numba_jit(nogil=True)
-def _biallelic_genotype_index(genotype: ArrayLike) -> int:
-    index = 0
-    for i in range(len(genotype)):
-        a = genotype[i]
-        if a < 0:
-            if a < -1:
-                raise ValueError("Mixed-ploidy genotype indicated by allele < -1")
-            return -1
-        if a > 1:
-            raise ValueError("Allele value > 1")
-        index += a
-    return index
-
-
-@numba_guvectorize(  # type: ignore
-    [
-        "void(int8[:,:], uint64[:], uint64[:])",
-        "void(int16[:,:], uint64[:], uint64[:])",
-        "void(int32[:,:], uint64[:], uint64[:])",
-        "void(int64[:,:], uint64[:], uint64[:])",
-    ],
-    "(n, k),(g)->(g)",
-)
-def _count_biallelic_genotypes(
-    genotypes: ArrayLike, _: ArrayLike, out: ArrayLike
-) -> ArrayLike:  # pragma: no cover
-    out[:] = 0
-    for i in range(len(genotypes)):
-        index = _biallelic_genotype_index(genotypes[i])
-        if index >= 0:
-            out[index] += 1
-
-
-# implementation from github.com/PlantandFoodResearch/MCHap
-# TODO: replace with math.comb when supported by numba
-@numba_jit(nogil=True)
-def _comb(n: int, k: int) -> int:
-    if k > n:
-        return 0
-    r = 1
-    for d in range(1, k + 1):
-        gcd_ = math.gcd(r, d)
-        r //= gcd_
-        r *= n
-        r //= d // gcd_
-        n -= 1
-    return r
-
-
-_COMB_REP_LOOKUP = np.array(
-    [[math.comb(max(0, n + k - 1), k) for k in range(11)] for n in range(11)]
-)
-_COMB_REP_LOOKUP[0, 0] = 0  # special case
-
-
-@numba_jit(nogil=True)
-def _comb_with_replacement(n: int, k: int) -> int:
-    if (n < _COMB_REP_LOOKUP.shape[0]) and (k < _COMB_REP_LOOKUP.shape[1]):
-        return _COMB_REP_LOOKUP[n, k]
-    n = n + k - 1
-    return _comb(n, k)
-
-
-@numba_jit(nogil=True)
-def _sorted_genotype_index(genotype: ArrayLike) -> int:
-    # Warning: genotype alleles must be sorted in ascending order!
-    if genotype[0] < 0:
-        if genotype[0] < -1:
-            raise ValueError("Mixed-ploidy genotype indicated by allele < -1")
-        return -1
-    index = 0
-    for i in range(len(genotype)):
-        a = genotype[i]
-        index += _comb_with_replacement(a, i + 1)
-    return index
-
-
-@numba_guvectorize(  # type: ignore
-    [
-        "void(int8[:,:], uint64[:], uint64[:])",
-        "void(int16[:,:], uint64[:], uint64[:])",
-        "void(int32[:,:], uint64[:], uint64[:])",
-        "void(int64[:,:], uint64[:], uint64[:])",
-    ],
-    "(n, k),(g)->(g)",
-)
-def _count_sorted_genotypes(
-    genotypes: ArrayLike, _: ArrayLike, out: ArrayLike
-) -> ArrayLike:  # pragma: no cover
-    # Warning: genotype alleles must be sorted in ascending order!
-    out[:] = 0
-    for i in range(len(genotypes)):
-        index = _sorted_genotype_index(genotypes[i])
-        if index >= 0:
-            out[index] += 1
-
-
 def count_variant_genotypes(
     ds: Dataset,
     *,
     call_genotype: Hashable = variables.call_genotype,
     genotype_id: Hashable = variables.genotype_id,
     assign_coords: bool = True,
     merge: bool = True,
@@ -452,14 +316,20 @@
 
     >>> sg.count_variant_genotypes(ds)["variant_genotype_count"].values # doctest: +NORMALIZE_WHITESPACE
     array([[0, 2, 0],
            [0, 1, 1],
            [0, 2, 0],
            [2, 0, 0]], dtype=uint64)
     """
+    from .conversion_numba_fns import (
+        _comb_with_replacement,
+        _count_biallelic_genotypes,
+        _count_sorted_genotypes,
+    )
+
     ds = define_variable_if_absent(
         ds,
         variables.genotype_id,
         genotype_id,
         genotype_coords,
         assign_coords=assign_coords,
     )
@@ -504,137 +374,14 @@
     )
     if assign_coords and not merge:
         # pass through coords
         new_ds = new_ds.assign_coords({"genotypes": ds.coords["genotypes"]})
     return conditional_merge_datasets(ds, new_ds, merge)
 
 
-@numba_guvectorize(  # type: ignore
-    [
-        "void(int64[:], int8[:], int8[:])",
-        "void(int64[:], int16[:], int16[:])",
-        "void(int64[:], int32[:], int32[:])",
-        "void(int64[:], int64[:], int64[:])",
-    ],
-    "(),(k)->(k)",
-)
-def _index_as_genotype(
-    index: int, _: ArrayLike, out: ArrayLike
-) -> None:  # pragma: no cover
-    """Convert the integer index of a genotype to a
-    genotype call following the VCF specification
-    for fields of length G.
-
-    Parameters
-    ----------
-    index
-        Index of genotype following the sort order described in the
-        VCF spec. An index less than 0 is invalid and will return an
-        uncalled genotype.
-    _
-        Dummy variable of length ploidy. The dtype of this variable is
-        used as the dtype of the returned genotype array.
-
-    Returns
-    -------
-    genotype
-        Integer alleles of the genotype call.
-    """
-    ploidy = len(out)
-    remainder = index
-    for index in range(ploidy):
-        # find allele n for position k
-        p = ploidy - index
-        n = -1
-        new = 0
-        prev = 0
-        while new <= remainder:
-            n += 1
-            prev = new
-            new = _comb_with_replacement(n, p)
-        n -= 1
-        remainder -= prev
-        out[p - 1] = n
-
-
-@numba_guvectorize(  # type: ignore
-    [
-        "void(uint8[:], uint8[:], uint8[:], uint8[:])",
-    ],
-    "(b),(),(c)->(c)",
-)
-def _format_genotype_bytes(
-    chars: ArrayLike, ploidy: int, _: ArrayLike, out: ArrayLike
-) -> None:  # pragma: no cover
-    ploidy = ploidy[0]
-    chars_per_allele = len(chars) // ploidy
-    slot = 0
-    for slot in range(ploidy):
-        offset_inp = slot * chars_per_allele
-        offset_out = slot * (chars_per_allele + 1)
-        if slot > 0:
-            out[offset_out - 1] = 47  # "/"
-        for char in range(chars_per_allele):
-            i = offset_inp + char
-            j = offset_out + char
-            val = chars[i]
-            if val == 45:  # "-"
-                if chars[i + 1] == 49:  # "1"
-                    # this is an unknown allele
-                    out[j] = 46  # "."
-                    out[j + 1 : j + chars_per_allele] = 0
-                    break
-                else:
-                    # < -1 indicates a gap
-                    out[j : j + chars_per_allele] = 0
-                    if slot > 0:
-                        # remove separator
-                        out[offset_out - 1] = 0
-                    break
-            else:
-                out[j] = val
-    # shuffle zeros to end
-    c = len(out)
-    for i in range(c):
-        if out[i] == 0:
-            for j in range(i + 1, c):
-                if out[j] != 0:
-                    out[i] = out[j]
-                    out[j] = 0
-                    break
-
-
-def _genotype_as_bytes(genotype: ArrayLike, max_allele_chars: int = 2) -> ArrayLike:
-    """Convert integer encoded genotype calls to (unphased)
-    VCF style byte strings.
-
-    Parameters
-    ----------
-    genotype
-        Genotype call.
-    max_allele_chars
-        Maximum number of chars required for any allele.
-        This should include signed sentinel values.
-
-    Returns
-    -------
-    genotype_string
-        Genotype encoded as byte string.
-    """
-    ploidy = genotype.shape[-1]
-    b = genotype.astype("|S{}".format(max_allele_chars))
-    b.dtype = np.uint8
-    n_num = b.shape[-1]
-    n_char = n_num + ploidy - 1
-    dummy = np.empty(n_char, np.uint8)
-    c = _format_genotype_bytes(b, ploidy, dummy)
-    c.dtype = "|S{}".format(n_char)
-    return np.squeeze(c)
-
-
 def genotype_coords(
     ds: Dataset,
     *,
     chunks=10_000,
     assign_coords: bool = True,
     merge: bool = True,
 ) -> Dataset:
@@ -658,27 +405,29 @@
         See :ref:`dataset_merge` for more details.
 
     Returns
     -------
     A dataset containing :data:`sgkit.variables.genotype_id_spec`
     containing all possible genotype strings.
     """
+    from .conversion_numba_fns import _comb_with_replacement, _index_as_genotype
+
     n_alleles = ds.dims["alleles"]
     ploidy = ds.dims["ploidy"]
     n_genotypes = _comb_with_replacement(n_alleles, ploidy)
     max_chars = len(str(n_alleles - 1))
     # dummy variable for ploidy dim also specifies output dtype
     K = np.empty(ploidy, smallest_numpy_int_dtype(n_alleles - 1))
     X = da.arange(n_genotypes, chunks=chunks)
     chunks = X.chunks + (ploidy,)
     G = da.map_blocks(_index_as_genotype, X, K, new_axis=1, chunks=chunks)
     # allow enough room for all alleles and separators
     dtype = "|S{}".format(max_chars * ploidy + ploidy - 1)
     S = da.map_blocks(
-        _genotype_as_bytes, G, max_chars, drop_axis=1, dtype=dtype
+        genotype_as_bytes, G, False, max_chars, drop_axis=1, dtype=dtype
     ).astype("U")
     new_ds = create_dataset({variables.genotype_id: ("genotypes", S)})
     ds = conditional_merge_datasets(ds, new_ds, merge)
     if assign_coords:
         ds = ds.assign_coords({"genotypes": S})
     return ds
```

### Comparing `sgkit-0.6.0/sgkit/stats/association.py` & `sgkit-0.7.0/sgkit/stats/association.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/genee.py` & `sgkit-0.7.0/sgkit/stats/genee.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/genee_momentchi2py.py` & `sgkit-0.7.0/sgkit/stats/genee_momentchi2py.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/hwe.py` & `sgkit-0.7.0/sgkit/stats/hwe.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/ibs.py` & `sgkit-0.7.0/sgkit/stats/ibs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Hashable
 
 import dask.array as da
-import numpy as np
 from xarray import Dataset
 
 from sgkit import variables
 from sgkit.stats.aggregation import call_allele_frequencies
 from sgkit.utils import (
     conditional_merge_datasets,
     create_dataset,
@@ -13,14 +12,15 @@
 )
 
 
 def identity_by_state(
     ds: Dataset,
     *,
     call_allele_frequency: Hashable = variables.call_allele_frequency,
+    skipna: bool = True,
     merge: bool = True,
 ) -> Dataset:
     """Compute identity by state (IBS) probabilities between
     all pairs of samples.
 
     The IBS probability between a pair of individuals is the
     probability that a randomly drawn allele from the first individual
@@ -32,14 +32,17 @@
     ds
         Dataset containing call genotype alleles.
     call_allele_frequency
         Input variable name holding call_allele_frequency as defined by
         :data:`sgkit.variables.call_allele_frequency_spec`.
         If the variable is not present in ``ds``, it will be computed
         using :func:`call_allele_frequencies`.
+    skipna
+        If True (the default), missing (nan) allele frequencies will be
+        skipped.
     merge
         If True (the default), merge the input dataset and the computed
         output variables into a single dataset, otherwise return only
         the computed output variables.
         See :ref:`dataset_merge` for more details.
 
     Returns
@@ -69,19 +72,22 @@
         call_allele_frequency,
         call_allele_frequencies,
     )
     variables.validate(
         ds, {call_allele_frequency: variables.call_allele_frequency_spec}
     )
     af = da.asarray(ds[call_allele_frequency])
-    af0 = da.where(da.isnan(af), 0.0, af)
-    num = da.einsum("ixj,iyj->xy", af0, af0)
-    called = da.nansum(af, axis=-1)
-    count = da.einsum("ix,iy->xy", called, called)
-    denom = da.where(count == 0, np.nan, count)
+    if skipna:
+        af0 = da.where(da.isnan(af), 0.0, af)
+        num = sum(m.T @ m for m in af0.transpose(2, 0, 1))
+        called = da.nansum(af, axis=-1)
+        denom = called.T @ called
+    else:
+        num = sum(m.T @ m for m in af.transpose(2, 0, 1))
+        denom = len(af)
     new_ds = create_dataset(
         {
             variables.stat_identity_by_state: (
                 ("samples_0", "samples_1"),
                 num / denom,
             )
         }
```

### Comparing `sgkit-0.6.0/sgkit/stats/ld.py` & `sgkit-0.7.0/sgkit/stats/ld.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     func: Callable[..., DataFrame],
     *args: Sequence[ArrayLike],
     window_starts: ArrayLike,
     window_stops: ArrayLike,
     meta: Optional[Any],
     **kwargs: Any,
 ) -> DataFrame:
-
     # Get chunks in leading dimension
     chunks = args[0].chunks[0]
 
     # Find windows in each chunk
     window_lengths = window_stops - window_starts
 
     chunk_starts = _sizes_to_start_offsets(chunks)
@@ -227,15 +226,14 @@
     chunk_window_stops: ArrayLike,
     abs_chunk_start: int,
     chunk_max_window_start: int,
     index_dtype: DType,
     value_dtype: DType,
     threshold: float,
 ) -> List[Any]:  # pragma: no cover
-
     rows = list()
     no_threshold = np.isnan(threshold)
 
     # Iterate over each window in this chunk
     for ti in range(len(chunk_window_starts)):
         window_start = chunk_window_starts[ti]
         window_stop = chunk_window_stops[ti]
@@ -279,15 +277,14 @@
     chunk_window_stops: ArrayLike,
     abs_chunk_start: int,
     chunk_max_window_start: int,
     index_dtype: DType,
     value_dtype: DType,
     threshold: float = np.nan,
 ) -> ArrayLike:
-
     x = np.asarray(args[0])
 
     if len(args) == 2:
         scores = np.asarray(args[1])
     else:
         scores = np.empty(0)
```

### Comparing `sgkit-0.6.0/sgkit/stats/pc_relate.py` & `sgkit-0.7.0/sgkit/stats/pc_relate.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/pca.py` & `sgkit-0.7.0/sgkit/stats/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     >>> # Visualize first two PCs
     >>> ax = (
     ...     ds.sample_pca_projection
     ...     .to_dataframe().unstack()
     ...     .plot.scatter(x=("sample_pca_projection", 0), y=("sample_pca_projection", 1))
     ... )
     >>> ax
-    <AxesSubplot: xlabel='(sample_pca_projection, 0)', ylabel='(sample_pca_projection, 1)'>
+    <Axes: xlabel='(sample_pca_projection, 0)', ylabel='(sample_pca_projection, 1)'>
 
     References
     ----------
     [1] - A. Benson, D. Gleich, and J. Demmel.
     Direct QR factorizations for tall-and-skinny matrices in MapReduce architectures.
     IEEE International Conference on Big Data, 2013.
     https://arxiv.org/abs/1301.1071
```

### Comparing `sgkit-0.6.0/sgkit/stats/pedigree.py` & `sgkit-0.7.0/sgkit/stats/pedigree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Hashable, Tuple
 
 import dask.array as da
 import numpy as np
 import xarray as xr
 from typing_extensions import Literal
 from xarray import Dataset
@@ -297,34 +298,30 @@
         if (parent[i, 0] < 0) or (parent[i, 1] < 0):
             out[i] = True
     return out
 
 
 @numba_jit
 def project_kinship_diploid(
+    initial: ArrayLike,
     parent: ArrayLike,
-    founder_kinship: ArrayLike,
-    founder_indices: ArrayLike,
     allow_half_founders: bool = False,
 ) -> ArrayLike:
     """Project founder kinships along a pedigree to their decedents assuming
     all individuals are diploid.
 
     Parameters
     ----------
+    initial
+        A matrix of shape (samples, samples) containing kinship values among
+        founding samples.
     parent
         A matrix of shape (samples, parents) containing the indices of each
         sample's parents with negative values indicating unknown parents as
         defined in :data:`sgkit.variables.parent_spec`.
-    founder_kinship
-        A matrix of shape (founders, founders) containing kinship values among
-        founding samples.
-    founder_indices
-        An integer array of length founders mapping each founder to a sample
-        in the pedigree.
     allow_half_founders
         If False (the default) then a ValueError will be raised if any
         individuals only have a single recorded parent.
         If True then the unrecorded parent will be assumed to be
         a unique founder unrelated to all other founders.
 
     Note
@@ -341,48 +338,35 @@
     Raises
     ------
     ValueError
         If the pedigree contains a directed loop.
     ValueError
         If the pedigree contains half-founders and allow_half_founders=False.
     ValueError
-        If kinship is not specified for a founder or is specified for a non-founder.
-    ValueError
         If the parents dimension does not have a length of 2.
     """
-    n = len(parent)
-    f = len(founder_indices)
-    assert f < n
-    assert founder_kinship.shape == (f, f)
+    kinship = initial.copy()
+    n_sample = len(parent)
+    assert kinship.shape == (n_sample, n_sample)
     if parent.shape[1] != 2:
         raise ValueError("The parents dimension must be length 2")
     if not allow_half_founders:
         _raise_on_half_founder(parent)
     is_founder = _identify_founders_diploid(parent)
-    if not is_founder[founder_indices].all():
-        raise ValueError("Initial kinship is specified for a non-founder")
-    if is_founder.sum() > f:
-        raise ValueError("Initial kinship is not specified for all founders")
-    kinship = np.zeros((n, n), dtype=founder_kinship.dtype)
-    # populate kinship matrix with founder kinships
-    for idx in range(f):
-        i = founder_indices[idx]
-        for jdx in range(f):
-            j = founder_indices[jdx]
-            kinship[i, j] = founder_kinship[idx, jdx]
+    n_founder = is_founder.sum()
     # order must have founders first
     order = topological_argsort(parent)
     order = np.concatenate(
         (
             order[is_founder[order]],
             order[~is_founder[order]],
         )
     )
     # project founder kinships to other samples
-    for idx in range(f, n):
+    for idx in range(n_founder, n_sample):
         i = order[idx]
         _insert_diploid_self_kinship(kinship, parent, i)
         for jdx in range(idx):
             j = order[jdx]
             _insert_diploid_pair_kinship(kinship, parent, i, j)
     return kinship
 
@@ -679,42 +663,38 @@
             if (parent[i, j] < 0) and tau[i, j] > 0:
                 out[i] = True
     return out
 
 
 @numba_jit
 def project_kinship_Hamilton_Kerr(
+    initial: ArrayLike,
     parent: ArrayLike,
     tau: ArrayLike,
     lambda_: ArrayLike,
-    founder_kinship: ArrayLike,
-    founder_indices: ArrayLike,
     allow_half_founders: bool = False,
 ) -> ArrayLike:
     """Project founder kinships along a pedigree to their decedents within
     an autopolyploid or mixed-ploidy pedigree.
 
     Parameters
     ----------
+    initial
+        A matrix of shape (samples, samples) containing kinship values among
+        founding samples.
     parent
         A matrix of shape (samples, parents) containing the indices of each
         sample's parents with negative values indicating unknown parents as
         defined in :data:`sgkit.variables.parent_spec`.
     tau
         A matrix of shape (samples, parents) containing
         :data:`sgkit.variables.stat_Hamilton_Kerr_tau_spec`.
     lambda_
         A matrix of shape (samples, parents) containing
         :data:`sgkit.variables.stat_Hamilton_Kerr_lambda_spec`.
-    founder_kinship
-        A matrix of shape (founders, founders) containing kinship values among
-        founding samples.
-    founder_indices
-        An integer array of length founders mapping each founder to a sample
-        in the pedigree.
     allow_half_founders
         If False (the default) then a ValueError will be raised if any
         individuals only have a single recorded parent.
         If True then the unrecorded parent will be assumed to be
         a unique founder unrelated to all other founders.
 
     Returns
@@ -726,49 +706,35 @@
     Raises
     ------
     ValueError
         If the pedigree contains a directed loop.
     ValueError
         If the pedigree contains half-founders and allow_half_founders=False.
     ValueError
-        If kinship is not specified for a founder or is specified for a non-founder.
-    ValueError
         If a sample has more than two contributing parents.
     """
-    n = len(parent)
-    f = len(founder_indices)
-    assert f < n
-    assert founder_kinship.shape == (f, f)
+    kinship = initial.copy()
+    n_sample = len(parent)
+    assert kinship.shape == (n_sample, n_sample)
     if parent.shape[1] != 2:
         parent, tau, lambda_ = _compress_hamilton_kerr_parameters(parent, tau, lambda_)
     if not allow_half_founders:
         _raise_on_half_founder(parent, tau)
     is_founder = _identify_founders_Hamilton_Kerr(parent, tau)
-    if not is_founder[founder_indices].all():
-        raise ValueError("Initial kinship is specified for a non-founder")
-    if is_founder.sum() > f:
-        raise ValueError("Initial kinship is not specified for all founders")
-    order = topological_argsort(parent)
-    kinship = np.zeros((n, n), dtype=founder_kinship.dtype)
-    # populate kinship matrix with founder kinships
-    for idx in range(f):
-        i = founder_indices[idx]
-        for jdx in range(f):
-            j = founder_indices[jdx]
-            kinship[i, j] = founder_kinship[idx, jdx]
+    n_founder = is_founder.sum()
     # order must have founders first
     order = topological_argsort(parent)
     order = np.concatenate(
         (
             order[is_founder[order]],
             order[~is_founder[order]],
         )
     )
     # project founder kinships to other samples
-    for idx in range(f, n):
+    for idx in range(n_founder, n_sample):
         i = order[idx]
         _insert_hamilton_kerr_self_kinship(kinship, parent, tau, lambda_, i)
         for jdx in range(idx):
             j = order[jdx]
             _insert_hamilton_kerr_pair_kinship(kinship, parent, tau, i, j)
     return kinship
 
@@ -823,24 +789,28 @@
         If True then the unrecorded parent will be assumed to be
         a unique founder unrelated to all other founders.
         If the Hamilton-Kerr method is used with half-founders then
         the tau and lambda parameters for gametes contributing to the
         unrecorded parent will be assumed to be equal to those of the
         gamete originating from that parent.
     founder_kinship
-        Optionally specify a matrix of pairwise kinship estimates among
-        founder samples which will be used to initialize pedigree estimates
-        as outlined by Goudet et al. 2018 [2].
-        This variable must be a square matrix of shape (founders, founders)
-        and must be used in conjunction with founder_indices.
+        Optionally specify an input kinship matrix as defined by
+        :data:`sgkit.variables.stat_genomic_kinship_spec`. Kinship
+        estimates among founders within this matrix will be used to
+        initialize the pedigree estimates as outlined by Goudet et al
+        2018 [2]. Kinship estimates for non-founders are ignored.
     founder_indices
         Optionally specify an array of integer indices mapping rows/columns
-        in the founder_kinship matrix to sample positions in the samples
+        in a founder_kinship sub-matrix to sample positions in the samples
         dimension (i.e., the order of rows in the parent array).
         This variable must have the same length as founder_kinship.
+
+        .. deprecated:: 0.7.0
+            Instead, use a 'founder_kinship' matrix with values for
+            all pairs of samples (these may be nan values).
     merge
         If True (the default), merge the input dataset and the computed
         output variables into a single dataset, otherwise return only
         the computed output variables.
 
     Returns
     -------
@@ -861,22 +831,20 @@
         have a length of two.
     ValueError
         If the Hamilton-Kerr method is used and a sample has more than
         two contributing parents.
     ValueError
         If the pedigree contains half-founders and allow_half_founders=False.
     ValueError
-        If only one of the ``founder_kinship`` or ``founder_indices``
-        variables is specified.
-    ValueError
-        If the ``founder_kinship`` or ``founder_indices`` variables have
-        inconsistent shapes.
+        If the dimension sizes of ``founder_kinship`` are not equal to
+        the number of samples in the pedigree (when ``founder_indices`` is
+        not specified).
     ValueError
-        If a founder is missing from the ``founder_indices`` array or if
-        a non-founder is indicated by this array.
+        If the ``founder_kinship`` and ``founder_indices`` variables are
+        both specified and have inconsistent shapes.
 
     Note
     ----
     This method is faster when a pedigree is sorted in topological order
     such that parents occur before their children.
 
     Note
@@ -931,34 +899,34 @@
            [0.  , 1.  , 0.5 , 0.25],
            [0.5 , 0.5 , 1.  , 0.75],
            [0.75, 0.25, 0.75, 1.25]])
 
     Inbred diploid pedigree with related founders:
 
     >>> import sgkit as sg
+    >>> from numpy import nan
     >>> ds = sg.simulate_genotype_call_dataset(n_variant=1, n_sample=4, seed=1)
     >>> ds.sample_id.values # doctest: +NORMALIZE_WHITESPACE
     array(['S0', 'S1', 'S2', 'S3'], dtype='<U2')
     >>> ds["parent_id"] = ["samples", "parents"], [
     ...     [".", "."],
     ...     [".", "."],
     ...     ["S0", "S1"],
     ...     ["S0", "S2"]
     ... ]
     >>> # add "known" kinships among founders
-    >>> ds["founder_kinship"] = ["founders_0", "founders_1"], [
-    ...     [0.5, 0.1],
-    ...     [0.1, 0.6],
+    >>> ds["founder_kinship"] = ["samples_0", "samples_1"], [
+    ...     [0.5, 0.1, nan, nan],
+    ...     [0.1, 0.6, nan, nan],
+    ...     [nan, nan, nan, nan],
+    ...     [nan, nan, nan, nan],
     ... ]
-    >>> # founder kinships correspond to the first two samples
-    >>> ds["founder_indices"] = ["founders"], [0, 1]
     >>> ds = sg.pedigree_kinship(
     ...     ds,
     ...     founder_kinship="founder_kinship",
-    ...     founder_indices="founder_indices",
     ... )
     >>> ds["stat_pedigree_kinship"].values # doctest: +NORMALIZE_WHITESPACE
     array([[0.5  , 0.1  , 0.3  , 0.4  ],
            [0.1  , 0.6  , 0.35 , 0.225],
            [0.3  , 0.35 , 0.55 , 0.425],
            [0.4  , 0.225, 0.425, 0.65 ]])
 
@@ -1033,53 +1001,74 @@
     "How to estimate kinship." Molecular Ecology 27: 4121-4135.
     """
     if method not in {"diploid", "Hamilton-Kerr"}:
         raise ValueError("Unknown method '{}'".format(method))
     ds = define_variable_if_absent(ds, variables.parent, parent, parent_indices)
     variables.validate(ds, {parent: variables.parent_spec})
     parent = da.asarray(ds[parent].data, chunks=ds[parent].shape)
-    if (founder_kinship is not None) or (founder_indices is not None):
-        if (founder_kinship is None) or (founder_indices is None):
-            raise ValueError(
-                "Variables founder_kinship and founder_indices must be specified together"
+    n_samples = len(parent)
+    if founder_kinship is not None:
+        if founder_indices is not None:
+            # Deprecated API
+            warnings.warn(
+                (
+                    "The 'founder_indices' parameter is deprecated and, instead, the "
+                    "dimension sizes of 'founder_kinship' should equal the number of samples"
+                ),
+                DeprecationWarning,
             )
-        founder_kinship = da.asarray(
-            ds[founder_kinship].data, chunks=ds[founder_kinship].shape
-        )
-        founder_indices = da.asarray(
-            ds[founder_indices].data, chunks=ds[founder_indices].shape
-        )
-        n_founders = len(founder_indices)
-        if founder_kinship.shape != (n_founders, n_founders):
-            raise ValueError(
-                "Variables founder_kinship and founder_indices have mismatching dimensions"
+            founder_kinship = da.asarray(
+                ds[founder_kinship].data, chunks=ds[founder_kinship].shape
             )
-        if n_founders > len(parent):
-            raise ValueError(
-                "The number of founders exceeds the total number of samples"
+            founder_indices = ds[founder_indices].values
+            n_founders = len(founder_indices)
+            if founder_kinship.shape != (n_founders, n_founders):
+                raise ValueError(
+                    "Variables founder_kinship and founder_indices have mismatching dimensions"
+                )
+            if n_founders > n_samples:
+                raise ValueError(
+                    "The number of founders exceeds the total number of samples"
+                )
+            # pad with nans for non-founder values
+            _founder_kinship_ff = founder_kinship
+            _founder_kinship_sf = da.full((n_samples, n_founders), np.nan)
+            _founder_kinship_sf[founder_indices] = _founder_kinship_ff
+            founder_kinship = da.full((n_samples, n_samples), np.nan)
+            founder_kinship[:, founder_indices] = _founder_kinship_sf
+        else:
+            # New API
+            variables.validate(
+                ds, {founder_kinship: variables.stat_genomic_kinship_spec}
             )
+            founder_kinship = da.asarray(
+                ds[founder_kinship].data, chunks=ds[founder_kinship].shape
+            )
+            if founder_kinship.shape != (n_samples, n_samples):
+                raise ValueError(
+                    "Dimension sizes of founder_kinship should equal the number of samples"
+                )
     if method == "diploid":
         # check ploidy dimension and assume diploid if it's absent
         if ds.dims.get("ploidy", 2) != 2:
             raise ValueError("Dataset is not diploid")
         if founder_kinship is None:
             func = da.gufunc(
                 kinship_diploid, signature="(n, p) -> (n, n)", output_dtypes=float
             )
             kinship = func(parent, allow_half_founders=allow_half_founders)
         else:
             func = da.gufunc(
                 project_kinship_diploid,
-                signature="(n, p),(f, f),(f)-> (n, n)",
+                signature="(n, n),(n, p)-> (n, n)",
                 output_dtypes=float,
             )
             kinship = func(
-                parent,
                 founder_kinship,
-                founder_indices,
+                parent,
                 allow_half_founders=allow_half_founders,
             )
     elif method == "Hamilton-Kerr":
         tau = da.asarray(
             ds[stat_Hamilton_Kerr_tau].data, ds[stat_Hamilton_Kerr_tau].shape
         )
         lambda_ = da.asarray(
@@ -1093,23 +1082,22 @@
             )
             kinship = func(
                 parent, tau, lambda_, allow_half_founders=allow_half_founders
             )
         else:
             func = da.gufunc(
                 project_kinship_Hamilton_Kerr,
-                signature="(n, p),(n, p),(n, p),(f, f),(f)-> (n, n)",
+                signature="(n, n),(n, p),(n, p),(n, p)-> (n, n)",
                 output_dtypes=float,
             )
             kinship = func(
+                founder_kinship,
                 parent,
                 tau,
                 lambda_,
-                founder_kinship,
-                founder_indices,
                 allow_half_founders=allow_half_founders,
             )
     dims = ["samples_0", "samples_1"]
     if return_relationship:
         relationship = kinship * 2
         if method == "Hamilton-Kerr":
             ploidy = tau.sum(axis=-1)
```

### Comparing `sgkit-0.6.0/sgkit/stats/popgen.py` & `sgkit-0.7.0/sgkit/stats/popgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 import itertools
 from typing import Hashable, Optional, Sequence, Tuple, Union
 
 import dask.array as da
 import numpy as np
 from xarray import Dataset
 
-from sgkit.accelerate import numba_guvectorize
 from sgkit.cohorts import _cohorts_to_array
 from sgkit.stats.utils import assert_array_shape
-from sgkit.typing import ArrayLike
 from sgkit.utils import (
     conditional_merge_datasets,
     create_dataset,
     define_variable_if_absent,
-    hash_array,
 )
 from sgkit.window import has_windows, window_statistic
 
 from .. import variables
 from .aggregation import (
     count_cohort_alleles,
     count_variant_alleles,
     individual_heterozygosity,
 )
-from .utils import cohort_nanmean
 
 
 def diversity(
     ds: Dataset,
     *,
     cohort_allele_count: Hashable = variables.cohort_allele_count,
     merge: bool = True,
@@ -128,59 +124,14 @@
                     pi.data,
                 )
             }
         )
     return conditional_merge_datasets(ds, new_ds, merge)
 
 
-# c = cohorts, k = alleles
-@numba_guvectorize(  # type: ignore
-    ["void(int64[:, :], float64[:,:])", "void(uint64[:, :], float64[:,:])"],
-    "(c, k)->(c,c)",
-)
-def _divergence(ac: ArrayLike, out: ArrayLike) -> None:  # pragma: no cover
-    """Generalized U-function for computing divergence.
-
-    Parameters
-    ----------
-    ac
-        Allele counts of shape (cohorts, alleles) containing per-cohort allele counts.
-    out
-        Pairwise divergence stats with shape (cohorts, cohorts), where the entry at
-        (i, j) is the divergence between cohort i and cohort j.
-    """
-    an = ac.sum(axis=-1)
-    out[:, :] = np.nan  # (cohorts, cohorts)
-    n_cohorts = ac.shape[0]
-    n_alleles = ac.shape[1]
-    # calculate the divergence for each cohort pair
-    for i in range(n_cohorts):
-        for j in range(i + 1, n_cohorts):
-            n_pairs = an[i] * an[j]
-            if n_pairs != 0.0:
-                n_same = 0
-                for k in range(n_alleles):
-                    n_same += ac[i, k] * ac[j, k]
-                n_diff = n_pairs - n_same
-                div = n_diff / n_pairs
-                out[i, j] = div
-                out[j, i] = div
-
-    # calculate the diversity for each cohort
-    for i in range(n_cohorts):
-        n_pairs = an[i] * (an[i] - 1)
-        n_same = 0
-        for k in range(n_alleles):
-            n_same += ac[i, k] * (ac[i, k] - 1)
-        n_diff = n_pairs - n_same
-        if n_pairs != 0.0:
-            div = n_diff / n_pairs
-            out[i, i] = div
-
-
 def divergence(
     ds: Dataset,
     *,
     cohort_allele_count: Hashable = variables.cohort_allele_count,
     merge: bool = True,
 ) -> Dataset:
     """Compute divergence between pairs of cohorts.
@@ -253,14 +204,15 @@
     >>> sg.divergence(ds)["stat_divergence"].values # doctest: +NORMALIZE_WHITESPACE
     array([[[1.83333333, 1.5       ],
             [1.5       , 1.83333333]],
     <BLANKLINE>
         [[1.        , 1.        ],
             [1.        , 1.        ]]])
     """
+    from .popgen_numba_fns import _divergence
 
     ds = define_variable_if_absent(
         ds, variables.cohort_allele_count, cohort_allele_count, count_cohort_alleles
     )
     variables.validate(ds, {cohort_allele_count: variables.cohort_allele_count_spec})
     ac = ds[cohort_allele_count]
 
@@ -296,75 +248,14 @@
                     d,
                 )
             }
         )
     return conditional_merge_datasets(ds, new_ds, merge)
 
 
-# c = cohorts
-@numba_guvectorize(  # type: ignore
-    [
-        "void(float32[:,:], float32[:,:])",
-        "void(float64[:,:], float64[:,:])",
-    ],
-    "(c,c)->(c,c)",
-)
-def _Fst_Hudson(d: ArrayLike, out: ArrayLike) -> None:  # pragma: no cover
-    """Generalized U-function for computing Fst using Hudson's estimator.
-
-    Parameters
-    ----------
-    d
-        Pairwise divergence values of shape (cohorts, cohorts),
-        with diversity values on the diagonal.
-    out
-        Pairwise Fst with shape (cohorts, cohorts), where the entry at
-        (i, j) is the Fst for cohort i and cohort j.
-    """
-    out[:, :] = np.nan  # (cohorts, cohorts)
-    n_cohorts = d.shape[0]
-    for i in range(n_cohorts):
-        for j in range(i + 1, n_cohorts):
-            if d[i, j] != 0.0:
-                fst = 1 - ((d[i, i] + d[j, j]) / 2) / d[i, j]
-                out[i, j] = fst
-                out[j, i] = fst
-
-
-# c = cohorts
-@numba_guvectorize(  # type: ignore
-    [
-        "void(float32[:,:], float32[:,:])",
-        "void(float64[:,:], float64[:,:])",
-    ],
-    "(c,c)->(c,c)",
-)
-def _Fst_Nei(d: ArrayLike, out: ArrayLike) -> None:  # pragma: no cover
-    """Generalized U-function for computing Fst using Nei's estimator.
-
-    Parameters
-    ----------
-    d
-        Pairwise divergence values of shape (cohorts, cohorts),
-        with diversity values on the diagonal.
-    out
-        Pairwise Fst with shape (cohorts, cohorts), where the entry at
-        (i, j) is the Fst for cohort i and cohort j.
-    """
-    out[:, :] = np.nan  # (cohorts, cohorts)
-    n_cohorts = d.shape[0]
-    for i in range(n_cohorts):
-        for j in range(i + 1, n_cohorts):
-            den = d[i, i] + 2 * d[i, j] + d[j, j]
-            if den != 0.0:
-                fst = 1 - (2 * (d[i, i] + d[j, j]) / den)
-                out[i, j] = fst
-                out[j, i] = fst
-
-
 def Fst(
     ds: Dataset,
     *,
     estimator: Optional[str] = None,
     stat_divergence: Hashable = variables.stat_divergence,
     merge: bool = True,
 ) -> Dataset:
@@ -441,14 +332,16 @@
     >>> sg.Fst(ds)["stat_Fst"].values # doctest: +NORMALIZE_WHITESPACE
     array([[[        nan, -0.22222222],
             [-0.22222222,         nan]],
     <BLANKLINE>
         [[        nan,  0.        ],
             [ 0.        ,         nan]]])
     """
+    from .popgen_numba_fns import _Fst_Hudson, _Fst_Nei
+
     known_estimators = {"Hudson": _Fst_Hudson, "Nei": _Fst_Nei}
     if estimator is not None and estimator not in known_estimators:
         raise ValueError(
             f"Estimator '{estimator}' is not a known estimator: {known_estimators.keys()}"
         )
     estimator = estimator or "Hudson"
     ds = define_variable_if_absent(
@@ -608,57 +501,14 @@
     else:
         new_ds = create_dataset(
             {variables.stat_Tajimas_D: (["variants", "cohorts"], D.data)}
         )
     return conditional_merge_datasets(ds, new_ds, merge)
 
 
-# c = cohorts
-@numba_guvectorize(  # type: ignore
-    ["void(float32[:, :], float32[:,:,:])", "void(float64[:, :], float64[:,:,:])"],
-    "(c,c)->(c,c,c)",
-)
-def _pbs(t: ArrayLike, out: ArrayLike) -> None:  # pragma: no cover
-    """Generalized U-function for computing PBS."""
-    out[:, :, :] = np.nan  # (cohorts, cohorts, cohorts)
-    n_cohorts = t.shape[0]
-    # calculate PBS for each cohort triple
-    for i in range(n_cohorts):
-        for j in range(i + 1, n_cohorts):
-            for k in range(j + 1, n_cohorts):
-                ret = (t[i, j] + t[i, k] - t[j, k]) / 2
-                norm = 1 + (t[i, j] + t[i, k] + t[j, k]) / 2
-                ret = ret / norm
-                out[i, j, k] = ret
-
-
-# c = cohorts, ct = cohort_triples, i = index (size 3)
-@numba_guvectorize(  # type: ignore
-    [
-        "void(float32[:, :], int32[:, :], float32[:,:,:])",
-        "void(float64[:, :], int32[:, :], float64[:,:,:])",
-    ],
-    "(c,c),(ct,i)->(c,c,c)",
-)
-def _pbs_cohorts(
-    t: ArrayLike, ct: ArrayLike, out: ArrayLike
-) -> None:  # pragma: no cover
-    """Generalized U-function for computing PBS."""
-    out[:, :, :] = np.nan  # (cohorts, cohorts, cohorts)
-    n_cohort_triples = ct.shape[0]
-    for n in range(n_cohort_triples):
-        i = ct[n, 0]
-        j = ct[n, 1]
-        k = ct[n, 2]
-        ret = (t[i, j] + t[i, k] - t[j, k]) / 2
-        norm = 1 + (t[i, j] + t[i, k] + t[j, k]) / 2
-        ret = ret / norm
-        out[i, j, k] = ret
-
-
 def pbs(
     ds: Dataset,
     *,
     stat_Fst: Hashable = variables.stat_Fst,
     cohorts: Optional[
         Sequence[Union[Tuple[int, int, int], Tuple[str, str, str]]]
     ] = None,
@@ -717,14 +567,15 @@
     >>> ds = ds.assign_coords({"cohorts_0": cohort_names, "cohorts_1": cohort_names, "cohorts_2": cohort_names})
 
     >>> # Divide into two windows of size three (variants)
     >>> ds = sg.window_by_variant(ds, size=3)
     >>> sg.pbs(ds)["stat_pbs"].sel(cohorts_0="co_0", cohorts_1="co_1", cohorts_2="co_2").values # doctest: +NORMALIZE_WHITESPACE
     array([ 0.      , -0.160898])
     """
+    from .popgen_numba_fns import _pbs_cohorts
 
     ds = define_variable_if_absent(ds, variables.stat_Fst, stat_Fst, Fst)
     variables.validate(ds, {stat_Fst: variables.stat_Fst_spec})
 
     fst = ds[variables.stat_Fst]
     fst = fst.clip(min=0, max=(1 - np.finfo(float).epsneg))
 
@@ -779,14 +630,16 @@
     return np.array([h1, h12, h123, h2_h1])
 
 
 def _Garud_h_cohorts(
     gt: np.ndarray, sample_cohort: np.ndarray, n_cohorts: int, ct: np.ndarray
 ) -> np.ndarray:
     # transpose to hash columns (haplotypes)
+    from .popgen_numba_fns import hash_array
+
     haplotypes = hash_array(gt.transpose()).transpose().flatten()
     arr = np.full((n_cohorts, N_GARUD_H_STATS), np.nan)
     for c in np.nditer(ct):
         arr[c, :] = _Garud_h(haplotypes[sample_cohort == c])
     return arr
 
 
@@ -998,14 +851,16 @@
 
     >>> # Divide into windows of size three (variants)
     >>> ds = sg.window_by_variant(ds, size=3)
     >>> sg.observed_heterozygosity(ds)["stat_observed_heterozygosity"].values # doctest: +NORMALIZE_WHITESPACE
     array([[1.5, 2.5],
         [1. , 1. ]])
     """
+    from .cohort_numba_fns import cohort_nanmean
+
     ds = define_variable_if_absent(
         ds,
         variables.call_heterozygosity,
         call_heterozygosity,
         individual_heterozygosity,
     )
     variables.validate(ds, {call_heterozygosity: variables.call_heterozygosity_spec})
```

### Comparing `sgkit-0.6.0/sgkit/stats/preprocessing.py` & `sgkit-0.7.0/sgkit/stats/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/stats/regenie.py` & `sgkit-0.7.0/sgkit/stats/regenie.py`

 * *Files identical despite different names*

### Comparing `sgkit-0.6.0/sgkit/utils.py` & `sgkit-0.7.0/sgkit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import warnings
 from itertools import product
 from typing import Any, Callable, Hashable, List, Mapping, Optional, Set, Tuple, Union
 
+import dask.array as da
 import numpy as np
 from xarray import Dataset
 
-from sgkit.accelerate import numba_guvectorize
-
 from . import variables
 from .typing import ArrayLike, DType
 
 
 class DimensionWarning(UserWarning):
     "Warning about dimension mismatches."
     pass
@@ -382,54 +381,23 @@
     if a.size == 0:
         raise ValueError("Max string length cannot be calculated for empty array")
     if a.dtype.kind == "O":
         a = a.astype(str)
     if a.dtype.kind not in {"U", "S"}:
         raise ValueError(f"Array must have string dtype (got dtype {a.dtype})")
 
-    lens = np.frompyfunc(len, 1, 1)(a)  # type: ignore[no-untyped-call]
+    lens = da.frompyfunc(len, 1, 1)(a)  # type: ignore[no-untyped-call]
     if isinstance(a, np.ndarray):
         lens = np.asarray(lens)
     if a.ndim == 0:
         return lens
     else:
         return lens.max()
 
 
-@numba_guvectorize(  # type: ignore
-    [
-        "void(int8[:], int64[:])",
-        "void(int16[:], int64[:])",
-        "void(int32[:], int64[:])",
-        "void(int64[:], int64[:])",
-    ],
-    "(n)->()",
-)
-def hash_array(x: ArrayLike, out: ArrayLike) -> None:  # pragma: no cover
-    """Hash entries of ``x`` using the DJBX33A hash function.
-
-    This is ~5 times faster than calling ``tobytes()`` followed
-    by ``hash()`` on array columns. This function also does not
-    hold the GIL, making it suitable for use with the Dask
-    threaded scheduler.
-
-    Parameters
-    ----------
-    x
-        1D array of type integer.
-
-    Returns
-    -------
-    Array containing a single hash value of type int64.
-    """
-    out[0] = 5381
-    for i in range(x.shape[0]):
-        out[0] = out[0] * 33 + x[i]
-
-
 def smallest_numpy_int_dtype(value: int) -> Optional[DType]:
     """Return the smallest NumPy signed integer dtype that can be used to store the given value.
 
     Parameters
     ----------
     value
         An integer value to be stored.
```

### Comparing `sgkit-0.6.0/sgkit/variables.py` & `sgkit-0.7.0/sgkit/variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -302,15 +302,18 @@
         "call_genotype_mask",
         kind="b",
         dims=("variants", "samples", "ploidy"),
         __doc__="""A flag for each call indicating which values are missing.""",
     )
 )
 
-(call_genotype_fill, call_genotype_fill_spec,) = SgkitVariables.register_variable(
+(
+    call_genotype_fill,
+    call_genotype_fill_spec,
+) = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "call_genotype_fill",
         kind="b",
         dims=("variants", "samples", "ploidy"),
         __doc__="""
 A flag for each allele position within mixed ploidy call genotypes
 indicating fill (non-allele) values of lower ploidy calls.
@@ -350,14 +353,48 @@
         "call_genotype_complete_mask",
         kind="b",
         dims=("variants", "samples", "ploidy"),
         __doc__="""A flag for each call indicating which values are missing.""",
     )
 )
 
+
+(
+    call_genotype_index,
+    call_genotype_index_spec,
+) = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "call_genotype_index",
+        kind="i",
+        dims=("variants", "samples"),
+        __doc__="""
+Single integer values encoding each call genotype. Each unique integer corresponds
+to a unique call genotype following the VCF specification for arrays of size "G".
+For biallelic genotypes, this is the count of the alternate allele. Values of -1
+indicate call genotypes with missing alleles.
+""",
+    )
+)
+
+(
+    call_genotype_index_mask,
+    call_genotype_index_mask_spec,
+) = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "call_genotype_index_mask",
+        kind="b",
+        dims=("variants", "samples"),
+        __doc__="""
+A flag for each call genotype index indicating missing indices (-1) which correspond
+to call genotypes with missing alleles.
+""",
+    )
+)
+
+
 (
     call_genotype_probability,
     call_genotype_probability_spec,
 ) = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "call_genotype_probability",
         kind="f",
@@ -418,14 +455,23 @@
         __doc__="""
 Cohort Allele frequencies. With shape (variants, cohorts, alleles) and values
 corresponding to the frequencies of non-missing occurrences of each allele.
 """,
     )
 )
 
+contig_id, contig_id_spec = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "contig_id",
+        dims=("contigs",),
+        kind={"S", "U", "O"},
+        __doc__="""Contig identifiers.""",
+    )
+)
+
 covariates, covariates_spec = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "covariates",
         ndim={1, 2},
         __doc__="""
 Covariate variable names. Must correspond to 1 or 2D dataset
 variables of shape (samples[, covariates]). All covariate arrays
@@ -776,14 +822,25 @@
         "stat_Garud_h2_h1",
         dims=("windows", "cohorts"),
         kind="f",
         __doc__="""Garud H2/H1 statistic for cohorts.""",
     )
 )
 
+stat_genomic_kinship, stat_genomic_kinship_spec = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "stat_genomic_kinship",
+        dims=("samples_0", "samples_1"),
+        kind="f",
+        __doc__="""
+Genomic kinship matrix with self-kinship values on the diagonal.
+""",
+    )
+)
+
 (
     stat_genomic_relationship,
     stat_genomic_relationship_spec,
 ) = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "stat_genomic_relationship",
         dims=("samples_0", "samples_1"),
@@ -842,14 +899,39 @@
         dims=("samples_0", "samples_1"),
         kind="f",
         __doc__="""Inverse of a kinship matrix calculated from pedigree structure.""",
     )
 )
 
 (
+    stat_hybrid_relationship,
+    stat_hybrid_relationship_spec,
+) = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "stat_hybrid_relationship",
+        dims=("samples_0", "samples_1"),
+        kind="f",
+        __doc__="""The hybrid relationship matrix or "H-matrix".""",
+    )
+)
+
+
+(
+    stat_hybrid_inverse_relationship,
+    stat_hybrid_inverse_relationship_spec,
+) = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "stat_hybrid_inverse_relationship",
+        dims=("samples_0", "samples_1"),
+        kind="f",
+        __doc__="""Inverse of the hybrid relationship matrix or "H-matrix".""",
+    )
+)
+
+(
     stat_pedigree_inverse_relationship,
     stat_pedigree_inverse_relationship_spec,
 ) = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "stat_pedigree_inverse_relationship",
         dims=("samples_0", "samples_1"),
         kind="f",
@@ -912,14 +994,30 @@
         "stat_pedigree_relationship",
         dims=("samples_0", "samples_1"),
         kind="f",
         __doc__="""Relationship matrix derived from pedigree structure.""",
     )
 )
 
+
+(
+    stat_inverse_relationship,
+    stat_inverse_relationship_spec,
+) = SgkitVariables.register_variable(
+    ArrayLikeSpec(
+        "stat_inverse_relationship",
+        dims=("samples_0", "samples_1"),
+        kind="f",
+        __doc__="""
+The inverse of a relationship matrix. This may contain the inverse of a subset of
+a relationship matrix in which nan values indicate elements outside of the subset.
+""",
+    )
+)
+
 stat_Tajimas_D, stat_Tajimas_D_spec = SgkitVariables.register_variable(
     ArrayLikeSpec(
         "stat_Tajimas_D",
         dims=({"windows", "variants"}, "cohorts"),
         kind="f",
         __doc__="""Tajima’s D for cohorts.""",
     )
```

### Comparing `sgkit-0.6.0/sgkit/window.py` & `sgkit-0.7.0/sgkit/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Callable, Hashable, Iterable, Optional, Tuple, Union
 
 import dask.array as da
 import numpy as np
 from xarray import Dataset
 
 from sgkit import variables
+from sgkit.model import get_contigs, num_contigs
 from sgkit.utils import conditional_merge_datasets, create_dataset
 from sgkit.variables import window_contig, window_start, window_stop
 
 from .typing import ArrayLike, DType
 
 # Window definition (user code)
 
@@ -302,24 +303,24 @@
     variant_contig: Hashable,
     merge: bool,
     windowing_fn: Callable[..., Any],
     *args: Any,
     **kwargs: Any,
 ) -> Dataset:
     n_variants = ds.dims["variants"]
-    n_contigs = len(ds.attrs["contigs"])
+    n_contigs = num_contigs(ds)
     contig_ids = np.arange(n_contigs)
     variant_contig = ds["variant_contig"]
     contig_starts = np.searchsorted(variant_contig.values, contig_ids)
     contig_bounds = np.append(contig_starts, [n_variants], axis=0)  # type: ignore[no-untyped-call]
 
     contig_window_contigs = []
     contig_window_starts = []
     contig_window_stops = []
-    for i, contig in enumerate(ds.attrs["contigs"]):
+    for i, contig in enumerate(get_contigs(ds)):
         starts, stops = windowing_fn(
             contig, contig_bounds[i], contig_bounds[i + 1], *args, **kwargs
         )
         contig_window_starts.append(starts)
         contig_window_stops.append(stops)
         contig_window_contigs.append(np.full_like(starts, i))
 
@@ -495,15 +496,14 @@
     window_starts: ArrayLike,
     window_stops: ArrayLike,
     dtype: DType,
     chunks: Any = None,
     new_axis: Union[None, int, Iterable[int]] = None,
     **kwargs: Any,
 ) -> da.Array:
-
     values = da.asarray(values)
     desired_chunks = chunks or values.chunks
 
     # special-case for whole-genome
     if (
         len(window_starts) == 1
         and window_starts == np.array([0])
```

### Comparing `sgkit-0.6.0/sgkit.egg-info/PKG-INFO` & `sgkit-0.7.0/sgkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgkit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Statistical genetics toolkit
 Home-page: https://github.com/pystatgen/sgkit
 Author: sgkit Developers
 Author-email: project@pystatgen.org
 License: Apache
 Description: 
         **sgkit** is an open source project for analyzing and manipulating genetic
```

### Comparing `sgkit-0.6.0/sgkit.egg-info/SOURCES.txt` & `sgkit-0.7.0/sgkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements-dev.txt
 requirements-doc.txt
 requirements.txt
 setup.cfg
 setup.py
 benchmarks/__init__.py
 benchmarks/asv.conf.json
+benchmarks/benchmarks_plink.py
 benchmarks/benchmarks_stats.py
 benchmarks/benchmarks_vcf.py
 docs/.gitignore
 docs/Makefile
 docs/about.rst
 docs/api.rst
 docs/changelog.rst
@@ -39,14 +40,15 @@
 docs/examples/index.rst
 docs/extensions/typed_returns.py
 docs/news/introducing_sgkit.md
 sgkit/__init__.py
 sgkit/accelerate.py
 sgkit/cohorts.py
 sgkit/display.py
+sgkit/display_numba_fns.py
 sgkit/model.py
 sgkit/py.typed
 sgkit/testing.py
 sgkit/typing.py
 sgkit/utils.py
 sgkit/variables.py
 sgkit/window.py
@@ -63,32 +65,37 @@
 sgkit/io/dataset.py
 sgkit/io/utils.py
 sgkit/io/vcfzarr_reader.py
 sgkit/io/bgen/__init__.py
 sgkit/io/bgen/bgen_reader.py
 sgkit/io/plink/__init__.py
 sgkit/io/plink/plink_reader.py
+sgkit/io/plink/plink_writer.py
 sgkit/io/vcf/__init__.py
 sgkit/io/vcf/csi.py
 sgkit/io/vcf/tbi.py
 sgkit/io/vcf/utils.py
 sgkit/io/vcf/vcf_partition.py
 sgkit/io/vcf/vcf_reader.py
 sgkit/io/vcf/vcf_writer.py
 sgkit/io/vcf/vcf_writer_utils.py
 sgkit/stats/__init__.py
 sgkit/stats/aggregation.py
+sgkit/stats/aggregation_numba_fns.py
 sgkit/stats/association.py
+sgkit/stats/cohort_numba_fns.py
 sgkit/stats/conversion.py
+sgkit/stats/conversion_numba_fns.py
 sgkit/stats/genee.py
 sgkit/stats/genee_momentchi2py.py
 sgkit/stats/grm.py
 sgkit/stats/hwe.py
 sgkit/stats/ibs.py
 sgkit/stats/ld.py
 sgkit/stats/pc_relate.py
 sgkit/stats/pca.py
 sgkit/stats/pedigree.py
 sgkit/stats/popgen.py
+sgkit/stats/popgen_numba_fns.py
 sgkit/stats/preprocessing.py
 sgkit/stats/regenie.py
 sgkit/stats/utils.py
```

