# Comparing `tmp/pyunigen-2.5.3.tar.gz` & `tmp/pyunigen-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunigen-2.5.3.tar", last modified: Sat Apr  1 06:11:19 2023, max compression
+gzip compressed data, was "pyunigen-2.5.4.tar", last modified: Mon May  1 22:08:39 2023, max compression
```

## Comparing `pyunigen-2.5.3.tar` & `pyunigen-2.5.4.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.982832 pyunigen-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-01 06:10:54.000000 pyunigen-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-01 06:11:19.982832 pyunigen-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-01 06:10:54.000000 pyunigen-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-01 06:10:54.000000 pyunigen-2.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-01 06:10:54.000000 pyunigen-2.5.3/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/approxmc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/approxmc/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/approxmc/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/python/src/GitSHA1.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.942831 pyunigen-2.5.3/python/approxmc/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/approxmc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/approxmc.h
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/config.h
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/constants.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/counter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/counter.h
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-01 06:11:08.000000 pyunigen-2.5.3/python/approxmc/src/time_mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/arjun/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/arjun/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.942831 pyunigen-2.5.3/python/arjun/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/python/src/GitSHA1.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.946831 pyunigen-2.5.3/python/arjun/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/MersenneTwister.h
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/arjun.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/arjun.h
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/backward.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/config.h
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/simplify.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-01 06:11:07.000000 pyunigen-2.5.3/python/arjun/src/time_mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/cryptominisat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.938831 pyunigen-2.5.3/python/cryptominisat/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.946831 pyunigen-2.5.3/python/cryptominisat/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/python/src/GitSHA1.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.974831 pyunigen-2.5.3/python/cryptominisat/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/MersenneTwister.h
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/Vec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/XAlloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/alg.h
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/avgcalc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/boundedqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)    27004 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/bva.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/bva.h
--rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cardfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cardfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ccnr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ccnr.h
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ccnr_cms.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ccnr_cms.h
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ccnr_mersenne.h
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_abs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_lgbm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_py.h
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_xgb.h
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clabstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clause.h
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clauseallocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clauseallocator.h
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clausecleaner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/clausecleaner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cloffset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cms_bosphorus.h
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cms_breakid.h
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cms_windows_includes.h
--rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cnf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cnf.h
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/community_finder.h
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/completedetachreattacher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/completedetachreattacher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    55778 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cryptominisat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cryptominisat.h
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cryptominisat_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cryptominisat_c.h
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/cset.h
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/datasync.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/datasync.h
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/datasyncserver.h
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/dimacsparser.h
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerbin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerbin.h
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlitrem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlitrem.h
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlong.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlong.h
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlongwithimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/distillerlongwithimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/frat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/frat.h
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gatefinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gatefinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    54015 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gausswatched.h
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/get_clause_query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/get_clause_query.h
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/gqueuedata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/hasher.h
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/hyperengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/hyperengine.h
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/intree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/intree.h
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/ipasir.h
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/lucky.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/lucky.h
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/main_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/matrixfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/matrixfinder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.978831 pyunigen-2.5.3/python/cryptominisat/src/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/msvc/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/mystack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/nomutex.h
--rw-r--r--   0 runner    (1001) docker     (123)   177837 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/occsimplifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/occsimplifier.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.978831 pyunigen-2.5.3/python/cryptominisat/src/oracle/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/oracle/bitset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/oracle/oracle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/oracle/oracle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/oracle/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/packedmatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/packedrow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/packedrow.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.978831 pyunigen-2.5.3/python/cryptominisat/src/picosat/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/picosat/config.h
--rw-r--r--   0 runner    (1001) docker     (123)   162828 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/picosat/picosat.c
--rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/picosat/picosat.h
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/picosat/version.c
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/popcnt.h
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/predict_func_type.h
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/propby.h
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/propby_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/propbyforgraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/propengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/propengine.h
--rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/reducedb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/reducedb.h
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/satzilla_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/satzilla_features_calc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sccfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sccfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)   121848 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/searcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/searcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/searchhist.h
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/searchstats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/searchstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/shareddata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/signalcode.h
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/simplefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sls.h
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solutionextender.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solutionextender.h
--rw-r--r--   0 runner    (1001) docker     (123)   161063 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solverconf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solverconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solvertypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/solvertypesmini.h
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sql_tablestructure.h
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sqlitestats.h
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/sqlstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/str_impl_w_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/str_impl_w_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/streambuffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/subsumeimplicit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/subsumeimplicit.h
--rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/subsumestrengthen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/subsumestrengthen.h
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/time_mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/toplevelgauss.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/toplevelgaussabst.h
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/touchlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/trim.h
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/vardata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/vardistgen.h
--rw-r--r--   0 runner    (1001) docker     (123)    38447 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/varreplacer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/varreplacer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/varupdatehelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/vmtf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/watchalgos.h
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/watcharray.h
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/watcharray_handrolled.h
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/watched.h
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/xor.h
--rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/xorfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-01 06:11:06.000000 pyunigen-2.5.3/python/cryptominisat/src/xorfinder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.978831 pyunigen-2.5.3/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-01 06:10:54.000000 pyunigen-2.5.3/python/src/GitSHA1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-04-01 06:10:54.000000 pyunigen-2.5.3/python/src/pyunigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 06:11:19.982832 pyunigen-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-01 06:10:54.000000 pyunigen-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.982832 pyunigen-2.5.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/config.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 06:11:19.982832 pyunigen-2.5.3/src/pyunigen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-01 06:11:19.000000 pyunigen-2.5.3/src/pyunigen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-01 06:11:19.000000 pyunigen-2.5.3/src/pyunigen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/sampler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/sampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/time_mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/unigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-01 06:10:54.000000 pyunigen-2.5.3/src/unigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.929216 pyunigen-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 22:08:16.000000 pyunigen-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-01 22:08:39.929216 pyunigen-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-01 22:08:16.000000 pyunigen-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 22:08:16.000000 pyunigen-2.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-01 22:08:16.000000 pyunigen-2.5.4/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/approxmc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/approxmc/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/approxmc/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/python/src/GitSHA1.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/approxmc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/approxmc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/approxmc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/counter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/counter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-01 22:08:30.000000 pyunigen-2.5.4/python/approxmc/src/time_mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/arjun/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/arjun/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/arjun/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/python/src/GitSHA1.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.905216 pyunigen-2.5.4/python/arjun/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/MersenneTwister.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/arjun.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/arjun.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/backward.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15879 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/simplify.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-01 22:08:29.000000 pyunigen-2.5.4/python/arjun/src/time_mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/cryptominisat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.901216 pyunigen-2.5.4/python/cryptominisat/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.905216 pyunigen-2.5.4/python/cryptominisat/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/python/src/GitSHA1.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.925216 pyunigen-2.5.4/python/cryptominisat/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/MersenneTwister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/XAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/avgcalc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/boundedqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27004 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/bva.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/bva.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cardfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cardfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ccnr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ccnr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ccnr_cms.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ccnr_cms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ccnr_mersenne.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_lgbm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_py.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_xgb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clabstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18502 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clause.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clauseallocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clauseallocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clausecleaner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/clausecleaner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cloffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cms_bosphorus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cms_breakid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cms_windows_includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cnf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cnf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/community_finder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/completedetachreattacher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/completedetachreattacher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56483 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cryptominisat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cryptominisat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cryptominisat_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cryptominisat_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/cset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/datasync.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/datasync.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/datasyncserver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/dimacsparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerbin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerbin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlitrem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlitrem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlong.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlong.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlongwithimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/distillerlongwithimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/frat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/frat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gatefinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gatefinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54015 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gausswatched.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/get_clause_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/get_clause_query.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/gqueuedata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/hasher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21346 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/hyperengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/hyperengine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/intree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/intree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/ipasir.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/lucky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/lucky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/main_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/matrixfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/matrixfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.925216 pyunigen-2.5.4/python/cryptominisat/src/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/msvc/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/mystack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/nomutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)   177386 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/occsimplifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/occsimplifier.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.925216 pyunigen-2.5.4/python/cryptominisat/src/oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/oracle/bitset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/oracle/oracle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/oracle/oracle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/oracle/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/packedmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/packedrow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/packedrow.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.929216 pyunigen-2.5.4/python/cryptominisat/src/picosat/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/picosat/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)   162828 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/picosat/picosat.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/picosat/picosat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/picosat/version.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/popcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/predict_func_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/propby.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/propby_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/propbyforgraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/propengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/propengine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/reducedb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/reducedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/satzilla_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/satzilla_features_calc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sccfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sccfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)   121913 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/searcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/searcher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/searchhist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/searchstats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/searchstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/shareddata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/signalcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/simplefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solutionextender.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solutionextender.h
+-rw-r--r--   0 runner    (1001) docker     (123)   168174 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solverconf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solverconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solvertypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/solvertypesmini.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sql_tablestructure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sqlitestats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/sqlstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/str_impl_w_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/str_impl_w_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/streambuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/subsumeimplicit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/subsumeimplicit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/subsumestrengthen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/subsumestrengthen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/time_mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/toplevelgauss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/toplevelgaussabst.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/touchlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/trim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/vardata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/vardistgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38447 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/varreplacer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/varreplacer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/varupdatehelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/vmtf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/watchalgos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/watcharray.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/watcharray_handrolled.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/watched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/xorfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-01 22:08:28.000000 pyunigen-2.5.4/python/cryptominisat/src/xorfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.929216 pyunigen-2.5.4/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-01 22:08:16.000000 pyunigen-2.5.4/python/src/GitSHA1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-05-01 22:08:16.000000 pyunigen-2.5.4/python/src/pyunigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:08:39.929216 pyunigen-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-01 22:08:16.000000 pyunigen-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.929216 pyunigen-2.5.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/config.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:08:39.929216 pyunigen-2.5.4/src/pyunigen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-01 22:08:39.000000 pyunigen-2.5.4/src/pyunigen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-01 22:08:39.000000 pyunigen-2.5.4/src/pyunigen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/sampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/sampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/time_mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/unigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-01 22:08:16.000000 pyunigen-2.5.4/src/unigen.h
```

### Comparing `pyunigen-2.5.3/LICENSE` & `pyunigen-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/PKG-INFO` & `pyunigen-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunigen
-Version: 2.5.3
+Version: 2.5.4
 Summary: Bindings to UniGen, an approximate sampler
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Meel Group
         Kuldeep Meel
```

### Comparing `pyunigen-2.5.3/README.md` & `pyunigen-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/pyproject.toml` & `pyunigen-2.5.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "toml", "pathlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyunigen"
-version = "2.5.3"
+version = "2.5.4"
 description = "Bindings to UniGen, an approximate sampler"
 keywords = ["sat", "model-counting"]
 license = { file = "LICENSE" }
 maintainers = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 authors = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pyunigen-2.5.3/python/README.md` & `pyunigen-2.5.4/python/README.md`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/python/src/GitSHA1.cpp` & `pyunigen-2.5.4/python/approxmc/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/GitSHA1.h` & `pyunigen-2.5.4/python/approxmc/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/approxmc.cpp` & `pyunigen-2.5.4/python/approxmc/src/approxmc.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/approxmc.h` & `pyunigen-2.5.4/python/approxmc/src/approxmc.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/config.h` & `pyunigen-2.5.4/python/approxmc/src/config.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/constants.cpp` & `pyunigen-2.5.4/python/approxmc/src/constants.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/constants.h` & `pyunigen-2.5.4/python/approxmc/src/constants.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/counter.cpp` & `pyunigen-2.5.4/python/approxmc/src/counter.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/counter.h` & `pyunigen-2.5.4/python/approxmc/src/counter.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/approxmc/src/time_mem.h` & `pyunigen-2.5.4/python/approxmc/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/python/src/GitSHA1.cpp` & `pyunigen-2.5.4/python/arjun/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/src/GitSHA1.h` & `pyunigen-2.5.4/python/arjun/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/src/MersenneTwister.h` & `pyunigen-2.5.4/python/arjun/src/MersenneTwister.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/src/arjun.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/ccnr_cms.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,469 +1,369 @@
-/*
- Arjun
+/******************************************
+Copyright (C) 2009-2020 Authors of CryptoMiniSat, see AUTHORS file <soos.mate@gmail.com>
 
- Copyright (c) 2020, Mate Soos and Kuldeep S. Meel. All rights reserved.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+***********************************************/
 
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in
- all copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
- THE SOFTWARE.
- */
-
-#include "arjun.h"
-#include "config.h"
-#include "common.h"
-#include "GitSHA1.h"
-#include <utility>
-#include <tuple>
+#include "time_mem.h"
 #include <limits>
+#include <cstdio>
+#include <cmath>
+#include <cstdlib>
+#include "constants.h"
+#include "ccnr_cms.h"
+#include "solver.h"
+#include "ccnr.h"
+#include "sqlstats.h"
+//#define SLOW_DEBUG
+
+using namespace CMSat;
+
+CMS_ccnr::CMS_ccnr(Solver* _solver) :
+    solver(_solver),
+    seen(_solver->seen),
+    toClear(_solver->toClear)
+{
+    ls_s = new CCNR::ls_solver(solver->conf.sls_ccnr_asipire);
+    ls_s->set_verbosity(solver->conf.verbosity);
+}
+
+CMS_ccnr::~CMS_ccnr()
+{
+    delete ls_s;
+}
+
+lbool CMS_ccnr::main(const uint32_t num_sls_called)
+{
+    //It might not work well with few number of variables
+    //rnovelty could also die/exit(-1), etc.
+    if (solver->nVars() < 50 ||
+        solver->binTri.irredBins + solver->longIrredCls.size() < 10
+    ) {
+        verb_print(1, "[ccnr] too few variables & clauses");
+        return l_Undef;
+    }
+    double startTime = cpuTime();
+
+    if (!init_problem()) {
+        //it's actually l_False under assumptions
+        //but we'll set the real SAT solver deal with that
+        if (solver->conf.verbosity) {
+            cout << "c [ccnr] problem UNSAT under assumptions, returning to main solver"
+            << endl;
+        }
+        return l_Undef;
+    }
 
-using std::pair;
-using std::numeric_limits;
-using namespace ArjunInt;
-
-#if defined _WIN32
-    #define DLL_PUBLIC __declspec(dllexport)
-#else
-    #define DLL_PUBLIC __attribute__ ((visibility ("default")))
-    #define DLL_LOCAL  __attribute__ ((visibility ("hidden")))
-#endif
-
-#define set_get_macro(TYPE, NAME) \
-DLL_PUBLIC void Arjun::set_##NAME (TYPE NAME) \
-{ \
-    arjdata->common.conf.NAME = NAME; \
-} \
-DLL_PUBLIC TYPE Arjun::get_##NAME () const \
-{ \
-    return arjdata->common.conf.NAME; \
-} \
-
-namespace ArjunNS {
-    struct ArjPrivateData {
-        Common common;
-    };
-}
-
-using namespace ArjunNS;
-
-
-DLL_PUBLIC Arjun::Arjun()
-{
-    arjdata = new ArjPrivateData;
-}
-
-DLL_PUBLIC Arjun::~Arjun()
-{
-    delete arjdata;
-}
-
-DLL_PUBLIC uint32_t Arjun::nVars() {
-    return arjdata->common.solver->nVars();
-}
-
-DLL_PUBLIC void Arjun::new_vars(uint32_t num)
-{
-    arjdata->common.solver->new_vars(num);
-}
+    vector<bool> phases(solver->nVars()+1);
+    for(uint32_t i = 0; i < solver->nVars(); i++) {
+        phases[i+1] = solver->varData[i].best_polarity;
+    }
 
-DLL_PUBLIC void Arjun::new_var()
-{
-    arjdata->common.solver->new_var();
-}
+    int res = ls_s->local_search(&phases, solver->conf.yalsat_max_mems*2*1000*1000);
+    lbool ret = deal_with_solution(res, num_sls_called);
 
-DLL_PUBLIC bool Arjun::add_clause(const vector<CMSat::Lit>& lits)
-{
-    return arjdata->common.solver->add_clause(lits);
-}
+    double time_used = cpuTime()-startTime;
+    if (solver->conf.verbosity) {
+        cout << "c [ccnr] time: " << time_used << endl;
+    }
+    if (solver->sqlStats) {
+        solver->sqlStats->time_passed_min(
+            solver
+            , "sls-ccnr"
+            , time_used
+        );
+    }
 
-DLL_PUBLIC bool Arjun::add_xor_clause(const vector<uint32_t>& vars, bool rhs)
-{
-    assert(false && "Funnily enough this does NOT work. The XORs would generate a BVA variable, and that would then not be returned as part of the simplified CNF. We could calculate a smaller independent set, but that's all.");
-    return arjdata->common.solver->add_xor_clause(vars, rhs);
+    return ret;
 }
 
-DLL_PUBLIC bool Arjun::add_bnn_clause(
-            const std::vector<CMSat::Lit>& lits,
-            signed cutoff,
-            Lit out
-        )
+template<class T>
+CMS_ccnr::add_cl_ret CMS_ccnr::add_this_clause(const T& cl)
 {
-    return arjdata->common.solver->add_bnn_clause(lits, cutoff, out);
-}
+    uint32_t sz = 0;
+    bool sat = false;
+    yals_lits.clear();
+    for(size_t i3 = 0; i3 < cl.size(); i3++) {
+        Lit lit = cl[i3];
+        assert(solver->varData[lit.var()].removed == Removed::none);
+        lbool val = l_Undef;
+        if (solver->value(lit) != l_Undef) {
+            val = solver->value(lit);
+        } else {
+            val = solver->lit_inside_assumptions(lit);
+        }
 
-DLL_PUBLIC uint32_t Arjun::set_starting_sampling_set(const vector<uint32_t>& vars)
-{
-    *arjdata->common.sampling_set = vars;
-    return arjdata->common.sampling_set->size();
-}
+        if (val == l_True) {
+            //clause is SAT, skip!
+            sat = true;
+            continue;
+        } else if (val == l_False) {
+            continue;
+        }
+        int l = lit.var()+1;
+        l *= lit.sign() ? -1 : 1;
+        yals_lits.push_back(l);
+        sz++;
+    }
+    if (sat) {
+        return add_cl_ret::skipped_cl;
+    }
+    if (sz == 0) {
+        //it's unsat because of assumptions
+        if (solver->conf.verbosity) {
+            cout << "c [walksat] UNSAT because of assumptions in clause: " << cl << endl;
+        }
+        return add_cl_ret::unsat;
+    }
 
-DLL_PUBLIC uint32_t Arjun::start_with_clean_sampling_set()
-{
-    arjdata->common.start_with_clean_sampling_set();
-    return arjdata->common.sampling_set->size();
-}
+    for(auto& lit: yals_lits) {
+        ls_s->_clauses[cl_num].literals.push_back(CCNR::lit(lit, cl_num));
+    }
+    cl_num++;
 
-DLL_PUBLIC string Arjun::get_version_info()
-{
-    return ArjunIntNS::get_version_sha1();
+    return add_cl_ret::added_cl;
 }
 
-DLL_PUBLIC std::string Arjun::get_solver_version_info()
+bool CMS_ccnr::init_problem()
 {
-    return CMSat::SATSolver::get_text_version_info();
-}
+    if (solver->check_assumptions_contradict_foced_assignment())
+    {
+        return false;
+    }
+    #ifdef SLOWDEBUG
+    solver->check_stats();
+    #endif
 
-DLL_PUBLIC std::string Arjun::get_compilation_env()
-{
-    return ArjunIntNS::get_compilation_env();
-}
+    ls_s->_num_vars = solver->nVars();
+    ls_s->_num_clauses = solver->longIrredCls.size() + solver->binTri.irredBins;
+    ls_s->make_space();
 
-DLL_PUBLIC const std::vector<Lit>& Arjun::get_orig_cnf()
-{
-    return arjdata->common.orig_cnf;
-}
+    vector<Lit> this_clause;
+    for(size_t i2 = 0; i2 < solver->nVars()*2; i2++) {
+        Lit lit = Lit::toLit(i2);
+        for(const Watched& w: solver->watches[lit]) {
+            if (w.isBin() && !w.red() && lit < w.lit2()) {
+                this_clause.clear();
+                this_clause.push_back(lit);
+                this_clause.push_back(w.lit2());
 
-template <class T>
-void check_sanity_sampling_vars(T vars, const uint32_t nvars)
-{
-    for(const auto& v: vars) if (v >= nvars) {
-        cout << "ERROR: sampling set provided is incorrect, it has a variable in it: " << v+1 << " that is larger than the total number of variables: " << nvars << endl;
-        exit(-1);
+                if (add_this_clause(this_clause) == add_cl_ret::unsat) {
+                    return false;
+                }
+            }
+        }
     }
-}
-
-DLL_PUBLIC vector<uint32_t> Arjun::get_indep_set()
-{
-    double starTime = cpuTime();
-    arjdata->common.orig_cnf = arjdata->common.get_cnf();
-    check_sanity_sampling_vars(*arjdata->common.sampling_set, get_orig_num_vars());
-    if (!arjdata->common.preproc_and_duplicate()) goto end;
+    for(ClOffset offs: solver->longIrredCls) {
+        const Clause* cl = solver->cl_alloc.ptr(offs);
+        assert(!cl->freed());
+        assert(!cl->getRemoved());
 
-    //Backward
-    if (arjdata->common.conf.backward) {
-        arjdata->common.backward_round();
+        if (add_this_clause(*cl) == add_cl_ret::unsat) {
+            return false;
+        }
     }
 
-    end:
-    arjdata->common.empty_out_indep_set_if_unsat();
-    if (arjdata->common.conf.verb) {
-        cout << "c [arjun] get_indep_set finished "
-        << "T: " << std::setprecision(2) << std::fixed << (cpuTime() - starTime)
-        << endl;
+    //Shrink the space if we have to
+    assert(ls_s->_num_clauses >= (int)cl_num);
+    ls_s->_num_clauses = (int)cl_num;
+    ls_s->make_space();
+
+    for (int c=0; c < ls_s->_num_clauses; c++) {
+        for(CCNR::lit item: ls_s->_clauses[c].literals) {
+            int v = item.var_num;
+            ls_s->_vars[v].literals.push_back(item);
+        }
     }
+    ls_s->build_neighborhood();
 
-    // Deal with empty_occs
-    arjdata->common.sampling_set->insert(
-        arjdata->common.sampling_set->begin(),
-        arjdata->common.empty_occs.begin(),
-        arjdata->common.empty_occs.end());
-
-    return *arjdata->common.sampling_set;
+    return true;
 }
 
-DLL_PUBLIC const vector<CMSat::BNN*>& Arjun::get_bnns() const
+struct ClWeightSorter
 {
-    return arjdata->common.solver->get_bnns();
-}
-
-DLL_PUBLIC void Arjun::start_getting_small_clauses(uint32_t max_len, uint32_t max_glue, bool red)
-{
-    arjdata->common.solver->start_getting_small_clauses(max_len, max_glue, red);
-}
-
-DLL_PUBLIC bool Arjun::get_next_small_clause(std::vector<CMSat::Lit>& ret)
-{
-    return arjdata->common.solver->get_next_small_clause(ret);
-}
+    bool operator()(const CCNR::clause& a, const CCNR::clause& b)
+    {
+        return a.weight > b.weight;
+    }
+};
 
-DLL_PUBLIC void Arjun::end_getting_small_clauses()
-{
-    arjdata->common.solver->end_getting_small_clauses();
-}
+struct VarAndVal {
+    VarAndVal(uint32_t _var, long long _score) :
+        var(_var),
+        val(_score)
+    {
+    }
+    uint32_t var;
+    long long val;
+};
 
-DLL_PUBLIC uint32_t Arjun::get_orig_num_vars() const
+struct VarValSorter
 {
-    if (arjdata->common.orig_num_vars == std::numeric_limits<uint32_t>::max()) {
-        return arjdata->common.solver->nVars();
+    bool operator()(const VarAndVal& a, const VarAndVal& b) {
+        return a.val > b.val;
     }
+};
 
-    return arjdata->common.orig_num_vars;
-}
-
-
-DLL_PUBLIC void Arjun::set_verbosity(uint32_t verb)
+vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_cls()
 {
-    arjdata->common.conf.verb = verb;
-    arjdata->common.solver->set_verbosity(verb);
-}
+    verb_print(1,"[ccnr] bumping based on clause weights");
 
-DLL_PUBLIC void Arjun::set_seed(uint32_t seed)
-{
-    arjdata->common.random_source.seed(seed);
-}
+    //Check prerequisites
+    assert(toClear.empty());
+    SLOW_DEBUG_DO(for(const auto x: seen) assert(x == 0));
 
-DLL_PUBLIC uint32_t Arjun::get_verbosity() const
-{
-    return arjdata->common.conf.verb;
-}
+    vector<pair<uint32_t, double>> tobump_cl_var;
+    std::sort(ls_s->_clauses.begin(), ls_s->_clauses.end(), ClWeightSorter());
+    uint32_t vars_bumped = 0;
+    uint32_t individual_vars_bumped = 0;
+    for(const auto& c: ls_s->_clauses) {
+        if (vars_bumped > solver->conf.sls_how_many_to_bump)
+            break;
 
-set_get_macro(bool, fast_backw)
-set_get_macro(bool, distill)
-set_get_macro(bool, intree)
-set_get_macro(bool, bve_pre_simplify)
-set_get_macro(bool, simp)
-set_get_macro(uint32_t, unknown_sort)
-set_get_macro(uint32_t, incidence_count)
-set_get_macro(bool, or_gate_based)
-set_get_macro(bool, xor_gates_based)
-set_get_macro(bool, probe_based)
-set_get_macro(bool, backward)
-set_get_macro(uint32_t, backw_max_confl)
-set_get_macro(uint64_t, backbone_simpl_max_confl)
-set_get_macro(bool, gauss_jordan)
-set_get_macro(bool, ite_gate_based)
-set_get_macro(bool, irreg_gate_based)
-set_get_macro(double, no_gates_below)
-set_get_macro(std::string, specified_order_fname)
-set_get_macro(bool, backbone_simpl)
-set_get_macro(bool, empty_occs_based)
-set_get_macro(bool, bce)
+        for(uint32_t i = 0; i < c.literals.size(); i++) {
+            uint32_t v = c.literals[i].var_num-1;
+            if (v < solver->nVars() &&
+                solver->varData[v].removed == Removed::none &&
+                solver->value(v) == l_Undef &&
+                seen[v] < solver->conf.sls_bump_var_max_n_times)
+            {
+                if (seen[v] == 0) individual_vars_bumped++;
+                seen[v]++;
+                toClear.push_back(Lit(v, false));
+                tobump_cl_var.push_back(std::make_pair(v, 3.0));
+                vars_bumped++;
+            }
+        }
+    }
 
-DLL_PUBLIC vector<uint32_t> Arjun::get_empty_occ_sampl_vars() const
-{
-    return arjdata->common.empty_occs;
-}
+    for(const auto x: toClear) seen[x.var()] = 0;
+    toClear.clear();
 
-DLL_PUBLIC void Arjun::set_pred_forever_cutoff(int pred_forever_cutoff)
-{
-    arjdata->common.solver->set_pred_forever_cutoff(pred_forever_cutoff);
+    return tobump_cl_var;
 }
 
-DLL_PUBLIC void Arjun::set_every_pred_reduce(int every_pred_reduce)
+vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_var_scores()
 {
-    arjdata->common.solver->set_every_pred_reduce(every_pred_reduce);
-}
-
-DLL_PUBLIC vector<Lit> Arjun::get_zero_assigned_lits() const
-{
-    vector<Lit> ret;
-    vector<Lit> lits = arjdata->common.solver->get_zero_assigned_lits();
-    for(const auto& lit: lits) {
-        if (lit.var() < arjdata->common.orig_num_vars) {
-            ret.push_back(lit);
-        }
+    vector<VarAndVal> vs;
+    for(uint32_t i = 1; i < ls_s->_vars.size(); i++) {
+        vs.push_back(VarAndVal(i-1, ls_s->_vars[i].score));
     }
+    std::sort(vs.begin(), vs.end(), VarValSorter());
 
-    return ret;
+    vector<pair<uint32_t, double>> tobump;
+    for(uint32_t i = 0; i < solver->conf.sls_how_many_to_bump; i++) {
+//         cout << "var: " << vs[i].var + 1 << " score: " <<  vs[i].val << endl;
+        tobump.push_back(std::make_pair(vs[i].var, 3.0));
+    }
+    return tobump;
 }
 
-DLL_PUBLIC std::vector<std::pair<CMSat::Lit, CMSat::Lit> > Arjun::get_all_binary_xors() const
+vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_conflict_ct()
 {
-    vector<pair<Lit, Lit>> ret;
-    const auto bin_xors = arjdata->common.solver->get_all_binary_xors();
-    for(const auto& bx: bin_xors) {
-        if (bx.first.var() < arjdata->common.orig_num_vars &&
-            bx.second.var() < arjdata->common.orig_num_vars)
-        {
-            ret.push_back(bx);
-        }
+    if (solver->conf.verbosity) {
+        cout << "c [ccnr] bumping based on var unsat frequency: conflict_ct" << endl;
     }
 
-    return ret;
-}
+    vector<pair<uint32_t, double>> tobump;
+    int mymax = 0;
+    for(uint32_t i = 1; i < ls_s->_conflict_ct.size(); i++) {
+        mymax = std::max(mymax, ls_s->_conflict_ct[i]);
+    }
 
-DLL_PUBLIC void Arjun::varreplace()
-{
-    //arjdata->common.solver->backbone_simpl();
-    std::string tmp("must-scc-vrepl, cl-consolidate");
-    arjdata->common.solver->simplify(NULL, &tmp);
+    for(uint32_t i = 1; i < ls_s->_conflict_ct.size(); i++) {
+        double val = ls_s->_conflict_ct[i];
+        if (mymax > 0) {
+            tobump.push_back(std::make_pair(i-1, (double)val/(double)mymax * 3.0));
+        } else {
+            tobump.push_back(std::make_pair(i-1, 0));
+        }
+//         if (tobump.back().second > 0) {
+//             cout << "var: " << tobump.back().first << " bump by: " << tobump.back().second << endl;
+//         }
+    }
+    return tobump;
 }
 
-DLL_PUBLIC const vector<Lit> Arjun::get_internal_cnf(uint32_t& num_cls) const
+lbool CMS_ccnr::deal_with_solution(int res, const uint32_t num_sls_called)
 {
-    vector<Lit> cnf;
-    bool ret = true;
-    num_cls = 0;
-
-    arjdata->common.solver->start_getting_small_clauses(
-        std::numeric_limits<uint32_t>::max(),
-        std::numeric_limits<uint32_t>::max(),
-        false);
-    vector<Lit> clause;
-    while (ret) {
-        ret = arjdata->common.solver->get_next_small_clause(clause);
-        if (!ret) break;
-
-        bool ok = true;
-        for(auto l: clause) {
-            if (l.var() >= arjdata->common.orig_num_vars) {
-                ok = false;
-                break;
-            }
+    if (solver->conf.sls_get_phase || res) {
+        if (solver->conf.verbosity) {
+            cout
+            << "c [ccnr] saving best assignment phase to stable_polar";
+            if (res) cout << " + best_polar";
+            cout << endl;
         }
 
-        if (ok) {
-            for(auto const& l: clause) cnf.push_back(l);
-            cnf.push_back(lit_Undef);
-            num_cls++;
+        for(size_t i = 0; i < solver->nVars(); i++) {
+            solver->varData[i].stable_polarity = ls_s->_best_solution[i+1];
+            if (res) {
+                solver->varData[i].best_polarity = ls_s->_best_solution[i+1];
+            }
         }
     }
-    arjdata->common.solver->end_getting_small_clauses();
-    return cnf;
-}
 
-static void get_simplified_cnf(
-        SATSolver* solver, vector<uint32_t>& sampl_vars, const bool renumber,
-        vector<vector<Lit>>& cnf, uint32_t& nvars)
-{
-    assert(cnf.empty());
-    solver->start_getting_small_clauses(
-        std::numeric_limits<uint32_t>::max(),
-        std::numeric_limits<uint32_t>::max(),
-        false, //red
-        false, //bva vars
-        renumber); //simplified
-    if (renumber) sampl_vars = solver->translate_sampl_set(sampl_vars);
-
-    bool ret = true;
-    vector<Lit> clause;
-    while(ret) {
-        ret = solver->get_next_small_clause(clause);
-        if (ret) {
-            cnf.push_back(clause);
-        }
+    //Clause score sorting
+    vector<pair<uint32_t, double>> tobump;
+    switch (solver->conf.sls_bump_type) {
+        case 1:
+            tobump = get_bump_based_on_cls();
+            break;
+        case 2:
+            assert(false && "Does not work, removed");
+            break;
+        case 3:
+            tobump = get_bump_based_on_var_scores();
+            break;
+        case 4:
+            tobump = get_bump_based_on_conflict_ct();
+            break;
+        case 5:
+            if (num_sls_called % 3 == 0) {
+                tobump = get_bump_based_on_conflict_ct();
+            } else {
+                tobump = get_bump_based_on_cls();
+            }
+            break;
+        case 6:
+            if (num_sls_called % 3 == 0) {
+                tobump = get_bump_based_on_cls();
+            } else {
+                tobump = get_bump_based_on_conflict_ct();
+            }
+            break;
+        default:
+            assert(false && "No such SLS bump type");
+            exit(-1);
     }
-    solver->end_getting_small_clauses();
-    nvars = renumber ? solver->simplified_nvars() :  solver->nVars();
-}
 
-static void fill_solver(
-    SATSolver& solver,
-    Arjun* arjun)
-{
-    assert(solver.nVars() == 0); // Solver here is empty
-    solver.new_vars(arjun->get_orig_num_vars());
-
-    // Inject original CNF
-    const auto cnf = arjun->get_orig_cnf();
-    vector<Lit> cl;
-    for(const auto& l: cnf) {
-        if (l != lit_Undef) {
-            assert(l.var() < arjun->get_orig_num_vars());
-            cl.push_back(l);
-            continue;
-        }
-        solver.add_clause(cl);
-        cl.clear();
-    }
 
-    // inject set vars
-    const auto lits =  arjun->get_zero_assigned_lits();
-    for(const auto& l: lits) {
-        if (l.var() < arjun->get_orig_num_vars()) {
-            cl.clear();
-            cl.push_back(l);
-            solver.add_clause(cl);
-        }
+    for(const auto& v: tobump) solver->bump_var_importance_all(v.first);
+    if (solver->branch_strategy == branch::vsids) {
+        solver->vsids_decay_var_act();
     }
 
-    // inject bin-xor clauses
-    auto bin_xors = arjun->get_all_binary_xors();
-    vector<uint32_t> dummy_v;
-    for(const auto& bx: bin_xors) {
-        dummy_v.clear();
-        dummy_v.push_back(bx.first.var());
-        dummy_v.push_back(bx.second.var());
-        solver.add_xor_clause(dummy_v, bx.first.sign()^bx.second.sign());
-    }
-}
 
-DLL_PUBLIC SimplifiedCNF Arjun::get_fully_simplified_renumbered_cnf(
-    const vector<uint32_t>& sampl_vars, //contains empty_vars!
-    const bool sparsify,
-    const bool renumber,
-    const bool need_sol_extend)
-{
-    CMSat::SATSolver solver;
-    solver.set_verbosity(arjdata->common.conf.verb);
-    solver.set_renumber(renumber);
-    solver.set_scc(renumber);
-
-    // Create a new SAT solver that contains no empties.
-    // dont_elim now how no empties in it
-    fill_solver(solver, this);
-    vector<Lit> dont_elim;
-    for(uint32_t v: sampl_vars) dont_elim.push_back(Lit(v, false));
-
-    //Below works VERY WELL for: ProcessBean, pollard, track1_116.mcc2020_cnf
-    //   and blasted_TR_b14_even3_linear.cnf.gz.no_w.cnf
-    //with CMS ef6ea7e87e00bde50c0cce0c1e13a012191c4e1c and Arjun 5f2dfe814e07ee6ee0dde65b1350b5c343209ed0
-    solver.set_min_bva_gain(0);
-    solver.set_varelim_check_resolvent_subs(true);
-    solver.set_max_red_linkin_size(0);
-    solver.set_timeout_all_calls(100);
-    solver.set_weaken_time_limitM(2000);
-    solver.set_occ_based_lit_rem_time_limitM(500);
-
-    // occ-ternary-res not used
-    // eqlit-find ? (too slow)
-    string str("full-probe, sub-cls-with-bin, must-scc-vrepl, must-scc-vrepl, distill-cls-onlyrem, sub-impl, occ-resolv-subs, occ-del-elimed, occ-backw-sub, occ-rem-with-orgates, occ-bve, occ-ternary-res, ");
-    solver.simplify(&dont_elim, &str);
-
-    string str2;
-    if (arjdata->common.conf.bce) str2 += "occ-bce,";
-    str = str2 + string("intree-probe, occ-backw-sub-str, sub-str-cls-with-bin, clean-cls, distill-cls,distill-bins, ") + str;
-
-    solver.simplify(&dont_elim, &str);
-    solver.simplify(&dont_elim, &str);
-    solver.simplify(&dont_elim, &str);
-    if (sparsify) {
-        str2.clear();
-        if (arjdata->common.conf.bce) str2+= "occ-bce,";
-        str2 += string("sparsify,") + str;
-        solver.simplify(&dont_elim, &str2);
-    }
-    //one more without sparsify
-    solver.simplify(&dont_elim, &str);
-
-    str.clear();
-    if (arjdata->common.definitely_satisfiable) {
-        str += string("occ-rem-unconn-assumps, ");
-    }
-    str += string(", must-scc-vrepl, must-renumber,");
-    if (arjdata->common.conf.bce) str += "occ-bce,";
-    solver.simplify(&dont_elim, &str);
-
-    vector<uint32_t> new_sampl_vars (sampl_vars);
-    vector<uint32_t> empty_occs;
-    SimplifiedCNF cnf;
-    if (arjdata->common.conf.empty_occs_based) {
-        solver.clean_sampl_and_get_empties(new_sampl_vars, empty_occs);
-        dont_elim.clear();
-        for(uint32_t v: new_sampl_vars) dont_elim.push_back(Lit(v, false));
-        str = "occ-bve-empty, must-renumber";
-        solver.simplify(&dont_elim, &str);
-    }
-    get_simplified_cnf(&solver, new_sampl_vars, renumber, cnf.cnf, cnf.nvars);
-
-    std::sort(new_sampl_vars.begin(), new_sampl_vars.end());
-    cnf.sampling_vars = new_sampl_vars;
-    cnf.empty_occs = empty_occs.size();
-    if (need_sol_extend) cnf.sol_ext_data = solver.serialize_solution_reconstruction_data();
+    verb_print(1, "[ccnr] Bumped vars: " << tobump.size()
+        << " bump type: " << solver->conf.sls_bump_type);
 
-    return cnf;
-}
+    if (!res) verb_print(2, "[ccnr] ASSIGNMENT NOT FOUND");
+    else verb_print(1, "[ccnr] ASSIGNMENT FOUND");
 
+    return l_Undef;
+}
```

### Comparing `pyunigen-2.5.3/python/arjun/src/arjun.h` & `pyunigen-2.5.4/python/arjun/src/arjun.h`

 * *Files 8% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         //void set_polar_mode(CMSat::PolarityMode mode);
         void set_no_gates_below(double no_gates_below);
         void set_pred_forever_cutoff(int pred_forever_cutoff = -1);
         void set_every_pred_reduce(int every_pred_reduce = -1);
         void set_empty_occs_based(const bool empty_occs_based);
         void set_specified_order_fname(std::string specified_order_fname);
         void set_bce(const bool bce);
+        void set_bve_during_elimtofile(const bool);
+        void set_backbone_simpl_cmsgen(const bool);
 
         //Get config
         bool get_empty_occs_based() const;
         std::string get_specified_order_fname() const;
         double get_no_gates_below() const;
         bool get_simp() const;
         uint32_t get_verbosity() const;
@@ -150,14 +152,16 @@
         bool get_find_xors() const;
         bool get_backbone_simpl() const;
         bool get_ite_gate_based() const;
         bool get_irreg_gate_based() const;
         bool get_gate_sort_special() const;
         uint64_t get_backbone_simpl_max_confl() const;
         bool get_bce() const;
+        bool get_bve_during_elimtofile() const;
+        bool get_backbone_simpl_cmsgen() const;
 
     private:
         ArjPrivateData* arjdata = NULL;
     };
 }
 
 #endif
```

### Comparing `pyunigen-2.5.3/python/arjun/src/backward.cpp` & `pyunigen-2.5.4/python/arjun/src/backward.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/src/common.cpp` & `pyunigen-2.5.4/python/arjun/src/common.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/arjun/src/common.h` & `pyunigen-2.5.4/python/arjun/src/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,14 @@
     bool simplify();
     bool remove_definable_by_gates();
     void remove_definable_by_irreg_gates();
     void remove_zero_assigned_literals(bool print = true);
     void remove_eq_literals(bool print = true);
     void find_equiv_subformula();
     bool probe_all();
-    bool backbone_simpl();
     void empty_out_indep_set_if_unsat();
     bool simplify_bve_only();
     bool run_gauss_jordan();
     void check_no_duplicate_in_sampling_set();
     void order_sampl_set_for_simp();
 
     //backward
```

### Comparing `pyunigen-2.5.3/python/arjun/src/config.h` & `pyunigen-2.5.4/python/arjun/src/config.h`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,21 @@
     int xor_gates_based = 1;
     int ite_gate_based = 1;
     int irreg_gate_based = 1;
     int empty_occs_based = 1;
     int probe_based = 1;
     int backward = 1;
     int gauss_jordan = 0;
-    int backbone_simpl = 0;
+    int backbone_simpl = 1;
+    int backbone_simpl_cmsgen = 1;
+    uint64_t backbone_simpl_max_confl = 20ULL*1000ULL;
     int bce = 0;
     double no_gates_below = 0.01;
     std::string specified_order_fname;
-    unsigned long backbone_simpl_max_confl = 10ULL*1000ULL;
     uint32_t backw_max_confl = 5000;
+    int bve_during_elimtofile = true;
 };
 
 }
 
 //ARJUN_CONFIG_H
 #endif
```

### Comparing `pyunigen-2.5.3/python/arjun/src/simplify.cpp` & `pyunigen-2.5.4/python/arjun/src/simplify.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -69,24 +69,20 @@
         solver->set_intree_probe(1);
         if (solver->simplify() == l_False) return false;
         solver->set_intree_probe(conf.intree);
         verb_print(1,"[arjun-simp] CMS::simplify() with no BVE finished."
             << " T: " << (cpuTime() - simpTime));
     }
 
-    if (conf.backbone_simpl) {
-        if (!backbone_simpl()) return false;
-    } else {
-        // Find at least one solution (so it's not UNSAT) within some timeout
-        solver->set_verbosity(0);
-        solver->set_max_confl(1000);
-        lbool ret = solver->solve();
-        if (ret == l_True) definitely_satisfiable = true;
-        solver->set_verbosity(std::max<int>(conf.verb-2, 0));
-    }
+    // Find at least one solution (so it's not UNSAT) within some timeout
+    solver->set_verbosity(0);
+    solver->set_max_confl(1000);
+    lbool ret = solver->solve();
+    if (ret == l_True) definitely_satisfiable = true;
+    solver->set_verbosity(std::max<int>(conf.verb-2, 0));
 
     remove_eq_literals();
     remove_zero_assigned_literals();
     if (conf.probe_based && !probe_all()) return false;
     if (conf.empty_occs_based) find_equiv_subformula();
     if (conf.irreg_gate_based) remove_definable_by_irreg_gates();
 
@@ -98,135 +94,14 @@
         << stats_line_percent(old_size-sampling_set->size(), old_size)
         << " T: " << (cpuTime() - myTime));
 
     check_no_duplicate_in_sampling_set();
     return true;
 }
 
-bool Common::backbone_simpl()
-{
-    if (conf.verb) {
-        cout << "c [backbone-simpl] starting backbone simplification..." << endl;
-    }
-    uint64_t last_sum_conflicts = 0;
-    int64_t max_confl = conf.backbone_simpl_max_confl;
-
-    solver->set_verbosity(0);
-    double myTime = cpuTime();
-    uint32_t orig_vars_set = solver->get_zero_assigned_lits().size();
-    bool finished = false;
-    Lit l;
-
-    vector<Lit> tmp_clause;
-    vector<Lit> assumps;
-    vector<lbool> model;
-    vector<char> model_enabled;
-    const auto old_polar_mode = solver->get_polarity_mode();
-    solver->set_polarity_mode(PolarityMode::polarmode_neg);
-
-    vector<Lit> zero_set = solver->get_zero_assigned_lits();
-    for(auto const& l2: zero_set) seen[l2.var()] = 1;
-    for(auto const& v: empty_occs) seen[v] = 1;
-    vector<uint32_t> var_order;
-    for(uint32_t i = 0, max = solver->nVars(); i < max; i++) {
-        if (seen[i]) continue;
-        var_order.push_back(i);
-    }
-    for(auto const& l2: zero_set) seen[l2.var()] = 0;
-    for(auto const& v: empty_occs) seen[v] = 0;
-    if (var_order.empty()) return true;
-
-    std::mt19937 g;
-    g.seed(1337);
-    std::shuffle(var_order.begin(), var_order.end(), g);
-
-    solver->set_max_confl(max_confl);
-//     cout << "c [backbone] sum conf: " << solver->get_sum_conflicts() << endl;
-    max_confl -= solver->get_sum_conflicts();
-    last_sum_conflicts = solver->get_sum_conflicts();
-    lbool ret = solver->solve();
-    if (ret == l_False) {
-        return false;
-    }
-    if (ret == l_Undef || max_confl < 0) {
-        goto end;
-    }
-
-    model = solver->get_model();
-    model_enabled.resize(solver->nVars(), 1);
-
-    for(const uint32_t var: var_order) {
-        if (!model_enabled[var]) {
-            continue;
-        }
-
-        l = Lit(var, model[var] == l_False);
-
-        //There is definitely a solution with "l". Let's see if ~l fails.
-        assumps.clear();
-        assumps.push_back(~l);
-//         cout << "c [backbone]  assumps: " << endl;
-//         for (auto const& l2: assumps) cout << l2 << " , ";
-//         cout << " -- sum conf: " << solver->get_sum_conflicts() << endl;
-        solver->set_max_confl(max_confl);
-        ret = solver->solve(&assumps);
-
-        //Update max confl
-        assert(last_sum_conflicts <= solver->get_sum_conflicts());
-        max_confl -= ((int64_t)solver->get_sum_conflicts() - last_sum_conflicts);
-        max_confl -= 100;
-        last_sum_conflicts = solver->get_sum_conflicts();
-//         cout << "max_confl: " << max_confl << endl;
-
-        //Check return value
-        if (ret == l_True) {
-            const auto& this_model = solver->get_model();
-            for(uint32_t i2 = 0, max = solver->nVars(); i2 < max; i2++) {
-                if (this_model[i2] != model[i2]) {
-                    model_enabled[i2] = 0;
-                }
-            }
-        } else if (ret == l_False) {
-            tmp_clause.clear();
-            tmp_clause.push_back(l);
-            if (!solver->add_clause(tmp_clause)) {
-                return false;
-            }
-        }
-        if (ret == l_Undef || max_confl < 0) {
-            goto end;
-        }
-    }
-    finished = true;
-    assert(solver->okay());
-
-    end:
-    uint32_t num_set = solver->get_zero_assigned_lits().size() - orig_vars_set;
-    double time_used = cpuTime() - myTime;
-    solver->set_polarity_mode(old_polar_mode);
-
-    if (conf.verb) {
-        if (!finished) {
-            cout << "c [backbone-simpl] "
-            << "skipping, taking more than max conflicts:"
-            << print_value_kilo_mega(conf.backbone_simpl_max_confl)
-            << endl;
-        }
-        cout << "c [backbone-simpl]"
-        << " set: " << num_set
-        << " conflicts used: " << print_value_kilo_mega(solver->get_sum_conflicts())
-        << " conflicts max: " << print_value_kilo_mega(conf.backbone_simpl_max_confl)
-        << " T: " << std::setprecision(2) << time_used
-        << endl;
-    }
-    solver->set_verbosity(std::max<int>(conf.verb-2, 0));
-
-    return true;
-}
-
 void Common::empty_out_indep_set_if_unsat()
 {
     if (solver->okay()) return;
 
     //It's UNSAT so the sampling set is empty
     other_sampling_set->clear();
     std::swap(sampling_set, other_sampling_set);
```

### Comparing `pyunigen-2.5.3/python/arjun/src/time_mem.h` & `pyunigen-2.5.4/python/arjun/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/python/src/GitSHA1.cpp` & `pyunigen-2.5.4/python/cryptominisat/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/GitSHA1.h` & `pyunigen-2.5.4/python/cryptominisat/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/MersenneTwister.h` & `pyunigen-2.5.4/python/cryptominisat/src/MersenneTwister.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/Vec.h` & `pyunigen-2.5.4/python/cryptominisat/src/Vec.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/XAlloc.h` & `pyunigen-2.5.4/python/cryptominisat/src/XAlloc.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/alg.h` & `pyunigen-2.5.4/python/cryptominisat/src/alg.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/avgcalc.h` & `pyunigen-2.5.4/python/cryptominisat/src/avgcalc.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/bitarray.h` & `pyunigen-2.5.4/python/cryptominisat/src/bitarray.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/boundedqueue.h` & `pyunigen-2.5.4/python/cryptominisat/src/boundedqueue.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/bva.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/bva.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/bva.h` & `pyunigen-2.5.4/python/cryptominisat/src/bva.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cardfinder.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/cardfinder.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cardfinder.h` & `pyunigen-2.5.4/python/cryptominisat/src/cardfinder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ccnr.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/ccnr.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ccnr.h` & `pyunigen-2.5.4/python/cryptominisat/src/ccnr.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ccnr_cms.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/gatefinder.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /******************************************
-Copyright (C) 2009-2020 Authors of CryptoMiniSat, see AUTHORS file <soos.mate@gmail.com>
+Copyright (C) 2009-2020 Authors of CryptoMiniSat, see AUTHORS file
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -16,354 +16,359 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
+#include "gatefinder.h"
 #include "time_mem.h"
-#include <limits>
-#include <cstdio>
-#include <cmath>
-#include <cstdlib>
-#include "constants.h"
-#include "ccnr_cms.h"
 #include "solver.h"
-#include "ccnr.h"
+#include "occsimplifier.h"
+#include "subsumestrengthen.h"
+#include "clauseallocator.h"
+#include <array>
+#include <utility>
 #include "sqlstats.h"
-//#define SLOW_DEBUG
 
 using namespace CMSat;
+using std::cout;
+using std::endl;
 
-CMS_ccnr::CMS_ccnr(Solver* _solver) :
-    solver(_solver),
-    seen(_solver->seen),
-    toClear(_solver->toClear)
+GateFinder::GateFinder(OccSimplifier *_simplifier, Solver *_solver) :
+    numDotPrinted(0)
+    , simplifier(_simplifier)
+    , solver(_solver)
+    , seen(_solver->seen)
+    , seen2(_solver->seen2)
+    , toClear(solver->toClear)
 {
-    ls_s = new CCNR::ls_solver(solver->conf.sls_ccnr_asipire);
-    ls_s->set_verbosity(solver->conf.verbosity);
+//     sizeSortedOcc.resize(solver->conf.maxGateBasedClReduceSize+1);
 }
 
-CMS_ccnr::~CMS_ccnr()
+void GateFinder::cleanup()
 {
-    delete ls_s;
+    solver->clean_occur_from_idx_types_only_smudged();
+    orGates.clear();
 }
 
-lbool CMS_ccnr::main(const uint32_t num_sls_called)
+void GateFinder::find_all()
 {
-    //It might not work well with few number of variables
-    //rnovelty could also die/exit(-1), etc.
-    if (solver->nVars() < 50 ||
-        solver->binTri.irredBins + solver->longIrredCls.size() < 10
-    ) {
-        verb_print(1, "[ccnr] too few variables & clauses");
-        return l_Undef;
-    }
-    double startTime = cpuTime();
-
-    if (!init_problem()) {
-        //it's actually l_False under assumptions
-        //but we'll set the real SAT solver deal with that
-        if (solver->conf.verbosity) {
-            cout << "c [ccnr] problem UNSAT under assumptions, returning to main solver"
-            << endl;
-        }
-        return l_Undef;
-    }
+    runStats.clear();
+    orGates.clear();
 
-    vector<bool> phases(solver->nVars()+1);
-    for(uint32_t i = 0; i < solver->nVars(); i++) {
-        phases[i+1] = solver->varData[i].best_polarity;
-    }
+    assert(solver->watches.get_smudged_list().empty());
+    find_or_gates_and_update_stats();
+    if (solver->conf.doPrintGateDot) print_graphviz_dot();
+    VERBOSE_DEBUG_DO(for(auto g: orGates) cout << "found: OR gate" << g << endl;);
+
+    if (solver->conf.verbosity >= 3) runStats.print(solver->nVars());
+    globalStats += runStats;
+    solver->sumSearchStats.num_gates_found_last = orGates.size();
+}
 
-    int res = ls_s->local_search(&phases, solver->conf.yalsat_max_mems*2*1000*1000);
-    lbool ret = deal_with_solution(res, num_sls_called);
+void GateFinder::find_or_gates_and_update_stats()
+{
+    assert(solver->ok);
 
-    double time_used = cpuTime()-startTime;
-    if (solver->conf.verbosity) {
-        cout << "c [ccnr] time: " << time_used << endl;
-    }
+    double myTime = cpuTime();
+    const int64_t orig_numMaxGateFinder =
+        solver->conf.gatefinder_time_limitM*100LL*1000LL
+        *solver->conf.global_timeout_multiplier;
+    numMaxGateFinder = orig_numMaxGateFinder;
+    simplifier->limit_to_decrease = &numMaxGateFinder;
+
+    find_or_gates();
+    runStats.gatesSize += 2*orGates.size();
+    runStats.num+=orGates.size();
+
+    const double time_used = cpuTime() - myTime;
+    const bool time_out = (numMaxGateFinder <= 0);
+    const double time_remain = float_div(numMaxGateFinder, orig_numMaxGateFinder);
+    runStats.findGateTime = time_used;
+    runStats.find_gate_timeout = time_out;
     if (solver->sqlStats) {
-        solver->sqlStats->time_passed_min(
+        solver->sqlStats->time_passed(
             solver
-            , "sls-ccnr"
+            , "gate find"
             , time_used
+            , time_out
+            , time_remain
         );
     }
 
-    return ret;
+    verb_print(1, "[occ-gates]"
+        << " found: " << print_value_kilo_mega(runStats.num)
+        << " avg-s: " << std::fixed << std::setprecision(1)
+        << float_div(runStats.gatesSize, runStats.num)
+        /*<< " avg-s: " << std::fixed << std::setprecision(1)
+        << float_div(learntGatesSize, numRed)*/
+        << solver->conf.print_times(time_used, time_out, time_remain));
 }
 
-template<class T>
-CMS_ccnr::add_cl_ret CMS_ccnr::add_this_clause(const T& cl)
+struct IncidenceSorter
 {
-    uint32_t sz = 0;
-    bool sat = false;
-    yals_lits.clear();
-    for(size_t i3 = 0; i3 < cl.size(); i3++) {
-        Lit lit = cl[i3];
-        assert(solver->varData[lit.var()].removed == Removed::none);
-        lbool val = l_Undef;
-        if (solver->value(lit) != l_Undef) {
-            val = solver->value(lit);
-        } else {
-            val = solver->lit_inside_assumptions(lit);
-        }
+    IncidenceSorter(const vector<uint32_t>& _inc) :
+        inc(_inc)
+    {}
 
-        if (val == l_True) {
-            //clause is SAT, skip!
-            sat = true;
-            continue;
-        } else if (val == l_False) {
-            continue;
-        }
-        int l = lit.var()+1;
-        l *= lit.sign() ? -1 : 1;
-        yals_lits.push_back(l);
-        sz++;
-    }
-    if (sat) {
-        return add_cl_ret::skipped_cl;
-    }
-    if (sz == 0) {
-        //it's unsat because of assumptions
-        if (solver->conf.verbosity) {
-            cout << "c [walksat] UNSAT because of assumptions in clause: " << cl << endl;
-        }
-        return add_cl_ret::unsat;
+    bool operator()(const uint32_t a, const uint32_t b) {
+        return inc[a] < inc[b];
     }
 
-    for(auto& lit: yals_lits) {
-        ls_s->_clauses[cl_num].literals.push_back(CCNR::lit(lit, cl_num));
-    }
-    cl_num++;
-
-    return add_cl_ret::added_cl;
-}
+    const vector<uint32_t>& inc;
+};
 
-bool CMS_ccnr::init_problem()
+void GateFinder::find_or_gates()
 {
-    if (solver->check_assumptions_contradict_foced_assignment())
-    {
-        return false;
-    }
-    #ifdef SLOWDEBUG
-    solver->check_stats();
-    #endif
-
-    ls_s->_num_vars = solver->nVars();
-    ls_s->_num_clauses = solver->longIrredCls.size() + solver->binTri.irredBins;
-    ls_s->make_space();
-
-    vector<Lit> this_clause;
-    for(size_t i2 = 0; i2 < solver->nVars()*2; i2++) {
-        Lit lit = Lit::toLit(i2);
-        for(const Watched& w: solver->watches[lit]) {
-            if (w.isBin() && !w.red() && lit < w.lit2()) {
-                this_clause.clear();
-                this_clause.push_back(lit);
-                this_clause.push_back(w.lit2());
-
-                if (add_this_clause(this_clause) == add_cl_ret::unsat) {
-                    return false;
-                }
-            }
-        }
-    }
-    for(ClOffset offs: solver->longIrredCls) {
-        const Clause* cl = solver->cl_alloc.ptr(offs);
-        assert(!cl->freed());
-        assert(!cl->getRemoved());
-
-        if (add_this_clause(*cl) == add_cl_ret::unsat) {
-            return false;
-        }
-    }
+    if (solver->nVars() < 1)
+        return;
 
-    //Shrink the space if we have to
-    assert(ls_s->_num_clauses >= (int)cl_num);
-    ls_s->_num_clauses = (int)cl_num;
-    ls_s->make_space();
-
-    for (int c=0; c < ls_s->_num_clauses; c++) {
-        for(CCNR::lit item: ls_s->_clauses[c].literals) {
-            int v = item.var_num;
-            ls_s->_vars[v].literals.push_back(item);
-        }
+    const size_t offs = solver->mtrand.randInt(solver->nVars()*2-1);
+    for(size_t i = 0
+        ; i < solver->nVars()*2
+            && *simplifier->limit_to_decrease > 0
+            && !solver->must_interrupt_asap()
+        ; i++
+    ) {
+        const size_t at = (offs + i) % (solver->nVars()*2);
+        const Lit lit = Lit::toLit(at);
+        find_or_gates_in_sweep_mode(lit);
+        find_or_gates_in_sweep_mode(~lit);
     }
-    ls_s->build_neighborhood();
-
-    return true;
 }
 
-struct ClWeightSorter
+void GateFinder::find_or_gates_in_sweep_mode(const Lit lit)
 {
-    bool operator()(const CCNR::clause& a, const CCNR::clause& b)
-    {
-        return a.weight > b.weight;
-    }
-};
-
-struct VarAndVal {
-    VarAndVal(uint32_t _var, long long _score) :
-        var(_var),
-        val(_score)
-    {
-    }
-    uint32_t var;
-    long long val;
-};
-
-struct VarValSorter
-{
-    bool operator()(const VarAndVal& a, const VarAndVal& b) {
-        return a.val > b.val;
-    }
-};
-
-vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_cls()
-{
-    verb_print(1,"[ccnr] bumping based on clause weights");
-
-    //Check prerequisites
     assert(toClear.empty());
-    SLOW_DEBUG_DO(for(const auto x: seen) assert(x == 0));
 
-    vector<pair<uint32_t, double>> tobump_cl_var;
-    std::sort(ls_s->_clauses.begin(), ls_s->_clauses.end(), ClWeightSorter());
-    uint32_t vars_bumped = 0;
-    uint32_t individual_vars_bumped = 0;
-    for(const auto& c: ls_s->_clauses) {
-        if (vars_bumped > solver->conf.sls_how_many_to_bump)
-            break;
-
-        for(uint32_t i = 0; i < c.literals.size(); i++) {
-            uint32_t v = c.literals[i].var_num-1;
-            if (v < solver->nVars() &&
-                solver->varData[v].removed == Removed::none &&
-                solver->value(v) == l_Undef &&
-                seen[v] < solver->conf.sls_bump_var_max_n_times)
-            {
-                if (seen[v] == 0) individual_vars_bumped++;
-                seen[v]++;
-                toClear.push_back(Lit(v, false));
-                tobump_cl_var.push_back(std::make_pair(v, 3.0));
-                vars_bumped++;
+    //From the clauses
+    //a V -b
+    //a V -c
+    //mark b and c with seen[b]=1 and seen[c]=1
+    watch_subarray_const ws = solver->watches[lit];
+    *simplifier->limit_to_decrease -= ws.size();
+    for(const Watched w: ws) {
+        if (w.isBin() && !w.red()) {
+            seen[(~w.lit2()).toInt()] = 1;
+            toClear.push_back(~w.lit2());
+        }
+    }
+    //avoid loops
+    seen[(~lit).toInt()] = 0;
+
+    //Now look for
+    //b V c V -a
+    //so look through watches[-a] and check for 3-long clauses
+    watch_subarray_const ws2 = solver->watches[~lit];
+    *simplifier->limit_to_decrease -= ws2.size();
+    for(const Watched w: ws2) {
+        //Looking for tri or longer
+        if (!w.isClause()) continue;
+        ClOffset offset = w.get_offset();
+        const Clause& cl = *solver->cl_alloc.ptr(offset);
+        if (cl.red() || cl.getRemoved() || cl.size() > 5) continue;
+        tmp_lhs.clear();
+
+        bool ok = true;
+        for(auto const& l: cl) {
+            if (l != ~lit && !seen[l.toInt()]) {
+                ok = false;
+                break;
             }
+            if (l != ~lit) tmp_lhs.push_back(l);
         }
+        if (!ok) continue;
+        SLOW_DEBUG_DO(assert(std::is_sorted(tmp_lhs.begin(), tmp_lhs.end())));
+        add_gate_if_not_already_inside(lit, tmp_lhs, cl.stats.ID);
     }
 
-    for(const auto x: toClear) seen[x.var()] = 0;
+    *simplifier->limit_to_decrease -= toClear.size();
+    for(const Lit toclear: toClear) seen[toclear.toInt()] = 0;
     toClear.clear();
-
-    return tobump_cl_var;
 }
 
-vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_var_scores()
+
+void GateFinder::add_gate_if_not_already_inside(
+    const Lit rhs , const vector<Lit>& lhs, const int32_t ID)
 {
-    vector<VarAndVal> vs;
-    for(uint32_t i = 1; i < ls_s->_vars.size(); i++) {
-        vs.push_back(VarAndVal(i-1, ls_s->_vars[i].score));
+    OrGate gate(rhs, lhs, ID);
+    for (Watched ws: solver->watches[gate.rhs]) {
+        if (ws.isIdx()
+            && orGates[ws.get_idx()] == gate
+        ) {
+            return;
+        }
     }
-    std::sort(vs.begin(), vs.end(), VarValSorter());
+    link_in_gate(gate);
+}
 
-    vector<pair<uint32_t, double>> tobump;
-    for(uint32_t i = 0; i < solver->conf.sls_how_many_to_bump; i++) {
-//         cout << "var: " << vs[i].var + 1 << " score: " <<  vs[i].val << endl;
-        tobump.push_back(std::make_pair(vs[i].var, 3.0));
-    }
-    return tobump;
+void GateFinder::link_in_gate(const OrGate& gate)
+{
+    const size_t at = orGates.size();
+    orGates.push_back(gate);
+    solver->watches[gate.rhs].push(Watched(at, WatchType::watch_idx_t));
+    solver->watches.smudge(gate.rhs);
 }
 
-vector<pair<uint32_t, double>> CMS_ccnr::get_bump_based_on_conflict_ct()
+////////////////////////// PRINTING //////////////////////////////
+
+void GateFinder::print_graphviz_dot()
 {
-    if (solver->conf.verbosity) {
-        cout << "c [ccnr] bumping based on var unsat frequency: conflict_ct" << endl;
-    }
+    std::stringstream ss;
+    ss << "Gates" << (numDotPrinted++) << ".dot";
+    std::string filenename = ss.str();
+    std::ofstream file(filenename.c_str(), std::ios::out);
+    file << "digraph G {" << endl;
+    vector<bool> gateUsed;
+    gateUsed.resize(orGates.size(), false);
+    size_t index = 0;
+    for (const OrGate& orGate: orGates) {
+        index++;
+        for (const Lit lit: orGate.get_lhs()) {
+            for (Watched ws: solver->watches[lit]) {
+                if (!ws.isIdx()) {
+                    continue;
+                }
+                uint32_t at = ws.get_idx();
 
-    vector<pair<uint32_t, double>> tobump;
-    int mymax = 0;
-    for(uint32_t i = 1; i < ls_s->_conflict_ct.size(); i++) {
-        mymax = std::max(mymax, ls_s->_conflict_ct[i]);
-    }
+                //The same one, skip
+                if (at == index)
+                    continue;
 
-    for(uint32_t i = 1; i < ls_s->_conflict_ct.size(); i++) {
-        double val = ls_s->_conflict_ct[i];
-        if (mymax > 0) {
-            tobump.push_back(std::make_pair(i-1, (double)val/(double)mymax * 3.0));
-        } else {
-            tobump.push_back(std::make_pair(i-1, 0));
-        }
-//         if (tobump.back().second > 0) {
-//             cout << "var: " << tobump.back().first << " bump by: " << tobump.back().second << endl;
-//         }
-    }
-    return tobump;
-}
+                file << "Gate" << at;
+                gateUsed[at] = true;
+                file << " -> ";
 
-lbool CMS_ccnr::deal_with_solution(int res, const uint32_t num_sls_called)
-{
-    if (solver->conf.sls_get_phase || res) {
-        if (solver->conf.verbosity) {
-            cout
-            << "c [ccnr] saving best assignment phase to stable_polar";
-            if (res) cout << " + best_polar";
-            cout << endl;
-        }
+                file << "Gate" << index;
+                gateUsed[index] = true;
 
-        for(size_t i = 0; i < solver->nVars(); i++) {
-            solver->varData[i].stable_polarity = ls_s->_best_solution[i+1];
-            if (res) {
-                solver->varData[i].best_polarity = ls_s->_best_solution[i+1];
+                file << "[arrowsize=\"0.4\"];" << endl;
             }
+
+            /*vector<uint32_t>& occ2 = gateOccEq[(~*it2).toInt()];
+            for (vector<uint32_t>::const_iterator it3 = occ2.begin(), end3 = occ2.end(); it3 != end3; it3++) {
+                if (*it3 == index) continue;
+
+                file << "Gate" << *it3;
+                gateUsed[*it3] = true;
+                file << " -> ";
+
+                file << "Gate" << index;
+                gateUsed[index] = true;
+
+                file << "[style = \"dotted\", arrowsize=\"0.4\"];" << endl;
+            }*/
         }
     }
 
-    //Clause score sorting
-    vector<pair<uint32_t, double>> tobump;
-    switch (solver->conf.sls_bump_type) {
-        case 1:
-            tobump = get_bump_based_on_cls();
-            break;
-        case 2:
-            assert(false && "Does not work, removed");
-            break;
-        case 3:
-            tobump = get_bump_based_on_var_scores();
-            break;
-        case 4:
-            tobump = get_bump_based_on_conflict_ct();
-            break;
-        case 5:
-            if (num_sls_called % 3 == 0) {
-                tobump = get_bump_based_on_conflict_ct();
-            } else {
-                tobump = get_bump_based_on_cls();
-            }
-            break;
-        case 6:
-            if (num_sls_called % 3 == 0) {
-                tobump = get_bump_based_on_cls();
-            } else {
-                tobump = get_bump_based_on_conflict_ct();
-            }
-            break;
-        default:
-            assert(false && "No such SLS bump type");
-            exit(-1);
+    for (index = 0; index < orGates.size(); index++) {
+        if (gateUsed[index]) {
+            file << "Gate" << index << " [ shape=\"point\"";
+            file << ", size = 0.8";
+            file << ", style=\"filled\"";
+            file << ", color=\"darkseagreen\"";
+            file << "];" << endl;
+        }
     }
 
+    file  << "}" << endl;
+    file.close();
+    cout << "c Printed gate structure to file " << filenename << endl;
+}
 
-    for(const auto& v: tobump) solver->bump_var_importance_all(v.first);
-    if (solver->branch_strategy == branch::vsids) {
-        solver->vsids_decay_var_act();
-    }
-
+GateFinder::Stats& GateFinder::Stats::operator+=(const Stats& other)
+{
+    findGateTime += other.findGateTime;
+    find_gate_timeout += other.find_gate_timeout;
+    orBasedTime += other.orBasedTime;
+    or_based_timeout += other.or_based_timeout;
+    varReplaceTime += other.varReplaceTime;
+    andBasedTime += other.andBasedTime;
+    and_based_timeout += other.and_based_timeout;
+    erTime += other.erTime;
+
+    //OR-gate
+    orGateUseful += other.orGateUseful;
+    numLongCls += other.numLongCls;
+    numLongClsLits += other.numLongClsLits;
+    litsRem += other.litsRem;
+    varReplaced += other.varReplaced;
+
+    //And-gate
+    andGateUseful += other.andGateUseful;
+    clauseSizeRem += other.clauseSizeRem;
+
+    //ER
+    numERVars += other.numERVars;
+
+    //Gates
+    gatesSize += other.gatesSize;
+    num += other.num;
 
-    verb_print(1, "[ccnr] Bumped vars: " << tobump.size()
-        << " bump type: " << solver->conf.sls_bump_type);
+    return *this;
+}
 
-    if (!res) verb_print(2, "[ccnr] ASSIGNMENT NOT FOUND");
-    else verb_print(1, "[ccnr] ASSIGNMENT FOUND");
+void GateFinder::Stats::print(const size_t nVars) const
+{
+    cout << "c -------- GATE FINDING ----------" << endl;
+    print_stats_line("c time"
+        , total_time()
+    );
+
+    print_stats_line("c find gate time"
+        , findGateTime
+        , stats_line_percent(findGateTime, total_time())
+        , "% time"
+    );
+
+    print_stats_line("c gate-based cl-sh time"
+        , orBasedTime
+        , stats_line_percent(orBasedTime, total_time())
+        , "% time"
+    );
+
+    print_stats_line("c gate-based cl-rem time"
+        , andBasedTime
+        , stats_line_percent(andBasedTime, total_time())
+        , "% time"
+    );
+
+    print_stats_line("c gate-based varrep time"
+        , varReplaceTime
+        , stats_line_percent(varReplaceTime, total_time())
+        , "% time"
+    );
+
+    print_stats_line("c gatefinder cl-short"
+        , orGateUseful
+        , stats_line_percent(orGateUseful, numLongCls)
+        , "% long cls"
+    );
+
+    print_stats_line("c gatefinder lits-rem"
+        , litsRem
+        , stats_line_percent(litsRem, numLongClsLits)
+        , "% long cls lits"
+    );
+
+    print_stats_line("c gatefinder cl-rem"
+        , andGateUseful
+        , stats_line_percent(andGateUseful, numLongCls)
+        , "% long cls"
+    );
+
+    print_stats_line("c gatefinder cl-rem's lits"
+        , clauseSizeRem
+        , stats_line_percent(clauseSizeRem, numLongClsLits)
+        , "% long cls lits"
+    );
+
+    print_stats_line("c gatefinder var-rep"
+        , varReplaced
+        , stats_line_percent(varReplaced, nVars)
+        , "% vars"
+    );
 
-    return l_Undef;
+    cout << "c -------- GATE FINDING END ----------" << endl;
 }
+
```

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ccnr_cms.h` & `pyunigen-2.5.4/python/cryptominisat/src/ccnr_cms.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ccnr_mersenne.h` & `pyunigen-2.5.4/python/cryptominisat/src/ccnr_mersenne.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_abs.h` & `pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_abs.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_lgbm.h` & `pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_lgbm.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_py.h` & `pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_py.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cl_predictors_xgb.h` & `pyunigen-2.5.4/python/cryptominisat/src/cl_predictors_xgb.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clabstraction.h` & `pyunigen-2.5.4/python/cryptominisat/src/clabstraction.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clause.h` & `pyunigen-2.5.4/python/cryptominisat/src/clause.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clauseallocator.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/clauseallocator.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clauseallocator.h` & `pyunigen-2.5.4/python/cryptominisat/src/clauseallocator.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clausecleaner.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/clausecleaner.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/clausecleaner.h` & `pyunigen-2.5.4/python/cryptominisat/src/clausecleaner.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cloffset.h` & `pyunigen-2.5.4/python/cryptominisat/src/cloffset.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cms_bosphorus.h` & `pyunigen-2.5.4/python/cryptominisat/src/cms_bosphorus.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cms_breakid.h` & `pyunigen-2.5.4/python/cryptominisat/src/cms_breakid.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cms_windows_includes.h` & `pyunigen-2.5.4/python/cryptominisat/src/cms_windows_includes.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cnf.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/cnf.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cnf.h` & `pyunigen-2.5.4/python/cryptominisat/src/cnf.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/community_finder.h` & `pyunigen-2.5.4/python/cryptominisat/src/community_finder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/completedetachreattacher.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/completedetachreattacher.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/completedetachreattacher.h` & `pyunigen-2.5.4/python/cryptominisat/src/completedetachreattacher.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/constants.h` & `pyunigen-2.5.4/python/cryptominisat/src/constants.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cryptominisat.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/cryptominisat.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cryptominisat.h` & `pyunigen-2.5.4/python/cryptominisat/src/cryptominisat.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cryptominisat_c.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/cryptominisat_c.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cryptominisat_c.h` & `pyunigen-2.5.4/python/cryptominisat/src/cryptominisat_c.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/cset.h` & `pyunigen-2.5.4/python/cryptominisat/src/cset.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/datasync.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/datasync.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/datasync.h` & `pyunigen-2.5.4/python/cryptominisat/src/datasync.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/datasyncserver.h` & `pyunigen-2.5.4/python/cryptominisat/src/datasyncserver.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/dimacsparser.h` & `pyunigen-2.5.4/python/cryptominisat/src/dimacsparser.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerbin.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/distillerbin.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerbin.h` & `pyunigen-2.5.4/python/cryptominisat/src/distillerbin.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlitrem.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlitrem.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlitrem.h` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlitrem.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlong.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlong.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlong.h` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlong.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlongwithimpl.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlongwithimpl.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/distillerlongwithimpl.h` & `pyunigen-2.5.4/python/cryptominisat/src/distillerlongwithimpl.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/frat.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/frat.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/frat.h` & `pyunigen-2.5.4/python/cryptominisat/src/frat.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/gatefinder.h` & `pyunigen-2.5.4/python/cryptominisat/src/gatefinder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/gaussian.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/gaussian.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/gaussian.h` & `pyunigen-2.5.4/python/cryptominisat/src/gaussian.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/gausswatched.h` & `pyunigen-2.5.4/python/cryptominisat/src/gausswatched.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/get_clause_query.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/get_clause_query.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/get_clause_query.h` & `pyunigen-2.5.4/python/cryptominisat/src/get_clause_query.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/gqueuedata.h` & `pyunigen-2.5.4/python/cryptominisat/src/gqueuedata.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/hasher.h` & `pyunigen-2.5.4/python/cryptominisat/src/hasher.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/heap.h` & `pyunigen-2.5.4/python/cryptominisat/src/heap.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/hyperengine.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/hyperengine.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/hyperengine.h` & `pyunigen-2.5.4/python/cryptominisat/src/hyperengine.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/intree.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/intree.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/intree.h` & `pyunigen-2.5.4/python/cryptominisat/src/intree.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/ipasir.h` & `pyunigen-2.5.4/python/cryptominisat/src/ipasir.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/lucky.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/lucky.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/lucky.h` & `pyunigen-2.5.4/python/cryptominisat/src/lucky.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/main.h` & `pyunigen-2.5.4/python/cryptominisat/src/main.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/main_common.h` & `pyunigen-2.5.4/python/cryptominisat/src/main_common.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/matrixfinder.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/matrixfinder.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/matrixfinder.h` & `pyunigen-2.5.4/python/cryptominisat/src/matrixfinder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/msvc/stdint.h` & `pyunigen-2.5.4/python/cryptominisat/src/msvc/stdint.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/mystack.h` & `pyunigen-2.5.4/python/cryptominisat/src/mystack.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/nomutex.h` & `pyunigen-2.5.4/python/cryptominisat/src/nomutex.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/occsimplifier.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/occsimplifier.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/occsimplifier.h` & `pyunigen-2.5.4/python/cryptominisat/src/occsimplifier.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/oracle/bitset.hpp` & `pyunigen-2.5.4/python/cryptominisat/src/oracle/bitset.hpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/oracle/oracle.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/oracle/oracle.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/oracle/oracle.hpp` & `pyunigen-2.5.4/python/cryptominisat/src/oracle/oracle.hpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/oracle/utils.hpp` & `pyunigen-2.5.4/python/cryptominisat/src/oracle/utils.hpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/packedmatrix.h` & `pyunigen-2.5.4/python/cryptominisat/src/packedmatrix.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/packedrow.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/packedrow.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/packedrow.h` & `pyunigen-2.5.4/python/cryptominisat/src/packedrow.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/picosat/picosat.c` & `pyunigen-2.5.4/python/cryptominisat/src/picosat/picosat.c`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/picosat/picosat.h` & `pyunigen-2.5.4/python/cryptominisat/src/picosat/picosat.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/popcnt.h` & `pyunigen-2.5.4/python/cryptominisat/src/popcnt.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/predict_func_type.h` & `pyunigen-2.5.4/python/cryptominisat/src/predict_func_type.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/propby.h` & `pyunigen-2.5.4/python/cryptominisat/src/propby.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/propby_backup.h` & `pyunigen-2.5.4/python/cryptominisat/src/propby_backup.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/propbyforgraph.h` & `pyunigen-2.5.4/python/cryptominisat/src/propbyforgraph.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/propengine.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/propengine.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/propengine.h` & `pyunigen-2.5.4/python/cryptominisat/src/propengine.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/reducedb.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/reducedb.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/reducedb.h` & `pyunigen-2.5.4/python/cryptominisat/src/reducedb.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/satzilla_features.h` & `pyunigen-2.5.4/python/cryptominisat/src/satzilla_features.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/satzilla_features_calc.h` & `pyunigen-2.5.4/python/cryptominisat/src/satzilla_features_calc.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sccfinder.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/sccfinder.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sccfinder.h` & `pyunigen-2.5.4/python/cryptominisat/src/sccfinder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/searcher.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/searcher.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/searcher.h` & `pyunigen-2.5.4/python/cryptominisat/src/searcher.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/searchhist.h` & `pyunigen-2.5.4/python/cryptominisat/src/searchhist.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/searchstats.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/searchstats.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/searchstats.h` & `pyunigen-2.5.4/python/cryptominisat/src/searchstats.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/shareddata.h` & `pyunigen-2.5.4/python/cryptominisat/src/shareddata.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/signalcode.h` & `pyunigen-2.5.4/python/cryptominisat/src/signalcode.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/simplefile.h` & `pyunigen-2.5.4/python/cryptominisat/src/simplefile.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sls.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/sls.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sls.h` & `pyunigen-2.5.4/python/cryptominisat/src/sls.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solutionextender.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/solutionextender.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solutionextender.h` & `pyunigen-2.5.4/python/cryptominisat/src/solutionextender.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solver.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/solver.cpp`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solver.h` & `pyunigen-2.5.4/python/cryptominisat/src/solver.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solverconf.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/solverconf.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solverconf.h` & `pyunigen-2.5.4/python/cryptominisat/src/solverconf.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solvertypes.h` & `pyunigen-2.5.4/python/cryptominisat/src/solvertypes.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/solvertypesmini.h` & `pyunigen-2.5.4/python/cryptominisat/src/solvertypesmini.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sql_tablestructure.h` & `pyunigen-2.5.4/python/cryptominisat/src/sql_tablestructure.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sqlitestats.h` & `pyunigen-2.5.4/python/cryptominisat/src/sqlitestats.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/sqlstats.h` & `pyunigen-2.5.4/python/cryptominisat/src/sqlstats.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/str_impl_w_impl.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/str_impl_w_impl.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/str_impl_w_impl.h` & `pyunigen-2.5.4/python/cryptominisat/src/str_impl_w_impl.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/streambuffer.h` & `pyunigen-2.5.4/python/cryptominisat/src/streambuffer.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/subsumeimplicit.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/subsumeimplicit.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/subsumeimplicit.h` & `pyunigen-2.5.4/python/cryptominisat/src/subsumeimplicit.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/subsumestrengthen.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/subsumestrengthen.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/subsumestrengthen.h` & `pyunigen-2.5.4/python/cryptominisat/src/subsumestrengthen.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/time_mem.h` & `pyunigen-2.5.4/python/cryptominisat/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/toplevelgauss.h` & `pyunigen-2.5.4/python/cryptominisat/src/toplevelgauss.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/toplevelgaussabst.h` & `pyunigen-2.5.4/python/cryptominisat/src/toplevelgaussabst.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/touchlist.h` & `pyunigen-2.5.4/python/cryptominisat/src/touchlist.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/trim.h` & `pyunigen-2.5.4/python/cryptominisat/src/trim.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/vardata.h` & `pyunigen-2.5.4/python/cryptominisat/src/vardata.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/vardistgen.h` & `pyunigen-2.5.4/python/cryptominisat/src/vardistgen.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/varreplacer.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/varreplacer.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/varreplacer.h` & `pyunigen-2.5.4/python/cryptominisat/src/varreplacer.h`

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

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/varupdatehelper.h` & `pyunigen-2.5.4/python/cryptominisat/src/varupdatehelper.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/vmtf.h` & `pyunigen-2.5.4/python/cryptominisat/src/vmtf.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/watchalgos.h` & `pyunigen-2.5.4/python/cryptominisat/src/watchalgos.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/watcharray.h` & `pyunigen-2.5.4/python/cryptominisat/src/watcharray.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/watcharray_handrolled.h` & `pyunigen-2.5.4/python/cryptominisat/src/watcharray_handrolled.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/watched.h` & `pyunigen-2.5.4/python/cryptominisat/src/watched.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/xor.h` & `pyunigen-2.5.4/python/cryptominisat/src/xor.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/xorfinder.cpp` & `pyunigen-2.5.4/python/cryptominisat/src/xorfinder.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/cryptominisat/src/xorfinder.h` & `pyunigen-2.5.4/python/cryptominisat/src/xorfinder.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/src/GitSHA1.cpp` & `pyunigen-2.5.4/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/python/src/pyunigen.cpp` & `pyunigen-2.5.4/python/src/pyunigen.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/setup.py` & `pyunigen-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/GitSHA1.h` & `pyunigen-2.5.4/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/config.h` & `pyunigen-2.5.4/src/config.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/pyunigen.egg-info/PKG-INFO` & `pyunigen-2.5.4/src/pyunigen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunigen
-Version: 2.5.3
+Version: 2.5.4
 Summary: Bindings to UniGen, an approximate sampler
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Meel Group
         Kuldeep Meel
```

### Comparing `pyunigen-2.5.3/src/pyunigen.egg-info/SOURCES.txt` & `pyunigen-2.5.4/src/pyunigen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/sampler.cpp` & `pyunigen-2.5.4/src/sampler.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/sampler.h` & `pyunigen-2.5.4/src/sampler.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/time_mem.h` & `pyunigen-2.5.4/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/unigen.cpp` & `pyunigen-2.5.4/src/unigen.cpp`

 * *Files identical despite different names*

### Comparing `pyunigen-2.5.3/src/unigen.h` & `pyunigen-2.5.4/src/unigen.h`

 * *Files identical despite different names*

