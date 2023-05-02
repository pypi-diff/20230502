# Comparing `tmp/bdsf-1.9.1.tar.gz` & `tmp/bdsf-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bdsf-1.9.1.tar", last modified: Tue Nov 19 12:26:12 2019, max compression
+gzip compressed data, was "dist/bdsf-1.9.2.tar", last modified: Fri Dec  6 10:20:26 2019, max compression
```

## Comparing `bdsf-1.9.1.tar` & `bdsf-1.9.2.tar`

### file list

```diff
@@ -1,83 +1,738 @@
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/src/
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/src/c++/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)      862 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/boost_python.h
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3738 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/c++/Fitter_dn2g.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     1401 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/cbdsm_main.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4878 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/MGFunction.h
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)      195 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/pyndarray.h
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     6337 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/stat.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)      417 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/stat.h
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4485 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/c++/Fitter_dnsg.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    15104 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/MGFunction2.cc
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/src/c++/num_util/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    12833 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/num_util/num_util.cpp
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    10354 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/num_util/num_util.h
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     6671 2019-10-03 08:55:11.000000 bdsf-1.9.1/src/c++/MGFunction1.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     2947 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/c++/Fitter_lmder.cc
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)      381 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/c++/Fitters.h
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/src/fortran/
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)     5279 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/fortran/pytess_roundness.f
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)     1788 2017-05-31 18:40:19.000000 bdsf-1.9.1/src/fortran/pytess_simple.f
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)       38 2019-11-19 12:26:12.000000 bdsf-1.9.1/setup.cfg
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/test/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     6695 2017-05-31 18:40:19.000000 bdsf-1.9.1/test/test.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4358 2017-05-31 18:40:19.000000 bdsf-1.9.1/test/test_watershed.py
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)     6901 2019-10-03 08:55:11.000000 bdsf-1.9.1/setup.py
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/bdsf/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    24999 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/readimage.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    13266 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/shapelets.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    49211 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/psf_vary.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     7345 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/multi_proc.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     6799 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/preprocess.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3257 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/statusbar.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     9400 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/make_residimage.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    28330 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/spectralindex.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4603 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/threshold.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    29388 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/plotresults.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    20582 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/tc.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4331 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/mylogger.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    10785 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/collapse.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    16961 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/islands.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    47046 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/rmsimage.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    99458 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/opts.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    47001 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/interface.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    12587 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/sourcecounts.py
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)    29209 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/pybdsm
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    49286 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/output.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    33988 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/gaul2srl.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    27537 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/_version.py
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/bdsf/nat/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    88775 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/nat/__init__.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     6326 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/shapefit.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     7512 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/image.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    46166 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/gausfit.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    75948 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/functions.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     9386 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/__init__.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     1688 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/cleanup.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    30672 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/polarisation.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    30695 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/wavelet_atrous.py
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)      147 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/const.py
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)    29209 2019-11-19 12:25:13.000000 bdsf-1.9.1/bdsf/pybdsf
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:11.000000 bdsf-1.9.1/natgrid/
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/natgrid/Src/
--rwxrwxr-x   0 dijkema   (7664) dijkema   (7664)    97317 2019-10-03 08:55:11.000000 bdsf-1.9.1/natgrid/Src/natgridmodule.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     4395 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nnuser.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3570 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nnerror.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3510 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/natgridd.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    17856 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nncrunchd.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     1270 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/natgrid.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3931 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nnusers.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     5341 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nnuserd.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    17848 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nncrunchs.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)    32424 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/nncrunch.c
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     3499 2017-05-31 18:40:19.000000 bdsf-1.9.1/natgrid/Src/natgrids.c
-drwxrwxr-x   0 dijkema   (7664) dijkema   (7664)        0 2019-11-19 12:26:12.000000 bdsf-1.9.1/bdsf.egg-info/
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     1416 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/SOURCES.txt
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)        5 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/top_level.txt
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)       47 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/requires.txt
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)        1 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/dependency_links.txt
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     2973 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/PKG-INFO
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)        1 2019-11-19 12:26:11.000000 bdsf-1.9.1/bdsf.egg-info/not-zip-safe
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     2093 2019-10-03 08:55:11.000000 bdsf-1.9.1/README.rst
--rw-rw-r--   0 dijkema   (7664) dijkema   (7664)     2973 2019-11-19 12:26:12.000000 bdsf-1.9.1/PKG-INFO
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:26.000000 bdsf-1.9.2/
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/manylinux2010/
+-rw-r--r--   0 dijkema    (501) staff       (20)     1362 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/wheel35.docker
+-rw-r--r--   0 dijkema    (501) staff       (20)     1363 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/wheel27.docker
+-rw-r--r--   0 dijkema    (501) staff       (20)     1362 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/wheel37.docker
+-rwxr-xr-x   0 dijkema    (501) staff       (20)      257 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/build.sh
+-rw-r--r--   0 dijkema    (501) staff       (20)        6 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/.gitignore
+-rw-r--r--   0 dijkema    (501) staff       (20)     1362 2019-12-06 10:05:52.000000 bdsf-1.9.2/manylinux2010/wheel36.docker
+-rw-r--r--   0 dijkema    (501) staff       (20)     2973 2019-12-06 10:20:26.000000 bdsf-1.9.2/PKG-INFO
+-rw-r--r--   0 dijkema    (501) staff       (20)    35141 2017-03-22 13:48:50.000000 bdsf-1.9.2/LICENSE
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:26.000000 bdsf-1.9.2/test/
+-rw-r--r--   0 dijkema    (501) staff       (20)     1932 2018-06-20 12:21:15.000000 bdsf-1.9.2/test/Ateammodels.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     2153 2017-03-03 18:36:00.000000 bdsf-1.9.2/test/do_stuff.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     4358 2018-06-20 12:21:08.000000 bdsf-1.9.2/test/test_watershed.py
+-rw-r--r--   0 dijkema    (501) staff       (20)  5333760 2017-03-22 13:48:50.000000 bdsf-1.9.2/test/tbdsf_process_image.in_fits
+-rw-r--r--   0 dijkema    (501) staff       (20)     3214 2017-03-03 18:36:00.000000 bdsf-1.9.2/test/colourcorrection.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     6695 2017-03-03 18:36:00.000000 bdsf-1.9.2/test/test.py
+-rw-r--r--   0 dijkema    (501) staff       (20)      558 2017-03-22 13:48:50.000000 bdsf-1.9.2/test/tbdsf_process_image.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     3555 2019-09-25 07:38:04.000000 bdsf-1.9.2/test/tbdsf_process_image.in
+-rwxr-xr-x   0 dijkema    (501) staff       (20)     8129 2019-12-06 10:05:52.000000 bdsf-1.9.2/setup.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     1066 2019-12-06 10:05:52.000000 bdsf-1.9.2/.gitignore
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/natgrid/
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/natgrid/Test/
+-rwxr-xr-x   0 dijkema    (501) staff       (20)    51193 2018-06-20 12:21:08.000000 bdsf-1.9.2/natgrid/Test/test_natgrid.py
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/natgrid/Include/
+-rw-r--r--   0 dijkema    (501) staff       (20)      280 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnexver.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      465 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nntypes.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      560 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nncheads.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     1483 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnuheads.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     1361 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnuhead.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      359 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nngheads.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     2413 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnmhead.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      363 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nngheadd.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     2001 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnchead.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     1542 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnghead.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     1523 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nnuheadd.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      736 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nncheadd.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      245 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Include/nntpvrs.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      404 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/setup.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    23412 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/natgridmodule.doc
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/natgrid/Src/
+-rw-r--r--   0 dijkema    (501) staff       (20)     5341 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nnuserd.c
+-rw-r--r--   0 dijkema    (501) staff       (20)    17848 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nncrunchs.c
+-rw-r--r--   0 dijkema    (501) staff       (20)    32424 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nncrunch.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     1270 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/natgrid.c
+-rwxr-xr-x   0 dijkema    (501) staff       (20)    97317 2019-09-25 07:38:04.000000 bdsf-1.9.2/natgrid/Src/natgridmodule.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     3499 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/natgrids.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     4395 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nnuser.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     3570 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nnerror.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     3510 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/natgridd.c
+-rw-r--r--   0 dijkema    (501) staff       (20)    17856 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nncrunchd.c
+-rw-r--r--   0 dijkema    (501) staff       (20)     3931 2017-03-10 09:38:46.000000 bdsf-1.9.2/natgrid/Src/nnusers.c
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:24.000000 bdsf-1.9.2/bdsf/
+-rw-r--r--   0 dijkema    (501) staff       (20)    30695 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/wavelet_atrous.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    76034 2019-12-03 09:23:58.000000 bdsf-1.9.2/bdsf/functions.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     4331 2018-06-14 20:44:44.000000 bdsf-1.9.2/bdsf/mylogger.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    20582 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/tc.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     3257 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/statusbar.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    16961 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/islands.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    12587 2017-03-15 13:38:07.000000 bdsf-1.9.2/bdsf/sourcecounts.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    27705 2019-12-06 10:05:52.000000 bdsf-1.9.2/bdsf/_version.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     6799 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/preprocess.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     7345 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/multi_proc.py
+-rwxr-xr-x   0 dijkema    (501) staff       (20)    29209 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/pybdsm
+-rw-r--r--   0 dijkema    (501) staff       (20)    49211 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/psf_vary.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    33988 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/gaul2srl.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    25414 2019-12-05 13:32:59.000000 bdsf-1.9.2/bdsf/readimage.py
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:24.000000 bdsf-1.9.2/bdsf/nat/
+-rw-r--r--   0 dijkema    (501) staff       (20)    88775 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/nat/__init__.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    47004 2019-12-03 09:23:58.000000 bdsf-1.9.2/bdsf/interface.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    10785 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/collapse.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     9386 2019-12-03 09:23:58.000000 bdsf-1.9.2/bdsf/__init__.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    13371 2019-12-03 09:23:58.000000 bdsf-1.9.2/bdsf/shapelets.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     1688 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/cleanup.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     4603 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/threshold.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    28330 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/spectralindex.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     9400 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/make_residimage.py
+-rwxr-xr-x   0 dijkema    (501) staff       (20)    29209 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/pybdsf
+-rw-r--r--   0 dijkema    (501) staff       (20)    99458 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/opts.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    30672 2019-12-03 09:23:58.000000 bdsf-1.9.2/bdsf/polarisation.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    47125 2019-12-05 13:32:59.000000 bdsf-1.9.2/bdsf/rmsimage.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    46166 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/gausfit.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     6326 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/shapefit.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    29388 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/plotresults.py
+-rw-r--r--   0 dijkema    (501) staff       (20)     7512 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/image.py
+-rw-r--r--   0 dijkema    (501) staff       (20)      147 2017-03-15 13:38:07.000000 bdsf-1.9.2/bdsf/const.py
+-rw-r--r--   0 dijkema    (501) staff       (20)    49286 2019-09-25 07:38:04.000000 bdsf-1.9.2/bdsf/output.py
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:24.000000 bdsf-1.9.2/doc/
+-rw-r--r--   0 dijkema    (501) staff       (20)     5573 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/Makefile
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/doc/source/
+-rw-r--r--   0 dijkema    (501) staff       (20)    47018 2017-05-30 10:40:12.000000 bdsf-1.9.2/doc/source/pybdsf_manual_dia.png
+-rw-r--r--   0 dijkema    (501) staff       (20)     1500 2017-03-15 13:38:08.000000 bdsf-1.9.2/doc/source/index.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)   909193 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/source/art_fit_def.png
+-rw-r--r--   0 dijkema    (501) staff       (20)   189050 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/art_rms_def.png
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/doc/source/_templates/
+-rw-r--r--   0 dijkema    (501) staff       (20)      837 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/source/_templates/searchbox.html
+-rw-r--r--   0 dijkema    (501) staff       (20)   154507 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/colourcorr_full.png
+-rw-r--r--   0 dijkema    (501) staff       (20)     9136 2019-12-06 10:05:52.000000 bdsf-1.9.2/doc/source/conf.py
+-rw-r--r--   0 dijkema    (501) staff       (20)   152992 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/colourcorr_order1-2.png
+-rw-r--r--   0 dijkema    (501) staff       (20)    17278 2019-09-25 07:38:04.000000 bdsf-1.9.2/doc/source/examples.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)   692148 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/quick_example.png
+-rw-r--r--   0 dijkema    (501) staff       (20)     3894 2019-12-03 09:23:58.000000 bdsf-1.9.2/doc/source/capabilities.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)    41828 2017-05-30 10:40:12.000000 bdsf-1.9.2/doc/source/front_pic.png
+-rw-r--r--   0 dijkema    (501) staff       (20)      441 2019-09-25 07:38:04.000000 bdsf-1.9.2/doc/source/installation.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)     3069 2019-09-25 07:38:04.000000 bdsf-1.9.2/doc/source/context.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)    17438 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/write_catalog.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)   150308 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/colourcorr_delta_spin.png
+-rw-r--r--   0 dijkema    (501) staff       (20)    77475 2019-09-25 07:38:04.000000 bdsf-1.9.2/doc/source/process_image.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)     3710 2019-12-03 09:23:58.000000 bdsf-1.9.2/doc/source/export_image.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)     2475 2019-09-25 07:38:04.000000 bdsf-1.9.2/doc/source/scripting.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)   789424 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/source/HydraA_74MHz_fit.png
+-rw-r--r--   0 dijkema    (501) staff       (20)     4754 2017-03-15 13:38:08.000000 bdsf-1.9.2/doc/source/show_fit.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)   946480 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/pt_src_example.png
+-rw-r--r--   0 dijkema    (501) staff       (20)   895878 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/source/art_fit_alt.png
+-rw-r--r--   0 dijkema    (501) staff       (20)   254440 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/art_rms_alt.png
+-rw-r--r--   0 dijkema    (501) staff       (20)    17264 2019-12-06 10:05:52.000000 bdsf-1.9.2/doc/source/whats_new.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)     5430 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/source/algorithms.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)    11955 2017-05-30 10:40:12.000000 bdsf-1.9.2/doc/source/ug_basics.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)      191 2017-03-03 18:36:00.000000 bdsf-1.9.2/doc/source/parameters.rst
+-rw-r--r--   0 dijkema    (501) staff       (20)     2090 2017-03-03 18:35:59.000000 bdsf-1.9.2/doc/anaamika_overview.doc
+-rw-r--r--   0 dijkema    (501) staff       (20)       38 2019-12-06 10:20:26.000000 bdsf-1.9.2/setup.cfg
+-rw-r--r--   0 dijkema    (501) staff       (20)     2093 2019-12-03 09:23:58.000000 bdsf-1.9.2/README.rst
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:24.000000 bdsf-1.9.2/bdsf.egg-info/
+-rw-r--r--   0 dijkema    (501) staff       (20)     2973 2019-12-06 10:20:20.000000 bdsf-1.9.2/bdsf.egg-info/PKG-INFO
+-rw-r--r--   0 dijkema    (501) staff       (20)        1 2019-12-06 10:20:20.000000 bdsf-1.9.2/bdsf.egg-info/not-zip-safe
+-rw-r--r--   0 dijkema    (501) staff       (20)    14398 2019-12-06 10:20:21.000000 bdsf-1.9.2/bdsf.egg-info/SOURCES.txt
+-rw-r--r--   0 dijkema    (501) staff       (20)       47 2019-12-06 10:20:20.000000 bdsf-1.9.2/bdsf.egg-info/requires.txt
+-rw-r--r--   0 dijkema    (501) staff       (20)        5 2019-12-06 10:20:20.000000 bdsf-1.9.2/bdsf.egg-info/top_level.txt
+-rw-r--r--   0 dijkema    (501) staff       (20)        1 2019-12-06 10:20:20.000000 bdsf-1.9.2/bdsf.egg-info/dependency_links.txt
+-rw-r--r--   0 dijkema    (501) staff       (20)      322 2019-12-06 10:05:52.000000 bdsf-1.9.2/.travis.yml
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:24.000000 bdsf-1.9.2/src/
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/c++/
+-rw-r--r--   0 dijkema    (501) staff       (20)    15104 2019-09-25 07:38:04.000000 bdsf-1.9.2/src/c++/MGFunction2.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)     1401 2019-09-25 07:38:04.000000 bdsf-1.9.2/src/c++/cbdsm_main.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)      195 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/pyndarray.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      417 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/stat.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     2947 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/c++/Fitter_lmder.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)     6337 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/stat.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)      862 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/boost_python.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     3738 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/c++/Fitter_dn2g.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)     4485 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/c++/Fitter_dnsg.cc
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/c++/num_util/
+-rw-r--r--   0 dijkema    (501) staff       (20)    12833 2019-09-25 07:38:04.000000 bdsf-1.9.2/src/c++/num_util/num_util.cpp
+-rw-r--r--   0 dijkema    (501) staff       (20)    10354 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/num_util/num_util.h
+-rw-r--r--   0 dijkema    (501) staff       (20)      381 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/c++/Fitters.h
+-rw-r--r--   0 dijkema    (501) staff       (20)     6671 2019-09-25 07:38:04.000000 bdsf-1.9.2/src/c++/MGFunction1.cc
+-rw-r--r--   0 dijkema    (501) staff       (20)     4878 2018-05-18 07:59:20.000000 bdsf-1.9.2/src/c++/MGFunction.h
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/minpack/
+-rw-r--r--   0 dijkema    (501) staff       (20)     3805 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/rwupdt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2494 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/qform.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4892 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/chkder.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      335 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/CMakeLists.txt_minpack
+-rw-r--r--   0 dijkema    (501) staff       (20)     5303 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/dogleg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4328 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/hybrj1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4950 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/fdjac1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5702 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/r1updt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4204 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/index.html
+-rw-r--r--   0 dijkema    (501) staff       (20)     2246 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/DISCLAIMER
+-rw-r--r--   0 dijkema    (501) staff       (20)     3135 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/enorm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15890 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmstr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3924 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/hybrd1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6178 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/qrsolv.f
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/minpack/ex/
+-rw-r--r--   0 dijkema    (501) staff       (20)    28502 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file18
+-rw-r--r--   0 dijkema    (501) staff       (20)    22981 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file20
+-rw-r--r--   0 dijkema    (501) staff       (20)    23034 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file16
+-rw-r--r--   0 dijkema    (501) staff       (20)    28092 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file11
+-rw-r--r--   0 dijkema    (501) staff       (20)    28051 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file17
+-rw-r--r--   0 dijkema    (501) staff       (20)      368 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file21
+-rw-r--r--   0 dijkema    (501) staff       (20)    19066 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file19
+-rw-r--r--   0 dijkema    (501) staff       (20)     1759 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/index.html
+-rw-r--r--   0 dijkema    (501) staff       (20)     6491 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file04
+-rw-r--r--   0 dijkema    (501) staff       (20)   166066 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file03
+-rw-r--r--   0 dijkema    (501) staff       (20)   154695 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file02
+-rw-r--r--   0 dijkema    (501) staff       (20)   156151 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file05
+-rw-r--r--   0 dijkema    (501) staff       (20)      165 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file23
+-rw-r--r--   0 dijkema    (501) staff       (20)    18795 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file12
+-rw-r--r--   0 dijkema    (501) staff       (20)    14439 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file15
+-rw-r--r--   0 dijkema    (501) staff       (20)    11224 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file14
+-rw-r--r--   0 dijkema    (501) staff       (20)    22669 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file13
+-rw-r--r--   0 dijkema    (501) staff       (20)      609 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file22
+-rw-r--r--   0 dijkema    (501) staff       (20)    11128 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file07
+-rw-r--r--   0 dijkema    (501) staff       (20)    22708 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file09
+-rw-r--r--   0 dijkema    (501) staff       (20)    14225 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file08
+-rw-r--r--   0 dijkema    (501) staff       (20)   167359 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file06
+-rw-r--r--   0 dijkema    (501) staff       (20)     4427 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/ex/file01
+-rw-r--r--   0 dijkema    (501) staff       (20)     3340 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/fdjac2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1001 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/cmake_install.cmake
+-rw-r--r--   0 dijkema    (501) staff       (20)     5593 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmstr1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      773 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/README
+-rw-r--r--   0 dijkema    (501) staff       (20)     5674 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmder1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5417 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/qrfac.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15518 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmder.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8243 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmpar.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15544 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmdif.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2861 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/r1mpyq.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5790 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/dpmpar.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14892 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/hybrd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4467 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/lmdif1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14077 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/minpack/hybrj.f
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/port3/
+-rw-r--r--   0 dijkema    (501) staff       (20)      336 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7swp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2568 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dortra.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    10150 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dnsf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3493 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dzero.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3781 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2603 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dsmnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7870 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16382 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmnhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1111 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7nvr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14123 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmng.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7914 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/itsum.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8396 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4256 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7upd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7391 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6474 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5135 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2gb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      601 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7cpr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    12714 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nsgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9645 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/stkdmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      927 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/cddiv.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      424 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dh2rfa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4237 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7bqn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      540 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/frmati.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    13985 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmnh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5876 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      528 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s2mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5757 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a9rntl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5742 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2f.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      265 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movebd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      688 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rldst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      213 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/eprint.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4958 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmnf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      185 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/iceil.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      646 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/retsrc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3510 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      880 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d4sqr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      949 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7sqr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2714 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dw7zbf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8644 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      119 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/stinit.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4750 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx10.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      277 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i8tsel.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7094 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15116 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dhqr2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5014 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7dgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6836 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7066 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/aprntr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4061 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      253 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movefd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7455 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1960 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkrl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2666 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/w7zbf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      925 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7sqr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5069 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7dgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    34975 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/index.html
+-rw-r--r--   0 dijkema    (501) staff       (20)     2353 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mngb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      294 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i7pnvr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      263 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/sdump.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1536 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d0xtrp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5761 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmnh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7111 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/aprntd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6242 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1358 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkqu.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      229 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movefr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7054 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      910 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd4sqr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      195 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/seti.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4290 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7bqn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      400 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/h2rfa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      321 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/setc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3186 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n7msrt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2865 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7etr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      724 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drldst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6036 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7357 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5852 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2fb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    10341 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nsfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2659 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ortra.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      310 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7swp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5965 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      241 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movebr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2543 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/smnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14948 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rnsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1135 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7nvr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16314 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmnhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7941 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ditsum.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      964 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/entsrc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4304 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7upd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      854 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6728 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3397 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmnf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      613 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7cpr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    21540 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s1mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5652 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mnhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4463 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx10.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1473 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dq7rsh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9272 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s3grd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1113 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7dup.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2365 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l5stp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      685 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkin.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    10330 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drnsgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9403 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drn2gb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6253 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/f7hes.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1128 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s88fmt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1051 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i0tk00.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    17511 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/CHANGES
+-rw-r--r--   0 dijkema    (501) staff       (20)     7667 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      331 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movefc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3102 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1642 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7lup.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7387 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dsm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7587 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      129 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ialloc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      235 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movefi.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7352 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5672 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1648 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7srt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5781 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2f.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      782 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7ivm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1311 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/r7mdc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      189 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/setr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5196 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      723 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkmd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7534 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7dog.f
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:26.000000 bdsf-1.9.2/src/port3/ex/
+-rw-r--r--   0 dijkema    (501) staff       (20)     4165 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nmsk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1467 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbap.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4032 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8107 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      659 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cpla.f
+-rw-r--r--   0 dijkema    (501) staff       (20)       51 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zap.ed
+-rw-r--r--   0 dijkema    (501) staff       (20)      713 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zona.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6725 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7594 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8107 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1002 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntle.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3275 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgeb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6112 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      806 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3374 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      903 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cspa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1390 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgeh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3076 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prs3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)       40 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zap.ex
+-rw-r--r--   0 dijkema    (501) staff       (20)     4251 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      478 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/rnrm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      981 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7073 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1322 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lymk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      821 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgel.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1336 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1783 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgef.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1344 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lyma.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4298 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1404 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cspe.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4986 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx10.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6479 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4986 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dptt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7073 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1201 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2390 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4298 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7706 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    26149 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/index.html
+-rw-r--r--   0 dijkema    (501) staff       (20)     6479 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2016 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbab.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7291 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7706 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1421 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6725 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst8.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1621 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbal.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2553 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbaf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4032 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6273 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7594 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7389 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4714 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pstt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      261 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zap.t
+-rw-r--r--   0 dijkema    (501) staff       (20)     6112 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtgp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1542 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgea.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1082 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4714 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx10.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7904 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3501 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7904 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2717 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/mftg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3353 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11923 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1043 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zonb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1389 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5908 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1802 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6753 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1347 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ftra.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7536 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1168 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qbla.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3580 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1259 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      580 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cdex.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1347 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ffta
+-rw-r--r--   0 dijkema    (501) staff       (20)      927 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsj.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3580 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3003 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lymb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      194 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zap.head
+-rw-r--r--   0 dijkema    (501) staff       (20)     1936 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/llza.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7536 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11527 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1774 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbaa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6753 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1002 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbak.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1770 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4267 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8315 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1651 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1242 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lymp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      858 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/xkt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1852 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lrpg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1362 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prma.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      974 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      824 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/extr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2128 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsj.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2455 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nsnm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      209 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/README
+-rw-r--r--   0 dijkema    (501) staff       (20)     1835 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nsfa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11923 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6489 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3353 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1190 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/errk.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1369 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgej.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1513 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1597 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prs1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      569 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cdlg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4507 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1336 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/np2a.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2051 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2363 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/desa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1540 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/burb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2027 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/mftf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1378 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4507 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4226 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7626 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2321 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1083 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/fmtr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      883 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cspg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1787 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/np2e.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1520 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lbaj.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7626 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4226 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2219 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qpra.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7291 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2603 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lrpb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1386 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/cspq.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2086 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlu.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1535 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/vdsb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2615 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lrpf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      843 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lsfa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6273 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7389 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1934 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2854 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lban.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      853 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/xkhi.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4616 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8600 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dtg4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1144 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ebea.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      858 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/xkth
+-rw-r--r--   0 dijkema    (501) staff       (20)     1130 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/evaa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2751 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7737 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1138 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qblg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2601 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/mfte.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1219 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/bura.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4554 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1559 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/fftc
+-rw-r--r--   0 dijkema    (501) staff       (20)      613 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zera.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3842 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsj.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      800 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/mnna.f
+-rw-r--r--   0 dijkema    (501) staff       (20)       16 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/zip.ed
+-rw-r--r--   0 dijkema    (501) staff       (20)     1573 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/np2b.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7737 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4837 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2060 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/np2f.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      856 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1293 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lgem.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4920 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpt9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      940 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qblc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7330 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/postx7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7167 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pdew.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4837 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1099 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lpsj.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3064 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1468 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lnab.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1559 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ftrc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1835 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsz.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4920 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dpostx9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1575 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ddea.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11527 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2529 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prea.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      967 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3988 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/nlsr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1175 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lrpa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1079 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/vdsa.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1633 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qodd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      944 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ranc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1021 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/mllr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5908 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7330 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8315 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttgrx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3789 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pdea.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3329 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/prsf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1182 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/sdba.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      804 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/xkhd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8600 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/dttgrx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4554 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4616 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/pst9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1112 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/apnr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1353 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/lrpe.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      946 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/qgsp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      658 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/rpad.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1978 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ntlr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1976 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/vdse.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      942 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/splf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6489 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ex/ttg2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7285 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx5.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    21853 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/g7qts.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3343 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx1.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1063 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/frmatd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      343 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movebc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7440 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/df7dhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      675 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/srecap.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16225 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmngb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      953 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7lvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      247 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movebi.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      554 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s3mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1757 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/cmake_install.cmake
+-rw-r--r--   0 dijkema    (501) staff       (20)    10091 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nsf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3373 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mnf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      213 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/setd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7399 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/f7dhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11290 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6516 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      989 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7lvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16298 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmngb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6910 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux1p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      179 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nerror.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5992 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2p.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15464 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rn2g.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1686 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7srt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1063 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/frmatr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5656 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2pb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5157 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1365 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dr7mdc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      818 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7ivm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7584 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7dog.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    21919 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dg7qts.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2325 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/u9dmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      566 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i8save.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1690 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7lup.f
+-rw-r--r--   0 dijkema    (501) staff       (20)       25 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/call.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      223 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i7copy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5733 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mnh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5919 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/aprnti.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1434 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/q7rsh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9332 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds3grd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9699 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i1mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1075 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7dup.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     9339 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rn2gb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    10263 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rnsgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7785 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/aprntc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2782 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/README
+-rw-r--r--   0 dijkema    (501) staff       (20)    11686 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx6.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6252 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6287 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/df7hes.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3458 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/divset.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2792 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dq7apl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      626 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7ipr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2981 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/deigen.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      256 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7scl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      249 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v2axy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      676 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7tvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      247 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movebl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2198 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2lrd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6506 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a9rntd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      741 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7mlp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      763 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7dmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      744 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7vml.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      206 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7scp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7948 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2950 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i0tk01.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4270 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      134 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/erroff.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      224 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7cpy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3975 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5692 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmnhb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7888 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2g.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      147 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/c6lcf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      235 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/movefl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3230 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7msb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4362 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dxtrap.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      757 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/do7prd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7733 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      873 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7tsq.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3194 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7dfl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    12954 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16464 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7mst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      854 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dh2rfg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1441 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v2nrm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1119 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2rdp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4190 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dq7rad.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2326 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/leave.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3156 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7dfl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      794 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/h2rfg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    16387 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7mst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5775 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/aprntl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1501 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv2nrm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7389 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      178 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/iflr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4124 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/q7rad.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1107 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2rdp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    26454 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mng.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      211 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7cpy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      160 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dc6lcf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7319 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/m7slo.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      731 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/o7prd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3282 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7msb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4300 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/xtrap.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      897 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7tsq.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      115 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/mtstak.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      799 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7dmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      718 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7vml.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      194 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7scp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4152 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7egr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6463 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a9rntr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5012 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/m7seq.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4026 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/istkgt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7152 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3442 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ivset.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2766 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/q7apl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      602 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7ipr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15535 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drn2g.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      268 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7scl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      262 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv2axy.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2960 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/eigen.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      700 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7tvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5683 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2pb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      777 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7mlp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2259 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2lrd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2835 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/e9rint.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4365 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3228 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dorthe.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1018 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7tpr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4919 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmnf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1856 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7upd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6200 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/q7rfh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8041 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgux4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    25126 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dg7lit.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7500 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      644 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7prm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      116 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/fdump.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1329 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dc7vfn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3546 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmnfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2284 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/g7qsb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4303 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    12982 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dnsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    21061 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a7sst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14234 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/hqr2.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7856 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2g.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      343 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7shf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2550 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/n2cvp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3370 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/zero.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      800 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/stopx.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    11986 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/parck.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1500 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a0xtrp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      711 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dr7tvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7172 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a9rntc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)       95 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dalloc.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5167 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2gb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    12742 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dnsgb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      390 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7vmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    14196 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drmng.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    28687 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/g7itb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5698 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/a9rnti.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5161 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7svx.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1876 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7ipr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7079 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/postx7.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      871 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7itv.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4600 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx3.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5756 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7svn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1268 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/enter.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7861 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/r1mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    13915 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/rmnh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     4683 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dpostx9.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7464 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7grd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8318 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgux4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      847 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7itv.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2838 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/seterr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5695 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/l7svn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7524 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7grd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5891 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2fb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    10400 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dnsfb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     7646 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d1mach.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    15019 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/drnsg.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8308 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i7do.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    12031 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dparck.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      675 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/r7tvm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      195 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/setl.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8078 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ttgrx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      402 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dv7vmp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    28772 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dg7itb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     5223 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dl7svx.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1900 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/ds7ipr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     8363 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dttgrx4.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    21107 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/da7sst.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      319 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7shf.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2392 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmngb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3544 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/s7rtdt.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1201 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/CMakeLists.txt_port3
+-rw-r--r--   0 dijkema    (501) staff       (20)      359 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i10wid.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2574 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dn2cvp.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    26492 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dmng.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      970 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/d7tpr.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     3305 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/orthe.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      115 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/nirall.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     6265 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dq7rfh.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1906 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dd7upd.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      668 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i7shft.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      618 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/v7prm.f
+-rw-r--r--   0 dijkema    (501) staff       (20)    25028 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/g7lit.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     2335 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/dg7qsb.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1305 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/c7vfn.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      824 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/port3/i7mdcn.f
+drwxr-xr-x   0 dijkema    (501) staff       (20)        0 2019-12-06 10:20:25.000000 bdsf-1.9.2/src/fortran/
+-rw-r--r--   0 dijkema    (501) staff       (20)     1332 2017-03-03 18:36:00.000000 bdsf-1.9.2/src/fortran/gaul2gaulbin.f
+-rw-r--r--   0 dijkema    (501) staff       (20)     1520 2017-03-07 11:01:46.000000 bdsf-1.9.2/src/fortran/Makefile
+-rwxr-xr-x   0 dijkema    (501) staff       (20)     1788 2017-03-07 11:01:50.000000 bdsf-1.9.2/src/fortran/pytess_simple.f
+-rwxr-xr-x   0 dijkema    (501) staff       (20)     5279 2017-03-07 11:01:50.000000 bdsf-1.9.2/src/fortran/pytess_roundness.f
+-rw-r--r--   0 dijkema    (501) staff       (20)      302 2017-05-30 10:40:12.000000 bdsf-1.9.2/src/fortran/constants.inc
```

### Comparing `bdsf-1.9.1/src/c++/boost_python.h` & `bdsf-1.9.2/src/c++/boost_python.h`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/Fitter_dn2g.cc` & `bdsf-1.9.2/src/c++/Fitter_dn2g.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/cbdsm_main.cc` & `bdsf-1.9.2/src/c++/cbdsm_main.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/MGFunction.h` & `bdsf-1.9.2/src/c++/MGFunction.h`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/stat.cc` & `bdsf-1.9.2/src/c++/stat.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/Fitter_dnsg.cc` & `bdsf-1.9.2/src/c++/Fitter_dnsg.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/MGFunction2.cc` & `bdsf-1.9.2/src/c++/MGFunction2.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/num_util/num_util.cpp` & `bdsf-1.9.2/src/c++/num_util/num_util.cpp`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/num_util/num_util.h` & `bdsf-1.9.2/src/c++/num_util/num_util.h`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/MGFunction1.cc` & `bdsf-1.9.2/src/c++/MGFunction1.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/c++/Fitter_lmder.cc` & `bdsf-1.9.2/src/c++/Fitter_lmder.cc`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/fortran/pytess_roundness.f` & `bdsf-1.9.2/src/fortran/pytess_roundness.f`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/src/fortran/pytess_simple.f` & `bdsf-1.9.2/src/fortran/pytess_simple.f`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/test/test.py` & `bdsf-1.9.2/test/test.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/test/test_watershed.py` & `bdsf-1.9.2/test/test_watershed.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/setup.py` & `bdsf-1.9.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,27 @@
 from os.path import join, realpath, dirname
 import subprocess
 import glob
 import distutils.cmd
 import distutils.log
 from numpy.distutils.command.build_ext import build_ext as numpy_build_ext
 from distutils.command.clean import clean as distutils_clean
+from distutils import ccompiler
+import os
+import warnings
 
 
+no_boost_error = """
+Could not find a Python boost library! Please use your package manager to install boost.
+
+Or install it manually:
+
+http://boostorg.github.io/python/doc/html/index.html
+"""
+
 minpack_src = ["lmder.f", "lmpar.f", "qrfac.f", "qrsolv.f", "enorm.f", "dpmpar.f"]
 port3_src = ["dnsg.f", "dn2g.f", "drnsg.f", "drn2g.f", "d1mach.f", "da7sst.f",
              "dc7vfn.f", "dd7tpr.f", "dd7upd.f", "df7hes.f", "dg7lit.f", "dg7qts.f",
              "ditsum.f", "divset.f", "dl7itv.f", "dl7ivm.f", "dl7mst.f", "dl7nvr.f",
              "dl7sqr.f", "dl7srt.f", "dl7svn.f", "dl7svx.f", "dl7tsq.f", "dl7tvm.f",
              "dl7vml.f", "dn2cvp.f", "dn2lrd.f", "dn2rdp.f", "do7prd.f", "dparck.f",
              "dq7apl.f", "dq7rad.f", "dq7rfh.f", "dr7mdc.f", "drldst.f", "ds7cpr.f",
@@ -86,83 +97,88 @@
 class Clean(distutils_clean):
     """Custom clean command that calls mclean to clean static libs"""
 
     def run(self):
         self.run_command("mclean")
         distutils_clean.run(self)
 
-
-def find_boost():
-    # Find correct boost-python library.
-    system = platform.system()
-    if system == 'Linux':
-        # Use version suffix if present
-        boost_python = 'boost_python-py%s%s' % (sys.version_info[0], sys.version_info[1])
-        if not find_library(boost_python):
-            boost_python = "boost_python"
-    elif system == 'Darwin':
-        if sys.version_info[0] == 2:
-            boost_python = "boost_python-mt"
-        else:
-            boost_python = "boost_python3-mt"
-    return boost_python
-
+def find_library_file(libname):
+    """
+    Try to get the directory of the specified library.
+    It adds to the search path the library paths given to distutil's build_ext.
+    """
+    # Use a dummy argument parser to get user specified library dirs
+    lib_dirs = [os.path.join(sys.prefix, 'lib'),
+                             '/usr/local/lib',
+                             '/usr/lib64',
+                             '/usr/lib',
+                             '/usr/lib/x86_64-linux-gnu']
+
+    if 'LD_LIBRARY_PATH' in os.environ:
+        lib_dirs += os.environ['LD_LIBRARY_PATH'].split(':')
+
+    compiler = ccompiler.new_compiler()
+    return compiler.find_library_file(lib_dirs, libname)
+
+
+def find_boost_python():
+    """Find the name of the boost-python library. Returns None if none is found."""
+    short_version = "{}{}".format(sys.version_info[0], sys.version_info[1])
+    boostlibnames = ['boost_python-py' + short_version,
+                     'boost_python' + short_version,
+                     'boost_python',
+                     ]
+    # The -mt (multithread) extension is used on macOS but not Linux.
+    # Look for it first to avoid ending up with a single-threaded version.
+    boostlibnames = [name + '-mt' for name in boostlibnames] + boostlibnames
+    for libboostname in boostlibnames:
+        if find_library_file(libboostname):
+            return libboostname
+    warnings.warn(no_boost_error)
+    return boostlibnames[0]
 
 def find_boost_numpy():
-    # Find correct boost-python library.
-    system = platform.system()
-    major = sys.version_info.major
-    minor = sys.version_info.minor
-
-    if system == 'Linux':
-        # Use version suffix if present
-        if major == 3:
-            boost_numpy = 'boost_numpy3-py%s%s' % (major, minor)
-        else:
-            boost_numpy = 'boost_numpy-py%s%s' % (major, minor)
-
-        if not find_library(boost_numpy):
-            return None
-        return boost_numpy
-
-    elif system == 'Darwin':
-        if sys.version_info[0] == 2:
-            boost_numpy = "boost_numpy-mt"
-        else:
-            boost_numpy = "boost_numpy3-mt"
-
-        if not find_library(boost_numpy):
-            return None
-        return boost_numpy
+    """Find the name of the boost-numpy library. Returns None if none is found."""
+    short_version = "{}{}".format(sys.version_info[0], sys.version_info[1])
+    boostlibnames = ['boost_numpy-py' + short_version,
+                     'boost_numpy' + short_version,
+                     'boost_numpy',
+                     ]
+    # The -mt (multithread) extension is used on macOS but not Linux.
+    # Look for it first to avoid ending up with a single-threaded version.
+    boostlibnames = [name + '-mt' for name in boostlibnames] + boostlibnames
+    for libboostname in boostlibnames:
+        if find_library_file(libboostname):
+            return libboostname
 
+    warnings.warn("No library boost_numpy found (this may be no problem)")
+    return None
 
-def main():
 
-    boost_python = find_boost()
+def main():
+    boost_python_libname = find_boost_python()
+    boost_numpy_libname = find_boost_numpy()
 
     extensions = []
 
     fext = Extension(
         name="bdsf._pytesselate",
         sources=[
             "src/fortran/pytess_simple.f",
             "src/fortran/pytess_roundness.f"
         ]
     )
     fext.f2py_options = [""]
     extensions.append(fext)
 
     libraries = [
-        'minpack', 'port3', 'gfortran',
-        boost_python,
+        'minpack', 'port3', 'gfortran', boost_python_libname
     ]
-
-    boost_numpy = find_boost_numpy()
-    if boost_numpy is not None:
-        libraries.append(boost_numpy)
+    if boost_numpy_libname is not None:
+        libraries.append(boost_numpy_libname)
 
     extensions.append(Extension(
         name="bdsf._cbdsm",
         sources=[
             "src/c++/Fitter_dn2g.cc",
             "src/c++/Fitter_dnsg.cc",
             "src/c++/Fitter_lmder.cc",
@@ -186,15 +202,15 @@
     # HACK for supporting older versions of NumPy
     for ext in extensions:
         ext.extra_f77_compile_args = []
         ext.extra_f90_compile_args = []
 
     setup(
         name='bdsf',
-        version='1.9.1',
+        version='1.9.2',
         author='David Rafferty',
         author_email='drafferty@hs.uni-hamburg.de',
         url='https://github.com/lofar-astron/PyBDSF',
         description='Blob Detection and Source Finder',
         long_description=open('README.rst', 'rt').read(),
         platforms='Linux, Mac OS X',
         packages=['bdsf', 'bdsf.nat'],
```

### Comparing `bdsf-1.9.1/bdsf/readimage.py` & `bdsf-1.9.2/bdsf/readimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,15 +441,24 @@
         elif img.opts.frequency is not None and img.image_arr.shape[1] == 1:
             img.frequency = img.opts.frequency
             img.freq_pars = (img.frequency, 0.0, 0.0)
             mylog.info('Using user-specified frequency.')
         else:
             spec_indx = img.wcs_obj.wcs.spec
             if spec_indx == -1:
-                raise RuntimeError('No frequency information found in image header.')
+                # No frequency axis; check header instead
+                hdr = img.header
+                if 'RESTFREQ' in hdr:
+                    img.frequency = hdr['RESTFREQ']
+                    img.freq_pars = (img.frequency, 0.0, 0.0)
+                elif 'FREQ' in hdr:
+                    img.frequency = hdr['FREQ']
+                    img.freq_pars = (img.frequency, 0.0, 0.0)
+                else:
+                    raise RuntimeError('No frequency information found in image header.')
             else:
                 # Here we define p2f and f2p to allow pixel to frequency
                 # transformations. Transformations for other axes (e.g.,
                 # celestial) are striped out.
                 #
                 # First, convert frequency to Hz if needed:
                 img.wcs_obj.wcs.sptr('FREQ-???')
```

### Comparing `bdsf-1.9.1/bdsf/shapelets.py` & `bdsf-1.9.2/bdsf/shapelets.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,18 @@
     from math import sqrt,pi
     try:
         from scipy import factorial
     except ImportError:
         try:
             from scipy.misc.common import factorial
         except ImportError:
-            from scipy.misc import factorial
+            try:
+                from scipy.misc import factorial
+            except ImportError:
+                from scipy.special import factorial
 
     hcx = hc[nx,:]
     hcy = hc[ny,:]
     ind = N.array([nx,ny])
     fact = factorial(ind)
     dumr1 = N.sqrt((2.0**(ind))*sqrt(pi)*fact)
```

### Comparing `bdsf-1.9.1/bdsf/psf_vary.py` & `bdsf-1.9.2/bdsf/psf_vary.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/multi_proc.py` & `bdsf-1.9.2/bdsf/multi_proc.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/preprocess.py` & `bdsf-1.9.2/bdsf/preprocess.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/statusbar.py` & `bdsf-1.9.2/bdsf/statusbar.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/make_residimage.py` & `bdsf-1.9.2/bdsf/make_residimage.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/spectralindex.py` & `bdsf-1.9.2/bdsf/spectralindex.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/threshold.py` & `bdsf-1.9.2/bdsf/threshold.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/plotresults.py` & `bdsf-1.9.2/bdsf/plotresults.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/tc.py` & `bdsf-1.9.2/bdsf/tc.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/mylogger.py` & `bdsf-1.9.2/bdsf/mylogger.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/collapse.py` & `bdsf-1.9.2/bdsf/collapse.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/islands.py` & `bdsf-1.9.2/bdsf/islands.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/rmsimage.py` & `bdsf-1.9.2/bdsf/rmsimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,14 +452,15 @@
                        logname=None, ncores=None):
         """Calls map_2d and checks for problems"""
         mylog = mylogger.logging.getLogger("PyBDSM."+img.log+"Rmsimage.Calcmaps ")
         rms_ok = False
         mylog = mylogger.logging.getLogger("PyBDSM."+img.log+"Rmsimage.Calcmaps ")
         opts = img.opts
         kappa = map_opts[0]
+        spline_rank = opts.spline_rank
         while not rms_ok:
             self.map_2d(data, mean, rms, mask, *map_opts, do_adapt=do_adapt,
                         bright_pt_coords=bright_pt_coords, rms_box2=rms_box2,
                         logname=logname, ncores=ncores)
             if img.masked:
                 test = N.any(rms[~img.mask_arr] < 0.0)
             else:
@@ -478,39 +479,40 @@
                             mylogger.userinfo(mylog, 'Size of rms_box_bright larger than 1/4 of image size')
                             mylogger.userinfo(mylog, 'Using constant background rms and mean')
                             img.use_rms_map = False
                             img.rms_box = img.rms_box_bright
                             img.mean_map_type = 'const'
                             rms_ok = True
                         else:
-                            map_opts = (kappa, img.rms_box_bright, opts.spline_rank)
+                            map_opts = (kappa, img.rms_box_bright, spline_rank)
                     else:
                         new_width = int(img.rms_box[0]*1.2)
                         if new_width == img.rms_box[0]:
                             new_width = img.rms_box[0] + 1
                         new_step = int(new_width/3.0)
                         img.rms_box = (new_width, new_step)
                         if img.rms_box[0] > min(img.ch0_arr.shape)/4.0:
                             mylogger.userinfo(mylog, 'Size of rms_box larger than 1/4 of image size')
                             mylogger.userinfo(mylog, 'Using constant background rms and mean')
                             img.use_rms_map = False
                             img.mean_map_type = 'const'
                             rms_ok = True
                         else:
-                            map_opts = (kappa, img.rms_box, opts.spline_rank)
+                            map_opts = (kappa, img.rms_box, spline_rank)
 
                 else:
                     # User has specified box size, use order=1 to prevent negatives
-                    if opts.spline_rank > 1:
-                        mylog.warning('Negative values found in rms map interpolated with spline_rank = %i' % opts.spline_rank)
+                    if spline_rank > 1:
+                        mylog.warning('Negative values found in rms map interpolated with spline_rank = %i' % spline_rank)
                         mylog.warning('Using spline_rank = 1 (bilinear interpolation) instead')
+                        spline_rank = 1
                         if do_adapt:
-                            map_opts = (kappa, img.rms_box_bright, 1)
+                            map_opts = (kappa, img.rms_box_bright, spline_rank)
                         else:
-                            map_opts = (kappa, img.rms_box, 1)
+                            map_opts = (kappa, img.rms_box, spline_rank)
                     else:
                         raise RuntimeError('RMS map has negative values')
             else:
                 rms_ok = True
 
         return mean, rms
```

### Comparing `bdsf-1.9.1/bdsf/opts.py` & `bdsf-1.9.2/bdsf/opts.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/interface.py` & `bdsf-1.9.2/bdsf/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,15 +908,15 @@
             print("\n\033[91mERROR\033[0m: img_type not recognized.")
             return False
         if filename == 'SAMP':
             print('--> Image sent to SMAP hub')
         else:
             print('--> Wrote file ' + repr(filename))
             if use_io == 'rap':
-                # remove the temporary fits file used as a pyrap template
+                # remove the temporary fits file used as a casacore template
                 import os
                 os.remove(filename+'.fits')
 
         return True
     except RuntimeError as err:
         # Catch and log error
         mylog.error(str(err))
```

### Comparing `bdsf-1.9.1/bdsf/sourcecounts.py` & `bdsf-1.9.2/bdsf/sourcecounts.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/pybdsm` & `bdsf-1.9.2/bdsf/pybdsm`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/output.py` & `bdsf-1.9.2/bdsf/output.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/gaul2srl.py` & `bdsf-1.9.2/bdsf/gaul2srl.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/_version.py` & `bdsf-1.9.2/bdsf/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Version module.
 
 This module simply stores the version number, as well as a changelog.
 """
 
 # Version number
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 
 
 # Changelog
 def changelog():
     """
     PyBDSF Changelog.
     -----------------------------------------------------------------------
+    2019/12/05 - Version 1.9.2
+
+    2019/12/04 - Fix exception behaviour if spline order change does not work
+
+    2019/09/27 - Add check for frequency info in header
+
     2019/09/25 - Version 1.9.1
 
     2019/09/25 - Fix various minor bugs
 
     2019/06/06 - Fix blank_limit check_low error (#100)
 
     2019/05/09 - Fix various shapelet decomposition issues
```

### Comparing `bdsf-1.9.1/bdsf/nat/__init__.py` & `bdsf-1.9.2/bdsf/nat/__init__.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/shapefit.py` & `bdsf-1.9.2/bdsf/shapefit.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/image.py` & `bdsf-1.9.2/bdsf/image.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/gausfit.py` & `bdsf-1.9.2/bdsf/gausfit.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/functions.py` & `bdsf-1.9.2/bdsf/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,18 +1056,18 @@
       obj = default
 
     return obj
 
 def read_image_from_file(filename, img, indir, quiet=False):
     """ Reads data and header from indir/filename.
 
-    We can use either pyfits or pyrap depending on the value
+    We can use either pyfits or python-casacore depending on the value
     of img.use_io = 'fits'/'rap'
 
-    PyFITS is required, as it is used to standardize the header format. pyrap
+    PyFITS is required, as it is used to standardize the header format. python-casacore
     is optional.
     """
     from . import mylogger
     import os
     import numpy as N
     from copy import deepcopy as cp
     from distutils.version import StrictVersion
@@ -1107,22 +1107,22 @@
                     fits = pyfits.open(image_file, mode="readonly", ignore_missing_end=True)
                 else:
                     fits = pyfits.open(image_file, mode="readonly")
             except IOError as err:
                 img._reason = 'Problem reading file.\nOriginal error: {0}'.format(str(err))
                 return None
         if img.use_io == 'rap':
-            import pyrap.images as pim
+            import casacore.images as pim
             try:
                 inputimage = pim.image(image_file)
             except IOError as err:
                 img._reason = 'Problem reading file.\nOriginal error: {0}'.format(str(err))
                 return None
     else:
-        # Simple check of whether pyrap and pyfits are available
+        # Simple check of whether casacore and pyfits are available
         # We need pyfits version 2.2 or greater to use the
         # "ignore_missing_end" argument to pyfits.open().
         try:
             try:
                 from astropy.io import fits as pyfits
                 old_pyfits = False
                 use_sections = True
@@ -1137,55 +1137,55 @@
                 else:
                     old_pyfits = False
                     use_sections = True
             has_pyfits = True
         except ImportError as err:
             raise RuntimeError("Astropy or PyFITS is required.")
         try:
-            import pyrap.images as pim
-            has_pyrap = True
+            import casacore.images as pim
+            has_casacore = True
         except ImportError as err:
-            has_pyrap = False
-            e_pyrap = str(err)
+            has_casacore = False
+            e_casacore = str(err)
 
         # First assume image is a fits file, and use pyfits to open it (if
-        # available). If that fails, try to use pyrap if available.
+        # available). If that fails, try to use casacore if available.
         failed_read = False
         reason = 0
         try:
             if not old_pyfits:
                 fits = pyfits.open(image_file, mode="readonly", ignore_missing_end=True)
             else:
                 fits = pyfits.open(image_file, mode="readonly")
             img.use_io = 'fits'
         except IOError as err:
             e_pyfits = str(err)
-            if has_pyrap:
+            if has_casacore:
                 try:
                     inputimage = pim.image(image_file)
                     img.use_io = 'rap'
                 except IOError as err:
-                    e_pyrap = str(err)
+                    e_casacore = str(err)
                     failed_read = True
                     img._reason = 'File is not a valid FITS, CASA, or HDF5 image.'
             else:
                 failed_read = True
-                e_pyrap = "Pyrap unavailable"
+                e_casacore = "Casacore unavailable"
                 img._reason = 'Problem reading file.'
         if failed_read:
-            img._reason += '\nOriginal error: {0}\n {1}'.format(e_pyfits, e_pyrap)
+            img._reason += '\nOriginal error: {0}\n {1}'.format(e_pyfits, e_casacore)
             return None
 
     # Now that image has been read in successfully, get header (data is loaded
     # later to take advantage of sectioning if trim_box is specified).
     if not quiet:
         mylogger.userinfo(mylog, "Opened '"+image_file+"'")
     if img.use_io == 'rap':
         tmpdir = img.parentname+'_tmp'
-        hdr = convert_pyrap_header(inputimage, tmpdir)
+        hdr = convert_casacore_header(inputimage, tmpdir)
         coords = inputimage.coordinates()
         img.coords_dict = coords.dict()
         if 'telescope' in img.coords_dict:
             img._telescope = img.coords_dict['telescope']
         else:
             img._telescope = None
     if img.use_io == 'fits':
@@ -1195,15 +1195,15 @@
             img._telescope = hdr['TELESCOP']
         else:
             img._telescope = None
 
     # Make sure data is in proper order. Final order is [pol, chan, x (RA), y (DEC)],
     # so we need to rearrange dimensions if they are not in this order. Use the
     # ctype FITS keywords to determine order of dimensions. Note that both PyFITS
-    # and pyrap reverse the order of the axes relative to NAXIS, so we must too.
+    # and casacore reverse the order of the axes relative to NAXIS, so we must too.
     naxis = hdr['NAXIS']
     data_shape = []
     for i in range(naxis):
         data_shape.append(hdr['NAXIS'+str(i+1)])
     data_shape.reverse()
     data_shape = tuple(data_shape)
     mylog.info("Original data shape of " + image_file +': ' +str(data_shape))
@@ -1251,15 +1251,15 @@
                 from pywcs import WCS
                 t = WCS(hdr)
                 t.wcs.fix()
         spec_indx = t.wcs.spec
         if spec_indx != -1:
             ctype_in[spec_indx] = 'FREQ'
 
-    # Now reverse the axes order to match PyFITS/pyrap order and define the
+    # Now reverse the axes order to match PyFITS/casacore order and define the
     # final desired order (cytpe_out) and shape (shape_out).
     ctype_in.reverse()
     if lat_lon:
         ctype_out = ['STOKES', 'FREQ', 'GLON', 'GLAT']
     else:
         ctype_out = ['STOKES', 'FREQ', 'RA', 'DEC']
     indx_out = [-1, -1, -1, -1]
@@ -1319,15 +1319,15 @@
             data.shape = data.shape[0:4] # trim unused dimensions (if any)
             if naxis > 4 or not use_sections:
                 data = data.reshape(shape_out_untrimmed) # Add axes if needed
                 data = data[:, :, xmin:xmax, ymin:ymax] # trim to trim_box
             else:
                 data = data.reshape(shape_out) # Add axes if needed
         else:
-            # With pyrap, just read in the whole image and then trim
+            # With casacore, just read in the whole image and then trim
             data = inputimage.getdata()
             data = data.transpose(*indx_out) # transpose axes to final order
             data.shape = data.shape[0:4] # trim unused dimensions (if any)
             data = data.reshape(shape_out_untrimmed) # Add axes if needed
             data = data[:, :, xmin:xmax, ymin:ymax] # trim to trim_box
 
         # Adjust WCS keywords for trim_box starting x and y.
@@ -1349,29 +1349,29 @@
     ### and make a copy of it to get proper layout & byteorder
     data = N.array(data, order='C',
                    dtype=data.dtype.newbyteorder('='))
 
     return data, hdr
 
 
-def convert_pyrap_header(pyrap_image, tmpdir):
-    """Converts a pyrap header to a PyFITS header."""
+def convert_casacore_header(casacore_image, tmpdir):
+    """Converts a casacore header to a PyFITS header."""
     import tempfile
     import os
     import atexit
     import shutil
     try:
         from astropy.io import fits as pyfits
     except ImportError as err:
         import pyfits
 
     if not os.path.exists(tmpdir):
         os.makedirs(tmpdir)
     tfile = tempfile.NamedTemporaryFile(delete=False, dir=tmpdir)
-    pyrap_image.tofits(tfile.name)
+    casacore_image.tofits(tfile.name)
     hdr = pyfits.getheader(tfile.name)
     if os.path.isfile(tfile.name):
         os.remove(tfile.name)
 
     # Register deletion of temp directory at exit to be sure it is deleted
     atexit.register(shutil.rmtree, tmpdir, ignore_errors=True)
 
@@ -1454,16 +1454,16 @@
             # if it doesn't work
             temp_im.writeto(outfile,  clobber=clobber)
         temp_im.close()
 
         if use == 'rap':
             # For CASA images, read in FITS image and convert
             try:
-                import pyrap.images as pim
-                import pyrap.tables as pt
+                import casacore.images as pim
+                import casacore.tables as pt
                 import os
                 outimage = pim.image(outfile)
                 outimage.saveas(outdir+filename, overwrite=clobber)
 
                 # For masks, use the coordinates dictionary from the input
                 # image, as this is needed in order for the
                 # image to work as a clean mask in CASA.
```

### Comparing `bdsf-1.9.1/bdsf/__init__.py` & `bdsf-1.9.2/bdsf/__init__.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/cleanup.py` & `bdsf-1.9.2/bdsf/cleanup.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/polarisation.py` & `bdsf-1.9.2/bdsf/polarisation.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/wavelet_atrous.py` & `bdsf-1.9.2/bdsf/wavelet_atrous.py`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf/pybdsf` & `bdsf-1.9.2/bdsf/pybdsf`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/natgridmodule.c` & `bdsf-1.9.2/natgrid/Src/natgridmodule.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nnuser.c` & `bdsf-1.9.2/natgrid/Src/nnuser.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nnerror.c` & `bdsf-1.9.2/natgrid/Src/nnerror.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/natgridd.c` & `bdsf-1.9.2/natgrid/Src/natgridd.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nncrunchd.c` & `bdsf-1.9.2/natgrid/Src/nncrunchd.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/natgrid.c` & `bdsf-1.9.2/natgrid/Src/natgrid.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nnusers.c` & `bdsf-1.9.2/natgrid/Src/nnusers.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nnuserd.c` & `bdsf-1.9.2/natgrid/Src/nnuserd.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nncrunchs.c` & `bdsf-1.9.2/natgrid/Src/nncrunchs.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/nncrunch.c` & `bdsf-1.9.2/natgrid/Src/nncrunch.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/natgrid/Src/natgrids.c` & `bdsf-1.9.2/natgrid/Src/natgrids.c`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/bdsf.egg-info/PKG-INFO` & `bdsf-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bdsf
-Version: 1.9.1
+Version: 1.9.2
 Summary: Blob Detection and Source Finder
 Home-page: https://github.com/lofar-astron/PyBDSF
 Author: David Rafferty
 Author-email: drafferty@hs.uni-hamburg.de
 License: UNKNOWN
 Description: PyBDSF
         ======
```

### Comparing `bdsf-1.9.1/README.rst` & `bdsf-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `bdsf-1.9.1/PKG-INFO` & `bdsf-1.9.2/bdsf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bdsf
-Version: 1.9.1
+Version: 1.9.2
 Summary: Blob Detection and Source Finder
 Home-page: https://github.com/lofar-astron/PyBDSF
 Author: David Rafferty
 Author-email: drafferty@hs.uni-hamburg.de
 License: UNKNOWN
 Description: PyBDSF
         ======
```

