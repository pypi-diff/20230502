# Comparing `tmp/pysnptools-0.5.8.tar.gz` & `tmp/pysnptools-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnptools-0.5.8.tar", last modified: Wed Feb  1 15:08:11 2023, max compression
+gzip compressed data, was "pysnptools-0.5.9.tar", last modified: Mon May  1 23:49:51 2023, max compression
```

## Comparing `pysnptools-0.5.8.tar` & `pysnptools-0.5.9.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.427321 pysnptools-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-01 15:07:21.000000 pysnptools-0.5.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-02-01 15:07:21.000000 pysnptools-0.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-01 15:07:21.000000 pysnptools-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-01 15:08:11.427321 pysnptools-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-02-01 15:07:21.000000 pysnptools-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.415321 pysnptools-0.5.8/pysnptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.419321 pysnptools-0.5.8/pysnptools/distreader/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/_distmergesids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/_snp2dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/bgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/distdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/distgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/disthdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/distmemmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/distnpz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/distreader.py
--rw-r--r--   0 runner    (1001) docker     (123)    30989 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/distreader/test_bgen2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.419321 pysnptools-0.5.8/pysnptools/kernelreader/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/kerneldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/kernelhdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/kernelnpz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/kernelreader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/snpkernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelreader/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.419321 pysnptools-0.5.8/pysnptools/kernelstandardizer/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/kernelstandardizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.419321 pysnptools-0.5.8/pysnptools/pstreader/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/_mergecols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/_mergerows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/_oneshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/pstdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/psthdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/pstmemmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/pstnpz.py
--rw-r--r--   0 runner    (1001) docker     (123)    36719 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/pstreader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/pstreader/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.423321 pysnptools-0.5.8/pysnptools/snpreader/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/_dist2snp.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/_mergeiids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/_mergesids.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/bed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/distributedbed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/ped.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/pheno.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snpdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snpgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snphdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snpmemmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snpnpz.py
--rw-r--r--   0 runner    (1001) docker     (123)    44949 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/snpreader/snpreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.423321 pysnptools-0.5.8/pysnptools/standardizer/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/betatrained.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/bysidcount.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/bysqrtsidcount.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/diag_K_to_N.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/standardizer/unittrained.py
--rw-r--r--   0 runner    (1001) docker     (123)    64624 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.423321 pysnptools-0.5.8/pysnptools/util/
--rw-r--r--   0 runner    (1001) docker     (123)    27140 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/_example_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.427321 pysnptools-0.5.8/pysnptools/util/filecache/
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/filecache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/hashdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/localcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/peertopeer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/filecache/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    69653 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/intrangeset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.427321 pysnptools-0.5.8/pysnptools/util/mapreduce1/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/distributable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/distributabletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/mapreduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.427321 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hadoop.py
--rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hadoop2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24421 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localinparts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localmultiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localmultithread.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/pheno.py
--rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/pysnptools.hashdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-02-01 15:07:21.000000 pysnptools-0.5.8/pysnptools/util/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:08:11.419321 pysnptools-0.5.8/pysnptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-01 15:08:11.000000 pysnptools-0.5.8/pysnptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-02-01 15:08:11.000000 pysnptools-0.5.8/pysnptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 15:08:11.000000 pysnptools-0.5.8/pysnptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-01 15:08:11.000000 pysnptools-0.5.8/pysnptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-01 15:08:11.000000 pysnptools-0.5.8/pysnptools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 15:08:11.427321 pysnptools-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-02-01 15:07:21.000000 pysnptools-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 23:48:58.000000 pysnptools-0.5.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-01 23:48:58.000000 pysnptools-0.5.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 23:48:58.000000 pysnptools-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-01 23:49:51.280926 pysnptools-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-01 23:48:58.000000 pysnptools-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.268926 pysnptools-0.5.9/pysnptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.272926 pysnptools-0.5.9/pysnptools/distreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/_distmergesids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/_snp2dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45574 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/bgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/distdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/distgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/disthdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/distmemmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/distnpz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/distreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-05-01 23:48:58.000000 pysnptools-0.5.9/pysnptools/distreader/test_bgen2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.272926 pysnptools-0.5.9/pysnptools/kernelreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/kerneldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/kernelhdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/kernelnpz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/kernelreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/snpkernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelreader/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.272926 pysnptools-0.5.9/pysnptools/kernelstandardizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/kernelstandardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.276926 pysnptools-0.5.9/pysnptools/pstreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/_mergecols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/_mergerows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/_oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/pstdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/psthdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/pstmemmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/pstnpz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36719 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/pstreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/pstreader/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.276926 pysnptools-0.5.9/pysnptools/snpreader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/_dist2snp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/_mergeiids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/_mergesids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/distributedbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/ped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/pheno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snpdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snpgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snphdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snpmemmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snpnpz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44949 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/snpreader/snpreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.276926 pysnptools-0.5.9/pysnptools/standardizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/betatrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/bysidcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/bysqrtsidcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/diag_K_to_N.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/standardizer/unittrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/pysnptools/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    27140 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/_example_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/pysnptools/util/filecache/
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/filecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/hashdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/localcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/peertopeer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/filecache/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69653 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/intrangeset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/pysnptools/util/mapreduce1/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/distributable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/distributabletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/mapreduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hadoop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hadoop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24421 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localinparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localmultiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localmultithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/pheno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/pysnptools.hashdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-01 23:48:59.000000 pysnptools-0.5.9/pysnptools/util/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.272926 pysnptools-0.5.9/pysnptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-01 23:49:51.000000 pysnptools-0.5.9/pysnptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-01 23:49:51.000000 pysnptools-0.5.9/pysnptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:49:51.000000 pysnptools-0.5.9/pysnptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-01 23:49:51.000000 pysnptools-0.5.9/pysnptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 23:49:51.000000 pysnptools-0.5.9/pysnptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:49:51.280926 pysnptools-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-01 23:48:59.000000 pysnptools-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:51.280926 pysnptools-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 23:48:59.000000 pysnptools-0.5.9/tests/test.py
```

### Comparing `pysnptools-0.5.8/LICENSE.md` & `pysnptools-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/PKG-INFO` & `pysnptools-0.5.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnptools
-Version: 0.5.8
+Version: 0.5.9
 Summary: PySnpTools
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/PySnpTools/issues
 Project-URL: Documentation, http://fastlmm.github.io/PySnpTools
@@ -46,15 +46,16 @@
 * [filecache](https://fastlmm.github.io/PySnpTools/#module-pysnptools.util.filecache):  Read and write files locally or from/to any remote storage.
 
 Install
 -------
 
     pip install pysnptools
 
-    Note: Windows users must use Python 3.7 to 3.9. Python 3.10 is not supported on Windows.
+| Note: On Windows and Python 3.10, BgenReader isn't supported. See
+[bgen-reader-py issue #45](https://github.com/limix/bgen-reader-py/issues/45)
 
 Documentation
 -------------
 
 * [Main Documentation](http://fastlmm.github.io/PySnpTools/) with examples. It includes links to tutorial slides, notebooks, and video.
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
```

### Comparing `pysnptools-0.5.8/README.md` & `pysnptools-0.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 * [filecache](https://fastlmm.github.io/PySnpTools/#module-pysnptools.util.filecache):  Read and write files locally or from/to any remote storage.
 
 Install
 -------
 
     pip install pysnptools
 
-    Note: Windows users must use Python 3.7 to 3.9. Python 3.10 is not supported on Windows.
+| Note: On Windows and Python 3.10, BgenReader isn't supported. See
+[bgen-reader-py issue #45](https://github.com/limix/bgen-reader-py/issues/45)
 
 Documentation
 -------------
 
 * [Main Documentation](http://fastlmm.github.io/PySnpTools/) with examples. It includes links to tutorial slides, notebooks, and video.
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
```

### Comparing `pysnptools-0.5.8/pysnptools/distreader/__init__.py` & `pysnptools-0.5.9/pysnptools/distreader/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/_distmergesids.py` & `pysnptools-0.5.9/pysnptools/distreader/_distmergesids.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/_snp2dist.py` & `pysnptools-0.5.9/pysnptools/distreader/_snp2dist.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/bgen.py` & `pysnptools-0.5.9/pysnptools/distreader/bgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 import logging
 import numpy as np
 import unittest
 from pathlib import Path
 
-from bgen_reader import example_filepath
-from bgen_reader import open_bgen
-from bgen_reader._multimemmap import MultiMemMap
+try:
+    from bgen_reader import example_filepath
+    from bgen_reader import open_bgen
+    from bgen_reader._multimemmap import MultiMemMap
+    _BGEN_AVAILABLE = True
+except ImportError:
+    logging.warning("bgen_reader not installed. Some tests will be skipped.")
+    _BGEN_AVAILABLE = False
 from pysnptools.util import log_in_place
 import shutil
 import math
 import subprocess
 import pysnptools.util as pstutil
 from pysnptools.distreader import DistReader
 from bed_reader import get_num_threads
```

### Comparing `pysnptools-0.5.8/pysnptools/distreader/distdata.py` & `pysnptools-0.5.9/pysnptools/distreader/distdata.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/distgen.py` & `pysnptools-0.5.9/pysnptools/distreader/distgen.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/disthdf5.py` & `pysnptools-0.5.9/pysnptools/distreader/disthdf5.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/distmemmap.py` & `pysnptools-0.5.9/pysnptools/distreader/distmemmap.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/distnpz.py` & `pysnptools-0.5.9/pysnptools/distreader/distnpz.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/distreader.py` & `pysnptools-0.5.9/pysnptools/distreader/distreader.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/distreader/test.py` & `pysnptools-0.5.9/pysnptools/distreader/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 import scipy as sp
 import logging
 import doctest
 import shutil
 import unittest
 import os.path
 import time
+import sys
+
 
 from pysnptools.distreader.distmemmap import TestDistMemMap
-from pysnptools.distreader.bgen import TestBgen
+try:
+    from bgen_reader import open_bgen
+    from pysnptools.distreader.bgen import TestBgen
+    _TEST_BGEN_AVAILABLE = True
+except:
+    logging.warning("BgenReader will not be available")
+    _TEST_BGEN_AVAILABLE = False
 from pysnptools.distreader.distgen import TestDistGen
 from pysnptools.distreader import DistNpz, DistHdf5, DistMemMap, DistData, _DistMergeSIDs
 from pysnptools.util import create_directory_if_necessary
 from pysnptools.snpreader import SnpNpz, Bed
 from pysnptools.kernelreader.test import _fortesting_JustCheckExists
 from pysnptools.pstreader import PstData
 from pysnptools.snpreader import SnpData
@@ -170,21 +178,26 @@
         result5 = result4.read(view_ok=True)
         self.assertTrue(np.may_share_memory(result4.val,result5.val))
 
 
 
 
     def test_writes(self):
-        from pysnptools.distreader import DistData, DistHdf5, DistNpz, DistMemMap, Bgen
+        from pysnptools.distreader import DistData, DistHdf5, DistNpz, DistMemMap
         from pysnptools.kernelreader.test import _fortesting_JustCheckExists
 
         the_class_and_suffix_list = [(DistNpz,"npz",None,None),
-                                     (Bgen,"bgen",None,lambda filename,distdata: Bgen.write(filename,distdata,bits=32)),
+                                     # Bgen used to be here
                                      (DistHdf5,"hdf5",None,None),
                                      (DistMemMap,"memmap",None,None)]
+        # Skip because write requires qctool, which is not installed by default
+        # if _TEST_BGEN_AVAILABLE:
+        #     from pysnptools.distreader import Bgen
+        #     the_class_and_suffix_list.append((Bgen,"bgen",None,lambda filename,distdata: Bgen.write(filename,distdata,bits=32)))
+
         cant_do_col_prop_none_set = {'bgen'}
         cant_do_col_len_0_set = {'bgen'}
         cant_do_row_count_zero_set = {'bgen'}
         can_swap_0_2_set = {}
         can_change_col_names_set = {}
         ignore_fam_id_set = {}
         ignore_pos1_set = {'bgen'}
@@ -370,32 +383,36 @@
         distdata1 = sub.read()
         expected = snpreader.as_dist(max_weight=2)[::2,::2].read()
         np.testing.assert_array_almost_equal(distdata1.val, expected.val, decimal=10)
 
         logging.info("done with test")
 
     def test_respect_read_inputs(self):
-        from pysnptools.distreader import Bgen,DistGen,DistHdf5,DistMemMap,DistNpz
+        from pysnptools.distreader import DistGen,DistHdf5,DistMemMap,DistNpz
+        if _TEST_BGEN_AVAILABLE:
+            from pysnptools.distreader import Bgen
         from pysnptools.snpreader import Bed
 
         previous_wd = os.getcwd()
         os.chdir(os.path.dirname(os.path.realpath(__file__)))
 
-        for distreader in [
-                           _DistMergeSIDs([Bgen('../examples/example.bgen')[:,:5].read(),Bgen('../examples/example.bgen')[:,5:].read()]),
-                           Bed('../examples/toydata.5chrom.bed',count_A1=True).as_dist(block_size=2000),
+        distreader_list = [Bed('../examples/toydata.5chrom.bed',count_A1=True).as_dist(block_size=2000),
                            Bed('../examples/toydata.5chrom.bed',count_A1=True).as_dist(),
-                           Bgen('../examples/example.bgen').read(),
-                           Bgen('../examples/bits1.bgen'),                          
                            DistGen(seed=0,iid_count=500,sid_count=50),
                            DistGen(seed=0,iid_count=500,sid_count=50)[::2,::2],
                            DistHdf5('../examples/toydata.snpmajor.dist.hdf5'),
                            DistMemMap('../examples/tiny.dist.memmap'),
                            DistNpz('../examples/toydata10.dist.npz')
-                          ]:
+                          ]
+        if _TEST_BGEN_AVAILABLE:
+            distreader_list += [_DistMergeSIDs([Bgen('../examples/example.bgen')[:,:5].read(),Bgen('../examples/example.bgen')[:,5:].read()]),
+                                Bgen('../examples/example.bgen').read(),
+                                Bgen('../examples/bits1.bgen')]
+
+        for distreader in distreader_list:
             logging.info(str(distreader))
             for order in ['F','C','A']:
                 for dtype in [np.float32,np.float64]:
                     for force_python_only in [True,False]:
                         for view_ok in [True,False]:
                             val = distreader.read(order=order,dtype=dtype,force_python_only=force_python_only,view_ok=view_ok).val
                             has_right_order = order=="A" or (order=="C" and val.flags["C_CONTIGUOUS"]) or (order=="F" and val.flags["F_CONTIGUOUS"])
@@ -569,15 +586,16 @@
 def getTestSuite():
     """
     set up composite test suite
     """
 
     test_suite = unittest.TestSuite([])
 
-    test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestBgen))
+    if _TEST_BGEN_AVAILABLE:
+        test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestBgen))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistReaderDocStrings))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistGen))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistMemMap))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistReaders))
     test_suite.addTests(TestDistNaNCNC.factory_iterator())
```

### Comparing `pysnptools-0.5.8/pysnptools/distreader/test_bgen2.py` & `pysnptools-0.5.9/pysnptools/distreader/test_bgen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 from shutil import copyfile
 
 import numpy as np
 import pytest
 from numpy import array, array_equal, isnan
 from numpy.testing import assert_allclose, assert_equal
 
-from bgen_reader import open_bgen
-from bgen_reader import example_filepath
-from bgen_reader._environment import BGEN_READER_CACHE_HOME
-from bgen_reader.test.write_random import _write_random
-from bgen_reader.test.test_bgen_reader import nowrite_permission, noread_permission
+try:
+    from bgen_reader import open_bgen
+    from bgen_reader import example_filepath
+    from bgen_reader._environment import BGEN_READER_CACHE_HOME
+    from bgen_reader.test.write_random import _write_random
+    from bgen_reader.test.test_bgen_reader import nowrite_permission, noread_permission
+    _BGEN_AVAILABLE = True
+except ImportError:
+    import logging
+    logging.warning("bgen_reader not installed. Some tests will be skipped.")
+    _BGEN_AVAILABLE = False
 
 
 def example_filepath2(filename):
     filepath = example_filepath(filename)
     metadata2_path = open_bgen._metadata_path_from_filename(filepath,samples_filepath=None)
     if metadata2_path.exists():
         metadata2_path.unlink()
```

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/identity.py` & `pysnptools-0.5.9/pysnptools/kernelreader/identity.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/kerneldata.py` & `pysnptools-0.5.9/pysnptools/kernelreader/kerneldata.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/kernelhdf5.py` & `pysnptools-0.5.9/pysnptools/kernelreader/kernelhdf5.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/kernelnpz.py` & `pysnptools-0.5.9/pysnptools/kernelreader/kernelnpz.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/kernelreader.py` & `pysnptools-0.5.9/pysnptools/kernelreader/kernelreader.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/snpkernel.py` & `pysnptools-0.5.9/pysnptools/kernelreader/snpkernel.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelreader/test.py` & `pysnptools-0.5.9/pysnptools/kernelreader/test.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/kernelstandardizer/__init__.py` & `pysnptools-0.5.9/pysnptools/kernelstandardizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/__init__.py` & `pysnptools-0.5.9/pysnptools/pstreader/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/_mergecols.py` & `pysnptools-0.5.9/pysnptools/pstreader/_mergecols.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/_mergerows.py` & `pysnptools-0.5.9/pysnptools/pstreader/_mergerows.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/_oneshot.py` & `pysnptools-0.5.9/pysnptools/pstreader/_oneshot.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/_subset.py` & `pysnptools-0.5.9/pysnptools/pstreader/_subset.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/pstdata.py` & `pysnptools-0.5.9/pysnptools/pstreader/pstdata.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/psthdf5.py` & `pysnptools-0.5.9/pysnptools/pstreader/psthdf5.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/pstmemmap.py` & `pysnptools-0.5.9/pysnptools/pstreader/pstmemmap.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/pstnpz.py` & `pysnptools-0.5.9/pysnptools/pstreader/pstnpz.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/pstreader.py` & `pysnptools-0.5.9/pysnptools/pstreader/pstreader.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/pstreader/test.py` & `pysnptools-0.5.9/pysnptools/pstreader/test.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/__init__.py` & `pysnptools-0.5.9/pysnptools/snpreader/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/_dist2snp.py` & `pysnptools-0.5.9/pysnptools/snpreader/_dist2snp.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/_mergesids.py` & `pysnptools-0.5.9/pysnptools/snpreader/_mergesids.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/bed.py` & `pysnptools-0.5.9/pysnptools/snpreader/bed.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/dat.py` & `pysnptools-0.5.9/pysnptools/snpreader/dat.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/dense.py` & `pysnptools-0.5.9/pysnptools/snpreader/dense.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/distributedbed.py` & `pysnptools-0.5.9/pysnptools/snpreader/distributedbed.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/pairs.py` & `pysnptools-0.5.9/pysnptools/snpreader/pairs.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/ped.py` & `pysnptools-0.5.9/pysnptools/snpreader/ped.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/pheno.py` & `pysnptools-0.5.9/pysnptools/snpreader/pheno.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snpdata.py` & `pysnptools-0.5.9/pysnptools/snpreader/snpdata.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snpgen.py` & `pysnptools-0.5.9/pysnptools/snpreader/snpgen.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snphdf5.py` & `pysnptools-0.5.9/pysnptools/snpreader/snphdf5.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snpmemmap.py` & `pysnptools-0.5.9/pysnptools/snpreader/snpmemmap.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snpnpz.py` & `pysnptools-0.5.9/pysnptools/snpreader/snpnpz.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/snpreader/snpreader.py` & `pysnptools-0.5.9/pysnptools/snpreader/snpreader.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/__init__.py` & `pysnptools-0.5.9/pysnptools/standardizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/beta.py` & `pysnptools-0.5.9/pysnptools/standardizer/beta.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/betatrained.py` & `pysnptools-0.5.9/pysnptools/standardizer/betatrained.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/diag_K_to_N.py` & `pysnptools-0.5.9/pysnptools/standardizer/diag_K_to_N.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/identity.py` & `pysnptools-0.5.9/pysnptools/standardizer/identity.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/standardizer.py` & `pysnptools-0.5.9/pysnptools/standardizer/standardizer.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/unit.py` & `pysnptools-0.5.9/pysnptools/standardizer/unit.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/standardizer/unittrained.py` & `pysnptools-0.5.9/pysnptools/standardizer/unittrained.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/test.py` & `pysnptools-0.5.9/pysnptools/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pysnptools.snpreader.distributedbed import TestDistributedBed
 from pysnptools.util.generate import TestGenerate
 from pysnptools.util._example_file import TestExampleFile
 from pysnptools.kernelreader.test import _fortesting_JustCheckExists
 from pysnptools.util.intrangeset import TestIntRangeSet
 from pysnptools.util.test import TestUtilTools
 from pysnptools.util.filecache.test import TestFileCache
+from pysnptools.distreader.test import TestDistReaders
 
 import unittest
 import os.path
 import time
 
 
 class TestPySnpTools(unittest.TestCase):
@@ -1546,14 +1547,15 @@
 
 def getTestSuite():
     """
     set up composite test suite
     """
     test_suite = unittest.TestSuite([])
 
+    test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistReaders))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestPySnpTools))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDistributedBed))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestFileCache))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestUtilTools))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestIntRangeSet))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestSnpDocStrings))
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestPstDocStrings))
```

### Comparing `pysnptools-0.5.8/pysnptools/util/__init__.py` & `pysnptools-0.5.9/pysnptools/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/_example_file.py` & `pysnptools-0.5.9/pysnptools/util/_example_file.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/__init__.py` & `pysnptools-0.5.9/pysnptools/util/filecache/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/filecache.py` & `pysnptools-0.5.9/pysnptools/util/filecache/filecache.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/hashdown.py` & `pysnptools-0.5.9/pysnptools/util/filecache/hashdown.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/localcache.py` & `pysnptools-0.5.9/pysnptools/util/filecache/localcache.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/peertopeer.py` & `pysnptools-0.5.9/pysnptools/util/filecache/peertopeer.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/filecache/test.py` & `pysnptools-0.5.9/pysnptools/util/filecache/test.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/generate.py` & `pysnptools-0.5.9/pysnptools/util/generate.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/intrangeset.py` & `pysnptools-0.5.9/pysnptools/util/intrangeset.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/distributable.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/distributable.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/distributabletest.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/distributabletest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pysnptools.util.mapreduce1.runner import *
 import logging
 import unittest
 import io
+import sys
 
 class DistributableTest(object) : #implements IDistributable
     '''
     This is a class for distributing any testing.
     '''
     def __init__(self,test_or_suite,tempdirectory=None):
         self._test_or_suite = test_or_suite
```

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/examples.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/examples.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/mapreduce.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/mapreduce.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/__init__.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hadoop.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hadoop.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hadoop2.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hadoop2.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/hpc.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/hpc.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/local.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/local.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localinparts.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localinparts.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localmultiproc.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localmultiproc.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/mapreduce1/runner/localmultithread.py` & `pysnptools-0.5.9/pysnptools/util/mapreduce1/runner/localmultithread.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/pairs.py` & `pysnptools-0.5.9/pysnptools/util/pairs.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/pheno.py` & `pysnptools-0.5.9/pysnptools/util/pheno.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/pysnptools.hashdown.json` & `pysnptools-0.5.9/pysnptools/util/pysnptools.hashdown.json`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools/util/test.py` & `pysnptools-0.5.9/pysnptools/util/test.py`

 * *Files identical despite different names*

### Comparing `pysnptools-0.5.8/pysnptools.egg-info/PKG-INFO` & `pysnptools-0.5.9/pysnptools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnptools
-Version: 0.5.8
+Version: 0.5.9
 Summary: PySnpTools
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/PySnpTools/issues
 Project-URL: Documentation, http://fastlmm.github.io/PySnpTools
@@ -46,15 +46,16 @@
 * [filecache](https://fastlmm.github.io/PySnpTools/#module-pysnptools.util.filecache):  Read and write files locally or from/to any remote storage.
 
 Install
 -------
 
     pip install pysnptools
 
-    Note: Windows users must use Python 3.7 to 3.9. Python 3.10 is not supported on Windows.
+| Note: On Windows and Python 3.10, BgenReader isn't supported. See
+[bgen-reader-py issue #45](https://github.com/limix/bgen-reader-py/issues/45)
 
 Documentation
 -------------
 
 * [Main Documentation](http://fastlmm.github.io/PySnpTools/) with examples. It includes links to tutorial slides, notebooks, and video.
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
```

### Comparing `pysnptools-0.5.8/pysnptools.egg-info/SOURCES.txt` & `pysnptools-0.5.9/pysnptools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,8 +96,9 @@
 pysnptools/util/mapreduce1/runner/hadoop.py
 pysnptools/util/mapreduce1/runner/hadoop2.py
 pysnptools/util/mapreduce1/runner/hpc.py
 pysnptools/util/mapreduce1/runner/local.py
 pysnptools/util/mapreduce1/runner/localinparts.py
 pysnptools/util/mapreduce1/runner/localmultiproc.py
 pysnptools/util/mapreduce1/runner/localmultithread.py
-pysnptools/util/mapreduce1/runner/runner.py
+pysnptools/util/mapreduce1/runner/runner.py
+tests/test.py
```

### Comparing `pysnptools-0.5.8/setup.py` & `pysnptools-0.5.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import shutil
 from setuptools import setup
 import numpy
 
 # Version number
-version = "0.5.8"
+version = "0.5.9"
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
@@ -18,18 +18,19 @@
     "scipy>=1.1.0",
     "numpy>=1.17.0",
     "pandas>=1.1.1",
     "psutil>=5.6.3",
     "h5py>=2.10.0",
     "cloudpickle>=2.2.0",
     "more-itertools>=8.7.0",
-    "cbgen == 1.0.1; platform_system=='Windows' or python_version=='3.7'",
+    "cbgen == 1.0.1; platform_system!='Windows' and python_version=='3.7'",
+    "cbgen == 1.0.1; platform_system=='Windows' and python_version<'3.10'",
     "cbgen >= 1.0.2; platform_system!='Windows' and python_version!='3.7'",
-    "bgen-reader>=4.0.7",
-    "bed-reader>=0.2.5",
+    "bgen-reader>=4.0.7; platform_system!='Windows' or python_version<'3.10'",
+    "bed-reader>=0.2.33",
 ]
 
 # python setup.py sdist bdist_wininst upload
 setup(
     name="pysnptools",
     version=version,
     description="PySnpTools",
```

