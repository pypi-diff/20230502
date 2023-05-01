# Comparing `tmp/pycryptosat-5.11.8.tar.gz` & `tmp/pycryptosat-5.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptosat-5.11.8.tar", last modified: Sat Apr  1 06:40:44 2023, max compression
+gzip compressed data, was "pycryptosat-5.11.9.tar", last modified: Mon May  1 21:52:37 2023, max compression
```

## Comparing `pycryptosat-5.11.8.tar` & `pycryptosat-5.11.9.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.062507 pycryptosat-5.11.8/python/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.062507 pycryptosat-5.11.8/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/python/src/GitSHA1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30244 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/python/src/pycryptosat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/MersenneTwister.h
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/Vec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/XAlloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/alg.h
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/avgcalc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/boundedqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)    27004 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/bva.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/bva.h
--rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cardfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cardfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ccnr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ccnr.h
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ccnr_cms.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ccnr_cms.h
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ccnr_mersenne.h
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cl_predictors_abs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cl_predictors_lgbm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cl_predictors_py.h
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cl_predictors_xgb.h
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clabstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clause.h
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clauseallocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clauseallocator.h
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clausecleaner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/clausecleaner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cloffset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cms_bosphorus.h
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cms_breakid.h
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cms_windows_includes.h
--rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cnf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cnf.h
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/community_finder.h
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/completedetachreattacher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/completedetachreattacher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    55778 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cryptominisat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cryptominisat.h
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cryptominisat_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cryptominisat_c.h
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/cset.h
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/datasync.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/datasync.h
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/datasyncserver.h
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/dimacsparser.h
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerbin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerbin.h
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlitrem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlitrem.h
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlong.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlong.h
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlongwithimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/distillerlongwithimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/frat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/frat.h
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gatefinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gatefinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    54015 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gausswatched.h
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/get_clause_query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/get_clause_query.h
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/gqueuedata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/hasher.h
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/hyperengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/hyperengine.h
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/intree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/intree.h
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/ipasir.h
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/lucky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/lucky.h
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/main_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/matrixfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/matrixfinder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/src/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/msvc/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/mystack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/nomutex.h
--rw-r--r--   0 runner    (1001) docker     (123)   177837 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/occsimplifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/occsimplifier.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/src/oracle/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/oracle/bitset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/oracle/oracle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/oracle/oracle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/oracle/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/packedmatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/packedrow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/packedrow.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/src/picosat/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/picosat/config.h
--rw-r--r--   0 runner    (1001) docker     (123)   162828 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/picosat/picosat.c
--rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/picosat/picosat.h
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/picosat/version.c
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/popcnt.h
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/predict_func_type.h
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/propby.h
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/propby_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/propbyforgraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/propengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/propengine.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:40:44.086509 pycryptosat-5.11.8/src/pycryptosat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-04-01 06:40:44.000000 pycryptosat-5.11.8/src/pycryptosat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-01 06:40:44.000000 pycryptosat-5.11.8/src/pycryptosat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/reducedb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/reducedb.h
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/satzilla_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/satzilla_features_calc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sccfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sccfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)   121848 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/searcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/searcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/searchhist.h
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/searchstats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/searchstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/shareddata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/signalcode.h
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/simplefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sls.h
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solutionextender.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solutionextender.h
--rw-r--r--   0 runner    (1001) docker     (123)   161063 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solverconf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solverconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solvertypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/solvertypesmini.h
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sql_tablestructure.h
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sqlitestats.h
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/sqlstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/str_impl_w_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/str_impl_w_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/streambuffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/subsumeimplicit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/subsumeimplicit.h
--rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/subsumestrengthen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/subsumestrengthen.h
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/time_mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/toplevelgauss.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/toplevelgaussabst.h
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/touchlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/trim.h
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/vardata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/vardistgen.h
--rw-r--r--   0 runner    (1001) docker     (123)    38447 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/varreplacer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/varreplacer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/varupdatehelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/vmtf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/watchalgos.h
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/watcharray.h
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/watcharray_handrolled.h
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/watched.h
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/xor.h
--rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/xorfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-01 06:40:25.000000 pycryptosat-5.11.8/src/xorfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.368175 pycryptosat-5.11.9/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.368175 pycryptosat-5.11.9/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/python/src/GitSHA1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30244 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/python/src/pycryptosat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 21:52:37.392175 pycryptosat-5.11.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/MersenneTwister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/XAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/avgcalc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/boundedqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27004 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/bva.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/bva.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cardfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cardfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ccnr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ccnr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ccnr_cms.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ccnr_cms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ccnr_mersenne.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cl_predictors_abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cl_predictors_lgbm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cl_predictors_py.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cl_predictors_xgb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clabstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18502 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clause.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clauseallocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clauseallocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clausecleaner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/clausecleaner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cloffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cms_bosphorus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cms_breakid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cms_windows_includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cnf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cnf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/community_finder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/completedetachreattacher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/completedetachreattacher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56483 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cryptominisat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cryptominisat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cryptominisat_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cryptominisat_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/cset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/datasync.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/datasync.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/datasyncserver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/dimacsparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerbin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerbin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlitrem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlitrem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlong.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlong.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlongwithimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/distillerlongwithimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/frat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/frat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gatefinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gatefinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54015 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gausswatched.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/get_clause_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/get_clause_query.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/gqueuedata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/hasher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/hyperengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/hyperengine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/intree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/intree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/ipasir.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/lucky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/lucky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/main_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/matrixfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/matrixfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/src/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/msvc/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/mystack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/nomutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)   177386 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/occsimplifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/occsimplifier.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/src/oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/oracle/bitset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/oracle/oracle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/oracle/oracle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/oracle/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/packedmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/packedrow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/packedrow.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/src/picosat/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/picosat/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)   162828 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/picosat/picosat.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/picosat/picosat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/picosat/version.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/popcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/predict_func_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/propby.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/propby_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/propbyforgraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/propengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/propengine.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:52:37.388175 pycryptosat-5.11.9/src/pycryptosat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-01 21:52:37.000000 pycryptosat-5.11.9/src/pycryptosat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-01 21:52:37.000000 pycryptosat-5.11.9/src/pycryptosat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/reducedb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/reducedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/satzilla_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/satzilla_features_calc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sccfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sccfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)   121913 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/searcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/searcher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/searchhist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/searchstats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/searchstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/shareddata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/signalcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/simplefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solutionextender.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solutionextender.h
+-rw-r--r--   0 runner    (1001) docker     (123)   168174 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solverconf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solverconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solvertypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/solvertypesmini.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sql_tablestructure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sqlitestats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/sqlstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/str_impl_w_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/str_impl_w_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/streambuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/subsumeimplicit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/subsumeimplicit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/subsumestrengthen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/subsumestrengthen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/time_mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/toplevelgauss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/toplevelgaussabst.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/touchlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/trim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/vardata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/vardistgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38447 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/varreplacer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/varreplacer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/varupdatehelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/vmtf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/watchalgos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/watcharray.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/watcharray_handrolled.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/watched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/xorfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-01 21:52:18.000000 pycryptosat-5.11.9/src/xorfinder.h
```

### Comparing `pycryptosat-5.11.8/AUTHORS` & `pycryptosat-5.11.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/LICENSE.txt` & `pycryptosat-5.11.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/PKG-INFO` & `pycryptosat-5.11.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycryptosat
-Version: 5.11.8
+Version: 5.11.9
 Summary: Bindings to CryptoMiniSat, an advanced SAT solver
 Home-page: https://github.com/msoos/cryptominisat
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: Copyright (C) 2009-2020 Authors of CryptoMiniSat, see AUTHORS file
         All rights reserved.
         
@@ -73,15 +73,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS
 
-# pycryptosatiniSat SAT solver
+# pycryptosat SAT solver
 
 This directory provides Python bindings to CryptoMiniSat on the C++ level,
 i.e. when importing pycryptosat, the CryptoMiniSat solver becomes part of the
 Python process itself.
 
 ## Installing
```

### Comparing `pycryptosat-5.11.8/pyproject.toml` & `pycryptosat-5.11.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "toml", "pathlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycryptosat"
-version = "5.11.8"
+version = "5.11.9"
 description = "Bindings to CryptoMiniSat, an advanced SAT solver"
 keywords = ["sat", "cryptography"]
 license = { file = "LICENSE.txt" }
 maintainers = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 authors = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pycryptosat-5.11.8/python/README.md` & `pycryptosat-5.11.9/python/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pycryptosatiniSat SAT solver
+# pycryptosat SAT solver
 
 This directory provides Python bindings to CryptoMiniSat on the C++ level,
 i.e. when importing pycryptosat, the CryptoMiniSat solver becomes part of the
 Python process itself.
 
 ## Installing
```

### Comparing `pycryptosat-5.11.8/python/src/GitSHA1.cpp` & `pycryptosat-5.11.9/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/python/src/pycryptosat.cpp` & `pycryptosat-5.11.9/python/src/pycryptosat.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/setup.py` & `pycryptosat-5.11.9/setup.py`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/GitSHA1.h` & `pycryptosat-5.11.9/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/MersenneTwister.h` & `pycryptosat-5.11.9/src/MersenneTwister.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/Vec.h` & `pycryptosat-5.11.9/src/Vec.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/XAlloc.h` & `pycryptosat-5.11.9/src/XAlloc.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/alg.h` & `pycryptosat-5.11.9/src/alg.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/avgcalc.h` & `pycryptosat-5.11.9/src/avgcalc.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/bitarray.h` & `pycryptosat-5.11.9/src/bitarray.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/boundedqueue.h` & `pycryptosat-5.11.9/src/boundedqueue.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/bva.cpp` & `pycryptosat-5.11.9/src/bva.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/bva.h` & `pycryptosat-5.11.9/src/bva.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cardfinder.cpp` & `pycryptosat-5.11.9/src/cardfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cardfinder.h` & `pycryptosat-5.11.9/src/cardfinder.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ccnr.cpp` & `pycryptosat-5.11.9/src/ccnr.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ccnr.h` & `pycryptosat-5.11.9/src/ccnr.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ccnr_cms.cpp` & `pycryptosat-5.11.9/src/ccnr_cms.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ccnr_cms.h` & `pycryptosat-5.11.9/src/ccnr_cms.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ccnr_mersenne.h` & `pycryptosat-5.11.9/src/ccnr_mersenne.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cl_predictors_abs.h` & `pycryptosat-5.11.9/src/cl_predictors_abs.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cl_predictors_lgbm.h` & `pycryptosat-5.11.9/src/cl_predictors_lgbm.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cl_predictors_py.h` & `pycryptosat-5.11.9/src/cl_predictors_py.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cl_predictors_xgb.h` & `pycryptosat-5.11.9/src/cl_predictors_xgb.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/clabstraction.h` & `pycryptosat-5.11.9/src/clabstraction.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/clause.h` & `pycryptosat-5.11.9/src/clause.h`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     uint32_t sum_props_made = 0; ///<Number of times caused propagation
     float discounted_uip1_used3 = 0;
     float discounted_uip1_used2 = 0;
     float discounted_props_made2 = 0;
     float discounted_props_made3 = 0;
     #ifdef STATS_NEEDED
     uint32_t dump_no = 0;
-    uint32_t orig_ID = 0;
+    int32_t orig_ID = 0;
     uint32_t orig_connects_num_communities = 0;
     uint32_t connects_num_communities = 0;
     uint32_t conflicts_made = 0; ///<Number of times caused conflict
     uint32_t ttl_stats = 0;
     AtecedentData<uint16_t> antec_data;
     #endif
```

### Comparing `pycryptosat-5.11.8/src/clauseallocator.cpp` & `pycryptosat-5.11.9/src/clauseallocator.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/clauseallocator.h` & `pycryptosat-5.11.9/src/clauseallocator.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/clausecleaner.cpp` & `pycryptosat-5.11.9/src/clausecleaner.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/clausecleaner.h` & `pycryptosat-5.11.9/src/clausecleaner.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cloffset.h` & `pycryptosat-5.11.9/src/cloffset.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cms_bosphorus.h` & `pycryptosat-5.11.9/src/cms_bosphorus.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cms_breakid.h` & `pycryptosat-5.11.9/src/cms_breakid.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cms_windows_includes.h` & `pycryptosat-5.11.9/src/cms_windows_includes.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cnf.cpp` & `pycryptosat-5.11.9/src/cnf.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cnf.h` & `pycryptosat-5.11.9/src/cnf.h`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
-#ifndef __CNF_H__
-#define __CNF_H__
+#pragma once
 
 #include <atomic>
 #include <limits>
 
 #include "constants.h"
 #include "vardata.h"
 #include "propby.h"
@@ -804,9 +803,7 @@
 template<class T> void CNF::serialize(T& ar) const
 {
     ar << outer_to_with_bva_map;
     ar << num_bva_vars;
 }
 
 }
-
-#endif //__CNF_H__
```

### Comparing `pycryptosat-5.11.8/src/community_finder.h` & `pycryptosat-5.11.9/src/community_finder.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/completedetachreattacher.cpp` & `pycryptosat-5.11.9/src/completedetachreattacher.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/completedetachreattacher.h` & `pycryptosat-5.11.9/src/completedetachreattacher.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/constants.h` & `pycryptosat-5.11.9/src/constants.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cryptominisat.cpp` & `pycryptosat-5.11.9/src/cryptominisat.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1448,14 +1448,20 @@
 }
 
 DLL_PUBLIC const vector<BNN*>& SATSolver::get_bnns() const
 {
     return data->solvers[0]->get_bnns();
 }
 
+DLL_PUBLIC uint32_t SATSolver::get_verbosity() const
+{
+   const SolverConf& conf = data->solvers[0]->getConf();
+   return conf.verbosity;
+}
+
 DLL_PUBLIC void SATSolver::set_verbosity_detach_warning(bool verb)
 {
     for (size_t i = 0; i < data->solvers.size(); i++) {
         SolverConf conf = data->solvers[i]->getConf();
         conf.xor_detach_verb = verb;
         data->solvers[i]->setConf(conf);
     }
@@ -1890,7 +1896,28 @@
 
 DLL_PUBLIC void SATSolver::delete_extend_solution_setup(void* s)
 {
     CMSat::Solver* solver = (CMSat::Solver*)s;
     delete solver->get_must_interrupt_inter_asap_ptr();
     delete solver;
 }
+
+DLL_PUBLIC bool SATSolver::minimize_clause(std::vector<Lit>& cl)
+{
+    Solver& s = *data->solvers[0];
+    actually_add_clauses_to_threads(data);
+    return s.minimize_clause(cl);
+}
+
+
+DLL_PUBLIC bool SATSolver::backbone_simpl(int64_t max_confl, bool cmsgen)
+{
+    Solver& s = *data->solvers[0];
+    actually_add_clauses_to_threads(data);
+    return s.backbone_simpl(max_confl, cmsgen);
+}
+
+DLL_PUBLIC bool SATSolver::removed_var(uint32_t var) const{
+    Solver& s = *data->solvers[0];
+    actually_add_clauses_to_threads(data);
+    return s.removed_var_ext(var);
+}
```

### Comparing `pycryptosat-5.11.8/src/cryptominisat.h` & `pycryptosat-5.11.9/src/cryptominisat.h`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         /**
          * Conflicts that can be consumed before the next call to solve() must return
          *
          * \pre max_confl >= 0
          */
         void set_max_confl(uint64_t max_confl);
         void set_verbosity(unsigned verbosity = 0); //default is 0, silent
+        uint32_t get_verbosity() const;
         void set_verbosity_detach_warning(bool verb); //default is 0, silent
         void set_default_polarity(bool polarity); //default polarity when branching for all vars
         void set_polarity_mode(CMSat::PolarityMode mode); //set polarity type
         CMSat::PolarityMode get_polarity_mode() const;
         void set_no_simplify(); //never simplify
         void set_no_simplify_at_startup(); //doesn't simplify at start, faster startup time
         void set_no_equivalent_lit_replacement(); //don't replace equivalent literals
@@ -151,14 +152,15 @@
         void set_max_red_linkin_size(uint32_t sz);
         void set_seed(const uint32_t seed);
         void set_renumber(const bool renumber);
         void set_weaken_time_limitM(const uint32_t lim);
         void set_occ_based_lit_rem_time_limitM(const uint32_t lim);
         void set_orig_global_timeout_multiplier(const double mult);
         double get_orig_global_timeout_multiplier();
+        bool minimize_clause(std::vector<Lit>& cl);
 
         ////////////////////////////
         // Predictive system tuning
         ////////////////////////////
         void set_pred_short_size(int32_t sz = -1);
         void set_pred_long_size(int32_t sz = -1);
         void set_pred_forever_size(int32_t sz = -1);
@@ -221,14 +223,15 @@
         std::vector<uint32_t> get_lit_incidence();
         std::vector<uint32_t> get_var_incidence_also_red();
         std::vector<double> get_vsids_scores();
 
         lbool find_fast_backw(FastBackwData fast_backw);
         void remove_and_clean_all();
         lbool probe(Lit l, uint32_t& min_props);
+        bool backbone_simpl(int64_t max_confl, bool cmsgen);
 
         //Given a set of literals to enqueue, returns:
         // 1) Whether they imply UNSAT. If "false": UNSAT
         // 2) into "out_implied" the set of literals they imply, including the literals themselves
         // NOTES:
         // * In case some variables have been eliminated, they cannot be implied
         // * You must not put any variable into it that's been eliminated. Pass a pointer to solve() and simplif() to make sure some variables are never elimianted, or call set_no_bve()
@@ -244,24 +247,24 @@
         bool get_next_small_clause(std::vector<Lit>& ret, bool all_in_one = false); //returns FALSE if no more
         void end_getting_small_clauses();
         uint32_t simplified_nvars();
         std::vector<uint32_t> translate_sampl_set(const std::vector<uint32_t>& sampl_set);
         void get_all_irred_clauses(std::vector<Lit>& ret);
         const std::vector<BNN*>& get_bnns() const;
 
-
         // Solution reconstruction after minimization
         std::string serialize_solution_reconstruction_data() const;
         static void* create_extend_solution_setup(std::string& data);
         static std::pair<lbool, std::vector<lbool>> extend_solution(void* s, const std::vector<lbool>& simp_sol);
         static void delete_extend_solution_setup(void* s);
 
         /////////////////////
         // Backwards compatibility, implemented using the above "small clauses" functions
         void open_file_and_dump_irred_clauses(const char* fname);
+        bool removed_var(uint32_t var) const;
 
     private:
 
         ////////////////////////////
         // Do not bother with this, it's private
         ////////////////////////////
```

### Comparing `pycryptosat-5.11.8/src/cryptominisat_c.cpp` & `pycryptosat-5.11.9/src/cryptominisat_c.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cryptominisat_c.h` & `pycryptosat-5.11.9/src/cryptominisat_c.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/cset.h` & `pycryptosat-5.11.9/src/cset.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/datasync.cpp` & `pycryptosat-5.11.9/src/datasync.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/datasync.h` & `pycryptosat-5.11.9/src/datasync.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/datasyncserver.h` & `pycryptosat-5.11.9/src/datasyncserver.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/dimacsparser.h` & `pycryptosat-5.11.9/src/dimacsparser.h`

 * *Files 1% similar despite different names*

```diff
@@ -471,14 +471,26 @@
             cout << "c Parsed Solver::new_vars( " << n << " )" << endl;
         }
     } else if (str == "ind") {
         sampling_vars_found = true;
         if (!parseIndependentSet(in)) {
             return false;
         }
+    } else if (str == "p") {
+        in.skipWhitespace();
+        std::string str2;
+        in.parseString(str2);
+        if (str2 == "show") {
+            in.skipWhitespace();
+            sampling_vars_found = true;
+            if (!parseIndependentSet(in)) { return false; }
+        } else {
+            cout << "ERROR, 'c p' followed by unknown text: '" << str2 << "'" << endl;
+            exit(-1);
+        }
     } else {
         if (verbosity >= 6) {
             cout
             << "didn't understand in CNF file comment line:"
             << "'c " << str << "'"
             << endl;
         }
```

### Comparing `pycryptosat-5.11.8/src/distillerbin.cpp` & `pycryptosat-5.11.9/src/distillerbin.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/distillerbin.h` & `pycryptosat-5.11.9/src/distillerbin.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/distillerlitrem.cpp` & `pycryptosat-5.11.9/src/distillerlitrem.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,14 @@
 
 bool DistillerLitRem::go_through_clauses(
     vector<ClOffset>& cls,
     uint32_t at
 ) {
     double myTime = cpuTime();
     bool time_out = false;
-    uint32_t skipped = 0;
-    uint32_t tried = 0;
     vector<ClOffset>::iterator i, j;
     i = j = cls.begin();
     for (vector<ClOffset>::iterator end = cls.end()
         ; i != end
         ; ++i
     ) {
         //Check if we are in state where we only copy offsets around
@@ -148,15 +146,14 @@
                 solver->conf.pred_distill_only_smallgue &&
 #else
                 false &&
 #endif
                 cl.red() &&
                 cl.stats.glue > 3)
         ) {
-            skipped++;
             *j++ = *i;
             continue;
         }
         runStats.checkedClauses++;
         assert(cl.size() > 2);
 
         //we will detach the clause no matter what
@@ -167,15 +164,14 @@
         if (solver->satisfied(cl)) {
             solver->detachClause(cl);
             solver->free_cl(&cl);
             continue;
         }
 
         //Try to distill clause
-        tried++;
         offset2 = try_distill_clause_and_return_new(
             offset
             , &cl.stats
             , at
         );
 
         if (offset2 != CL_OFFSET_MAX) {
```

### Comparing `pycryptosat-5.11.8/src/distillerlitrem.h` & `pycryptosat-5.11.9/src/distillerlitrem.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/distillerlong.cpp` & `pycryptosat-5.11.9/src/distillerlong.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -639,17 +639,15 @@
         if (also_remove) {
             cl2->tried_to_remove = 1;
         } else {
             cl2->distilled = 1;
         }
         return solver->cl_alloc.get_offset(cl2);
     } else {
-        #ifdef STATS_NEEDED
-        solver->stats_del_cl(offset);
-        #endif
+        STATS_DO(solver->stats_del_cl(offset));
         //it became a bin/unit/zero
         return CL_OFFSET_MAX;
     }
 }
 
 DistillerLong::Stats& DistillerLong::Stats::operator+=(const Stats& other)
 {
```

### Comparing `pycryptosat-5.11.8/src/distillerlong.h` & `pycryptosat-5.11.9/src/distillerlong.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/distillerlongwithimpl.cpp` & `pycryptosat-5.11.9/src/distillerlongwithimpl.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/distillerlongwithimpl.h` & `pycryptosat-5.11.9/src/distillerlongwithimpl.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/frat.cpp` & `pycryptosat-5.11.9/src/frat.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/frat.h` & `pycryptosat-5.11.9/src/frat.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gatefinder.cpp` & `pycryptosat-5.11.9/src/gatefinder.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gatefinder.h` & `pycryptosat-5.11.9/src/gatefinder.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gaussian.cpp` & `pycryptosat-5.11.9/src/gaussian.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gaussian.h` & `pycryptosat-5.11.9/src/gaussian.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gausswatched.h` & `pycryptosat-5.11.9/src/gausswatched.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/get_clause_query.cpp` & `pycryptosat-5.11.9/src/get_clause_query.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/get_clause_query.h` & `pycryptosat-5.11.9/src/get_clause_query.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/gqueuedata.h` & `pycryptosat-5.11.9/src/gqueuedata.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/hasher.h` & `pycryptosat-5.11.9/src/hasher.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/heap.h` & `pycryptosat-5.11.9/src/heap.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/hyperengine.cpp` & `pycryptosat-5.11.9/src/hyperengine.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/hyperengine.h` & `pycryptosat-5.11.9/src/hyperengine.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/intree.cpp` & `pycryptosat-5.11.9/src/intree.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/intree.h` & `pycryptosat-5.11.9/src/intree.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/ipasir.h` & `pycryptosat-5.11.9/src/ipasir.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/lucky.cpp` & `pycryptosat-5.11.9/src/lucky.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/lucky.h` & `pycryptosat-5.11.9/src/lucky.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/main.h` & `pycryptosat-5.11.9/src/main.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/main_common.h` & `pycryptosat-5.11.9/src/main_common.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/matrixfinder.cpp` & `pycryptosat-5.11.9/src/matrixfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/matrixfinder.h` & `pycryptosat-5.11.9/src/matrixfinder.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/msvc/stdint.h` & `pycryptosat-5.11.9/src/msvc/stdint.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/mystack.h` & `pycryptosat-5.11.9/src/mystack.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/nomutex.h` & `pycryptosat-5.11.9/src/nomutex.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/occsimplifier.cpp` & `pycryptosat-5.11.9/src/occsimplifier.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1787,68 +1787,56 @@
 }
 
 void OccSimplifier::clean_sampl_and_get_empties(
     vector<uint32_t>& sampl_vars, vector<uint32_t>& empty_vars)
 {
     assert(solver->okay());
     assert(solver->prop_at_head());
+    release_assert(empty_vars.empty());
     if (!setup()) return;
 
     auto origTrailSize = solver->trail_size();
     startup = false;
     const double backup = solver->conf.maxOccurRedMB;
     solver->conf.maxOccurRedMB = 0;
     const double myTime = cpuTime();
 
     set<uint32_t> empty_vars_set;
-    for(auto& v: empty_vars) {
-        v = solver->varReplacer->get_var_replaced_with(v);
-        empty_vars_set.insert(v);
-    }
 
     // Clean up sampl_vars from replaced and set variables
     set<uint32_t> sampl_vars_set;
     for(uint32_t& v: sampl_vars) {
         assert(v < solver->nVarsOutside());
         auto rem_val = solver->varData[v].removed;
         assert(rem_val == Removed::none || rem_val == Removed::replaced);
         v = solver->varReplacer->get_var_replaced_with(v);
         rem_val = solver->varData[v].removed;
         assert(rem_val == Removed::none);
         assert(v < solver->nVars());
         assert(solver->varData[v].removed == Removed::none);
 
         if (solver->value(v) != l_Undef) continue;
-        if (empty_vars_set.find(v) != empty_vars_set.end()) continue;
         sampl_vars_set.insert(v);
     }
 
     // Find empties
     uint32_t mirror = 0;
     uint32_t empty_occ = 0;
     for(auto& v: sampl_vars_set) {
         if (!solver->okay()) goto end;
         const Lit l = Lit(v, false);
 
-        uint32_t total = solver->watches[l].size() + solver->watches[~l].size();
-        if (total == 0 || (solver->zero_irred_cls(l) && solver->zero_irred_cls(~l))) {
+        uint32_t irred_and_red = solver->watches[l].size() + solver->watches[~l].size();
+        if (irred_and_red == 0 || (solver->zero_irred_cls(l) && solver->zero_irred_cls(~l))) {
             empty_occ++;
             empty_vars_set.insert(v);
             elim_var_by_str(l.var(), {});
             assert(solver->watches[l].empty() && solver->watches[~l].empty());
             continue;
         }
-
-        /*if (mirror_empty && solver->bnns.empty()) {
-            if (!check_equiv_subformula(l)) continue;
-            if (!solver->okay()) goto end;
-            assert(solver->watches[l].empty() && solver->watches[~l].empty());
-            empty_vars.push_back(orig_v);
-            mirror++;
-        }*/
     }
 
     // Replace what we were given with cleaned + empty removed
     sampl_vars.clear();
     for(auto const& v: sampl_vars_set) {
         if (empty_vars_set.find(v) == empty_vars_set.end())
             sampl_vars.push_back(v);
```

### Comparing `pycryptosat-5.11.8/src/occsimplifier.h` & `pycryptosat-5.11.9/src/occsimplifier.h`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
-#ifndef SIMPLIFIER_H
-#define SIMPLIFIER_H
-
+#pragma once
 
 #include <map>
 #include <vector>
 #include <list>
 #include <set>
 #include <queue>
 #include <map>
@@ -677,21 +675,14 @@
 }
 
 inline bool OccSimplifier::getAnythingHasBeenElimed() const
 {
     return anythingHasBeenElimed;
 }
 
-/*inline std::ostream& operator<<(std::ostream& os, const ElimedClauses& bl)
-{
-    os << bl.lits << " to remove: " << bl.toRemove;
-
-    return os;
-}*/
-
 inline bool OccSimplifier::subsetReverse(const Clause& B) const
 {
     for (uint32_t i = 0; i != B.size(); i++) {
         if (!seen[B[i].toInt()])
             return false;
     }
     return true;
@@ -713,9 +704,7 @@
 void OccSimplifier::serialize_elimed_cls(T& ar) const
 {
     ar << eClsLits;
     ar << elimedClauses;
 }
 
 } //end namespace
-
-#endif //SIMPLIFIER_H
```

### Comparing `pycryptosat-5.11.8/src/oracle/bitset.hpp` & `pycryptosat-5.11.9/src/oracle/bitset.hpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/oracle/oracle.cpp` & `pycryptosat-5.11.9/src/oracle/oracle.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/oracle/oracle.hpp` & `pycryptosat-5.11.9/src/oracle/oracle.hpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/oracle/utils.hpp` & `pycryptosat-5.11.9/src/oracle/utils.hpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/packedmatrix.h` & `pycryptosat-5.11.9/src/packedmatrix.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/packedrow.cpp` & `pycryptosat-5.11.9/src/packedrow.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/packedrow.h` & `pycryptosat-5.11.9/src/packedrow.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/picosat/picosat.c` & `pycryptosat-5.11.9/src/picosat/picosat.c`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/picosat/picosat.h` & `pycryptosat-5.11.9/src/picosat/picosat.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/popcnt.h` & `pycryptosat-5.11.9/src/popcnt.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/predict_func_type.h` & `pycryptosat-5.11.9/src/predict_func_type.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/propby.h` & `pycryptosat-5.11.9/src/propby.h`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
-#ifndef PROPBY_H
-#define PROPBY_H
+#pragma once
 
 #include "constants.h"
 #include "solvertypes.h"
 #include "clause.h"
 #include "cloffset.h"
 
 #include <boost/serialization/split_member.hpp>
@@ -337,9 +336,7 @@
             assert(false);
             break;
     }
     return os;
 }
 
 } //end namespace
-
-#endif //PROPBY_H
```

### Comparing `pycryptosat-5.11.8/src/propby_backup.h` & `pycryptosat-5.11.9/src/propby_backup.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/propbyforgraph.h` & `pycryptosat-5.11.9/src/propbyforgraph.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/propengine.cpp` & `pycryptosat-5.11.9/src/propengine.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/propengine.h` & `pycryptosat-5.11.9/src/propengine.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/pycryptosat.egg-info/PKG-INFO` & `pycryptosat-5.11.9/src/pycryptosat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycryptosat
-Version: 5.11.8
+Version: 5.11.9
 Summary: Bindings to CryptoMiniSat, an advanced SAT solver
 Home-page: https://github.com/msoos/cryptominisat
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: Copyright (C) 2009-2020 Authors of CryptoMiniSat, see AUTHORS file
         All rights reserved.
         
@@ -73,15 +73,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS
 
-# pycryptosatiniSat SAT solver
+# pycryptosat SAT solver
 
 This directory provides Python bindings to CryptoMiniSat on the C++ level,
 i.e. when importing pycryptosat, the CryptoMiniSat solver becomes part of the
 Python process itself.
 
 ## Installing
```

### Comparing `pycryptosat-5.11.8/src/pycryptosat.egg-info/SOURCES.txt` & `pycryptosat-5.11.9/src/pycryptosat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/reducedb.cpp` & `pycryptosat-5.11.9/src/reducedb.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/reducedb.h` & `pycryptosat-5.11.9/src/reducedb.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/satzilla_features.h` & `pycryptosat-5.11.9/src/satzilla_features.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/satzilla_features_calc.h` & `pycryptosat-5.11.9/src/satzilla_features_calc.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sccfinder.cpp` & `pycryptosat-5.11.9/src/sccfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sccfinder.h` & `pycryptosat-5.11.9/src/sccfinder.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/searcher.cpp` & `pycryptosat-5.11.9/src/searcher.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2595,20 +2595,21 @@
     check_calc_vardist_features(true);
     #endif
 
     SLOW_DEBUG_DO(assert(fast_backw.fast_backw_on || solver->check_order_heap_sanity()));
     while(stats.conflicts < max_confl_per_search_solve_call
         && status == l_Undef
     ) {
-        if (distill_clauses_if_needed() == l_False
-            || full_probe_if_needed() == l_False
-            || !distill_bins_if_needed()
-            || !sub_str_with_bin_if_needed()
-            || !str_impl_with_impl_if_needed()
-            || !intree_if_needed()
+        if (!conf.never_stop_search &&
+                (distill_clauses_if_needed() == l_False
+                || full_probe_if_needed() == l_False
+                || !distill_bins_if_needed()
+                || !sub_str_with_bin_if_needed()
+                || !str_impl_with_impl_if_needed()
+                || !intree_if_needed())
         ) {
             status = l_False;
             goto end;
         }
         SLOW_DEBUG_DO(assert(solver->check_order_heap_sanity()));
         sls_if_needed();
```

### Comparing `pycryptosat-5.11.8/src/searcher.h` & `pycryptosat-5.11.9/src/searcher.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/searchhist.h` & `pycryptosat-5.11.9/src/searchhist.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/searchstats.cpp` & `pycryptosat-5.11.9/src/searchstats.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/searchstats.h` & `pycryptosat-5.11.9/src/searchstats.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/shareddata.h` & `pycryptosat-5.11.9/src/shareddata.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/signalcode.h` & `pycryptosat-5.11.9/src/signalcode.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/simplefile.h` & `pycryptosat-5.11.9/src/simplefile.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sls.cpp` & `pycryptosat-5.11.9/src/sls.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sls.h` & `pycryptosat-5.11.9/src/sls.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/solutionextender.cpp` & `pycryptosat-5.11.9/src/solutionextender.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/solutionextender.h` & `pycryptosat-5.11.9/src/solutionextender.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/solver.cpp` & `pycryptosat-5.11.9/src/solver.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 #include <limits>
 #include <string>
 #include <algorithm>
 #include <vector>
 #include <complex>
 #include <locale>
 #include <random>
+
 #include <boost/archive/text_iarchive.hpp>
 #include <boost/archive/text_oarchive.hpp>
 #include <boost/archive/binary_iarchive.hpp>
 #include <boost/archive/binary_oarchive.hpp>
 #include <boost/serialization/vector.hpp>
 
-
 #include "varreplacer.h"
 #include "time_mem.h"
 #include "searcher.h"
 #include "occsimplifier.h"
 #include "distillerlong.h"
 #include "distillerbin.h"
 #include "distillerlitrem.h"
@@ -75,14 +75,15 @@
 #include "lucky.h"
 #include "get_clause_query.h"
 #include "community_finder.h"
 #include "oracle/oracle.hpp"
 extern "C" {
 #include "picosat/picosat.h"
 }
+#include "cryptominisat.h"
 
 #ifdef USE_BREAKID
 #include "cms_breakid.h"
 #endif
 
 #ifdef USE_BOSPHORUS
 #include "cms_bosphorus.h"
@@ -1592,14 +1593,16 @@
 }
 
 void Solver::reset_for_solving()
 {
     longest_trail_ever_best = 0;
     longest_trail_ever_inv = 0;
     fresh_solver = false;
+    polarity_strategy_change = 0;
+    increasing_phase_size = conf.restart_first;
     set_assumptions();
     #ifdef SLOW_DEBUG
     if (ok) {
         assert(check_order_heap_sanity());
         check_implicit_stats();
         find_all_attach();
         check_no_duplicate_lits_anywhere();
@@ -4141,15 +4144,15 @@
 {
     for(auto& x: var_act_vsids) x = 0;
 }
 
 #ifdef STATS_NEEDED
 void Solver::stats_del_cl(Clause* cl)
 {
-    if (cl->stats.is_tracked != 0 && sqlStats) {
+    if (cl->stats.is_tracked && sqlStats) {
         const ClauseStatsExtra& stats_extra = solver->red_stats_extra[cl->stats.extra_pos];
         assert(stats_extra.orig_ID != 0);
         assert(stats_extra.orig_ID <= cl->stats.ID);
         sqlStats->cl_last_in_solver(this, stats_extra.orig_ID);
     }
 }
 
@@ -4786,14 +4789,18 @@
 
 void Solver::clean_sampl_and_get_empties(
     vector<uint32_t>& sampl_vars, vector<uint32_t>& empty_vars)
 {
     if (!okay()) return;
     assert(get_num_bva_vars() == 0);
     map_outer_to_inter(sampl_vars);
+    map_outer_to_inter(empty_vars);
+    for(const auto& v: empty_vars) sampl_vars.push_back(v);
+    empty_vars.clear();
+
     occsimplifier->clean_sampl_and_get_empties(sampl_vars, empty_vars);
     map_inter_to_outer(sampl_vars);
     map_inter_to_outer(empty_vars);
 }
 
 bool Solver::remove_and_clean_all() {
     return clauseCleaner->remove_and_clean_all();
@@ -5392,23 +5399,226 @@
     updateArrayRev(model, interToOuterMain);
 
     SolutionExtender extender(this, occsimplifier);
     extender.extend();
     return make_pair(l_True, model);
 }
 
+// returns whether it can be removed
+bool Solver::minimize_clause(vector<Lit>& cl) {
+    assert(get_num_bva_vars() == 0);
+
+    addClauseHelper(cl);
+    new_decision_level();
+    uint32_t i = 0;
+    uint32_t j = 0;
+    PropBy confl;
+
+    for (uint32_t sz = cl.size(); i < sz; i++) {
+        const Lit lit = cl[i];
+        lbool val = value(lit);
+        if (val == l_Undef) {
+            enqueue<true>(~lit);
+            cl[j++] = cl[i];
+            confl = solver->propagate<true, true, true>();
+            if (!confl.isNULL()) break;
+        } else if (val == l_False) {
+        } else {
+            assert(val == l_True);
+            cl[j++] = cl[i];
+            break;
+        }
+    }
+    assert(solver->ok);
+    cl.resize(j);
+    cancelUntil<false, true>(0);
+    map_inter_to_outer(cl);
+
+    bool can_be_removed = !confl.isNULL();
+    return can_be_removed;
+}
+
+bool Solver::backbone_simpl(int64_t orig_max_confl, bool cmsgen)
+{
+    if (!okay()) return false;
+    assert(get_num_bva_vars() == 0);
+    verb_print(1, "[backbone-simpl] starting backbone simplification...");
+    uint64_t last_sum_conflicts = 0;
+
+    double myTime = cpuTime();
+    bool finished = false;
+    Lit l;
+    uint32_t undefs = 0;
+    uint32_t tried = 0;
+    const auto orig_trail_size = trail.size();
+
+    vector<Lit> tmp_clause;
+    vector<lbool> old_model;
+    uint32_t num_seen_flipped = 0;
+    vector<char> seen_flipped;
+    seen_flipped.resize(nVars(), 0);
+    const auto old_verb = conf.verbosity;
+    conf.verbosity = 0;
+
+    if (cmsgen) {
+        //CMSGen-based seen_flipped detection, so we don't need to query so much
+        SATSolver s2;
+        s2.new_vars(nVars());
+        s2.set_verbosity(0);
+        bool ret = true;
+        start_getting_small_clauses(
+            std::numeric_limits<uint32_t>::max(),
+            std::numeric_limits<uint32_t>::max(),
+            false,
+            false,
+            true);
+        vector<Lit> clause;
+        while (ret) {
+            ret = get_next_small_clause(clause);
+            if (!ret) break;
+            s2.add_clause(clause);
+        }
+        end_getting_small_clauses();
+
+        uint64_t last_num_conflicts = 0;
+        int64_t remaining_confls = orig_max_confl;
+        s2.set_max_confl(remaining_confls*2);
+        uint32_t num_runs = 0;
+        auto s2_ret = s2.solve();
+        remaining_confls -= (s2.get_sum_conflicts() - last_num_conflicts);
+        if (s2_ret == l_True) {
+            old_model = s2.get_model();
+            s2.set_up_for_sample_counter(100);
+            for(uint32_t i = 0; i < 30 && remaining_confls > 0; i++) {
+                last_num_conflicts = s2.get_sum_conflicts();
+                s2.set_max_confl(remaining_confls);
+                s2_ret = s2.solve();
+                remaining_confls -= (s2.get_sum_conflicts() - last_num_conflicts);
+                if (s2_ret == l_Undef) break;
+                num_runs++;
+                const auto& this_model = s2.get_model();
+                for(uint32_t i2 = 0, max = s2.nVars(); i2 < max; i2++) {
+                    if (value(i2) != l_Undef) continue;
+                    if (varData[i2].removed != Removed::none) continue;
+                    if (seen_flipped[i2]) continue;
+                    if (this_model[i2] != old_model[i2]) {
+                        seen_flipped[i2] = 1;
+                        num_seen_flipped++;
+                    }
+                }
+            }
+        }
+        if (old_verb >=1) cout << "c [backbone-simpl] num seen flipped: "
+            << num_seen_flipped
+            << " conflicts used: " << print_value_kilo_mega(s2.get_sum_conflicts())
+            << " num runs succeeded: " << num_runs
+            << " T: " << std::fixed << std::setprecision(2) << (cpuTime() - myTime) << endl;
+    }
+
+    // Sort according to occurrence
+    vector<uint32_t> var_order;
+    for(uint32_t var = 0; var < nVars(); var++) {
+        if (seen_flipped[var]) continue;
+        if (value(var) != l_Undef) continue;
+        if (varData[var].removed != Removed::none) continue;
+        var_order.push_back(var);
+    }
+    std::mt19937 g;
+    g.seed(18337);
+    std::shuffle(var_order.begin(), var_order.end(), g);
+
+    int64_t remaining_confl = orig_max_confl;
+    set_max_confl(remaining_confl);
+    last_sum_conflicts = sumConflicts;
+
+    const auto old_polar_mode = conf.polarity_mode;
+    conf.polarity_mode = PolarityMode::polarmode_neg;
+    lbool ret = iterate_until_solved();
+    old_model = assigns;
+    cancelUntil(0);
+    if (ret == l_False) goto end;
+    if (ret == l_Undef || remaining_confl < 0) goto end;
+    assert(last_sum_conflicts <= sumConflicts);
+    remaining_confl -= (sumConflicts - last_sum_conflicts);
+
+    for(const auto& var: var_order) {
+        if (seen_flipped[var]) continue;
+        if (value(var) != l_Undef) continue;
+        if (varData[var].removed != Removed::none) continue;
+
+        l = Lit(var, old_model[var] == l_False);
+
+        //There is definitely a solution with "l". Let's see if ~l fails.
+        assert(assumptions.empty());
+        assumptions.push_back(AssumptionPair(map_inter_to_outer(~l), lit_Undef));
+        fill_assumptions_set();
+        set_max_confl(remaining_confl/20);
+        ret = iterate_until_solved();
+        auto new_model = assigns;
+        cancelUntil(0);
+        unfill_assumptions_set();
+        assumptions.clear();
+        tried++;
+
+        //Update max confl
+        assert(last_sum_conflicts <= sumConflicts);
+        remaining_confl -= (sumConflicts - last_sum_conflicts);
+        last_sum_conflicts = sumConflicts;
+
+        if (ret == l_True) {
+            for(uint32_t i2 = 0; i2 < nVars(); i2++) {
+                if (seen_flipped[i2] ||
+                        value(i2) != l_Undef || new_model[i2] == l_Undef ||
+                        varData[i2].removed != Removed::none) continue;
+                if (new_model[i2] != old_model[i2]) {
+                    seen_flipped[i2] = 1;
+                    num_seen_flipped++;
+                }
+            }
+        } else if (ret == l_False) {
+            tmp_clause.clear();
+            tmp_clause.push_back(l);
+            Clause* ptr = add_clause_int(tmp_clause);
+            assert(ptr == 0);
+            if (!okay()) goto end;
+        } else {
+            undefs++;
+        }
+        if (remaining_confl < 0) goto end;
+    }
+    finished = true;
+    assert(okay());
+
+    end:
+    uint32_t num_set = trail.size() - orig_trail_size;
+    double time_used = cpuTime() - myTime;
+    conf.polarity_mode = old_polar_mode;
+    conf.verbosity = old_verb;
+
+    verb_print(1,
+        "[backbone-simpl]"
+        << " finished: " << finished
+        << " undefs: " << undefs
+        << " tried: "  << tried
+        << " set: " << num_set
+        << " T: " << std::setprecision(2) << time_used);
+
+    return okay();
+}
+
 #ifdef STATS_NEEDED
 void Solver::dump_clauses_at_finishup_as_last()
 {
     if (!sqlStats)
         return;
 
     for(auto& red_cls: longRedCls) {
         for(auto& offs: red_cls) {
             Clause* cl = cl_alloc.ptr(offs);
-            if (cl->stats.ID != 0) {
-                sqlStats->cl_last_in_solver(solver, cl->stats.ID);
+            if (cl->stats.is_tracked) {
+                ClauseStatsExtra& stats_extra = solver->red_stats_extra[cl->stats.extra_pos];
+                sqlStats->cl_last_in_solver(solver, stats_extra.orig_ID);
             }
         }
     }
 }
 #endif
```

### Comparing `pycryptosat-5.11.8/src/solver.h` & `pycryptosat-5.11.9/src/solver.h`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             std::vector<Lit>& out_implied
         );
 
         //get clauses
         void start_getting_small_clauses(
             uint32_t max_len, uint32_t max_glue, bool red = true,
             bool bva_vars = false, bool simplified = false);
-        bool get_next_small_clause(std::vector<Lit>& out, bool all_in_one);
+        bool get_next_small_clause(std::vector<Lit>& out, bool all_in_one = false);
         void end_getting_small_clauses();
         void get_all_irred_clauses(vector<Lit>& out);
         vector<uint32_t> translate_sampl_set(const vector<uint32_t>& sampl_set);
 
         //Version
         static const char* get_version_tag();
         static const char* get_version_sha1();
@@ -156,15 +156,15 @@
         uint64_t print_watch_mem_used(uint64_t totalMem) const;
         const SolveStats& get_solve_stats() const;
         const SearchStats& get_stats() const;
         void add_in_partial_solving_stats();
         void check_implicit_stats(const bool onlypairs = false) const;
         void check_stats(const bool allowFreed = false) const;
         void reset_vsids();
-
+        bool minimize_clause(vector<Lit>& cl);
 
         //Checks
         void check_implicit_propagated() const;
         bool find_with_watchlist_a_or_b(Lit a, Lit b, int64_t* limit) const;
 
         //Systems that are used to accompilsh the tasks
         ClauseCleaner*         clauseCleaner = NULL;
@@ -325,14 +325,16 @@
         SatZillaFeatures last_solve_satzilla_feature;
         #endif
 
         //Helper
         void renumber_xors_to_outside(const vector<Xor>& xors, vector<Xor>& xors_ret);
         void testing_set_solver_not_fresh();
         bool full_probe(const bool bin_only);
+        bool backbone_simpl(int64_t max_confl, bool cmsgen);
+        bool removed_var_ext(uint32_t var) const;
 
     private:
         friend class ClauseDumper;
         #ifdef CMS_TESTING_ENABLED
         FRIEND_TEST(SearcherTest, pickpolar_auto_not_changed_by_simp);
         #endif
 
@@ -674,10 +676,17 @@
     if (also_remove_clid) {
         stats_del_cl(offs);
     }
     #endif
     cl_alloc.clauseFree(offs);
 }
 
+inline bool Solver::removed_var_ext(uint32_t var) const
+{
+    assert(get_num_bva_vars() == 0);
+    var = map_outer_to_inter(var);
+    return value(var) != l_Undef || varData[var].removed != Removed::none;
+}
+
 } //end namespace
 
 #endif //SOLVER_H
```

### Comparing `pycryptosat-5.11.8/src/solverconf.cpp` & `pycryptosat-5.11.9/src/solverconf.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/solverconf.h` & `pycryptosat-5.11.9/src/solverconf.h`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,17 @@
 
         case Restart::geom:
             return "geometric";
 
         case Restart::luby:
             return "luby";
 
+        case Restart::fixed:
+            return "fixed";
+
         case Restart::never:
             return "never";
 
         default:
             assert(false && "Unknown clause cleaning type?");
     }
     assert(false);
```

### Comparing `pycryptosat-5.11.8/src/solvertypes.h` & `pycryptosat-5.11.9/src/solvertypes.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/solvertypesmini.h` & `pycryptosat-5.11.9/src/solvertypesmini.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sql_tablestructure.h` & `pycryptosat-5.11.9/src/sql_tablestructure.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sqlitestats.h` & `pycryptosat-5.11.9/src/sqlitestats.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/sqlstats.h` & `pycryptosat-5.11.9/src/sqlstats.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/str_impl_w_impl.cpp` & `pycryptosat-5.11.9/src/str_impl_w_impl.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/str_impl_w_impl.h` & `pycryptosat-5.11.9/src/str_impl_w_impl.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/streambuffer.h` & `pycryptosat-5.11.9/src/streambuffer.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/subsumeimplicit.cpp` & `pycryptosat-5.11.9/src/subsumeimplicit.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/subsumeimplicit.h` & `pycryptosat-5.11.9/src/subsumeimplicit.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/subsumestrengthen.cpp` & `pycryptosat-5.11.9/src/subsumestrengthen.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/subsumestrengthen.h` & `pycryptosat-5.11.9/src/subsumestrengthen.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/time_mem.h` & `pycryptosat-5.11.9/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/toplevelgauss.h` & `pycryptosat-5.11.9/src/toplevelgauss.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/toplevelgaussabst.h` & `pycryptosat-5.11.9/src/toplevelgaussabst.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/touchlist.h` & `pycryptosat-5.11.9/src/touchlist.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/trim.h` & `pycryptosat-5.11.9/src/trim.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/vardata.h` & `pycryptosat-5.11.9/src/vardata.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/vardistgen.h` & `pycryptosat-5.11.9/src/vardistgen.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/varreplacer.cpp` & `pycryptosat-5.11.9/src/varreplacer.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/varreplacer.h` & `pycryptosat-5.11.9/src/varreplacer.h`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
-#ifndef VARREPLACER_H
-#define VARREPLACER_H
+#pragma once
 
 #include <map>
 #include <vector>
 #include <utility>
 #include <tuple>
 #include <boost/serialization/vector.hpp>
 #include <boost/serialization/map.hpp>
@@ -336,9 +335,7 @@
 void VarReplacer::unserialize_tables(T& ar)
 {
     ar >> table;
     ar >> reverseTable;
 }
 
 } //end namespace
-
-#endif //VARREPLACER_H
```

### Comparing `pycryptosat-5.11.8/src/varupdatehelper.h` & `pycryptosat-5.11.9/src/varupdatehelper.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/vmtf.h` & `pycryptosat-5.11.9/src/vmtf.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/watchalgos.h` & `pycryptosat-5.11.9/src/watchalgos.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/watcharray.h` & `pycryptosat-5.11.9/src/watcharray.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/watcharray_handrolled.h` & `pycryptosat-5.11.9/src/watcharray_handrolled.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/watched.h` & `pycryptosat-5.11.9/src/watched.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/xor.h` & `pycryptosat-5.11.9/src/xor.h`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/xorfinder.cpp` & `pycryptosat-5.11.9/src/xorfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycryptosat-5.11.8/src/xorfinder.h` & `pycryptosat-5.11.9/src/xorfinder.h`

 * *Files identical despite different names*

