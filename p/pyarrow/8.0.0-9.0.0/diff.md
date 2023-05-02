# Comparing `tmp/pyarrow-8.0.0.tar.gz` & `tmp/pyarrow-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarrow-8.0.0.tar", last modified: Tue May  3 17:04:01 2022, max compression
+gzip compressed data, was "pyarrow-9.0.0.tar", last modified: Fri Jul 29 16:47:06 2022, max compression
```

## Comparing `pyarrow-8.0.0.tar` & `pyarrow-9.0.0.tar`

### file list

```diff
@@ -1,240 +1,246 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.191038 pyarrow-8.0.0/
--rw-r--r--   0 root         (0) root         (0)    22178 2022-05-03 17:03:09.000000 pyarrow-8.0.0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      264 2022-05-03 17:03:09.000000 pyarrow-8.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3396 2022-05-03 17:04:01.191038 pyarrow-8.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2214 2022-05-03 17:03:09.000000 pyarrow-8.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.171038 pyarrow-8.0.0/cmake_modules/
--rw-r--r--   0 root         (0) root         (0)    35195 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/BuildUtils.cmake
--rw-r--r--   0 root         (0) root         (0)    23941 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/DefineOptions.cmake
--rw-r--r--   0 root         (0) root         (0)    16731 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrow.cmake
--rw-r--r--   0 root         (0) root         (0)     3330 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowCUDA.cmake
--rw-r--r--   0 root         (0) root         (0)     3360 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowDataset.cmake
--rw-r--r--   0 root         (0) root         (0)     3427 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowFlight.cmake
--rw-r--r--   0 root         (0) root         (0)     3579 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowFlightSql.cmake
--rw-r--r--   0 root         (0) root         (0)     3850 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowFlightTesting.cmake
--rw-r--r--   0 root         (0) root         (0)     3292 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowPython.cmake
--rw-r--r--   0 root         (0) root         (0)     3765 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowPythonFlight.cmake
--rw-r--r--   0 root         (0) root         (0)     3501 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowSubstrait.cmake
--rw-r--r--   0 root         (0) root         (0)     3382 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindArrowTesting.cmake
--rw-r--r--   0 root         (0) root         (0)     2237 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindBoostAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     5611 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindBrotli.cmake
--rw-r--r--   0 root         (0) root         (0)     3858 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindClangTools.cmake
--rw-r--r--   0 root         (0) root         (0)     1960 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindGLOG.cmake
--rw-r--r--   0 root         (0) root         (0)     3445 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindGandiva.cmake
--rw-r--r--   0 root         (0) root         (0)     1487 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindInferTools.cmake
--rw-r--r--   0 root         (0) root         (0)     3396 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindLLVMAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     2995 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindLz4.cmake
--rw-r--r--   0 root         (0) root         (0)     4008 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindNumPy.cmake
--rw-r--r--   0 root         (0) root         (0)     2073 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindORC.cmake
--rw-r--r--   0 root         (0) root         (0)     1873 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindOpenSSLAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     5068 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindParquet.cmake
--rw-r--r--   0 root         (0) root         (0)     3864 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindPlasma.cmake
--rw-r--r--   0 root         (0) root         (0)     3477 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindPython3Alt.cmake
--rw-r--r--   0 root         (0) root         (0)    11358 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindPythonLibsNew.cmake
--rw-r--r--   0 root         (0) root         (0)     2857 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindRapidJSONAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     1690 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindSQLite3Alt.cmake
--rw-r--r--   0 root         (0) root         (0)     2349 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindSnappy.cmake
--rw-r--r--   0 root         (0) root         (0)     5002 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindThrift.cmake
--rw-r--r--   0 root         (0) root         (0)     2701 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findc-aresAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     4175 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindgRPCAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     2083 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/FindgflagsAlt.cmake
--rw-r--r--   0 root         (0) root         (0)     3222 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findjemalloc.cmake
--rw-r--r--   0 root         (0) root         (0)     1424 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findlibrados.cmake
--rw-r--r--   0 root         (0) root         (0)     3224 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findre2Alt.cmake
--rw-r--r--   0 root         (0) root         (0)     4012 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findutf8proc.cmake
--rw-r--r--   0 root         (0) root         (0)     3198 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Findzstd.cmake
--rw-r--r--   0 root         (0) root         (0)    27595 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/SetupCxxFlags.cmake
--rw-r--r--   0 root         (0) root         (0)   184116 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/ThirdpartyToolchain.cmake
--rw-r--r--   0 root         (0) root         (0)     6781 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/UseCython.cmake
--rw-r--r--   0 root         (0) root         (0)     9057 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/Usevcpkg.cmake
--rw-r--r--   0 root         (0) root         (0)     5331 2022-05-03 17:03:09.000000 pyarrow-8.0.0/cmake_modules/san-config.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.179038 pyarrow-8.0.0/pyarrow/
--rw-r--r--   0 root         (0) root         (0)     2195 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)    23122 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1593 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_compute.pxd
--rw-r--r--   0 root         (0) root         (0)    71197 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_compute.pyx
--rw-r--r--   0 root         (0) root         (0)     1721 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_compute_docstrings.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_csv.pxd
--rw-r--r--   0 root         (0) root         (0)    51976 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_csv.pyx
--rw-r--r--   0 root         (0) root         (0)     1922 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_cuda.pxd
--rw-r--r--   0 root         (0) root         (0)    34731 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_cuda.pyx
--rw-r--r--   0 root         (0) root         (0)     4305 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_dataset.pxd
--rw-r--r--   0 root         (0) root         (0)    95745 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_dataset.pyx
--rw-r--r--   0 root         (0) root         (0)     1345 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_dataset_orc.pyx
--rw-r--r--   0 root         (0) root         (0)    28890 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_dataset_parquet.pyx
--rw-r--r--   0 root         (0) root         (0)    14545 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_exec_plan.pyx
--rw-r--r--   0 root         (0) root         (0)     3773 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_feather.pyx
--rw-r--r--   0 root         (0) root         (0)   100233 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_flight.pyx
--rw-r--r--   0 root         (0) root         (0)     2484 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_fs.pxd
--rw-r--r--   0 root         (0) root         (0)    40858 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_fs.pyx
--rw-r--r--   0 root         (0) root         (0)      142 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow/_generated_version.py
--rw-r--r--   0 root         (0) root         (0)     5471 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_hdfs.pyx
--rw-r--r--   0 root         (0) root         (0)    13681 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_hdfsio.pyx
--rw-r--r--   0 root         (0) root         (0)     8713 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_json.pyx
--rw-r--r--   0 root         (0) root         (0)     5689 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_orc.pxd
--rw-r--r--   0 root         (0) root         (0)    15726 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_orc.pyx
--rw-r--r--   0 root         (0) root         (0)    25078 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_parquet.pxd
--rw-r--r--   0 root         (0) root         (0)    57655 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_parquet.pyx
--rw-r--r--   0 root         (0) root         (0)     6041 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_parquet_encryption.pxd
--rw-r--r--   0 root         (0) root         (0)    17536 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_parquet_encryption.pyx
--rw-r--r--   0 root         (0) root         (0)    29669 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_plasma.pyx
--rw-r--r--   0 root         (0) root         (0)    12199 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/_s3fs.pyx
--rw-r--r--   0 root         (0) root         (0)    89841 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/array.pxi
--rw-r--r--   0 root         (0) root         (0)      869 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/benchmark.pxi
--rw-r--r--   0 root         (0) root         (0)      856 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     2688 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/builder.pxi
--rw-r--r--   0 root         (0) root         (0)     2178 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/cffi.py
--rw-r--r--   0 root         (0) root         (0)     2030 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/compat.pxi
--rw-r--r--   0 root         (0) root         (0)     1076 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/compat.py
--rw-r--r--   0 root         (0) root         (0)    20303 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/compute.py
--rw-r--r--   0 root         (0) root         (0)     2720 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/config.pxi
--rw-r--r--   0 root         (0) root         (0)      974 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/csv.py
--rw-r--r--   0 root         (0) root         (0)     1087 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/cuda.py
--rw-r--r--   0 root         (0) root         (0)    36485 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/dataset.py
--rw-r--r--   0 root         (0) root         (0)     8129 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/error.pxi
--rw-r--r--   0 root         (0) root         (0)     9787 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/feather.py
--rw-r--r--   0 root         (0) root         (0)    14468 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/filesystem.py
--rw-r--r--   0 root         (0) root         (0)     1794 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/flight.py
--rw-r--r--   0 root         (0) root         (0)    13712 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/fs.py
--rw-r--r--   0 root         (0) root         (0)    19585 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/gandiva.pyx
--rw-r--r--   0 root         (0) root         (0)     7527 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/hdfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.183038 pyarrow-8.0.0/pyarrow/includes/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/__init__.pxd
--rw-r--r--   0 root         (0) root         (0)     4326 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/common.pxd
--rw-r--r--   0 root         (0) root         (0)    97772 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow.pxd
--rw-r--r--   0 root         (0) root         (0)     4841 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_cuda.pxd
--rw-r--r--   0 root         (0) root         (0)    15830 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_dataset.pxd
--rw-r--r--   0 root         (0) root         (0)     3717 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_dataset_parquet.pxd
--rw-r--r--   0 root         (0) root         (0)     2140 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_feather.pxd
--rw-r--r--   0 root         (0) root         (0)    22292 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_flight.pxd
--rw-r--r--   0 root         (0) root         (0)    12658 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_fs.pxd
--rw-r--r--   0 root         (0) root         (0)    11257 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libarrow_python.pxd
--rw-r--r--   0 root         (0) root         (0)    11259 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libgandiva.pxd
--rw-r--r--   0 root         (0) root         (0)     1095 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/includes/libplasma.pxd
--rw-r--r--   0 root         (0) root         (0)    66129 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/io.pxi
--rw-r--r--   0 root         (0) root         (0)    32999 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/ipc.pxi
--rw-r--r--   0 root         (0) root         (0)     9672 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/ipc.py
--rw-r--r--   0 root         (0) root         (0)      858 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/json.py
--rw-r--r--   0 root         (0) root         (0)     9593 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/jvm.py
--rw-r--r--   0 root         (0) root         (0)    14628 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/lib.pxd
--rw-r--r--   0 root         (0) root         (0)     4743 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/lib.pyx
--rw-r--r--   0 root         (0) root         (0)     7675 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/memory.pxi
--rw-r--r--   0 root         (0) root         (0)    12451 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/orc.py
--rw-r--r--   0 root         (0) root         (0)     7987 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/pandas-shim.pxi
--rw-r--r--   0 root         (0) root         (0)    43197 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/pandas_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.183038 pyarrow-8.0.0/pyarrow/parquet/
--rw-r--r--   0 root         (0) root         (0)   126072 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/parquet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1153 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/parquet/encryption.py
--rw-r--r--   0 root         (0) root         (0)     6145 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/plasma.py
--rw-r--r--   0 root         (0) root         (0)    12814 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/public-api.pxi
--rw-r--r--   0 root         (0) root         (0)    29459 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/scalar.pxi
--rw-r--r--   0 root         (0) root         (0)    19086 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/serialization.pxi
--rw-r--r--   0 root         (0) root         (0)    18202 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/serialization.py
--rw-r--r--   0 root         (0) root         (0)   160599 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/table.pxi
--rw-r--r--   0 root         (0) root         (0)    39185 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tensor.pxi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.183038 pyarrow-8.0.0/pyarrow/tensorflow/
--rw-r--r--   0 root         (0) root         (0)    14537 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tensorflow/plasma_op.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.187038 pyarrow-8.0.0/pyarrow/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1094 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/arrow_7980.py
--rw-r--r--   0 root         (0) root         (0)     2047 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/bound_function_visit_strings.pyx
--rw-r--r--   0 root         (0) root         (0)     8209 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.167037 pyarrow-8.0.0/pyarrow/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.187038 pyarrow-8.0.0/pyarrow/tests/data/feather/
--rw-r--r--   0 root         (0) root         (0)      594 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/feather/v0.17.0.version.2-compression.lz4.feather
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.191038 pyarrow-8.0.0/pyarrow/tests/data/orc/
--rw-r--r--   0 root         (0) root         (0)      934 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/README.md
--rw-r--r--   0 root         (0) root         (0)       50 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.jsn.gz
--rw-r--r--   0 root         (0) root         (0)      523 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.orc
--rw-r--r--   0 root         (0) root         (0)      323 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.jsn.gz
--rw-r--r--   0 root         (0) root         (0)     1711 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.orc
--rw-r--r--   0 root         (0) root         (0)   182453 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.jsn.gz
--rw-r--r--   0 root         (0) root         (0)    30941 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.orc
--rw-r--r--   0 root         (0) root         (0)    19313 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/decimal.jsn.gz
--rw-r--r--   0 root         (0) root         (0)    16337 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/orc/decimal.orc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.191038 pyarrow-8.0.0/pyarrow/tests/data/parquet/
--rw-r--r--   0 root         (0) root         (0)     3948 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.all-named-index.parquet
--rw-r--r--   0 root         (0) root         (0)     2012 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.column-metadata-handling.parquet
--rw-r--r--   0 root         (0) root         (0)     4372 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.parquet
--rw-r--r--   0 root         (0) root         (0)     4008 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.some-named-index.parquet
--rw-r--r--   0 root         (0) root         (0)      961 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/deserialize_buffer.py
--rw-r--r--   0 root         (0) root         (0)     5115 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/pandas_examples.py
--rw-r--r--   0 root         (0) root         (0)     1429 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/pandas_threaded_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.191038 pyarrow-8.0.0/pyarrow/tests/parquet/
--rw-r--r--   0 root         (0) root         (0)     1040 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6741 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/common.py
--rw-r--r--   0 root         (0) root         (0)     2535 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2517 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/encryption.py
--rw-r--r--   0 root         (0) root         (0)    29247 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_basic.py
--rw-r--r--   0 root         (0) root         (0)     4372 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_compliant_nested_type.py
--rw-r--r--   0 root         (0) root         (0)    17129 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_data_types.py
--rw-r--r--   0 root         (0) root         (0)    60051 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)    15800 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_datetime.py
--rw-r--r--   0 root         (0) root         (0)    20329 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_encryption.py
--rw-r--r--   0 root         (0) root         (0)    18034 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_metadata.py
--rw-r--r--   0 root         (0) root         (0)    25031 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_pandas.py
--rw-r--r--   0 root         (0) root         (0)     7922 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_parquet_file.py
--rw-r--r--   0 root         (0) root         (0)     9778 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/parquet/test_parquet_writer.py
--rw-r--r--   0 root         (0) root         (0)     1951 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/pyarrow_cython_example.pyx
--rw-r--r--   0 root         (0) root         (0)      953 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/read_record_batch.py
--rw-r--r--   0 root         (0) root         (0)    13455 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/strategies.py
--rw-r--r--   0 root         (0) root         (0)     1410 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_adhoc_memory_leak.py
--rw-r--r--   0 root         (0) root         (0)   104736 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_array.py
--rw-r--r--   0 root         (0) root         (0)     2184 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_builder.py
--rw-r--r--   0 root         (0) root         (0)    13637 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_cffi.py
--rw-r--r--   0 root         (0) root         (0)   102660 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    71942 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_convert_builtin.py
--rw-r--r--   0 root         (0) root         (0)    72377 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_csv.py
--rw-r--r--   0 root         (0) root         (0)    27863 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_cuda.py
--rw-r--r--   0 root         (0) root         (0)     8730 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_cuda_numba_interop.py
--rw-r--r--   0 root         (0) root         (0)     5948 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_cython.py
--rw-r--r--   0 root         (0) root         (0)   166572 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)      891 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_deprecations.py
--rw-r--r--   0 root         (0) root         (0)     5600 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_exec_plan.py
--rw-r--r--   0 root         (0) root         (0)    26841 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_extension_type.py
--rw-r--r--   0 root         (0) root         (0)    24126 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_feather.py
--rw-r--r--   0 root         (0) root         (0)     2380 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_filesystem.py
--rw-r--r--   0 root         (0) root         (0)    75264 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_flight.py
--rw-r--r--   0 root         (0) root         (0)    51520 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_fs.py
--rw-r--r--   0 root         (0) root         (0)    14385 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_gandiva.py
--rw-r--r--   0 root         (0) root         (0)    44530 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_gdb.py
--rw-r--r--   0 root         (0) root         (0)    13452 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_hdfs.py
--rw-r--r--   0 root         (0) root         (0)    54208 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)    36915 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_ipc.py
--rw-r--r--   0 root         (0) root         (0)    11938 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    15471 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_jvm.py
--rw-r--r--   0 root         (0) root         (0)     7591 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_memory.py
--rw-r--r--   0 root         (0) root         (0)     5913 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_misc.py
--rw-r--r--   0 root         (0) root         (0)    19279 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_orc.py
--rw-r--r--   0 root         (0) root         (0)   160630 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_pandas.py
--rw-r--r--   0 root         (0) root         (0)    44011 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_plasma.py
--rw-r--r--   0 root         (0) root         (0)     3523 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_plasma_tf_op.py
--rw-r--r--   0 root         (0) root         (0)    21341 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_scalars.py
--rw-r--r--   0 root         (0) root         (0)    21282 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)    42026 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_serialization.py
--rw-r--r--   0 root         (0) root         (0)     1661 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_serialization_deprecated.py
--rw-r--r--   0 root         (0) root         (0)    17436 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_sparse_tensor.py
--rw-r--r--   0 root         (0) root         (0)     1739 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_strategies.py
--rw-r--r--   0 root         (0) root         (0)    64108 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_table.py
--rw-r--r--   0 root         (0) root         (0)     6270 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_tensor.py
--rw-r--r--   0 root         (0) root         (0)    33313 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_types.py
--rw-r--r--   0 root         (0) root         (0)     1791 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/test_util.py
--rw-r--r--   0 root         (0) root         (0)    13470 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/tests/util.py
--rw-r--r--   0 root         (0) root         (0)    90409 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/types.pxi
--rw-r--r--   0 root         (0) root         (0)    10381 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/types.py
--rw-r--r--   0 root         (0) root         (0)     4692 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.191038 pyarrow-8.0.0/pyarrow/vendored/
--rw-r--r--   0 root         (0) root         (0)      785 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/vendored/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22975 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/vendored/docscrape.py
--rw-r--r--   0 root         (0) root         (0)    14345 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyarrow/vendored/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 17:04:01.179038 pyarrow-8.0.0/pyarrow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3396 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6631 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-05-03 17:04:01.000000 pyarrow-8.0.0/pyarrow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      939 2022-05-03 17:03:09.000000 pyarrow-8.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      324 2022-05-03 17:04:01.191038 pyarrow-8.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)    25661 2022-05-03 17:03:09.000000 pyarrow-8.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.387117 pyarrow-9.0.0/
+-rw-r--r--   0 root         (0) root         (0)    22909 2022-07-29 16:46:08.000000 pyarrow-9.0.0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2022-07-29 16:46:08.000000 pyarrow-9.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3396 2022-07-29 16:47:06.387117 pyarrow-9.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2214 2022-07-29 16:46:08.000000 pyarrow-9.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.367117 pyarrow-9.0.0/cmake_modules/
+-rw-r--r--   0 root         (0) root         (0)    32333 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/BuildUtils.cmake
+-rw-r--r--   0 root         (0) root         (0)    24099 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/DefineOptions.cmake
+-rw-r--r--   0 root         (0) root         (0)    16731 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrow.cmake
+-rw-r--r--   0 root         (0) root         (0)     3330 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowCUDA.cmake
+-rw-r--r--   0 root         (0) root         (0)     3360 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowDataset.cmake
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowFlight.cmake
+-rw-r--r--   0 root         (0) root         (0)     3579 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowFlightSql.cmake
+-rw-r--r--   0 root         (0) root         (0)     3850 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowFlightTesting.cmake
+-rw-r--r--   0 root         (0) root         (0)     3292 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowPython.cmake
+-rw-r--r--   0 root         (0) root         (0)     3765 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowPythonFlight.cmake
+-rw-r--r--   0 root         (0) root         (0)     3501 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowSubstrait.cmake
+-rw-r--r--   0 root         (0) root         (0)     3382 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindArrowTesting.cmake
+-rw-r--r--   0 root         (0) root         (0)     5611 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindBrotli.cmake
+-rw-r--r--   0 root         (0) root         (0)     3858 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindClangTools.cmake
+-rw-r--r--   0 root         (0) root         (0)     1960 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindGLOG.cmake
+-rw-r--r--   0 root         (0) root         (0)     3445 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindGandiva.cmake
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindInferTools.cmake
+-rw-r--r--   0 root         (0) root         (0)     3396 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindLLVMAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     4008 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindNumPy.cmake
+-rw-r--r--   0 root         (0) root         (0)     2073 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindORC.cmake
+-rw-r--r--   0 root         (0) root         (0)     1873 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindOpenSSLAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     5068 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindParquet.cmake
+-rw-r--r--   0 root         (0) root         (0)     3864 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindPlasma.cmake
+-rw-r--r--   0 root         (0) root         (0)     3692 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindPython3Alt.cmake
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindPythonLibsNew.cmake
+-rw-r--r--   0 root         (0) root         (0)     2857 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindRapidJSONAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     1690 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindSQLite3Alt.cmake
+-rw-r--r--   0 root         (0) root         (0)     3618 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindSnappyAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     5483 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindThrift.cmake
+-rw-r--r--   0 root         (0) root         (0)     2701 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findc-aresAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     4175 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindgRPCAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     2083 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/FindgflagsAlt.cmake
+-rw-r--r--   0 root         (0) root         (0)     2972 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findjemalloc.cmake
+-rw-r--r--   0 root         (0) root         (0)     1424 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findlibrados.cmake
+-rw-r--r--   0 root         (0) root         (0)     3303 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findlz4Alt.cmake
+-rw-r--r--   0 root         (0) root         (0)     3224 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findre2Alt.cmake
+-rw-r--r--   0 root         (0) root         (0)     4011 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findutf8proc.cmake
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Findzstd.cmake
+-rw-r--r--   0 root         (0) root         (0)    27673 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/SetupCxxFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)   198695 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/ThirdpartyToolchain.cmake
+-rw-r--r--   0 root         (0) root         (0)     6781 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/UseCython.cmake
+-rw-r--r--   0 root         (0) root         (0)     9057 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/Usevcpkg.cmake
+-rw-r--r--   0 root         (0) root         (0)     5338 2022-07-29 16:46:08.000000 pyarrow-9.0.0/cmake_modules/san-config.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.375117 pyarrow-9.0.0/pyarrow/
+-rw-r--r--   0 root         (0) root         (0)     2195 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)    19662 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_compute.pxd
+-rw-r--r--   0 root         (0) root         (0)    84688 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_compute.pyx
+-rw-r--r--   0 root         (0) root         (0)     1707 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_compute_docstrings.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_csv.pxd
+-rw-r--r--   0 root         (0) root         (0)    51976 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_csv.pyx
+-rw-r--r--   0 root         (0) root         (0)     1922 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_cuda.pxd
+-rw-r--r--   0 root         (0) root         (0)    34731 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_cuda.pyx
+-rw-r--r--   0 root         (0) root         (0)     4366 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_dataset.pxd
+-rw-r--r--   0 root         (0) root         (0)    97013 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_dataset.pyx
+-rw-r--r--   0 root         (0) root         (0)     1345 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_dataset_orc.pyx
+-rw-r--r--   0 root         (0) root         (0)    31024 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_dataset_parquet.pyx
+-rw-r--r--   0 root         (0) root         (0)    15974 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_exec_plan.pyx
+-rw-r--r--   0 root         (0) root         (0)     3773 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_feather.pyx
+-rw-r--r--   0 root         (0) root         (0)   101462 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_flight.pyx
+-rw-r--r--   0 root         (0) root         (0)     2484 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_fs.pxd
+-rw-r--r--   0 root         (0) root         (0)    52170 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_fs.pyx
+-rw-r--r--   0 root         (0) root         (0)     8155 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_gcsfs.pyx
+-rw-r--r--   0 root         (0) root         (0)      176 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow/_generated_version.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_hdfs.pyx
+-rw-r--r--   0 root         (0) root         (0)    13681 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_hdfsio.pyx
+-rw-r--r--   0 root         (0) root         (0)     8713 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_json.pyx
+-rw-r--r--   0 root         (0) root         (0)     5689 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_orc.pxd
+-rw-r--r--   0 root         (0) root         (0)    15726 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_orc.pyx
+-rw-r--r--   0 root         (0) root         (0)    25298 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_parquet.pxd
+-rw-r--r--   0 root         (0) root         (0)    58114 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_parquet.pyx
+-rw-r--r--   0 root         (0) root         (0)     6041 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_parquet_encryption.pxd
+-rw-r--r--   0 root         (0) root         (0)    17536 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_parquet_encryption.pyx
+-rw-r--r--   0 root         (0) root         (0)    29669 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_plasma.pyx
+-rw-r--r--   0 root         (0) root         (0)    13900 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_s3fs.pyx
+-rw-r--r--   0 root         (0) root         (0)     2308 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/_substrait.pyx
+-rw-r--r--   0 root         (0) root         (0)    90319 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/array.pxi
+-rw-r--r--   0 root         (0) root         (0)      869 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/benchmark.pxi
+-rw-r--r--   0 root         (0) root         (0)      856 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/builder.pxi
+-rw-r--r--   0 root         (0) root         (0)     2178 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/cffi.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/compat.pxi
+-rw-r--r--   0 root         (0) root         (0)    21796 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/compute.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/config.pxi
+-rw-r--r--   0 root         (0) root         (0)     6322 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      974 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/csv.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/cuda.py
+-rw-r--r--   0 root         (0) root         (0)    38541 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     8129 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/error.pxi
+-rw-r--r--   0 root         (0) root         (0)     9994 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/feather.py
+-rw-r--r--   0 root         (0) root         (0)    14468 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/filesystem.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/flight.py
+-rw-r--r--   0 root         (0) root         (0)    14528 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/fs.py
+-rw-r--r--   0 root         (0) root         (0)    20219 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/gandiva.pyx
+-rw-r--r--   0 root         (0) root         (0)     7527 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/hdfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.375117 pyarrow-9.0.0/pyarrow/includes/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/__init__.pxd
+-rw-r--r--   0 root         (0) root         (0)     4326 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/common.pxd
+-rw-r--r--   0 root         (0) root         (0)   100728 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow.pxd
+-rw-r--r--   0 root         (0) root         (0)     4841 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_cuda.pxd
+-rw-r--r--   0 root         (0) root         (0)    15873 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_dataset.pxd
+-rw-r--r--   0 root         (0) root         (0)     3717 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_dataset_parquet.pxd
+-rw-r--r--   0 root         (0) root         (0)     2140 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_feather.pxd
+-rw-r--r--   0 root         (0) root         (0)    22292 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_flight.pxd
+-rw-r--r--   0 root         (0) root         (0)    13924 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_fs.pxd
+-rw-r--r--   0 root         (0) root         (0)    11257 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_python.pxd
+-rw-r--r--   0 root         (0) root         (0)     1172 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libarrow_substrait.pxd
+-rw-r--r--   0 root         (0) root         (0)    11259 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libgandiva.pxd
+-rw-r--r--   0 root         (0) root         (0)     1095 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/includes/libplasma.pxd
+-rw-r--r--   0 root         (0) root         (0)    66662 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/io.pxi
+-rw-r--r--   0 root         (0) root         (0)    33250 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/ipc.pxi
+-rw-r--r--   0 root         (0) root         (0)     9913 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/ipc.py
+-rw-r--r--   0 root         (0) root         (0)      858 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/json.py
+-rw-r--r--   0 root         (0) root         (0)     9593 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/jvm.py
+-rw-r--r--   0 root         (0) root         (0)    14677 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/lib.pxd
+-rw-r--r--   0 root         (0) root         (0)     4743 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/lib.pyx
+-rw-r--r--   0 root         (0) root         (0)     7827 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/memory.pxi
+-rw-r--r--   0 root         (0) root         (0)    12451 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/orc.py
+-rw-r--r--   0 root         (0) root         (0)     7987 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/pandas-shim.pxi
+-rw-r--r--   0 root         (0) root         (0)    43703 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/pandas_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.379117 pyarrow-9.0.0/pyarrow/parquet/
+-rw-r--r--   0 root         (0) root         (0)   130684 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/parquet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/parquet/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/plasma.py
+-rw-r--r--   0 root         (0) root         (0)    12831 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/public-api.pxi
+-rw-r--r--   0 root         (0) root         (0)    30328 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/scalar.pxi
+-rw-r--r--   0 root         (0) root         (0)    19087 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/serialization.pxi
+-rw-r--r--   0 root         (0) root         (0)    18202 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/serialization.py
+-rw-r--r--   0 root         (0) root         (0)      844 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/substrait.py
+-rw-r--r--   0 root         (0) root         (0)   161790 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/table.pxi
+-rw-r--r--   0 root         (0) root         (0)    39185 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tensor.pxi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.379117 pyarrow-9.0.0/pyarrow/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)    14537 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tensorflow/plasma_op.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.383117 pyarrow-9.0.0/pyarrow/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/arrow_16597.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/arrow_7980.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/bound_function_visit_strings.pyx
+-rw-r--r--   0 root         (0) root         (0)     6270 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.359117 pyarrow-9.0.0/pyarrow/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.383117 pyarrow-9.0.0/pyarrow/tests/data/feather/
+-rw-r--r--   0 root         (0) root         (0)      594 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/feather/v0.17.0.version.2-compression.lz4.feather
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.387117 pyarrow-9.0.0/pyarrow/tests/data/orc/
+-rw-r--r--   0 root         (0) root         (0)      934 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/README.md
+-rw-r--r--   0 root         (0) root         (0)       50 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.jsn.gz
+-rw-r--r--   0 root         (0) root         (0)      523 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.orc
+-rw-r--r--   0 root         (0) root         (0)      323 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.jsn.gz
+-rw-r--r--   0 root         (0) root         (0)     1711 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.orc
+-rw-r--r--   0 root         (0) root         (0)   182453 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.jsn.gz
+-rw-r--r--   0 root         (0) root         (0)    30941 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.orc
+-rw-r--r--   0 root         (0) root         (0)    19313 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/decimal.jsn.gz
+-rw-r--r--   0 root         (0) root         (0)    16337 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/orc/decimal.orc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.387117 pyarrow-9.0.0/pyarrow/tests/data/parquet/
+-rw-r--r--   0 root         (0) root         (0)     3948 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.all-named-index.parquet
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.column-metadata-handling.parquet
+-rw-r--r--   0 root         (0) root         (0)     4372 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.parquet
+-rw-r--r--   0 root         (0) root         (0)     4008 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.some-named-index.parquet
+-rw-r--r--   0 root         (0) root         (0)      961 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/deserialize_buffer.py
+-rw-r--r--   0 root         (0) root         (0)     5115 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/pandas_examples.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/pandas_threaded_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.387117 pyarrow-9.0.0/pyarrow/tests/parquet/
+-rw-r--r--   0 root         (0) root         (0)     1035 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6619 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/common.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/encryption.py
+-rw-r--r--   0 root         (0) root         (0)    30280 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_basic.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_compliant_nested_type.py
+-rw-r--r--   0 root         (0) root         (0)    17252 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_data_types.py
+-rw-r--r--   0 root         (0) root         (0)    63659 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_datetime.py
+-rw-r--r--   0 root         (0) root         (0)    20262 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    18532 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    25154 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_pandas.py
+-rw-r--r--   0 root         (0) root         (0)     8045 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_parquet_file.py
+-rw-r--r--   0 root         (0) root         (0)     9901 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/parquet/test_parquet_writer.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/pyarrow_cython_example.pyx
+-rw-r--r--   0 root         (0) root         (0)      953 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/read_record_batch.py
+-rw-r--r--   0 root         (0) root         (0)    13455 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/strategies.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_adhoc_memory_leak.py
+-rw-r--r--   0 root         (0) root         (0)   104735 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_array.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_builder.py
+-rw-r--r--   0 root         (0) root         (0)    13637 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_cffi.py
+-rw-r--r--   0 root         (0) root         (0)   108409 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    71942 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_convert_builtin.py
+-rw-r--r--   0 root         (0) root         (0)    72377 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_csv.py
+-rw-r--r--   0 root         (0) root         (0)    27863 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_cuda.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_cuda_numba_interop.py
+-rw-r--r--   0 root         (0) root         (0)     6029 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_cython.py
+-rw-r--r--   0 root         (0) root         (0)   171660 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      891 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_deprecations.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_exec_plan.py
+-rw-r--r--   0 root         (0) root         (0)    29082 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_extension_type.py
+-rw-r--r--   0 root         (0) root         (0)    24126 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_feather.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_filesystem.py
+-rw-r--r--   0 root         (0) root         (0)    78339 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_flight.py
+-rw-r--r--   0 root         (0) root         (0)    55307 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_fs.py
+-rw-r--r--   0 root         (0) root         (0)    15501 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_gandiva.py
+-rw-r--r--   0 root         (0) root         (0)    44541 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_gdb.py
+-rw-r--r--   0 root         (0) root         (0)    13452 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    56102 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)    36310 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    15471 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_jvm.py
+-rw-r--r--   0 root         (0) root         (0)     7801 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_misc.py
+-rw-r--r--   0 root         (0) root         (0)    19279 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_orc.py
+-rw-r--r--   0 root         (0) root         (0)   161595 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_pandas.py
+-rw-r--r--   0 root         (0) root         (0)    44011 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_plasma.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_plasma_tf_op.py
+-rw-r--r--   0 root         (0) root         (0)    20605 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_scalars.py
+-rw-r--r--   0 root         (0) root         (0)    21282 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)    42026 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_serialization.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_serialization_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)    17436 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_sparse_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_strategies.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_substrait.py
+-rw-r--r--   0 root         (0) root         (0)    65758 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_table.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_tensor.py
+-rw-r--r--   0 root         (0) root         (0)    33313 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_types.py
+-rw-r--r--   0 root         (0) root         (0)    17126 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_udf.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    13470 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/tests/util.py
+-rw-r--r--   0 root         (0) root         (0)    91301 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/types.pxi
+-rw-r--r--   0 root         (0) root         (0)    10381 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/types.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.387117 pyarrow-9.0.0/pyarrow/vendored/
+-rw-r--r--   0 root         (0) root         (0)      785 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/vendored/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22975 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/vendored/docscrape.py
+-rw-r--r--   0 root         (0) root         (0)    14345 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyarrow/vendored/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-29 16:47:06.375117 pyarrow-9.0.0/pyarrow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3396 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6796 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-07-29 16:47:06.000000 pyarrow-9.0.0/pyarrow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2022-07-29 16:46:08.000000 pyarrow-9.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      324 2022-07-29 16:47:06.387117 pyarrow-9.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)    26967 2022-07-29 16:46:08.000000 pyarrow-9.0.0/setup.py
```

### Comparing `pyarrow-8.0.0/CMakeLists.txt` & `pyarrow-9.0.0/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
   set(CMAKE_EXPORT_COMPILE_COMMANDS 1)
 endif()
 
 # Top level cmake dir
 if("${CMAKE_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_SOURCE_DIR}")
   option(PYARROW_BUILD_CUDA "Build the PyArrow CUDA support" OFF)
   option(PYARROW_BUILD_FLIGHT "Build the PyArrow Flight integration" OFF)
+  option(PYARROW_BUILD_SUBSTRAIT "Build the PyArrow Substrait integration" OFF)
   option(PYARROW_BUILD_DATASET "Build the PyArrow Dataset integration" OFF)
   option(PYARROW_BUILD_GANDIVA "Build the PyArrow Gandiva integration" OFF)
   option(PYARROW_BUILD_PARQUET "Build the PyArrow Parquet integration" OFF)
   option(PYARROW_PARQUET_USE_SHARED "Rely on parquet shared libraries where relevant" ON)
   option(PYARROW_BUILD_PARQUET_ENCRYPTION
          "Build the PyArrow Parquet encryption integration" OFF)
   option(PYARROW_BOOST_USE_SHARED
@@ -223,14 +224,18 @@
 # Dependencies
 #
 
 if(PYARROW_BUILD_FLIGHT)
   set(ARROW_FLIGHT TRUE)
 endif()
 
+if(PYARROW_BUILD_SUBSTRAIT)
+  set(ARROW_SUBSTRAIT TRUE)
+endif()
+
 # Arrow
 find_package(ArrowPython REQUIRED)
 include_directories(SYSTEM ${ARROW_INCLUDE_DIR})
 
 function(bundle_arrow_lib library_path)
   set(options)
   set(one_value_args SO_VERSION)
@@ -403,14 +408,18 @@
     _feather
     _fs
     _hdfsio
     _json)
 
 set(LINK_LIBS arrow_shared arrow_python_shared)
 
+if(PYARROW_BUILD_GCS)
+  set(CYTHON_EXTENSIONS ${CYTHON_EXTENSIONS} _gcsfs)
+endif()
+
 if(PYARROW_BUILD_S3)
   set(CYTHON_EXTENSIONS ${CYTHON_EXTENSIONS} _s3fs)
 endif()
 
 if(PYARROW_BUILD_HDFS)
   set(CYTHON_EXTENSIONS ${CYTHON_EXTENSIONS} _hdfs)
 endif()
@@ -531,14 +540,28 @@
     endif()
   endif()
 
   set(FLIGHT_LINK_LIBS arrow_flight_shared arrow_python_flight_shared)
   set(CYTHON_EXTENSIONS ${CYTHON_EXTENSIONS} _flight)
 endif()
 
+# Engine
+if(PYARROW_BUILD_SUBSTRAIT)
+  find_package(ArrowSubstrait REQUIRED)
+  if(PYARROW_BUNDLE_ARROW_CPP)
+    bundle_arrow_lib(ARROW_SUBSTRAIT_SHARED_LIB SO_VERSION ${ARROW_SO_VERSION})
+    if(MSVC)
+      bundle_arrow_import_lib(ARROW_SUBSTRAIT_IMPORT_LIB)
+    endif()
+  endif()
+
+  set(SUBSTRAIT_LINK_LIBS arrow_substrait_shared)
+  set(CYTHON_EXTENSIONS ${CYTHON_EXTENSIONS} _substrait)
+endif()
+
 # Gandiva
 if(PYARROW_BUILD_GANDIVA)
   find_package(Gandiva REQUIRED)
 
   include_directories(SYSTEM ${GANDIVA_INCLUDE_DIR})
 
   if(PYARROW_BUNDLE_ARROW_CPP)
@@ -621,14 +644,18 @@
   target_link_libraries(_cuda PRIVATE ${CUDA_LINK_LIBS})
 endif()
 
 if(PYARROW_BUILD_FLIGHT)
   target_link_libraries(_flight PRIVATE ${FLIGHT_LINK_LIBS})
 endif()
 
+if(PYARROW_BUILD_SUBSTRAIT)
+  target_link_libraries(_substrait PRIVATE ${SUBSTRAIT_LINK_LIBS})
+endif()
+
 if(PYARROW_BUILD_DATASET)
   target_link_libraries(_dataset PRIVATE ${DATASET_LINK_LIBS})
   target_link_libraries(_exec_plan PRIVATE ${DATASET_LINK_LIBS})
   if(PYARROW_BUILD_ORC)
     target_link_libraries(_dataset_orc PRIVATE ${DATASET_LINK_LIBS})
   endif()
   if(PYARROW_BUILD_PARQUET)
```

### Comparing `pyarrow-8.0.0/PKG-INFO` & `pyarrow-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarrow
-Version: 8.0.0
+Version: 9.0.0
 Summary: Python library for Apache Arrow
 Home-page: https://arrow.apache.org/
 Maintainer: Apache Arrow Developers
 Maintainer-email: dev@arrow.apache.org
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://arrow.apache.org/docs/python
 Project-URL: Source, https://github.com/apache/arrow
```

### Comparing `pyarrow-8.0.0/README.md` & `pyarrow-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/BuildUtils.cmake` & `pyarrow-9.0.0/cmake_modules/BuildUtils.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -26,115 +26,46 @@
     "lib"
     "bin"
     "Library"
     "Library/lib"
     "Library/bin")
 set(ARROW_INCLUDE_PATH_SUFFIXES "include" "Library" "Library/include")
 
-set(ARROW_BOOST_PROCESS_COMPILE_DEFINITIONS)
-if(WIN32 AND CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
-  # boost/process/detail/windows/handle_workaround.hpp doesn't work
-  # without BOOST_USE_WINDOWS_H with MinGW because MinGW doesn't
-  # provide __kernel_entry without winternl.h.
-  #
-  # See also:
-  # https://github.com/boostorg/process/blob/develop/include/boost/process/detail/windows/handle_workaround.hpp
-  #
-  # You can use this like the following:
-  #
-  #   target_compile_definitions(target PRIVATE
-  #                              ${ARROW_BOOST_PROCESS_COMPILE_DEFINITIONS})
-  list(APPEND ARROW_BOOST_PROCESS_COMPILE_DEFINITIONS "BOOST_USE_WINDOWS_H=1")
-endif()
-
-function(ADD_THIRDPARTY_LIB LIB_NAME)
+function(add_thirdparty_lib LIB_NAME LIB_TYPE LIB)
   set(options)
-  set(one_value_args SHARED_LIB STATIC_LIB)
+  set(one_value_args)
   set(multi_value_args DEPS INCLUDE_DIRECTORIES)
   cmake_parse_arguments(ARG
                         "${options}"
                         "${one_value_args}"
                         "${multi_value_args}"
                         ${ARGN})
   if(ARG_UNPARSED_ARGUMENTS)
     message(SEND_ERROR "Error: unrecognized arguments: ${ARG_UNPARSED_ARGUMENTS}")
   endif()
 
-  if(ARG_STATIC_LIB AND ARG_SHARED_LIB)
-    set(AUG_LIB_NAME "${LIB_NAME}_static")
-    add_library(${AUG_LIB_NAME} STATIC IMPORTED)
-    set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_LOCATION
-                                                     "${ARG_STATIC_LIB}")
-    if(ARG_DEPS)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_LINK_LIBRARIES
-                                                       "${ARG_DEPS}")
-    endif()
-    message(STATUS "Added static library dependency ${AUG_LIB_NAME}: ${ARG_STATIC_LIB}")
-    if(ARG_INCLUDE_DIRECTORIES)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
-                                                       "${ARG_INCLUDE_DIRECTORIES}")
-    endif()
-
-    set(AUG_LIB_NAME "${LIB_NAME}_shared")
-    add_library(${AUG_LIB_NAME} SHARED IMPORTED)
-
-    if(WIN32)
-      # Mark the ".lib" location as part of a Windows DLL
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_IMPLIB
-                                                       "${ARG_SHARED_LIB}")
-    else()
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_LOCATION
-                                                       "${ARG_SHARED_LIB}")
-    endif()
-    if(ARG_DEPS)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_LINK_LIBRARIES
-                                                       "${ARG_DEPS}")
-    endif()
-    message(STATUS "Added shared library dependency ${AUG_LIB_NAME}: ${ARG_SHARED_LIB}")
-    if(ARG_INCLUDE_DIRECTORIES)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
-                                                       "${ARG_INCLUDE_DIRECTORIES}")
-    endif()
-  elseif(ARG_STATIC_LIB)
-    set(AUG_LIB_NAME "${LIB_NAME}_static")
-    add_library(${AUG_LIB_NAME} STATIC IMPORTED)
-    set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_LOCATION
-                                                     "${ARG_STATIC_LIB}")
-    if(ARG_DEPS)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_LINK_LIBRARIES
-                                                       "${ARG_DEPS}")
-    endif()
-    message(STATUS "Added static library dependency ${AUG_LIB_NAME}: ${ARG_STATIC_LIB}")
-    if(ARG_INCLUDE_DIRECTORIES)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
-                                                       "${ARG_INCLUDE_DIRECTORIES}")
-    endif()
-  elseif(ARG_SHARED_LIB)
-    set(AUG_LIB_NAME "${LIB_NAME}_shared")
-    add_library(${AUG_LIB_NAME} SHARED IMPORTED)
-
+  add_library(${LIB_NAME} ${LIB_TYPE} IMPORTED)
+  if(${LIB_TYPE} STREQUAL "STATIC")
+    set_target_properties(${LIB_NAME} PROPERTIES IMPORTED_LOCATION "${LIB}")
+    message(STATUS "Added static library dependency ${LIB_NAME}: ${LIB}")
+  else()
     if(WIN32)
       # Mark the ".lib" location as part of a Windows DLL
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_IMPLIB
-                                                       "${ARG_SHARED_LIB}")
+      set_target_properties(${LIB_NAME} PROPERTIES IMPORTED_IMPLIB "${LIB}")
     else()
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES IMPORTED_LOCATION
-                                                       "${ARG_SHARED_LIB}")
-    endif()
-    message(STATUS "Added shared library dependency ${AUG_LIB_NAME}: ${ARG_SHARED_LIB}")
-    if(ARG_DEPS)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_LINK_LIBRARIES
-                                                       "${ARG_DEPS}")
-    endif()
-    if(ARG_INCLUDE_DIRECTORIES)
-      set_target_properties(${AUG_LIB_NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
-                                                       "${ARG_INCLUDE_DIRECTORIES}")
+      set_target_properties(${LIB_NAME} PROPERTIES IMPORTED_LOCATION "${LIB}")
     endif()
-  else()
-    message(FATAL_ERROR "No static or shared library provided for ${LIB_NAME}")
+    message(STATUS "Added shared library dependency ${LIB_NAME}: ${LIB}")
+  endif()
+  if(ARG_DEPS)
+    set_target_properties(${LIB_NAME} PROPERTIES INTERFACE_LINK_LIBRARIES "${ARG_DEPS}")
+  endif()
+  if(ARG_INCLUDE_DIRECTORIES)
+    set_target_properties(${LIB_NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                                 "${ARG_INCLUDE_DIRECTORIES}")
   endif()
 endfunction()
 
 function(REUSE_PRECOMPILED_HEADER_LIB TARGET_NAME LIB_NAME)
   if(ARROW_USE_PRECOMPILED_HEADERS)
     target_precompile_headers(${TARGET_NAME} REUSE_FROM ${LIB_NAME})
   endif()
@@ -267,30 +198,36 @@
   endif()
   if(ARG_OUTPUT_PATH)
     set(OUTPUT_PATH ${ARG_OUTPUT_PATH})
   else()
     set(OUTPUT_PATH ${BUILD_OUTPUT_ROOT_DIRECTORY})
   endif()
 
-  if(WIN32 OR (CMAKE_GENERATOR STREQUAL Xcode))
+  if(WIN32
+     OR (CMAKE_GENERATOR STREQUAL Xcode)
+     OR CMAKE_VERSION VERSION_LESS 3.12
+     OR NOT ARROW_POSITION_INDEPENDENT_CODE)
     # We need to compile C++ separately for each library kind (shared and static)
     # because of dllexport declarations on Windows.
     # The Xcode generator doesn't reliably work with Xcode as target names are not
     # guessed correctly.
+    # We can't use target for object library with CMake 3.11 or earlier.
+    # See also: Object Libraries:
+    # https://cmake.org/cmake/help/latest/command/add_library.html#object-libraries
     set(USE_OBJLIB OFF)
   else()
     set(USE_OBJLIB ON)
   endif()
 
   if(USE_OBJLIB)
     # Generate a single "objlib" from all C++ modules and link
     # that "objlib" into each library kind, to avoid compiling twice
     add_library(${LIB_NAME}_objlib OBJECT ${ARG_SOURCES})
     # Necessary to make static linking into other shared libraries work properly
-    set_property(TARGET ${LIB_NAME}_objlib PROPERTY POSITION_INDEPENDENT_CODE 1)
+    set_property(TARGET ${LIB_NAME}_objlib PROPERTY POSITION_INDEPENDENT_CODE ON)
     if(ARG_DEPENDENCIES)
       add_dependencies(${LIB_NAME}_objlib ${ARG_DEPENDENCIES})
     endif()
     if(ARG_PRECOMPILED_HEADER_LIB)
       reuse_precompiled_header_lib(${LIB_NAME}_objlib ${ARG_PRECOMPILED_HEADER_LIB})
     endif()
     if(ARG_PRECOMPILED_HEADERS AND ARROW_USE_PRECOMPILED_HEADERS)
@@ -306,14 +243,17 @@
 
     if(ARG_EXTRA_INCLUDES)
       target_include_directories(${LIB_NAME}_objlib SYSTEM PUBLIC ${ARG_EXTRA_INCLUDES})
     endif()
     if(ARG_PRIVATE_INCLUDES)
       target_include_directories(${LIB_NAME}_objlib PRIVATE ${ARG_PRIVATE_INCLUDES})
     endif()
+    target_link_libraries(${LIB_NAME}_objlib
+                          PRIVATE ${ARG_SHARED_LINK_LIBS} ${ARG_SHARED_PRIVATE_LINK_LIBS}
+                                  ${ARG_STATIC_LINK_LIBS})
   else()
     # Prepare arguments for separate compilation of static and shared libs below
     # TODO: add PCH directives
     set(LIB_DEPS ${ARG_SOURCES})
     set(EXTRA_DEPS ${ARG_DEPENDENCIES})
 
     if(ARG_EXTRA_INCLUDES)
@@ -439,17 +379,18 @@
 
     if(MSVC_TOOLCHAIN)
       set(LIB_NAME_STATIC ${LIB_NAME}_static)
     else()
       set(LIB_NAME_STATIC ${LIB_NAME})
     endif()
 
-    if(ARROW_BUILD_STATIC AND WIN32)
+    if(WIN32)
       target_compile_definitions(${LIB_NAME}_static PUBLIC ARROW_STATIC)
       target_compile_definitions(${LIB_NAME}_static PUBLIC ARROW_FLIGHT_STATIC)
+      target_compile_definitions(${LIB_NAME}_static PUBLIC ARROW_FLIGHT_SQL_STATIC)
     endif()
 
     set_target_properties(${LIB_NAME}_static
                           PROPERTIES LIBRARY_OUTPUT_DIRECTORY "${OUTPUT_PATH}"
                                      OUTPUT_NAME ${LIB_NAME_STATIC})
 
     if(ARG_STATIC_INSTALL_INTERFACE_LIBS)
@@ -482,30 +423,29 @@
 
   if(ARG_CMAKE_PACKAGE_NAME)
     arrow_install_cmake_find_module("${ARG_CMAKE_PACKAGE_NAME}")
 
     set(TARGETS_CMAKE "${ARG_CMAKE_PACKAGE_NAME}Targets.cmake")
     install(EXPORT ${LIB_NAME}_targets
             FILE "${TARGETS_CMAKE}"
-            DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
+            DESTINATION "${ARROW_CMAKE_DIR}")
 
     set(CONFIG_CMAKE "${ARG_CMAKE_PACKAGE_NAME}Config.cmake")
     set(BUILT_CONFIG_CMAKE "${CMAKE_CURRENT_BINARY_DIR}/${CONFIG_CMAKE}")
     configure_package_config_file("${CONFIG_CMAKE}.in" "${BUILT_CONFIG_CMAKE}"
-                                  INSTALL_DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
-    install(FILES "${BUILT_CONFIG_CMAKE}" DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
+                                  INSTALL_DESTINATION "${ARROW_CMAKE_DIR}")
+    install(FILES "${BUILT_CONFIG_CMAKE}" DESTINATION "${ARROW_CMAKE_DIR}")
 
     set(CONFIG_VERSION_CMAKE "${ARG_CMAKE_PACKAGE_NAME}ConfigVersion.cmake")
     set(BUILT_CONFIG_VERSION_CMAKE "${CMAKE_CURRENT_BINARY_DIR}/${CONFIG_VERSION_CMAKE}")
     write_basic_package_version_file(
       "${BUILT_CONFIG_VERSION_CMAKE}"
       VERSION ${${PROJECT_NAME}_VERSION}
       COMPATIBILITY AnyNewerVersion)
-    install(FILES "${BUILT_CONFIG_VERSION_CMAKE}"
-            DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
+    install(FILES "${BUILT_CONFIG_VERSION_CMAKE}" DESTINATION "${ARROW_CMAKE_DIR}")
   endif()
 
   if(ARG_PKG_CONFIG_NAME)
     arrow_add_pkg_config("${ARG_PKG_CONFIG_NAME}")
   endif()
 
   # Modify variable in calling scope
@@ -964,15 +904,15 @@
   configure_file(${MODULE}.pc.in "${CMAKE_CURRENT_BINARY_DIR}/${MODULE}.pc" @ONLY)
   install(FILES "${CMAKE_CURRENT_BINARY_DIR}/${MODULE}.pc"
           DESTINATION "${CMAKE_INSTALL_LIBDIR}/pkgconfig/")
 endfunction()
 
 function(ARROW_INSTALL_CMAKE_FIND_MODULE MODULE)
   install(FILES "${ARROW_SOURCE_DIR}/cmake_modules/Find${MODULE}.cmake"
-          DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
+          DESTINATION "${ARROW_CMAKE_DIR}")
 endfunction()
 
 # Implementations of lisp "car" and "cdr" functions
 macro(ARROW_CAR var)
   set(${var} ${ARGV1})
 endmacro()
```

### Comparing `pyarrow-8.0.0/cmake_modules/DefineOptions.cmake` & `pyarrow-9.0.0/cmake_modules/DefineOptions.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
   if(NOT ("${${name}_OPTION_ENUM}" STREQUAL ""))
     set_property(CACHE ${name} PROPERTY STRINGS "${name}_OPTION_POSSIBLE_VALUES")
   endif()
 endmacro()
 
 # Top level cmake dir
 if("${CMAKE_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_SOURCE_DIR}")
+  set(ARROW_DEFINE_OPTIONS_DEFAULT ON)
+else()
+  set(ARROW_DEFINE_OPTIONS_DEFAULT OFF)
+endif()
+option(ARROW_DEFINE_OPTIONS "Define Arrow options" ${ARROW_DEFINE_OPTIONS_DEFAULT})
+if(ARROW_DEFINE_OPTIONS)
   #----------------------------------------------------------------------
   set_option_category("Compile and link")
 
   define_option_string(ARROW_CXXFLAGS "Compiler flags to append when compiling Arrow" "")
 
   define_option(ARROW_BUILD_STATIC "Build static libraries" ON)
 
@@ -99,14 +105,17 @@
   define_option_string(ARROW_GIT_ID "The Arrow git commit id (if any)" "")
 
   define_option_string(ARROW_GIT_DESCRIPTION "The Arrow git commit description (if any)"
                        "")
 
   define_option(ARROW_NO_DEPRECATED_API "Exclude deprecated APIs from build" OFF)
 
+  define_option(ARROW_POSITION_INDEPENDENT_CODE
+                "Whether to create position-independent target" ON)
+
   define_option(ARROW_USE_CCACHE "Use ccache when compiling (if available)" ON)
 
   define_option(ARROW_USE_LD_GOLD "Use ld.gold for linking on Linux (if available)" OFF)
 
   define_option(ARROW_USE_PRECOMPILED_HEADERS "Use precompiled headers when compiling"
                 OFF)
 
@@ -234,20 +243,17 @@
 
   define_option(ARROW_FLIGHT_SQL "Build the Arrow Flight SQL extension" OFF)
 
   define_option(ARROW_GANDIVA "Build the Gandiva libraries" OFF)
 
   define_option(ARROW_GCS
                 "Build Arrow with GCS support (requires the GCloud SDK for C++)" OFF)
-  mark_as_advanced(ARROW_GCS) # TODO(ARROW-1231) - remove once completed
 
   define_option(ARROW_HDFS "Build the Arrow HDFS bridge" OFF)
 
-  define_option(ARROW_HIVESERVER2 "Build the HiveServer2 client and Arrow adapter" OFF)
-
   define_option(ARROW_IPC "Build the Arrow IPC extensions" ON)
 
   set(ARROW_JEMALLOC_DESCRIPTION "Build the Arrow jemalloc-based allocator")
   if(WIN32 OR "${CMAKE_SYSTEM_NAME}" STREQUAL "FreeBSD")
     # jemalloc is not supported on Windows.
     #
     # jemalloc is the default malloc implementation on FreeBSD and can't
@@ -322,61 +328,61 @@
                        "BREW")
 
   define_option(ARROW_VERBOSE_THIRDPARTY_BUILD
                 "Show output from ExternalProjects rather than just logging to files" OFF)
 
   define_option(ARROW_DEPENDENCY_USE_SHARED "Link to shared libraries" ON)
 
-  define_option(ARROW_BOOST_USE_SHARED "Rely on boost shared libraries where relevant"
+  define_option(ARROW_BOOST_USE_SHARED "Rely on Boost shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_BROTLI_USE_SHARED "Rely on Brotli shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_BZ2_USE_SHARED "Rely on Bz2 shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_GFLAGS_USE_SHARED "Rely on GFlags shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_GRPC_USE_SHARED "Rely on gRPC shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
+  define_option(ARROW_JEMALLOC_USE_SHARED
+                "Rely on jemalloc shared libraries where relevant"
+                ${ARROW_DEPENDENCY_USE_SHARED})
+
   define_option(ARROW_LZ4_USE_SHARED "Rely on lz4 shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_OPENSSL_USE_SHARED
                 "Rely on OpenSSL shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_PROTOBUF_USE_SHARED
                 "Rely on Protocol Buffers shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
+  define_option(ARROW_SNAPPY_USE_SHARED "Rely on snappy shared libraries where relevant"
+                ${ARROW_DEPENDENCY_USE_SHARED})
+
   if(WIN32)
     # It seems that Thrift doesn't support DLL well yet.
     # MSYS2, conda-forge and vcpkg don't build shared library.
     set(ARROW_THRIFT_USE_SHARED_DEFAULT OFF)
   else()
     set(ARROW_THRIFT_USE_SHARED_DEFAULT ${ARROW_DEPENDENCY_USE_SHARED})
   endif()
   define_option(ARROW_THRIFT_USE_SHARED "Rely on thrift shared libraries where relevant"
                 ${ARROW_THRIFT_USE_SHARED_DEFAULT})
 
   define_option(ARROW_UTF8PROC_USE_SHARED
                 "Rely on utf8proc shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
-  define_option(ARROW_SNAPPY_USE_SHARED "Rely on snappy shared libraries where relevant"
-                ${ARROW_DEPENDENCY_USE_SHARED})
-
-  define_option(ARROW_UTF8PROC_USE_SHARED
-                "Rely on utf8proc shared libraries where relevant"
-                ${ARROW_DEPENDENCY_USE_SHARED})
-
   define_option(ARROW_ZSTD_USE_SHARED "Rely on zstd shared libraries where relevant"
                 ${ARROW_DEPENDENCY_USE_SHARED})
 
   define_option(ARROW_USE_GLOG "Build libraries with glog support for pluggable logging"
                 OFF)
 
   define_option(ARROW_WITH_BACKTRACE "Build with backtrace support" ON)
```

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrow.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrow.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowCUDA.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowCUDA.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowDataset.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowDataset.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowFlight.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowFlight.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowFlightSql.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowFlightSql.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowFlightTesting.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowFlightTesting.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowPython.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowPython.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowPythonFlight.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowPythonFlight.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowSubstrait.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowSubstrait.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindArrowTesting.cmake` & `pyarrow-9.0.0/cmake_modules/FindArrowTesting.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindBrotli.cmake` & `pyarrow-9.0.0/cmake_modules/FindBrotli.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindClangTools.cmake` & `pyarrow-9.0.0/cmake_modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindGLOG.cmake` & `pyarrow-9.0.0/cmake_modules/FindGLOG.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindGandiva.cmake` & `pyarrow-9.0.0/cmake_modules/FindGandiva.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindInferTools.cmake` & `pyarrow-9.0.0/cmake_modules/FindInferTools.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindLLVMAlt.cmake` & `pyarrow-9.0.0/cmake_modules/FindLLVMAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindLz4.cmake` & `pyarrow-9.0.0/cmake_modules/Findlz4Alt.cmake`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
+set(find_package_args)
+if(lz4Alt_FIND_VERSION)
+  list(APPEND find_package_args ${lz4Alt_FIND_VERSION})
+endif()
+if(lz4Alt_FIND_QUIETLY)
+  list(APPEND find_package_args QUIET)
+endif()
+find_package(lz4 ${find_package_args})
+if(lz4_FOUND)
+  set(lz4Alt_FOUND TRUE)
+  return()
+endif()
+
 if(MSVC_TOOLCHAIN AND NOT DEFINED LZ4_MSVC_LIB_PREFIX)
   set(LZ4_MSVC_LIB_PREFIX "lib")
 endif()
 set(LZ4_LIB_NAME_BASE "${LZ4_MSVC_LIB_PREFIX}lz4")
 
 if(ARROW_LZ4_USE_SHARED)
   set(LZ4_LIB_NAMES)
@@ -69,16 +82,17 @@
                  PATH_SUFFIXES ${ARROW_LIBRARY_PATH_SUFFIXES})
     find_path(LZ4_INCLUDE_DIR
               NAMES lz4.h
               PATH_SUFFIXES ${ARROW_INCLUDE_PATH_SUFFIXES})
   endif()
 endif()
 
-find_package_handle_standard_args(Lz4 REQUIRED_VARS LZ4_LIB LZ4_INCLUDE_DIR)
+find_package_handle_standard_args(lz4Alt REQUIRED_VARS LZ4_LIB LZ4_INCLUDE_DIR)
 
-if(Lz4_FOUND)
-  set(Lz4_FOUND TRUE)
-  add_library(LZ4::lz4 UNKNOWN IMPORTED)
-  set_target_properties(LZ4::lz4
-                        PROPERTIES IMPORTED_LOCATION "${LZ4_LIB}"
-                                   INTERFACE_INCLUDE_DIRECTORIES "${LZ4_INCLUDE_DIR}")
+if(lz4Alt_FOUND)
+  if(NOT TARGET lz4::lz4)
+    add_library(lz4::lz4 UNKNOWN IMPORTED)
+    set_target_properties(lz4::lz4
+                          PROPERTIES IMPORTED_LOCATION "${LZ4_LIB}"
+                                     INTERFACE_INCLUDE_DIRECTORIES "${LZ4_INCLUDE_DIR}")
+  endif()
 endif()
```

### Comparing `pyarrow-8.0.0/cmake_modules/FindNumPy.cmake` & `pyarrow-9.0.0/cmake_modules/FindNumPy.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindORC.cmake` & `pyarrow-9.0.0/cmake_modules/FindORC.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindOpenSSLAlt.cmake` & `pyarrow-9.0.0/cmake_modules/FindOpenSSLAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindParquet.cmake` & `pyarrow-9.0.0/cmake_modules/FindParquet.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindPlasma.cmake` & `pyarrow-9.0.0/cmake_modules/FindPlasma.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindPython3Alt.cmake` & `pyarrow-9.0.0/cmake_modules/FindPython3Alt.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -19,48 +19,46 @@
 # and the NumPy package, and sets the following variables:
 # - PYTHON_EXECUTABLE
 # - PYTHON_INCLUDE_DIRS
 # - PYTHON_LIBRARIES
 # - PYTHON_OTHER_LIBS
 # - NUMPY_INCLUDE_DIRS
 
+set(Python3Alt_FIND_PACKAGE_OPTIONS)
+set(Python3Alt_NumPy_FIND_PACKAGE_OPTIONS)
+if(Python3Alt_FIND_VERSION)
+  list(APPEND Python3Alt_FIND_PACKAGE_OPTIONS ${Python3Alt_FIND_VERSION})
+endif()
+if(Python3Alt_FIND_REQUIRED)
+  list(APPEND Python3Alt_FIND_PACKAGE_OPTIONS REQUIRED)
+  list(APPEND Python3Alt_NumPy_FIND_PACKAGE_OPTIONS REQUIRED)
+endif()
+if(Python3Alt_FIND_QUIETLY)
+  list(APPEND Python3Alt_FIND_PACKAGE_OPTIONS QUIET)
+  list(APPEND Python3Alt_NumPy_FIND_PACKAGE_OPTIONS QUIET)
+endif()
+
 # Need CMake 3.15 or later for Python3_FIND_STRATEGY
 if(${CMAKE_VERSION} VERSION_LESS "3.15.0")
-  # Use deprecated Python- and NumPy-finding code
-  if(Python3Alt_FIND_REQUIRED)
-    find_package(PythonLibsNew REQUIRED)
-    find_package(NumPy REQUIRED)
-  else()
-    find_package(PythonLibsNew)
-    find_package(NumPy)
-  endif()
+  find_package(PythonLibsNew ${Python3Alt_FIND_PACKAGE_OPTIONS})
+  find_package(NumPy ${Python3Alt_NumPy_FIND_PACKAGE_OPTIONS})
   find_package_handle_standard_args(
     Python3Alt REQUIRED_VARS PYTHON_EXECUTABLE PYTHON_INCLUDE_DIRS NUMPY_INCLUDE_DIRS)
   return()
 endif()
 
 if(${CMAKE_VERSION} VERSION_LESS "3.18.0" OR ARROW_BUILD_TESTS)
   # When building arrow-python-test, we need libpython to be present, so ask for
   # the full "Development" component.  Also ask for it on CMake < 3.18,
   # where "Development.Module" is not available.
-  if(Python3Alt_FIND_REQUIRED)
-    find_package(Python3
-                 COMPONENTS Interpreter Development NumPy
-                 REQUIRED)
-  else()
-    find_package(Python3 COMPONENTS Interpreter Development NumPy)
-  endif()
+  find_package(Python3 ${Python3Alt_FIND_PACKAGE_OPTIONS} COMPONENTS Interpreter
+                                                                     Development NumPy)
 else()
-  if(Python3Alt_FIND_REQUIRED)
-    find_package(Python3
-                 COMPONENTS Interpreter Development.Module NumPy
-                 REQUIRED)
-  else()
-    find_package(Python3 COMPONENTS Interpreter Development.Module NumPy)
-  endif()
+  find_package(Python3 ${Python3Alt_FIND_PACKAGE_OPTIONS}
+               COMPONENTS Interpreter Development.Module NumPy)
 endif()
 
 if(NOT Python3_FOUND)
   return()
 endif()
 
 set(PYTHON_EXECUTABLE ${Python3_EXECUTABLE})
```

### Comparing `pyarrow-8.0.0/cmake_modules/FindPythonLibsNew.cmake` & `pyarrow-9.0.0/cmake_modules/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindRapidJSONAlt.cmake` & `pyarrow-9.0.0/cmake_modules/FindRapidJSONAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindSQLite3Alt.cmake` & `pyarrow-9.0.0/cmake_modules/FindSQLite3Alt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindSnappy.cmake` & `pyarrow-9.0.0/cmake_modules/FindSnappyAlt.cmake`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,48 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
+set(find_package_args)
+if(SnappyAlt_FIND_VERSION)
+  list(APPEND find_package_args ${SnappyAlt_FIND_VERSION})
+endif()
+if(SnappyAlt_FIND_QUIETLY)
+  list(APPEND find_package_args QUIET)
+endif()
+find_package(Snappy ${find_package_args})
+if(Snappy_FOUND)
+  if(ARROW_SNAPPY_USE_SHARED)
+    set(Snappy_TARGET Snappy::snappy)
+    set(SnappyAlt_FOUND TRUE)
+    return()
+  else()
+    if(TARGET Snappy::snappy-static)
+      # The official SnappyTargets.cmake uses Snappy::snappy-static for
+      # static version.
+      set(Snappy_TARGET Snappy::snappy-static)
+      set(SnappyAlt_FOUND TRUE)
+      return()
+    else()
+      # The Conan's Snappy package always uses Snappy::snappy and it's
+      # an INTERFACE_LIBRARY.
+      get_target_property(Snappy Snappy::snappy TYPE)
+      if(Snappy_TYPE STREQUAL "STATIC_LIBRARY" OR Snappy_TYPE STREQUAL
+                                                  "INTERFACE_LIBRARY")
+        set(Snappy_TARGET Snappy::snappy)
+        set(SnappyAlt_FOUND TRUE)
+        return()
+      endif()
+    endif()
+  endif()
+endif()
+
 if(ARROW_SNAPPY_USE_SHARED)
   set(SNAPPY_LIB_NAMES)
   if(CMAKE_IMPORT_LIBRARY_SUFFIX)
     list(APPEND SNAPPY_LIB_NAMES
          "${CMAKE_IMPORT_LIBRARY_PREFIX}snappy${CMAKE_IMPORT_LIBRARY_SUFFIX}")
   endif()
   list(APPEND SNAPPY_LIB_NAMES
@@ -48,15 +82,22 @@
 else()
   find_library(Snappy_LIB NAMES ${SNAPPY_LIB_NAMES})
   find_path(Snappy_INCLUDE_DIR
             NAMES snappy.h
             PATH_SUFFIXES ${ARROW_INCLUDE_PATH_SUFFIXES})
 endif()
 
-find_package_handle_standard_args(Snappy REQUIRED_VARS Snappy_LIB Snappy_INCLUDE_DIR)
+find_package_handle_standard_args(SnappyAlt REQUIRED_VARS Snappy_LIB Snappy_INCLUDE_DIR)
 
-if(Snappy_FOUND)
-  add_library(Snappy::snappy UNKNOWN IMPORTED)
-  set_target_properties(Snappy::snappy
+if(SnappyAlt_FOUND)
+  if(ARROW_SNAPPY_USE_SHARED)
+    set(Snappy_TARGET Snappy::snappy)
+    set(Snappy_TARGET_TYPE SHARED)
+  else()
+    set(Snappy_TARGET Snappy::snappy-static)
+    set(Snappy_TARGET_TYPE STATIC)
+  endif()
+  add_library(${Snappy_TARGET} ${Snappy_TARGET_TYPE} IMPORTED)
+  set_target_properties(${Snappy_TARGET}
                         PROPERTIES IMPORTED_LOCATION "${Snappy_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${Snappy_INCLUDE_DIR}")
 endif()
```

### Comparing `pyarrow-8.0.0/cmake_modules/FindThrift.cmake` & `pyarrow-9.0.0/cmake_modules/FindThrift.cmake`

 * *Files 7% similar despite different names*

```diff
@@ -18,41 +18,50 @@
 # to be set before calling find_package:
 #
 #  Thrift_ROOT - When set, this path is inspected instead of standard library
 #                locations as the root of the Thrift installation.
 #                The environment variable THRIFT_HOME overrides this variable.
 #
 # This module defines
-#  THRIFT_VERSION, version string of ant if found
-#  THRIFT_INCLUDE_DIR, where to find THRIFT headers
-#  THRIFT_LIB, THRIFT library
-#  THRIFT_FOUND, If false, do not try to use ant
+#  Thrift_FOUND, whether Thrift is found or not
+#  Thrift_COMPILER_FOUND, whether Thrift compiler is found or not
+#
+#  thrift::thrift, a library target to use Thrift
+#  thrift::compiler, a executable target to use Thrift compiler
 
 function(EXTRACT_THRIFT_VERSION)
   if(THRIFT_INCLUDE_DIR)
     file(READ "${THRIFT_INCLUDE_DIR}/thrift/config.h" THRIFT_CONFIG_H_CONTENT)
     string(REGEX MATCH "#define PACKAGE_VERSION \"[0-9.]+\"" THRIFT_VERSION_DEFINITION
                  "${THRIFT_CONFIG_H_CONTENT}")
-    string(REGEX MATCH "[0-9.]+" THRIFT_VERSION "${THRIFT_VERSION_DEFINITION}")
-    set(THRIFT_VERSION
-        "${THRIFT_VERSION}"
+    string(REGEX MATCH "[0-9.]+" Thrift_VERSION "${THRIFT_VERSION_DEFINITION}")
+    set(Thrift_VERSION
+        "${Thrift_VERSION}"
         PARENT_SCOPE)
   else()
-    set(THRIFT_VERSION
+    set(Thrift_VERSION
         ""
         PARENT_SCOPE)
   endif()
 endfunction(EXTRACT_THRIFT_VERSION)
 
 if(MSVC_TOOLCHAIN AND NOT DEFINED THRIFT_MSVC_LIB_SUFFIX)
   if(NOT ARROW_THRIFT_USE_SHARED)
     if(ARROW_USE_STATIC_CRT)
-      set(THRIFT_MSVC_LIB_SUFFIX "mt")
+      if("${CMAKE_BUILD_TYPE}" STREQUAL "DEBUG")
+        set(THRIFT_MSVC_LIB_SUFFIX "mtd")
+      else()
+        set(THRIFT_MSVC_LIB_SUFFIX "mt")
+      endif()
     else()
-      set(THRIFT_MSVC_LIB_SUFFIX "md")
+      if("${CMAKE_BUILD_TYPE}" STREQUAL "DEBUG")
+        set(THRIFT_MSVC_LIB_SUFFIX "mdd")
+      else()
+        set(THRIFT_MSVC_LIB_SUFFIX "md")
+      endif()
     endif()
   endif()
 endif()
 set(THRIFT_LIB_NAME_BASE "thrift${THRIFT_MSVC_LIB_SUFFIX}")
 
 if(ARROW_THRIFT_USE_SHARED)
   set(THRIFT_LIB_NAMES thrift)
@@ -98,15 +107,15 @@
                  NAMES ${THRIFT_LIB_NAMES}
                  PATHS ${THRIFT_PC_LIBRARY_DIRS}
                  NO_DEFAULT_PATH)
     find_program(THRIFT_COMPILER thrift
                  HINTS ${THRIFT_PC_PREFIX}
                  NO_DEFAULT_PATH
                  PATH_SUFFIXES "bin")
-    set(THRIFT_VERSION ${THRIFT_PC_VERSION})
+    set(Thrift_VERSION ${THRIFT_PC_VERSION})
   else()
     find_library(THRIFT_LIB
                  NAMES ${THRIFT_LIB_NAMES}
                  PATH_SUFFIXES "lib/${CMAKE_LIBRARY_ARCHITECTURE}" "lib")
     find_path(THRIFT_INCLUDE_DIR thrift/Thrift.h PATH_SUFFIXES "include")
     find_program(THRIFT_COMPILER thrift PATH_SUFFIXES "bin")
     extract_thrift_version()
@@ -118,27 +127,32 @@
 else()
   set(Thrift_COMPILER_FOUND FALSE)
 endif()
 
 find_package_handle_standard_args(
   Thrift
   REQUIRED_VARS THRIFT_LIB THRIFT_INCLUDE_DIR
-  VERSION_VAR THRIFT_VERSION
+  VERSION_VAR Thrift_VERSION
   HANDLE_COMPONENTS)
 
-if(Thrift_FOUND OR THRIFT_FOUND)
-  set(Thrift_FOUND TRUE)
+if(Thrift_FOUND)
   if(ARROW_THRIFT_USE_SHARED)
     add_library(thrift::thrift SHARED IMPORTED)
   else()
     add_library(thrift::thrift STATIC IMPORTED)
   endif()
   set_target_properties(thrift::thrift
                         PROPERTIES IMPORTED_LOCATION "${THRIFT_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${THRIFT_INCLUDE_DIR}")
   if(WIN32 AND NOT MSVC_TOOLCHAIN)
     # We don't need this for Visual C++ because Thrift uses
     # "#pragma comment(lib, "Ws2_32.lib")" in
     # thrift/windows/config.h for Visual C++.
     set_target_properties(thrift::thrift PROPERTIES INTERFACE_LINK_LIBRARIES "ws2_32")
   endif()
+
+  if(Thrift_COMPILER_FOUND)
+    add_executable(thrift::compiler IMPORTED)
+    set_target_properties(thrift::compiler PROPERTIES IMPORTED_LOCATION
+                                                      "${THRIFT_COMPILER}")
+  endif()
 endif()
```

### Comparing `pyarrow-8.0.0/cmake_modules/Findc-aresAlt.cmake` & `pyarrow-9.0.0/cmake_modules/Findc-aresAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindgRPCAlt.cmake` & `pyarrow-9.0.0/cmake_modules/FindgRPCAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/FindgflagsAlt.cmake` & `pyarrow-9.0.0/cmake_modules/FindgflagsAlt.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/Findlibrados.cmake` & `pyarrow-9.0.0/cmake_modules/Findlibrados.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/Findre2Alt.cmake` & `pyarrow-9.0.0/cmake_modules/Findre2Alt.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 endif()
 find_package(re2 ${find_package_args})
 if(re2_FOUND)
   set(re2Alt_FOUND TRUE)
   return()
 endif()
 
-if(RE2_ROOT)
+if(re2_ROOT)
   find_library(RE2_LIB
                NAMES re2_static
                      re2
                      "${CMAKE_STATIC_LIBRARY_PREFIX}re2${RE2_MSVC_STATIC_LIB_SUFFIX}${CMAKE_STATIC_LIBRARY_SUFFIX}"
                      "${CMAKE_SHARED_LIBRARY_PREFIX}re2${CMAKE_SHARED_LIBRARY_SUFFIX}"
-               PATHS ${RE2_ROOT}
+               PATHS ${re2_ROOT}
                PATH_SUFFIXES ${ARROW_LIBRARY_PATH_SUFFIXES}
                NO_DEFAULT_PATH)
   find_path(RE2_INCLUDE_DIR
             NAMES re2/re2.h
             PATHS ${RE2_ROOT}
             NO_DEFAULT_PATH
             PATH_SUFFIXES ${ARROW_INCLUDE_PATH_SUFFIXES})
```

### Comparing `pyarrow-8.0.0/cmake_modules/Findutf8proc.cmake` & `pyarrow-9.0.0/cmake_modules/Findutf8proc.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -91,11 +91,11 @@
   set(utf8proc_FOUND TRUE)
   add_library(utf8proc::utf8proc UNKNOWN IMPORTED)
   set_target_properties(utf8proc::utf8proc
                         PROPERTIES IMPORTED_LOCATION "${utf8proc_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${utf8proc_INCLUDE_DIR}")
   if(NOT ARROW_UTF8PROC_USE_SHARED)
-    set_target_properties(utf8proc::utf8proc PROPERTIES INTERFACE_COMPILER_DEFINITIONS
+    set_target_properties(utf8proc::utf8proc PROPERTIES INTERFACE_COMPILE_DEFINITIONS
                                                         "UTF8PROC_STATIC")
   endif()
 endif()
```

### Comparing `pyarrow-8.0.0/cmake_modules/Findzstd.cmake` & `pyarrow-9.0.0/cmake_modules/Findzstd.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/SetupCxxFlags.cmake` & `pyarrow-9.0.0/cmake_modules/SetupCxxFlags.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 # ARROW-6848: Do not use GNU (or other CXX) extensions
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 # Build with -fPIC so that can static link our libraries into other people's
 # shared libraries
-set(CMAKE_POSITION_INDEPENDENT_CODE ON)
+set(CMAKE_POSITION_INDEPENDENT_CODE ${ARROW_POSITION_INDEPENDENT_CODE})
 
 string(TOUPPER ${CMAKE_BUILD_TYPE} CMAKE_BUILD_TYPE)
 
 set(UNKNOWN_COMPILER_MESSAGE
     "Unknown compiler: ${CMAKE_CXX_COMPILER_ID} ${CMAKE_CXX_COMPILER_VERSION}")
 
 # compiler flags that are common across debug/release builds
@@ -282,18 +282,18 @@
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wall")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wextra")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wdocumentation")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wshorten-64-to-32")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-missing-braces")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-unused-parameter")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-constant-logical-operand")
+    set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-return-stack-address")
   elseif(CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wall")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-conversion")
-    set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-deprecated-declarations")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wno-sign-conversion")
     set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} -Wunused-result")
   elseif(CMAKE_CXX_COMPILER_ID STREQUAL "Intel")
     if(WIN32)
       set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} /Wall")
       set(CXX_COMMON_FLAGS "${CXX_COMMON_FLAGS} /Wno-deprecated")
     else()
@@ -543,16 +543,16 @@
     # We can't use the gold linker if it's inside devtoolset because the compiler
     # won't find it when invoked directly from make/ninja (which is typically
     # done outside devtoolset).
     execute_process(COMMAND which ld.gold
                     OUTPUT_VARIABLE GOLD_LOCATION
                     OUTPUT_STRIP_TRAILING_WHITESPACE ERROR_QUIET)
     if("${GOLD_LOCATION}" MATCHES "^/opt/rh/devtoolset")
-      message("Skipping optional gold linker (version ${GOLD_VERSION}) because "
-              "it's in devtoolset")
+      message(STATUS "Skipping optional gold linker (version ${GOLD_VERSION}) because "
+                     "it's in devtoolset")
       set(GOLD_VERSION)
     endif()
   endif()
 
   if(GOLD_VERSION)
     # Older versions of the gold linker are vulnerable to a bug [1] which
     # prevents weak symbols from being overridden properly. This leads to
@@ -566,31 +566,31 @@
     #   - Drop tcmalloc in all other builds.
     #
     # 1. https://sourceware.org/bugzilla/show_bug.cgi?id=16979.
     if("${GOLD_VERSION}" VERSION_LESS "1.12")
       set(ARROW_BUGGY_GOLD 1)
     endif()
     if(MUST_USE_GOLD)
-      message("Using hard-wired gold linker (version ${GOLD_VERSION})")
+      message(STATUS "Using hard-wired gold linker (version ${GOLD_VERSION})")
       if(ARROW_BUGGY_GOLD)
         if("${ARROW_LINK}" STREQUAL "d" AND "${CMAKE_BUILD_TYPE}" STREQUAL "RELEASE")
           message(SEND_ERROR "Configured to use buggy gold with dynamic linking "
                              "in a RELEASE build")
         endif()
       endif()
     elseif(NOT ARROW_BUGGY_GOLD)
       # The Gold linker must be manually enabled.
       set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fuse-ld=gold")
       set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fuse-ld=gold")
-      message("Using optional gold linker (version ${GOLD_VERSION})")
+      message(STATUS "Using optional gold linker (version ${GOLD_VERSION})")
     else()
-      message("Optional gold linker is buggy, using ld linker instead")
+      message(STATUS "Optional gold linker is buggy, using ld linker instead")
     endif()
   else()
-    message("Using ld linker")
+    message(STATUS "Using ld linker")
   endif()
 endif()
 
 # compiler flags for different build types (run 'cmake -DCMAKE_BUILD_TYPE=<type> .')
 # For all builds:
 # For CMAKE_BUILD_TYPE=Debug
 #   -ggdb: Enable gdb debugging
@@ -620,15 +620,15 @@
 
 set(C_FLAGS_PROFILE_GEN "${CXX_FLAGS_RELEASE} -fprofile-generate")
 set(C_FLAGS_PROFILE_BUILD "${CXX_FLAGS_RELEASE} -fprofile-use")
 set(CXX_FLAGS_PROFILE_GEN "${CXX_FLAGS_RELEASE} -fprofile-generate")
 set(CXX_FLAGS_PROFILE_BUILD "${CXX_FLAGS_RELEASE} -fprofile-use")
 
 # Set compile flags based on the build type.
-message("Configured for ${CMAKE_BUILD_TYPE} build (set with cmake -DCMAKE_BUILD_TYPE={release,debug,...})"
+message(STATUS "Configured for ${CMAKE_BUILD_TYPE} build (set with cmake -DCMAKE_BUILD_TYPE={release,debug,...})"
 )
 if("${CMAKE_BUILD_TYPE}" STREQUAL "DEBUG")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${C_FLAGS_DEBUG}")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${CXX_FLAGS_DEBUG}")
 elseif("${CMAKE_BUILD_TYPE}" STREQUAL "RELWITHDEBINFO")
 
 elseif("${CMAKE_BUILD_TYPE}" STREQUAL "FASTDEBUG")
```

### Comparing `pyarrow-8.0.0/cmake_modules/ThirdpartyToolchain.cmake` & `pyarrow-9.0.0/cmake_modules/ThirdpartyToolchain.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -57,38 +57,32 @@
     BZip2
     c-ares
     gflags
     GLOG
     google_cloud_cpp_storage
     gRPC
     GTest
+    jemalloc
     LLVM
-    Lz4
+    lz4
     nlohmann_json
     opentelemetry-cpp
     ORC
     re2
     Protobuf
     RapidJSON
     Snappy
     Substrait
     Thrift
+    ucx
     utf8proc
     xsimd
     ZLIB
     zstd)
 
-# TODO(wesm): External GTest shared libraries are not currently
-# supported when building with MSVC because of the way that
-# conda-forge packages have 4 variants of the libraries packaged
-# together
-if(MSVC AND "${GTest_SOURCE}" STREQUAL "")
-  set(GTest_SOURCE "BUNDLED")
-endif()
-
 # For backward compatibility. We use "BOOST_SOURCE" if "Boost_SOURCE"
 # isn't specified and "BOOST_SOURCE" is specified.
 # We renamed "BOOST" dependency name to "Boost" in 3.0.0 because
 # upstreams (CMake and Boost) use "Boost" not "BOOST" as package name.
 if("${Boost_SOURCE}" STREQUAL "" AND NOT "${BOOST_SOURCE}" STREQUAL "")
   set(Boost_SOURCE ${BOOST_SOURCE})
 endif()
@@ -97,14 +91,33 @@
 # isn't specified and "RE2_SOURCE" is specified.
 # We renamed "RE2" dependency name to "re2" in 3.0.0 because
 # upstream uses "re2" not "RE2" as package name.
 if("${re2_SOURCE}" STREQUAL "" AND NOT "${RE2_SOURCE}" STREQUAL "")
   set(re2_SOURCE ${RE2_SOURCE})
 endif()
 
+# For backward compatibility. We use "RE2_ROOT" if "re2_ROOT"
+# isn't specified and "RE2_ROOT" is specified.
+if("${re2_ROOT}" STREQUAL "" AND NOT "${RE2_ROOT}" STREQUAL "")
+  set(re2_ROOT ${RE2_ROOT})
+endif()
+
+# For backward compatibility. We use "Lz4_SOURCE" if "lz4_SOURCE"
+# isn't specified and "lz4_SOURCE" is specified.
+# We renamed "Lz4" dependency name to "lz4" in 9.0.0 because
+# upstream uses "lz4" not "Lz4" as package name.
+if("${lz4_SOURCE}" STREQUAL "" AND NOT "${Lz4_SOURCE}" STREQUAL "")
+  set(lz4_SOURCE ${Lz4_SOURCE})
+endif()
+
+# For backward compatibility. We use bundled jemalloc by default.
+if("${jemalloc_SOURCE}" STREQUAL "")
+  set(jemalloc_SOURCE "BUNDLED")
+endif()
+
 message(STATUS "Using ${ARROW_DEPENDENCY_SOURCE} approach to find dependencies")
 
 if(ARROW_DEPENDENCY_SOURCE STREQUAL "CONDA")
   if(MSVC)
     set(ARROW_PACKAGE_PREFIX "$ENV{CONDA_PREFIX}/Library")
   else()
     set(ARROW_PACKAGE_PREFIX $ENV{CONDA_PREFIX})
@@ -157,15 +170,17 @@
     build_glog()
   elseif("${DEPENDENCY_NAME}" STREQUAL "google_cloud_cpp_storage")
     build_google_cloud_cpp_storage()
   elseif("${DEPENDENCY_NAME}" STREQUAL "gRPC")
     build_grpc()
   elseif("${DEPENDENCY_NAME}" STREQUAL "GTest")
     build_gtest()
-  elseif("${DEPENDENCY_NAME}" STREQUAL "Lz4")
+  elseif("${DEPENDENCY_NAME}" STREQUAL "jemalloc")
+    build_jemalloc()
+  elseif("${DEPENDENCY_NAME}" STREQUAL "lz4")
     build_lz4()
   elseif("${DEPENDENCY_NAME}" STREQUAL "nlohmann_json")
     build_nlohmann_json()
   elseif("${DEPENDENCY_NAME}" STREQUAL "opentelemetry-cpp")
     build_opentelemetry()
   elseif("${DEPENDENCY_NAME}" STREQUAL "ORC")
     build_orc()
@@ -177,14 +192,16 @@
     build_re2()
   elseif("${DEPENDENCY_NAME}" STREQUAL "Snappy")
     build_snappy()
   elseif("${DEPENDENCY_NAME}" STREQUAL "Substrait")
     build_substrait()
   elseif("${DEPENDENCY_NAME}" STREQUAL "Thrift")
     build_thrift()
+  elseif("${DEPENDENCY_NAME}" STREQUAL "ucx")
+    build_ucx()
   elseif("${DEPENDENCY_NAME}" STREQUAL "utf8proc")
     build_utf8proc()
   elseif("${DEPENDENCY_NAME}" STREQUAL "xsimd")
     build_xsimd()
   elseif("${DEPENDENCY_NAME}" STREQUAL "ZLIB")
     build_zlib()
   elseif("${DEPENDENCY_NAME}" STREQUAL "zstd")
@@ -196,23 +213,23 @@
 
 # Find modules are needed by the consumer in case of a static build, or if the
 # linkage is PUBLIC or INTERFACE.
 macro(provide_find_module PACKAGE_NAME)
   set(module_ "${CMAKE_SOURCE_DIR}/cmake_modules/Find${PACKAGE_NAME}.cmake")
   if(EXISTS "${module_}")
     message(STATUS "Providing CMake module for ${PACKAGE_NAME}")
-    install(FILES "${module_}" DESTINATION "${ARROW_CMAKE_INSTALL_DIR}")
+    install(FILES "${module_}" DESTINATION "${ARROW_CMAKE_DIR}")
   endif()
   unset(module_)
 endmacro()
 
 macro(resolve_dependency DEPENDENCY_NAME)
   set(options)
   set(one_value_args HAVE_ALT IS_RUNTIME_DEPENDENCY REQUIRED_VERSION USE_CONFIG)
-  set(multi_value_args PC_PACKAGE_NAMES)
+  set(multi_value_args COMPONENTS PC_PACKAGE_NAMES)
   cmake_parse_arguments(ARG
                         "${options}"
                         "${one_value_args}"
                         "${multi_value_args}"
                         ${ARGN})
   if(ARG_UNPARSED_ARGUMENTS)
     message(SEND_ERROR "Error: unrecognized arguments: ${ARG_UNPARSED_ARGUMENTS}")
@@ -229,14 +246,17 @@
   set(FIND_PACKAGE_ARGUMENTS ${PACKAGE_NAME})
   if(ARG_REQUIRED_VERSION)
     list(APPEND FIND_PACKAGE_ARGUMENTS ${ARG_REQUIRED_VERSION})
   endif()
   if(ARG_USE_CONFIG)
     list(APPEND FIND_PACKAGE_ARGUMENTS CONFIG)
   endif()
+  if(ARG_COMPONENTS)
+    list(APPEND FIND_PACKAGE_ARGUMENTS COMPONENTS ${ARG_COMPONENTS})
+  endif()
   if(${DEPENDENCY_NAME}_SOURCE STREQUAL "AUTO")
     find_package(${FIND_PACKAGE_ARGUMENTS})
     if(${${PACKAGE_NAME}_FOUND})
       set(${DEPENDENCY_NAME}_SOURCE "SYSTEM")
     else()
       build_dependency(${DEPENDENCY_NAME})
       set(${DEPENDENCY_NAME}_SOURCE "BUNDLED")
@@ -264,16 +284,23 @@
 endmacro()
 
 # ----------------------------------------------------------------------
 # Thirdparty versions, environment variables, source URLs
 
 set(THIRDPARTY_DIR "${arrow_SOURCE_DIR}/thirdparty")
 
-# Include vendored Flatbuffers
-include_directories(SYSTEM "${THIRDPARTY_DIR}/flatbuffers/include")
+add_library(arrow::flatbuffers INTERFACE IMPORTED)
+if(CMAKE_VERSION VERSION_LESS 3.11)
+  set_target_properties(arrow::flatbuffers
+                        PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                   "${THIRDPARTY_DIR}/flatbuffers/include")
+else()
+  target_include_directories(arrow::flatbuffers
+                             INTERFACE "${THIRDPARTY_DIR}/flatbuffers/include")
+endif()
 
 # ----------------------------------------------------------------------
 # Some EP's require other EP's
 
 if(PARQUET_REQUIRE_ENCRYPTION)
   set(ARROW_JSON ON)
 endif()
@@ -283,37 +310,31 @@
   set(ARROW_WITH_PROTOBUF ON)
 endif()
 
 if(ARROW_THRIFT)
   set(ARROW_WITH_ZLIB ON)
 endif()
 
-if(ARROW_HIVESERVER2 OR ARROW_PARQUET)
+if(ARROW_PARQUET)
   set(ARROW_WITH_THRIFT ON)
-  if(ARROW_HIVESERVER2)
-    set(ARROW_THRIFT_REQUIRED_COMPONENTS COMPILER)
-  else()
-    set(ARROW_THRIFT_REQUIRED_COMPONENTS)
-  endif()
-else()
-  set(ARROW_WITH_THRIFT OFF)
 endif()
 
 if(ARROW_FLIGHT)
   set(ARROW_WITH_GRPC ON)
 endif()
 
 if(ARROW_WITH_GRPC)
   set(ARROW_WITH_RE2 ON)
   set(ARROW_WITH_ZLIB ON)
 endif()
 
 if(ARROW_GCS)
   set(ARROW_WITH_GOOGLE_CLOUD_CPP ON)
   set(ARROW_WITH_NLOHMANN_JSON ON)
+  set(ARROW_WITH_ZLIB ON)
 endif()
 
 if(ARROW_JSON)
   set(ARROW_WITH_RAPIDJSON ON)
 endif()
 
 if(ARROW_ORC
@@ -457,15 +478,15 @@
 else()
   set_urls(CARES_SOURCE_URL
            "https://c-ares.haxx.se/download/c-ares-${ARROW_CARES_BUILD_VERSION}.tar.gz"
            "${THIRDPARTY_MIRROR_URL}/cares-${ARROW_CARES_BUILD_VERSION}.tar.gz")
 endif()
 
 if(DEFINED ENV{ARROW_CRC32C_URL})
-  set(CRC32C_URL "$ENV{ARROW_CRC32C_URL}")
+  set(CRC32C_SOURCE_URL "$ENV{ARROW_CRC32C_URL}")
 else()
   set_urls(CRC32C_SOURCE_URL
            "https://github.com/google/crc32c/archive/${ARROW_CRC32C_BUILD_VERSION}.tar.gz"
   )
 endif()
 
 if(DEFINED ENV{ARROW_GBENCHMARK_URL})
@@ -647,14 +668,21 @@
            "https://mirrors.koehn.com/apache/thrift/${ARROW_THRIFT_BUILD_VERSION}/thrift-${ARROW_THRIFT_BUILD_VERSION}.tar.gz"
            "https://mirrors.ocf.berkeley.edu/apache/thrift/${ARROW_THRIFT_BUILD_VERSION}/thrift-${ARROW_THRIFT_BUILD_VERSION}.tar.gz"
            "https://mirrors.sonic.net/apache/thrift/${ARROW_THRIFT_BUILD_VERSION}/thrift-${ARROW_THRIFT_BUILD_VERSION}.tar.gz"
            "https://us.mirrors.quenda.co/apache/thrift/${ARROW_THRIFT_BUILD_VERSION}/thrift-${ARROW_THRIFT_BUILD_VERSION}.tar.gz"
            "${THIRDPARTY_MIRROR_URL}/thrift-${ARROW_THRIFT_BUILD_VERSION}.tar.gz")
 endif()
 
+if(DEFINED ENV{ARROW_UCX_URL})
+  set(ARROW_UCX_SOURCE_URL "$ENV{ARROW_UCX_URL}")
+else()
+  set_urls(ARROW_UCX_SOURCE_URL
+           "https://github.com/openucx/ucx/archive/v${ARROW_UCX_BUILD_VERSION}.tar.gz")
+endif()
+
 if(DEFINED ENV{ARROW_UTF8PROC_URL})
   set(ARROW_UTF8PROC_SOURCE_URL "$ENV{ARROW_UTF8PROC_URL}")
 else()
   set_urls(ARROW_UTF8PROC_SOURCE_URL
            "https://github.com/JuliaStrings/utf8proc/archive/${ARROW_UTF8PROC_BUILD_VERSION}.tar.gz"
   )
 endif()
@@ -726,14 +754,21 @@
     -DCMAKE_CXX_FLAGS=${EP_CXX_FLAGS}
     -DCMAKE_CXX_FLAGS_${UPPERCASE_BUILD_TYPE}=${EP_CXX_FLAGS}
     -DCMAKE_CXX_STANDARD=${CMAKE_CXX_STANDARD}
     -DCMAKE_EXPORT_NO_PACKAGE_REGISTRY=${CMAKE_EXPORT_NO_PACKAGE_REGISTRY}
     -DCMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY=${CMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY}
     -DCMAKE_VERBOSE_MAKEFILE=${CMAKE_VERBOSE_MAKEFILE})
 
+# Enable s/ccache if set by parent.
+if(CMAKE_C_COMPILER_LAUNCHER AND CMAKE_CXX_COMPILER_LAUNCHER)
+  list(APPEND EP_COMMON_CMAKE_ARGS
+       -DCMAKE_C_COMPILER_LAUNCHER=${CMAKE_C_COMPILER_LAUNCHER}
+       -DCMAKE_CXX_COMPILER_LAUNCHER=${CMAKE_CXX_COMPILER_LAUNCHER})
+endif()
+
 if(NOT ARROW_VERBOSE_THIRDPARTY_BUILD)
   set(EP_LOG_OPTIONS
       LOG_CONFIGURE
       1
       LOG_BUILD
       1
       LOG_INSTALL
@@ -774,14 +809,15 @@
 # Add Boost dependencies (code adapted from Apache Kudu)
 
 macro(build_boost)
   set(BOOST_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/boost_ep-prefix/src/boost_ep")
 
   # This is needed by the thrift_ep build
   set(BOOST_ROOT ${BOOST_PREFIX})
+  set(Boost_INCLUDE_DIR "${BOOST_PREFIX}")
 
   if(ARROW_BOOST_REQUIRE_LIBRARY)
     set(BOOST_LIB_DIR "${BOOST_PREFIX}/stage/lib")
     set(BOOST_BUILD_LINK "static")
     if("${CMAKE_BUILD_TYPE}" STREQUAL "DEBUG")
       set(BOOST_BUILD_VARIANT "debug")
     else()
@@ -833,44 +869,69 @@
         "${BOOST_LIB_DIR}/libboost_filesystem${BOOST_LIBRARY_SUFFIX}${CMAKE_STATIC_LIBRARY_SUFFIX}"
     )
     set(BOOST_SYSTEM_LIBRARY boost_system_static)
     set(BOOST_FILESYSTEM_LIBRARY boost_filesystem_static)
     set(BOOST_BUILD_PRODUCTS ${BOOST_STATIC_SYSTEM_LIBRARY}
                              ${BOOST_STATIC_FILESYSTEM_LIBRARY})
 
-    add_thirdparty_lib(boost_system STATIC_LIB "${BOOST_STATIC_SYSTEM_LIBRARY}")
-
-    add_thirdparty_lib(boost_filesystem STATIC_LIB "${BOOST_STATIC_FILESYSTEM_LIBRARY}")
+    add_thirdparty_lib(Boost::system
+                       STATIC
+                       "${BOOST_STATIC_SYSTEM_LIBRARY}"
+                       INCLUDE_DIRECTORIES
+                       "${Boost_INCLUDE_DIR}")
+    add_thirdparty_lib(Boost::filesystem
+                       STATIC
+                       "${BOOST_STATIC_FILESYSTEM_LIBRARY}"
+                       INCLUDE_DIRECTORIES
+                       "${Boost_INCLUDE_DIR}")
 
     externalproject_add(boost_ep
                         URL ${BOOST_SOURCE_URL}
                         URL_HASH "SHA256=${ARROW_BOOST_BUILD_SHA256_CHECKSUM}"
                         BUILD_BYPRODUCTS ${BOOST_BUILD_PRODUCTS}
                         BUILD_IN_SOURCE 1
                         CONFIGURE_COMMAND ${BOOST_CONFIGURE_COMMAND}
                         BUILD_COMMAND ${BOOST_BUILD_COMMAND}
                         INSTALL_COMMAND "" ${EP_LOG_OPTIONS})
-    add_dependencies(boost_system_static boost_ep)
-    add_dependencies(boost_filesystem_static boost_ep)
+    add_dependencies(Boost::system boost_ep)
+    add_dependencies(Boost::filesystem boost_ep)
   else()
     externalproject_add(boost_ep
                         ${EP_LOG_OPTIONS}
                         BUILD_COMMAND ""
                         CONFIGURE_COMMAND ""
                         INSTALL_COMMAND ""
                         URL ${BOOST_SOURCE_URL}
                         URL_HASH "SHA256=${ARROW_BOOST_BUILD_SHA256_CHECKSUM}")
   endif()
-  set(Boost_INCLUDE_DIR "${BOOST_PREFIX}")
-  set(Boost_INCLUDE_DIRS "${Boost_INCLUDE_DIR}")
-  add_dependencies(toolchain boost_ep)
+  add_library(Boost::headers INTERFACE IMPORTED)
+  if(CMAKE_VERSION VERSION_LESS 3.11)
+    set_target_properties(Boost::headers PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                                    "${Boost_INCLUDE_DIR}")
+  else()
+    target_include_directories(Boost::headers INTERFACE "${Boost_INCLUDE_DIR}")
+  endif()
+  add_dependencies(Boost::headers boost_ep)
+  # If Boost is found but one of system or filesystem components aren't found,
+  # Boost::disable_autolinking and Boost::dynamic_linking are already defined.
+  if(NOT TARGET Boost::disable_autolinking)
+    add_library(Boost::disable_autolinking INTERFACE IMPORTED)
+    if(WIN32)
+      target_compile_definitions(Boost::disable_autolinking INTERFACE "BOOST_ALL_NO_LIB")
+    endif()
+  endif()
+  if(NOT TARGET Boost::dynamic_linking)
+    # This doesn't add BOOST_ALL_DYN_LINK because bundled Boost is a static library.
+    add_library(Boost::dynamic_linking INTERFACE IMPORTED)
+    add_dependencies(toolchain boost_ep)
+  endif()
   set(BOOST_VENDORED TRUE)
 endmacro()
 
-if(ARROW_FLIGHT AND ARROW_BUILD_TESTS)
+if(ARROW_BUILD_TESTS)
   set(ARROW_BOOST_REQUIRED_VERSION "1.64")
 else()
   set(ARROW_BOOST_REQUIRED_VERSION "1.58")
 endif()
 
 set(Boost_USE_MULTITHREADED ON)
 if(MSVC AND ARROW_USE_STATIC_CRT)
@@ -906,42 +967,14 @@
     "1.62.0"
     "1.61"
     "1.61.0"
     "1.62"
     "1.60.0"
     "1.60")
 
-# Thrift needs Boost if we're building the bundled version with version < 0.13,
-# so we first need to determine whether we're building it
-if(ARROW_WITH_THRIFT AND Thrift_SOURCE STREQUAL "AUTO")
-  find_package(Thrift 0.11.0 MODULE COMPONENTS ${ARROW_THRIFT_REQUIRED_COMPONENTS})
-  if(Thrift_FOUND)
-    find_package(PkgConfig QUIET)
-    pkg_check_modules(THRIFT_PC
-                      thrift
-                      NO_CMAKE_PATH
-                      NO_CMAKE_ENVIRONMENT_PATH
-                      QUIET)
-    if(THRIFT_PC_FOUND)
-      string(APPEND ARROW_PC_REQUIRES_PRIVATE " thrift")
-    endif()
-  else()
-    set(Thrift_SOURCE "BUNDLED")
-  endif()
-endif()
-
-# Thrift < 0.13 has a compile-time header dependency on boost
-if(Thrift_SOURCE STREQUAL "BUNDLED" AND ARROW_THRIFT_BUILD_VERSION VERSION_LESS "0.13")
-  set(THRIFT_REQUIRES_BOOST TRUE)
-elseif(THRIFT_VERSION VERSION_LESS "0.13")
-  set(THRIFT_REQUIRES_BOOST TRUE)
-else()
-  set(THRIFT_REQUIRES_BOOST FALSE)
-endif()
-
 # Compilers that don't support int128_t have a compile-time
 # (header-only) dependency on Boost for int128_t.
 if(ARROW_USE_UBSAN)
   # NOTE: Avoid native int128_t on clang with UBSan as it produces linker errors
   # (such as "undefined reference to '__muloti4'")
   set(ARROW_USE_NATIVE_INT128 FALSE)
 else()
@@ -958,51 +991,91 @@
 # - Gandiva has a compile-time (header-only) dependency on Boost, not runtime.
 # - Tests need Boost at runtime.
 # - S3FS and Flight benchmarks need Boost at runtime.
 if(ARROW_BUILD_INTEGRATION
    OR ARROW_BUILD_TESTS
    OR (ARROW_FLIGHT AND ARROW_BUILD_BENCHMARKS)
    OR (ARROW_S3 AND ARROW_BUILD_BENCHMARKS))
-  set(ARROW_BOOST_REQUIRED TRUE)
+  set(ARROW_USE_BOOST TRUE)
   set(ARROW_BOOST_REQUIRE_LIBRARY TRUE)
 elseif(ARROW_GANDIVA
-       OR (ARROW_WITH_THRIFT AND THRIFT_REQUIRES_BOOST)
+       OR ARROW_WITH_THRIFT
        OR (NOT ARROW_USE_NATIVE_INT128))
-  set(ARROW_BOOST_REQUIRED TRUE)
+  set(ARROW_USE_BOOST TRUE)
   set(ARROW_BOOST_REQUIRE_LIBRARY FALSE)
 else()
-  set(ARROW_BOOST_REQUIRED FALSE)
+  set(ARROW_USE_BOOST FALSE)
 endif()
 
-if(ARROW_BOOST_REQUIRED)
+if(ARROW_USE_BOOST)
+  if(ARROW_BOOST_USE_SHARED)
+    # Find shared Boost libraries.
+    set(Boost_USE_STATIC_LIBS OFF)
+    set(BUILD_SHARED_LIBS_KEEP ${BUILD_SHARED_LIBS})
+    set(BUILD_SHARED_LIBS ON)
+  else()
+    # Find static boost headers and libs
+    set(Boost_USE_STATIC_LIBS ON)
+  endif()
   resolve_dependency(Boost
-                     HAVE_ALT
-                     TRUE
                      REQUIRED_VERSION
                      ${ARROW_BOOST_REQUIRED_VERSION}
+                     COMPONENTS
+                     system
+                     filesystem
                      IS_RUNTIME_DEPENDENCY
                      # libarrow.so doesn't depend on libboost*.
                      FALSE)
+  if(ARROW_BOOST_USE_SHARED)
+    set(BUILD_SHARED_LIBS ${BUILD_SHARED_LIBS_KEEP})
+    unset(BUILD_SHARED_LIBS_KEEP)
+  endif()
 
-  if(TARGET Boost::system)
-    set(BOOST_SYSTEM_LIBRARY Boost::system)
-    set(BOOST_FILESYSTEM_LIBRARY Boost::filesystem)
-  elseif(BoostAlt_FOUND)
-    set(BOOST_SYSTEM_LIBRARY ${Boost_SYSTEM_LIBRARY})
-    set(BOOST_FILESYSTEM_LIBRARY ${Boost_FILESYSTEM_LIBRARY})
-  else()
-    set(BOOST_SYSTEM_LIBRARY boost_system_static)
-    set(BOOST_FILESYSTEM_LIBRARY boost_filesystem_static)
+  # For CMake < 3.15
+  if(NOT TARGET Boost::headers)
+    add_library(Boost::headers INTERFACE IMPORTED)
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_target_properties(Boost::headers PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                                      "${Boost_INCLUDE_DIR}")
+    else()
+      target_include_directories(Boost::headers INTERFACE "${Boost_INCLUDE_DIR}")
+    endif()
   endif()
-  set(ARROW_BOOST_LIBS ${BOOST_SYSTEM_LIBRARY} ${BOOST_FILESYSTEM_LIBRARY})
 
-  message(STATUS "Boost include dir: ${Boost_INCLUDE_DIR}")
-  message(STATUS "Boost libraries: ${ARROW_BOOST_LIBS}")
+  foreach(BOOST_LIBRARY Boost::headers Boost::filesystem Boost::system)
+    if(NOT TARGET ${BOOST_LIBRARY})
+      continue()
+    endif()
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_target_properties(${BOOST_LIBRARY} PROPERTIES INTERFACE_LINK_LIBRARIES
+                                                        Boost::disable_autolinking)
+    else()
+      target_link_libraries(${BOOST_LIBRARY} INTERFACE Boost::disable_autolinking)
+    endif()
+    if(ARROW_BOOST_USE_SHARED)
+      if(CMAKE_VERSION VERSION_LESS 3.11)
+        set_target_properties(${BOOST_LIBRARY} PROPERTIES INTERFACE_LINK_LIBRARIES
+                                                          Boost::dynamic_linking)
+      else()
+        target_link_libraries(${BOOST_LIBRARY} INTERFACE Boost::dynamic_linking)
+      endif()
+    endif()
+  endforeach()
+
+  if(WIN32 AND CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
+    # boost/process/detail/windows/handle_workaround.hpp doesn't work
+    # without BOOST_USE_WINDOWS_H with MinGW because MinGW doesn't
+    # provide __kernel_entry without winternl.h.
+    #
+    # See also:
+    # https://github.com/boostorg/process/blob/develop/include/boost/process/detail/windows/handle_workaround.hpp
+    target_compile_definitions(Boost::headers INTERFACE "BOOST_USE_WINDOWS_H=1")
+  endif()
 
-  include_directories(SYSTEM ${Boost_INCLUDE_DIR})
+  message(STATUS "Boost include dir: ${Boost_INCLUDE_DIR}")
 endif()
 
 # ----------------------------------------------------------------------
 # cURL
 
 macro(find_curl)
   if(NOT TARGET CURL::libcurl)
@@ -1043,34 +1116,46 @@
                       URL ${SNAPPY_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_SNAPPY_BUILD_SHA256_CHECKSUM}"
                       CMAKE_ARGS ${SNAPPY_CMAKE_ARGS}
                       BUILD_BYPRODUCTS "${SNAPPY_STATIC_LIB}")
 
   file(MAKE_DIRECTORY "${SNAPPY_PREFIX}/include")
 
-  add_library(Snappy::snappy STATIC IMPORTED)
-  set_target_properties(Snappy::snappy
+  set(Snappy_TARGET Snappy::snappy-static)
+  add_library(${Snappy_TARGET} STATIC IMPORTED)
+  set_target_properties(${Snappy_TARGET}
                         PROPERTIES IMPORTED_LOCATION "${SNAPPY_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${SNAPPY_PREFIX}/include")
   add_dependencies(toolchain snappy_ep)
-  add_dependencies(Snappy::snappy snappy_ep)
+  add_dependencies(${Snappy_TARGET} snappy_ep)
 
-  list(APPEND ARROW_BUNDLED_STATIC_LIBS Snappy::snappy)
+  list(APPEND ARROW_BUNDLED_STATIC_LIBS ${Snappy_TARGET})
 endmacro()
 
 if(ARROW_WITH_SNAPPY)
-  resolve_dependency(Snappy PC_PACKAGE_NAMES snappy)
+  resolve_dependency(Snappy
+                     HAVE_ALT
+                     TRUE
+                     PC_PACKAGE_NAMES
+                     snappy)
   if(${Snappy_SOURCE} STREQUAL "SYSTEM" AND NOT snappy_PC_FOUND)
-    get_target_property(SNAPPY_LIB Snappy::snappy IMPORTED_LOCATION)
-    string(APPEND ARROW_PC_LIBS_PRIVATE " ${SNAPPY_LIB}")
+    get_target_property(SNAPPY_TYPE ${Snappy_TARGET} TYPE)
+    if(NOT SNAPPY_TYPE STREQUAL "INTERFACE_LIBRARY")
+      get_target_property(SNAPPY_LIB ${Snappy_TARGET}
+                          IMPORTED_LOCATION_${UPPERCASE_BUILD_TYPE})
+      if(NOT SNAPPY_LIB)
+        get_target_property(SNAPPY_LIB ${Snappy_TARGET} IMPORTED_LOCATION_RELEASE)
+      endif()
+      if(NOT SNAPPY_LIB)
+        get_target_property(SNAPPY_LIB ${Snappy_TARGET} IMPORTED_LOCATION)
+      endif()
+      string(APPEND ARROW_PC_LIBS_PRIVATE " ${SNAPPY_LIB}")
+    endif()
   endif()
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(SNAPPY_INCLUDE_DIRS Snappy::snappy INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${SNAPPY_INCLUDE_DIRS})
 endif()
 
 # ----------------------------------------------------------------------
 # Brotli
 
 macro(build_brotli)
   message(STATUS "Building brotli from source")
@@ -1126,18 +1211,14 @@
        Brotli::brotlicommon
        Brotli::brotlienc
        Brotli::brotlidec)
 endmacro()
 
 if(ARROW_WITH_BROTLI)
   resolve_dependency(Brotli PC_PACKAGE_NAMES libbrotlidec libbrotlienc)
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(BROTLI_INCLUDE_DIR Brotli::brotlicommon
-                      INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${BROTLI_INCLUDE_DIR})
 endif()
 
 if(PARQUET_REQUIRE_ENCRYPTION AND NOT ARROW_PARQUET)
   set(PARQUET_REQUIRE_ENCRYPTION OFF)
 endif()
 set(ARROW_OPENSSL_REQUIRED_VERSION "1.0.2")
 if(BREW_BIN AND NOT OPENSSL_ROOT_DIR)
@@ -1181,17 +1262,15 @@
   set(ARROW_USE_OPENSSL ON)
 endif()
 
 if(ARROW_USE_OPENSSL)
   message(STATUS "Found OpenSSL Crypto Library: ${OPENSSL_CRYPTO_LIBRARY}")
   message(STATUS "Building with OpenSSL (Version: ${OPENSSL_VERSION}) support")
 
-  list(APPEND ARROW_SYSTEM_DEPENDENCIES "OpenSSL")
-
-  include_directories(SYSTEM ${OPENSSL_INCLUDE_DIR})
+  list(APPEND ARROW_SYSTEM_DEPENDENCIES OpenSSL)
 else()
   message(STATUS "Building without OpenSSL support. Minimum OpenSSL version ${ARROW_OPENSSL_REQUIRED_VERSION} required."
   )
 endif()
 
 # ----------------------------------------------------------------------
 # GLOG
@@ -1246,17 +1325,14 @@
   add_dependencies(glog::glog glog_ep)
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS glog::glog)
 endmacro()
 
 if(ARROW_USE_GLOG)
   resolve_dependency(GLOG PC_PACKAGE_NAMES libglog)
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(GLOG_INCLUDE_DIR glog::glog INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${GLOG_INCLUDE_DIR})
 endif()
 
 # ----------------------------------------------------------------------
 # gflags
 
 if(ARROW_BUILD_TESTS
    OR ARROW_BUILD_BENCHMARKS
@@ -1300,44 +1376,45 @@
                       URL_HASH "SHA256=${ARROW_GFLAGS_BUILD_SHA256_CHECKSUM}"
                       BUILD_IN_SOURCE 1
                       BUILD_BYPRODUCTS "${GFLAGS_STATIC_LIB}"
                       CMAKE_ARGS ${GFLAGS_CMAKE_ARGS})
 
   add_dependencies(toolchain gflags_ep)
 
-  add_thirdparty_lib(gflags STATIC_LIB ${GFLAGS_STATIC_LIB})
-  set(GFLAGS_LIBRARY gflags_static)
+  add_thirdparty_lib(gflags::gflags_static STATIC ${GFLAGS_STATIC_LIB})
+  add_dependencies(gflags::gflags_static gflags_ep)
+  set(GFLAGS_LIBRARY gflags::gflags_static)
   set_target_properties(${GFLAGS_LIBRARY}
                         PROPERTIES INTERFACE_COMPILE_DEFINITIONS "GFLAGS_IS_A_DLL=0"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GFLAGS_INCLUDE_DIR}")
   if(MSVC)
     set_target_properties(${GFLAGS_LIBRARY} PROPERTIES INTERFACE_LINK_LIBRARIES
                                                        "shlwapi.lib")
   endif()
   set(GFLAGS_LIBRARIES ${GFLAGS_LIBRARY})
 
   set(GFLAGS_VENDORED TRUE)
 
-  list(APPEND ARROW_BUNDLED_STATIC_LIBS gflags_static)
+  list(APPEND ARROW_BUNDLED_STATIC_LIBS gflags::gflags_static)
 endmacro()
 
 if(ARROW_NEED_GFLAGS)
   set(ARROW_GFLAGS_REQUIRED_VERSION "2.1.0")
   resolve_dependency(gflags
                      HAVE_ALT
                      TRUE
                      REQUIRED_VERSION
                      ${ARROW_GFLAGS_REQUIRED_VERSION}
                      IS_RUNTIME_DEPENDENCY
                      FALSE)
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${GFLAGS_INCLUDE_DIR})
 
   if(NOT TARGET ${GFLAGS_LIBRARIES})
-    if(TARGET gflags-shared)
+    if(TARGET gflags::gflags_shared)
+      set(GFLAGS_LIBRARIES gflags::gflags_shared)
+    elseif(TARGET gflags-shared)
       set(GFLAGS_LIBRARIES gflags-shared)
     elseif(TARGET gflags_shared)
       set(GFLAGS_LIBRARIES gflags_shared)
     endif()
   endif()
 endif()
 
@@ -1345,110 +1422,116 @@
 # Thrift
 
 macro(build_thrift)
   if(CMAKE_VERSION VERSION_LESS 3.10)
     message(FATAL_ERROR "Building thrift using ExternalProject requires at least CMake 3.10"
     )
   endif()
-  message("Building Apache Thrift from source")
+  message(STATUS "Building Apache Thrift from source")
   set(THRIFT_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/thrift_ep-install")
   set(THRIFT_INCLUDE_DIR "${THRIFT_PREFIX}/include")
   set(THRIFT_CMAKE_ARGS
       ${EP_COMMON_CMAKE_ARGS}
       "-DCMAKE_INSTALL_PREFIX=${THRIFT_PREFIX}"
       "-DCMAKE_INSTALL_RPATH=${THRIFT_PREFIX}/lib"
+      # Work around https://gitlab.kitware.com/cmake/cmake/issues/18865
+      -DBoost_NO_BOOST_CMAKE=ON
       -DBUILD_COMPILER=OFF
+      -DBUILD_EXAMPLES=OFF
       -DBUILD_SHARED_LIBS=OFF
       -DBUILD_TESTING=OFF
-      -DBUILD_EXAMPLES=OFF
       -DBUILD_TUTORIALS=OFF
-      -DWITH_QT4=OFF
+      -DCMAKE_DEBUG_POSTFIX=
+      -DWITH_AS3=OFF
+      -DWITH_CPP=ON
       -DWITH_C_GLIB=OFF
       -DWITH_JAVA=OFF
-      -DWITH_PYTHON=OFF
-      -DWITH_HASKELL=OFF
-      -DWITH_CPP=ON
-      -DWITH_STATIC_LIB=ON
+      -DWITH_JAVASCRIPT=OFF
       -DWITH_LIBEVENT=OFF
-      # Work around https://gitlab.kitware.com/cmake/cmake/issues/18865
-      -DBoost_NO_BOOST_CMAKE=ON)
+      -DWITH_NODEJS=OFF
+      -DWITH_PYTHON=OFF
+      -DWITH_QT5=OFF
+      -DWITH_ZLIB=OFF)
 
   # Thrift also uses boost. Forward important boost settings if there were ones passed.
   if(DEFINED BOOST_ROOT)
     list(APPEND THRIFT_CMAKE_ARGS "-DBOOST_ROOT=${BOOST_ROOT}")
   endif()
   if(DEFINED Boost_NAMESPACE)
     list(APPEND THRIFT_CMAKE_ARGS "-DBoost_NAMESPACE=${Boost_NAMESPACE}")
   endif()
 
-  set(THRIFT_STATIC_LIB_NAME "${CMAKE_STATIC_LIBRARY_PREFIX}thrift")
   if(MSVC)
     if(ARROW_USE_STATIC_CRT)
-      set(THRIFT_STATIC_LIB_NAME "${THRIFT_STATIC_LIB_NAME}mt")
+      set(THRIFT_LIB_SUFFIX "mt")
       list(APPEND THRIFT_CMAKE_ARGS "-DWITH_MT=ON")
     else()
-      set(THRIFT_STATIC_LIB_NAME "${THRIFT_STATIC_LIB_NAME}md")
+      set(THRIFT_LIB_SUFFIX "md")
       list(APPEND THRIFT_CMAKE_ARGS "-DWITH_MT=OFF")
     endif()
+    set(THRIFT_LIB
+        "${THRIFT_PREFIX}/bin/${CMAKE_IMPORT_LIBRARY_PREFIX}thrift${THRIFT_LIB_SUFFIX}${CMAKE_IMPORT_LIBRARY_SUFFIX}"
+    )
+  else()
+    set(THRIFT_LIB
+        "${THRIFT_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}thrift${CMAKE_STATIC_LIBRARY_SUFFIX}"
+    )
   endif()
-  if(${UPPERCASE_BUILD_TYPE} STREQUAL "DEBUG")
-    set(THRIFT_STATIC_LIB_NAME "${THRIFT_STATIC_LIB_NAME}d")
-  endif()
-  set(THRIFT_STATIC_LIB
-      "${THRIFT_PREFIX}/lib/${THRIFT_STATIC_LIB_NAME}${CMAKE_STATIC_LIBRARY_SUFFIX}")
 
   if(BOOST_VENDORED)
     set(THRIFT_DEPENDENCIES ${THRIFT_DEPENDENCIES} boost_ep)
   endif()
 
   externalproject_add(thrift_ep
                       URL ${THRIFT_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_THRIFT_BUILD_SHA256_CHECKSUM}"
-                      BUILD_BYPRODUCTS "${THRIFT_STATIC_LIB}"
+                      BUILD_BYPRODUCTS "${THRIFT_LIB}"
                       CMAKE_ARGS ${THRIFT_CMAKE_ARGS}
                       DEPENDS ${THRIFT_DEPENDENCIES} ${EP_LOG_OPTIONS})
 
   add_library(thrift::thrift STATIC IMPORTED)
   # The include directory must exist before it is referenced by a target.
   file(MAKE_DIRECTORY "${THRIFT_INCLUDE_DIR}")
   set_target_properties(thrift::thrift
-                        PROPERTIES IMPORTED_LOCATION "${THRIFT_STATIC_LIB}"
+                        PROPERTIES IMPORTED_LOCATION "${THRIFT_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${THRIFT_INCLUDE_DIR}")
+  if(ARROW_USE_BOOST)
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_target_properties(thrift::thrift PROPERTIES INTERFACE_LINK_LIBRARIES
+                                                      Boost::headers)
+    else()
+      target_link_libraries(thrift::thrift INTERFACE Boost::headers)
+    endif()
+  endif()
   add_dependencies(toolchain thrift_ep)
   add_dependencies(thrift::thrift thrift_ep)
-  set(THRIFT_VERSION ${ARROW_THRIFT_BUILD_VERSION})
+  set(Thrift_VERSION ${ARROW_THRIFT_BUILD_VERSION})
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS thrift::thrift)
 endmacro()
 
 if(ARROW_WITH_THRIFT)
-  # We already may have looked for Thrift earlier, when considering whether
-  # to build Boost, so don't look again if already found.
-  if(NOT Thrift_FOUND)
-    # Thrift c++ code generated by 0.13 requires 0.11 or greater
-    resolve_dependency(Thrift
-                       REQUIRED_VERSION
-                       0.11.0
-                       PC_PACKAGE_NAMES
-                       thrift)
-  endif()
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${THRIFT_INCLUDE_DIR})
-
-  string(REPLACE "." ";" VERSION_LIST ${THRIFT_VERSION})
-  list(GET VERSION_LIST 0 THRIFT_VERSION_MAJOR)
-  list(GET VERSION_LIST 1 THRIFT_VERSION_MINOR)
-  list(GET VERSION_LIST 2 THRIFT_VERSION_PATCH)
+  # Thrift c++ code generated by 0.13 requires 0.11 or greater
+  resolve_dependency(Thrift
+                     REQUIRED_VERSION
+                     0.11.0
+                     PC_PACKAGE_NAMES
+                     thrift)
+
+  string(REPLACE "." ";" Thrift_VERSION_LIST ${Thrift_VERSION})
+  list(GET Thrift_VERSION_LIST 0 Thrift_VERSION_MAJOR)
+  list(GET Thrift_VERSION_LIST 1 Thrift_VERSION_MINOR)
+  list(GET Thrift_VERSION_LIST 2 Thrift_VERSION_PATCH)
 endif()
 
 # ----------------------------------------------------------------------
 # Protocol Buffers (required for ORC, Flight, Gandiva and Substrait libraries)
 
 macro(build_protobuf)
-  message("Building Protocol Buffers from source")
+  message(STATUS "Building Protocol Buffers from source")
   set(PROTOBUF_VENDORED TRUE)
   set(PROTOBUF_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/protobuf_ep-install")
   set(PROTOBUF_INCLUDE_DIR "${PROTOBUF_PREFIX}/include")
   # This flag is based on what the user initially requested but if
   # we've fallen back to building protobuf we always build it statically
   # so we need to reset the flag so that we can link against it correctly
   # later.
@@ -1516,14 +1599,16 @@
                       BUILD_BYPRODUCTS "${PROTOBUF_STATIC_LIB}" "${PROTOBUF_COMPILER}"
                                        ${EP_LOG_OPTIONS}
                       BUILD_IN_SOURCE 1
                       URL ${PROTOBUF_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_PROTOBUF_BUILD_SHA256_CHECKSUM}")
 
   file(MAKE_DIRECTORY "${PROTOBUF_INCLUDE_DIR}")
+  # For compatibility of CMake's FindProtobuf.cmake.
+  set(Protobuf_INCLUDE_DIRS "${PROTOBUF_INCLUDE_DIR}")
 
   add_library(arrow::protobuf::libprotobuf STATIC IMPORTED)
   set_target_properties(arrow::protobuf::libprotobuf
                         PROPERTIES IMPORTED_LOCATION "${PROTOBUF_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${PROTOBUF_INCLUDE_DIR}")
   add_library(arrow::protobuf::libprotoc STATIC IMPORTED)
@@ -1562,17 +1647,14 @@
                      PC_PACKAGE_NAMES
                      protobuf)
 
   if(NOT Protobuf_USE_STATIC_LIBS AND MSVC_TOOLCHAIN)
     add_definitions(-DPROTOBUF_USE_DLLS)
   endif()
 
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${PROTOBUF_INCLUDE_DIR})
-
   if(TARGET arrow::protobuf::libprotobuf)
     set(ARROW_PROTOBUF_LIBPROTOBUF arrow::protobuf::libprotobuf)
   else()
     # CMake 3.8 or older don't define the targets
     if(NOT TARGET protobuf::libprotobuf)
       add_library(protobuf::libprotobuf UNKNOWN IMPORTED)
       set_target_properties(protobuf::libprotobuf
@@ -1625,60 +1707,57 @@
   message(STATUS "Found protobuf headers: ${PROTOBUF_INCLUDE_DIR}")
 endif()
 
 # ----------------------------------------------------------------------
 # Substrait (required by compute engine)
 
 macro(build_substrait)
-  message("Building Substrait from source")
+  message(STATUS "Building Substrait from source")
 
-  set(SUBSTRAIT_PROTOS
-      capabilities
-      expression
-      extensions/extensions
-      function
-      parameterized_types
-      plan
-      relations
-      type
-      type_expressions)
+  # Note: not all protos in Substrait actually matter to plan
+  # consumption. No need to build the ones we don't need.
+  set(SUBSTRAIT_PROTOS algebra extensions/extensions plan type)
 
   externalproject_add(substrait_ep
                       CONFIGURE_COMMAND ""
                       BUILD_COMMAND ""
                       INSTALL_COMMAND ""
                       URL ${SUBSTRAIT_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_SUBSTRAIT_BUILD_SHA256_CHECKSUM}")
 
   externalproject_get_property(substrait_ep SOURCE_DIR)
   set(SUBSTRAIT_LOCAL_DIR ${SOURCE_DIR})
 
   set(SUBSTRAIT_CPP_DIR "${CMAKE_CURRENT_BINARY_DIR}/substrait_ep-generated")
   file(MAKE_DIRECTORY ${SUBSTRAIT_CPP_DIR})
 
-  set(SUBSTRAIT_SUPPRESSED_WARNINGS)
+  set(SUBSTRAIT_SUPPRESSED_FLAGS)
   if(MSVC)
     # Protobuf generated files trigger some spurious warnings on MSVC.
 
     # Implicit conversion from uint64_t to uint32_t:
-    list(APPEND SUBSTRAIT_SUPPRESSED_WARNINGS "/wd4244")
+    list(APPEND SUBSTRAIT_SUPPRESSED_FLAGS "/wd4244")
 
     # Missing dll-interface:
-    list(APPEND SUBSTRAIT_SUPPRESSED_WARNINGS "/wd4251")
+    list(APPEND SUBSTRAIT_SUPPRESSED_FLAGS "/wd4251")
+  elseif(CMAKE_CXX_COMPILER_ID STREQUAL "AppleClang" OR CMAKE_CXX_COMPILER_ID STREQUAL
+                                                        "Clang")
+    # Protobuf generated files trigger some errors on CLANG TSAN builds
+    list(APPEND SUBSTRAIT_SUPPRESSED_FLAGS "-Wno-error=shorten-64-to-32")
   endif()
 
   set(SUBSTRAIT_SOURCES)
   set(SUBSTRAIT_PROTO_GEN_ALL)
   foreach(SUBSTRAIT_PROTO ${SUBSTRAIT_PROTOS})
     set(SUBSTRAIT_PROTO_GEN "${SUBSTRAIT_CPP_DIR}/substrait/${SUBSTRAIT_PROTO}.pb")
 
     foreach(EXT h cc)
       set_source_files_properties("${SUBSTRAIT_PROTO_GEN}.${EXT}"
                                   PROPERTIES COMPILE_OPTIONS
-                                             "${SUBSTRAIT_SUPPRESSED_WARNINGS}"
+                                             "${SUBSTRAIT_SUPPRESSED_FLAGS}"
                                              GENERATED TRUE
                                              SKIP_UNITY_BUILD_INCLUSION TRUE)
       list(APPEND SUBSTRAIT_PROTO_GEN_ALL "${SUBSTRAIT_PROTO_GEN}.${EXT}")
     endforeach()
     add_custom_command(OUTPUT "${SUBSTRAIT_PROTO_GEN}.cc" "${SUBSTRAIT_PROTO_GEN}.h"
                        COMMAND ${ARROW_PROTOBUF_PROTOC} "-I${SUBSTRAIT_LOCAL_DIR}/proto"
                                "--cpp_out=${SUBSTRAIT_CPP_DIR}"
@@ -1706,21 +1785,20 @@
   set(Substrait_SOURCE "BUNDLED")
   resolve_dependency(Substrait)
 endif()
 
 # ----------------------------------------------------------------------
 # jemalloc - Unix-only high-performance allocator
 
-if(ARROW_JEMALLOC)
-  message(STATUS "Building (vendored) jemalloc from source")
-  # We only use a vendored jemalloc as we want to control its version.
-  # Also our build of jemalloc is specially prefixed so that it will not
+macro(build_jemalloc)
+  # Our build of jemalloc is specially prefixed so that it will not
   # conflict with the default allocator as well as other jemalloc
   # installations.
-  # find_package(jemalloc)
+
+  message(STATUS "Building jemalloc from source")
 
   set(ARROW_JEMALLOC_USE_SHARED OFF)
   set(JEMALLOC_PREFIX
       "${CMAKE_CURRENT_BINARY_DIR}/jemalloc_ep-prefix/src/jemalloc_ep/dist/")
   set(JEMALLOC_LIB_DIR "${JEMALLOC_PREFIX}/lib")
   set(JEMALLOC_STATIC_LIB
       "${JEMALLOC_LIB_DIR}/libjemalloc_pic${CMAKE_STATIC_LIBRARY_SUFFIX}")
@@ -1764,26 +1842,34 @@
                       BUILD_IN_SOURCE 1
                       BUILD_COMMAND ${JEMALLOC_BUILD_COMMAND}
                       BUILD_BYPRODUCTS "${JEMALLOC_STATIC_LIB}"
                       INSTALL_COMMAND ${MAKE} -j1 install)
 
   # Don't use the include directory directly so that we can point to a path
   # that is unique to our codebase.
-  include_directories(SYSTEM "${CMAKE_CURRENT_BINARY_DIR}/jemalloc_ep-prefix/src/")
+  set(JEMALLOC_INCLUDE_DIR "${CMAKE_CURRENT_BINARY_DIR}/jemalloc_ep-prefix/src/")
   # The include directory must exist before it is referenced by a target.
-  file(MAKE_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}/jemalloc_ep-prefix/src/")
-  add_library(jemalloc::jemalloc STATIC IMPORTED)
-  set_target_properties(jemalloc::jemalloc
+  file(MAKE_DIRECTORY "${JEMALLOC_INCLUDE_DIR}")
+  add_library(jemalloc STATIC IMPORTED)
+  set_target_properties(jemalloc
                         PROPERTIES INTERFACE_LINK_LIBRARIES Threads::Threads
                                    IMPORTED_LOCATION "${JEMALLOC_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES
-                                   "${CMAKE_CURRENT_BINARY_DIR}/jemalloc_ep-prefix/src")
-  add_dependencies(jemalloc::jemalloc jemalloc_ep)
+                                   "${JEMALLOC_INCLUDE_DIR}")
+  add_dependencies(jemalloc jemalloc_ep)
+
+  list(APPEND ARROW_BUNDLED_STATIC_LIBS jemalloc)
+
+  set(jemalloc_VENDORED TRUE)
+  # For config.h.cmake
+  set(ARROW_JEMALLOC_VENDORED ${jemalloc_VENDORED})
+endmacro()
 
-  list(APPEND ARROW_BUNDLED_STATIC_LIBS jemalloc::jemalloc)
+if(ARROW_JEMALLOC)
+  resolve_dependency(jemalloc)
 endif()
 
 # ----------------------------------------------------------------------
 # mimalloc - Cross-platform high-performance allocator, from Microsoft
 
 if(ARROW_MIMALLOC)
   message(STATUS "Building (vendored) mimalloc from source")
@@ -1794,35 +1880,36 @@
     set(MIMALLOC_LIB_BASE_NAME "${MIMALLOC_LIB_BASE_NAME}-static")
   endif()
   if(${UPPERCASE_BUILD_TYPE} STREQUAL "DEBUG")
     set(MIMALLOC_LIB_BASE_NAME "${MIMALLOC_LIB_BASE_NAME}-${LOWERCASE_BUILD_TYPE}")
   endif()
 
   set(MIMALLOC_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/mimalloc_ep/src/mimalloc_ep")
-  set(MIMALLOC_INCLUDE_DIR "${MIMALLOC_PREFIX}/include/mimalloc-1.7")
+  set(MIMALLOC_INCLUDE_DIR "${MIMALLOC_PREFIX}/include/mimalloc-2.0")
   set(MIMALLOC_STATIC_LIB
-      "${MIMALLOC_PREFIX}/lib/mimalloc-1.7/${CMAKE_STATIC_LIBRARY_PREFIX}${MIMALLOC_LIB_BASE_NAME}${CMAKE_STATIC_LIBRARY_SUFFIX}"
+      "${MIMALLOC_PREFIX}/lib/mimalloc-2.0/${CMAKE_STATIC_LIBRARY_PREFIX}${MIMALLOC_LIB_BASE_NAME}${CMAKE_STATIC_LIBRARY_SUFFIX}"
   )
 
+  # Override CMAKE_INSTALL_LIBDIR to avoid lib64 installation on RedHat derivatives
   set(MIMALLOC_CMAKE_ARGS
       ${EP_COMMON_CMAKE_ARGS}
       "-DCMAKE_INSTALL_PREFIX=${MIMALLOC_PREFIX}"
+      "-DCMAKE_INSTALL_LIBDIR=lib"
       -DMI_OVERRIDE=OFF
       -DMI_LOCAL_DYNAMIC_TLS=ON
       -DMI_BUILD_OBJECT=OFF
       -DMI_BUILD_SHARED=OFF
       -DMI_BUILD_TESTS=OFF)
 
   externalproject_add(mimalloc_ep
                       URL ${MIMALLOC_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_MIMALLOC_BUILD_SHA256_CHECKSUM}"
                       CMAKE_ARGS ${MIMALLOC_CMAKE_ARGS}
                       BUILD_BYPRODUCTS "${MIMALLOC_STATIC_LIB}")
 
-  include_directories(SYSTEM ${MIMALLOC_INCLUDE_DIR})
   file(MAKE_DIRECTORY ${MIMALLOC_INCLUDE_DIR})
 
   add_library(mimalloc::mimalloc STATIC IMPORTED)
   set_target_properties(mimalloc::mimalloc
                         PROPERTIES INTERFACE_LINK_LIBRARIES Threads::Threads
                                    IMPORTED_LOCATION "${MIMALLOC_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES
@@ -1832,14 +1919,16 @@
                  APPEND
                  PROPERTY INTERFACE_LINK_LIBRARIES "bcrypt.lib" "psapi.lib")
   endif()
   add_dependencies(mimalloc::mimalloc mimalloc_ep)
   add_dependencies(toolchain mimalloc_ep)
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS mimalloc::mimalloc)
+
+  set(mimalloc_VENDORED TRUE)
 endif()
 
 # ----------------------------------------------------------------------
 # Google gtest
 
 macro(build_gtest)
   message(STATUS "Building gtest from source")
@@ -1896,16 +1985,14 @@
       -DCMAKE_CXX_FLAGS_${UPPERCASE_BUILD_TYPE}=${GTEST_CMAKE_CXX_FLAGS}
       -DCMAKE_INSTALL_LIBDIR=lib
       -DCMAKE_INSTALL_NAME_DIR=${GTEST_INSTALL_NAME_DIR}
       -DCMAKE_INSTALL_PREFIX=${GTEST_PREFIX}
       -DCMAKE_MACOSX_RPATH=OFF)
   set(GMOCK_INCLUDE_DIR "${GTEST_PREFIX}/include")
 
-  add_definitions(-DGTEST_LINKED_AS_SHARED_LIBRARY=1)
-
   if(MSVC AND NOT ARROW_USE_STATIC_CRT)
     set(GTEST_CMAKE_ARGS ${GTEST_CMAKE_ARGS} -Dgtest_force_shared_crt=ON)
   endif()
 
   externalproject_add(googletest_ep
                       URL ${GTEST_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_GTEST_BUILD_SHA256_CHECKSUM}"
@@ -1955,70 +2042,50 @@
 
   # The include directory must exist before it is referenced by a target.
   file(MAKE_DIRECTORY "${GTEST_INCLUDE_DIR}")
 
   add_library(GTest::gtest SHARED IMPORTED)
   set_target_properties(GTest::gtest
                         PROPERTIES ${_GTEST_IMPORTED_TYPE} "${GTEST_SHARED_LIB}"
+                                   INTERFACE_COMPILE_DEFINITIONS
+                                   "GTEST_LINKED_AS_SHARED_LIBRARY=1"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GTEST_INCLUDE_DIR}")
 
   add_library(GTest::gtest_main SHARED IMPORTED)
   set_target_properties(GTest::gtest_main
                         PROPERTIES ${_GTEST_IMPORTED_TYPE} "${GTEST_MAIN_SHARED_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GTEST_INCLUDE_DIR}")
 
   add_library(GTest::gmock SHARED IMPORTED)
   set_target_properties(GTest::gmock
                         PROPERTIES ${_GTEST_IMPORTED_TYPE} "${GMOCK_SHARED_LIB}"
+                                   INTERFACE_COMPILE_DEFINITIONS
+                                   "GMOCK_LINKED_AS_SHARED_LIBRARY=1"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GTEST_INCLUDE_DIR}")
   add_dependencies(toolchain-tests googletest_ep)
   add_dependencies(GTest::gtest googletest_ep)
   add_dependencies(GTest::gtest_main googletest_ep)
   add_dependencies(GTest::gmock googletest_ep)
 endmacro()
 
 if(ARROW_TESTING)
+  if(CMAKE_VERSION VERSION_LESS 3.23)
+    set(GTEST_USE_CONFIG TRUE)
+  else()
+    set(GTEST_USE_CONFIG FALSE)
+  endif()
+  # We can't find shred library version of GoogleTest on Windows with
+  # Conda's gtest package because it doesn't provide GTestConfig.cmake
+  # provided by GoogleTest and CMake's built-in FindGTtest.cmake
+  # doesn't support gtest_dll.dll.
   resolve_dependency(GTest
                      REQUIRED_VERSION
                      1.10.0
                      USE_CONFIG
-                     TRUE)
-
-  if(NOT GTEST_VENDORED)
-    # TODO(wesm): This logic does not work correctly with the MSVC static libraries
-    # built for the shared crt
-
-    #     set(CMAKE_REQUIRED_LIBRARIES GTest::GTest GTest::Main GTest::GMock)
-    #     CHECK_CXX_SOURCE_COMPILES("
-    # #include <gmock/gmock.h>
-    # #include <gtest/gtest.h>
-
-    # class A {
-    #   public:
-    #     int run() const { return 1; }
-    # };
-
-    # class B : public A {
-    #   public:
-    #     MOCK_CONST_METHOD0(run, int());
-    # };
-
-    # TEST(Base, Test) {
-    #   B b;
-    # }" GTEST_COMPILES_WITHOUT_MACRO)
-    #     if (NOT GTEST_COMPILES_WITHOUT_MACRO)
-    #       message(STATUS "Setting GTEST_LINKED_AS_SHARED_LIBRARY=1 on GTest::GTest")
-    #       add_compile_definitions("GTEST_LINKED_AS_SHARED_LIBRARY=1")
-    #     endif()
-    #     set(CMAKE_REQUIRED_LIBRARIES)
-  endif()
-
-  get_target_property(GTEST_INCLUDE_DIR GTest::gtest INTERFACE_INCLUDE_DIRECTORIES)
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${GTEST_INCLUDE_DIR})
+                     ${GTEST_USE_CONFIG})
 endif()
 
 macro(build_benchmark)
   message(STATUS "Building benchmark from source")
   if(CMAKE_VERSION VERSION_LESS 3.6)
     message(FATAL_ERROR "Building gbenchmark from source requires at least CMake 3.6")
   endif()
@@ -2081,18 +2148,14 @@
 if(ARROW_BUILD_BENCHMARKS)
   set(BENCHMARK_REQUIRED_VERSION 1.6.0)
   resolve_dependency(benchmark
                      REQUIRED_VERSION
                      ${BENCHMARK_REQUIRED_VERSION}
                      IS_RUNTIME_DEPENDENCY
                      FALSE)
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(BENCHMARK_INCLUDE_DIR benchmark::benchmark
-                      INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${BENCHMARK_INCLUDE_DIR})
 endif()
 
 macro(build_rapidjson)
   message(STATUS "Building RapidJSON from source")
   set(RAPIDJSON_PREFIX
       "${CMAKE_CURRENT_BINARY_DIR}/rapidjson_ep/src/rapidjson_ep-install")
   set(RAPIDJSON_CMAKE_ARGS
@@ -2106,14 +2169,16 @@
                       ${EP_LOG_OPTIONS}
                       PREFIX "${CMAKE_BINARY_DIR}"
                       URL ${RAPIDJSON_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_RAPIDJSON_BUILD_SHA256_CHECKSUM}"
                       CMAKE_ARGS ${RAPIDJSON_CMAKE_ARGS})
 
   set(RAPIDJSON_INCLUDE_DIR "${RAPIDJSON_PREFIX}/include")
+  # The include directory must exist before it is referenced by a target.
+  file(MAKE_DIRECTORY "${RAPIDJSON_INCLUDE_DIR}")
 
   add_dependencies(toolchain rapidjson_ep)
   add_dependencies(toolchain-tests rapidjson_ep)
   add_dependencies(rapidjson rapidjson_ep)
 
   set(RAPIDJSON_VENDORED TRUE)
 endmacro()
@@ -2127,17 +2192,28 @@
                      ${ARROW_RAPIDJSON_REQUIRED_VERSION}
                      IS_RUNTIME_DEPENDENCY
                      FALSE)
 
   if(RapidJSON_INCLUDE_DIR)
     set(RAPIDJSON_INCLUDE_DIR "${RapidJSON_INCLUDE_DIR}")
   endif()
+  if(WIN32 AND "${RAPIDJSON_INCLUDE_DIR}" MATCHES "^/")
+    # MSYS2
+    execute_process(COMMAND "cygpath" "--windows" "${RAPIDJSON_INCLUDE_DIR}"
+                    OUTPUT_VARIABLE RAPIDJSON_INCLUDE_DIR
+                    OUTPUT_STRIP_TRAILING_WHITESPACE)
+  endif()
 
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${RAPIDJSON_INCLUDE_DIR})
+  add_library(rapidjson::rapidjson INTERFACE IMPORTED)
+  if(CMAKE_VERSION VERSION_LESS 3.11)
+    set_target_properties(rapidjson::rapidjson PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                                          "${RAPIDJSON_INCLUDE_DIR}")
+  else()
+    target_include_directories(rapidjson::rapidjson INTERFACE "${RAPIDJSON_INCLUDE_DIR}")
+  endif()
 endif()
 
 macro(build_xsimd)
   message(STATUS "Building xsimd from source")
   set(XSIMD_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/xsimd_ep/src/xsimd_ep-install")
   set(XSIMD_CMAKE_ARGS ${EP_COMMON_CMAKE_ARGS} "-DCMAKE_INSTALL_PREFIX=${XSIMD_PREFIX}")
 
@@ -2145,27 +2221,44 @@
                       ${EP_LOG_OPTIONS}
                       PREFIX "${CMAKE_BINARY_DIR}"
                       URL ${XSIMD_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_XSIMD_BUILD_SHA256_CHECKSUM}"
                       CMAKE_ARGS ${XSIMD_CMAKE_ARGS})
 
   set(XSIMD_INCLUDE_DIR "${XSIMD_PREFIX}/include")
+  # The include directory must exist before it is referenced by a target.
+  file(MAKE_DIRECTORY "${XSIMD_INCLUDE_DIR}")
 
   add_dependencies(toolchain xsimd_ep)
   add_dependencies(toolchain-tests xsimd_ep)
 
   set(XSIMD_VENDORED TRUE)
 endmacro()
 
 if((NOT ARROW_SIMD_LEVEL STREQUAL "NONE") OR (NOT ARROW_RUNTIME_SIMD_LEVEL STREQUAL "NONE"
                                              ))
-  set(xsimd_SOURCE "BUNDLED")
-  resolve_dependency(xsimd)
-  # TODO: Don't use global includes but rather target_include_directories
-  include_directories(SYSTEM ${XSIMD_INCLUDE_DIR})
+  set(ARROW_USE_XSIMD TRUE)
+else()
+  set(ARROW_USE_XSIMD FALSE)
+endif()
+
+if(ARROW_USE_XSIMD)
+  resolve_dependency(xsimd REQUIRED_VERSION "8.1.0")
+
+  if(xsimd_SOURCE STREQUAL "BUNDLED")
+    add_library(xsimd INTERFACE IMPORTED)
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_target_properties(xsimd PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                             "${XSIMD_INCLUDE_DIR}")
+    else()
+      target_include_directories(xsimd INTERFACE "${XSIMD_INCLUDE_DIR}")
+    endif()
+  else()
+    message(STATUS "xsimd found. Headers: ${xsimd_INCLUDE_DIRS}")
+  endif()
 endif()
 
 macro(build_zlib)
   message(STATUS "Building ZLIB from source")
   set(ZLIB_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/zlib_ep/src/zlib_ep-install")
   if(MSVC)
     if(${UPPERCASE_BUILD_TYPE} STREQUAL "DEBUG")
@@ -2195,22 +2288,19 @@
                         PROPERTIES IMPORTED_LOCATION ${ZLIB_LIBRARIES}
                                    INTERFACE_INCLUDE_DIRECTORIES ${ZLIB_INCLUDE_DIRS})
 
   add_dependencies(toolchain zlib_ep)
   add_dependencies(ZLIB::ZLIB zlib_ep)
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS ZLIB::ZLIB)
+  set(ZLIB_VENDORED TRUE)
 endmacro()
 
 if(ARROW_WITH_ZLIB)
   resolve_dependency(ZLIB PC_PACKAGE_NAMES zlib)
-
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(ZLIB_INCLUDE_DIR ZLIB::ZLIB INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${ZLIB_INCLUDE_DIR})
 endif()
 
 macro(build_lz4)
   message(STATUS "Building lz4 from source")
   set(LZ4_BUILD_DIR "${CMAKE_CURRENT_BINARY_DIR}/lz4_ep-prefix/src/lz4_ep")
   set(LZ4_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/lz4_ep-prefix")
 
@@ -2228,15 +2318,15 @@
         BUILD_COMMAND msbuild.exe /m /p:Configuration=${CMAKE_BUILD_TYPE} /p:Platform=x64
         /p:PlatformToolset=v140 ${LZ4_RUNTIME_LIBRARY_LINKAGE} /t:Build
         ${LZ4_BUILD_DIR}/build/VS2010/lz4.sln)
   else()
     set(LZ4_STATIC_LIB "${LZ4_BUILD_DIR}/lib/liblz4.a")
     # Must explicitly invoke sh on MinGW
     set(LZ4_BUILD_COMMAND
-        BUILD_COMMAND sh "${CMAKE_SOURCE_DIR}/build-support/build-lz4-lib.sh"
+        BUILD_COMMAND sh "${CMAKE_CURRENT_SOURCE_DIR}/build-support/build-lz4-lib.sh"
         "AR=${CMAKE_AR}" "OS=${CMAKE_SYSTEM_NAME}")
   endif()
 
   # We need to copy the header in lib to directory outside of the build
   externalproject_add(lz4_ep
                       URL ${LZ4_SOURCE_URL} ${EP_LOG_OPTIONS}
                       URL_HASH "SHA256=${ARROW_LZ4_BUILD_SHA256_CHECKSUM}"
@@ -2245,30 +2335,30 @@
                                      ${LZ4_PATCH_COMMAND}
                       CONFIGURE_COMMAND ""
                       INSTALL_COMMAND ""
                       BINARY_DIR ${LZ4_BUILD_DIR}
                       BUILD_BYPRODUCTS ${LZ4_STATIC_LIB} ${LZ4_BUILD_COMMAND})
 
   file(MAKE_DIRECTORY "${LZ4_PREFIX}/include")
-  add_library(LZ4::lz4 STATIC IMPORTED)
-  set_target_properties(LZ4::lz4
+  add_library(lz4::lz4 STATIC IMPORTED)
+  set_target_properties(lz4::lz4
                         PROPERTIES IMPORTED_LOCATION "${LZ4_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${LZ4_PREFIX}/include")
   add_dependencies(toolchain lz4_ep)
-  add_dependencies(LZ4::lz4 lz4_ep)
+  add_dependencies(lz4::lz4 lz4_ep)
 
-  list(APPEND ARROW_BUNDLED_STATIC_LIBS LZ4::lz4)
+  list(APPEND ARROW_BUNDLED_STATIC_LIBS lz4::lz4)
 endmacro()
 
 if(ARROW_WITH_LZ4)
-  resolve_dependency(Lz4 PC_PACKAGE_NAMES liblz4)
-
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(LZ4_INCLUDE_DIR LZ4::lz4 INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${LZ4_INCLUDE_DIR})
+  resolve_dependency(lz4
+                     HAVE_ALT
+                     TRUE
+                     PC_PACKAGE_NAMES
+                     liblz4)
 endif()
 
 macro(build_zstd)
   message(STATUS "Building zstd from source")
   set(ZSTD_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/zstd_ep-install")
 
   set(ZSTD_CMAKE_ARGS
@@ -2343,19 +2433,14 @@
       endif()
     else()
       if(TARGET zstd::libzstd_static)
         set(ARROW_ZSTD_LIBZSTD zstd::libzstd_static)
       endif()
     endif()
   endif()
-
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(ZSTD_INCLUDE_DIR ${ARROW_ZSTD_LIBZSTD}
-                      INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${ZSTD_INCLUDE_DIR})
 endif()
 
 # ----------------------------------------------------------------------
 # RE2 (required for Gandiva)
 
 macro(build_re2)
   message(STATUS "Building RE2 from source")
@@ -2392,29 +2477,27 @@
 
 if(ARROW_WITH_RE2)
   # Don't specify "PC_PACKAGE_NAMES re2" here because re2.pc may
   # include -std=c++11. It's not compatible with C source and C++
   # source not uses C++ 11.
   resolve_dependency(re2 HAVE_ALT TRUE)
   if(${re2_SOURCE} STREQUAL "SYSTEM")
-    get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION_${UPPERCASE_BUILD_TYPE})
-    if(NOT RE2_LIB)
-      get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION_RELEASE)
-    endif()
-    if(NOT RE2_LIB)
-      get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION)
+    get_target_property(RE2_TYPE re2::re2 TYPE)
+    if(NOT RE2_TYPE STREQUAL "INTERFACE_LIBRARY")
+      get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION_${UPPERCASE_BUILD_TYPE})
+      if(NOT RE2_LIB)
+        get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION_RELEASE)
+      endif()
+      if(NOT RE2_LIB)
+        get_target_property(RE2_LIB re2::re2 IMPORTED_LOCATION)
+      endif()
+      string(APPEND ARROW_PC_LIBS_PRIVATE " ${RE2_LIB}")
     endif()
-
-    string(APPEND ARROW_PC_LIBS_PRIVATE " ${RE2_LIB}")
   endif()
   add_definitions(-DARROW_WITH_RE2)
-
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(RE2_INCLUDE_DIR re2::re2 INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${RE2_INCLUDE_DIR})
 endif()
 
 macro(build_bzip2)
   message(STATUS "Building BZip2 from source")
   set(BZIP2_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/bzip2_ep-install")
   set(BZIP2_STATIC_LIB
       "${BZIP2_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}bz2${CMAKE_STATIC_LIBRARY_SUFFIX}"
@@ -2469,15 +2552,14 @@
 
   if(NOT TARGET BZip2::BZip2)
     add_library(BZip2::BZip2 UNKNOWN IMPORTED)
     set_target_properties(BZip2::BZip2
                           PROPERTIES IMPORTED_LOCATION "${BZIP2_LIBRARIES}"
                                      INTERFACE_INCLUDE_DIRECTORIES "${BZIP2_INCLUDE_DIR}")
   endif()
-  include_directories(SYSTEM "${BZIP2_INCLUDE_DIR}")
 endif()
 
 macro(build_utf8proc)
   message(STATUS "Building utf8proc from source")
   set(UTF8PROC_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/utf8proc_ep-install")
   if(MSVC)
     set(UTF8PROC_STATIC_LIB "${UTF8PROC_PREFIX}/lib/utf8proc_static.lib")
@@ -2502,15 +2584,15 @@
                       URL_HASH "SHA256=${ARROW_UTF8PROC_BUILD_SHA256_CHECKSUM}"
                       BUILD_BYPRODUCTS "${UTF8PROC_STATIC_LIB}")
 
   file(MAKE_DIRECTORY "${UTF8PROC_PREFIX}/include")
   add_library(utf8proc::utf8proc STATIC IMPORTED)
   set_target_properties(utf8proc::utf8proc
                         PROPERTIES IMPORTED_LOCATION "${UTF8PROC_STATIC_LIB}"
-                                   INTERFACE_COMPILER_DEFINITIONS "UTF8PROC_STATIC"
+                                   INTERFACE_COMPILE_DEFINITIONS "UTF8PROC_STATIC"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${UTF8PROC_PREFIX}/include")
 
   add_dependencies(toolchain utf8proc_ep)
   add_dependencies(utf8proc::utf8proc utf8proc_ep)
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS utf8proc::utf8proc)
@@ -2518,30 +2600,15 @@
 
 if(ARROW_WITH_UTF8PROC)
   resolve_dependency(utf8proc
                      REQUIRED_VERSION
                      "2.2.0"
                      PC_PACKAGE_NAMES
                      libutf8proc)
-
   add_definitions(-DARROW_WITH_UTF8PROC)
-
-  # TODO: Don't use global definitions but rather
-  # target_compile_definitions or target_link_libraries
-  get_target_property(UTF8PROC_COMPILER_DEFINITIONS utf8proc::utf8proc
-                      INTERFACE_COMPILER_DEFINITIONS)
-  if(UTF8PROC_COMPILER_DEFINITIONS)
-    add_definitions(-D${UTF8PROC_COMPILER_DEFINITIONS})
-  endif()
-
-  # TODO: Don't use global includes but rather
-  # target_include_directories or target_link_libraries
-  get_target_property(UTF8PROC_INCLUDE_DIR utf8proc::utf8proc
-                      INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${UTF8PROC_INCLUDE_DIR})
 endif()
 
 macro(build_cares)
   message(STATUS "Building c-ares from source")
   set(CARES_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/cares_ep-install")
   set(CARES_INCLUDE_DIR "${CARES_PREFIX}/include")
 
@@ -2610,14 +2677,19 @@
         bad_any_cast_impl
         bad_optional_access
         bad_variant_access
         base
         city
         civil_time
         cord
+        cord_internal
+        cordz_functions
+        cordz_handle
+        cordz_info
+        cordz_sample_token
         debugging_internal
         demangle_internal
         examine_stack
         exponential_biased
         failure_signal_handler
         flags
         flags_commandlineflag
@@ -2634,14 +2706,15 @@
         graphcycles_internal
         hash
         hashtablez_sampler
         int128
         leak_check
         leak_check_disable
         log_severity
+        low_level_hash
         malloc_internal
         periodic_sampler
         random_distributions
         random_internal_distribution_test_util
         random_internal_platform
         random_internal_pool_urbg
         random_internal_randen
@@ -2654,16 +2727,16 @@
         raw_hash_set
         raw_logging_internal
         scoped_set_env
         spinlock_wait
         stacktrace
         status
         statusor
-        strerror
         str_format_internal
+        strerror
         strings
         strings_internal
         symbolize
         synchronization
         throw_delegate
         time
         time_zone
@@ -2685,14 +2758,17 @@
         cleanup
         cleanup_internal
         compare
         compressed_tuple
         config
         container_common
         container_memory
+        cordz_statistics
+        cordz_update_scope
+        cordz_update_tracker
         core_headers
         counting_allocator
         debugging
         dynamic_annotations
         endian
         errno_saver
         fast_type_id
@@ -2717,28 +2793,29 @@
         node_hash_set
         numeric
         numeric_representation
         optional
         pretty_function
         random_bit_gen_ref
         random_internal_distribution_caller
-        random_internal_fastmath
         random_internal_fast_uniform_bits
+        random_internal_fastmath
         random_internal_generate_real
         random_internal_iostream_state_saver
         random_internal_mock_helpers
         random_internal_nonsecure_base
         random_internal_pcg_engine
         random_internal_randen_engine
         random_internal_salted_seed_seq
         random_internal_traits
         random_internal_uniform_helper
         random_internal_wide_multiply
         random_random
         raw_hash_map
+        sample_recorder
         span
         str_format
         type_traits
         utility
         variant)
 
     foreach(_ABSL_LIB ${_ABSL_LIBS})
@@ -2755,60 +2832,59 @@
     foreach(_ABSL_LIB ${_ABSL_INTERFACE_LIBS})
       add_library(absl::${_ABSL_LIB} INTERFACE IMPORTED)
       set_target_properties(absl::${_ABSL_LIB} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
                                                           "${ABSL_INCLUDE_DIR}")
     endforeach()
 
     # Extracted the dependency information using the Abseil pkg-config files:
-    #   grep Requires $PREFIX/pkgconfig/absl_*.pc | \
+    #   grep Requires $PREFIX/lib/pkgconfig/absl_*.pc | \
     #   sed -e 's;.*/absl_;set_property(TARGET absl::;' \
     #       -e 's/.pc:Requires:/ PROPERTY INTERFACE_LINK_LIBRARIES /' \
-    #       -e 's/ = 20210324,//g' \
-    #       -e 's/ = 20210324//g' \
+    #       -E -e 's/ = 20[0-9]{6},?//g' \
     #       -e 's/absl_/absl::/g' \
     #       -e 's/$/)/'  | \
     #   grep -v 'INTERFACE_LINK_LIBRARIES[ ]*)'
+    set_property(TARGET absl::algorithm PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
     set_property(TARGET absl::algorithm_container
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::algorithm absl::core_headers
                           absl::meta)
-    set_property(TARGET absl::algorithm PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
     set_property(TARGET absl::any
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::bad_any_cast
                           absl::config
                           absl::core_headers
                           absl::fast_type_id
                           absl::type_traits
                           absl::utility)
     set_property(TARGET absl::atomic_hook PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                                                    absl::core_headers)
+    set_property(TARGET absl::bad_any_cast PROPERTY INTERFACE_LINK_LIBRARIES
+                                                    absl::bad_any_cast_impl absl::config)
     set_property(TARGET absl::bad_any_cast_impl
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                           absl::raw_logging_internal)
-    set_property(TARGET absl::bad_any_cast PROPERTY INTERFACE_LINK_LIBRARIES
-                                                    absl::bad_any_cast_impl absl::config)
     set_property(TARGET absl::bad_optional_access
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                           absl::raw_logging_internal)
     set_property(TARGET absl::bad_variant_access
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                           absl::raw_logging_internal)
-    set_property(TARGET absl::base_internal PROPERTY INTERFACE_LINK_LIBRARIES
-                                                     absl::config absl::type_traits)
     set_property(TARGET absl::base
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::atomic_hook
                           absl::base_internal
                           absl::config
                           absl::core_headers
                           absl::dynamic_annotations
                           absl::log_severity
                           absl::raw_logging_internal
                           absl::spinlock_wait
                           absl::type_traits)
+    set_property(TARGET absl::base_internal PROPERTY INTERFACE_LINK_LIBRARIES
+                                                     absl::config absl::type_traits)
     set_property(TARGET absl::bind_front
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal
                           absl::compressed_tuple)
     set_property(TARGET absl::bits PROPERTY INTERFACE_LINK_LIBRARIES absl::core_headers)
     set_property(TARGET absl::btree
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::container_common
@@ -2821,20 +2897,20 @@
                           absl::memory
                           absl::strings
                           absl::throw_delegate
                           absl::type_traits
                           absl::utility)
     set_property(TARGET absl::city PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                                             absl::core_headers absl::endian)
-    set_property(TARGET absl::cleanup_internal
-                 PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal absl::core_headers
-                          absl::utility)
     set_property(TARGET absl::cleanup
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::cleanup_internal absl::config
                           absl::core_headers)
+    set_property(TARGET absl::cleanup_internal
+                 PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal absl::core_headers
+                          absl::utility)
     set_property(TARGET absl::compare PROPERTY INTERFACE_LINK_LIBRARIES
                                                absl::core_headers absl::type_traits)
     set_property(TARGET absl::compressed_tuple PROPERTY INTERFACE_LINK_LIBRARIES
                                                         absl::utility)
     set_property(TARGET absl::container_common PROPERTY INTERFACE_LINK_LIBRARIES
                                                         absl::type_traits)
     set_property(TARGET absl::container_memory
@@ -2842,40 +2918,99 @@
                           absl::config
                           absl::memory
                           absl::type_traits
                           absl::utility)
     set_property(TARGET absl::cord
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::base
-                          absl::base_internal
-                          absl::compressed_tuple
                           absl::config
+                          absl::cord_internal
+                          absl::cordz_functions
+                          absl::cordz_info
+                          absl::cordz_update_scope
+                          absl::cordz_update_tracker
                           absl::core_headers
                           absl::endian
                           absl::fixed_array
                           absl::function_ref
                           absl::inlined_vector
                           absl::optional
                           absl::raw_logging_internal
                           absl::strings
-                          absl::strings_internal
+                          absl::type_traits)
+    set_property(TARGET absl::cord_internal
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::base_internal
+                          absl::compressed_tuple
+                          absl::config
+                          absl::core_headers
+                          absl::endian
+                          absl::inlined_vector
+                          absl::layout
+                          absl::raw_logging_internal
+                          absl::strings
                           absl::throw_delegate
                           absl::type_traits)
+    set_property(TARGET absl::cordz_functions
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::core_headers
+                          absl::exponential_biased
+                          absl::raw_logging_internal)
+    set_property(TARGET absl::cordz_handle
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::base
+                          absl::config
+                          absl::raw_logging_internal
+                          absl::synchronization)
+    set_property(TARGET absl::cordz_info
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::base
+                          absl::config
+                          absl::cord_internal
+                          absl::cordz_functions
+                          absl::cordz_handle
+                          absl::cordz_statistics
+                          absl::cordz_update_tracker
+                          absl::core_headers
+                          absl::inlined_vector
+                          absl::span
+                          absl::raw_logging_internal
+                          absl::stacktrace
+                          absl::synchronization)
+    set_property(TARGET absl::cordz_sample_token
+                 PROPERTY INTERFACE_LINK_LIBRARIES absl::config absl::cordz_handle
+                          absl::cordz_info)
+    set_property(TARGET absl::cordz_statistics
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::core_headers
+                          absl::cordz_update_tracker
+                          absl::synchronization)
+    set_property(TARGET absl::cordz_update_scope
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::cord_internal
+                          absl::cordz_info
+                          absl::cordz_update_tracker
+                          absl::core_headers)
+    set_property(TARGET absl::cordz_update_tracker PROPERTY INTERFACE_LINK_LIBRARIES
+                                                            absl::config)
     set_property(TARGET absl::core_headers PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
     set_property(TARGET absl::counting_allocator PROPERTY INTERFACE_LINK_LIBRARIES
                                                           absl::config)
+    set_property(TARGET absl::debugging PROPERTY INTERFACE_LINK_LIBRARIES
+                                                 absl::stacktrace absl::leak_check)
     set_property(TARGET absl::debugging_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::core_headers
                           absl::config
                           absl::dynamic_annotations
                           absl::errno_saver
                           absl::raw_logging_internal)
-    set_property(TARGET absl::debugging PROPERTY INTERFACE_LINK_LIBRARIES
-                                                 absl::stacktrace absl::leak_check)
     set_property(TARGET absl::demangle_internal PROPERTY INTERFACE_LINK_LIBRARIES
                                                          absl::base absl::core_headers)
     set_property(TARGET absl::dynamic_annotations PROPERTY INTERFACE_LINK_LIBRARIES
                                                            absl::config)
     set_property(TARGET absl::endian PROPERTY INTERFACE_LINK_LIBRARIES absl::base
                                               absl::config absl::core_headers)
     set_property(TARGET absl::errno_saver PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
@@ -2903,23 +3038,33 @@
                           absl::compressed_tuple
                           absl::algorithm
                           absl::config
                           absl::core_headers
                           absl::dynamic_annotations
                           absl::throw_delegate
                           absl::memory)
-    set_property(TARGET absl::flags_commandlineflag_internal
-                 PROPERTY INTERFACE_LINK_LIBRARIES absl::config absl::fast_type_id)
+    set_property(TARGET absl::flags
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::flags_commandlineflag
+                          absl::flags_config
+                          absl::flags_internal
+                          absl::flags_reflection
+                          absl::base
+                          absl::core_headers
+                          absl::strings)
     set_property(TARGET absl::flags_commandlineflag
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::config
                           absl::fast_type_id
                           absl::flags_commandlineflag_internal
                           absl::optional
                           absl::strings)
+    set_property(TARGET absl::flags_commandlineflag_internal
+                 PROPERTY INTERFACE_LINK_LIBRARIES absl::config absl::fast_type_id)
     set_property(TARGET absl::flags_config
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::config
                           absl::flags_path_util
                           absl::flags_program_name
                           absl::core_headers
                           absl::strings
@@ -2955,24 +3100,14 @@
                           absl::flags_program_name
                           absl::flags_reflection
                           absl::flags_usage
                           absl::strings
                           absl::synchronization)
     set_property(TARGET absl::flags_path_util PROPERTY INTERFACE_LINK_LIBRARIES
                                                        absl::config absl::strings)
-    set_property(TARGET absl::flags
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::config
-                          absl::flags_commandlineflag
-                          absl::flags_config
-                          absl::flags_internal
-                          absl::flags_reflection
-                          absl::base
-                          absl::core_headers
-                          absl::strings)
     set_property(TARGET absl::flags_private_handle_accessor
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::config
                           absl::flags_commandlineflag
                           absl::flags_commandlineflag_internal
                           absl::strings)
     set_property(TARGET absl::flags_program_name
@@ -2987,32 +3122,33 @@
                           absl::config
                           absl::flags_commandlineflag
                           absl::flags_private_handle_accessor
                           absl::flags_config
                           absl::strings
                           absl::synchronization
                           absl::flat_hash_map)
+    set_property(TARGET absl::flags_usage
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::core_headers
+                          absl::flags_usage_internal
+                          absl::strings
+                          absl::synchronization)
     set_property(TARGET absl::flags_usage_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::config
                           absl::flags_config
                           absl::flags
                           absl::flags_commandlineflag
                           absl::flags_internal
                           absl::flags_path_util
                           absl::flags_private_handle_accessor
                           absl::flags_program_name
                           absl::flags_reflection
-                          absl::strings
-                          absl::synchronization)
-    set_property(TARGET absl::flags_usage
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::config
-                          absl::core_headers
-                          absl::flags_usage_internal
+                          absl::flat_hash_map
                           absl::strings
                           absl::synchronization)
     set_property(TARGET absl::flat_hash_map
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::container_memory
                           absl::hash_function_defaults
                           absl::raw_hash_map
@@ -3022,70 +3158,72 @@
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::container_memory
                           absl::hash_function_defaults
                           absl::raw_hash_set
                           absl::algorithm_container
                           absl::core_headers
                           absl::memory)
-    set_property(TARGET absl::function_ref PROPERTY INTERFACE_LINK_LIBRARIES
-                                                    absl::base_internal absl::meta)
+    set_property(TARGET absl::function_ref
+                 PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal absl::core_headers
+                          absl::meta)
     set_property(TARGET absl::graphcycles_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::base
                           absl::base_internal
                           absl::config
                           absl::core_headers
                           absl::malloc_internal
                           absl::raw_logging_internal)
-    set_property(TARGET absl::hash_function_defaults
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::config
-                          absl::cord
-                          absl::hash
-                          absl::strings)
     set_property(TARGET absl::hash
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::city
                           absl::config
                           absl::core_headers
                           absl::endian
                           absl::fixed_array
                           absl::meta
                           absl::int128
                           absl::strings
                           absl::optional
                           absl::variant
                           absl::utility
-                          absl::wyhash)
+                          absl::low_level_hash)
+    set_property(TARGET absl::hash_function_defaults
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::cord
+                          absl::hash
+                          absl::strings)
     set_property(TARGET absl::hash_policy_traits PROPERTY INTERFACE_LINK_LIBRARIES
                                                           absl::meta)
-    set_property(TARGET absl::hashtable_debug_hooks PROPERTY INTERFACE_LINK_LIBRARIES
-                                                             absl::config)
     set_property(TARGET absl::hashtable_debug PROPERTY INTERFACE_LINK_LIBRARIES
                                                        absl::hashtable_debug_hooks)
+    set_property(TARGET absl::hashtable_debug_hooks PROPERTY INTERFACE_LINK_LIBRARIES
+                                                             absl::config)
     set_property(TARGET absl::hashtablez_sampler
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::base
                           absl::exponential_biased
                           absl::have_sse
+                          absl::sample_recorder
                           absl::synchronization)
-    set_property(TARGET absl::inlined_vector_internal
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::compressed_tuple
-                          absl::core_headers
-                          absl::memory
-                          absl::span
-                          absl::type_traits)
     set_property(TARGET absl::inlined_vector
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::algorithm
                           absl::core_headers
                           absl::inlined_vector_internal
                           absl::throw_delegate
                           absl::memory)
+    set_property(TARGET absl::inlined_vector_internal
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::compressed_tuple
+                          absl::core_headers
+                          absl::memory
+                          absl::span
+                          absl::type_traits)
     set_property(TARGET absl::int128 PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                                               absl::core_headers absl::bits)
     set_property(TARGET absl::kernel_timeout_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::core_headers
                           absl::raw_logging_internal absl::time)
     set_property(TARGET absl::layout
                  PROPERTY INTERFACE_LINK_LIBRARIES
@@ -3095,14 +3233,20 @@
                           absl::strings
                           absl::span
                           absl::utility)
     set_property(TARGET absl::leak_check PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                                                   absl::core_headers)
     set_property(TARGET absl::log_severity PROPERTY INTERFACE_LINK_LIBRARIES
                                                     absl::core_headers)
+    set_property(TARGET absl::low_level_hash
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::bits
+                          absl::config
+                          absl::endian
+                          absl::int128)
     set_property(TARGET absl::malloc_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::base
                           absl::base_internal
                           absl::config
                           absl::core_headers
                           absl::dynamic_annotations
@@ -3170,18 +3314,18 @@
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::config
                           absl::core_headers
                           absl::raw_logging_internal
                           absl::strings
                           absl::str_format
                           absl::span)
-    set_property(TARGET absl::random_internal_fastmath PROPERTY INTERFACE_LINK_LIBRARIES
-                                                                absl::bits)
     set_property(TARGET absl::random_internal_fast_uniform_bits
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
+    set_property(TARGET absl::random_internal_fastmath PROPERTY INTERFACE_LINK_LIBRARIES
+                                                                absl::bits)
     set_property(TARGET absl::random_internal_generate_real
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::bits
                           absl::random_internal_fastmath
                           absl::random_internal_traits
                           absl::type_traits)
     set_property(TARGET absl::random_internal_iostream_state_saver
@@ -3214,31 +3358,31 @@
                           absl::endian
                           absl::random_internal_randen
                           absl::random_internal_seed_material
                           absl::random_internal_traits
                           absl::random_seed_gen_exception
                           absl::raw_logging_internal
                           absl::span)
+    set_property(TARGET absl::random_internal_randen
+                 PROPERTY INTERFACE_LINK_LIBRARIES absl::random_internal_platform
+                          absl::random_internal_randen_hwaes
+                          absl::random_internal_randen_slow)
     set_property(TARGET absl::random_internal_randen_engine
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::endian
                           absl::random_internal_iostream_state_saver
                           absl::random_internal_randen
                           absl::raw_logging_internal
                           absl::type_traits)
-    set_property(TARGET absl::random_internal_randen_hwaes_impl
-                 PROPERTY INTERFACE_LINK_LIBRARIES absl::random_internal_platform
-                          absl::config)
     set_property(TARGET absl::random_internal_randen_hwaes
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::random_internal_platform
                           absl::random_internal_randen_hwaes_impl absl::config)
-    set_property(TARGET absl::random_internal_randen
+    set_property(TARGET absl::random_internal_randen_hwaes_impl
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::random_internal_platform
-                          absl::random_internal_randen_hwaes
-                          absl::random_internal_randen_slow)
+                          absl::config)
     set_property(TARGET absl::random_internal_randen_slow
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::random_internal_platform
                           absl::config)
     set_property(TARGET absl::random_internal_salted_seed_seq
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::inlined_vector
                           absl::optional
@@ -3290,26 +3434,27 @@
                           absl::container_common
                           absl::container_memory
                           absl::core_headers
                           absl::endian
                           absl::hash_policy_traits
                           absl::hashtable_debug_hooks
                           absl::have_sse
-                          absl::layout
                           absl::memory
                           absl::meta
                           absl::optional
                           absl::utility
                           absl::hashtablez_sampler)
     set_property(TARGET absl::raw_logging_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::atomic_hook
                           absl::config
                           absl::core_headers
                           absl::log_severity)
+    set_property(TARGET absl::sample_recorder PROPERTY INTERFACE_LINK_LIBRARIES
+                                                       absl::base absl::synchronization)
     set_property(TARGET absl::scoped_set_env
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                           absl::raw_logging_internal)
     set_property(TARGET absl::span
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::algorithm
                           absl::core_headers
@@ -3317,70 +3462,72 @@
                           absl::type_traits)
     set_property(TARGET absl::spinlock_wait
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal absl::core_headers
                           absl::errno_saver)
     set_property(TARGET absl::stacktrace
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::debugging_internal absl::config
                           absl::core_headers)
-    set_property(TARGET absl::statusor
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::status
-                          absl::core_headers
-                          absl::raw_logging_internal
-                          absl::type_traits
-                          absl::strings
-                          absl::utility
-                          absl::variant)
     set_property(TARGET absl::status
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::atomic_hook
                           absl::config
                           absl::core_headers
+                          absl::function_ref
                           absl::raw_logging_internal
                           absl::inlined_vector
                           absl::stacktrace
                           absl::symbolize
                           absl::strings
                           absl::cord
                           absl::str_format
                           absl::optional)
-    set_property(TARGET absl::strerror PROPERTY INTERFACE_LINK_LIBRARIES absl::config
-                                                absl::core_headers absl::errno_saver)
+    set_property(TARGET absl::statusor
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::base
+                          absl::status
+                          absl::core_headers
+                          absl::raw_logging_internal
+                          absl::type_traits
+                          absl::strings
+                          absl::utility
+                          absl::variant)
+    set_property(TARGET absl::str_format PROPERTY INTERFACE_LINK_LIBRARIES
+                                                  absl::str_format_internal)
     set_property(TARGET absl::str_format_internal
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::bits
                           absl::strings
                           absl::config
                           absl::core_headers
                           absl::numeric_representation
                           absl::type_traits
                           absl::int128
                           absl::span)
-    set_property(TARGET absl::str_format PROPERTY INTERFACE_LINK_LIBRARIES
-                                                  absl::str_format_internal)
-    set_property(TARGET absl::strings_internal
-                 PROPERTY INTERFACE_LINK_LIBRARIES
-                          absl::config
-                          absl::core_headers
-                          absl::endian
-                          absl::raw_logging_internal
-                          absl::type_traits)
+    set_property(TARGET absl::strerror PROPERTY INTERFACE_LINK_LIBRARIES absl::config
+                                                absl::core_headers absl::errno_saver)
     set_property(TARGET absl::strings
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::strings_internal
                           absl::base
                           absl::bits
                           absl::config
                           absl::core_headers
                           absl::endian
                           absl::int128
                           absl::memory
                           absl::raw_logging_internal
                           absl::throw_delegate
                           absl::type_traits)
+    set_property(TARGET absl::strings_internal
+                 PROPERTY INTERFACE_LINK_LIBRARIES
+                          absl::config
+                          absl::core_headers
+                          absl::endian
+                          absl::raw_logging_internal
+                          absl::type_traits)
     set_property(TARGET absl::symbolize
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::debugging_internal
                           absl::demangle_internal
                           absl::base
                           absl::config
                           absl::core_headers
@@ -3411,22 +3558,14 @@
                           absl::base
                           absl::civil_time
                           absl::core_headers
                           absl::int128
                           absl::raw_logging_internal
                           absl::strings
                           absl::time_zone)
-    if(APPLE)
-      # This is due to upstream absl::cctz issue
-      # https://github.com/abseil/abseil-cpp/issues/283
-      find_library(CoreFoundation CoreFoundation)
-      set_property(TARGET absl::time
-                   APPEND
-                   PROPERTY INTERFACE_LINK_LIBRARIES ${CoreFoundation})
-    endif()
     set_property(TARGET absl::type_traits PROPERTY INTERFACE_LINK_LIBRARIES absl::config)
     set_property(TARGET absl::utility
                  PROPERTY INTERFACE_LINK_LIBRARIES absl::base_internal absl::config
                           absl::type_traits)
     set_property(TARGET absl::variant
                  PROPERTY INTERFACE_LINK_LIBRARIES
                           absl::bad_variant_access
@@ -3434,14 +3573,23 @@
                           absl::config
                           absl::core_headers
                           absl::type_traits
                           absl::utility)
     set_property(TARGET absl::wyhash PROPERTY INTERFACE_LINK_LIBRARIES absl::config
                                               absl::endian absl::int128)
 
+    if(APPLE)
+      # This is due to upstream absl::cctz issue
+      # https://github.com/abseil/abseil-cpp/issues/283
+      find_library(CoreFoundation CoreFoundation)
+      set_property(TARGET absl::time
+                   APPEND
+                   PROPERTY INTERFACE_LINK_LIBRARIES ${CoreFoundation})
+    endif()
+
     externalproject_add(absl_ep
                         ${EP_LOG_OPTIONS}
                         URL ${ABSL_SOURCE_URL}
                         URL_HASH "SHA256=${ARROW_ABSL_BUILD_SHA256_CHECKSUM}"
                         CMAKE_ARGS ${ABSL_CMAKE_ARGS}
                         BUILD_BYPRODUCTS ${ABSL_BUILD_BYPRODUCTS})
 
@@ -3454,17 +3602,14 @@
 
 macro(build_grpc)
   resolve_dependency(c-ares
                      HAVE_ALT
                      TRUE
                      PC_PACKAGE_NAMES
                      libcares)
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(c-ares_INCLUDE_DIR c-ares::cares INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${c-ares_INCLUDE_DIR})
 
   # First need Abseil
   resolve_dependency_absl()
 
   message(STATUS "Building gRPC from source")
 
   set(GRPC_BUILD_DIR "${CMAKE_CURRENT_BINARY_DIR}/grpc_ep-prefix/src/grpc_ep-build")
@@ -3523,32 +3668,51 @@
   get_filename_component(GRPC_CARES_ROOT "${GRPC_CARES_INCLUDE_DIR}" DIRECTORY)
   get_target_property(GRPC_GFLAGS_INCLUDE_DIR ${GFLAGS_LIBRARIES}
                       INTERFACE_INCLUDE_DIRECTORIES)
   get_filename_component(GRPC_GFLAGS_ROOT "${GRPC_GFLAGS_INCLUDE_DIR}" DIRECTORY)
   get_target_property(GRPC_RE2_INCLUDE_DIR re2::re2 INTERFACE_INCLUDE_DIRECTORIES)
   get_filename_component(GRPC_RE2_ROOT "${GRPC_RE2_INCLUDE_DIR}" DIRECTORY)
 
+  # Put Abseil, etc. first so that local directories are searched
+  # before (what are likely) system directories
+  set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${ABSL_PREFIX}")
   set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${GRPC_PB_ROOT}")
   set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${GRPC_GFLAGS_ROOT}")
   set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${GRPC_CARES_ROOT}")
   set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${GRPC_RE2_ROOT}")
 
   # ZLIB is never vendored
   set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${ZLIB_ROOT}")
-  set(GRPC_CMAKE_PREFIX "${GRPC_CMAKE_PREFIX};${ABSL_PREFIX}")
 
   if(RAPIDJSON_VENDORED)
     add_dependencies(grpc_dependencies rapidjson_ep)
   endif()
 
   # Yuck, see https://stackoverflow.com/a/45433229/776560
   string(REPLACE ";" "|" GRPC_PREFIX_PATH_ALT_SEP "${GRPC_CMAKE_PREFIX}")
 
+  set(GRPC_C_FLAGS "${EP_C_FLAGS}")
+  set(GRPC_CXX_FLAGS "${EP_CXX_FLAGS}")
+  if(NOT MSVC)
+    # Negate warnings that gRPC cannot build under
+    # See https://github.com/grpc/grpc/issues/29417
+    set(GRPC_C_FLAGS
+        "${GRPC_C_FLAGS} -Wno-attributes -Wno-format-security -Wno-unknown-warning-option"
+    )
+    set(GRPC_CXX_FLAGS
+        "${GRPC_CXX_FLAGS} -Wno-attributes -Wno-format-security -Wno-unknown-warning-option"
+    )
+  endif()
+
   set(GRPC_CMAKE_ARGS
       "${EP_COMMON_CMAKE_ARGS}"
+      "-DCMAKE_C_FLAGS=${GRPC_C_FLAGS}"
+      "-DCMAKE_CXX_FLAGS=${GRPC_CXX_FLAGS}"
+      "-DCMAKE_C_FLAGS_${UPPERCASE_BUILD_TYPE}=${GRPC_C_FLAGS}"
+      "-DCMAKE_CXX_FLAGS_${UPPERCASE_BUILD_TYPE}=${GRPC_CXX_FLAGS}"
       -DCMAKE_PREFIX_PATH='${GRPC_PREFIX_PATH_ALT_SEP}'
       -DgRPC_ABSL_PROVIDER=package
       -DgRPC_BUILD_CSHARP_EXT=OFF
       -DgRPC_BUILD_GRPC_CSHARP_PLUGIN=OFF
       -DgRPC_BUILD_GRPC_NODE_PLUGIN=OFF
       -DgRPC_BUILD_GRPC_OBJECTIVE_C_PLUGIN=OFF
       -DgRPC_BUILD_GRPC_PHP_PLUGIN=OFF
@@ -3594,35 +3758,68 @@
 
   add_library(gRPC::upb STATIC IMPORTED)
   set_target_properties(gRPC::upb
                         PROPERTIES IMPORTED_LOCATION "${GRPC_STATIC_LIBRARY_UPB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GRPC_INCLUDE_DIR}")
 
   set(GRPC_GPR_ABSL_LIBRARIES
-      absl::bad_optional_access
-      absl::base
+      # We need a flattened list of Abseil libraries for the static linking case,
+      # because our method for creating arrow_bundled_dependencies.a doesn't walk
+      # the dependency tree of targets.
+      #
+      # This list should be updated when we change Abseil / gRPC versions. It can
+      # be generated with:
+      # pkg-config --libs --static grpc \
+      #   | tr " " "\n" \
+      #   | grep ^-labsl_ \
+      #   | sed 's/^-labsl_/absl::/'
+      absl::raw_hash_set
+      absl::hashtablez_sampler
+      absl::hash
+      absl::city
+      absl::low_level_hash
+      absl::random_distributions
+      absl::random_seed_sequences
+      absl::random_internal_pool_urbg
+      absl::random_internal_randen
+      absl::random_internal_randen_hwaes
+      absl::random_internal_randen_hwaes_impl
+      absl::random_internal_randen_slow
+      absl::random_internal_platform
+      absl::random_internal_seed_material
+      absl::random_seed_gen_exception
+      absl::statusor
+      absl::status
       absl::cord
+      absl::cordz_info
+      absl::cord_internal
+      absl::cordz_functions
+      absl::exponential_biased
+      absl::cordz_handle
+      absl::bad_optional_access
+      absl::str_format_internal
+      absl::synchronization
+      absl::graphcycles_internal
+      absl::stacktrace
+      absl::symbolize
       absl::debugging_internal
       absl::demangle_internal
-      absl::graphcycles_internal
-      absl::int128
       absl::malloc_internal
-      absl::raw_logging_internal
-      absl::spinlock_wait
-      absl::stacktrace
-      absl::status
-      absl::statusor
+      absl::time
+      absl::civil_time
       absl::strings
       absl::strings_internal
-      absl::str_format_internal
-      absl::symbolize
-      absl::synchronization
+      absl::base
+      absl::spinlock_wait
+      absl::int128
       absl::throw_delegate
-      absl::time
-      absl::time_zone)
+      absl::time_zone
+      absl::bad_variant_access
+      absl::raw_logging_internal
+      absl::log_severity)
 
   add_library(gRPC::gpr STATIC IMPORTED)
   set_target_properties(gRPC::gpr
                         PROPERTIES IMPORTED_LOCATION "${GRPC_STATIC_LIBRARY_GPR}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${GRPC_INCLUDE_DIR}"
                                    INTERFACE_LINK_LIBRARIES "${GRPC_GPR_ABSL_LIBRARIES}")
 
@@ -3712,25 +3909,22 @@
                      HAVE_ALT
                      TRUE
                      REQUIRED_VERSION
                      ${ARROW_GRPC_REQUIRED_VERSION}
                      PC_PACKAGE_NAMES
                      grpc++)
 
-  # TODO: Don't use global includes but rather target_include_directories
-  get_target_property(GRPC_INCLUDE_DIR gRPC::grpc++ INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${GRPC_INCLUDE_DIR})
-
   if(GRPC_VENDORED)
     set(GRPCPP_PP_INCLUDE TRUE)
     # Examples need to link to static Arrow if we're using static gRPC
     set(ARROW_GRPC_USE_SHARED OFF)
   else()
     # grpc++ headers may reside in ${GRPC_INCLUDE_DIR}/grpc++ or ${GRPC_INCLUDE_DIR}/grpcpp
     # depending on the gRPC version.
+    get_target_property(GRPC_INCLUDE_DIR gRPC::grpc++ INTERFACE_INCLUDE_DIRECTORIES)
     if(EXISTS "${GRPC_INCLUDE_DIR}/grpcpp/impl/codegen/config_protobuf.h")
       set(GRPCPP_PP_INCLUDE TRUE)
     elseif(EXISTS "${GRPC_INCLUDE_DIR}/grpc++/impl/codegen/config_protobuf.h")
       set(GRPCPP_PP_INCLUDE FALSE)
     else()
       message(FATAL_ERROR "Cannot find grpc++ headers in ${GRPC_INCLUDE_DIR}")
     endif()
@@ -3806,15 +4000,14 @@
                                    "${NLOHMANN_JSON_INCLUDE_DIR}")
   add_dependencies(nlohmann_json::nlohmann_json nlohmann_json_ep)
 endmacro()
 if(ARROW_WITH_NLOHMANN_JSON)
   resolve_dependency(nlohmann_json)
   get_target_property(nlohmann_json_INCLUDE_DIR nlohmann_json::nlohmann_json
                       INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${nlohmann_json_INCLUDE_DIR})
   message(STATUS "Found nlohmann_json headers: ${nlohmann_json_INCLUDE_DIR}")
 endif()
 
 macro(build_google_cloud_cpp_storage)
   message(STATUS "Building google-cloud-cpp from source")
   message(STATUS "Only building the google-cloud-cpp::storage component")
 
@@ -3829,14 +4022,17 @@
 
   # Build google-cloud-cpp, with only storage_client
 
   # Inject vendored packages via CMAKE_PREFIX_PATH
   if(ABSL_VENDORED)
     list(APPEND GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST ${ABSL_PREFIX})
   endif()
+  if(ZLIB_VENDORED)
+    list(APPEND GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST ${ZLIB_PREFIX})
+  endif()
   list(APPEND GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST ${CRC32C_PREFIX})
   list(APPEND GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST ${NLOHMANN_JSON_PREFIX})
 
   set(GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST_SEP_CHAR "|")
   # JOIN is CMake >=3.12 only
   string(REPLACE ";" ${GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST_SEP_CHAR}
                  GOOGLE_CLOUD_CPP_PREFIX_PATH "${GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST}")
@@ -3863,90 +4059,157 @@
   endif()
 
   add_custom_target(google_cloud_cpp_dependencies)
 
   if(ABSL_VENDORED)
     add_dependencies(google_cloud_cpp_dependencies absl_ep)
   endif()
+  if(ZLIB_VENDORED)
+    add_dependencies(google_cloud_cpp_dependencies zlib_ep)
+  endif()
   add_dependencies(google_cloud_cpp_dependencies crc32c_ep)
   add_dependencies(google_cloud_cpp_dependencies nlohmann_json::nlohmann_json)
 
   set(GOOGLE_CLOUD_CPP_STATIC_LIBRARY_STORAGE
       "${GOOGLE_CLOUD_CPP_INSTALL_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}google_cloud_cpp_storage${CMAKE_STATIC_LIBRARY_SUFFIX}"
   )
 
+  set(GOOGLE_CLOUD_CPP_STATIC_LIBRARY_REST_INTERNAL
+      "${GOOGLE_CLOUD_CPP_INSTALL_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}google_cloud_cpp_rest_internal${CMAKE_STATIC_LIBRARY_SUFFIX}"
+  )
+
   set(GOOGLE_CLOUD_CPP_STATIC_LIBRARY_COMMON
       "${GOOGLE_CLOUD_CPP_INSTALL_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}google_cloud_cpp_common${CMAKE_STATIC_LIBRARY_SUFFIX}"
   )
 
+  set(GOOGLE_CLOUD_CPP_PATCH_COMMAND)
+  if(CMAKE_VERSION VERSION_GREATER 3.9)
+    find_package(Patch)
+    if(Patch_FOUND)
+      # This patch is for google-cloud-cpp <= 1.42.0
+      # Upstreamed: https://github.com/googleapis/google-cloud-cpp/pull/9345
+      set(GOOGLE_CLOUD_CPP_PATCH_COMMAND
+          ${Patch_EXECUTABLE} "<SOURCE_DIR>/cmake/FindCurlWithTargets.cmake"
+          "${CMAKE_SOURCE_DIR}/build-support/google-cloud-cpp-curl-static-windows.patch")
+    endif()
+  endif()
   externalproject_add(google_cloud_cpp_ep
                       ${EP_LOG_OPTIONS}
                       LIST_SEPARATOR ${GOOGLE_CLOUD_CPP_PREFIX_PATH_LIST_SEP_CHAR}
                       INSTALL_DIR ${GOOGLE_CLOUD_CPP_INSTALL_PREFIX}
                       URL ${google_cloud_cpp_storage_SOURCE_URL}
                       URL_HASH "SHA256=${ARROW_GOOGLE_CLOUD_CPP_BUILD_SHA256_CHECKSUM}"
                       CMAKE_ARGS ${GOOGLE_CLOUD_CPP_CMAKE_ARGS}
+                      PATCH_COMMAND ${GOOGLE_CLOUD_CPP_PATCH_COMMAND}
                       BUILD_BYPRODUCTS ${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_STORAGE}
+                                       ${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_REST_INTERNAL}
                                        ${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_COMMON}
                       DEPENDS google_cloud_cpp_dependencies)
 
   # Work around https://gitlab.kitware.com/cmake/cmake/issues/15052
   file(MAKE_DIRECTORY ${GOOGLE_CLOUD_CPP_INCLUDE_DIR})
 
   add_dependencies(toolchain google_cloud_cpp_ep)
 
   add_library(google-cloud-cpp::common STATIC IMPORTED)
   set_target_properties(google-cloud-cpp::common
                         PROPERTIES IMPORTED_LOCATION
                                    "${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_COMMON}"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${GOOGLE_CLOUD_CPP_INCLUDE_DIR}")
+  # Refer to https://github.com/googleapis/google-cloud-cpp/blob/main/google/cloud/google_cloud_cpp_common.cmake
+  # (subsitute `main` for the SHA of the version we use)
+  # Version 1.39.0 is at a different place (they refactored after):
+  # https://github.com/googleapis/google-cloud-cpp/blob/29e5af8ca9b26cec62106d189b50549f4dc1c598/google/cloud/CMakeLists.txt#L146-L155
   set_property(TARGET google-cloud-cpp::common
                PROPERTY INTERFACE_LINK_LIBRARIES
-                        absl::any
-                        absl::flat_hash_map
+                        absl::base
                         absl::memory
                         absl::optional
+                        absl::span
                         absl::time
+                        absl::variant
                         Threads::Threads
                         OpenSSL::Crypto)
 
+  add_library(google-cloud-cpp::rest-internal STATIC IMPORTED)
+  set_target_properties(google-cloud-cpp::rest-internal
+                        PROPERTIES IMPORTED_LOCATION
+                                   "${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_REST_INTERNAL}"
+                                   INTERFACE_INCLUDE_DIRECTORIES
+                                   "${GOOGLE_CLOUD_CPP_INCLUDE_DIR}")
+  set_property(TARGET google-cloud-cpp::rest-internal
+               PROPERTY INTERFACE_LINK_LIBRARIES
+                        absl::span
+                        google-cloud-cpp::common
+                        CURL::libcurl
+                        nlohmann_json::nlohmann_json
+                        OpenSSL::SSL
+                        OpenSSL::Crypto)
+
   add_library(google-cloud-cpp::storage STATIC IMPORTED)
   set_target_properties(google-cloud-cpp::storage
                         PROPERTIES IMPORTED_LOCATION
                                    "${GOOGLE_CLOUD_CPP_STATIC_LIBRARY_STORAGE}"
                                    INTERFACE_INCLUDE_DIRECTORIES
                                    "${GOOGLE_CLOUD_CPP_INCLUDE_DIR}")
+  # Update this from https://github.com/googleapis/google-cloud-cpp/blob/main/google/cloud/storage/google_cloud_cpp_storage.cmake
   set_property(TARGET google-cloud-cpp::storage
                PROPERTY INTERFACE_LINK_LIBRARIES
                         google-cloud-cpp::common
+                        google-cloud-cpp::rest-internal
                         absl::memory
                         absl::strings
                         absl::str_format
                         absl::time
                         absl::variant
                         nlohmann_json::nlohmann_json
                         Crc32c::crc32c
                         CURL::libcurl
                         Threads::Threads
                         OpenSSL::SSL
-                        OpenSSL::Crypto)
+                        OpenSSL::Crypto
+                        ZLIB::ZLIB)
   add_dependencies(google-cloud-cpp::storage google_cloud_cpp_ep)
 
-  list(APPEND ARROW_BUNDLED_STATIC_LIBS google-cloud-cpp::storage
+  list(APPEND
+       ARROW_BUNDLED_STATIC_LIBS
+       google-cloud-cpp::storage
+       google-cloud-cpp::rest-internal
        google-cloud-cpp::common)
+  if(ABSL_VENDORED)
+    # Figure out what absl libraries (not header-only) are required by the
+    # google-cloud-cpp libraries above and add them to the bundled_dependencies
+    #
+    #   pkg-config --libs absl_memory absl_strings absl_str_format absl_time absl_variant absl_base absl_memory absl_optional absl_span absl_time absl_variant
+    # (and then some regexing)
+    list(APPEND
+         ARROW_BUNDLED_STATIC_LIBS
+         absl::bad_optional_access
+         absl::bad_variant_access
+         absl::base
+         absl::civil_time
+         absl::int128
+         absl::log_severity
+         absl::raw_logging_internal
+         absl::spinlock_wait
+         absl::strings
+         absl::strings_internal
+         absl::str_format_internal
+         absl::throw_delegate
+         absl::time
+         absl::time_zone
+         Crc32c::crc32c)
+  endif()
 endmacro()
 
 if(ARROW_WITH_GOOGLE_CLOUD_CPP)
   resolve_dependency(google_cloud_cpp_storage)
   get_target_property(google_cloud_cpp_storage_INCLUDE_DIR google-cloud-cpp::storage
                       INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${google_cloud_cpp_storage_INCLUDE_DIR})
-  get_target_property(absl_base_INCLUDE_DIR absl::base INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${absl_base_INCLUDE_DIR})
   message(STATUS "Found google-cloud-cpp::storage headers: ${google_cloud_cpp_storage_INCLUDE_DIR}"
   )
 endif()
 
 #
 # HDFS thirdparty setup
 
@@ -3960,41 +4223,48 @@
   set(HADOOP_HOME "${THIRDPARTY_DIR}/hadoop")
 endif()
 
 set(HDFS_H_PATH "${HADOOP_HOME}/include/hdfs.h")
 if(NOT EXISTS ${HDFS_H_PATH})
   message(FATAL_ERROR "Did not find hdfs.h at ${HDFS_H_PATH}")
 endif()
-message(STATUS "Found hdfs.h at: " ${HDFS_H_PATH})
+message(STATUS "Found hdfs.h at: ${HDFS_H_PATH}")
 
-include_directories(SYSTEM "${HADOOP_HOME}/include")
+add_library(arrow::hadoop INTERFACE IMPORTED)
+if(CMAKE_VERSION VERSION_LESS 3.11)
+  set_target_properties(arrow::hadoop PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                                 "${HADOOP_HOME}/include")
+else()
+  target_include_directories(arrow::hadoop INTERFACE "${HADOOP_HOME}/include")
+endif()
 
 # ----------------------------------------------------------------------
 # Apache ORC
 
 macro(build_orc)
-  message("Building Apache ORC from source")
+  message(STATUS "Building Apache ORC from source")
 
   set(ORC_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/orc_ep-install")
   set(ORC_HOME "${ORC_PREFIX}")
   set(ORC_INCLUDE_DIR "${ORC_PREFIX}/include")
   set(ORC_STATIC_LIB
       "${ORC_PREFIX}/lib/${CMAKE_STATIC_LIBRARY_PREFIX}orc${CMAKE_STATIC_LIBRARY_SUFFIX}")
 
   get_target_property(ORC_PROTOBUF_INCLUDE_DIR ${ARROW_PROTOBUF_LIBPROTOBUF}
                       INTERFACE_INCLUDE_DIRECTORIES)
   get_filename_component(ORC_PROTOBUF_ROOT "${ORC_PROTOBUF_INCLUDE_DIR}" DIRECTORY)
 
   get_target_property(ORC_PROTOBUF_LIBRARY ${ARROW_PROTOBUF_LIBPROTOBUF}
                       IMPORTED_LOCATION)
 
-  get_target_property(ORC_SNAPPY_INCLUDE_DIR Snappy::snappy INTERFACE_INCLUDE_DIRECTORIES)
+  get_target_property(ORC_SNAPPY_INCLUDE_DIR ${Snappy_TARGET}
+                      INTERFACE_INCLUDE_DIRECTORIES)
   get_filename_component(ORC_SNAPPY_ROOT "${ORC_SNAPPY_INCLUDE_DIR}" DIRECTORY)
 
-  get_target_property(ORC_LZ4_ROOT LZ4::lz4 INTERFACE_INCLUDE_DIRECTORIES)
+  get_target_property(ORC_LZ4_ROOT lz4::lz4 INTERFACE_INCLUDE_DIRECTORIES)
   get_filename_component(ORC_LZ4_ROOT "${ORC_LZ4_ROOT}" DIRECTORY)
 
   # Weirdly passing in PROTOBUF_LIBRARY for PROTOC_LIBRARY still results in ORC finding
   # the protoc library.
   set(ORC_CMAKE_ARGS
       ${EP_COMMON_CMAKE_ARGS}
       "-DCMAKE_INSTALL_PREFIX=${ORC_PREFIX}"
@@ -4030,16 +4300,16 @@
                       BUILD_BYPRODUCTS ${ORC_STATIC_LIB}
                       CMAKE_ARGS ${ORC_CMAKE_ARGS} ${EP_LOG_OPTIONS})
 
   add_dependencies(toolchain orc_ep)
 
   set(ORC_VENDORED 1)
   add_dependencies(orc_ep ZLIB::ZLIB)
-  add_dependencies(orc_ep LZ4::lz4)
-  add_dependencies(orc_ep Snappy::snappy)
+  add_dependencies(orc_ep lz4::lz4)
+  add_dependencies(orc_ep ${Snappy_TARGET})
   add_dependencies(orc_ep ${ARROW_PROTOBUF_LIBPROTOBUF})
 
   add_library(orc::liborc STATIC IMPORTED)
   set_target_properties(orc::liborc
                         PROPERTIES IMPORTED_LOCATION "${ORC_STATIC_LIB}"
                                    INTERFACE_INCLUDE_DIRECTORIES "${ORC_INCLUDE_DIR}")
 
@@ -4047,15 +4317,14 @@
   add_dependencies(orc::liborc orc_ep)
 
   list(APPEND ARROW_BUNDLED_STATIC_LIBS orc::liborc)
 endmacro()
 
 if(ARROW_ORC)
   resolve_dependency(ORC)
-  include_directories(SYSTEM ${ORC_INCLUDE_DIR})
   message(STATUS "Found ORC static library: ${ORC_STATIC_LIB}")
   message(STATUS "Found ORC headers: ${ORC_INCLUDE_DIR}")
 endif()
 
 # ----------------------------------------------------------------------
 # OpenTelemetry C++
 
@@ -4264,23 +4533,22 @@
   # cURL is required whether we build from source or use an existing installation
   # (OTel's cmake files do not call find_curl for you)
   find_curl()
   set(opentelemetry-cpp_SOURCE "AUTO")
   resolve_dependency(opentelemetry-cpp)
   get_target_property(OPENTELEMETRY_INCLUDE_DIR opentelemetry-cpp::api
                       INTERFACE_INCLUDE_DIRECTORIES)
-  include_directories(SYSTEM ${OPENTELEMETRY_INCLUDE_DIR})
   message(STATUS "Found OpenTelemetry headers: ${OPENTELEMETRY_INCLUDE_DIR}")
 endif()
 
 # ----------------------------------------------------------------------
 # AWS SDK for C++
 
 macro(build_awssdk)
-  message("Building AWS C++ SDK from source")
+  message(STATUS "Building AWS C++ SDK from source")
   if(CMAKE_CXX_COMPILER_ID STREQUAL "GNU" AND CMAKE_CXX_COMPILER_VERSION VERSION_LESS
                                               "4.9")
     message(FATAL_ERROR "AWS C++ SDK requires gcc >= 4.9")
   endif()
   set(AWSSDK_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/awssdk_ep-install")
   set(AWSSDK_INCLUDE_DIR "${AWSSDK_PREFIX}/include")
   set(AWSSDK_LIB_DIR "lib")
@@ -4300,14 +4568,22 @@
       -DBUILD_SHARED_LIBS=OFF
       -DCMAKE_BUILD_TYPE=${AWSSDK_BUILD_TYPE}
       -DCMAKE_INSTALL_LIBDIR=${AWSSDK_LIB_DIR}
       -DENABLE_TESTING=OFF
       -DENABLE_UNITY_BUILD=ON
       "-DCMAKE_INSTALL_PREFIX=${AWSSDK_PREFIX}"
       "-DCMAKE_PREFIX_PATH=${AWSSDK_PREFIX}")
+  if(NOT MSVC)
+    list(APPEND
+         AWSSDK_COMMON_CMAKE_ARGS
+         # Workaround for https://github.com/aws/aws-sdk-cpp/issues/1582
+         "-DCMAKE_CXX_FLAGS=${EP_CXX_FLAGS} -Wno-error=deprecated-declarations"
+         "-DCMAKE_CXX_FLAGS_${UPPERCASE_BUILD_TYPE}=${EP_CXX_FLAGS} -Wno-error=deprecated-declarations"
+    )
+  endif()
 
   # provide hint for AWS SDK to link with the already located openssl
   get_filename_component(OPENSSL_ROOT_HINT "${OPENSSL_INCLUDE_DIR}" DIRECTORY)
 
   set(AWSSDK_CMAKE_ARGS
       ${AWSSDK_COMMON_CMAKE_ARGS}
       -DOPENSSL_ROOT_DIR=${OPENSSL_ROOT_HINT}
@@ -4425,15 +4701,15 @@
     # on Linux and macOS curl seems to be required
     set_property(TARGET aws-cpp-sdk-core
                  APPEND
                  PROPERTY INTERFACE_LINK_LIBRARIES CURL::libcurl)
     set_property(TARGET CURL::libcurl
                  APPEND
                  PROPERTY INTERFACE_LINK_LIBRARIES OpenSSL::SSL)
-    if(TARGET zlib_ep)
+    if(ZLIB_VENDORED)
       set_property(TARGET aws-cpp-sdk-core
                    APPEND
                    PROPERTY INTERFACE_LINK_LIBRARIES ZLIB::ZLIB)
       add_dependencies(awssdk_ep zlib_ep)
     endif()
   elseif(WIN32)
     set_property(TARGET aws-cpp-sdk-core
@@ -4490,29 +4766,111 @@
     if(BUILD_SHARED_LIBS_WAS_SET)
       set(BUILD_SHARED_LIBS ${BUILD_SHARED_LIBS_VALUE})
     else()
       unset(BUILD_SHARED_LIBS)
     endif()
   endif()
 
-  include_directories(SYSTEM ${AWSSDK_INCLUDE_DIR})
   message(STATUS "Found AWS SDK headers: ${AWSSDK_INCLUDE_DIR}")
   message(STATUS "Found AWS SDK libraries: ${AWSSDK_LINK_LIBRARIES}")
 
   if(APPLE)
     # CoreFoundation's path is hardcoded in the CMake files provided by
     # aws-sdk-cpp to use the MacOSX SDK provided by XCode which makes
     # XCode a hard dependency. Command Line Tools is often used instead
     # of the full XCode suite, so let the linker to find it.
     set_target_properties(AWS::aws-c-common
                           PROPERTIES INTERFACE_LINK_LIBRARIES
                                      "-pthread;pthread;-framework CoreFoundation")
   endif()
 endif()
 
+# ----------------------------------------------------------------------
+# ucx - communication framework for modern, high-bandwidth and low-latency networks
+
+macro(build_ucx)
+  message(STATUS "Building UCX from source")
+
+  set(UCX_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/ucx_ep-install")
+
+  # link with static ucx libraries leads to test failures, use shared libs instead
+  set(UCX_SHARED_LIB_UCP "${UCX_PREFIX}/lib/libucp${CMAKE_SHARED_LIBRARY_SUFFIX}")
+  set(UCX_SHARED_LIB_UCT "${UCX_PREFIX}/lib/libuct${CMAKE_SHARED_LIBRARY_SUFFIX}")
+  set(UCX_SHARED_LIB_UCS "${UCX_PREFIX}/lib/libucs${CMAKE_SHARED_LIBRARY_SUFFIX}")
+  set(UCX_SHARED_LIB_UCM "${UCX_PREFIX}/lib/libucm${CMAKE_SHARED_LIBRARY_SUFFIX}")
+
+  set(UCX_CONFIGURE_COMMAND ./autogen.sh COMMAND ./configure)
+  list(APPEND
+       UCX_CONFIGURE_COMMAND
+       "CC=${CMAKE_C_COMPILER}"
+       "CXX=${CMAKE_CXX_COMPILER}"
+       "CFLAGS=${EP_C_FLAGS}"
+       "CXXFLAGS=${EP_CXX_FLAGS}"
+       "--prefix=${UCX_PREFIX}"
+       "--enable-mt"
+       "--enable-shared")
+  if(${UPPERCASE_BUILD_TYPE} STREQUAL "DEBUG")
+    list(APPEND
+         UCX_CONFIGURE_COMMAND
+         "--enable-profiling"
+         "--enable-frame-pointer"
+         "--enable-stats"
+         "--enable-fault-injection"
+         "--enable-debug-data")
+  else()
+    list(APPEND
+         UCX_CONFIGURE_COMMAND
+         "--disable-logging"
+         "--disable-debug"
+         "--disable-assertions"
+         "--disable-params-check")
+  endif()
+  set(UCX_BUILD_COMMAND ${MAKE} ${MAKE_BUILD_ARGS})
+  externalproject_add(ucx_ep
+                      ${EP_LOG_OPTIONS}
+                      URL ${ARROW_UCX_SOURCE_URL}
+                      URL_HASH "SHA256=${ARROW_UCX_BUILD_SHA256_CHECKSUM}"
+                      CONFIGURE_COMMAND ${UCX_CONFIGURE_COMMAND}
+                      BUILD_IN_SOURCE 1
+                      BUILD_COMMAND ${UCX_BUILD_COMMAND}
+                      BUILD_BYPRODUCTS "${UCX_SHARED_LIB_UCP}" "${UCX_SHARED_LIB_UCT}"
+                                       "${UCX_SHARED_LIB_UCS}" "${UCX_SHARED_LIB_UCM}"
+                      INSTALL_COMMAND ${MAKE} install)
+
+  # ucx cmake module sets UCX_INCLUDE_DIRS
+  set(UCX_INCLUDE_DIRS "${UCX_PREFIX}/include")
+  file(MAKE_DIRECTORY "${UCX_INCLUDE_DIRS}")
+
+  add_library(ucx::ucp SHARED IMPORTED)
+  set_target_properties(ucx::ucp PROPERTIES IMPORTED_LOCATION "${UCX_SHARED_LIB_UCP}")
+  add_library(ucx::uct SHARED IMPORTED)
+  set_target_properties(ucx::uct PROPERTIES IMPORTED_LOCATION "${UCX_SHARED_LIB_UCT}")
+  add_library(ucx::ucs SHARED IMPORTED)
+  set_target_properties(ucx::ucs PROPERTIES IMPORTED_LOCATION "${UCX_SHARED_LIB_UCS}")
+
+  add_dependencies(toolchain ucx_ep)
+  add_dependencies(ucx::ucp ucx_ep)
+  add_dependencies(ucx::uct ucx_ep)
+  add_dependencies(ucx::ucs ucx_ep)
+endmacro()
+
+if(ARROW_WITH_UCX)
+  resolve_dependency(ucx PC_PACKAGE_NAMES ucx)
+  add_library(ucx::ucx INTERFACE IMPORTED)
+  if(CMAKE_VERSION VERSION_LESS 3.11)
+    set_target_properties(ucx::ucx PROPERTIES INTERFACE_INCLUDE_DIRECTORIES
+                                              "${UCX_INCLUDE_DIRS}")
+    set_property(TARGET ucx::ucx PROPERTY INTERFACE_LINK_LIBRARIES ucx::ucp ucx::uct
+                                          ucx::ucs)
+  else()
+    target_include_directories(ucx::ucx INTERFACE "${UCX_INCLUDE_DIRS}")
+    target_link_libraries(ucx::ucx INTERFACE ucx::ucp ucx::uct ucx::ucs)
+  endif()
+endif()
+
 message(STATUS "All bundled static libraries: ${ARROW_BUNDLED_STATIC_LIBS}")
 
 # Write out the package configurations.
 
 configure_file("src/arrow/util/config.h.cmake" "src/arrow/util/config.h" ESCAPE_QUOTES)
 install(FILES "${ARROW_BINARY_DIR}/src/arrow/util/config.h"
         DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}/arrow/util")
```

### Comparing `pyarrow-8.0.0/cmake_modules/UseCython.cmake` & `pyarrow-9.0.0/cmake_modules/UseCython.cmake`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/cmake_modules/Usevcpkg.cmake` & `pyarrow-9.0.0/cmake_modules/Usevcpkg.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
   message(STATUS "vcpkg.json manifest found. Using VCPKG_MANIFEST_MODE: ON")
 endif()
 # vcpkg can install packages in three different places
 set(_INST_BUILD_DIR "${CMAKE_CURRENT_BINARY_DIR}/vcpkg_installed") # try here first
 set(_INST_SOURCE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/vcpkg_installed") # try here second
 set(_INST_VCPKG_ROOT "${VCPKG_ROOT}/installed")
 # Iterate over the places
-foreach(_INST_DIR IN LISTS _INST_BUILD_DIR _INST_SOURCE_DIR _INST_VCPKG_ROOT "notfound")
+foreach(_INST_DIR ${_INST_BUILD_DIR} ${_INST_SOURCE_DIR} ${_INST_VCPKG_ROOT} "notfound")
   if(_INST_DIR STREQUAL "notfound")
     message(FATAL_ERROR "vcpkg installed libraries directory not found. "
                         "Install packages with vcpkg before executing cmake.")
   elseif(NOT EXISTS "${_INST_DIR}")
     continue()
   elseif((_INST_DIR STREQUAL _INST_BUILD_DIR OR _INST_DIR STREQUAL _INST_SOURCE_DIR)
          AND NOT VCPKG_MANIFEST_MODE)
```

### Comparing `pyarrow-8.0.0/cmake_modules/san-config.cmake` & `pyarrow-9.0.0/cmake_modules/san-config.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
   set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -pie -fsanitize=thread")
 
   # Strictly speaking, TSAN doesn't require dynamic linking. But it does
   # require all code to be position independent, and the easiest way to
   # guarantee that is via dynamic linking (not all 3rd party archives are
   # compiled with -fPIC e.g. boost).
   if("${ARROW_LINK}" STREQUAL "a")
-    message("Using dynamic linking for TSAN")
+    message(STATUS "Using dynamic linking for TSAN")
     set(ARROW_LINK "d")
   elseif("${ARROW_LINK}" STREQUAL "s")
     message(SEND_ERROR "Cannot use TSAN with static linking")
   endif()
 endif()
 
 if(${ARROW_USE_COVERAGE})
```

### Comparing `pyarrow-8.0.0/pyarrow/__init__.pxd` & `pyarrow-9.0.0/pyarrow/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_compute.pxd` & `pyarrow-9.0.0/pyarrow/_compute.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 # cython: language_level = 3
 
 from pyarrow.lib cimport *
 from pyarrow.includes.common cimport *
 from pyarrow.includes.libarrow cimport *
 
+cdef class ScalarUdfContext(_Weakrefable):
+    cdef:
+        CScalarUdfContext c_context
+
+    cdef void init(self, const CScalarUdfContext& c_context)
 
 cdef class FunctionOptions(_Weakrefable):
     cdef:
         shared_ptr[CFunctionOptions] wrapped
 
     cdef const CFunctionOptions* get_options(self) except NULL
     cdef void init(self, const shared_ptr[CFunctionOptions]& sp)
```

### Comparing `pyarrow-8.0.0/pyarrow/_compute.pyx` & `pyarrow-9.0.0/pyarrow/_compute.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 from cpython.object cimport Py_LT, Py_EQ, Py_GT, Py_LE, Py_NE, Py_GE
 from cython.operator cimport dereference as deref
 
 from collections import namedtuple
 
 from pyarrow.lib import frombytes, tobytes, ordered_dict
 from pyarrow.lib cimport *
+from pyarrow.includes.common cimport *
 from pyarrow.includes.libarrow cimport *
 import pyarrow.lib as lib
 
+from libcpp cimport bool as c_bool
+
+import inspect
 import numpy as np
 
 
 cdef wrap_scalar_function(const shared_ptr[CFunction]& sp_func):
     """
     Wrap a C++ scalar Function in a ScalarFunction object.
     """
@@ -306,45 +310,56 @@
     def num_kernels(self):
         """
         The number of kernels implementing this function.
         """
         return self.base_func.num_kernels()
 
     def call(self, args, FunctionOptions options=None,
-             MemoryPool memory_pool=None):
+             MemoryPool memory_pool=None, length=None):
         """
         Call the function on the given arguments.
 
         Parameters
         ----------
         args : iterable
             The arguments to pass to the function.  Accepted types depend
             on the specific function.
         options : FunctionOptions, optional
             Options instance for executing this function.  This should have
             the right concrete options type.
         memory_pool : pyarrow.MemoryPool, optional
             If not passed, will allocate memory from the default memory pool.
+        length : int, optional
+            Batch size for execution, for nullary (no argument) functions. If
+            not passed, will be inferred from passed data.
         """
         cdef:
             const CFunctionOptions* c_options = NULL
             CMemoryPool* pool = maybe_unbox_memory_pool(memory_pool)
             CExecContext c_exec_ctx = CExecContext(pool)
-            vector[CDatum] c_args
+            CExecBatch c_batch
             CDatum result
 
-        _pack_compute_args(args, &c_args)
+        _pack_compute_args(args, &c_batch.values)
 
         if options is not None:
             c_options = options.get_options()
 
-        with nogil:
-            result = GetResultValue(
-                self.base_func.Execute(c_args, c_options, &c_exec_ctx)
-            )
+        if length is not None:
+            c_batch.length = length
+            with nogil:
+                result = GetResultValue(
+                    self.base_func.Execute(c_batch, c_options, &c_exec_ctx)
+                )
+        else:
+            with nogil:
+                result = GetResultValue(
+                    self.base_func.Execute(c_batch.values, c_options,
+                                           &c_exec_ctx)
+                )
 
         return wrap_datum(result)
 
 
 cdef class ScalarFunction(Function):
     cdef const CScalarFunction* func
 
@@ -516,15 +531,15 @@
 def list_functions():
     """
     Return all function names in the global registry.
     """
     return _global_func_registry.list_functions()
 
 
-def call_function(name, args, options=None, memory_pool=None):
+def call_function(name, args, options=None, memory_pool=None, length=None):
     """
     Call a named function.
 
     The function is looked up in the global registry
     (as returned by `function_registry()`).
 
     Parameters
@@ -533,17 +548,21 @@
         The name of the function to call.
     args : list
         The arguments to the function.
     options : optional
         options provided to the function.
     memory_pool : MemoryPool, optional
         memory pool to use for allocations during function execution.
+    length : int, optional
+        Batch size for execution, for nullary (no argument) functions. If not
+        passed, inferred from data.
     """
     func = _global_func_registry.get_function(name)
-    return func.call(args, options=options, memory_pool=memory_pool)
+    return func.call(args, options=options, memory_pool=memory_pool,
+                     length=length)
 
 
 cdef class FunctionOptions(_Weakrefable):
     __slots__ = ()  # avoid mistakingly creating attributes
 
     cdef const CFunctionOptions* get_options(self) except NULL:
         return self.wrapped.get()
@@ -874,19 +893,21 @@
         return CCalendarUnit_QUARTER
     elif unit == "year":
         return CCalendarUnit_YEAR
     _raise_invalid_function_option(unit, "Calendar unit")
 
 
 cdef class _RoundTemporalOptions(FunctionOptions):
-    def _set_options(self, multiple, unit, week_starts_monday):
+    def _set_options(self, multiple, unit, week_starts_monday,
+                     ceil_is_strictly_greater, calendar_based_origin):
         self.wrapped.reset(
             new CRoundTemporalOptions(
                 multiple, unwrap_round_temporal_unit(unit),
-                week_starts_monday)
+                week_starts_monday, ceil_is_strictly_greater,
+                calendar_based_origin)
         )
 
 
 class RoundTemporalOptions(_RoundTemporalOptions):
     """
     Options for rounding temporal values.
 
@@ -897,18 +918,49 @@
     unit : str, default "day"
         The unit in which `multiple` is expressed.
         Accepted values are "year", "quarter", "month", "week", "day",
         "hour", "minute", "second", "millisecond", "microsecond",
         "nanosecond".
     week_starts_monday : bool, default True
         If True, weeks start on Monday; if False, on Sunday.
+    ceil_is_strictly_greater : bool, default False
+        If True, ceil returns a rounded value that is strictly greater than the
+        input. For example: ceiling 1970-01-01T00:00:00 to 3 hours would
+        yield 1970-01-01T03:00:00 if set to True and 1970-01-01T00:00:00
+        if set to False.
+        This applies to the ceil_temporal function only.
+    calendar_based_origin : bool, default False
+        By default, the origin is 1970-01-01T00:00:00. By setting this to True,
+        rounding origin will be beginning of one less precise calendar unit.
+        E.g.: rounding to hours will use beginning of day as origin.
+
+        By default time is rounded to a multiple of units since
+        1970-01-01T00:00:00. By setting calendar_based_origin to true,
+        time will be rounded to number of units since the last greater
+        calendar unit.
+        For example: rounding to multiple of days since the beginning of the
+        month or to hours since the beginning of the day.
+        Exceptions: week and quarter are not used as greater units,
+        therefore days will be rounded to the beginning of the month not
+        week. Greater unit of week is a year.
+        Note that ceiling and rounding might change sorting order of an array
+        near greater unit change. For example rounding YYYY-mm-dd 23:00:00 to
+        5 hours will ceil and round to YYYY-mm-dd+1 01:00:00 and floor to
+        YYYY-mm-dd 20:00:00. On the other hand YYYY-mm-dd+1 00:00:00 will
+        ceil, round and floor to YYYY-mm-dd+1 00:00:00. This can break the
+        order of an already ordered array.
+
     """
 
-    def __init__(self, multiple=1, unit="day", week_starts_monday=True):
-        self._set_options(multiple, unit, week_starts_monday)
+    def __init__(self, multiple=1, unit="day", *, week_starts_monday=True,
+                 ceil_is_strictly_greater=False,
+                 calendar_based_origin=False):
+        self._set_options(multiple, unit, week_starts_monday,
+                          ceil_is_strictly_greater,
+                          calendar_based_origin)
 
 
 cdef class _RoundToMultipleOptions(FunctionOptions):
     def _set_options(self, multiple, round_mode):
         if not isinstance(multiple, Scalar):
             try:
                 multiple = lib.scalar(multiple)
@@ -1740,14 +1792,42 @@
         Accepted values are "at_start", "at_end".
     """
 
     def __init__(self, pivot, *, null_placement="at_end"):
         self._set_options(pivot, null_placement)
 
 
+cdef class _CumulativeSumOptions(FunctionOptions):
+    def _set_options(self, start, skip_nulls):
+        if not isinstance(start, Scalar):
+            try:
+                start = lib.scalar(start)
+            except Exception:
+                _raise_invalid_function_option(
+                    start, "`start` type for CumulativeSumOptions", TypeError)
+
+        self.wrapped.reset(new CCumulativeSumOptions((<Scalar> start).unwrap(), skip_nulls))
+
+
+class CumulativeSumOptions(_CumulativeSumOptions):
+    """
+    Options for `cumulative_sum` function.
+
+    Parameters
+    ----------
+    start : Scalar, default 0.0
+        Starting value for sum computation
+    skip_nulls : bool, default False
+        When false, the first encountered null is propagated.
+    """
+
+    def __init__(self, start=0.0, *, skip_nulls=False):
+        self._set_options(start, skip_nulls)
+
+
 cdef class _ArraySortOptions(FunctionOptions):
     def _set_options(self, order, null_placement):
         self.wrapped.reset(new CArraySortOptions(
             unwrap_sort_order(order), unwrap_null_placement(null_placement)))
 
 
 class ArraySortOptions(_ArraySortOptions):
@@ -1938,52 +2018,112 @@
     """
 
     def __init__(self, form):
         self._set_options(form)
 
 
 cdef class _RandomOptions(FunctionOptions):
-    def _set_options(self, length, initializer):
+    def _set_options(self, initializer):
         if initializer == 'system':
             self.wrapped.reset(new CRandomOptions(
-                CRandomOptions.FromSystemRandom(length)))
+                CRandomOptions.FromSystemRandom()))
             return
 
         if not isinstance(initializer, int):
             try:
                 initializer = hash(initializer)
             except TypeError:
                 raise TypeError(
                     f"initializer should be 'system', an integer, "
                     f"or a hashable object; got {initializer!r}")
 
         if initializer < 0:
             initializer += 2**64
         self.wrapped.reset(new CRandomOptions(
-            CRandomOptions.FromSeed(length, initializer)))
+            CRandomOptions.FromSeed(initializer)))
 
 
 class RandomOptions(_RandomOptions):
     """
     Options for random generation.
 
     Parameters
     ----------
-    length : int
-        Number of random values to generate.
     initializer : int or str
         How to initialize the underlying random generator.
         If an integer is given, it is used as a seed.
         If "system" is given, the random generator is initialized with
         a system-specific source of (hopefully true) randomness.
         Other values are invalid.
     """
 
-    def __init__(self, length, *, initializer='system'):
-        self._set_options(length, initializer)
+    def __init__(self, *, initializer='system'):
+        self._set_options(initializer)
+
+
+cdef class _RankOptions(FunctionOptions):
+
+    _tiebreaker_map = {
+        "min": CRankOptionsTiebreaker_Min,
+        "max": CRankOptionsTiebreaker_Max,
+        "first": CRankOptionsTiebreaker_First,
+        "dense": CRankOptionsTiebreaker_Dense,
+    }
+
+    def _set_options(self, sort_keys, null_placement, tiebreaker):
+        cdef vector[CSortKey] c_sort_keys
+        if isinstance(sort_keys, str):
+            c_sort_keys.push_back(
+                CSortKey(tobytes(""), unwrap_sort_order(sort_keys))
+            )
+        else:
+            for name, order in sort_keys:
+                c_sort_keys.push_back(
+                    CSortKey(tobytes(name), unwrap_sort_order(order))
+                )
+        try:
+            self.wrapped.reset(
+                new CRankOptions(c_sort_keys,
+                                 unwrap_null_placement(null_placement),
+                                 self._tiebreaker_map[tiebreaker])
+            )
+        except KeyError:
+            _raise_invalid_function_option(tiebreaker, "tiebreaker")
+
+
+class RankOptions(_RankOptions):
+    """
+    Options for the `rank` function.
+
+    Parameters
+    ----------
+    sort_keys : sequence of (name, order) tuples or str, default "ascending"
+        Names of field/column keys to sort the input on,
+        along with the order each field/column is sorted in.
+        Accepted values for `order` are "ascending", "descending".
+        Alternatively, one can simply pass "ascending" or "descending" as a string
+        if the input is array-like.
+    null_placement : str, default "at_end"
+        Where nulls in input should be sorted.
+        Accepted values are "at_start", "at_end".
+    tiebreaker : str, default "first"
+        Configure how ties between equal values are handled.
+        Accepted values are:
+
+        - "min": Ties get the smallest possible rank in sorted order.
+        - "max": Ties get the largest possible rank in sorted order.
+        - "first": Ranks are assigned in order of when ties appear in the
+                   input. This ensures the ranks are a stable permutation
+                   of the input.
+        - "dense": The ranks span a dense [1, M] interval where M is the
+                   number of distinct values in the input.
+    """
+
+    def __init__(self, sort_keys="ascending", *, null_placement="at_end", tiebreaker="first"):
+        self._set_options(sort_keys, null_placement, tiebreaker)
 
 
 def _group_by(args, keys, aggregations):
     cdef:
         vector[CDatum] c_args
         vector[CDatum] c_keys
         vector[CAggregate] c_aggregations
@@ -1992,17 +2132,17 @@
 
     _pack_compute_args(args, &c_args)
     _pack_compute_args(keys, &c_keys)
 
     for aggr_func_name, aggr_opts in aggregations:
         c_aggr.function = tobytes(aggr_func_name)
         if aggr_opts is not None:
-            c_aggr.options = (<FunctionOptions?> aggr_opts).get_options()
+            c_aggr.options = (<FunctionOptions?>aggr_opts).wrapped
         else:
-            c_aggr.options = NULL
+            c_aggr.options = <shared_ptr[CFunctionOptions]>nullptr
         c_aggregations.push_back(c_aggr)
 
     with nogil:
         result = GetResultValue(
             GroupBy(c_args, c_keys, c_aggregations)
         )
 
@@ -2028,23 +2168,23 @@
       ``pyarrow.compute.Expression.isin()``.
 
     Examples
     --------
 
     >>> import pyarrow.compute as pc
     >>> (pc.field("a") < pc.scalar(3)) | (pc.field("b") > 7)
-    <pyarrow.compute.Expression ((a < 3:int64) or (b > 7:int64))>
-    >>> ds.field('a') != 3
+    <pyarrow.compute.Expression ((a < 3) or (b > 7))>
+    >>> pc.field('a') != 3
     <pyarrow.compute.Expression (a != 3)>
-    >>> ds.field('a').isin([1, 2, 3])
-    <pyarrow.compute.Expression (a is in [
+    >>> pc.field('a').isin([1, 2, 3])
+    <pyarrow.compute.Expression is_in(a, {value_set=int64:[
       1,
       2,
       3
-    ])>
+    ], skip_nulls=false})>
     """
 
     def __init__(self):
         msg = 'Expression is an abstract class thus cannot be initialized.'
         raise TypeError(msg)
 
     cdef void init(self, const CExpression& sp):
@@ -2176,33 +2316,46 @@
         Returns
         -------
         is_null : Expression
         """
         options = NullOptions(nan_is_null=nan_is_null)
         return Expression._call("is_null", [self], options)
 
-    def cast(self, type, bint safe=True):
+    def cast(self, type=None, safe=None, options=None):
         """
         Explicitly set or change the expression's data type.
 
         This creates a new expression equivalent to calling the
         `cast` compute function on this expression.
 
         Parameters
         ----------
-        type : DataType
+        type : DataType, default None
             Type to cast array to.
         safe : boolean, default True
             Whether to check for conversion errors such as overflow.
+        options : CastOptions, default None
+            Additional checks pass by CastOptions
 
         Returns
         -------
         cast : Expression
         """
-        options = CastOptions.safe(ensure_type(type))
+        safe_vars_passed = (safe is not None) or (type is not None)
+
+        if safe_vars_passed and (options is not None):
+            raise ValueError("Must either pass values for 'type' and 'safe' or pass a "
+                             "value for 'options'")
+
+        if options is None:
+            type = ensure_type(type, allow_none=False)
+            if safe is False:
+                options = CastOptions.unsafe(type)
+            else:
+                options = CastOptions.safe(type)
         return Expression._call("cast", [self], options)
 
     def isin(self, values):
         """
         Check whether the expression is contained in values.
 
         This creates a new expression equivalent to calling the
@@ -2271,7 +2424,215 @@
     assert schema is not None
 
     if filter is None:
         return _true
 
     return GetResultValue(filter.unwrap().Bind(
         deref(pyarrow_unwrap_schema(schema).get())))
+
+
+cdef class ScalarUdfContext:
+    """
+    Per-invocation function context/state.
+
+    This object will always be the first argument to a user-defined
+    function. It should not be used outside of a call to the function.
+    """
+
+    def __init__(self):
+        raise TypeError("Do not call {}'s constructor directly"
+                        .format(self.__class__.__name__))
+
+    cdef void init(self, const CScalarUdfContext &c_context):
+        self.c_context = c_context
+
+    @property
+    def batch_length(self):
+        """
+        The common length of all input arguments (int).
+
+        In the case that all arguments are scalars, this value
+        is used to pass the "actual length" of the arguments,
+        e.g. because the scalar values are encoding a column
+        with a constant value.
+        """
+        return self.c_context.batch_length
+
+    @property
+    def memory_pool(self):
+        """
+        A memory pool for allocations (:class:`MemoryPool`).
+
+        This is the memory pool supplied by the user when they invoked
+        the function and it should be used in any calls to arrow that the
+        UDF makes if that call accepts a memory_pool.
+        """
+        return box_memory_pool(self.c_context.pool)
+
+
+cdef inline CFunctionDoc _make_function_doc(dict func_doc) except *:
+    """
+    Helper function to generate the FunctionDoc
+    This function accepts a dictionary and expects the
+    summary(str), description(str) and arg_names(List[str]) keys.
+    """
+    cdef:
+        CFunctionDoc f_doc
+        vector[c_string] c_arg_names
+
+    f_doc.summary = tobytes(func_doc["summary"])
+    f_doc.description = tobytes(func_doc["description"])
+    for arg_name in func_doc["arg_names"]:
+        c_arg_names.push_back(tobytes(arg_name))
+    f_doc.arg_names = c_arg_names
+    # UDFOptions integration:
+    # TODO: https://issues.apache.org/jira/browse/ARROW-16041
+    f_doc.options_class = b""
+    f_doc.options_required = False
+    return f_doc
+
+
+cdef object box_scalar_udf_context(const CScalarUdfContext& c_context):
+    cdef ScalarUdfContext context = ScalarUdfContext.__new__(ScalarUdfContext)
+    context.init(c_context)
+    return context
+
+
+cdef _scalar_udf_callback(user_function, const CScalarUdfContext& c_context, inputs):
+    """
+    Helper callback function used to wrap the ScalarUdfContext from Python to C++
+    execution.
+    """
+    context = box_scalar_udf_context(c_context)
+    return user_function(context, *inputs)
+
+
+def _get_scalar_udf_context(memory_pool, batch_length):
+    cdef CScalarUdfContext c_context
+    c_context.pool = maybe_unbox_memory_pool(memory_pool)
+    c_context.batch_length = batch_length
+    context = box_scalar_udf_context(c_context)
+    return context
+
+
+def register_scalar_function(func, function_name, function_doc, in_types,
+                             out_type):
+    """
+    Register a user-defined scalar function.
+
+    A scalar function is a function that executes elementwise
+    operations on arrays or scalars, i.e. a scalar function must
+    be computed row-by-row with no state where each output row
+    is computed only from its corresponding input row.
+    In other words, all argument arrays have the same length,
+    and the output array is of the same length as the arguments.
+    Scalar functions are the only functions allowed in query engine
+    expressions.
+
+    Parameters
+    ----------
+    func : callable
+        A callable implementing the user-defined function.
+        The first argument is the context argument of type
+        ScalarUdfContext.
+        Then, it must take arguments equal to the number of
+        in_types defined. It must return an Array or Scalar
+        matching the out_type. It must return a Scalar if
+        all arguments are scalar, else it must return an Array.
+
+        To define a varargs function, pass a callable that takes
+        varargs. The last in_type will be the type of all varargs
+        arguments.
+    function_name : str
+        Name of the function. This name must be globally unique.
+    function_doc : dict
+        A dictionary object with keys "summary" (str),
+        and "description" (str).
+    in_types : Dict[str, DataType]
+        A dictionary mapping function argument names to
+        their respective DataType.
+        The argument names will be used to generate
+        documentation for the function. The number of
+        arguments specified here determines the function
+        arity.
+    out_type : DataType
+        Output type of the function.
+
+    Examples
+    --------
+    >>> import pyarrow as pa
+    >>> import pyarrow.compute as pc
+    >>>
+    >>> func_doc = {}
+    >>> func_doc["summary"] = "simple udf"
+    >>> func_doc["description"] = "add a constant to a scalar"
+    >>>
+    >>> def add_constant(ctx, array):
+    ...     return pc.add(array, 1, memory_pool=ctx.memory_pool)
+    >>>
+    >>> func_name = "py_add_func"
+    >>> in_types = {"array": pa.int64()}
+    >>> out_type = pa.int64()
+    >>> pc.register_scalar_function(add_constant, func_name, func_doc,
+    ...                   in_types, out_type)
+    >>>
+    >>> func = pc.get_function(func_name)
+    >>> func.name
+    'py_add_func'
+    >>> answer = pc.call_function(func_name, [pa.array([20])])
+    >>> answer
+    <pyarrow.lib.Int64Array object at ...>
+    [
+      21
+    ]
+    """
+    cdef:
+        c_string c_func_name
+        CArity c_arity
+        CFunctionDoc c_func_doc
+        vector[shared_ptr[CDataType]] c_in_types
+        PyObject* c_function
+        shared_ptr[CDataType] c_out_type
+        CScalarUdfOptions c_options
+
+    if callable(func):
+        c_function = <PyObject*>func
+    else:
+        raise TypeError("func must be a callable")
+
+    c_func_name = tobytes(function_name)
+
+    func_spec = inspect.getfullargspec(func)
+    num_args = -1
+    if isinstance(in_types, dict):
+        for in_type in in_types.values():
+            c_in_types.push_back(
+                pyarrow_unwrap_data_type(ensure_type(in_type)))
+        function_doc["arg_names"] = in_types.keys()
+        num_args = len(in_types)
+    else:
+        raise TypeError(
+            "in_types must be a dictionary of DataType")
+
+    c_arity = CArity(num_args, func_spec.varargs)
+
+    if "summary" not in function_doc:
+        raise ValueError("Function doc must contain a summary")
+
+    if "description" not in function_doc:
+        raise ValueError("Function doc must contain a description")
+
+    if "arg_names" not in function_doc:
+        raise ValueError("Function doc must contain arg_names")
+
+    c_func_doc = _make_function_doc(function_doc)
+
+    c_out_type = pyarrow_unwrap_data_type(ensure_type(out_type))
+
+    c_options.func_name = c_func_name
+    c_options.arity = c_arity
+    c_options.func_doc = c_func_doc
+    c_options.input_types = c_in_types
+    c_options.output_type = c_out_type
+
+    check_status(RegisterScalarFunction(c_function,
+                                        <function[CallbackUdf]> &_scalar_udf_callback, c_options))
```

### Comparing `pyarrow-8.0.0/pyarrow/_compute_docstrings.py` & `pyarrow-9.0.0/pyarrow/_compute_docstrings.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 function_doc_additions["filter"] = """
     Examples
     --------
     >>> import pyarrow as pa
     >>> arr = pa.array(["a", "b", "c", None, "e"])
     >>> mask = pa.array([True, False, None, False, True])
     >>> arr.filter(mask)
-    <pyarrow.lib.StringArray object at 0x7fa826df9200>
+    <pyarrow.lib.StringArray object at ...>
     [
       "a",
       "e"
     ]
     >>> arr.filter(mask, null_selection_behavior='emit_null')
-    <pyarrow.lib.StringArray object at 0x7fa826df9200>
+    <pyarrow.lib.StringArray object at ...>
     [
       "a",
       null,
       "e"
     ]
     """
 
@@ -46,11 +46,11 @@
     Examples
     --------
     >>> import pyarrow as pa
     >>> import pyarrow.compute as pc
     >>> arr = pa.array([1, 1, 2, 2, 3, 2, 2, 2])
     >>> modes = pc.mode(arr, 2)
     >>> modes[0]
-    <pyarrow.StructScalar: {'mode': 2, 'count': 5}>
+    <pyarrow.StructScalar: [('mode', 2), ('count', 5)]>
     >>> modes[1]
-    <pyarrow.StructScalar: {'mode': 1, 'count': 2}>
+    <pyarrow.StructScalar: [('mode', 1), ('count', 2)]>
     """
```

### Comparing `pyarrow-8.0.0/pyarrow/_csv.pxd` & `pyarrow-9.0.0/pyarrow/_csv.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_csv.pyx` & `pyarrow-9.0.0/pyarrow/_csv.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_cuda.pxd` & `pyarrow-9.0.0/pyarrow/_cuda.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_cuda.pyx` & `pyarrow-9.0.0/pyarrow/_cuda.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_dataset.pxd` & `pyarrow-9.0.0/pyarrow/_dataset.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -156,7 +156,9 @@
 
     # The full path to the created file
     cdef public str path
     # Optional Parquet metadata
     # This metadata will have the file path attribute set to the path of
     # the written file.
     cdef public object metadata
+    # The size of the file in bytes
+    cdef public int size
```

### Comparing `pyarrow-8.0.0/pyarrow/_dataset.pyx` & `pyarrow-9.0.0/pyarrow/_dataset.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -247,30 +247,57 @@
 
         Returns
         -------
         scanner : Scanner
 
         Examples
         --------
+        >>> import pyarrow as pa
+        >>> table = pa.table({'year': [2020, 2022, 2021, 2022, 2019, 2021],
+        ...                   'n_legs': [2, 2, 4, 4, 5, 100],
+        ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
+        ...                              "Brittle stars", "Centipede"]})
+        >>> 
+        >>> import pyarrow.parquet as pq
+        >>> pq.write_table(table, "dataset_scanner.parquet")
+
         >>> import pyarrow.dataset as ds
-        >>> dataset = ds.dataset("path/to/dataset")
+        >>> dataset = ds.dataset("dataset_scanner.parquet")
 
         Selecting a subset of the columns:
 
-        >>> dataset.scanner(columns=["A", "B"]).to_table()
+        >>> dataset.scanner(columns=["year", "n_legs"]).to_table()
+        pyarrow.Table
+        year: int64
+        n_legs: int64
+        ----
+        year: [[2020,2022,2021,2022,2019,2021]]
+        n_legs: [[2,2,4,4,5,100]]
 
         Projecting selected columns using an expression:
 
         >>> dataset.scanner(columns={
-        ...     "A_int": ds.field("A").cast("int64"),
+        ...     "n_legs_uint": ds.field("n_legs").cast("uint8"),
         ... }).to_table()
+        pyarrow.Table
+        n_legs_uint: uint8
+        ----
+        n_legs_uint: [[2,2,4,4,5,100]]
 
         Filtering rows while scanning:
 
-        >>> dataset.scanner(filter=ds.field("A") > 0).to_table()
+        >>> dataset.scanner(filter=ds.field("year") > 2020).to_table()
+        pyarrow.Table
+        year: int64
+        n_legs: int64
+        animal: string
+        ----
+        year: [[2022,2021,2022,2021]]
+        n_legs: [[2,4,4,100]]
+        animal: [["Parrot","Dog","Horse","Centipede"]]
         """
         return Scanner.from_dataset(self, **kwargs)
 
     def to_batches(self, **kwargs):
         """
         Read the dataset as materialized record batches.
 
@@ -735,15 +762,16 @@
         cdef FileFormat self = class_.__new__(class_)
         self.init(sp)
         return self
 
     cdef WrittenFile _finish_write(self, path, base_dir,
                                    CFileWriter* file_writer):
         parquet_metadata = None
-        return WrittenFile(path, parquet_metadata)
+        size = GetResultValue(file_writer.GetBytesWritten())
+        return WrittenFile(path, parquet_metadata, size)
 
     cdef inline shared_ptr[CFileFormat] unwrap(self):
         return self.wrapped
 
     def inspect(self, file, filesystem=None):
         """
         Infer the schema of a file.
@@ -1437,16 +1465,16 @@
     DirectoryPartitioning
 
     Examples
     --------
     >>> from pyarrow.dataset import DirectoryPartitioning
     >>> partitioning = DirectoryPartitioning(
     ...     pa.schema([("year", pa.int16()), ("month", pa.int8())]))
-    >>> print(partitioning.parse("/2009/11"))
-    ((year == 2009:int16) and (month == 11:int8))
+    >>> print(partitioning.parse("/2009/11/"))
+    ((year == 2009) and (month == 11))
     """
 
     cdef:
         CDirectoryPartitioning* directory_partitioning
 
     def __init__(self, Schema schema not None, dictionaries=None,
                  segment_encoding="uri"):
@@ -1564,16 +1592,16 @@
     HivePartitioning
 
     Examples
     --------
     >>> from pyarrow.dataset import HivePartitioning
     >>> partitioning = HivePartitioning(
     ...     pa.schema([("year", pa.int16()), ("month", pa.int8())]))
-    >>> print(partitioning.parse("/year=2009/month=11"))
-    ((year == 2009:int16) and (month == 11:int8))
+    >>> print(partitioning.parse("/year=2009/month=11/"))
+    ((year == 2009) and (month == 11))
 
     """
 
     cdef:
         CHivePartitioning* hive_partitioning
 
     def __init__(self,
@@ -1688,16 +1716,16 @@
     FilenamePartitioning
 
     Examples
     --------
     >>> from pyarrow.dataset import FilenamePartitioning
     >>> partitioning = FilenamePartitioning(
     ...     pa.schema([("year", pa.int16()), ("month", pa.int8())]))
-    >>> print(partitioning.parse("2009_11_"))
-    ((year == 2009:int16) and (month == 11:int8))
+    >>> print(partitioning.parse("2009_11_data.parquet"))
+    ((year == 2009) and (month == 11))
     """
 
     cdef:
         CFilenamePartitioning* filename_partitioning
 
     def __init__(self, Schema schema not None, dictionaries=None,
                  segment_encoding="uri"):
@@ -2646,19 +2674,29 @@
     return out
 
 
 cdef class WrittenFile(_Weakrefable):
     """
     Metadata information about files written as
     part of a dataset write operation
+
+    Parameters
+    ----------
+    path : str
+        Path to the file.
+    metadata : pyarrow.parquet.FileMetaData, optional
+        For Parquet files, the Parquet file metadata.
+    size : int
+        The size of the file in bytes.
     """
 
-    def __init__(self, path, metadata):
+    def __init__(self, path, metadata, size):
         self.path = path
         self.metadata = metadata
+        self.size = size
 
 
 cdef void _filesystemdataset_write_visitor(
         dict visit_args,
         CFileWriter* file_writer):
     cdef:
         str path
```

### Comparing `pyarrow-8.0.0/pyarrow/_dataset_orc.pyx` & `pyarrow-9.0.0/pyarrow/_dataset_orc.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_dataset_parquet.pyx` & `pyarrow-9.0.0/pyarrow/_dataset_parquet.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -156,15 +156,17 @@
             metadata = deref(
                 deref(parquet_file_writer).parquet_writer()).metadata()
         if metadata:
             parquet_metadata = FileMetaData()
             parquet_metadata.init(metadata)
             parquet_metadata.set_file_path(os.path.relpath(path, base_dir))
 
-        return WrittenFile(path, parquet_metadata)
+        size = GetResultValue(file_writer.GetBytesWritten())
+
+        return WrittenFile(path, parquet_metadata, size)
 
     @property
     def read_options(self):
         cdef CParquetFileFormatReaderOptions* options
         options = &self.parquet_format.reader_options
         parquet_read_options = ParquetReadOptions(
             dictionary_columns={frombytes(col)
@@ -594,30 +596,44 @@
         Disabled by default.
     buffer_size : int, default 8192
         Size of buffered stream, if enabled. Default is 8KB.
     pre_buffer : bool, default False
         If enabled, pre-buffer the raw Parquet data instead of issuing one
         read per column chunk. This can improve performance on high-latency
         filesystems.
+    thrift_string_size_limit : int, default None
+        If not None, override the maximum total string size allocated
+        when decoding Thrift structures. The default limit should be
+        sufficient for most Parquet files.
+    thrift_container_size_limit : int, default None
+        If not None, override the maximum total size of containers allocated
+        when decoding Thrift structures. The default limit should be
+        sufficient for most Parquet files.
     """
 
     cdef:
         CParquetFragmentScanOptions* parquet_options
 
     # Avoid mistakingly creating attributes
     __slots__ = ()
 
-    def __init__(self, bint use_buffered_stream=False,
+    def __init__(self, *, bint use_buffered_stream=False,
                  buffer_size=8192,
-                 bint pre_buffer=False):
+                 bint pre_buffer=False,
+                 thrift_string_size_limit=None,
+                 thrift_container_size_limit=None):
         self.init(shared_ptr[CFragmentScanOptions](
             new CParquetFragmentScanOptions()))
         self.use_buffered_stream = use_buffered_stream
         self.buffer_size = buffer_size
         self.pre_buffer = pre_buffer
+        if thrift_string_size_limit is not None:
+            self.thrift_string_size_limit = thrift_string_size_limit
+        if thrift_container_size_limit is not None:
+            self.thrift_container_size_limit = thrift_container_size_limit
 
     cdef void init(self, const shared_ptr[CFragmentScanOptions]& sp):
         FragmentScanOptions.init(self, sp)
         self.parquet_options = <CParquetFragmentScanOptions*> sp.get()
 
     cdef CReaderProperties* reader_properties(self):
         return self.parquet_options.reader_properties.get()
@@ -650,25 +666,57 @@
     def pre_buffer(self):
         return self.arrow_reader_properties().pre_buffer()
 
     @pre_buffer.setter
     def pre_buffer(self, bint pre_buffer):
         self.arrow_reader_properties().set_pre_buffer(pre_buffer)
 
+    @property
+    def thrift_string_size_limit(self):
+        return self.reader_properties().thrift_string_size_limit()
+
+    @thrift_string_size_limit.setter
+    def thrift_string_size_limit(self, size):
+        if size <= 0:
+            raise ValueError("size must be larger than zero")
+        self.reader_properties().set_thrift_string_size_limit(size)
+
+    @property
+    def thrift_container_size_limit(self):
+        return self.reader_properties().thrift_container_size_limit()
+
+    @thrift_container_size_limit.setter
+    def thrift_container_size_limit(self, size):
+        if size <= 0:
+            raise ValueError("size must be larger than zero")
+        self.reader_properties().set_thrift_container_size_limit(size)
+
     def equals(self, ParquetFragmentScanOptions other):
-        return (
-            self.use_buffered_stream == other.use_buffered_stream and
-            self.buffer_size == other.buffer_size and
-            self.pre_buffer == other.pre_buffer
-        )
+        attrs = (
+            self.use_buffered_stream, self.buffer_size, self.pre_buffer,
+            self.thrift_string_size_limit, self.thrift_container_size_limit)
+        other_attrs = (
+            other.use_buffered_stream, other.buffer_size, other.pre_buffer,
+            other.thrift_string_size_limit,
+            other.thrift_container_size_limit)
+        return attrs == other_attrs
+
+    @classmethod
+    def _reconstruct(cls, kwargs):
+        return cls(**kwargs)
 
     def __reduce__(self):
-        return ParquetFragmentScanOptions, (
-            self.use_buffered_stream, self.buffer_size, self.pre_buffer
+        kwargs = dict(
+            use_buffered_stream=self.use_buffered_stream,
+            buffer_size=self.buffer_size,
+            pre_buffer=self.pre_buffer,
+            thrift_string_size_limit=self.thrift_string_size_limit,
+            thrift_container_size_limit=self.thrift_container_size_limit,
         )
+        return type(self)._reconstruct, (kwargs,)
 
 
 cdef class ParquetFactoryOptions(_Weakrefable):
     """
     Influences the discovery of parquet dataset.
 
     Parameters
```

### Comparing `pyarrow-8.0.0/pyarrow/_exec_plan.pyx` & `pyarrow-9.0.0/pyarrow/_exec_plan.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         If the duplicated keys should be omitted from one of the sides
         in the join result.
     output_type: Table or InMemoryDataset
         The output type for the exec plan result.
 
     Returns
     -------
-    result_table : Table
+    result_table : Table or InMemoryDataset
     """
     cdef:
         vector[CFieldRef] c_left_keys
         vector[CFieldRef] c_right_keys
         vector[CFieldRef] c_left_columns
         vector[CFieldRef] c_right_columns
         vector[CDeclaration] c_decl_plan
@@ -255,21 +255,27 @@
         c_join_type = CJoinType_LEFT_ANTI
         right_columns = []
     elif join_type == "right anti":
         c_join_type = CJoinType_RIGHT_ANTI
         left_columns = []
     elif join_type == "inner":
         c_join_type = CJoinType_INNER
-        right_columns = set(right_columns) - set(right_keys)
+        right_columns = [
+            col for col in right_columns if col not in right_keys_order
+        ]
     elif join_type == "left outer":
         c_join_type = CJoinType_LEFT_OUTER
-        right_columns = set(right_columns) - set(right_keys)
+        right_columns = [
+            col for col in right_columns if col not in right_keys_order
+        ]
     elif join_type == "right outer":
         c_join_type = CJoinType_RIGHT_OUTER
-        left_columns = set(left_columns) - set(left_keys)
+        left_columns = [
+            col for col in left_columns if col not in left_keys_order
+        ]
     elif join_type == "full outer":
         c_join_type = CJoinType_FULL_OUTER
     else:
         raise ValueError("Unsupported join type")
 
     # Turn the columns to vectors of FieldRefs
     # and set aside indices of keys.
@@ -347,7 +353,49 @@
 
     result_table = execplan([left_operand, right_operand],
                             plan=c_decl_plan,
                             output_type=output_type,
                             use_threads=use_threads)
 
     return result_table
+
+
+def _filter_table(table, expression, output_type=Table):
+    """Filter rows of a table or dataset based on the provided expression.
+
+    The result will be an output table with only the rows matching
+    the provided expression.
+
+    Parameters
+    ----------
+    table : Table or Dataset
+        Table or Dataset that should be filtered.
+    expression : Expression
+        The expression on which rows should be filtered.
+    output_type: Table or InMemoryDataset
+        The output type for the filtered result.
+
+    Returns
+    -------
+    result_table : Table or InMemoryDataset
+    """
+    cdef:
+        vector[CDeclaration] c_decl_plan
+        Expression expr = expression
+
+    c_decl_plan.push_back(
+        CDeclaration(tobytes("filter"), CFilterNodeOptions(
+            <CExpression>expr.unwrap(), True
+        ))
+    )
+
+    r = execplan([table], plan=c_decl_plan,
+                 output_type=Table, use_threads=False)
+
+    if output_type == Table:
+        return r
+    elif output_type == InMemoryDataset:
+        # Get rid of special dataset columns
+        # "__fragment_index", "__batch_index", "__last_in_fragment", "__filename"
+        return InMemoryDataset(r.select(table.schema.names))
+    else:
+        raise TypeError("Unsupported output type")
```

### Comparing `pyarrow-8.0.0/pyarrow/_feather.pyx` & `pyarrow-9.0.0/pyarrow/_feather.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_flight.pyx` & `pyarrow-9.0.0/pyarrow/_flight.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import contextlib
 import enum
 import re
 import socket
 import time
 import threading
 import warnings
+import weakref
 
 from cython.operator cimport dereference as deref
 from cython.operator cimport postincrement
 from libcpp cimport bool as c_bool
 
 from pyarrow.lib cimport *
 from pyarrow.lib import (ArrowCancelled, ArrowException, ArrowInvalid,
@@ -2116,15 +2117,16 @@
         return (<FlightError> flight_error).to_status()
 
     if headers:
         for header, values in headers.items():
             if isinstance(values, (str, bytes)):
                 values = (values,)
             # Headers in gRPC (and HTTP/1, HTTP/2) are required to be
-            # valid ASCII.
+            # valid, lowercase ASCII.
+            header = header.lower()
             if isinstance(header, str):
                 header = header.encode("ascii")
             for value in values:
                 if isinstance(value, str):
                     value = value.encode("ascii")
                 # Allow bytes values to pass through.
                 add_headers.AddHeader(header, value)
@@ -2343,14 +2345,16 @@
             None if no headers are to be added. The dictionary should
             have string keys and string or list-of-string values.
 
             Bytes values are allowed, but the underlying transport may
             not support them or may restrict them. For gRPC, binary
             values are only allowed on headers ending in "-bin".
 
+            Header names must be lowercase ASCII.
+
         """
 
     def received_headers(self, headers):
         """A callback when headers are received.
 
         The default implementation does nothing.
 
@@ -2442,14 +2446,16 @@
             None if no headers are to be added. The dictionary should
             have string keys and string or list-of-string values.
 
             Bytes values are allowed, but the underlying transport may
             not support them or may restrict them. For gRPC, binary
             values are only allowed on headers ending in "-bin".
 
+            Header names must be lowercase ASCII.
+
         """
 
     def call_completed(self, exception):
         """A callback when the call finishes.
 
         Parameters
         ----------
@@ -2502,24 +2508,53 @@
         for instance in self.middleware.values():
             more_headers = instance.sending_headers()
             if not more_headers:
                 continue
             # Manually merge with existing headers (since headers are
             # multi-valued)
             for key, values in more_headers.items():
+                # ARROW-16606 gRPC aborts given non-lowercase headers
+                key = key.lower()
                 if isinstance(values, (bytes, str)):
                     values = (values,)
                 headers[key].extend(values)
         return headers
 
     def call_completed(self, exception):
         for instance in self.middleware.values():
             instance.call_completed(exception)
 
 
+cdef class _FlightServerFinalizer(_Weakrefable):
+    """
+    A finalizer that shuts down the server on destruction.
+
+    See ARROW-16597. If the server is still active at interpreter
+    exit, the process may segfault.
+    """
+
+    cdef:
+        shared_ptr[PyFlightServer] server
+
+    def finalize(self):
+        cdef:
+            PyFlightServer* server = self.server.get()
+            CStatus status
+        if server == NULL:
+            return
+        try:
+            with nogil:
+                status = server.Shutdown()
+                if status.ok():
+                    status = server.Wait()
+            check_flight_status(status)
+        finally:
+            self.server.reset()
+
+
 cdef class FlightServerBase(_Weakrefable):
     """A Flight service definition.
 
     To start the server, create an instance of this class with an
     appropriate location. The server will be running as soon as the
     instance is created; it is not required to call :meth:`serve`.
 
@@ -2538,27 +2573,29 @@
         A list of (certificate, key) pairs.
     verify_client : boolean optional, default False
         If True, then enable mutual TLS: require the client to present
         a client certificate, and validate the certificate.
     root_certificates : bytes optional, default None
         If enabling mutual TLS, this specifies the PEM-encoded root
         certificate used to validate client certificates.
-    middleware : list optional, default None
-        A dictionary of :class:`ServerMiddlewareFactory` items. The
-        keys are used to retrieve the middleware instance during calls
-        (see :meth:`ServerCallContext.get_middleware`).
+    middleware : dict optional, default None
+        A dictionary of :class:`ServerMiddlewareFactory` instances. The
+        string keys can be used to retrieve the middleware instance within
+        RPC handlers (see :meth:`ServerCallContext.get_middleware`).
 
     """
 
     cdef:
-        unique_ptr[PyFlightServer] server
+        shared_ptr[PyFlightServer] server
+        object finalizer
 
     def __init__(self, location=None, auth_handler=None,
                  tls_certificates=None, verify_client=None,
                  root_certificates=None, middleware=None):
+        self.finalizer = None
         if isinstance(location, (bytes, str)):
             location = Location(location)
         elif isinstance(location, (tuple, type(None))):
             if location is None:
                 location = ('localhost', 0)
             host, port = location
             if tls_certificates:
@@ -2618,14 +2655,17 @@
         vtable.list_actions = &_list_actions
         vtable.do_action = &_do_action
 
         c_server = new PyFlightServer(self, vtable)
         self.server.reset(c_server)
         with nogil:
             check_flight_status(c_server.Init(deref(c_options)))
+        cdef _FlightServerFinalizer finalizer = _FlightServerFinalizer()
+        finalizer.server = self.server
+        self.finalizer = weakref.finalize(self, finalizer.finalize)
 
     @property
     def port(self):
         """
         Get the port that this server is listening on.
 
         Returns a non-positive value if the operation is invalid
@@ -2839,16 +2879,16 @@
         with nogil:
             self.server.get().Wait()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        self.shutdown()
-        self.wait()
+        if self.finalizer:
+            self.finalizer()
 
 
 def connect(location, **kwargs):
     """
     Connect to a Flight server.
 
     Parameters
```

### Comparing `pyarrow-8.0.0/pyarrow/_fs.pxd` & `pyarrow-9.0.0/pyarrow/_fs.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_fs.pyx` & `pyarrow-9.0.0/pyarrow/_fs.pyx`

 * *Files 19% similar despite different names*

```diff
@@ -96,14 +96,56 @@
         If given, the modification time of the filesystem entry,
         in nanoseconds since the Unix epoch.
         `mtime` and `mtime_ns` are mutually exclusive.
     size : int, default None
         If given, the filesystem entry size in bytes.  This should only
         be given if `type` is `FileType.File`.
 
+    Examples
+    --------
+    Generate a file:
+
+    >>> from pyarrow import fs
+    >>> local = fs.LocalFileSystem()
+    >>> path_fs = local_path + '/pyarrow-fs-example.dat'
+    >>> with local.open_output_stream(path_fs) as stream:
+    ...     stream.write(b'data')
+    4
+
+    Get FileInfo object using ``get_file_info()``:
+
+    >>> file_info = local.get_file_info(path_fs)
+    >>> file_info
+    <FileInfo for '.../pyarrow-fs-example.dat': type=FileType.File, size=4>
+
+    Inspect FileInfo attributes:
+
+    >>> file_info.type
+    <FileType.File: 2>
+
+    >>> file_info.is_file
+    True
+
+    >>> file_info.path
+    '/.../pyarrow-fs-example.dat'
+
+    >>> file_info.base_name
+    'pyarrow-fs-example.dat'
+
+    >>> file_info.size
+    4
+
+    >>> file_info.extension
+    'dat'
+
+    >>> file_info.mtime # doctest: +SKIP
+    datetime.datetime(2022, 6, 29, 7, 56, 10, 873922, tzinfo=datetime.timezone.utc)
+
+    >>> file_info.mtime_ns # doctest: +SKIP
+    1656489370873922073
     """
 
     def __init__(self, path, FileType type=FileType.Unknown, *,
                  mtime=None, mtime_ns=None, size=None):
         self.info.set_path(tobytes(path))
         self.info.set_type(_unwrap_file_type(type))
         if mtime is not None:
@@ -175,23 +217,35 @@
         """
         return self.type == FileType.File
 
     @property
     def path(self):
         """
         The full file path in the filesystem.
+
+        Examples
+        --------
+        >>> file_info = local.get_file_info(path)
+        >>> file_info.path
+        '/.../pyarrow-fs-example.dat'
         """
         return frombytes(self.info.path())
 
     @property
     def base_name(self):
         """
         The file base name.
 
         Component after the last directory separator.
+
+        Examples
+        --------
+        >>> file_info = local.get_file_info(path)
+        >>> file_info.base_name
+        'pyarrow-fs-example.dat'
         """
         return frombytes(self.info.base_name())
 
     @property
     def size(self):
         """
         The size in bytes, if available.
@@ -206,25 +260,37 @@
         size = self.info.size()
         return (size if size != -1 else None)
 
     @property
     def extension(self):
         """
         The file extension.
+
+        Examples
+        --------
+        >>> file_info = local.get_file_info(path)
+        >>> file_info.extension
+        'dat'
         """
         return frombytes(self.info.extension())
 
     @property
     def mtime(self):
         """
         The time of last modification, if available.
 
         Returns
         -------
         mtime : datetime.datetime or None
+
+        Examples
+        --------
+        >>> file_info = local.get_file_info(path)
+        >>> file_info.mtime # doctest: +SKIP
+        datetime.datetime(2022, 6, 29, 7, 56, 10, 873922, tzinfo=datetime.timezone.utc)
         """
         cdef int64_t nanoseconds
         nanoseconds = TimePoint_to_ns(self.info.mtime())
         return (datetime.fromtimestamp(nanoseconds / 1.0e9, timezone.utc)
                 if nanoseconds != -1 else None)
 
     @property
@@ -232,14 +298,20 @@
         """
         The time of last modification, if available, expressed in nanoseconds
         since the Unix epoch.
 
         Returns
         -------
         mtime_ns : int or None
+
+        Examples
+        --------
+        >>> file_info = local.get_file_info(path)
+        >>> file_info.mtime_ns # doctest: +SKIP
+        1656489370873922073
         """
         cdef int64_t nanoseconds
         nanoseconds = TimePoint_to_ns(self.info.mtime())
         return (nanoseconds if nanoseconds != -1 else None)
 
 
 cdef class FileSelector(_Weakrefable):
@@ -256,14 +328,39 @@
         '.' for the current directory and '..' for the parent.
     allow_not_found : bool, default False
         The behavior if `base_dir` doesn't exist in the filesystem.
         If false, an error is returned.
         If true, an empty selection is returned.
     recursive : bool, default False
         Whether to recurse into subdirectories.
+
+    Examples
+    --------
+    List the contents of a directory and subdirectories:
+
+    >>> selector_1 = fs.FileSelector(local_path, recursive=True)
+    >>> local.get_file_info(selector_1) # doctest: +SKIP
+    [<FileInfo for 'tmp/alphabet/example.dat': type=FileType.File, size=4>,
+    <FileInfo for 'tmp/alphabet/subdir': type=FileType.Directory>,
+    <FileInfo for 'tmp/alphabet/subdir/example_copy.dat': type=FileType.File, size=4>]
+
+    List only the contents of the base directory:
+
+    >>> selector_2 = fs.FileSelector(local_path)
+    >>> local.get_file_info(selector_2) # doctest: +SKIP
+    [<FileInfo for 'tmp/alphabet/example.dat': type=FileType.File, size=4>,
+    <FileInfo for 'tmp/alphabet/subdir': type=FileType.Directory>]
+
+    Return empty selection if the directory doesn't exist:
+
+    >>> selector_not_found = fs.FileSelector(local_path + '/missing',
+    ...                                      recursive=True,
+    ...                                      allow_not_found=True)
+    >>> local.get_file_info(selector_not_found)
+    []
     """
 
     def __init__(self, base_dir, bint allow_not_found=False,
                  bint recursive=False):
         self.base_dir = base_dir
         self.recursive = recursive
         self.allow_not_found = allow_not_found
@@ -331,14 +428,30 @@
             URI-based path, for example: file:///some/local/path.
 
         Returns
         -------
         tuple of (FileSystem, str path)
             With (filesystem, path) tuple where path is the abstract path
             inside the FileSystem instance.
+
+        Examples
+        --------
+        Create a new FileSystem subclass from a URI:
+
+        >>> uri = 'file:///{}/pyarrow-fs-example.dat'.format(local_path)
+        >>> local_new, path_new = fs.FileSystem.from_uri(uri)
+        >>> local_new
+        <pyarrow._fs.LocalFileSystem object at ...
+        >>> path_new
+        '/.../pyarrow-fs-example.dat'
+
+        Or from a s3 bucket:
+
+        >>> fs.FileSystem.from_uri("s3://usgs-landsat/collection02/")
+        (<pyarrow._s3fs.S3FileSystem object at ...>, 'usgs-landsat/collection02')
         """
         cdef:
             c_string c_path
             c_string c_uri
             CResult[shared_ptr[CFileSystem]] result
 
         if isinstance(uri, pathlib.Path):
@@ -363,14 +476,17 @@
         elif typ == 'mock':
             self = _MockFileSystem.__new__(_MockFileSystem)
         elif typ == 'subtree':
             self = SubTreeFileSystem.__new__(SubTreeFileSystem)
         elif typ == 's3':
             from pyarrow._s3fs import S3FileSystem
             self = S3FileSystem.__new__(S3FileSystem)
+        elif typ == 'gcs':
+            from pyarrow._gcsfs import GcsFileSystem
+            self = GcsFileSystem.__new__(GcsFileSystem)
         elif typ == 'hdfs':
             from pyarrow._hdfs import HadoopFileSystem
             self = HadoopFileSystem.__new__(HadoopFileSystem)
         elif typ.startswith('py::'):
             self = PyFileSystem.__new__(PyFileSystem)
         else:
             raise TypeError('Cannot wrap FileSystem pointer')
@@ -415,14 +531,21 @@
             use `allow_not_found`.
 
         Returns
         -------
         FileInfo or list of FileInfo
             Single FileInfo object is returned for a single path, otherwise
             a list of FileInfo objects is returned.
+
+        Examples
+        --------
+        >>> local
+        <pyarrow._fs.LocalFileSystem object at ...>
+        >>> local.get_file_info("/{}/pyarrow-fs-example.dat".format(local_path))
+        <FileInfo for '/.../pyarrow-fs-example.dat': type=FileType.File, size=4>
         """
         cdef:
             CFileInfo info
             c_string path
             vector[CFileInfo] infos
             vector[c_string] paths
             CFileSelector selector
@@ -514,14 +637,36 @@
 
         Parameters
         ----------
         src : str
             The path of the file or the directory to be moved.
         dest : str
             The destination path where the file or directory is moved to.
+
+        Examples
+        --------
+        Create a new folder with a file:
+
+        >>> local.create_dir('/tmp/other_dir')
+        >>> local.copy_file(path,'/tmp/move_example.dat')
+
+        Move the file:
+
+        >>> local.move('/tmp/move_example.dat',
+        ...            '/tmp/other_dir/move_example_2.dat')
+
+        Inspect the file info:
+
+        >>> local.get_file_info('/tmp/other_dir/move_example_2.dat')
+        <FileInfo for '/tmp/other_dir/move_example_2.dat': type=FileType.File, size=4>
+        >>> local.get_file_info('/tmp/move_example.dat')
+        <FileInfo for '/tmp/move_example.dat': type=FileType.NotFound>
+
+        Delete the folder:
+        >>> local.delete_dir('/tmp/other_dir')
         """
         cdef:
             c_string source = _path_as_bytes(src)
             c_string destination = _path_as_bytes(dest)
         with nogil:
             check_status(self.fs.Move(source, destination))
 
@@ -534,14 +679,26 @@
 
         Parameters
         ----------
         src : str
             The path of the file to be copied from.
         dest : str
             The destination path where the file is copied to.
+
+        Examples
+        --------
+        >>> local.copy_file(path,
+        ...                 local_path + '/pyarrow-fs-example_copy.dat')
+
+        Inspect the file info:
+
+        >>> local.get_file_info(local_path + '/pyarrow-fs-example_copy.dat')
+        <FileInfo for '/.../pyarrow-fs-example_copy.dat': type=FileType.File, size=4>
+        >>> local.get_file_info(path)
+        <FileInfo for '/.../pyarrow-fs-example.dat': type=FileType.File, size=4>
         """
         cdef:
             c_string source = _path_as_bytes(src)
             c_string destination = _path_as_bytes(dest)
         with nogil:
             check_status(self.fs.CopyFile(source, destination))
 
@@ -584,14 +741,22 @@
         ----------
         path : str
             The source to open for reading.
 
         Returns
         -------
         stream : NativeFile
+
+        Examples
+        --------
+        Print the data from the file with `open_input_file()`:
+
+        >>> with local.open_input_file(path) as f:
+        ...     print(f.readall())
+        b'data'
         """
         cdef:
             c_string pathstr = _path_as_bytes(path)
             NativeFile stream = NativeFile()
             shared_ptr[CRandomAccessFile] in_handle
 
         with nogil:
@@ -618,14 +783,22 @@
         buffer_size : int optional, default None
             If None or 0, no buffering will happen. Otherwise the size of the
             temporary read buffer.
 
         Returns
         -------
         stream : NativeFile
+
+        Examples        
+        --------
+        Print the data from the file with `open_input_stream()`:
+
+        >>> with local.open_input_stream(path) as f:
+        ...     print(f.readall())
+        b'data'
         """
         cdef:
             c_string pathstr = _path_as_bytes(path)
             NativeFile stream = NativeFile()
             shared_ptr[CInputStream] in_handle
 
         with nogil:
@@ -663,14 +836,21 @@
             Some filesystems support storing metadata along the file
             (such as "Content-Type").
             Unsupported metadata keys will be ignored.
 
         Returns
         -------
         stream : NativeFile
+
+        Examples
+        --------
+        >>> local = fs.LocalFileSystem()
+        >>> with local.open_output_stream(path) as stream:
+        ...     stream.write(b'data')
+        4
         """
         cdef:
             c_string pathstr = _path_as_bytes(path)
             NativeFile stream = NativeFile()
             shared_ptr[COutputStream] out_handle
             shared_ptr[const CKeyValueMetadata] c_metadata
 
@@ -720,14 +900,28 @@
             Some filesystems support storing metadata along the file
             (such as "Content-Type").
             Unsupported metadata keys will be ignored.
 
         Returns
         -------
         stream : NativeFile
+
+        Examples        
+        --------
+        Append new data to a FileSystem subclass with nonempty file:
+
+        >>> with local.open_append_stream(path) as f:
+        ...     f.write(b'+newly added')
+        12
+
+        Print out the content fo the file:
+
+        >>> with local.open_input_file(path) as f:
+        ...     print(f.readall())
+        b'data+newly added'
         """
         cdef:
             c_string pathstr = _path_as_bytes(path)
             NativeFile stream = NativeFile()
             shared_ptr[COutputStream] out_handle
             shared_ptr[const CKeyValueMetadata] c_metadata
 
@@ -775,14 +969,114 @@
     except when deleting an entry).
 
     Parameters
     ----------
     use_mmap : bool, default False
         Whether open_input_stream and open_input_file should return
         a mmap'ed file or a regular file.
+
+    Examples
+    --------
+    Create a FileSystem object with LocalFileSystem constructor:
+
+    >>> from pyarrow import fs
+    >>> local = fs.LocalFileSystem()
+    >>> local
+    <pyarrow._fs.LocalFileSystem object at ...>
+
+    and write data on to the file:
+
+    >>> with local.open_output_stream('/tmp/local_fs.dat') as stream:
+    ...     stream.write(b'data')
+    4
+    >>> with local.open_input_stream('/tmp/local_fs.dat') as stream:
+    ...     print(stream.readall())
+    b'data'
+
+    Create a FileSystem object inferred from a URI of the saved file:
+
+    >>> local_new, path = fs.LocalFileSystem().from_uri('/tmp/local_fs.dat')
+    >>> local_new
+    <pyarrow._fs.LocalFileSystem object at ...
+    >>> path
+    '/tmp/local_fs.dat'
+
+    Check if FileSystems `local` and `local_new` are equal:
+
+    >>> local.equals(local_new)
+    True
+
+    Compare two different FileSystems:
+
+    >>> local2 = fs.LocalFileSystem(use_mmap=True)
+    >>> local.equals(local2)
+    False
+
+    Copy a file and print out the data:
+
+    >>> local.copy_file('/tmp/local_fs.dat', '/tmp/local_fs-copy.dat')
+    >>> with local.open_input_stream('/tmp/local_fs-copy.dat') as stream:
+    ...     print(stream.readall())
+    ...
+    b'data'
+
+    Open an output stream for appending, add text and print the new data:
+
+    >>> with local.open_append_stream('/tmp/local_fs-copy.dat') as f:
+    ...     f.write(b'+newly added')
+    12
+
+    >>> with local.open_input_stream('/tmp/local_fs-copy.dat') as f:
+    ...     print(f.readall())
+    b'data+newly added'
+
+    Create a directory, copy a file into it and then delete the whole directory:
+
+    >>> local.create_dir('/tmp/new_folder')
+    >>> local.copy_file('/tmp/local_fs.dat', '/tmp/new_folder/local_fs.dat')
+    >>> local.get_file_info('/tmp/new_folder')
+    <FileInfo for '/tmp/new_folder': type=FileType.Directory>
+    >>> local.delete_dir('/tmp/new_folder')
+    >>> local.get_file_info('/tmp/new_folder')
+    <FileInfo for '/tmp/new_folder': type=FileType.NotFound>
+
+    Create a directory, copy a file into it and then delete
+    the content of the directory:
+
+    >>> local.create_dir('/tmp/new_folder')
+    >>> local.copy_file('/tmp/local_fs.dat', '/tmp/new_folder/local_fs.dat')
+    >>> local.get_file_info('/tmp/new_folder/local_fs.dat')
+    <FileInfo for '/tmp/new_folder/local_fs.dat': type=FileType.File, size=4>
+    >>> local.delete_dir_contents('/tmp/new_folder')
+    >>> local.get_file_info('/tmp/new_folder')
+    <FileInfo for '/tmp/new_folder': type=FileType.Directory>
+    >>> local.get_file_info('/tmp/new_folder/local_fs.dat')
+    <FileInfo for '/tmp/new_folder/local_fs.dat': type=FileType.NotFound>
+
+    Create a directory, copy a file into it and then delete
+    the file from the directory:
+
+    >>> local.create_dir('/tmp/new_folder')
+    >>> local.copy_file('/tmp/local_fs.dat', '/tmp/new_folder/local_fs.dat')
+    >>> local.delete_file('/tmp/new_folder/local_fs.dat')
+    >>> local.get_file_info('/tmp/new_folder/local_fs.dat')
+    <FileInfo for '/tmp/new_folder/local_fs.dat': type=FileType.NotFound>
+    >>> local.get_file_info('/tmp/new_folder')
+    <FileInfo for '/tmp/new_folder': type=FileType.Directory>
+
+    Move the file:
+
+    >>> local.move('/tmp/local_fs-copy.dat', '/tmp/new_folder/local_fs-copy.dat')
+    >>> local.get_file_info('/tmp/new_folder/local_fs-copy.dat')
+    <FileInfo for '/tmp/new_folder/local_fs-copy.dat': type=FileType.File, size=16>
+    >>> local.get_file_info('/tmp/local_fs-copy.dat')
+    <FileInfo for '/tmp/local_fs-copy.dat': type=FileType.NotFound>
+
+    To finish delete the file left:
+    >>> local.delete_file('/tmp/local_fs.dat')
     """
 
     def __init__(self, *, use_mmap=False):
         cdef:
             CLocalFileSystemOptions opts
             shared_ptr[CLocalFileSystem] fs
 
@@ -821,14 +1115,57 @@
 
     Parameters
     ----------
     base_path : str
         The root of the subtree.
     base_fs : FileSystem
         FileSystem object the operations delegated to.
+
+    Examples
+    --------
+    Create a LocalFileSystem instance:
+
+    >>> from pyarrow import fs
+    >>> local = fs.LocalFileSystem()
+    >>> with local.open_output_stream('/tmp/local_fs.dat') as stream:
+    ...     stream.write(b'data') 
+    4
+
+    Create a directory and a SubTreeFileSystem instance:
+
+    >>> local.create_dir('/tmp/sub_tree')
+    >>> subtree = fs.SubTreeFileSystem('/tmp/sub_tree', local)
+
+    Write data into the existing file:
+
+    >>> with subtree.open_append_stream('sub_tree_fs.dat') as f:
+    ...     f.write(b'+newly added')
+    12
+
+    Print out the attributes:
+
+    >>> subtree.base_fs
+    <pyarrow._fs.LocalFileSystem object at ...>
+    >>> subtree.base_path
+    '/tmp/sub_tree/'
+
+    Get info for the given directory or given file:
+
+    >>> subtree.get_file_info('')
+    <FileInfo for '': type=FileType.Directory>
+    >>> subtree.get_file_info('sub_tree_fs.dat')
+    <FileInfo for 'sub_tree_fs.dat': type=FileType.File, size=12>
+
+    Delete the file and directory:
+
+    >>> subtree.delete_file('sub_tree_fs.dat')
+    >>> local.delete_dir('/tmp/sub_tree')
+    >>> local.delete_file('/tmp/local_fs.dat')
+
+    For usage of the methods see examples for :func:`~pyarrow.fs.LocalFileSystem`.
     """
 
     def __init__(self, base_path, FileSystem base_fs):
         cdef:
             c_string pathstr
             shared_ptr[CSubTreeFileSystem] wrapped
 
@@ -881,14 +1218,31 @@
     """
     A FileSystem with behavior implemented in Python.
 
     Parameters
     ----------
     handler : FileSystemHandler
         The handler object implementing custom filesystem behavior.
+
+    Examples
+    --------
+    Create an fsspec-based filesystem object for GitHub:
+
+    >>> from fsspec.implementations import github
+    >>> gfs = github.GithubFileSystem('apache', 'arrow', sha='ec51aec4d15035f4d9d6a1c4346d0a2b9a37fb75')
+
+    Get a PyArrow FileSystem object:
+
+    >>> from pyarrow.fs import PyFileSystem, FSSpecHandler
+    >>> pa_fs = PyFileSystem(FSSpecHandler(gfs))
+
+    Use :func:`~pyarrow.fs.FileSystem` functionality ``get_file_info()``:
+
+    >>> pa_fs.get_file_info('README.md')
+    <FileInfo for 'README.md': type=FileType.File, size=5302>
     """
 
     def __init__(self, handler):
         cdef:
             CPyFileSystemVtable vtable
             shared_ptr[CPyFileSystem] wrapped
```

### Comparing `pyarrow-8.0.0/pyarrow/_hdfs.pyx` & `pyarrow-9.0.0/pyarrow/_hdfs.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,21 @@
         None means the default configuration for HDFS, a typical block size is
         128 MB.
     kerb_ticket : string or path, default None
         If not None, the path to the Kerberos ticket cache.
     extra_conf : dict, default None
         Extra key/value pairs for configuration; will override any
         hdfs-site.xml properties.
+
+    Examples
+    --------
+    >>> from pyarrow import fs
+    >>> hdfs = fs.HadoopFileSystem(host, port, user=user, kerb_ticket=ticket_cache_path) # doctest: +SKIP
+
+    For usage of the methods see examples for :func:`~pyarrow.fs.LocalFileSystem`.
     """
 
     cdef:
         CHadoopFileSystem* hdfs
 
     def __init__(self, str host, int port=8020, *, str user=None,
                  int replication=3, int buffer_size=0,
```

### Comparing `pyarrow-8.0.0/pyarrow/_hdfsio.pyx` & `pyarrow-9.0.0/pyarrow/_hdfsio.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_json.pyx` & `pyarrow-9.0.0/pyarrow/_json.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_orc.pxd` & `pyarrow-9.0.0/pyarrow/_orc.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_orc.pyx` & `pyarrow-9.0.0/pyarrow/_orc.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_parquet.pxd` & `pyarrow-9.0.0/pyarrow/_parquet.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -355,16 +355,24 @@
         " parquet::FileMetaData::Make"(const void* serialized_metadata,
                                        uint32_t* metadata_len)
 
     cdef cppclass CReaderProperties" parquet::ReaderProperties":
         c_bool is_buffered_stream_enabled() const
         void enable_buffered_stream()
         void disable_buffered_stream()
+
         void set_buffer_size(int64_t buf_size)
         int64_t buffer_size() const
+
+        void set_thrift_string_size_limit(int32_t size)
+        int32_t thrift_string_size_limit() const
+
+        void set_thrift_container_size_limit(int32_t size)
+        int32_t thrift_container_size_limit() const
+
         void file_decryption_properties(shared_ptr[CFileDecryptionProperties]
                                         decryption)
         shared_ptr[CFileDecryptionProperties] file_decryption_properties() \
             const
 
     CReaderProperties default_reader_properties()
```

### Comparing `pyarrow-8.0.0/pyarrow/_parquet.pyx` & `pyarrow-9.0.0/pyarrow/_parquet.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         """
         Get a JSON string containing type and type parameters.
 
         Returns
         -------
         json : str
             JSON representation of type, with at least a field called 'Type'
-            which contains the type name. If the type is parameterized, such 
+            which contains the type name. If the type is parameterized, such
             as a decimal with scale and precision, will contain those as fields
             as well.
         """
         return frombytes(self.type.get().ToJSON())
 
     @property
     def type(self):
@@ -440,15 +440,15 @@
         return statistics
 
     @property
     def compression(self):
         """
         Type of compression used for column (str).
 
-        One of 'UNCOMPRESSED', 'SNAPPY', 'GZIP', 'LZO', 'BROTLI', 'LZ4', 'ZSTD', 
+        One of 'UNCOMPRESSED', 'SNAPPY', 'GZIP', 'LZO', 'BROTLI', 'LZ4', 'ZSTD',
         or 'UNKNOWN'.
         """
         return compression_name_from_enum(self.metadata.compression())
 
     @property
     def encodings(self):
         """
@@ -663,15 +663,15 @@
 
     def __eq__(self, other):
         try:
             return self.equals(other)
         except TypeError:
             return NotImplemented
 
-    def equals(self, FileMetaData other):
+    def equals(self, FileMetaData other not None):
         """
         Return whether the two file metadata objects are equal.
 
         Parameters
         ----------
         other : FileMetaData
             Metadata to compare against.
@@ -710,29 +710,29 @@
         return self._metadata.num_row_groups()
 
     @property
     def format_version(self):
         """
         Parquet format version used in file (str, such as '1.0', '2.4').
 
-        If version is missing or unparsable, will default to assuming '1.0'.
+        If version is missing or unparsable, will default to assuming '2.4'.
         """
         cdef ParquetVersion version = self._metadata.version()
         if version == ParquetVersion_V1:
             return '1.0'
         elif version == ParquetVersion_V2_0:
             return 'pseudo-2.0'
         elif version == ParquetVersion_V2_4:
             return '2.4'
         elif version == ParquetVersion_V2_6:
             return '2.6'
         else:
-            warnings.warn('Unrecognized file version, assuming 1.0: {}'
+            warnings.warn('Unrecognized file version, assuming 2.4: {}'
                           .format(version))
-            return '1.0'
+            return '2.4'
 
     @property
     def created_by(self):
         """
         String describing source of the parquet file (str).
 
         This typically includes library name and version number. For example, Arrow 7.0's
@@ -1163,19 +1163,21 @@
     cdef public:
         _column_idx_map
 
     def __cinit__(self, MemoryPool memory_pool=None):
         self.pool = maybe_unbox_memory_pool(memory_pool)
         self._metadata = None
 
-    def open(self, object source not None, bint use_memory_map=True,
+    def open(self, object source not None, *, bint use_memory_map=False,
              read_dictionary=None, FileMetaData metadata=None,
              int buffer_size=0, bint pre_buffer=False,
              coerce_int96_timestamp_unit=None,
-             FileDecryptionProperties decryption_properties=None):
+             FileDecryptionProperties decryption_properties=None,
+             thrift_string_size_limit=None,
+             thrift_container_size_limit=None):
         cdef:
             shared_ptr[CRandomAccessFile] rd_handle
             shared_ptr[CFileMetaData] c_metadata
             CReaderProperties properties = default_reader_properties()
             ArrowReaderProperties arrow_props = (
                 default_arrow_reader_properties())
             c_string path
@@ -1189,14 +1191,26 @@
             properties.enable_buffered_stream()
             properties.set_buffer_size(buffer_size)
         elif buffer_size == 0:
             properties.disable_buffered_stream()
         else:
             raise ValueError('Buffer size must be larger than zero')
 
+        if thrift_string_size_limit is not None:
+            if thrift_string_size_limit <= 0:
+                raise ValueError("thrift_string_size_limit "
+                                 "must be larger than zero")
+            properties.set_thrift_string_size_limit(thrift_string_size_limit)
+        if thrift_container_size_limit is not None:
+            if thrift_container_size_limit <= 0:
+                raise ValueError("thrift_container_size_limit "
+                                 "must be larger than zero")
+            properties.set_thrift_container_size_limit(
+                thrift_container_size_limit)
+
         if decryption_properties is not None:
             properties.file_decryption_properties(
                 decryption_properties.unwrap())
 
         arrow_props.set_pre_buffer(pre_buffer)
 
         if coerce_int96_timestamp_unit is None:
@@ -1417,21 +1431,14 @@
     def read_column(self, int column_index):
         cdef shared_ptr[CChunkedArray] out
         with nogil:
             check_status(self.reader.get()
                          .ReadColumn(column_index, &out))
         return pyarrow_wrap_chunked_array(out)
 
-    def read_schema_field(self, int field_index):
-        cdef shared_ptr[CChunkedArray] out
-        with nogil:
-            check_status(self.reader.get()
-                         .ReadSchemaField(field_index, &out))
-        return pyarrow_wrap_chunked_array(out)
-
 
 cdef shared_ptr[WriterProperties] _create_writer_properties(
         use_dictionary=None,
         compression=None,
         version=None,
         write_statistics=None,
         data_page_size=None,
```

### Comparing `pyarrow-8.0.0/pyarrow/_parquet_encryption.pxd` & `pyarrow-9.0.0/pyarrow/_parquet_encryption.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_parquet_encryption.pyx` & `pyarrow-9.0.0/pyarrow/_parquet_encryption.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_plasma.pyx` & `pyarrow-9.0.0/pyarrow/_plasma.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/_s3fs.pyx` & `pyarrow-9.0.0/pyarrow/_s3fs.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     """
     Initialize S3 support
 
     Parameters
     ----------
     log_level : S3LogLevel
         level of logging
+
+    Examples
+    --------
+    >>> fs.initialize_s3(fs.S3LogLevel.Error) # doctest: +SKIP
     """
     cdef CS3GlobalOptions options
     options.log_level = <CS3LogLevel> log_level
     check_status(CInitializeS3(options))
 
 
 def finalize_s3():
@@ -66,15 +70,15 @@
     Returns
     -------
     region : str
         A S3 region name
 
     Examples
     --------
-    >>> resolve_s3_region('ursa-labs-taxi-data')
+    >>> fs.resolve_s3_region('voltrondata-labs-datasets')
     'us-east-2'
     """
     cdef:
         c_string c_bucket
         c_string c_region
 
     c_bucket = tobytes(bucket)
@@ -95,14 +99,20 @@
     If role_arn is provided instead of access_key and secret_key, temporary
     credentials will be fetched by issuing a request to STS to assume the
     specified role.
 
     Note: S3 buckets are special and the operations available on them may be
     limited or more expensive than desired.
 
+    When S3FileSystem creates new buckets (assuming allow_bucket_creation is 
+    True), it does not pass any non-default settings. In AWS S3, the bucket and 
+    all objects will be not publicly visible, and will have no bucket policies 
+    and no resource tags. To have more control over how buckets are created,
+    use a different API to create them.
+
     Parameters
     ----------
     access_key : str, default None
         AWS Access Key ID. Pass None to use the standard AWS environment
         variables and/or configuration file.
     secret_key : str, default None
         AWS Secret Access key. Pass None to use the standard AWS environment
@@ -146,24 +156,42 @@
         will be derived from the provided URI.
         The following are equivalent::
 
             S3FileSystem(proxy_options='http://username:password@localhost:8020')
             S3FileSystem(proxy_options={'scheme': 'http', 'host': 'localhost',
                                         'port': 8020, 'username': 'username',
                                         'password': 'password'})
+    allow_bucket_creation : bool, default False
+        Whether to allow CreateDir at the bucket-level. This option may also be 
+        passed in a URI query parameter.
+    allow_bucket_deletion : bool, default False
+        Whether to allow DeleteDir at the bucket-level. This option may also be 
+        passed in a URI query parameter.
+
+    Examples
+    --------
+    >>> from pyarrow import fs
+    >>> s3 = fs.S3FileSystem(region='us-west-2')
+    >>> s3.get_file_info(fs.FileSelector(
+    ...    'power-analysis-ready-datastore/power_901_constants.zarr/FROCEAN', recursive=True
+    ... ))
+    [<FileInfo for 'power-analysis-ready-datastore/power_901_constants.zarr/FROCEAN/.zarray...
+
+    For usage of the methods see examples for :func:`~pyarrow.fs.LocalFileSystem`.
     """
 
     cdef:
         CS3FileSystem* s3fs
 
     def __init__(self, *, access_key=None, secret_key=None, session_token=None,
                  bint anonymous=False, region=None, scheme=None,
                  endpoint_override=None, bint background_writes=True,
                  default_metadata=None, role_arn=None, session_name=None,
-                 external_id=None, load_frequency=900, proxy_options=None):
+                 external_id=None, load_frequency=900, proxy_options=None,
+                 allow_bucket_creation=False, allow_bucket_deletion=False):
         cdef:
             CS3Options options
             shared_ptr[CS3FileSystem] wrapped
 
         if access_key is not None and secret_key is None:
             raise ValueError(
                 'In order to initialize with explicit credentials both '
@@ -206,14 +234,18 @@
         elif anonymous:
             if role_arn:
                 raise ValueError(
                     'Cannot provide role_arn with anonymous=True')
 
             options = CS3Options.Anonymous()
         elif role_arn:
+            if session_name is None:
+                session_name = ''
+            if external_id is None:
+                external_id = ''
 
             options = CS3Options.FromAssumeRole(
                 tobytes(role_arn),
                 tobytes(session_name),
                 tobytes(external_id),
                 load_frequency
             )
@@ -249,14 +281,17 @@
                 options.proxy_options = GetResultValue(
                     CS3ProxyOptions.FromUriString(tobytes(proxy_options)))
             else:
                 raise TypeError(
                     "'proxy_options': expected 'dict' or 'str', "
                     f"got {type(proxy_options)} instead.")
 
+        options.allow_bucket_creation = allow_bucket_creation
+        options.allow_bucket_deletion = allow_bucket_deletion
+
         with nogil:
             wrapped = GetResultValue(CS3FileSystem.Make(options))
 
         self.init(<shared_ptr[CFileSystem]> wrapped)
 
     cdef init(self, const shared_ptr[CFileSystem]& wrapped):
         FileSystem.init(self, wrapped)
@@ -291,22 +326,24 @@
                 scheme=frombytes(opts.scheme),
                 endpoint_override=frombytes(opts.endpoint_override),
                 role_arn=frombytes(opts.role_arn),
                 session_name=frombytes(opts.session_name),
                 external_id=frombytes(opts.external_id),
                 load_frequency=opts.load_frequency,
                 background_writes=opts.background_writes,
+                allow_bucket_creation=opts.allow_bucket_creation,
+                allow_bucket_deletion=opts.allow_bucket_deletion,
                 default_metadata=pyarrow_wrap_metadata(opts.default_metadata),
                 proxy_options={'scheme': frombytes(opts.proxy_options.scheme),
                                'host': frombytes(opts.proxy_options.host),
                                'port': opts.proxy_options.port,
                                'username': frombytes(
                                    opts.proxy_options.username),
                                'password': frombytes(
-                                   opts.proxy_options.password)}
+                                   opts.proxy_options.password)},
             ),)
         )
 
     @property
     def region(self):
         """
         The AWS region this filesystem connects to.
```

### Comparing `pyarrow-8.0.0/pyarrow/array.pxi` & `pyarrow-9.0.0/pyarrow/array.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -178,37 +178,38 @@
     explicit index type will not be demoted even if it is wider than required.
 
     Examples
     --------
     >>> import pandas as pd
     >>> import pyarrow as pa
     >>> pa.array(pd.Series([1, 2]))
-    <pyarrow.lib.Int64Array object at 0x7f674e4c0e10>
+    <pyarrow.lib.Int64Array object at ...>
     [
       1,
       2
     ]
 
     >>> pa.array(["a", "b", "a"], type=pa.dictionary(pa.int8(), pa.string()))
-    <pyarrow.lib.DictionaryArray object at 0x7feb288d9040>
+    <pyarrow.lib.DictionaryArray object at ...>
+    ...
     -- dictionary:
-    [
-      "a",
-      "b"
-    ]
+      [
+        "a",
+        "b"
+      ]
     -- indices:
-    [
-      0,
-      1,
-      0
-    ]
+      [
+        0,
+        1,
+        0
+      ]
 
     >>> import numpy as np
     >>> pa.array(pd.Series([1, 2]), mask=np.array([0, 1], dtype=bool))
-    <pyarrow.lib.Int64Array object at 0x7f9019e11208>
+    <pyarrow.lib.Int64Array object at ...>
     [
       1,
       null
     ]
 
     >>> arr = pa.array(range(1024), type=pa.dictionary(pa.int8(), pa.int64()))
     >>> arr.type.index_type
@@ -360,19 +361,19 @@
     -------
     arr : Array
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> pa.nulls(10)
-    <pyarrow.lib.NullArray object at 0x7ffaf04c2e50>
+    <pyarrow.lib.NullArray object at ...>
     10 nulls
 
     >>> pa.nulls(3, pa.uint32())
-    <pyarrow.lib.UInt32Array object at 0x7ffaf04c2e50>
+    <pyarrow.lib.UInt32Array object at ...>
     [
       null,
       null,
       null
     ]
     """
     cdef:
@@ -410,44 +411,44 @@
     -------
     arr : Array
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> pa.repeat(10, 3)
-    <pyarrow.lib.Int64Array object at 0x7ffac03a2750>
+    <pyarrow.lib.Int64Array object at ...>
     [
       10,
       10,
       10
     ]
 
     >>> pa.repeat([1, 2], 2)
-    <pyarrow.lib.ListArray object at 0x7ffaf04c2e50>
+    <pyarrow.lib.ListArray object at ...>
     [
       [
         1,
         2
       ],
       [
         1,
         2
       ]
     ]
 
     >>> pa.repeat("string", 3)
-    <pyarrow.lib.StringArray object at 0x7ffac03a2750>
+    <pyarrow.lib.StringArray object at ...>
     [
       "string",
       "string",
       "string"
     ]
 
     >>> pa.repeat(pa.scalar({'a': 1, 'b': [1, 2]}), 2)
-    <pyarrow.lib.StructArray object at 0x7ffac03a2750>
+    <pyarrow.lib.StructArray object at ...>
     -- is_valid: all not null
     -- child 0 type: int64
       [
         1,
         1
       ]
     -- child 1 type: list<item: int64>
@@ -875,48 +876,51 @@
         Returns
         -------
         diff : str
             A human-readable printout of the differences.
 
         Examples
         --------
+        >>> import pyarrow as pa
         >>> left = pa.array(["one", "two", "three"])
         >>> right = pa.array(["two", None, "two-and-a-half", "three"])
-        >>> print(left.diff(right))
+        >>> print(left.diff(right)) # doctest: +SKIP
 
         @@ -0, +0 @@
         -"one"
         @@ -2, +1 @@
         +null
         +"two-and-a-half"
 
         """
         cdef c_string result
         with nogil:
             result = self.ap.Diff(deref(other.ap))
         return frombytes(result, safe=True)
 
-    def cast(self, object target_type, safe=True):
+    def cast(self, object target_type=None, safe=None, options=None):
         """
         Cast array values to another data type
 
         See :func:`pyarrow.compute.cast` for usage.
 
         Parameters
         ----------
-        target_type : DataType
+        target_type : DataType, default None
             Type to cast array to.
         safe : boolean, default True
             Whether to check for conversion errors such as overflow.
+        options : CastOptions, default None
+            Additional checks pass by CastOptions
 
         Returns
         -------
         cast : Array
         """
-        return _pc().cast(self, target_type, safe=safe)
+        return _pc().cast(self, target_type, safe=safe, options=options)
 
     def view(self, object target_type):
         """
         Return zero-copy "view" of array as another data type.
 
         The data types must have compatible columnar buffer layouts
 
@@ -1840,18 +1844,19 @@
         """
         Return array of same length as list child values array where each
         output value is the index of the parent list array slot containing each
         child value.
 
         Examples
         --------
+        >>> import pyarrow as pa
         >>> arr = pa.array([[1, 2, 3], [], None, [4]],
         ...                type=pa.list_(pa.int32()))
         >>> arr.value_parent_indices()
-        <pyarrow.lib.Int32Array object at 0x7efc5db958a0>
+        <pyarrow.lib.Int64Array object at ...>
         [
           0,
           0,
           0,
           3
         ]
         """
@@ -1860,18 +1865,19 @@
     def value_lengths(self):
         """
         Return integers array with values equal to the respective length of
         each list element. Null list values are null in the output.
 
         Examples
         --------
+        >>> import pyarrow as pa
         >>> arr = pa.array([[1, 2, 3], [], None, [4]],
         ...                type=pa.list_(pa.int32()))
         >>> arr.value_lengths()
-        <pyarrow.lib.Int32Array object at 0x7efc5db95910>
+        <pyarrow.lib.Int32Array object at ...>
         [
           3,
           0,
           null,
           1
         ]
         """
@@ -1899,41 +1905,42 @@
 
         Returns
         -------
         list_array : ListArray
 
         Examples
         --------
+        >>> import pyarrow as pa
         >>> values = pa.array([1, 2, 3, 4])
         >>> offsets = pa.array([0, 2, 4])
         >>> pa.ListArray.from_arrays(offsets, values)
-        <pyarrow.lib.ListArray object at 0x7fbde226bf40>
+        <pyarrow.lib.ListArray object at ...>
         [
           [
-            0,
-            1
+            1,
+            2
           ],
           [
-            2,
-            3
+            3,
+            4
           ]
         ]
-        # nulls in the offsets array become null lists
+        >>> # nulls in the offsets array become null lists
         >>> offsets = pa.array([0, None, 2, 4])
         >>> pa.ListArray.from_arrays(offsets, values)
-        <pyarrow.lib.ListArray object at 0x7fbde226bf40>
+        <pyarrow.lib.ListArray object at ...>
         [
           [
-            0,
-            1
+            1,
+            2
           ],
           null,
           [
-            2,
-            3
+            3,
+            4
           ]
         ]
         """
         cdef:
             Array _offsets, _values
             shared_ptr[CArray] out
         cdef CMemoryPool* cpool = maybe_unbox_memory_pool(pool)
@@ -1971,17 +1978,18 @@
 
         Returns
         -------
         offsets : Int32Array
 
         Examples
         --------
-        >>> array = pa.array([[1, 2], None, [3, 4, 5])
+        >>> import pyarrow as pa
+        >>> array = pa.array([[1, 2], None, [3, 4, 5]])
         >>> array.offsets
-        <pyarrow.lib.Int32Array object at 0x7f3adc4776a0>
+        <pyarrow.lib.Int32Array object at ...>
         [
           0,
           2,
           2,
           5
         ]
         """
@@ -2130,33 +2138,46 @@
         FixedSizeListArray
 
         Examples
         --------
 
         Create from a values array and a list size:
 
+        >>> import pyarrow as pa
         >>> values = pa.array([1, 2, 3, 4])
         >>> arr = pa.FixedSizeListArray.from_arrays(values, 2)
         >>> arr
-        <pyarrow.lib.FixedSizeListArray object at 0x7f6436df3a00>
+        <pyarrow.lib.FixedSizeListArray object at ...>
         [
           [
             1,
             2
           ],
           [
             3,
             4
           ]
         ]
 
-        Or create from a values array and matching type:
-
-        >>> arr = pa.FixedSizeListArray.from_arrays(values, type=pa.list_(2))
+        Or create from a values array, list size and matching type:
 
+        >>> typ = pa.list_(pa.field("values", pa.int64()), 2)
+        >>> arr = pa.FixedSizeListArray.from_arrays(values,type=typ)
+        >>> arr
+        <pyarrow.lib.FixedSizeListArray object at ...>
+        [
+          [
+            1,
+            2
+          ],
+          [
+            3,
+            4
+          ]
+        ]
         """
         cdef:
             Array _values
             int32_t _list_size
             CResult[shared_ptr[CArray]] c_result
 
         _values = asarray(values)
@@ -2838,15 +2859,15 @@
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> arr1 = pa.array([2, 4, 5, 100])
     >>> arr2 = pa.array([2, 4])
     >>> pa.concat_arrays([arr1, arr2])
-    <pyarrow.lib.Int64Array object at 0x1166eb1c0>
+    <pyarrow.lib.Int64Array object at ...>
     [
       2,
       4,
       5,
       100,
       2,
       4
```

### Comparing `pyarrow-8.0.0/pyarrow/benchmark.pxi` & `pyarrow-9.0.0/pyarrow/benchmark.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/benchmark.py` & `pyarrow-9.0.0/pyarrow/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/builder.pxi` & `pyarrow-9.0.0/pyarrow/builder.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/cffi.py` & `pyarrow-9.0.0/pyarrow/cffi.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/compat.pxi` & `pyarrow-9.0.0/pyarrow/compat.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/compat.py` & `pyarrow-9.0.0/pyarrow/tests/test_deprecations.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,13 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-# flake8: noqa
-
-import pyarrow.util as util
-import warnings
-
-
-warnings.warn("pyarrow.compat has been deprecated and will be removed in a "
-              "future release", FutureWarning)
+# Check that various deprecation warnings are raised
 
+# flake8: noqa
 
-guid = util._deprecate_api("compat.guid", "util.guid",
-                           util.guid, "1.0.0")
+import pyarrow as pa
+import pytest
```

### Comparing `pyarrow-8.0.0/pyarrow/compute.py` & `pyarrow-9.0.0/pyarrow/compute.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     VectorFunction,
     VectorKernel,
     # Option classes
     ArraySortOptions,
     AssumeTimezoneOptions,
     CastOptions,
     CountOptions,
+    CumulativeSumOptions,
     DayOfWeekOptions,
     DictionaryEncodeOptions,
     ElementWiseAggregateOptions,
     ExtractRegexOptions,
     FilterOptions,
     IndexOptions,
     JoinOptions,
@@ -45,14 +46,15 @@
     MatchSubstringOptions,
     ModeOptions,
     NullOptions,
     PadOptions,
     PartitionNthOptions,
     QuantileOptions,
     RandomOptions,
+    RankOptions,
     ReplaceSliceOptions,
     ReplaceSubstringOptions,
     RoundOptions,
     RoundTemporalOptions,
     RoundToMultipleOptions,
     ScalarAggregateOptions,
     SelectKOptions,
@@ -72,14 +74,17 @@
     WeekOptions,
     # Functions
     call_function,
     function_registry,
     get_function,
     list_functions,
     _group_by,
+    # Udf
+    register_scalar_function,
+    ScalarUdfContext,
     # Expressions
     Expression,
 )
 
 from collections import namedtuple
 import inspect
 from textwrap import dedent
@@ -314,69 +319,77 @@
         assert name not in g, name
         g[cpp_name] = g[name] = _wrap_function(name, func)
 
 
 _make_global_functions()
 
 
-def cast(arr, target_type, safe=True):
+def cast(arr, target_type=None, safe=None, options=None):
     """
     Cast array values to another data type. Can also be invoked as an array
     instance method.
 
     Parameters
     ----------
     arr : Array-like
     target_type : DataType or str
         Type to cast to
     safe : bool, default True
         Check for overflows or other unsafe conversions
+    options : CastOptions, default None
+        Additional checks pass by CastOptions
 
     Examples
     --------
     >>> from datetime import datetime
     >>> import pyarrow as pa
     >>> arr = pa.array([datetime(2010, 1, 1), datetime(2015, 1, 1)])
     >>> arr.type
     TimestampType(timestamp[us])
 
     You can use ``pyarrow.DataType`` objects to specify the target type:
 
     >>> cast(arr, pa.timestamp('ms'))
-    <pyarrow.lib.TimestampArray object at 0x7fe93c0f6910>
+    <pyarrow.lib.TimestampArray object at ...>
     [
       2010-01-01 00:00:00.000,
       2015-01-01 00:00:00.000
     ]
 
     >>> cast(arr, pa.timestamp('ms')).type
     TimestampType(timestamp[ms])
 
     Alternatively, it is also supported to use the string aliases for these
     types:
 
     >>> arr.cast('timestamp[ms]')
-    <pyarrow.lib.TimestampArray object at 0x10420eb88>
+    <pyarrow.lib.TimestampArray object at ...>
     [
-      1262304000000,
-      1420070400000
+      2010-01-01 00:00:00.000,
+      2015-01-01 00:00:00.000
     ]
     >>> arr.cast('timestamp[ms]').type
     TimestampType(timestamp[ms])
 
     Returns
     -------
     casted : Array
     """
-    if target_type is None:
-        raise ValueError("Cast target type must not be None")
-    if safe:
-        options = CastOptions.safe(target_type)
-    else:
-        options = CastOptions.unsafe(target_type)
+    safe_vars_passed = (safe is not None) or (target_type is not None)
+
+    if safe_vars_passed and (options is not None):
+        raise ValueError("Must either pass values for 'target_type' and 'safe'"
+                         " or pass a value for 'options'")
+
+    if options is None:
+        target_type = pa.types.lib.ensure_type(target_type)
+        if safe is False:
+            options = CastOptions.unsafe(target_type)
+        else:
+            options = CastOptions.safe(target_type)
     return call_function("cast", [arr], options)
 
 
 def index(data, value, start=None, end=None, *, memory_pool=None):
     """
     Find the index of the first occurrence of a given value.
 
@@ -441,15 +454,15 @@
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> arr = pa.array(["a", "b", "c", None, "e", "f"])
     >>> indices = pa.array([0, None, 4, 3])
     >>> arr.take(indices)
-    <pyarrow.lib.StringArray object at 0x7ffa4fc7d368>
+    <pyarrow.lib.StringArray object at ...>
     [
       "a",
       null,
       "e",
       null
     ]
     """
@@ -479,15 +492,15 @@
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> arr = pa.array([1, 2, None, 3], type=pa.int8())
     >>> fill_value = pa.scalar(5, type=pa.int8())
     >>> arr.fill_null(fill_value)
-    pyarrow.lib.Int8Array object at 0x7f95437f01a0>
+    <pyarrow.lib.Int8Array object at ...>
     [
       1,
       2,
       5,
       3
     ]
     """
@@ -524,15 +537,15 @@
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> import pyarrow.compute as pc
     >>> arr = pa.array(["a", "b", "c", None, "e", "f"])
     >>> pc.top_k_unstable(arr, k=3)
-    <pyarrow.lib.UInt64Array object at 0x7fdcb19d7f30>
+    <pyarrow.lib.UInt64Array object at ...>
     [
       5,
       4,
       2
     ]
     """
     if sort_keys is None:
@@ -570,15 +583,15 @@
 
     Examples
     --------
     >>> import pyarrow as pa
     >>> import pyarrow.compute as pc
     >>> arr = pa.array(["a", "b", "c", None, "e", "f"])
     >>> pc.bottom_k_unstable(arr, k=3)
-    <pyarrow.lib.UInt64Array object at 0x7fdcb19d7fa0>
+    <pyarrow.lib.UInt64Array object at ...>
     [
       0,
       1,
       2
     ]
     """
     if sort_keys is None:
@@ -587,14 +600,40 @@
         sort_keys.append(("dummy", "ascending"))
     else:
         sort_keys = map(lambda key_name: (key_name, "ascending"), sort_keys)
     options = SelectKOptions(k, sort_keys)
     return call_function("select_k_unstable", [values], options, memory_pool)
 
 
+def random(n, *, initializer='system', options=None, memory_pool=None):
+    """
+    Generate numbers in the range [0, 1).
+
+    Generated values are uniformly-distributed, double-precision
+    in range [0, 1). Algorithm and seed can be changed via RandomOptions.
+
+    Parameters
+    ----------
+    n : int
+        Number of values to generate, must be greater than or equal to 0
+    initializer : int or str
+        How to initialize the underlying random generator.
+        If an integer is given, it is used as a seed.
+        If "system" is given, the random generator is initialized with
+        a system-specific source of (hopefully true) randomness.
+        Other values are invalid.
+    options : pyarrow.compute.RandomOptions, optional
+        Alternative way of passing options.
+    memory_pool : pyarrow.MemoryPool, optional
+        If not passed, will allocate memory from the default memory pool.
+    """
+    options = RandomOptions(initializer=initializer)
+    return call_function("random", [], options, memory_pool, length=n)
+
+
 def field(*name_or_index):
     """Reference a column of the dataset.
 
     Stores only the field's name. Type and other information is known only when
     the expression is bound to a dataset having an explicit scheme.
 
     Nested references are allowed by passing multiple names or a tuple of
```

### Comparing `pyarrow-8.0.0/pyarrow/config.pxi` & `pyarrow-9.0.0/pyarrow/config.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/csv.py` & `pyarrow-9.0.0/pyarrow/csv.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/cuda.py` & `pyarrow-9.0.0/pyarrow/cuda.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/dataset.py` & `pyarrow-9.0.0/pyarrow/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     InMemoryDataset,
     Partitioning,
     PartitioningFactory,
     Scanner,
     TaggedRecordBatch,
     UnionDataset,
     UnionDatasetFactory,
+    WrittenFile,
     _get_partition_keys,
     _filesystemdataset_write,
 )
 # keep Expression functionality exposed here for backwards compatibility
 from pyarrow.compute import Expression, scalar, field  # noqa
 
 
@@ -151,55 +152,57 @@
     Partitioning or PartitioningFactory
 
     Examples
     --------
 
     Specify the Schema for paths like "/2009/June":
 
-    >>> partitioning(pa.schema([("year", pa.int16()), ("month", pa.string())]))
+    >>> import pyarrow as pa
+    >>> import pyarrow.dataset as ds
+    >>> part = ds.partitioning(pa.schema([("year", pa.int16()),
+    ...                                   ("month", pa.string())]))
 
     or let the types be inferred by only specifying the field names:
 
-    >>> partitioning(field_names=["year", "month"])
+    >>> part =  ds.partitioning(field_names=["year", "month"])
 
     For paths like "/2009/June", the year will be inferred as int32 while month
     will be inferred as string.
 
     Specify a Schema with dictionary encoding, providing dictionary values:
 
-    >>> partitioning(
+    >>> part = ds.partitioning(
     ...     pa.schema([
     ...         ("year", pa.int16()),
     ...         ("month", pa.dictionary(pa.int8(), pa.string()))
     ...     ]),
     ...     dictionaries={
     ...         "month": pa.array(["January", "February", "March"]),
     ...     })
 
     Alternatively, specify a Schema with dictionary encoding, but have Arrow
     infer the dictionary values:
 
-    >>> partitioning(
+    >>> part = ds.partitioning(
     ...     pa.schema([
     ...         ("year", pa.int16()),
     ...         ("month", pa.dictionary(pa.int8(), pa.string()))
     ...     ]),
     ...     dictionaries="infer")
 
     Create a Hive scheme for a path like "/year=2009/month=11":
 
-    >>> partitioning(
+    >>> part = ds.partitioning(
     ...     pa.schema([("year", pa.int16()), ("month", pa.int8())]),
     ...     flavor="hive")
 
     A Hive scheme can also be discovered from the directory structure (and
     types will be inferred):
 
-    >>> partitioning(flavor="hive")
-
+    >>> part = ds.partitioning(flavor="hive")
     """
     if flavor is None:
         # default flavor
         if schema is not None:
             if field_names is not None:
                 raise ValueError(
                     "Cannot specify both 'schema' and 'field_names'")
@@ -214,15 +217,14 @@
                     "Expected list of field names, got {}".format(
                         type(field_names)))
         else:
             raise ValueError(
                 "For the default directory flavor, need to specify "
                 "a Schema or a list of field names")
     if flavor == "filename":
-        # default flavor
         if schema is not None:
             if field_names is not None:
                 raise ValueError(
                     "Cannot specify both 'schema' and 'field_names'")
             if dictionaries == 'infer':
                 return FilenamePartitioning.discover(schema=schema)
             return FilenamePartitioning(schema, dictionaries)
@@ -618,70 +620,123 @@
     -------
     dataset : Dataset
         Either a FileSystemDataset or a UnionDataset depending on the source
         parameter.
 
     Examples
     --------
+    Creating an example Table:
+
+    >>> import pyarrow as pa
+    >>> import pyarrow.parquet as pq
+    >>> table = pa.table({'year': [2020, 2022, 2021, 2022, 2019, 2021],
+    ...                   'n_legs': [2, 2, 4, 4, 5, 100],
+    ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
+    ...                              "Brittle stars", "Centipede"]})
+    >>> pq.write_table(table, "file.parquet")
+
     Opening a single file:
 
-    >>> dataset("path/to/file.parquet", format="parquet")
+    >>> import pyarrow.dataset as ds
+    >>> dataset = ds.dataset("file.parquet", format="parquet")
+    >>> dataset.to_table()
+    pyarrow.Table
+    year: int64
+    n_legs: int64
+    animal: string
+    ----
+    year: [[2020,2022,2021,2022,2019,2021]]
+    n_legs: [[2,2,4,4,5,100]]
+    animal: [["Flamingo","Parrot","Dog","Horse","Brittle stars","Centipede"]]
 
     Opening a single file with an explicit schema:
 
-    >>> dataset("path/to/file.parquet", schema=myschema, format="parquet")
+    >>> myschema = pa.schema([
+    ...     ('n_legs', pa.int64()),
+    ...     ('animal', pa.string())])
+    >>> dataset = ds.dataset("file.parquet", schema=myschema, format="parquet")
+    >>> dataset.to_table()
+    pyarrow.Table
+    n_legs: int64
+    animal: string
+    ----
+    n_legs: [[2,2,4,4,5,100]]
+    animal: [["Flamingo","Parrot","Dog","Horse","Brittle stars","Centipede"]]
 
     Opening a dataset for a single directory:
 
-    >>> dataset("path/to/nyc-taxi/", format="parquet")
-    >>> dataset("s3://mybucket/nyc-taxi/", format="parquet")
+    >>> ds.write_dataset(table, "partitioned_dataset", format="parquet",
+    ...                  partitioning=['year'])
+    >>> dataset = ds.dataset("partitioned_dataset", format="parquet")
+    >>> dataset.to_table()
+    pyarrow.Table
+    n_legs: int64
+    animal: string
+    ----
+    n_legs: [[5],[2],[4,100],[2,4]]
+    animal: [["Brittle stars"],["Flamingo"],...["Parrot","Horse"]]
+
+    For a single directory from a S3 bucket:
+
+    >>> ds.dataset("s3://mybucket/nyc-taxi/",
+    ...            format="parquet") # doctest: +SKIP
 
     Opening a dataset from a list of relatives local paths:
 
-    >>> dataset([
-    ...     "part0/data.parquet",
-    ...     "part1/data.parquet",
-    ...     "part3/data.parquet",
+    >>> dataset = ds.dataset([
+    ...     "partitioned_dataset/2019/part-0.parquet",
+    ...     "partitioned_dataset/2020/part-0.parquet",
+    ...     "partitioned_dataset/2021/part-0.parquet",
     ... ], format='parquet')
+    >>> dataset.to_table()
+    pyarrow.Table
+    n_legs: int64
+    animal: string
+    ----
+    n_legs: [[5],[2],[4,100]]
+    animal: [["Brittle stars"],["Flamingo"],["Dog","Centipede"]]
 
     With filesystem provided:
 
     >>> paths = [
     ...     'part0/data.parquet',
     ...     'part1/data.parquet',
     ...     'part3/data.parquet',
     ... ]
-    >>> dataset(paths, filesystem='file:///directory/prefix, format='parquet')
+    >>> ds.dataset(paths, filesystem='file:///directory/prefix,
+    ...            format='parquet') # doctest: +SKIP
 
     Which is equivalent with:
 
-    >>> fs = SubTreeFileSystem("/directory/prefix", LocalFileSystem())
-    >>> dataset(paths, filesystem=fs, format='parquet')
+    >>> fs = SubTreeFileSystem("/directory/prefix",
+    ...                        LocalFileSystem()) # doctest: +SKIP
+    >>> ds.dataset(paths, filesystem=fs, format='parquet') # doctest: +SKIP
 
     With a remote filesystem URI:
 
     >>> paths = [
     ...     'nested/directory/part0/data.parquet',
     ...     'nested/directory/part1/data.parquet',
     ...     'nested/directory/part3/data.parquet',
     ... ]
-    >>> dataset(paths, filesystem='s3://bucket/', format='parquet')
+    >>> ds.dataset(paths, filesystem='s3://bucket/',
+    ...            format='parquet') # doctest: +SKIP
 
     Similarly to the local example, the directory prefix may be included in the
     filesystem URI:
 
-    >>> dataset(paths, filesystem='s3://bucket/nested/directory',
-    ...         format='parquet')
+    >>> ds.dataset(paths, filesystem='s3://bucket/nested/directory',
+    ...         format='parquet') # doctest: +SKIP
 
     Construction of a nested dataset:
 
-    >>> dataset([
+    >>> ds.dataset([
     ...     dataset("s3://old-taxi-data", format="parquet"),
     ...     dataset("local/path/to/data", format="ipc")
-    ... ])
+    ... ]) # doctest: +SKIP
     """
     # collect the keyword arguments for later reuse
     kwargs = dict(
         schema=schema,
         filesystem=filesystem,
         partitioning=partitioning,
         format=format,
@@ -743,15 +798,15 @@
             "partitioning must be a Partitioning object or "
             "a list of column names"
         )
 
     return part
 
 
-def write_dataset(data, base_dir, basename_template=None, format=None,
+def write_dataset(data, base_dir, *, basename_template=None, format=None,
                   partitioning=None, partitioning_flavor=None, schema=None,
                   filesystem=None, file_options=None, use_threads=True,
                   max_partitions=None, max_open_files=None,
                   max_rows_per_file=None, min_rows_per_group=None,
                   max_rows_per_group=None, file_visitor=None,
                   existing_data_behavior='error', create_dir=True):
     """
```

### Comparing `pyarrow-8.0.0/pyarrow/error.pxi` & `pyarrow-9.0.0/pyarrow/error.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/feather.py` & `pyarrow-9.0.0/pyarrow/feather.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,54 +200,56 @@
             try:
                 os.remove(dest)
             except os.error:
                 pass
         raise
 
 
-def read_feather(source, columns=None, use_threads=True, memory_map=True):
+def read_feather(source, columns=None, use_threads=True, memory_map=False):
     """
     Read a pandas.DataFrame from Feather format. To read as pyarrow.Table use
     feather.read_table.
 
     Parameters
     ----------
     source : str file path, or file-like object
+        You can use MemoryMappedFile as source, for explicitly use memory map.
     columns : sequence, optional
         Only read a specific set of columns. If not provided, all columns are
         read.
     use_threads : bool, default True
         Whether to parallelize reading using multiple threads. If false the
         restriction is used in the conversion to Pandas as well as in the
         reading from Feather format.
-    memory_map : boolean, default True
-        Use memory mapping when opening file on disk
+    memory_map : boolean, default False
+        Use memory mapping when opening file on disk, when source is a str.
 
     Returns
     -------
     df : pandas.DataFrame
     """
     _check_pandas_version()
     return (read_table(
         source, columns=columns, memory_map=memory_map,
         use_threads=use_threads).to_pandas(use_threads=use_threads))
 
 
-def read_table(source, columns=None, memory_map=True, use_threads=True):
+def read_table(source, columns=None, memory_map=False, use_threads=True):
     """
     Read a pyarrow.Table from Feather format
 
     Parameters
     ----------
     source : str file path, or file-like object
+        You can use MemoryMappedFile as source, for explicitly use memory map.
     columns : sequence, optional
         Only read a specific set of columns. If not provided, all columns are
         read.
-    memory_map : boolean, default True
-        Use memory mapping when opening file on disk
+    memory_map : boolean, default False
+        Use memory mapping when opening file on disk, when source is a str
     use_threads : bool, default True
         Whether to parallelize reading using multiple threads.
 
     Returns
     -------
     table : pyarrow.Table
     """
```

### Comparing `pyarrow-8.0.0/pyarrow/filesystem.py` & `pyarrow-9.0.0/pyarrow/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/flight.py` & `pyarrow-9.0.0/pyarrow/flight.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/fs.py` & `pyarrow-9.0.0/pyarrow/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 
 try:
     from pyarrow._hdfs import HadoopFileSystem  # noqa
 except ImportError:
     _not_imported.append("HadoopFileSystem")
 
 try:
+    from pyarrow._gcsfs import GcsFileSystem  # noqa
+except ImportError:
+    _not_imported.append("GcsFileSystem")
+
+try:
     from pyarrow._s3fs import (  # noqa
         S3FileSystem, S3LogLevel, initialize_s3, finalize_s3,
         resolve_s3_region)
 except ImportError:
     _not_imported.append("S3FileSystem")
 else:
     initialize_s3()
@@ -218,23 +223,36 @@
         destination file. A larger chunk_size will use more memory while
         copying but may help accommodate high latency FileSystems.
     use_threads : bool, default True
         Whether to use multiple threads to accelerate copying.
 
     Examples
     --------
-    Copy an S3 bucket's files to a local directory:
+    Inspect an S3 bucket's files:
+
+    >>> s3, path = fs.FileSystem.from_uri(
+    ...            "s3://registry.opendata.aws/roda/ndjson/")
+    >>> selector = fs.FileSelector(path)
+    >>> s3.get_file_info(selector)
+    [<FileInfo for 'registry.opendata.aws/roda/ndjson/index.ndjson':...]
+
+    Copy one file from S3 bucket to a local directory:
 
-    >>> copy_files("s3://your-bucket-name", "local-directory")
+    >>> fs.copy_files("s3://registry.opendata.aws/roda/ndjson/index.ndjson",
+    ...               "file:///{}/index_copy.ndjson".format(local_path))
 
-    Using a FileSystem object:
+    >>> fs.LocalFileSystem().get_file_info(str(local_path)+
+    ...                                    '/index_copy.ndjson')
+    <FileInfo for '.../index_copy.ndjson': type=FileType.File, size=...>
 
-    >>> copy_files("your-bucket-name", "local-directory",
-    ...            source_filesystem=S3FileSystem(...))
+    Copy file using a FileSystem object:
 
+    >>> fs.copy_files("registry.opendata.aws/roda/ndjson/index.ndjson",
+    ...               "file:///{}/index_copy.ndjson".format(local_path),
+    ...               source_filesystem=fs.S3FileSystem())
     """
     source_fs, source_path = _resolve_filesystem_and_path(
         source, source_filesystem
     )
     destination_fs, destination_path = _resolve_filesystem_and_path(
         destination, destination_filesystem
     )
@@ -259,15 +277,15 @@
 
     Parameters
     ----------
     fs : FSSpec-compliant filesystem instance.
 
     Examples
     --------
-    >>> PyFileSystem(FSSpecHandler(fsspec_fs))
+    >>> PyFileSystem(FSSpecHandler(fsspec_fs)) # doctest: +SKIP
     """
 
     def __init__(self, fs):
         self.fs = fs
 
     def __eq__(self, other):
         if isinstance(other, FSSpecHandler):
```

### Comparing `pyarrow-8.0.0/pyarrow/gandiva.pyx` & `pyarrow-9.0.0/pyarrow/gandiva.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -288,140 +288,147 @@
         elif type.id == _Type_BINARY:
             r = TreeExprBuilder_MakeBinaryLiteral(value)
         else:
             raise TypeError("Didn't recognize dtype " + str(dtype))
 
         return Node.create(r)
 
-    def make_expression(self, Node root_node, Field return_field):
+    def make_expression(self, Node root_node not None,
+                        Field return_field not None):
         cdef shared_ptr[CGandivaExpression] r = TreeExprBuilder_MakeExpression(
             root_node.node, return_field.sp_field)
         cdef Expression expression = Expression()
         expression.init(r)
         return expression
 
     def make_function(self, name, children, DataType return_type):
         cdef c_vector[shared_ptr[CNode]] c_children
         cdef Node child
         for child in children:
+            if child is None:
+                raise TypeError("Child nodes must not be None")
             c_children.push_back(child.node)
         cdef shared_ptr[CNode] r = TreeExprBuilder_MakeFunction(
             name.encode(), c_children, return_type.sp_type)
         return Node.create(r)
 
-    def make_field(self, Field field):
+    def make_field(self, Field field not None):
         cdef shared_ptr[CNode] r = TreeExprBuilder_MakeField(field.sp_field)
         return Node.create(r)
 
-    def make_if(self, Node condition, Node this_node,
-                Node else_node, DataType return_type):
+    def make_if(self, Node condition not None, Node this_node not None,
+                Node else_node not None, DataType return_type not None):
         cdef shared_ptr[CNode] r = TreeExprBuilder_MakeIf(
             condition.node, this_node.node, else_node.node,
             return_type.sp_type)
         return Node.create(r)
 
     def make_and(self, children):
         cdef c_vector[shared_ptr[CNode]] c_children
         cdef Node child
         for child in children:
+            if child is None:
+                raise TypeError("Child nodes must not be None")
             c_children.push_back(child.node)
         cdef shared_ptr[CNode] r = TreeExprBuilder_MakeAnd(c_children)
         return Node.create(r)
 
     def make_or(self, children):
         cdef c_vector[shared_ptr[CNode]] c_children
         cdef Node child
         for child in children:
+            if child is None:
+                raise TypeError("Child nodes must not be None")
             c_children.push_back(child.node)
         cdef shared_ptr[CNode] r = TreeExprBuilder_MakeOr(c_children)
         return Node.create(r)
 
-    def _make_in_expression_int32(self, Node node, values):
+    def _make_in_expression_int32(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int32_t] c_values
         cdef int32_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionInt32(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_int64(self, Node node, values):
+    def _make_in_expression_int64(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int64_t] c_values
         cdef int64_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionInt64(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_time32(self, Node node, values):
+    def _make_in_expression_time32(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int32_t] c_values
         cdef int32_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionTime32(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_time64(self, Node node, values):
+    def _make_in_expression_time64(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int64_t] c_values
         cdef int64_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionTime64(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_date32(self, Node node, values):
+    def _make_in_expression_date32(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int32_t] c_values
         cdef int32_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionDate32(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_date64(self, Node node, values):
+    def _make_in_expression_date64(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int64_t] c_values
         cdef int64_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionDate64(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_timestamp(self, Node node, values):
+    def _make_in_expression_timestamp(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[int64_t] c_values
         cdef int64_t v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionTimeStamp(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_binary(self, Node node, values):
+    def _make_in_expression_binary(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[c_string] c_values
         cdef c_string v
         for v in values:
             c_values.insert(v)
         r = TreeExprBuilder_MakeInExpressionString(node.node, c_values)
         return Node.create(r)
 
-    def _make_in_expression_string(self, Node node, values):
+    def _make_in_expression_string(self, Node node not None, values):
         cdef shared_ptr[CNode] r
         cdef c_unordered_set[c_string] c_values
         cdef c_string _v
         for v in values:
             _v = v.encode('UTF-8')
             c_values.insert(_v)
         r = TreeExprBuilder_MakeInExpressionString(node.node, c_values)
         return Node.create(r)
 
-    def make_in_expression(self, Node node, values, dtype):
+    def make_in_expression(self, Node node not None, values, dtype):
         cdef DataType type = ensure_type(dtype)
 
         if type.id == _Type_INT32:
             return self._make_in_expression_int32(node, values)
         elif type.id == _Type_INT64:
             return self._make_in_expression_int64(node, values)
         elif type.id == _Type_TIME32:
@@ -437,15 +444,15 @@
         elif type.id == _Type_BINARY:
             return self._make_in_expression_binary(node, values)
         elif type.id == _Type_STRING:
             return self._make_in_expression_string(node, values)
         else:
             raise TypeError("Data type " + str(dtype) + " not supported.")
 
-    def make_condition(self, Node condition):
+    def make_condition(self, Node condition not None):
         cdef shared_ptr[CCondition] r = TreeExprBuilder_MakeCondition(
             condition.node)
         return Condition.create(r)
 
 
 cpdef make_projector(Schema schema, children, MemoryPool pool,
                      str selection_mode="NONE"):
@@ -472,14 +479,16 @@
     """
     cdef:
         Expression child
         c_vector[shared_ptr[CGandivaExpression]] c_children
         shared_ptr[CProjector] result
 
     for child in children:
+        if child is None:
+            raise TypeError("Expressions must not be None")
         c_children.push_back(child.expression)
 
     check_status(
         Projector_Make(schema.sp_schema, c_children,
                        _ensure_selection_mode(selection_mode),
                        CConfigurationBuilder.DefaultConfiguration(),
                        &result))
@@ -501,14 +510,16 @@
         Filter condition.
 
     Returns
     -------
     Filter instance
     """
     cdef shared_ptr[CFilter] result
+    if condition is None:
+        raise TypeError("Condition must not be None")
     check_status(
         Filter_Make(schema.sp_schema, condition.condition, &result))
     return Filter.create(result)
 
 
 cdef class FunctionSignature(_Weakrefable):
     """
```

### Comparing `pyarrow-8.0.0/pyarrow/hdfs.py` & `pyarrow-9.0.0/pyarrow/hdfs.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/common.pxd` & `pyarrow-9.0.0/pyarrow/includes/common.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,21 @@
         c_string ToString(int32_t scale) const
 
 
 cdef extern from "arrow/util/decimal.h" namespace "arrow" nogil:
     cdef cppclass CDecimal256" arrow::Decimal256":
         c_string ToString(int32_t scale) const
 
+cdef extern from "arrow/util/optional.h" namespace "arrow::util" nogil:
+    cdef cppclass c_optional"arrow::util::optional"[T]:
+        c_bool has_value()
+        T value()
+        c_optional(T&)
+        c_optional& operator=[U](U&)
+
 
 cdef extern from "arrow/config.h" namespace "arrow" nogil:
     cdef cppclass CBuildInfo" arrow::BuildInfo":
         int version
         int version_major
         int version_minor
         int version_patch
@@ -858,14 +865,15 @@
             const shared_ptr[CKeyValueMetadata]& metadata)
 
         shared_ptr[CTable] Slice(int64_t offset)
         shared_ptr[CTable] Slice(int64_t offset, int64_t length)
 
     cdef cppclass CRecordBatchReader" arrow::RecordBatchReader":
         shared_ptr[CSchema] schema()
+        CStatus Close()
         CStatus ReadNext(shared_ptr[CRecordBatch]* batch)
         CResult[shared_ptr[CTable]] ToTable()
 
     cdef cppclass TableBatchReader(CRecordBatchReader):
         TableBatchReader(const CTable& table)
         TableBatchReader(shared_ptr[CTable] table)
         void set_chunksize(int64_t chunksize)
@@ -1071,18 +1079,26 @@
         CDictionaryScalar(CDictionaryScalarIndexAndDictionary value,
                           shared_ptr[CDataType], c_bool is_valid)
         CDictionaryScalarIndexAndDictionary value
 
         CResult[shared_ptr[CScalar]] GetEncodedValue()
 
     cdef cppclass CUnionScalar" arrow::UnionScalar"(CScalar):
-        shared_ptr[CScalar] value
         int8_t type_code
 
+    cdef cppclass CDenseUnionScalar" arrow::DenseUnionScalar"(CUnionScalar):
+        shared_ptr[CScalar] value
+
+    cdef cppclass CSparseUnionScalar" arrow::SparseUnionScalar"(CUnionScalar):
+        vector[shared_ptr[CScalar]] value
+        int child_id
+
     cdef cppclass CExtensionScalar" arrow::ExtensionScalar"(CScalar):
+        CExtensionScalar(shared_ptr[CScalar] storage,
+                         shared_ptr[CDataType], c_bool is_valid)
         shared_ptr[CScalar] value
 
     shared_ptr[CScalar] MakeScalar[Value](Value value)
 
     cdef cppclass CConcatenateTablesOptions" arrow::ConcatenateTablesOptions":
         c_bool unify_schemas
         CField.CMergeOptions field_merge_options
@@ -1100,14 +1116,16 @@
         CResult[shared_ptr[CChunkedArray]] UnifyChunkedArray(
             shared_ptr[CChunkedArray] array, CMemoryPool* pool)
 
         @staticmethod
         CResult[shared_ptr[CTable]] UnifyTable(
             const CTable& table, CMemoryPool* pool)
 
+    shared_ptr[CScalar] MakeNullScalar(shared_ptr[CDataType] type)
+
 
 cdef extern from "arrow/builder.h" namespace "arrow" nogil:
 
     cdef cppclass CArrayBuilder" arrow::ArrayBuilder":
         CArrayBuilder(shared_ptr[CDataType], CMemoryPool* pool)
 
         int64_t length()
@@ -1834,14 +1852,18 @@
             " arrow::compute::HashAggregateKernel"(CKernel):
         pass
 
     cdef cppclass CArity" arrow::compute::Arity":
         int num_args
         c_bool is_varargs
 
+        CArity()
+
+        CArity(int num_args, c_bool is_varargs)
+
     cdef enum FunctionKind" arrow::compute::Function::Kind":
         FunctionKind_SCALAR" arrow::compute::Function::SCALAR"
         FunctionKind_VECTOR" arrow::compute::Function::VECTOR"
         FunctionKind_SCALAR_AGGREGATE \
             " arrow::compute::Function::SCALAR_AGGREGATE"
         FunctionKind_HASH_AGGREGATE \
             " arrow::compute::Function::HASH_AGGREGATE"
@@ -1875,14 +1897,17 @@
         FunctionKind kind() const
         const CArity& arity() const
         const CFunctionDoc& doc() const
         int num_kernels() const
         CResult[CDatum] Execute(const vector[CDatum]& args,
                                 const CFunctionOptions* options,
                                 CExecContext* ctx) const
+        CResult[CDatum] Execute(const CExecBatch& args,
+                                const CFunctionOptions* options,
+                                CExecContext* ctx) const
 
     cdef cppclass CScalarFunction" arrow::compute::ScalarFunction"(CFunction):
         vector[const CScalarKernel*] kernels() const
 
     cdef cppclass CVectorFunction" arrow::compute::VectorFunction"(CFunction):
         vector[const CVectorKernel*] kernels() const
 
@@ -1963,18 +1988,22 @@
             "arrow::compute::CalendarUnit::QUARTER"
         CCalendarUnit_YEAR \
             "arrow::compute::CalendarUnit::YEAR"
 
     cdef cppclass CRoundTemporalOptions \
             "arrow::compute::RoundTemporalOptions"(CFunctionOptions):
         CRoundTemporalOptions(int multiple, CCalendarUnit unit,
-                              c_bool week_starts_monday)
+                              c_bool week_starts_monday,
+                              c_bool ceil_is_strictly_greater,
+                              c_bool calendar_based_origin)
         int multiple
         CCalendarUnit unit
         c_bool week_starts_monday
+        c_bool ceil_is_strictly_greater
+        c_bool calendar_based_origin
 
     cdef cppclass CRoundToMultipleOptions \
             "arrow::compute::RoundToMultipleOptions"(CFunctionOptions):
         CRoundToMultipleOptions(shared_ptr[CScalar] multiple, CRoundMode round_mode)
         shared_ptr[CScalar] multiple
         CRoundMode round_mode
 
@@ -2237,14 +2266,20 @@
 
     cdef cppclass CPartitionNthOptions \
             "arrow::compute::PartitionNthOptions"(CFunctionOptions):
         CPartitionNthOptions(int64_t pivot, CNullPlacement)
         int64_t pivot
         CNullPlacement null_placement
 
+    cdef cppclass CCumulativeSumOptions \
+            "arrow::compute::CumulativeSumOptions"(CFunctionOptions):
+        CCumulativeSumOptions(shared_ptr[CScalar] start, c_bool skip_nulls)
+        shared_ptr[CScalar] start
+        c_bool skip_nulls
+
     cdef cppclass CArraySortOptions \
             "arrow::compute::ArraySortOptions"(CFunctionOptions):
         CArraySortOptions(CSortOrder, CNullPlacement)
         CSortOrder order
         CNullPlacement null_placement
 
     cdef cppclass CSortKey" arrow::compute::SortKey":
@@ -2311,18 +2346,33 @@
         c_bool skip_nulls
 
     cdef cppclass CRandomOptions \
             "arrow::compute::RandomOptions"(CFunctionOptions):
         CRandomOptions(CRandomOptions)
 
         @staticmethod
-        CRandomOptions FromSystemRandom(int64_t length)
+        CRandomOptions FromSystemRandom()
 
         @staticmethod
-        CRandomOptions FromSeed(int64_t length, uint64_t seed)
+        CRandomOptions FromSeed(uint64_t seed)
+
+    cdef enum CRankOptionsTiebreaker \
+            "arrow::compute::RankOptions::Tiebreaker":
+        CRankOptionsTiebreaker_Min "arrow::compute::RankOptions::Min"
+        CRankOptionsTiebreaker_Max "arrow::compute::RankOptions::Max"
+        CRankOptionsTiebreaker_First "arrow::compute::RankOptions::First"
+        CRankOptionsTiebreaker_Dense "arrow::compute::RankOptions::Dense"
+
+    cdef cppclass CRankOptions \
+            "arrow::compute::RankOptions"(CFunctionOptions):
+        CRankOptions(vector[CSortKey] sort_keys, CNullPlacement,
+                     CRankOptionsTiebreaker tiebreaker)
+        vector[CSortKey] sort_keys
+        CNullPlacement null_placement
+        CRankOptionsTiebreaker tiebreaker
 
     cdef enum DatumType" arrow::Datum::type":
         DatumType_NONE" arrow::Datum::NONE"
         DatumType_SCALAR" arrow::Datum::SCALAR"
         DatumType_ARRAY" arrow::Datum::ARRAY"
         DatumType_CHUNKED_ARRAY" arrow::Datum::CHUNKED_ARRAY"
         DatumType_RECORD_BATCH" arrow::Datum::RECORD_BATCH"
@@ -2342,14 +2392,15 @@
 
         const shared_ptr[CArrayData]& array() const
         const shared_ptr[CChunkedArray]& chunked_array() const
         const shared_ptr[CRecordBatch]& record_batch() const
         const shared_ptr[CTable]& table() const
         const shared_ptr[CScalar]& scalar() const
 
+    cdef c_string ToString(DatumType kind)
 
 cdef extern from * namespace "arrow::compute":
     # inlined from compute/function_internal.h to avoid exposing
     # implementation details
     """
     #include "arrow/compute/function.h"
     namespace arrow {
@@ -2362,19 +2413,19 @@
     } //  namespace arrow
     """
     CResult[unique_ptr[CFunctionOptions]] DeserializeFunctionOptions \
         " arrow::compute::internal::DeserializeFunctionOptions"(
             const CBuffer& buffer)
 
 
-cdef extern from "arrow/compute/api_aggregate.h" namespace \
+cdef extern from "arrow/compute/exec/aggregate.h" namespace \
         "arrow::compute::internal" nogil:
-    cdef cppclass CAggregate "arrow::compute::internal::Aggregate":
+    cdef cppclass CAggregate "arrow::compute::Aggregate":
         c_string function
-        const CFunctionOptions* options
+        shared_ptr[CFunctionOptions] options
 
     CResult[CDatum] GroupBy(const vector[CDatum]& arguments,
                             const vector[CDatum]& keys,
                             const vector[CAggregate]& aggregates)
 
 
 cdef extern from * namespace "arrow::compute":
@@ -2449,14 +2500,17 @@
 
     cdef cppclass CTableSourceNodeOptions "arrow::compute::TableSourceNodeOptions"(CExecNodeOptions):
         CTableSourceNodeOptions(shared_ptr[CTable] table, int64_t max_batch_size)
 
     cdef cppclass CSinkNodeOptions "arrow::compute::SinkNodeOptions"(CExecNodeOptions):
         pass
 
+    cdef cppclass CFilterNodeOptions "arrow::compute::FilterNodeOptions"(CExecNodeOptions):
+        CFilterNodeOptions(CExpression, c_bool async_mode)
+
     cdef cppclass CProjectNodeOptions "arrow::compute::ProjectNodeOptions"(CExecNodeOptions):
         CProjectNodeOptions(vector[CExpression] expressions)
         CProjectNodeOptions(vector[CExpression] expressions,
                             vector[c_string] names)
 
     cdef cppclass CHashJoinNodeOptions "arrow::compute::HashJoinNodeOptions"(CExecNodeOptions):
         CHashJoinNodeOptions(CJoinType, vector[CFieldRef] in_left_keys,
@@ -2507,15 +2561,16 @@
         vector[CExecNode*] sources() const
 
     cdef cppclass CExecNode "arrow::compute::ExecNode":
         const vector[CExecNode*]& inputs() const
         const shared_ptr[CSchema]& output_schema() const
 
     cdef cppclass CExecBatch "arrow::compute::ExecBatch":
-        pass
+        vector[CDatum] values
+        int64_t length
 
     shared_ptr[CRecordBatchReader] MakeGeneratorReader(
         shared_ptr[CSchema] schema,
         CAsyncExecBatchGenerator gen,
         CMemoryPool* memory_pool
     )
     CResult[CExecNode*] MakeExecNode(c_string factory_name, CExecPlan* plan,
@@ -2667,7 +2722,24 @@
     CResult[int64_t] ReferencedBufferSize(const CRecordBatch& record_batch)
     CResult[int64_t] ReferencedBufferSize(const CChunkedArray& chunked_array)
     CResult[int64_t] ReferencedBufferSize(const CTable& table)
     int64_t TotalBufferSize(const CArray& array)
     int64_t TotalBufferSize(const CChunkedArray& array)
     int64_t TotalBufferSize(const CRecordBatch& record_batch)
     int64_t TotalBufferSize(const CTable& table)
+
+ctypedef PyObject* CallbackUdf(object user_function, const CScalarUdfContext& context, object inputs)
+
+cdef extern from "arrow/python/udf.h" namespace "arrow::py":
+    cdef cppclass CScalarUdfContext" arrow::py::ScalarUdfContext":
+        CMemoryPool *pool
+        int64_t batch_length
+
+    cdef cppclass CScalarUdfOptions" arrow::py::ScalarUdfOptions":
+        c_string func_name
+        CArity arity
+        CFunctionDoc func_doc
+        vector[shared_ptr[CDataType]] input_types
+        shared_ptr[CDataType] output_type
+
+    CStatus RegisterScalarFunction(PyObject* function,
+                                   function[CallbackUdf] wrapper, const CScalarUdfOptions& options)
```

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_cuda.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_cuda.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_dataset.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_dataset.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 
     cdef cppclass CFileWriter \
             "arrow::dataset::FileWriter":
         const shared_ptr[CFileFormat]& format() const
         const shared_ptr[CSchema]& schema() const
         const shared_ptr[CFileWriteOptions]& options() const
         const CFileLocator& destination() const
+        CResult[int64_t] GetBytesWritten()
 
     cdef cppclass CFileFormat "arrow::dataset::FileFormat":
         shared_ptr[CFragmentScanOptions] default_fragment_scan_options
         c_string type_name() const
         CResult[shared_ptr[CSchema]] Inspect(const CFileSource&) const
         CResult[shared_ptr[CFileFragment]] MakeFragment(
             CFileSource source,
```

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_dataset_parquet.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_dataset_parquet.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_feather.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_feather.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_flight.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_flight.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_fs.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_fs.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,16 @@
             "arrow::fs::S3CredentialsKind::WebIdentity"
 
     cdef cppclass CS3Options "arrow::fs::S3Options":
         c_string region
         c_string endpoint_override
         c_string scheme
         c_bool background_writes
+        c_bool allow_bucket_creation
+        c_bool allow_bucket_deletion
         shared_ptr[const CKeyValueMetadata] default_metadata
         c_string role_arn
         c_string session_name
         c_string external_id
         int load_frequency
         CS3ProxyOptions proxy_options
         CS3CredentialsKind credentials_kind
@@ -196,14 +198,48 @@
 
     cdef CStatus CInitializeS3 "arrow::fs::InitializeS3"(
         const CS3GlobalOptions& options)
     cdef CStatus CFinalizeS3 "arrow::fs::FinalizeS3"()
 
     cdef CResult[c_string] ResolveS3BucketRegion(const c_string& bucket)
 
+    cdef cppclass CGcsCredentials "arrow::fs::GcsCredentials":
+        c_bool anonymous()
+        CTimePoint expiration()
+        c_string access_token()
+        c_string target_service_account()
+
+    cdef cppclass CGcsOptions "arrow::fs::GcsOptions":
+        CGcsCredentials credentials
+        c_string endpoint_override
+        c_string scheme
+        c_string default_bucket_location
+        c_optional[double] retry_limit_seconds
+        shared_ptr[const CKeyValueMetadata] default_metadata
+        c_bool Equals(const CS3Options& other)
+
+        @staticmethod
+        CGcsOptions Defaults()
+
+        @staticmethod
+        CGcsOptions Anonymous()
+
+        @staticmethod
+        CGcsOptions FromAccessToken(const c_string& access_token,
+                                    CTimePoint expiration)
+
+        @staticmethod
+        CGcsOptions FromImpersonatedServiceAccount(const CGcsCredentials& base_credentials,
+                                                   c_string& target_service_account)
+
+    cdef cppclass CGcsFileSystem "arrow::fs::GcsFileSystem":
+        @staticmethod
+        CResult[shared_ptr[CGcsFileSystem]] Make(const CGcsOptions& options)
+        CGcsOptions options()
+
     cdef cppclass CHdfsOptions "arrow::fs::HdfsOptions":
         HdfsConnectionConfig connection_config
         int32_t buffer_size
         int16_t replication
         int64_t default_block_size
 
         @staticmethod
```

### Comparing `pyarrow-8.0.0/pyarrow/includes/libarrow_python.pxd` & `pyarrow-9.0.0/pyarrow/includes/libarrow_python.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libgandiva.pxd` & `pyarrow-9.0.0/pyarrow/includes/libgandiva.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/includes/libplasma.pxd` & `pyarrow-9.0.0/pyarrow/includes/libplasma.pxd`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/io.pxi` & `pyarrow-9.0.0/pyarrow/io.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,18 @@
     facilities that will make use of it, such as Arrow IPC routines.
 
     Be aware that there are subtle differences with regular Python files,
     e.g. destroying a writable Arrow stream without closing it explicitly
     will not flush any pending data.
     """
 
+    # Default chunk size for chunked reads.
+    # Use a large enough value for networked filesystems.
+    _default_chunk_size = 256 * 1024
+
     def __cinit__(self):
         self.own_file = False
         self.is_readable = False
         self.is_writable = False
         self.is_seekable = False
 
     def __dealloc__(self):
@@ -322,16 +326,15 @@
         if self.is_writable:
             handle = self.get_output_stream()
             with nogil:
                 check_status(handle.get().Flush())
 
     def write(self, data):
         """
-        Write byte from any object implementing buffer protocol (bytes,
-        bytearray, ndarray, pyarrow.Buffer)
+        Write data to the file.
 
         Parameters
         ----------
         data : bytes-like object or exporter of buffer protocol
 
         Returns
         -------
@@ -345,16 +348,17 @@
 
         with nogil:
             check_status(handle.get().WriteBuffer(buf))
         return buf.get().size()
 
     def read(self, nbytes=None):
         """
-        Read indicated number of bytes from file, or read all remaining bytes
-        if no argument passed
+        Read and return up to n bytes.
+
+        If *nbytes* is None, then the entire remaining file contents are read.
 
         Parameters
         ----------
         nbytes : int, default None
 
         Returns
         -------
@@ -364,15 +368,15 @@
             int64_t c_nbytes
             int64_t bytes_read = 0
             PyObject* obj
 
         if nbytes is None:
             if not self.is_seekable:
                 # Cannot get file size => read chunkwise
-                bs = 16384
+                bs = self._default_chunk_size
                 chunks = []
                 while True:
                     chunk = self.read(bs)
                     if not chunk:
                         break
                     chunks.append(chunk)
                 return b"".join(chunks)
@@ -432,22 +436,33 @@
             cp._PyBytes_Resize(&obj, <Py_ssize_t> bytes_read)
 
         return PyObject_to_object(obj)
 
     def read1(self, nbytes=None):
         """Read and return up to n bytes.
 
-        Alias for read, needed to match the BufferedIOBase interface.
+        Unlike read(), if *nbytes* is None then a chunk is read, not the
+        entire file.
 
         Parameters
         ----------
-        nbytes : int
+        nbytes : int, default None
             The maximum number of bytes to read.
+
+        Returns
+        -------
+        data : bytes
         """
-        return self.read(nbytes=None)
+        if nbytes is None:
+            # The expectation when passing `nbytes=None` is not to read the
+            # entire file but to issue a single underlying read call up to
+            # a reasonable size (the use case being to read a bufferable
+            # amount of bytes, such as with io.TextIOWrapper).
+            nbytes = self._default_chunk_size
+        return self.read(nbytes)
 
     def readall(self):
         return self.read()
 
     def readinto(self, b):
         """
         Read into the supplied buffer
```

### Comparing `pyarrow-8.0.0/pyarrow/ipc.pxi` & `pyarrow-9.0.0/pyarrow/ipc.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,16 @@
         raise TypeError("Do not call {}'s constructor directly, use "
                         "`pyarrow.ipc.MessageReader.open_stream` function "
                         "instead.".format(self.__class__.__name__))
 
     @staticmethod
     def open_stream(source):
         """
-        Open stream from source.
+        Open stream from source, if you want to use memory map use
+        MemoryMappedFile as source.
 
         Parameters
         ----------
         source
             A readable source, like an InputStream
         """
         cdef:
@@ -593,37 +594,37 @@
         table = self.read_all()
         return table.to_pandas(**options)
 
 
 cdef class RecordBatchReader(_Weakrefable):
     """Base class for reading stream of record batches.
 
-    Record batch readers function as iterators of record batches that also 
+    Record batch readers function as iterators of record batches that also
     provide the schema (without the need to get any batches).
 
     Warnings
     --------
     Do not call this class's constructor directly, use one of the
     ``RecordBatchReader.from_*`` functions instead.
 
     Notes
     -----
-    To import and export using the Arrow C stream interface, use the 
+    To import and export using the Arrow C stream interface, use the
     ``_import_from_c`` and ``_export_from_c`` methods. However, keep in mind this
-    interface is experimental and intended for expert users.
+    interface is intended for expert users.
 
     Examples
     --------
+    >>> import pyarrow as pa
     >>> schema = pa.schema([('x', pa.int64())])
     >>> def iter_record_batches():
     ...     for i in range(2):
-    ...     yield pa.RecordBatch.from_arrays([pa.array([1, 2, 3])], schema=schema)
+    ...         yield pa.RecordBatch.from_arrays([pa.array([1, 2, 3])], schema=schema)
     >>> reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
     >>> print(reader.schema)
-    pyarrow.Schema
     x: int64
     >>> for batch in reader:
     ...     print(batch)
     pyarrow.RecordBatch
     x: int64
     pyarrow.RecordBatch
     x: int64
@@ -697,19 +698,26 @@
         cdef shared_ptr[CTable] table
         with nogil:
             check_status(self.reader.get().ToTable().Value(&table))
         return pyarrow_wrap_table(table)
 
     read_pandas = _ReadPandasMixin.read_pandas
 
+    def close(self):
+        """
+        Release any resources associated with the reader.
+        """
+        with nogil:
+            check_status(self.reader.get().Close())
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
+        self.close()
 
     def _export_to_c(self, out_ptr):
         """
         Export to a C ArrowArrayStream struct, given its pointer.
 
         Parameters
         ----------
@@ -843,15 +851,15 @@
         self.options = options.c_options
         self.options.memory_pool = maybe_unbox_memory_pool(memory_pool)
         try:
             source = as_buffer(source)
         except TypeError:
             pass
 
-        get_reader(source, True, &self.file)
+        get_reader(source, False, &self.file)
 
         cdef int64_t offset = 0
         if footer_offset is not None:
             offset = footer_offset
 
         with nogil:
             if offset != 0:
@@ -1085,15 +1093,15 @@
         shared_ptr[CRandomAccessFile] cpp_file
         CDictionaryMemo temp_memo
         CDictionaryMemo* arg_dict_memo
 
     if isinstance(obj, Message):
         raise NotImplementedError(type(obj))
 
-    get_reader(obj, True, &cpp_file)
+    get_reader(obj, False, &cpp_file)
 
     if dictionary_memo is not None:
         arg_dict_memo = dictionary_memo.memo
     else:
         arg_dict_memo = &temp_memo
 
     with nogil:
```

### Comparing `pyarrow-8.0.0/pyarrow/ipc.py` & `pyarrow-9.0.0/pyarrow/ipc.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     """
     Reader for the Arrow streaming binary format.
 
     Parameters
     ----------
     source : bytes/buffer-like, pyarrow.NativeFile, or file-like Python object
         Either an in-memory buffer, or a readable file object.
+        If you want to use memory map use MemoryMappedFile as source.
     options : pyarrow.ipc.IpcReadOptions
         Options for IPC deserialization.
         If None, default values will be used.
     memory_pool : MemoryPool, default None
         If None, default memory pool is used.
     """
 
@@ -87,15 +88,16 @@
 class RecordBatchFileReader(lib._RecordBatchFileReader):
     """
     Class for reading Arrow record batch data from the Arrow binary file format
 
     Parameters
     ----------
     source : bytes/buffer-like, pyarrow.NativeFile, or file-like Python object
-        Either an in-memory buffer, or a readable file object
+        Either an in-memory buffer, or a readable file object.
+        If you want to use memory map use MemoryMappedFile as source.
     footer_offset : int, default None
         If the file is embedded in some larger file, this is the byte offset to
         the very end of the file data
     options : pyarrow.ipc.IpcReadOptions
         Options for IPC serialization.
         If None, default values will be used.
     memory_pool : MemoryPool, default None
@@ -153,15 +155,20 @@
                                    use_legacy_format=use_legacy_format,
                                    options=options)
 
 
 new_stream.__doc__ = """\
 Create an Arrow columnar IPC stream writer instance
 
-{}""".format(_ipc_writer_class_doc)
+{}
+
+Returns
+-------
+writer : RecordBatchStreamWriter
+""".format(_ipc_writer_class_doc)
 
 
 def open_stream(source, *, options=None, memory_pool=None):
     """
     Create reader for Arrow streaming format.
 
     Parameters
@@ -186,15 +193,20 @@
                                  use_legacy_format=use_legacy_format,
                                  options=options)
 
 
 new_file.__doc__ = """\
 Create an Arrow columnar IPC file writer instance
 
-{}""".format(_ipc_writer_class_doc)
+{}
+
+Returns
+-------
+writer : RecordBatchFileWriter
+""".format(_ipc_writer_class_doc)
 
 
 def open_file(source, footer_offset=None, *, options=None, memory_pool=None):
     """
     Create reader for Arrow file format.
 
     Parameters
```

### Comparing `pyarrow-8.0.0/pyarrow/json.py` & `pyarrow-9.0.0/pyarrow/json.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/jvm.py` & `pyarrow-9.0.0/pyarrow/jvm.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/lib.pxd` & `pyarrow-9.0.0/pyarrow/lib.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
     cdef void init(self, CMemoryPool* pool)
 
 
 cdef CMemoryPool* maybe_unbox_memory_pool(MemoryPool memory_pool)
 
 
+cdef object box_memory_pool(CMemoryPool* pool)
+
+
 cdef class DataType(_Weakrefable):
     cdef:
         shared_ptr[CDataType] sp_type
         CDataType* type
         bytes pep3118_format
 
     cdef void init(self, const shared_ptr[CDataType]& type) except *
```

### Comparing `pyarrow-8.0.0/pyarrow/lib.pyx` & `pyarrow-9.0.0/pyarrow/lib.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/memory.pxi` & `pyarrow-9.0.0/pyarrow/memory.pxi`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,20 @@
 cdef CMemoryPool* maybe_unbox_memory_pool(MemoryPool memory_pool):
     if memory_pool is None:
         return c_get_memory_pool()
     else:
         return memory_pool.pool
 
 
+cdef api object box_memory_pool(CMemoryPool *c_pool):
+    cdef MemoryPool pool = MemoryPool.__new__(MemoryPool)
+    pool.init(c_pool)
+    return pool
+
+
 cdef class LoggingMemoryPool(MemoryPool):
     cdef:
         unique_ptr[CLoggingMemoryPool] logging_pool
 
     def __init__(self):
         raise TypeError("Do not call {}'s constructor directly, "
                         "use pyarrow.logging_memory_pool instead."
```

### Comparing `pyarrow-8.0.0/pyarrow/orc.py` & `pyarrow-9.0.0/pyarrow/orc.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/pandas-shim.pxi` & `pyarrow-9.0.0/pyarrow/pandas-shim.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/pandas_compat.py` & `pyarrow-9.0.0/pyarrow/pandas_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,25 +213,40 @@
         metadata = get_column_metadata(col, name=sanitized_name,
                                        arrow_type=arrow_type,
                                        field_name=sanitized_name)
         column_metadata.append(metadata)
 
     index_column_metadata = []
     if preserve_index is not False:
+        non_str_index_names = []
         for level, arrow_type, descriptor in zip(index_levels, index_types,
                                                  index_descriptors):
             if isinstance(descriptor, dict):
                 # The index is represented in a non-serialized fashion,
                 # e.g. RangeIndex
                 continue
-            metadata = get_column_metadata(level, name=level.name,
-                                           arrow_type=arrow_type,
-                                           field_name=descriptor)
+
+            if level.name is not None and not isinstance(level.name, str):
+                non_str_index_names.append(level.name)
+
+            metadata = get_column_metadata(
+                level,
+                name=_column_name_to_strings(level.name),
+                arrow_type=arrow_type,
+                field_name=descriptor,
+            )
             index_column_metadata.append(metadata)
 
+        if len(non_str_index_names) > 0:
+            warnings.warn(
+                f"The DataFrame has non-str index name `{non_str_index_names}`"
+                " which will be converted to string"
+                " and not roundtrip correctly.",
+                UserWarning, stacklevel=4)
+
         column_indexes = []
 
         levels = getattr(df.columns, 'levels', [df.columns])
         names = getattr(df.columns, 'names', [df.columns.name])
         for level, name in zip(levels, names):
             metadata = _get_simple_index_descriptor(level, name)
             column_indexes.append(metadata)
@@ -287,19 +302,19 @@
     Examples
     --------
     >>> name = 'foo'
     >>> _column_name_to_strings(name)
     'foo'
     >>> name = ('foo', 'bar')
     >>> _column_name_to_strings(name)
-    ('foo', 'bar')
+    "('foo', 'bar')"
     >>> import pandas as pd
     >>> name = (1, pd.Timestamp('2017-02-01 00:00:00'))
     >>> _column_name_to_strings(name)
-    ('1', '2017-02-01 00:00:00')
+    "('1', '2017-02-01 00:00:00')"
     """
     if isinstance(name, str):
         return name
     elif isinstance(name, bytes):
         # XXX: should we assume that bytes in Python 3 are UTF-8?
         return name.decode('utf8')
     elif isinstance(name, tuple):
@@ -321,15 +336,15 @@
     i : int
 
     Returns
     -------
     name : str
     """
     if index.name is not None and index.name not in column_names:
-        return index.name
+        return _column_name_to_strings(index.name)
     else:
         return '__index_level_{:d}__'.format(i)
 
 
 def _get_columns_to_convert(df, schema, preserve_index, columns):
     columns = _resolve_columns_of_interest(df, schema, columns)
```

### Comparing `pyarrow-8.0.0/pyarrow/parquet/__init__.py` & `pyarrow-9.0.0/pyarrow/parquet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,22 @@
     coerce_int96_timestamp_unit : str, default None.
         Cast timestamps that are stored in INT96 format to a particular
         resolution (e.g. 'ms'). Setting to None is equivalent to 'ns'
         and therefore INT96 timestamps will be inferred as timestamps
         in nanoseconds.
     decryption_properties : FileDecryptionProperties, default None
         File decryption properties for Parquet Modular Encryption.
+    thrift_string_size_limit : int, default None
+        If not None, override the maximum total string size allocated
+        when decoding Thrift structures. The default limit should be
+        sufficient for most Parquet files.
+    thrift_container_size_limit : int, default None
+        If not None, override the maximum total size of containers allocated
+        when decoding Thrift structures. The default limit should be
+        sufficient for most Parquet files.
 
     Examples
     --------
 
     Generate an example PyArrow Table and write it to Parquet file:
 
     >>> import pyarrow as pa
@@ -265,25 +273,28 @@
     ----
     n_legs: [[2,2,4,4,5,100]]
     animal: [  -- dictionary:
     ["Flamingo","Parrot",...,"Brittle stars","Centipede"]  -- indices:
     [0,1,2,3,4,5]]
     """
 
-    def __init__(self, source, metadata=None, common_metadata=None,
+    def __init__(self, source, *, metadata=None, common_metadata=None,
                  read_dictionary=None, memory_map=False, buffer_size=0,
                  pre_buffer=False, coerce_int96_timestamp_unit=None,
-                 decryption_properties=None):
+                 decryption_properties=None, thrift_string_size_limit=None,
+                 thrift_container_size_limit=None):
         self.reader = ParquetReader()
         self.reader.open(
             source, use_memory_map=memory_map,
             buffer_size=buffer_size, pre_buffer=pre_buffer,
             read_dictionary=read_dictionary, metadata=metadata,
             coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-            decryption_properties=decryption_properties
+            decryption_properties=decryption_properties,
+            thrift_string_size_limit=thrift_string_size_limit,
+            thrift_container_size_limit=thrift_container_size_limit,
         )
         self.common_metadata = common_metadata
         self._nested_paths_by_prefix = self._build_nested_paths()
 
     def _build_nested_paths(self):
         paths = self.reader.column_paths
 
@@ -670,15 +681,15 @@
     if 'spark' in flavor:
         column_data = [table[i] for i in range(table.num_columns)]
         return pa.Table.from_arrays(column_data, schema=new_schema)
     else:
         return table
 
 
-_parquet_writer_arg_docs = """version : {"1.0", "2.4", "2.6"}, default "1.0"
+_parquet_writer_arg_docs = """version : {"1.0", "2.4", "2.6"}, default "2.4"
     Determine which Parquet logical types are available for use, whether the
     reduced set from the Parquet 1.x.x format or the expanded logical types
     added in later format versions.
     Files written with version='2.4' or '2.6' may not be readable in all
     Parquet implementations, so version='1.0' is likely the choice that
     maximizes file compatibility.
     UINT32 and some logical types are only available with version '2.4'.
@@ -858,15 +869,15 @@
 Examples
 --------
 {}
 """.format(_parquet_writer_arg_docs, _parquet_writer_example_doc)
 
     def __init__(self, where, schema, filesystem=None,
                  flavor=None,
-                 version='1.0',
+                 version='2.4',
                  use_dictionary=True,
                  compression='snappy',
                  write_statistics=True,
                  use_deprecated_int96_timestamps=None,
                  compression_level=None,
                  use_byte_stream_split=False,
                  column_encoding=None,
@@ -1635,26 +1646,36 @@
     use_legacy_dataset=False. If using a filesystem layer that itself
     performs readahead (e.g. fsspec's S3FS), disable readahead for best
     results.
 coerce_int96_timestamp_unit : str, default None.
     Cast timestamps that are stored in INT96 format to a particular resolution
     (e.g. 'ms'). Setting to None is equivalent to 'ns' and therefore INT96
     timestamps will be inferred as timestamps in nanoseconds.
+thrift_string_size_limit : int, default None
+    If not None, override the maximum total string size allocated
+    when decoding Thrift structures. The default limit should be
+    sufficient for most Parquet files.
+thrift_container_size_limit : int, default None
+    If not None, override the maximum total size of containers allocated
+    when decoding Thrift structures. The default limit should be
+    sufficient for most Parquet files.
 
 Examples
 --------
 {2}
 """.format(_read_docstring_common, _DNF_filter_doc, _parquet_dataset_example)
 
     def __new__(cls, path_or_paths=None, filesystem=None, schema=None,
                 metadata=None, split_row_groups=False, validate_schema=True,
                 filters=None, metadata_nthreads=None, read_dictionary=None,
                 memory_map=False, buffer_size=0, partitioning="hive",
                 use_legacy_dataset=None, pre_buffer=True,
-                coerce_int96_timestamp_unit=None):
+                coerce_int96_timestamp_unit=None,
+                thrift_string_size_limit=None,
+                thrift_container_size_limit=None):
         if use_legacy_dataset is None:
             # if a new filesystem is passed -> default to new implementation
             if isinstance(filesystem, FileSystem):
                 use_legacy_dataset = False
             # otherwise the default is still True
             else:
                 use_legacy_dataset = True
@@ -1669,25 +1690,29 @@
                 buffer_size=buffer_size,
                 pre_buffer=pre_buffer,
                 coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
                 # unsupported keywords
                 schema=schema, metadata=metadata,
                 split_row_groups=split_row_groups,
                 validate_schema=validate_schema,
-                metadata_nthreads=metadata_nthreads
+                metadata_nthreads=metadata_nthreads,
+                thrift_string_size_limit=thrift_string_size_limit,
+                thrift_container_size_limit=thrift_container_size_limit,
             )
         self = object.__new__(cls)
         return self
 
     def __init__(self, path_or_paths, filesystem=None, schema=None,
                  metadata=None, split_row_groups=False, validate_schema=True,
                  filters=None, metadata_nthreads=None, read_dictionary=None,
                  memory_map=False, buffer_size=0, partitioning="hive",
                  use_legacy_dataset=True, pre_buffer=True,
-                 coerce_int96_timestamp_unit=None):
+                 coerce_int96_timestamp_unit=None,
+                 thrift_string_size_limit=None,
+                 thrift_container_size_limit=None):
         if partitioning != "hive":
             raise ValueError(
                 'Only "hive" for hive-like partitioning is supported when '
                 'using use_legacy_dataset=True')
         if metadata_nthreads is not None:
             warnings.warn(
                 "Specifying the 'metadata_nthreads' argument is deprecated as "
@@ -1855,15 +1880,15 @@
 
         Read multiple Parquet files as a single pyarrow.Table:
 
         >>> dataset.read(columns=["n_legs"])
         pyarrow.Table
         n_legs: int64
         ----
-        n_legs: [[5],[2],...,[2],[4]]
+        n_legs: [[5],[2],[4,100],[2,4]]
         """
         tables = []
         for piece in self._pieces:
             table = piece.read(columns=columns, use_threads=use_threads,
                                partitions=self._partitions,
                                use_pandas_metadata=use_pandas_metadata)
             tables.append(table)
@@ -1907,32 +1932,30 @@
         >>> import pandas as pd
         >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
         ...                    'n_legs': [2, 2, 4, 4, 5, 100],
         ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                    "Brittle stars", "Centipede"]})
         >>> table = pa.Table.from_pandas(df)
         >>> import pyarrow.parquet as pq
-        >>> pq.write_to_dataset(table, root_path='dataset_name_read_pandas',
-        ...                     partition_cols=['year'],
-        ...                     use_legacy_dataset=False)
-        >>> dataset = pq.ParquetDataset('dataset_name_read_pandas/',
+        >>> pq.write_table(table, 'table.parquet')
+        >>> dataset = pq.ParquetDataset('table.parquet',
         ...                             use_legacy_dataset=False)
 
         Read dataset including pandas metadata:
 
         >>> dataset.read_pandas(columns=["n_legs"])
         pyarrow.Table
         n_legs: int64
         ----
-        n_legs: [[5],[2],...,[2],[4]]
+        n_legs: [[2,2,4,4,5,100]]
 
         Select pandas metadata:
 
         >>> dataset.read_pandas(columns=["n_legs"]).schema.pandas_metadata
-        {'index_columns': [{'kind': 'range', ... 'pandas_version': '1.4.1'}
+        {'index_columns': [{'kind': 'range', 'name': None, 'start': 0, ...}
         """
         return self.read(use_pandas_metadata=True, **kwargs)
 
     def _get_common_pandas_metadata(self):
         if self._common_metadata is None:
             return None
 
@@ -2100,15 +2123,15 @@
         ...                   'n_legs': [2, 2, 4, 4, 5, 100],
         ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                              "Brittle stars", "Centipede"]})
         >>> import pyarrow.parquet as pq
         >>> pq.write_to_dataset(table, root_path='dataset_name_fragments',
         ...                     partition_cols=['year'],
         ...                     use_legacy_dataset=False)
-        >>> dataset = pq.ParquetDataset('dataset_name_files/',
+        >>> dataset = pq.ParquetDataset('dataset_name_fragments/',
         ...                             use_legacy_dataset=False)
 
         List the fragments:
 
         >>> dataset.fragments
         [<pyarrow.dataset.ParquetFileFragment path=dataset_name_fragments/...
         """
@@ -2138,15 +2161,15 @@
         ...                     use_legacy_dataset=False)
         >>> dataset = pq.ParquetDataset('dataset_name_files/',
         ...                             use_legacy_dataset=False)
 
         List the files:
 
         >>> dataset.files
-        ['dataset_name_files/year=2019/part-0.parquet', ...
+        ['dataset_name_files/year=2019/...-0.parquet', ...
         """
         raise NotImplementedError(
             "To use this property set 'use_legacy_dataset=False' while "
             "constructing the ParquetDataset")
 
     @property
     def filesystem(self):
@@ -2230,59 +2253,64 @@
     ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
     ...                              "Brittle stars", "Centipede"]})
     >>> import pyarrow.parquet as pq
     >>> pq.write_to_dataset(table, root_path='dataset_v2',
     ...                     partition_cols=['year'],
     ...                     use_legacy_dataset=False)
 
-    create a _ParquetDatasetV2 object from the dataset source:
+    create a ParquetDataset object from the dataset source:
 
-    >>> dataset = pq._ParquetDatasetV2('dataset_v2/')
+    >>> dataset = pq.ParquetDataset('dataset_v2/', use_legacy_dataset=False)
 
     and read the data:
 
     >>> dataset.read().to_pandas()
        n_legs         animal  year
     0       5  Brittle stars  2019
     1       2       Flamingo  2020
     2       4            Dog  2021
     3     100      Centipede  2021
     4       2         Parrot  2022
     5       4          Horse  2022
 
-    create a _ParquetDatasetV2 object with filter:
+    create a ParquetDataset object with filter:
 
-    >>> dataset = pq._ParquetDatasetV2('dataset_v2/',
-    ...                                filters=[('n_legs','=',4)])
+    >>> dataset = pq.ParquetDataset('dataset_v2/',
+    ...                             filters=[('n_legs','=',4)],
+    ...                             use_legacy_dataset=False)
     >>> dataset.read().to_pandas()
        n_legs animal  year
     0       4    Dog  2021
     1       4  Horse  2022
     """
 
-    def __init__(self, path_or_paths, filesystem=None, filters=None,
+    def __init__(self, path_or_paths, filesystem=None, *, filters=None,
                  partitioning="hive", read_dictionary=None, buffer_size=None,
                  memory_map=False, ignore_prefixes=None, pre_buffer=True,
                  coerce_int96_timestamp_unit=None, schema=None,
-                 decryption_properties=None, **kwargs):
+                 decryption_properties=None, thrift_string_size_limit=None,
+                 thrift_container_size_limit=None,
+                 **kwargs):
         import pyarrow.dataset as ds
 
         # Raise error for not supported keywords
         for keyword, default in [
                 ("metadata", None), ("split_row_groups", False),
                 ("validate_schema", True), ("metadata_nthreads", None)]:
             if keyword in kwargs and kwargs[keyword] is not default:
                 raise ValueError(
                     "Keyword '{0}' is not yet supported with the new "
                     "Dataset API".format(keyword))
 
         # map format arguments
         read_options = {
             "pre_buffer": pre_buffer,
-            "coerce_int96_timestamp_unit": coerce_int96_timestamp_unit
+            "coerce_int96_timestamp_unit": coerce_int96_timestamp_unit,
+            "thrift_string_size_limit": thrift_string_size_limit,
+            "thrift_container_size_limit": thrift_container_size_limit,
         }
         if buffer_size:
             read_options.update(use_buffered_stream=True,
                                 buffer_size=buffer_size)
         if read_dictionary is not None:
             read_options.update(dictionary_columns=read_dictionary)
 
@@ -2367,15 +2395,16 @@
         ...                   'n_legs': [2, 2, 4, 4, 5, 100],
         ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                              "Brittle stars", "Centipede"]})
         >>> import pyarrow.parquet as pq
         >>> pq.write_to_dataset(table, root_path='dataset_v2_schema',
         ...                     partition_cols=['year'],
         ...                     use_legacy_dataset=False)
-        >>> dataset = pq._ParquetDatasetV2('dataset_v2_schema/')
+        >>> dataset = pq.ParquetDataset('dataset_v2_schema/',
+        ...                             use_legacy_dataset=False)
 
         Read the schema:
 
         >>> dataset.schema
         n_legs: int64
         animal: string
         year: dictionary<values=int32, indices=int32, ordered=0>
@@ -2412,23 +2441,24 @@
         ...                   'n_legs': [2, 2, 4, 4, 5, 100],
         ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                              "Brittle stars", "Centipede"]})
         >>> import pyarrow.parquet as pq
         >>> pq.write_to_dataset(table, root_path='dataset_v2_read',
         ...                     partition_cols=['year'],
         ...                     use_legacy_dataset=False)
-        >>> dataset = pq._ParquetDatasetV2('dataset_v2_read/')
+        >>> dataset = pq.ParquetDataset('dataset_v2_read/',
+        ...                             use_legacy_dataset=False)
 
         Read the dataset:
 
         >>> dataset.read(columns=["n_legs"])
         pyarrow.Table
         n_legs: int64
         ----
-        n_legs: [[5],[2],...,[2],[4]]
+        n_legs: [[5],[2],[4,100],[2,4]]
         """
         # if use_pandas_metadata, we need to include index columns in the
         # column selection, to be able to restore those in the pandas DataFrame
         metadata = self.schema.metadata
         if columns is not None and use_pandas_metadata:
             if metadata and b'pandas' in metadata:
                 # RangeIndex can be represented as dict instead of column name
@@ -2458,37 +2488,38 @@
     def read_pandas(self, **kwargs):
         """
         Read dataset including pandas metadata, if any. Other arguments passed
         through to ParquetDataset.read, see docstring for further details.
 
         Examples
         --------
-        Generate an example dataset:
+        Generate an example parquet file:
 
         >>> import pyarrow as pa
-        >>> table = pa.table({'year': [2020, 2022, 2021, 2022, 2019, 2021],
-        ...                   'n_legs': [2, 2, 4, 4, 5, 100],
-        ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
-        ...                              "Brittle stars", "Centipede"]})
+        >>> import pandas as pd
+        >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
+        ...                    'n_legs': [2, 2, 4, 4, 5, 100],
+        ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
+        ...                    "Brittle stars", "Centipede"]})
+        >>> table = pa.Table.from_pandas(df)
         >>> import pyarrow.parquet as pq
-        >>> pq.write_to_dataset(table, root_path='dataset_v2_read_pandas',
-        ...                     partition_cols=['year'],
-        ...                     use_legacy_dataset=False)
-        >>> dataset = pq._ParquetDatasetV2('dataset_v2_read_pandas/')
+        >>> pq.write_table(table, 'table_V2.parquet')
+        >>> dataset = pq.ParquetDataset('table_V2.parquet',
+        ...                             use_legacy_dataset=False)
 
         Read the dataset with pandas metadata:
 
         >>> dataset.read_pandas(columns=["n_legs"])
         pyarrow.Table
         n_legs: int64
         ----
-        n_legs: [[5],[2],...,[2],[4]]
+        n_legs: [[2,2,4,4,5,100]]
 
         >>> dataset.read_pandas(columns=["n_legs"]).schema.pandas_metadata
-        {'index_columns': [{'kind': 'range', ... 'pandas_version': '1.4.1'}
+        {'index_columns': [{'kind': 'range', 'name': None, 'start': 0, ...}
         """
         return self.read(use_pandas_metadata=True, **kwargs)
 
     @property
     def pieces(self):
         warnings.warn(
             _DEPR_MSG.format("ParquetDataset.pieces",
@@ -2511,15 +2542,16 @@
         ...                   'n_legs': [2, 2, 4, 4, 5, 100],
         ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                              "Brittle stars", "Centipede"]})
         >>> import pyarrow.parquet as pq
         >>> pq.write_to_dataset(table, root_path='dataset_v2_fragments',
         ...                     partition_cols=['year'],
         ...                     use_legacy_dataset=False)
-        >>> dataset = pq._ParquetDatasetV2('dataset_v2_fragments/')
+        >>> dataset = pq.ParquetDataset('dataset_v2_fragments/',
+        ...                             use_legacy_dataset=False)
 
         List the fragments:
 
         >>> dataset.fragments
         [<pyarrow.dataset.ParquetFileFragment path=dataset_v2_fragments/...
         """
         return list(self._dataset.get_fragments())
@@ -2538,20 +2570,21 @@
         ...                   'n_legs': [2, 2, 4, 4, 5, 100],
         ...                   'animal': ["Flamingo", "Parrot", "Dog", "Horse",
         ...                              "Brittle stars", "Centipede"]})
         >>> import pyarrow.parquet as pq
         >>> pq.write_to_dataset(table, root_path='dataset_v2_files',
         ...                     partition_cols=['year'],
         ...                     use_legacy_dataset=False)
-        >>> dataset = pq._ParquetDatasetV2('dataset_v2_files/')
+        >>> dataset = pq.ParquetDataset('dataset_v2_files/',
+        ...                             use_legacy_dataset=False)
 
         List the files:
 
         >>> dataset.files
-        ['dataset_v2_files/year=2019/part-0.parquet', ...
+        ['dataset_v2_files/year=2019/...-0.parquet', ...
         """
         return self._dataset.files
 
     @property
     def filesystem(self):
         """
         The filesystem type of the Dataset source.
@@ -2628,14 +2661,23 @@
     resolution (e.g. 'ms'). Setting to None is equivalent to 'ns'
     and therefore INT96 timestamps will be inferred as timestamps
     in nanoseconds.
 decryption_properties : FileDecryptionProperties or None
     File-level decryption properties.
     The decryption properties can be created using
     ``CryptoFactory.file_decryption_properties()``.
+thrift_string_size_limit : int, default None
+    If not None, override the maximum total string size allocated
+    when decoding Thrift structures. The default limit should be
+    sufficient for most Parquet files.
+thrift_container_size_limit : int, default None
+    If not None, override the maximum total size of containers allocated
+    when decoding Thrift structures. The default limit should be
+    sufficient for most Parquet files.
+
 Returns
 -------
 {2}
 
 {4}
 """
 
@@ -2670,35 +2712,35 @@
 Read only a subset of columns:
 
 >>> pq.read_table('dataset_name_2', columns=["n_legs", "animal"])
 pyarrow.Table
 n_legs: int64
 animal: string
 ----
-n_legs: [[5],[2],...,[2],[4]]
-animal: [["Brittle stars"],["Flamingo"],...,["Parrot"],["Horse"]]
+n_legs: [[5],[2],[4,100],[2,4]]
+animal: [["Brittle stars"],["Flamingo"],["Dog","Centipede"],["Parrot","Horse"]]
 
 Read a subset of columns and read one column as DictionaryArray:
 
 >>> pq.read_table('dataset_name_2', columns=["n_legs", "animal"],
 ...               read_dictionary=["animal"])
 pyarrow.Table
 n_legs: int64
 animal: dictionary<values=string, indices=int32, ordered=0>
 ----
-n_legs: [[5],[2],...,[2],[4]]
+n_legs: [[5],[2],[4,100],[2,4]]
 animal: [  -- dictionary:
 ["Brittle stars"]  -- indices:
 [0],  -- dictionary:
 ["Flamingo"]  -- indices:
-[0],...,  -- dictionary:
-["Parrot"]  -- indices:
 [0],  -- dictionary:
-["Horse"]  -- indices:
-[0]]
+["Dog","Centipede"]  -- indices:
+[0,1],  -- dictionary:
+["Parrot","Horse"]  -- indices:
+[0,1]]
 
 Read the table with filter:
 
 >>> pq.read_table('dataset_name_2', columns=["n_legs", "animal"],
 ...               filters=[('n_legs','<',4)]).to_pandas()
    n_legs    animal
 0       2  Flamingo
@@ -2707,28 +2749,29 @@
 Read data from a single Parquet file:
 
 >>> pq.write_table(table, 'example.parquet')
 >>> pq.read_table('dataset_name_2').to_pandas()
    n_legs         animal  year
 0       5  Brittle stars  2019
 1       2       Flamingo  2020
-2     100      Centipede  2021
-3       4            Dog  2021
+2       4            Dog  2021
+3     100      Centipede  2021
 4       2         Parrot  2022
 5       4          Horse  2022
 """
 
 
-def read_table(source, columns=None, use_threads=True, metadata=None,
+def read_table(source, *, columns=None, use_threads=True, metadata=None,
                schema=None, use_pandas_metadata=False, memory_map=False,
                read_dictionary=None, filesystem=None, filters=None,
                buffer_size=0, partitioning="hive", use_legacy_dataset=False,
                ignore_prefixes=None, pre_buffer=True,
                coerce_int96_timestamp_unit=None,
-               decryption_properties=None):
+               decryption_properties=None, thrift_string_size_limit=None,
+               thrift_container_size_limit=None):
     if not use_legacy_dataset:
         if metadata is not None:
             raise ValueError(
                 "The 'metadata' keyword is no longer supported with the new "
                 "datasets-based implementation. Specify "
                 "'use_legacy_dataset=True' to temporarily recover the old "
                 "behaviour."
@@ -2741,15 +2784,17 @@
                 partitioning=partitioning,
                 memory_map=memory_map,
                 read_dictionary=read_dictionary,
                 buffer_size=buffer_size,
                 filters=filters,
                 ignore_prefixes=ignore_prefixes,
                 pre_buffer=pre_buffer,
-                coerce_int96_timestamp_unit=coerce_int96_timestamp_unit
+                coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
+                thrift_string_size_limit=thrift_string_size_limit,
+                thrift_container_size_limit=thrift_container_size_limit,
             )
         except ImportError:
             # fall back on ParquetFile for simple cases when pyarrow.dataset
             # module is not available
             if filters is not None:
                 raise ValueError(
                     "the 'filters' keyword is not supported when the "
@@ -2770,15 +2815,17 @@
                 source = filesystem.open_input_file(path)
             # TODO test that source is not a directory or a list
             dataset = ParquetFile(
                 source, metadata=metadata, read_dictionary=read_dictionary,
                 memory_map=memory_map, buffer_size=buffer_size,
                 pre_buffer=pre_buffer,
                 coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-                decryption_properties=decryption_properties
+                decryption_properties=decryption_properties,
+                thrift_string_size_limit=thrift_string_size_limit,
+                thrift_container_size_limit=thrift_container_size_limit,
             )
 
         return dataset.read(columns=columns, use_threads=use_threads,
                             use_pandas_metadata=use_pandas_metadata)
 
     warnings.warn(
         "Passing 'use_legacy_dataset=True' to get the legacy behaviour is "
@@ -2846,15 +2893,15 @@
     additional options for :func:`read_table`""")),
     """pyarrow.Table
     Content of the file as a Table of Columns, including DataFrame
     indexes as columns""",
     _DNF_filter_doc, "")
 
 
-def write_table(table, where, row_group_size=None, version='1.0',
+def write_table(table, where, row_group_size=None, version='2.4',
                 use_dictionary=True, compression='snappy',
                 write_statistics=True,
                 use_deprecated_int96_timestamps=None,
                 coerce_timestamps=None,
                 allow_truncated_timestamps=False,
                 data_page_size=None, flavor=None,
                 filesystem=None,
@@ -2967,15 +3014,16 @@
 def write_to_dataset(table, root_path, partition_cols=None,
                      partition_filename_cb=None, filesystem=None,
                      use_legacy_dataset=None, schema=None,
                      partitioning=None, basename_template=None,
                      use_threads=None, file_visitor=None,
                      existing_data_behavior=None,
                      **kwargs):
-    """Wrapper around parquet.write_table for writing a Table to
+    """Wrapper around dataset.write_dataset (when use_legacy_dataset=False) or
+    parquet.write_table (when use_legacy_dataset=True) for writing a Table to
     Parquet format by partitions.
     For each combination of partition columns and values,
     a subdirectories are created in the following
     manner:
 
     root_dir/
       group1=value1
@@ -3001,34 +3049,41 @@
     partition_cols : list,
         Column names by which to partition the dataset.
         Columns are partitioned in the order they are given
     partition_filename_cb : callable,
         A callback function that takes the partition key(s) as an argument
         and allow you to override the partition filename. If nothing is
         passed, the filename will consist of a uuid.
+        This option is only supported for use_legacy_dataset=True.
+        When use_legacy_dataset=None and this option is specified,
+        use_legacy_datase will be set to True.
     use_legacy_dataset : bool
         Default is False. Set to True to use the the legacy behaviour
         (this option is deprecated, and the legacy implementation will be
         removed in a future version). The legacy implementation still
         supports the `partition_filename_cb` keyword but is less efficient
         when using partition columns.
     use_threads : bool, default True
         Write files in parallel. If enabled, then maximum parallelism will be
         used determined by the number of available CPU cores.
+        This option is only supported for use_legacy_dataset=False.
     schema : Schema, optional
+        This option is only supported for use_legacy_dataset=False.
     partitioning : Partitioning or list[str], optional
         The partitioning scheme specified with the
         ``pyarrow.dataset.partitioning()`` function or a list of field names.
         When providing a list of field names, you can use
         ``partitioning_flavor`` to drive which partitioning type should be
         used.
+        This option is only supported for use_legacy_dataset=False.
     basename_template : str, optional
         A template string used to generate basenames of written data files.
         The token '{i}' will be replaced with an automatically incremented
         integer. If not specified, it defaults to "guid-{i}.parquet".
+        This option is only supported for use_legacy_dataset=False.
     file_visitor : function
         If set, this function will be called with a WrittenFile instance
         for each file created during the call.  This object will have both
         a path attribute and a metadata attribute.
 
         The path attribute will be a string containing the path to
         the created file.
@@ -3040,39 +3095,41 @@
 
         Example visitor which simple collects the filenames created::
 
             visited_paths = []
 
             def file_visitor(written_file):
                 visited_paths.append(written_file.path)
+        This option is only supported for use_legacy_dataset=False.
     existing_data_behavior : 'overwrite_or_ignore' | 'error' | \
 'delete_matching'
         Controls how the dataset will handle data that already exists in
         the destination. The default behaviour is 'overwrite_or_ignore'.
 
-        Only used in the new code path using the new Arrow Dataset API
-        (``use_legacy_dataset=False``). In case the legacy implementation
-        is selected the parameter is ignored as the old implementation does
-        not support it (only has the default behaviour).
-
         'overwrite_or_ignore' will ignore any existing data and will
         overwrite files with the same name as an output file.  Other
         existing files will be ignored.  This behavior, in combination
         with a unique basename_template for each write, will allow for
         an append workflow.
 
         'error' will raise an error if any data exists in the destination.
 
         'delete_matching' is useful when you are writing a partitioned
         dataset.  The first time each partition directory is encountered
         the entire directory will be deleted.  This allows you to overwrite
         old partitions completely.
+        This option is only supported for use_legacy_dataset=False.
     **kwargs : dict,
-        Additional kwargs for write_table function. See docstring for
-        `write_table` or `ParquetWriter` for more information.
+        When use_legacy_dataset=False, used as additional kwargs for
+        `dataset.write_dataset` function (passed to
+        `ParquetFileFormat.make_write_options`). See the docstring
+        of `write_table` for the available options.
+        When use_legacy_dataset=True, used as additional kwargs for
+        `parquet.write_table` function (See docstring for `write_table`
+        or `ParquetWriter` for more information).
         Using `metadata_collector` in kwargs allows one to collect the
         file metadata instances of dataset pieces. The file paths in the
         ColumnChunkMetaData will be set relative to `root_path`.
 
     Examples
     --------
     Generate an example PyArrow Table:
@@ -3085,31 +3142,59 @@
 
     and write it to a partitioned dataset:
 
     >>> import pyarrow.parquet as pq
     >>> pq.write_to_dataset(table, root_path='dataset_name_3',
     ...                     partition_cols=['year'])
     >>> pq.ParquetDataset('dataset_name_3', use_legacy_dataset=False).files
-    ['dataset_name_3/year=2019/part-0.parquet', ...
+    ['dataset_name_3/year=2019/...-0.parquet', ...
 
     Write a single Parquet file into the root folder:
 
     >>> pq.write_to_dataset(table, root_path='dataset_name_4')
     >>> pq.ParquetDataset('dataset_name_4/', use_legacy_dataset=False).files
-    ['dataset_name_4/part-0.parquet']
+    ['dataset_name_4/...-0.parquet']
     """
+    # Choose the implementation
     if use_legacy_dataset is None:
         # if partition_filename_cb is specified ->
         # default to the old implementation
         if partition_filename_cb:
             use_legacy_dataset = True
         # otherwise the default is False
         else:
             use_legacy_dataset = False
 
+    # Check for conflicting kewords
+    msg_confl_0 = (
+        "The '{0}' argument is not supported by use_legacy_dataset={2}. "
+        "Use only '{1}' instead."
+    )
+    msg_confl_1 = (
+        "The '{1}' argument is not supported by use_legacy_dataset={2}. "
+        "Use only '{0}' instead."
+    )
+    msg_confl = msg_confl_0 if use_legacy_dataset else msg_confl_1
+    if partition_filename_cb is not None and basename_template is not None:
+        raise ValueError(msg_confl.format("basename_template",
+                                          "partition_filename_cb",
+                                          use_legacy_dataset))
+
+    if partition_cols is not None and partitioning is not None:
+        raise ValueError(msg_confl.format("partitioning",
+                                          "partition_cols",
+                                          use_legacy_dataset))
+
+    metadata_collector = kwargs.pop('metadata_collector', None)
+    if metadata_collector is not None and file_visitor is not None:
+        raise ValueError(msg_confl.format("file_visitor",
+                                          "metadata_collector",
+                                          use_legacy_dataset))
+
+    # New dataset implementation
     if not use_legacy_dataset:
         import pyarrow.dataset as ds
 
         # extract non-file format options
         schema = kwargs.pop("schema", None)
         use_threads = kwargs.pop("use_threads", True)
         chunk_size = kwargs.pop("chunk_size", None)
@@ -3120,51 +3205,50 @@
         )
 
         # raise for unsupported keywords
         msg = (
             "The '{}' argument is not supported with the new dataset "
             "implementation."
         )
-        metadata_collector = kwargs.pop('metadata_collector', None)
-        file_visitor = None
+
         if metadata_collector is not None:
             def file_visitor(written_file):
                 metadata_collector.append(written_file.metadata)
         if partition_filename_cb is not None:
             raise ValueError(msg.format("partition_filename_cb"))
 
         # map format arguments
         parquet_format = ds.ParquetFileFormat()
         write_options = parquet_format.make_write_options(**kwargs)
 
         # map old filesystems to new one
         if filesystem is not None:
             filesystem = _ensure_filesystem(filesystem)
 
-        partitioning = None
         if partition_cols:
             part_schema = table.select(partition_cols).schema
             partitioning = ds.partitioning(part_schema, flavor="hive")
 
         if basename_template is None:
             basename_template = guid() + '-{i}.parquet'
-            if existing_data_behavior is None:
-                existing_data_behavior = 'overwrite_or_ignore'
+
+        if existing_data_behavior is None:
+            existing_data_behavior = 'overwrite_or_ignore'
 
         ds.write_dataset(
             table, root_path, filesystem=filesystem,
             format=parquet_format, file_options=write_options, schema=schema,
             partitioning=partitioning, use_threads=use_threads,
             file_visitor=file_visitor,
             basename_template=basename_template,
             existing_data_behavior=existing_data_behavior,
             max_rows_per_group=row_group_size)
         return
 
-    # warnings and errors when using legecy implementation
+    # warnings and errors when using legacy implementation
     if use_legacy_dataset:
         warnings.warn(
             "Passing 'use_legacy_dataset=True' to get the legacy behaviour is "
             "deprecated as of pyarrow 8.0.0, and the legacy implementation "
             "will be removed in a future version.",
             FutureWarning, stacklevel=2)
     msg2 = (
@@ -3179,29 +3263,30 @@
         raise ValueError(msg2.format("partitioning"))
     if use_threads is not None:
         raise ValueError(msg2.format("use_threads"))
     if file_visitor is not None:
         raise ValueError(msg2.format("file_visitor"))
     if existing_data_behavior is not None:
         raise ValueError(msg2.format("existing_data_behavior"))
+    if basename_template is not None:
+        raise ValueError(msg2.format("basename_template"))
     if partition_filename_cb is not None:
         warnings.warn(
             _DEPR_MSG.format("partition_filename_cb", " Specify "
                              "'use_legacy_dataset=False' while constructing "
                              "the ParquetDataset, and then use the "
                              "'basename_template' parameter instead. For "
                              "usage see `pyarrow.dataset.write_dataset`"),
             FutureWarning, stacklevel=2)
 
+    # Legacy implementation
     fs, root_path = legacyfs.resolve_filesystem_and_path(root_path, filesystem)
 
     _mkdir_if_not_exists(fs, root_path)
 
-    metadata_collector = kwargs.pop('metadata_collector', None)
-
     if partition_cols is not None and len(partition_cols) > 0:
         df = table.to_pandas()
         partition_keys = [df[col] for col in partition_cols]
         data_df = df.drop(partition_cols, axis='columns')
         data_cols = df.columns.drop(partition_cols)
         if len(data_cols) == 0:
             raise ValueError('No data left to save outside partition columns')
@@ -3329,15 +3414,15 @@
 
     >>> pq.read_metadata('example.parquet')
     <pyarrow._parquet.FileMetaData object at ...>
       created_by: parquet-cpp-arrow version ...
       num_columns: 2
       num_rows: 3
       num_row_groups: 1
-      format_version: 1.0
+      format_version: 2.6
       serialized_size: 561
     """
     return ParquetFile(where, memory_map=memory_map,
                        decryption_properties=decryption_properties).metadata
 
 
 def read_schema(where, memory_map=False, decryption_properties=None):
```

### Comparing `pyarrow-8.0.0/pyarrow/parquet/encryption.py` & `pyarrow-9.0.0/pyarrow/parquet/encryption.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/plasma.py` & `pyarrow-9.0.0/pyarrow/plasma.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/public-api.pxi` & `pyarrow-9.0.0/pyarrow/public-api.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
     if data_type.id() == _Type_NA:
         return _NULL
 
     if data_type.id() not in _scalar_classes:
         raise ValueError('Scalar type not supported')
 
-    klass = _scalar_classes[data_type.id()]
+    klass = get_scalar_class_from_type(sp_scalar.get().type)
 
     cdef Scalar scalar = klass.__new__(klass)
     scalar.init(sp_scalar)
     return scalar
 
 
 cdef api bint pyarrow_is_tensor(object tensor):
```

### Comparing `pyarrow-8.0.0/pyarrow/scalar.pxi` & `pyarrow-9.0.0/pyarrow/scalar.pxi`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,24 @@
         self.wrapped = wrapped
 
     @staticmethod
     cdef wrap(const shared_ptr[CScalar]& wrapped):
         cdef:
             Scalar self
             Type type_id = wrapped.get().type.get().id()
+            shared_ptr[CDataType] sp_data_type = wrapped.get().type
 
         if type_id == _Type_NA:
             return _NULL
 
-        try:
-            typ = _scalar_classes[type_id]
-        except KeyError:
+        if type_id not in _scalar_classes:
             raise NotImplementedError(
-                "Wrapping scalar of type " +
-                frombytes(wrapped.get().type.get().ToString()))
+                "Wrapping scalar of type " + frombytes(sp_data_type.get().ToString()))
+
+        typ = get_scalar_class_from_type(sp_data_type)
         self = typ.__new__(typ)
         self.init(wrapped)
 
         return self
 
     cdef inline shared_ptr[CScalar] unwrap(self) nogil:
         return self.wrapped
@@ -856,16 +856,22 @@
     """
 
     @property
     def value(self):
         """
         Return underlying value as a scalar.
         """
-        cdef CUnionScalar* sp = <CUnionScalar*> self.wrapped.get()
-        return Scalar.wrap(sp.value) if sp.is_valid else None
+        cdef CSparseUnionScalar* sp
+        cdef CDenseUnionScalar* dp
+        if self.type.id == _Type_SPARSE_UNION:
+            sp = <CSparseUnionScalar*> self.wrapped.get()
+            return Scalar.wrap(sp.value[sp.child_id]) if sp.is_valid else None
+        else:
+            dp = <CDenseUnionScalar*> self.wrapped.get()
+            return Scalar.wrap(dp.value) if dp.is_valid else None
 
     def as_py(self):
         """
         Return underlying value as a Python object.
         """
         value = self.value
         return None if value is None else value.as_py()
@@ -892,17 +898,15 @@
         cdef CExtensionScalar* sp = <CExtensionScalar*> self.wrapped.get()
         return Scalar.wrap(sp.value) if sp.is_valid else None
 
     def as_py(self):
         """
         Return this scalar as a Python object.
         """
-        # XXX should there be a hook to wrap the result in a custom class?
-        value = self.value
-        return None if value is None else value.as_py()
+        return None if self.value is None else self.value.as_py()
 
     @staticmethod
     def from_storage(BaseExtensionType typ, value):
         """
         Construct ExtensionScalar from type and storage value.
 
         Parameters
@@ -914,33 +918,37 @@
 
         Returns
         -------
         ext_scalar : ExtensionScalar
         """
         cdef:
             shared_ptr[CExtensionScalar] sp_scalar
+            shared_ptr[CScalar] sp_storage
             CExtensionScalar* ext_scalar
 
         if value is None:
             storage = None
         elif isinstance(value, Scalar):
             if value.type != typ.storage_type:
                 raise TypeError("Incompatible storage type {0} "
                                 "for extension type {1}"
                                 .format(value.type, typ))
             storage = value
         else:
             storage = scalar(value, typ.storage_type)
 
-        sp_scalar = make_shared[CExtensionScalar](typ.sp_type)
-        ext_scalar = sp_scalar.get()
-        ext_scalar.is_valid = storage is not None and storage.is_valid
-        if ext_scalar.is_valid:
-            ext_scalar.value = pyarrow_unwrap_scalar(storage)
-        check_status(ext_scalar.Validate())
+        cdef c_bool is_valid = storage is not None and storage.is_valid
+        if is_valid:
+            sp_storage = pyarrow_unwrap_scalar(storage)
+        else:
+            sp_storage = MakeNullScalar((<DataType> typ.storage_type).sp_type)
+        sp_scalar = make_shared[CExtensionScalar](sp_storage, typ.sp_type,
+                                                  is_valid)
+        with nogil:
+            check_status(sp_scalar.get().Validate())
         return pyarrow_wrap_scalar(<shared_ptr[CScalar]> sp_scalar)
 
 
 cdef dict _scalar_classes = {
     _Type_BOOL: BooleanScalar,
     _Type_UINT8: UInt8Scalar,
     _Type_UINT16: UInt16Scalar,
@@ -975,14 +983,27 @@
     _Type_SPARSE_UNION: UnionScalar,
     _Type_DENSE_UNION: UnionScalar,
     _Type_INTERVAL_MONTH_DAY_NANO: MonthDayNanoIntervalScalar,
     _Type_EXTENSION: ExtensionScalar,
 }
 
 
+cdef object get_scalar_class_from_type(
+        const shared_ptr[CDataType]& sp_data_type):
+    cdef CDataType* data_type = sp_data_type.get()
+    if data_type == NULL:
+        raise ValueError('Scalar data type was NULL')
+
+    if data_type.id() == _Type_EXTENSION:
+        py_ext_data_type = pyarrow_wrap_data_type(sp_data_type)
+        return py_ext_data_type.__arrow_ext_scalar_class__()
+    else:
+        return _scalar_classes[data_type.id()]
+
+
 def scalar(value, type=None, *, from_pandas=None, MemoryPool memory_pool=None):
     """
     Create a pyarrow.Scalar instance from a Python object.
 
     Parameters
     ----------
     value : Any
```

### Comparing `pyarrow-8.0.0/pyarrow/serialization.pxi` & `pyarrow-9.0.0/pyarrow/serialization.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
     """
     _deprecate_serialization("read_serialized")
     return _read_serialized(source, base=base)
 
 
 def _read_serialized(source, base=None):
     cdef shared_ptr[CRandomAccessFile] stream
-    get_reader(source, True, &stream)
+    get_reader(source, False, &stream)
 
     cdef SerializedPyObject serialized = SerializedPyObject()
     serialized.base = base
     with nogil:
         check_status(ReadSerializedObject(stream.get(), &serialized.data))
 
     return serialized
```

### Comparing `pyarrow-8.0.0/pyarrow/serialization.py` & `pyarrow-9.0.0/pyarrow/serialization.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/table.pxi` & `pyarrow-9.0.0/pyarrow/table.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -313,17 +313,15 @@
         >>> n_legs = pa.chunked_array([[2, 2, 4], [4, None, 100]])
         >>> n_legs.is_null()
         <pyarrow.lib.ChunkedArray object at ...>
         [
           [
             false,
             false,
-            false
-          ],
-          [
+            false,
             false,
             true,
             false
           ]
         ]
         """
         options = _pc().NullOptions(nan_is_null=nan_is_null)
@@ -486,26 +484,28 @@
 
     def __array__(self, dtype=None):
         values = self.to_numpy()
         if dtype is None:
             return values
         return values.astype(dtype)
 
-    def cast(self, object target_type, safe=True):
+    def cast(self, object target_type=None, safe=None, options=None):
         """
         Cast array values to another data type
 
         See :func:`pyarrow.compute.cast` for usage.
 
         Parameters
         ----------
-        target_type : DataType
+        target_type : DataType, None
             Type to cast array to.
         safe : boolean, default True
             Whether to check for conversion errors such as overflow.
+        options : CastOptions, default None
+            Additional checks pass by CastOptions
 
         Returns
         -------
         cast : Array or ChunkedArray
 
         Examples
         --------
@@ -516,15 +516,15 @@
 
         Change the data type of an array:
 
         >>> n_legs_seconds = n_legs.cast(pa.duration('s'))
         >>> n_legs_seconds.type
         DurationType(duration[s])
         """
-        return _pc().cast(self, target_type, safe=safe)
+        return _pc().cast(self, target_type, safe=safe, options=options)
 
     def dictionary_encode(self, null_encoding='mask'):
         """
         Compute dictionary-encoded representation of array.
 
         See :func:`pyarrow.compute.dictionary_encode` for full usage.
 
@@ -2882,38 +2882,55 @@
 
         return pyarrow_wrap_table(result)
 
     def filter(self, mask, object null_selection_behavior="drop"):
         """
         Select rows from the table.
 
-        See :func:`pyarrow.compute.filter` for full usage.
+        The Table can be filtered based on a mask, which will be passed to
+        :func:`pyarrow.compute.filter` to perform the filtering, or it can
+        be filtered through a boolean :class:`.Expression`
 
         Parameters
         ----------
-        mask : Array or array-like
-            The boolean mask to filter the table with.
+        mask : Array or array-like or .Expression
+            The boolean mask or the :class:`.Expression` to filter the table with.
         null_selection_behavior
-            How nulls in the mask should be handled.
+            How nulls in the mask should be handled, does nothing if
+            an :class:`.Expression` is used.
 
         Returns
         -------
         filtered : Table
             A table of the same schema, with only the rows selected
-            by the boolean mask.
+            by applied filtering
 
         Examples
         --------
         >>> import pyarrow as pa
         >>> import pandas as pd
         >>> df = pd.DataFrame({'year': [2020, 2022, 2019, 2021],
         ...                    'n_legs': [2, 4, 5, 100],
         ...                    'animals': ["Flamingo", "Horse", "Brittle stars", "Centipede"]})
         >>> table = pa.Table.from_pandas(df)
 
+        Define an expression and select rows:
+
+        >>> import pyarrow.compute as pc
+        >>> expr = pc.field("year") <= 2020
+        >>> table.filter(expr)
+        pyarrow.Table
+        year: int64
+        n_legs: int64
+        animals: string
+        ----
+        year: [[2020,2019]]
+        n_legs: [[2,5]]
+        animals: [["Flamingo","Brittle stars"]]
+
         Define a mask and select rows:
 
         >>> mask=[True, True, False, None]
         >>> table.filter(mask)
         pyarrow.Table
         year: int64
         n_legs: int64
@@ -2928,15 +2945,19 @@
         n_legs: int64
         animals: string
         ----
         year: [[2020,2022,null]]
         n_legs: [[2,4,null]]
         animals: [["Flamingo","Horse",null]]
         """
-        return _pc().filter(self, mask, null_selection_behavior)
+        if isinstance(mask, _pc().Expression):
+            return _pc()._exec_plan._filter_table(self, mask,
+                                                  output_type=Table)
+        else:
+            return _pc().filter(self, mask, null_selection_behavior)
 
     def take(self, object indices):
         """
         Select rows from the table.
 
         See :func:`pyarrow.compute.take` for full usage.
 
@@ -3298,15 +3319,15 @@
 
         Returns
         -------
         bool
 
         Examples
         --------
-        >>> import pyarrow as pa  
+        >>> import pyarrow as pa
         >>> n_legs = pa.array([2, 2, 4, 4, 5, 100])
         >>> animals = pa.array(["Flamingo", "Parrot", "Dog", "Horse", "Brittle stars", "Centipede"])
         >>> names=["n_legs", "animals"]
         >>> table = pa.Table.from_arrays([n_legs, animals], names=names)
         >>> table_0 = pa.Table.from_arrays([])
         >>> table_1 = pa.Table.from_arrays([n_legs, animals],
         ...                                 names=names,
@@ -3329,24 +3350,26 @@
             c_bool result
 
         with nogil:
             result = this_table.Equals(deref(other_table), check_metadata)
 
         return result
 
-    def cast(self, Schema target_schema, bint safe=True):
+    def cast(self, Schema target_schema, safe=None, options=None):
         """
         Cast table values to another schema.
 
         Parameters
         ----------
         target_schema : Schema
             Schema to cast to, the names and order of fields must match.
         safe : bool, default True
             Check for overflows or other unsafe conversions.
+        options : CastOptions, default None
+            Additional checks pass by CastOptions
 
         Returns
         -------
         Table
 
         Examples
         --------
@@ -3355,15 +3378,15 @@
         >>> df = pd.DataFrame({'n_legs': [2, 4, 5, 100],
         ...                    'animals': ["Flamingo", "Horse", "Brittle stars", "Centipede"]})
         >>> table = pa.Table.from_pandas(df)
         >>> table.schema
         n_legs: int64
         animals: string
         -- schema metadata --
-        pandas: '{"index_columns": [{"kind": "range", "name": null, "start": 0, "' + 509
+        pandas: '{"index_columns": [{"kind": "range", "name": null, "start": 0, ...
 
         Define new schema and cast table values:
 
         >>> my_schema = pa.schema([
         ...     pa.field('n_legs', pa.duration('s')),
         ...     pa.field('animals', pa.string())]
         ...     )
@@ -3382,15 +3405,15 @@
 
         if self.schema.names != target_schema.names:
             raise ValueError("Target schema's field names are not matching "
                              "the table's field names: {!r}, {!r}"
                              .format(self.schema.names, target_schema.names))
 
         for column, field in zip(self.itercolumns(), target_schema):
-            casted = column.cast(field.type, safe=safe)
+            casted = column.cast(field.type, safe=safe, options=options)
             newcols.append(casted)
 
         return Table.from_arrays(newcols, schema=target_schema)
 
     @classmethod
     def from_pandas(cls, df, Schema schema=None, preserve_index=None,
                     nthreads=None, columns=None, bint safe=True):
@@ -3701,14 +3724,15 @@
         Table
 
         Examples
         --------
         >>> import pyarrow as pa
         >>> n_legs = pa.array([2, 4, 5, 100])
         >>> animals = pa.array(["Flamingo", "Horse", "Brittle stars", "Centipede"])
+        >>> names = ["n_legs", "animals"]
         >>> batch = pa.record_batch([n_legs, animals], names=names)
         >>> batch.to_pandas()
            n_legs        animals
         0       2       Flamingo
         1       4          Horse
         2       5  Brittle stars
         3     100      Centipede
@@ -3855,15 +3879,15 @@
         <pyarrow.lib.RecordBatchReader object at ...>
 
         >>> reader = table.to_reader()
         >>> reader.schema
         n_legs: int64
         animals: string
         -- schema metadata --
-        pandas: '{"index_columns": [{"kind": "range", "name": null, "start": 0, "' + 509
+        pandas: '{"index_columns": [{"kind": "range", "name": null, "start": 0, ...
         >>> reader.read_all()
         pyarrow.Table
         n_legs: int64
         animals: string
         ----
         n_legs: [[2,4,5,100]]
         animals: [["Flamingo","Horse","Brittle stars","Centipede"]]
@@ -4098,15 +4122,15 @@
         >>> import pyarrow as pa
         >>> import pandas as pd
         >>> df = pd.DataFrame({'n_legs': [None, 4, 5, None],
         ...                    'animals': ["Flamingo", "Horse", None, "Centipede"]})
         >>> table = pa.Table.from_pandas(df)
         >>> for i in table.itercolumns():
         ...     print(i.null_count)
-        ... 
+        ...
         2
         1
         """
         for i in range(self.num_columns):
             yield self._column(i)
 
     @property
@@ -4603,14 +4627,97 @@
 
         table = self
         for idx in indices:
             table = table.remove_column(idx)
 
         return table
 
+    def group_by(self, keys):
+        """Declare a grouping over the columns of the table.
+
+        Resulting grouping can then be used to perform aggregations
+        with a subsequent ``aggregate()`` method.
+
+        Parameters
+        ----------
+        keys : str or list[str]
+            Name of the columns that should be used as the grouping key.
+
+        Returns
+        -------
+        TableGroupBy
+
+        See Also
+        --------
+        TableGroupBy.aggregate
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> import pyarrow as pa
+        >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
+        ...                    'n_legs': [2, 2, 4, 4, 5, 100],
+        ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
+        ...                    "Brittle stars", "Centipede"]})
+        >>> table = pa.Table.from_pandas(df)
+        >>> table.group_by('year').aggregate([('n_legs', 'sum')])
+        pyarrow.Table
+        n_legs_sum: int64
+        year: int64
+        ----
+        n_legs_sum: [[2,6,104,5]]
+        year: [[2020,2022,2021,2019]]
+        """
+        return TableGroupBy(self, keys)
+
+    def sort_by(self, sorting):
+        """
+        Sort the table by one or multiple columns.
+
+        Parameters
+        ----------
+        sorting : str or list[tuple(name, order)]
+            Name of the column to use to sort (ascending), or
+            a list of multiple sorting conditions where
+            each entry is a tuple with column name
+            and sorting order ("ascending" or "descending")
+
+        Returns
+        -------
+        Table
+            A new table sorted according to the sort keys.
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> import pyarrow as pa
+        >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
+        ...                    'n_legs': [2, 2, 4, 4, 5, 100],
+        ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
+        ...                    "Brittle stars", "Centipede"]})
+        >>> table = pa.Table.from_pandas(df)
+        >>> table.sort_by('animal')
+        pyarrow.Table
+        year: int64
+        n_legs: int64
+        animal: string
+        ----
+        year: [[2019,2021,2021,2020,2022,2022]]
+        n_legs: [[5,100,4,2,4,2]]
+        animal: [["Brittle stars","Centipede","Dog","Flamingo","Horse","Parrot"]]
+        """
+        if isinstance(sorting, str):
+            sorting = [(sorting, "ascending")]
+
+        indices = _pc().sort_indices(
+            self,
+            sort_keys=sorting
+        )
+        return self.take(indices)
+
     def join(self, right_table, keys, right_keys=None, join_type="left outer",
              left_suffix=None, right_suffix=None, coalesce_keys=True,
              use_threads=True):
         """
         Perform a join between this table and another one.
 
         Result of the join will be a new Table, where further
@@ -4622,15 +4729,15 @@
             The table to join to the current one, acting as the right table
             in the join operation.
         keys : str or list[str]
             The columns from current table that should be used as keys
             of the join operation left side.
         right_keys : str or list[str], default None
             The columns from the right_table that should be used as keys
-            on the join operation right side. 
+            on the join operation right side.
             When ``None`` use the same key names as the left table.
         join_type : str, default "left outer"
             The kind of join that should be performed, one of
             ("left semi", "right semi", "left anti", "right anti",
             "inner", "left outer", "right outer", "full outer")
         left_suffix : str, default None
             Which suffix to add to right column names. This prevents confusion
@@ -4658,53 +4765,53 @@
         ...                     'n_legs': [5, 100],
         ...                     'animal': ["Brittle stars", "Centipede"]})
         >>> t1 = pa.Table.from_pandas(df1)
         >>> t2 = pa.Table.from_pandas(df2)
 
         Left outer join:
 
-        >>> t1.join(t2, 'id')
+        >>> t1.join(t2, 'id').combine_chunks().sort_by('year')
         pyarrow.Table
         id: int64
         year: int64
         n_legs: int64
         animal: string
         ----
         id: [[3,1,2]]
         year: [[2019,2020,2022]]
         n_legs: [[5,null,null]]
         animal: [["Brittle stars",null,null]]
 
         Full outer join:
 
-        >>> t1.join(t2, 'id', join_type="full outer")
+        >>> t1.join(t2, 'id', join_type="full outer").combine_chunks().sort_by('year')
         pyarrow.Table
         id: int64
         year: int64
         n_legs: int64
         animal: string
         ----
-        id: [[3,1,2],[4]]
-        year: [[2019,2020,2022],[null]]
-        n_legs: [[5,null,null],[100]]
-        animal: [["Brittle stars",null,null],["Centipede"]]
+        id: [[3,1,2,4]]
+        year: [[2019,2020,2022,null]]
+        n_legs: [[5,null,null,100]]
+        animal: [["Brittle stars",null,null,"Centipede"]]
 
         Right outer join:
 
-        >>> t1.join(t2, 'id', join_type="right outer")
+        >>> t1.join(t2, 'id', join_type="right outer").combine_chunks().sort_by('year')
         pyarrow.Table
         year: int64
         id: int64
         n_legs: int64
         animal: string
         ----
-        year: [[2019],[null]]
-        id: [[3],[4]]
-        n_legs: [[5],[100]]
-        animal: [["Brittle stars"],["Centipede"]]
+        year: [[2019,null]]
+        id: [[3,4]]
+        n_legs: [[5,100]]
+        animal: [["Brittle stars","Centipede"]]
 
         Right anti join
 
         >>> t1.join(t2, 'id', join_type="right anti")
         pyarrow.Table
         id: int64
         n_legs: int64
@@ -4717,97 +4824,14 @@
         if right_keys is None:
             right_keys = keys
         return _pc()._exec_plan._perform_join(join_type, self, keys, right_table, right_keys,
                                               left_suffix=left_suffix, right_suffix=right_suffix,
                                               use_threads=use_threads, coalesce_keys=coalesce_keys,
                                               output_type=Table)
 
-    def group_by(self, keys):
-        """Declare a grouping over the columns of the table.
-
-        Resulting grouping can then be used to perform aggregations
-        with a subsequent ``aggregate()`` method.
-
-        Parameters
-        ----------
-        keys : str or list[str]
-            Name of the columns that should be used as the grouping key.
-
-        Returns
-        -------
-        TableGroupBy
-
-        See Also
-        --------
-        TableGroupBy.aggregate
-
-        Examples
-        --------
-        >>> import pandas as pd
-        >>> import pyarrow as pa
-        >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
-        ...                    'n_legs': [2, 2, 4, 4, 5, 100],
-        ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
-        ...                    "Brittle stars", "Centipede"]})
-        >>> table = pa.Table.from_pandas(df)
-        >>> table.group_by('year').aggregate([('n_legs', 'sum')])
-        pyarrow.Table
-        n_legs_sum: int64
-        year: int64
-        ----
-        n_legs_sum: [[2,6,104,5]]
-        year: [[2020,2022,2021,2019]]
-        """
-        return TableGroupBy(self, keys)
-
-    def sort_by(self, sorting):
-        """
-        Sort the table by one or multiple columns.
-
-        Parameters
-        ----------
-        sorting : str or list[tuple(name, order)]
-            Name of the column to use to sort (ascending), or
-            a list of multiple sorting conditions where
-            each entry is a tuple with column name
-            and sorting order ("ascending" or "descending")
-
-        Returns
-        -------
-        Table
-            A new table sorted according to the sort keys.
-
-        Examples
-        --------
-        >>> import pandas as pd
-        >>> import pyarrow as pa
-        >>> df = pd.DataFrame({'year': [2020, 2022, 2021, 2022, 2019, 2021],
-        ...                    'n_legs': [2, 2, 4, 4, 5, 100],
-        ...                    'animal': ["Flamingo", "Parrot", "Dog", "Horse",
-        ...                    "Brittle stars", "Centipede"]})
-        >>> table = pa.Table.from_pandas(df)
-        >>> table.sort_by('animal')
-        pyarrow.Table
-        year: int64
-        n_legs: int64
-        animal: string
-        ----
-        year: [[2019,2021,2021,2020,2022,2022]]
-        n_legs: [[5,100,4,2,4,2]]
-        animal: [["Brittle stars","Centipede","Dog","Flamingo","Horse","Parrot"]]
-        """
-        if isinstance(sorting, str):
-            sorting = [(sorting, "ascending")]
-
-        indices = _pc().sort_indices(
-            self,
-            sort_keys=sorting
-        )
-        return self.take(indices)
-
 
 def _reconstruct_table(arrays, schema):
     """
     Internal: reconstruct pa.Table from pickled components.
     """
     return Table.from_arrays(arrays, schema=schema)
 
@@ -5267,14 +5291,15 @@
         Returns
         -------
         Table
             Results of the aggregation functions.
 
         Examples
         --------
+        >>> import pyarrow as pa
         >>> t = pa.table([
         ...       pa.array(["a", "a", "b", "b", "c"]),
         ...       pa.array([1, 2, 3, 4, 5]),
         ... ], names=["keys", "values"])
         >>> t.group_by("keys").aggregate([("values", "sum")])
         pyarrow.Table
         values_sum: int64
```

### Comparing `pyarrow-8.0.0/pyarrow/tensor.pxi` & `pyarrow-9.0.0/pyarrow/tensor.pxi`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tensorflow/plasma_op.cc` & `pyarrow-9.0.0/pyarrow/tensorflow/plasma_op.cc`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/arrow_7980.py` & `pyarrow-9.0.0/pyarrow/tests/arrow_7980.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/bound_function_visit_strings.pyx` & `pyarrow-9.0.0/pyarrow/tests/bound_function_visit_strings.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/feather/v0.17.0.version.2-compression.lz4.feather` & `pyarrow-9.0.0/pyarrow/tests/data/feather/v0.17.0.version.2-compression.lz4.feather`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/README.md` & `pyarrow-9.0.0/pyarrow/tests/data/orc/README.md`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.orc` & `pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.emptyFile.orc`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.orc` & `pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.test1.orc`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.jsn.gz` & `pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.jsn.gz`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.orc` & `pyarrow-9.0.0/pyarrow/tests/data/orc/TestOrcFile.testDate1900.orc`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/decimal.jsn.gz` & `pyarrow-9.0.0/pyarrow/tests/data/orc/decimal.jsn.gz`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/orc/decimal.orc` & `pyarrow-9.0.0/pyarrow/tests/data/orc/decimal.orc`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.all-named-index.parquet` & `pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.all-named-index.parquet`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.column-metadata-handling.parquet` & `pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.column-metadata-handling.parquet`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.parquet` & `pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.parquet`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/data/parquet/v0.7.1.some-named-index.parquet` & `pyarrow-9.0.0/pyarrow/tests/data/parquet/v0.7.1.some-named-index.parquet`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/deserialize_buffer.py` & `pyarrow-9.0.0/pyarrow/tests/deserialize_buffer.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/pandas_examples.py` & `pyarrow-9.0.0/pyarrow/tests/pandas_examples.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/pandas_threaded_import.py` & `pyarrow-9.0.0/pyarrow/tests/pandas_threaded_import.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/__init__.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 import pytest
 
 # Marks all of the tests in this module
 # Ignore these with pytest ... -m 'not parquet'
 pytestmark = [
     pytest.mark.parquet,
     pytest.mark.filterwarnings(
-        "ignore:Passing 'use_legacy_dataset=True':DeprecationWarning"
+        "ignore:Passing 'use_legacy_dataset=True':FutureWarning"
     ),
 ]
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/common.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,14 @@
 )
 parametrize_legacy_dataset_fixed = pytest.mark.parametrize(
     "use_legacy_dataset",
     [pytest.param(True, marks=[pytest.mark.xfail, legacy_filter_mark]),
      pytest.param(False, marks=pytest.mark.dataset)]
 )
 
-# Marks all of the tests in this module
-# Ignore these with pytest ... -m 'not parquet'
-pytestmark = pytest.mark.parquet
-
 
 def _write_table(table, path, **kwargs):
     # So we see the ImportError somewhere
     import pyarrow.parquet as pq
     from pyarrow.pandas_compat import _pandas_api
 
     if _pandas_api.is_data_frame(table):
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/conftest.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/conftest.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/encryption.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/encryption.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_basic.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 
     from pyarrow.tests.pandas_examples import dataframe_with_lists
     from pyarrow.tests.parquet.common import alltypes_sample
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 def test_parquet_invalid_version(tempdir):
     table = pa.table({'a': [1, 2, 3]})
     with pytest.raises(ValueError, match="Unsupported Parquet format version"):
         _write_table(table, tempdir / 'test_version.parquet', version="2.2")
     with pytest.raises(ValueError, match="Unsupported Parquet data page " +
                        "version"):
         _write_table(table, tempdir / 'test_version.parquet',
@@ -793,7 +798,34 @@
     path = tempdir / 'data.parquet'
     pq.write_table(table, path)
 
     with pytest.warns(
         FutureWarning, match="Passing 'use_legacy_dataset=True'"
     ):
         pq.read_table(path, use_legacy_dataset=True)
+
+
+def test_thrift_size_limits(tempdir):
+    path = tempdir / 'largethrift.parquet'
+
+    array = pa.array(list(range(10)))
+    num_cols = 1000
+    table = pa.table(
+        [array] * num_cols,
+        names=[f'some_long_column_name_{i}' for i in range(num_cols)])
+    pq.write_table(table, path)
+
+    with pytest.raises(
+            OSError,
+            match="Couldn't deserialize thrift:.*Exceeded size limit"):
+        pq.read_table(path, thrift_string_size_limit=50 * num_cols)
+    with pytest.raises(
+            OSError,
+            match="Couldn't deserialize thrift:.*Exceeded size limit"):
+        pq.read_table(path, thrift_container_size_limit=num_cols)
+
+    got = pq.read_table(path, thrift_string_size_limit=100 * num_cols)
+    assert got == table
+    got = pq.read_table(path, thrift_container_size_limit=2 * num_cols)
+    assert got == table
+    got = pq.read_table(path)
+    assert got == table
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_compliant_nested_type.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_compliant_nested_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     import pandas.testing as tm
 
     from pyarrow.tests.parquet.common import _roundtrip_pandas_dataframe
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 # Tests for ARROW-11497
 _test_data_simple = [
     {'items': [1, 2]},
     {'items': [0]},
 ]
 
 _test_data_complex = [
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_data_types.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     from pyarrow.tests.pandas_examples import (dataframe_with_arrays,
                                                dataframe_with_lists)
     from pyarrow.tests.parquet.common import alltypes_sample
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 # General roundtrip of data types
 # -----------------------------------------------------------------------------
 
 
 @pytest.mark.pandas
 @parametrize_legacy_dataset
 @pytest.mark.parametrize('chunk_size', [None, 1000])
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_dataset.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import datetime
 import os
+import pathlib
 
 import numpy as np
 import pytest
 
 import pyarrow as pa
 from pyarrow import fs
 from pyarrow.filesystem import LocalFileSystem
@@ -43,14 +44,19 @@
     import pandas as pd
     import pandas.testing as tm
 
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 def test_parquet_piece_read(tempdir):
     df = _test_dataframe(1000)
     table = pa.Table.from_pandas(df)
 
     path = tempdir / 'parquet_piece_read.parquet'
     _write_table(table, path, version='2.6')
@@ -876,14 +882,16 @@
     # read single file using filter
     table = pq.read_table(tempdir, filters=[[('A', '==', 0)]],
                           use_legacy_dataset=use_legacy_dataset)
     assert table.column('B').equals(pa.chunked_array([[1, 2, 3]]))
 
 
 @pytest.mark.pandas
+@pytest.mark.filterwarnings(
+    "ignore:Specifying the 'metadata':FutureWarning")
 @parametrize_legacy_dataset
 def test_read_multiple_files(tempdir, use_legacy_dataset):
     nfiles = 10
     size = 5
 
     dirpath = tempdir / guid()
     dirpath.mkdir()
@@ -1407,15 +1415,17 @@
 ):
     fs, path = s3_example_s3fs
 
     _test_write_to_dataset_no_partitions(
         path, use_legacy_dataset, filesystem=fs)
 
 
-@pytest.mark.filterwarnings("ignore:'ParquetDataset:FutureWarning")
+@pytest.mark.filterwarnings(
+    "ignore:'ParquetDataset:FutureWarning",
+    "ignore:'partition_filename_cb':FutureWarning")
 @pytest.mark.pandas
 @parametrize_legacy_dataset_not_supported
 def test_write_to_dataset_with_partitions_and_custom_filenames(
     tempdir, use_legacy_dataset
 ):
     output_df = pd.DataFrame({'group1': list('aaabbbbccc'),
                               'group2': list('eefeffgeee'),
@@ -1534,15 +1544,16 @@
     df = pd.DataFrame({
         'one': [-1, 10, 2.5, 100, 1000, 1, 29.2],
         'two': [-1, 10, 2, 100, 1000, 1, 11],
         'three': [0, 0, 0, 0, 0, 0, 0]
     })
     table = pa.Table.from_pandas(df)
     pq.write_to_dataset(table, root_path=str(path),
-                        partition_cols=['one', 'two'])
+                        partition_cols=['one', 'two'],
+                        use_legacy_dataset=use_legacy_dataset)
     table = pq.ParquetDataset(
         path, use_legacy_dataset=use_legacy_dataset).read()
     pq.write_table(table, path / "output.parquet")
 
 
 @pytest.mark.pandas
 @parametrize_legacy_dataset
@@ -1775,10 +1786,87 @@
     with pytest.raises(ValueError, match="use_threads"):
         pq.write_to_dataset(table, path, use_legacy_dataset=True,
                             use_threads=False)
 
     with pytest.raises(ValueError, match="file_visitor"):
         pq.write_to_dataset(table, path, use_legacy_dataset=True,
                             file_visitor=lambda x: x)
+
     with pytest.raises(ValueError, match="existing_data_behavior"):
         pq.write_to_dataset(table, path, use_legacy_dataset=True,
                             existing_data_behavior='error')
+
+    with pytest.raises(ValueError, match="basename_template"):
+        pq.write_to_dataset(table, path, use_legacy_dataset=True,
+                            basename_template='part-{i}.parquet')
+
+
+@pytest.mark.dataset
+def test_parquet_write_to_dataset_exposed_keywords(tempdir):
+    table = pa.table({'a': [1, 2, 3]})
+    path = tempdir / 'partitioning'
+
+    paths_written = []
+
+    def file_visitor(written_file):
+        paths_written.append(written_file.path)
+
+    basename_template = 'part-{i}.parquet'
+
+    pq.write_to_dataset(table, path, partitioning=["a"],
+                        file_visitor=file_visitor,
+                        basename_template=basename_template,
+                        use_legacy_dataset=False)
+
+    expected_paths = {
+        path / '1' / 'part-0.parquet',
+        path / '2' / 'part-0.parquet',
+        path / '3' / 'part-0.parquet'
+    }
+    paths_written_set = set(map(pathlib.Path, paths_written))
+    assert paths_written_set == expected_paths
+
+
+@pytest.mark.dataset
+def test_write_to_dataset_conflicting_keywords(tempdir):
+    table = pa.table({'a': [1, 2, 3]})
+    path = tempdir / 'data.parquet'
+
+    with pytest.raises(ValueError, match="'basename_template' argument "
+                       "is not supported by use_legacy_dataset=True"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=True,
+                            partition_filename_cb=lambda x: 'filename.parquet',
+                            basename_template='file-{i}.parquet')
+    with pytest.raises(ValueError, match="'partition_filename_cb' argument "
+                       "is not supported by use_legacy_dataset=False"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=False,
+                            partition_filename_cb=lambda x: 'filename.parquet',
+                            basename_template='file-{i}.parquet')
+
+    with pytest.raises(ValueError, match="'partitioning' argument "
+                       "is not supported by use_legacy_dataset=True"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=True,
+                            partition_cols=["a"],
+                            partitioning=["a"])
+
+    with pytest.raises(ValueError, match="'partition_cols' argument "
+                       "is not supported by use_legacy_dataset=False"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=False,
+                            partition_cols=["a"],
+                            partitioning=["a"])
+
+    with pytest.raises(ValueError, match="'file_visitor' argument "
+                       "is not supported by use_legacy_dataset=True"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=True,
+                            metadata_collector=[],
+                            file_visitor=lambda x: x)
+    with pytest.raises(ValueError, match="'metadata_collector' argument "
+                       "is not supported by use_legacy_dataset=False"):
+        pq.write_to_dataset(table, path,
+                            use_legacy_dataset=False,
+                            metadata_collector=[],
+                            file_visitor=lambda x: x)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_datetime.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,19 @@
     import pandas.testing as tm
 
     from pyarrow.tests.parquet.common import _roundtrip_pandas_dataframe
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 @parametrize_legacy_dataset
 def test_pandas_parquet_datetime_tz(use_legacy_dataset):
     s = pd.Series([datetime.datetime(2017, 9, 6)])
     s = s.dt.tz_localize('utc')
 
     s.index = s
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_encryption.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 FOOTER_KEY_NAME = "footer_key"
 COL_KEY = b"1234567890123450"
 COL_KEY_NAME = "col_key"
 
 
 # Marks all of the tests in this module
 # Ignore these with pytest ... -m 'not parquet_encryption'
-pytestmark = pytest.mark.parquet_encryption
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = [
+    pytest.mark.parquet_encryption,
+    pytest.mark.parquet
+]
 
 
 @pytest.fixture(scope='module')
 def data_table():
     data_table = pa.Table.from_pydict({
         'a': pa.array([1, 2, 3]),
         'b': pa.array(['a', 'b', 'c']),
@@ -122,15 +126,15 @@
     assert(meta.num_columns == 3)
     schema = pq.read_schema(
         path, decryption_properties=file_decryption_properties)
     assert(len(schema.names) == 3)
 
     result = pq.ParquetFile(
         path, decryption_properties=file_decryption_properties)
-    return result.read(use_threads=False)
+    return result.read(use_threads=True)
 
 
 def test_encrypted_parquet_write_read_wrong_key(tempdir, data_table):
     """Write an encrypted parquet, verify it's encrypted,
     and then read it using wrong keys."""
     path = tempdir / PARQUET_NAME
 
@@ -482,16 +486,14 @@
 
     crypto_factory = pe.CryptoFactory(kms_factory)
     # Write with encryption properties
     write_encrypted_parquet(path, data_table, encryption_config,
                             kms_connection_config, crypto_factory)
 
 
-@pytest.mark.skip(reason="ARROW-14114: Multithreaded read sometimes fails"
-                  "decryption finalization or with Segmentation fault")
 def test_encrypted_parquet_loop(tempdir, data_table, basic_encryption_config):
     """Write an encrypted parquet, verify it's encrypted,
     and then read it multithreaded in a loop."""
     path = tempdir / PARQUET_NAME
 
     # Encrypt the footer with the footer key,
     # encrypt column `a` and column `b` with another key,
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_metadata.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,19 @@
     import pandas.testing as tm
 
     from pyarrow.tests.parquet.common import alltypes_sample
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 def test_parquet_metadata_api():
     df = alltypes_sample(size=10000)
     df = df.reindex(columns=sorted(df.columns))
     df.index = np.random.randint(0, 1000000, size=len(df))
 
     fileh = make_sample_file(df)
@@ -522,7 +527,19 @@
         metadata.append_row_groups(original_metadata)
 
     with pa.BufferOutputStream() as out:
         metadata.write_metadata_file(out)
         buf = out.getvalue()
 
     metadata = pq.read_metadata(pa.BufferReader(buf))
+
+
+def test_metadata_equals():
+    table = pa.table({"a": [1, 2, 3]})
+    with pa.BufferOutputStream() as out:
+        pq.write_table(table, out)
+        buf = out.getvalue()
+
+    original_metadata = pq.read_metadata(pa.BufferReader(buf))
+    match = "Argument 'other' has incorrect type"
+    with pytest.raises(TypeError, match=match):
+        original_metadata.equals(None)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_pandas.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 
     from pyarrow.tests.parquet.common import (_roundtrip_pandas_dataframe,
                                               alltypes_sample)
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 def test_pandas_parquet_custom_metadata(tempdir):
     df = alltypes_sample(size=10000)
 
     filename = tempdir / 'pandas_roundtrip.parquet'
     arrow_table = pa.Table.from_pandas(df)
     assert b'pandas' in arrow_table.schema.metadata
@@ -247,15 +252,15 @@
         'bool': np.random.randn(size) > 0,
         'strings': ['foo', 'bar', None, 'baz', 'qux']
     })
 
     arrow_table = pa.Table.from_pandas(df)
 
     with filename.open('wb') as f:
-        _write_table(arrow_table, f, version="1.0")
+        _write_table(arrow_table, f, version="2.4")
 
     data = io.BytesIO(filename.read_bytes())
 
     table_read = _read_table(data, use_legacy_dataset=use_legacy_dataset)
     df_read = table_read.to_pandas()
     tm.assert_frame_equal(df, df_read)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_parquet_file.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_parquet_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     import pandas.testing as tm
 
     from pyarrow.tests.parquet.common import alltypes_sample
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 def test_pass_separate_metadata():
     # ARROW-471
     df = alltypes_sample(size=10000)
 
     a_table = pa.Table.from_pandas(df)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/parquet/test_parquet_writer.py` & `pyarrow-9.0.0/pyarrow/tests/parquet/test_parquet_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     import pandas as pd
     import pandas.testing as tm
 
 except ImportError:
     pd = tm = None
 
 
+# Marks all of the tests in this module
+# Ignore these with pytest ... -m 'not parquet'
+pytestmark = pytest.mark.parquet
+
+
 @pytest.mark.pandas
 @parametrize_legacy_dataset
 def test_parquet_incremental_file_build(tempdir, use_legacy_dataset):
     df = _test_dataframe(100)
     df['unique_id'] = 0
 
     arrow_table = pa.Table.from_pandas(df, preserve_index=False)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/pyarrow_cython_example.pyx` & `pyarrow-9.0.0/pyarrow/tests/pyarrow_cython_example.pyx`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/read_record_batch.py` & `pyarrow-9.0.0/pyarrow/tests/read_record_batch.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/strategies.py` & `pyarrow-9.0.0/pyarrow/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_adhoc_memory_leak.py` & `pyarrow-9.0.0/pyarrow/tests/test_adhoc_memory_leak.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_array.py` & `pyarrow-9.0.0/pyarrow/tests/test_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1277,15 +1277,15 @@
             in_arr.cast(out_type)
 
 
 def test_cast_none():
     # ARROW-3735: Ensure that calling cast(None) doesn't segfault.
     arr = pa.array([1, 2, 3])
 
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         arr.cast(None)
 
 
 def test_cast_list_to_primitive():
     # ARROW-8070: cast segfaults on unsupported cast from list<binary> to utf8
     arr = pa.array([[1, 2], [3, 4]])
     with pytest.raises(NotImplementedError):
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_builder.py` & `pyarrow-9.0.0/pyarrow/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_cffi.py` & `pyarrow-9.0.0/pyarrow/tests/test_cffi.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_compute.py` & `pyarrow-9.0.0/pyarrow/tests/test_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,20 +143,23 @@
                                              pa.KeyValueMetadata({"b": "2"})]),
         pc.MapLookupOptions(pa.scalar(1), "first"),
         pc.MatchSubstringOptions("pattern"),
         pc.ModeOptions(),
         pc.NullOptions(),
         pc.PadOptions(5),
         pc.PartitionNthOptions(1, null_placement="at_start"),
+        pc.CumulativeSumOptions(start=0, skip_nulls=False),
         pc.QuantileOptions(),
-        pc.RandomOptions(10),
+        pc.RandomOptions(),
+        pc.RankOptions(sort_keys="ascending",
+                       null_placement="at_start", tiebreaker="max"),
         pc.ReplaceSliceOptions(0, 1, "a"),
         pc.ReplaceSubstringOptions("a", "b"),
         pc.RoundOptions(2, "towards_infinity"),
-        pc.RoundTemporalOptions(1, "second", True),
+        pc.RoundTemporalOptions(1, "second", week_starts_monday=True),
         pc.RoundToMultipleOptions(100, "towards_infinity"),
         pc.ScalarAggregateOptions(),
         pc.SelectKOptions(0, sort_keys=[("b", "ascending")]),
         pc.SetLookupOptions(pa.array([1])),
         pc.SliceOptions(0, 1, 1),
         pc.SortOptions([("dummy", "descending")], null_placement="at_start"),
         pc.SplitOptions(),
@@ -363,14 +366,20 @@
     mode = pc.mode(arr, skip_nulls=False)
     assert len(mode) == 0
     mode = pc.mode(arr, min_count=6)
     assert len(mode) == 0
     mode = pc.mode(arr, skip_nulls=False, min_count=5)
     assert len(mode) == 0
 
+    arr = pa.array([True, False])
+    mode = pc.mode(arr, n=2)
+    assert len(mode) == 2
+    assert mode[0].as_py() == {"mode": False, "count": 1}
+    assert mode[1].as_py() == {"mode": True, "count": 1}
+
 
 def test_mode_chunked_array():
     # ARROW-9917
     arr = pa.chunked_array([pa.array([1, 1, 3, 4, 3, 5], type='int64')])
     mode = pc.mode(arr)
     assert len(mode) == 1
     assert mode[0].as_py() == {"mode": 1, "count": 2}
@@ -724,39 +733,14 @@
             Whether to skip (ignore) nulls in the input.
             If False, any null in the input forces the output to null.
         options : pyarrow.compute.ElementWiseAggregateOptions, optional
             Alternative way of passing options.
         memory_pool : pyarrow.MemoryPool, optional
             If not passed, will allocate memory from the default memory pool.
         """)
-    # Nullary with options
-    assert pc.random.__doc__ == textwrap.dedent("""\
-        Generate numbers in the range [0, 1).
-
-        Generated values are uniformly-distributed, double-precision """ +
-                                                """in range [0, 1).
-        Length of generated data, algorithm and seed can be changed """ +
-                                                """via RandomOptions.
-
-        Parameters
-        ----------
-        length : int
-            Number of random values to generate.
-        initializer : int or str
-            How to initialize the underlying random generator.
-            If an integer is given, it is used as a seed.
-            If "system" is given, the random generator is initialized with
-            a system-specific source of (hopefully true) randomness.
-            Other values are invalid.
-        options : pyarrow.compute.RandomOptions, optional
-            Alternative way of passing options.
-        memory_pool : pyarrow.MemoryPool, optional
-            If not passed, will allocate memory from the default memory pool.
-        """)
-    # With custom examples
     assert pc.filter.__doc__ == textwrap.dedent("""\
         Filter with a boolean selection filter.
 
         The output is populated with values from the input at positions
         where the selection filter is non-zero.  Nulls in the selection filter
         are handled based on FilterOptions.
 
@@ -776,21 +760,21 @@
 
         Examples
         --------
         >>> import pyarrow as pa
         >>> arr = pa.array(["a", "b", "c", None, "e"])
         >>> mask = pa.array([True, False, None, False, True])
         >>> arr.filter(mask)
-        <pyarrow.lib.StringArray object at 0x7fa826df9200>
+        <pyarrow.lib.StringArray object at ...>
         [
           "a",
           "e"
         ]
         >>> arr.filter(mask, null_selection_behavior='emit_null')
-        <pyarrow.lib.StringArray object at 0x7fa826df9200>
+        <pyarrow.lib.StringArray object at ...>
         [
           "a",
           null,
           "e"
         ]
         """)
 
@@ -817,15 +801,15 @@
                         "null_replacement='', options=None, "
                         "memory_pool=None)")
     # Varargs without options
     sig = inspect.signature(pc.choose)
     assert str(sig) == "(indices, /, *values, memory_pool=None)"
     # Nullary with options
     sig = inspect.signature(pc.random)
-    assert str(sig) == ("(length, *, initializer='system', "
+    assert str(sig) == ("(n, *, initializer='system', "
                         "options=None, memory_pool=None)")
 
 
 # We use isprintable to find about codepoints that Python doesn't know, but
 # utf8proc does (or in a future version of Python the other way around).
 # These codepoints cannot be compared between Arrow and the Python
 # implementation.
@@ -1698,21 +1682,41 @@
 
     assert pc.xor(a, b) == pa.array([False, True, False, None])
 
     assert pc.invert(a) == pa.array([False, True, True, None])
 
 
 def test_cast():
+    arr = pa.array([1, 2, 3, 4], type='int64')
+    options = pc.CastOptions(pa.int8())
+
+    with pytest.raises(TypeError):
+        pc.cast(arr, target_type=None)
+
+    with pytest.raises(ValueError):
+        pc.cast(arr, 'int32', options=options)
+
+    with pytest.raises(ValueError):
+        pc.cast(arr, safe=True, options=options)
+
+    assert pc.cast(arr, options=options) == pa.array(
+        [1, 2, 3, 4], type='int8')
+
     arr = pa.array([2 ** 63 - 1], type='int64')
+    allow_overflow_options = pc.CastOptions(
+        pa.int32(), allow_int_overflow=True)
 
     with pytest.raises(pa.ArrowInvalid):
         pc.cast(arr, 'int32')
 
     assert pc.cast(arr, 'int32', safe=False) == pa.array([-1], type='int32')
 
+    assert pc.cast(arr, options=allow_overflow_options) == pa.array(
+        [-1], type='int32')
+
     arr = pa.array([datetime(2010, 1, 1), datetime(2015, 1, 1)])
     expected = pa.array([1262304000000, 1420070400000], type='timestamp[ms]')
     assert pc.cast(arr, 'timestamp[ms]') == expected
 
     arr = pa.array([[1, 2], [3, 4, 5]], type=pa.large_list(pa.int8()))
     expected = pa.array([["1", "2"], ["3", "4", "5"]],
                         type=pa.list_(pa.utf8()))
@@ -2033,14 +2037,22 @@
         "microsecond": "us",
         "millisecond": "L",
         "second": "s",
         "minute": "min",
         "hour": "H",
         "day": "D"
     }
+    greater_unit = {
+        "nanosecond": "us",
+        "microsecond": "ms",
+        "millisecond": "s",
+        "second": "min",
+        "minute": "H",
+        "hour": "d",
+    }
     ta = pa.array(ts)
 
     for value in values:
         frequency = str(value) + unit_shorthand[unit]
         options = pc.RoundTemporalOptions(value, unit)
 
         result = pc.ceil_temporal(ta, options=options).to_pandas()
@@ -2051,28 +2063,65 @@
         expected = ts.dt.floor(frequency)
         np.testing.assert_array_equal(result, expected)
 
         result = pc.round_temporal(ta, options=options).to_pandas()
         expected = ts.dt.round(frequency)
         np.testing.assert_array_equal(result, expected)
 
+        # Check rounding with calendar_based_origin=True.
+        # Note: rounding to month is not supported in Pandas so we can't
+        # approximate this functionallity and exclude unit == "day".
+        if unit != "day":
+            options = pc.RoundTemporalOptions(
+                value, unit, calendar_based_origin=True)
+            origin = ts.dt.floor(greater_unit[unit])
+
+            if ta.type.tz is None:
+                result = pc.ceil_temporal(ta, options=options).to_pandas()
+                expected = (ts - origin).dt.ceil(frequency) + origin
+                np.testing.assert_array_equal(result, expected)
+
+            result = pc.floor_temporal(ta, options=options).to_pandas()
+            expected = (ts - origin).dt.floor(frequency) + origin
+            np.testing.assert_array_equal(result, expected)
+
+            result = pc.round_temporal(ta, options=options).to_pandas()
+            expected = (ts - origin).dt.round(frequency) + origin
+            np.testing.assert_array_equal(result, expected)
+
         # Check RoundTemporalOptions partial defaults
         if unit == "day":
             result = pc.ceil_temporal(ta, multiple=value).to_pandas()
             expected = ts.dt.ceil(frequency)
             np.testing.assert_array_equal(result, expected)
 
             result = pc.floor_temporal(ta, multiple=value).to_pandas()
             expected = ts.dt.floor(frequency)
             np.testing.assert_array_equal(result, expected)
 
             result = pc.round_temporal(ta, multiple=value).to_pandas()
             expected = ts.dt.round(frequency)
             np.testing.assert_array_equal(result, expected)
 
+    # We naively test ceil_is_strictly_greater by adding time unit multiple
+    # to regular ceiled timestamp if it is equal to the original timestamp.
+    # This does not work if timestamp is zoned since our logic will not
+    # account for DST jumps.
+    if ta.type.tz is None:
+        options = pc.RoundTemporalOptions(
+            value, unit, ceil_is_strictly_greater=True)
+        result = pc.ceil_temporal(ta, options=options)
+        expected = ts.dt.ceil(frequency)
+
+        expected = np.where(
+            expected == ts,
+            expected + pd.Timedelta(value, unit_shorthand[unit]),
+            expected)
+        np.testing.assert_array_equal(result, expected)
+
     # Check RoundTemporalOptions defaults
     if unit == "day":
         frequency = "1D"
 
         result = pc.ceil_temporal(ta).to_pandas()
         expected = ts.dt.ceil(frequency)
         np.testing.assert_array_equal(result, expected)
@@ -2091,30 +2140,30 @@
                     reason="Timezone database is not available on Windows yet")
 @pytest.mark.parametrize('unit', ("nanosecond", "microsecond", "millisecond",
                                   "second", "minute", "hour", "day"))
 @pytest.mark.pandas
 def test_round_temporal(unit):
     from pyarrow.vendored.version import Version
 
-    if Version(pd.__version__) < Version('1.0.0') and \
-            unit in ("nanosecond", "microsecond"):
-        pytest.skip('Pandas < 1.0 rounds zoned small units differently.')
+    if Version(pd.__version__) < Version('1.0.0'):
+        pytest.skip('Pandas < 1.0 rounds differently.')
 
     values = (1, 2, 3, 4, 5, 6, 7, 10, 15, 24, 60, 250, 500, 750)
     timestamps = [
         "1923-07-07 08:52:35.203790336",
         "1931-03-17 10:45:00.641559040",
         "1932-06-16 01:16:42.911994368",
         "1941-05-27 11:46:43.822831872",
         "1943-12-14 07:32:05.424766464",
         "1954-04-12 04:31:50.699881472",
         "1966-02-12 17:41:28.693282560",
         "1967-02-26 05:56:46.922376960",
         "1975-11-01 10:55:37.016146432",
         "1982-01-21 18:43:44.517366784",
+        "1992-01-01 00:00:00.100000000",
         "1999-12-04 05:55:34.794991104",
         "2026-10-26 08:39:00.316686848"]
     ts = pd.Series([pd.Timestamp(x, unit="ns") for x in timestamps])
     _check_temporal_rounding(ts, values, unit)
 
     timezones = ["Asia/Kolkata", "America/New_York", "Etc/GMT-4", "Etc/GMT+4",
                  "Europe/Brussels", "Pacific/Marquesas", "US/Central", "UTC"]
@@ -2506,14 +2555,66 @@
     # not skipping nulls
     result = pc.max_element_wise(arr1, arr3, skip_nulls=False)
     assert result == pa.array([2, 3, None])
     result = pc.min_element_wise(arr1, arr3, skip_nulls=False)
     assert result == pa.array([1, 2, None])
 
 
+@pytest.mark.parametrize('start', (1.25, 10.5, -10.5))
+@pytest.mark.parametrize('skip_nulls', (True, False))
+def test_cumulative_sum(start, skip_nulls):
+    # Exact tests (e.g., integral types)
+    start_int = int(start)
+    starts = [start_int, pa.scalar(start_int, type=pa.int8()),
+              pa.scalar(start_int, type=pa.int64())]
+    for strt in starts:
+        arrays = [
+            pa.array([1, 2, 3]),
+            pa.array([0, None, 20, 30]),
+            pa.chunked_array([[0, None], [20, 30]])
+        ]
+        expected_arrays = [
+            pa.array([1, 3, 6]),
+            pa.array([0, None, 20, 50])
+            if skip_nulls else pa.array([0, None, None, None]),
+            pa.chunked_array([[0, None, 20, 50]])
+            if skip_nulls else pa.chunked_array([[0, None, None, None]])
+        ]
+        for i, arr in enumerate(arrays):
+            result = pc.cumulative_sum(arr, start=strt, skip_nulls=skip_nulls)
+            # Add `start` offset to expected array before comparing
+            expected = pc.add(expected_arrays[i], strt)
+            assert result.equals(expected)
+
+    starts = [start, pa.scalar(start, type=pa.float32()),
+              pa.scalar(start, type=pa.float64())]
+    for strt in starts:
+        arrays = [
+            pa.array([1.125, 2.25, 3.03125]),
+            pa.array([1, np.nan, 2, -3, 4, 5]),
+            pa.array([1, np.nan, None, 3, None, 5])
+        ]
+        expected_arrays = [
+            np.array([1.125, 3.375, 6.40625]),
+            np.array([1, np.nan, np.nan, np.nan, np.nan, np.nan]),
+            np.array([1, np.nan, None, np.nan, None, np.nan])
+            if skip_nulls else np.array([1, np.nan, None, None, None, None])
+        ]
+        for i, arr in enumerate(arrays):
+            result = pc.cumulative_sum(arr, start=strt, skip_nulls=skip_nulls)
+            # Add `start` offset to expected array before comparing
+            expected = pc.add(expected_arrays[i], strt)
+            np.testing.assert_array_almost_equal(result.to_numpy(
+                zero_copy_only=False), expected.to_numpy(zero_copy_only=False))
+
+    for strt in ['a', pa.scalar('arrow'), 1.1]:
+        with pytest.raises(pa.ArrowInvalid):
+            pc.cumulative_sum([1, 2, 3], start=strt)
+
+
 def test_make_struct():
     assert pc.make_struct(1, 'a').as_py() == {'0': 1, '1': 'a'}
 
     assert pc.make_struct(1, 'a', field_names=['i', 's']).as_py() == {
         'i': 1, 's': 'a'}
 
     assert pc.make_struct([1, 2, 3],
@@ -2641,14 +2742,64 @@
 
     with pytest.raises(TypeError,
                        match=r"initializer should be 'system', an integer, "
                              r"or a hashable object; got \[\]"):
         pc.random(100, initializer=[])
 
 
+@pytest.mark.parametrize(
+    "tiebreaker,expected_values",
+    [("min", [3, 1, 4, 6, 4, 6, 1]),
+     ("max", [3, 2, 5, 7, 5, 7, 2]),
+     ("first", [3, 1, 4, 6, 5, 7, 2]),
+     ("dense", [2, 1, 3, 4, 3, 4, 1])]
+)
+def test_rank_options_tiebreaker(tiebreaker, expected_values):
+    arr = pa.array([1.2, 0.0, 5.3, None, 5.3, None, 0.0])
+    rank_options = pc.RankOptions(sort_keys="ascending",
+                                  null_placement="at_end",
+                                  tiebreaker=tiebreaker)
+    result = pc.rank(arr, options=rank_options)
+    expected = pa.array(expected_values, type=pa.uint64())
+    assert result.equals(expected)
+
+
+def test_rank_options():
+    arr = pa.array([1.2, 0.0, 5.3, None, 5.3, None, 0.0])
+    expected = pa.array([3, 1, 4, 6, 5, 7, 2], type=pa.uint64())
+
+    # Ensure rank can be called without specifying options
+    result = pc.rank(arr)
+    assert result.equals(expected)
+
+    # Ensure default RankOptions
+    result = pc.rank(arr, options=pc.RankOptions())
+    assert result.equals(expected)
+
+    # Ensure sort_keys tuple usage
+    result = pc.rank(arr, options=pc.RankOptions(
+        sort_keys=[("b", "ascending")])
+    )
+    assert result.equals(expected)
+
+    result = pc.rank(arr, null_placement="at_start")
+    expected_at_start = pa.array([5, 3, 6, 1, 7, 2, 4], type=pa.uint64())
+    assert result.equals(expected_at_start)
+
+    result = pc.rank(arr, sort_keys="descending")
+    expected_descending = pa.array([3, 4, 1, 6, 2, 7, 5], type=pa.uint64())
+    assert result.equals(expected_descending)
+
+    with pytest.raises(ValueError,
+                       match=r'"NonExisting" is not a valid tiebreaker'):
+        pc.RankOptions(sort_keys="descending",
+                       null_placement="at_end",
+                       tiebreaker="NonExisting")
+
+
 def test_expression_serialization():
     a = pc.scalar(1)
     b = pc.scalar(1.1)
     c = pc.scalar(True)
     d = pc.scalar("string")
     e = pc.scalar(None)
     f = pc.scalar({'a': 1})
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_convert_builtin.py` & `pyarrow-9.0.0/pyarrow/tests/test_convert_builtin.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_csv.py` & `pyarrow-9.0.0/pyarrow/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_cuda.py` & `pyarrow-9.0.0/pyarrow/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_cuda_numba_interop.py` & `pyarrow-9.0.0/pyarrow/tests/test_cuda_numba_interop.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_cython.py` & `pyarrow-9.0.0/pyarrow/tests/test_cython.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 import pyarrow.tests.util as test_util
 
 
 here = os.path.dirname(os.path.abspath(__file__))
 test_ld_path = os.environ.get('PYARROW_TEST_LD_PATH', '')
 if os.name == 'posix':
     compiler_opts = ['-std=c++11']
+elif os.name == 'nt':
+    compiler_opts = ['-D_ENABLE_EXTENDED_ALIGNED_STORAGE']
 else:
     compiler_opts = []
 
 
 setup_template = """if 1:
     from setuptools import setup
     from Cython.Build import cythonize
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_dataset.py` & `pyarrow-9.0.0/pyarrow/tests/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,50 +578,50 @@
         pa.schema([
             pa.field('group', pa.int64()),
             pa.field('key', pa.float64())
         ])
     )
     assert len(partitioning.dictionaries) == 2
     assert all(x is None for x in partitioning.dictionaries)
-    expr = partitioning.parse('/3/3.14')
+    expr = partitioning.parse('/3/3.14/')
     assert isinstance(expr, ds.Expression)
 
     expected = (ds.field('group') == 3) & (ds.field('key') == 3.14)
     assert expr.equals(expected)
 
     with pytest.raises(pa.ArrowInvalid):
         partitioning.parse('/prefix/3/aaa')
 
-    expr = partitioning.parse('/3')
+    expr = partitioning.parse('/3/')
     expected = ds.field('group') == 3
     assert expr.equals(expected)
 
     partitioning = ds.HivePartitioning(
         pa.schema([
             pa.field('alpha', pa.int64()),
             pa.field('beta', pa.int64())
         ]),
         null_fallback='xyz'
     )
     assert len(partitioning.dictionaries) == 2
     assert all(x is None for x in partitioning.dictionaries)
-    expr = partitioning.parse('/alpha=0/beta=3')
+    expr = partitioning.parse('/alpha=0/beta=3/')
     expected = (
         (ds.field('alpha') == ds.scalar(0)) &
         (ds.field('beta') == ds.scalar(3))
     )
     assert expr.equals(expected)
 
-    expr = partitioning.parse('/alpha=xyz/beta=3')
+    expr = partitioning.parse('/alpha=xyz/beta=3/')
     expected = (
         (ds.field('alpha').is_null() & (ds.field('beta') == ds.scalar(3)))
     )
     assert expr.equals(expected)
 
-    for shouldfail in ['/alpha=one/beta=2', '/alpha=one', '/beta=two']:
+    for shouldfail in ['/alpha=one/beta=2/', '/alpha=one/', '/beta=two/']:
         with pytest.raises(pa.ArrowInvalid):
             partitioning.parse(shouldfail)
 
     partitioning = ds.FilenamePartitioning(
         pa.schema([
             pa.field('group', pa.int64()),
             pa.field('key', pa.float64())
@@ -658,14 +658,32 @@
         dictionaries={
             "key": pa.array(["first", "second", "third"]),
         })
     assert partitioning.dictionaries[0] is None
     assert partitioning.dictionaries[1].to_pylist() == [
         "first", "second", "third"]
 
+    # test partitioning roundtrip
+    table = pa.table([
+        pa.array(range(20)), pa.array(np.random.randn(20)),
+        pa.array(np.repeat(['a', 'b'], 10))],
+        names=["f1", "f2", "part"]
+    )
+    partitioning_schema = pa.schema([("part", pa.string())])
+    for klass in [ds.DirectoryPartitioning, ds.HivePartitioning,
+                  ds.FilenamePartitioning]:
+        with tempfile.TemporaryDirectory() as tempdir:
+            partitioning = klass(partitioning_schema)
+            ds.write_dataset(table, tempdir,
+                             format='ipc', partitioning=partitioning)
+            load_back = ds.dataset(tempdir, format='ipc',
+                                   partitioning=partitioning)
+            load_back_table = load_back.to_table()
+            assert load_back_table.equals(table)
+
 
 def test_expression_arithmetic_operators():
     dataset = ds.dataset(pa.table({'a': [1, 2, 3], 'b': [2, 2, 2]}))
     a = ds.field("a")
     b = ds.field("b")
     result = dataset.to_table(columns={
         "a+1": a + 1,
@@ -726,35 +744,44 @@
 @pytest.mark.parquet
 def test_parquet_scan_options():
     opts1 = ds.ParquetFragmentScanOptions()
     opts2 = ds.ParquetFragmentScanOptions(buffer_size=4096)
     opts3 = ds.ParquetFragmentScanOptions(
         buffer_size=2**13, use_buffered_stream=True)
     opts4 = ds.ParquetFragmentScanOptions(buffer_size=2**13, pre_buffer=True)
+    opts5 = ds.ParquetFragmentScanOptions(
+        thrift_string_size_limit=123456,
+        thrift_container_size_limit=987654,)
 
     assert opts1.use_buffered_stream is False
     assert opts1.buffer_size == 2**13
     assert opts1.pre_buffer is False
+    assert opts1.thrift_string_size_limit == 100_000_000  # default in C++
+    assert opts1.thrift_container_size_limit == 1_000_000  # default in C++
 
     assert opts2.use_buffered_stream is False
     assert opts2.buffer_size == 2**12
     assert opts2.pre_buffer is False
 
     assert opts3.use_buffered_stream is True
     assert opts3.buffer_size == 2**13
     assert opts3.pre_buffer is False
 
     assert opts4.use_buffered_stream is False
     assert opts4.buffer_size == 2**13
     assert opts4.pre_buffer is True
 
+    assert opts5.thrift_string_size_limit == 123456
+    assert opts5.thrift_container_size_limit == 987654
+
     assert opts1 == opts1
     assert opts1 != opts2
     assert opts2 != opts3
     assert opts3 != opts4
+    assert opts5 != opts1
 
 
 def test_file_format_pickling():
     formats = [
         ds.IpcFileFormat(),
         ds.CsvFileFormat(),
         ds.CsvFileFormat(pa.csv.ParseOptions(delimiter='\t',
@@ -773,14 +800,16 @@
         formats.extend([
             ds.ParquetFileFormat(),
             ds.ParquetFileFormat(dictionary_columns={'a'}),
             ds.ParquetFileFormat(use_buffered_stream=True),
             ds.ParquetFileFormat(
                 use_buffered_stream=True,
                 buffer_size=4096,
+                thrift_string_size_limit=123,
+                thrift_container_size_limit=456,
             ),
         ])
 
     for file_format in formats:
         assert pickle.loads(pickle.dumps(file_format)) == file_format
 
 
@@ -980,14 +1009,16 @@
     )
 
     return table, dataset
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments(tempdir, dataset_reader):
     table, dataset = _create_dataset_for_fragments(tempdir)
 
     # list fragments
     fragments = list(dataset.get_fragments())
     assert len(fragments) == 2
     f = fragments[0]
@@ -1028,14 +1059,16 @@
     dataset = ds.dataset(path, format="parquet", partitioning=part)
     fragments = dataset.get_fragments(filter=ds.field("part") >= 2)
     assert len(list(fragments)) == 1
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_reconstruct(tempdir, dataset_reader):
     table, dataset = _create_dataset_for_fragments(tempdir)
 
     def assert_yields_projected(fragment, row_slice,
                                 columns=None, filter=None):
         actual = fragment.to_table(
             schema=table.schema, columns=columns, filter=filter)
@@ -1090,14 +1123,16 @@
             fragment.path, fragment.filesystem,
             partition_expression=fragment.partition_expression)
         dataset_reader.to_table(new_fragment, filter=ds.field('part') == 'a')
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_row_groups(tempdir, dataset_reader):
     table, dataset = _create_dataset_for_fragments(tempdir, chunk_size=2)
 
     fragment = list(dataset.get_fragments())[0]
 
     # list and scan row group fragments
     row_group_fragments = list(fragment.split_by_row_group())
@@ -1156,14 +1191,16 @@
     result = dataset_reader.to_table(dataset, filter=ds.field("col1") == "a")
 
     assert (df.iloc[0] == result.to_pandas()).all().all()
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_ensure_metadata(tempdir, open_logging_fs):
     fs, assert_opens = open_logging_fs
     _, dataset = _create_dataset_for_fragments(
         tempdir, chunk_size=2, filesystem=fs
     )
     fragment = list(dataset.get_fragments())[0]
 
@@ -1272,14 +1309,16 @@
                         chunk_size=chunk_size)
 
     return table, ds.dataset(path, format="parquet", partitioning="hive")
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_parquet_fragment_statistics(tempdir):
     table, dataset = _create_dataset_all_types(tempdir)
 
     fragment = list(dataset.get_fragments())[0]
 
     import datetime
     def dt_s(x): return datetime.datetime(1970, 1, 1, 0, 0, x)
@@ -1339,14 +1378,16 @@
     fragments = list(dataset.get_fragments())[0].split_by_row_group()
     # Only row group is empty
     assert fragments[0].row_groups[0].statistics == {}
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_row_groups_predicate(tempdir):
     table, dataset = _create_dataset_for_fragments(tempdir, chunk_size=2)
 
     fragment = list(dataset.get_fragments())[0]
     assert fragment.partition_expression.equals(ds.field('part') == 'a')
 
     # predicate may reference a partition field not present in the
@@ -1363,14 +1404,16 @@
         fragment.split_by_row_group(filter=ds.field('part') == 'b',
                                     schema=dataset.schema))
     assert len(row_group_fragments) == 0
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_row_groups_reconstruct(tempdir, dataset_reader):
     table, dataset = _create_dataset_for_fragments(tempdir, chunk_size=2)
 
     fragment = list(dataset.get_fragments())[0]
     parquet_format = fragment.format
     row_group_fragments = list(fragment.split_by_row_group())
 
@@ -1405,14 +1448,16 @@
         row_groups={2})
     with pytest.raises(IndexError, match="references row group 2"):
         dataset_reader.to_table(new_fragment)
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_subset_ids(tempdir, open_logging_fs,
                                       dataset_reader):
     fs, assert_opens = open_logging_fs
     table, dataset = _create_dataset_for_fragments(tempdir, chunk_size=1,
                                                    filesystem=fs)
     fragment = list(dataset.get_fragments())[0]
 
@@ -1434,14 +1479,16 @@
     result = dataset_reader.to_table(subfrag, schema=dataset.schema)
     assert result.num_rows == 0
     assert result.equals(table[:0])
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_subset_filter(tempdir, open_logging_fs,
                                          dataset_reader):
     fs, assert_opens = open_logging_fs
     table, dataset = _create_dataset_for_fragments(tempdir, chunk_size=1,
                                                    filesystem=fs)
     fragment = list(dataset.get_fragments())[0]
 
@@ -1467,14 +1514,16 @@
     # passing schema to ensure filter on partition expression works
     subfrag = fragment.subset(ds.field("part") == "a", schema=dataset.schema)
     assert subfrag.num_row_groups == 4
 
 
 @pytest.mark.pandas
 @pytest.mark.parquet
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_fragments_parquet_subset_invalid(tempdir):
     _, dataset = _create_dataset_for_fragments(tempdir, chunk_size=1)
     fragment = list(dataset.get_fragments())[0]
 
     # passing none or both of filter / row_group_ids
     with pytest.raises(ValueError):
         fragment.subset(ds.field("f1") >= 1, row_group_ids=[1, 2])
@@ -1754,18 +1803,24 @@
     table = pa.table({'a': ['x', 'y', None], 'b': ['x', 'y', 'z']})
     part = ds.partitioning(
         pa.schema([pa.field('a', pa.string()), pa.field('b', pa.string())]))
     with pytest.raises(pa.ArrowInvalid):
         ds.write_dataset(table, tempdir, format='ipc', partitioning=part)
 
 
+def test_positional_keywords_raises(tempdir):
+    table = pa.table({'a': ['x', 'y', None], 'b': ['x', 'y', 'z']})
+    with pytest.raises(TypeError):
+        ds.write_dataset(table, tempdir, "basename-{i}.arrow")
+
+
 @pytest.mark.parquet
 @pytest.mark.pandas
 def test_read_partition_keys_only(tempdir):
-    BATCH_SIZE = 2 ** 17
+    BATCH_SIZE = 2 ** 15
     # This is a regression test for ARROW-15318 which saw issues
     # reading only the partition keys from files with batches larger
     # than the default batch size (e.g. so we need to return two chunks)
     table = pa.table({
         'key': pa.repeat(0, BATCH_SIZE + 1),
         'value': np.arange(BATCH_SIZE + 1)})
     pq.write_to_dataset(
@@ -2447,14 +2502,15 @@
 @pytest.mark.parquet
 def s3_example_simple(s3_server):
     from pyarrow.fs import FileSystem
 
     host, port, access_key, secret_key = s3_server['connection']
     uri = (
         "s3://{}:{}@mybucket/data.parquet?scheme=http&endpoint_override={}:{}"
+        "&allow_bucket_creation=True"
         .format(access_key, secret_key, host, port)
     )
 
     fs, path = FileSystem.from_uri(uri)
 
     fs.create_dir("mybucket")
     table = pa.table({'a': [1, 2, 3]})
@@ -2509,17 +2565,18 @@
 @pytest.mark.s3
 def test_open_dataset_from_s3_with_filesystem_uri(s3_server):
     from pyarrow.fs import FileSystem
 
     host, port, access_key, secret_key = s3_server['connection']
     bucket = 'theirbucket'
     path = 'nested/folder/data.parquet'
-    uri = "s3://{}:{}@{}/{}?scheme=http&endpoint_override={}:{}".format(
-        access_key, secret_key, bucket, path, host, port
-    )
+    uri = "s3://{}:{}@{}/{}?scheme=http&endpoint_override={}:{}"\
+        "&allow_bucket_creation=true".format(
+            access_key, secret_key, bucket, path, host, port
+        )
 
     fs, path = FileSystem.from_uri(uri)
     assert path == 'theirbucket/nested/folder/data.parquet'
 
     fs.create_dir(bucket)
 
     table = pa.table({'a': [1, 2, 3]})
@@ -2867,17 +2924,17 @@
     table = pa.table({'a': [1, 2, 3]})
     pq.write_table(table, fn)
 
     schema = pa.schema([('a', pa.null())])
     dataset = ds.dataset([str(fn)] * 100, schema=schema)
     assert dataset.schema.equals(schema)
     scanner = dataset_reader.scanner(dataset)
-    reader = scanner.to_reader()
     with pytest.raises(NotImplementedError,
                        match='Unsupported cast from int64 to null'):
+        reader = scanner.to_reader()
         reader.read_all()
 
 
 def test_ipc_format(tempdir, dataset_reader):
     table = pa.table({'a': pa.array([1, 2, 3], type="int8"),
                       'b': pa.array([.1, .2, .3], type="float64")})
 
@@ -3029,14 +3086,30 @@
     dataset = ds.dataset(path, format=ds.CsvFileFormat(
         read_options=pa.csv.ReadOptions(column_names=['foo'])))
     result = dataset_reader.to_table(dataset)
     assert result.equals(
         pa.table({'foo': pa.array(['skipped', 'col0', 'foo', 'bar'])}))
 
 
+def test_csv_format_options_generate_columns(tempdir, dataset_reader):
+    path = str(tempdir / 'test.csv')
+    with open(path, 'w') as sink:
+        sink.write('1,a,true,1\n')
+
+    dataset = ds.dataset(path, format=ds.CsvFileFormat(
+        read_options=pa.csv.ReadOptions(autogenerate_column_names=True)))
+    result = dataset_reader.to_table(dataset)
+    expected_column_names = ["f0", "f1", "f2", "f3"]
+    assert result.column_names == expected_column_names
+    assert result.equals(pa.table({'f0': pa.array([1]),
+                                   'f1': pa.array(["a"]),
+                                   'f2': pa.array([True]),
+                                   'f3': pa.array([1])}))
+
+
 def test_csv_fragment_options(tempdir, dataset_reader):
     path = str(tempdir / 'test.csv')
     with open(path, 'w') as sink:
         sink.write('col0\nfoo\nspam\nMYNULL\n')
     dataset = ds.dataset(path, format='csv')
     convert_options = pyarrow.csv.ConvertOptions(null_values=['MYNULL'],
                                                  strings_can_be_null=True)
@@ -3144,14 +3217,16 @@
     result = dataset.to_table()
     assert result.num_rows == 40
 
 
 @pytest.mark.parquet
 @pytest.mark.pandas  # write_to_dataset currently requires pandas
 @pytest.mark.parametrize('use_legacy_dataset', [False, True])
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_parquet_dataset_factory_roundtrip(tempdir, use_legacy_dataset):
     # Simple test to ensure we can roundtrip dataset to
     # _metadata/common_metadata and back.  A more complex test
     # using partitioning will have to wait for ARROW-13269.  The
     # above test (test_parquet_dataset_factory) will not work
     # when legacy is False as there is no "append" equivalent in
     # the new dataset until ARROW-12358
@@ -3489,14 +3564,16 @@
     assert actual_table.column('part').to_pylist(
     ) == table.column('part').to_pylist()
     assert actual_table.column('col').equals(table.column('col'))
 
 
 @pytest.mark.parquet
 @pytest.mark.pandas
+@pytest.mark.filterwarnings(
+    "ignore:Passing 'use_legacy_dataset=True':FutureWarning")
 def test_legacy_write_to_dataset_drops_null(tempdir):
     schema = pa.schema([
         pa.field('col', pa.int64()),
         pa.field('part', pa.dictionary(pa.int32(), pa.string()))
     ])
     table = pa.table({'part': ['a', 'a', None, None],
                       'col': list(range(4))}, schema=schema)
@@ -4079,25 +4156,29 @@
     base_dir = tempdir / 'partitioned'
     expected_paths = [
         base_dir / "part=a", base_dir / "part=a" / "dat_0.arrow",
         base_dir / "part=b", base_dir / "part=b" / "dat_0.arrow"
     ]
 
     visited_paths = []
+    visited_sizes = []
 
     def file_visitor(written_file):
         visited_paths.append(written_file.path)
+        visited_sizes.append(written_file.size)
 
     partitioning = ds.partitioning(
         pa.schema([("part", pa.string())]), flavor="hive")
     ds.write_dataset(table, base_dir, format="feather",
                      basename_template='dat_{i}.arrow',
                      partitioning=partitioning, file_visitor=file_visitor)
     file_paths = list(base_dir.rglob("*"))
     assert set(file_paths) == set(expected_paths)
+    actual_sizes = [os.path.getsize(path) for path in visited_paths]
+    assert visited_sizes == actual_sizes
     result = ds.dataset(base_dir, format="ipc", partitioning=partitioning)
     assert result.to_table().equals(table)
     assert len(visited_paths) == 2
     for visited_path in visited_paths:
         assert pathlib.Path(visited_path) in expected_paths
 
 
@@ -4461,17 +4542,46 @@
     )
     # check roundtrip
     result = ds.dataset(
         "existing-bucket", filesystem=fs, format="ipc", partitioning="hive"
     ).to_table()
     assert result.equals(table)
 
+    # Passing create_dir is fine if the bucket already exists
+    ds.write_dataset(
+        table, "existing-bucket", filesystem=fs,
+        format="feather", create_dir=True, partitioning=part,
+        existing_data_behavior='overwrite_or_ignore'
+    )
+    # check roundtrip
+    result = ds.dataset(
+        "existing-bucket", filesystem=fs, format="ipc", partitioning="hive"
+    ).to_table()
+    assert result.equals(table)
+
+    # Error enforced by filesystem
+    with pytest.raises(OSError,
+                       match="Bucket 'non-existing-bucket' not found"):
+        ds.write_dataset(
+            table, "non-existing-bucket", filesystem=fs,
+            format="feather", create_dir=True,
+            existing_data_behavior='overwrite_or_ignore'
+        )
+
+    # Error enforced by minio / S3 service
+    fs = S3FileSystem(
+        access_key='limited',
+        secret_key='limited123',
+        endpoint_override='{}:{}'.format(host, port),
+        scheme='http',
+        allow_bucket_creation=True,
+    )
     with pytest.raises(OSError, match="Access Denied"):
         ds.write_dataset(
-            table, "existing-bucket", filesystem=fs,
+            table, "non-existing-bucket", filesystem=fs,
             format="feather", create_dir=True,
             existing_data_behavior='overwrite_or_ignore'
         )
 
 
 @pytest.mark.parquet
 def test_dataset_null_to_dictionary_cast(tempdir, dataset_reader):
@@ -4494,23 +4604,23 @@
 
 @pytest.mark.dataset
 def test_dataset_join(tempdir):
     t1 = pa.table({
         "colA": [1, 2, 6],
         "col2": ["a", "b", "f"]
     })
-    ds.write_dataset(t1, tempdir / "t1", format="parquet")
-    ds1 = ds.dataset(tempdir / "t1")
+    ds.write_dataset(t1, tempdir / "t1", format="ipc")
+    ds1 = ds.dataset(tempdir / "t1", format="ipc")
 
     t2 = pa.table({
         "colB": [99, 2, 1],
         "col3": ["Z", "B", "A"]
     })
-    ds.write_dataset(t2, tempdir / "t2", format="parquet")
-    ds2 = ds.dataset(tempdir / "t2")
+    ds.write_dataset(t2, tempdir / "t2", format="ipc")
+    ds2 = ds.dataset(tempdir / "t2", format="ipc")
 
     result = ds1.join(ds2, "colA", "colB")
     assert result.to_table() == pa.table({
         "colA": [1, 2, 6],
         "col2": ["a", "b", "f"],
         "col3": ["A", "B", None]
     })
@@ -4525,23 +4635,23 @@
 
 @pytest.mark.dataset
 def test_dataset_join_unique_key(tempdir):
     t1 = pa.table({
         "colA": [1, 2, 6],
         "col2": ["a", "b", "f"]
     })
-    ds.write_dataset(t1, tempdir / "t1", format="parquet")
-    ds1 = ds.dataset(tempdir / "t1")
+    ds.write_dataset(t1, tempdir / "t1", format="ipc")
+    ds1 = ds.dataset(tempdir / "t1", format="ipc")
 
     t2 = pa.table({
         "colA": [99, 2, 1],
         "col3": ["Z", "B", "A"]
     })
-    ds.write_dataset(t2, tempdir / "t2", format="parquet")
-    ds2 = ds.dataset(tempdir / "t2")
+    ds.write_dataset(t2, tempdir / "t2", format="ipc")
+    ds2 = ds.dataset(tempdir / "t2", format="ipc")
 
     result = ds1.join(ds2, "colA")
     assert result.to_table() == pa.table({
         "colA": [1, 2, 6],
         "col2": ["a", "b", "f"],
         "col3": ["A", "B", None]
     })
@@ -4557,26 +4667,42 @@
 @pytest.mark.dataset
 def test_dataset_join_collisions(tempdir):
     t1 = pa.table({
         "colA": [1, 2, 6],
         "colB": [10, 20, 60],
         "colVals": ["a", "b", "f"]
     })
-    ds.write_dataset(t1, tempdir / "t1", format="parquet")
-    ds1 = ds.dataset(tempdir / "t1")
+    ds.write_dataset(t1, tempdir / "t1", format="ipc")
+    ds1 = ds.dataset(tempdir / "t1", format="ipc")
 
     t2 = pa.table({
         "colA": [99, 2, 1],
         "colB": [99, 20, 10],
         "colVals": ["Z", "B", "A"]
     })
-    ds.write_dataset(t2, tempdir / "t2", format="parquet")
-    ds2 = ds.dataset(tempdir / "t2")
+    ds.write_dataset(t2, tempdir / "t2", format="ipc")
+    ds2 = ds.dataset(tempdir / "t2", format="ipc")
 
     result = ds1.join(ds2, "colA", join_type="full outer", right_suffix="_r")
     assert result.to_table().sort_by("colA") == pa.table([
         [1, 2, 6, 99],
         [10, 20, 60, None],
         ["a", "b", "f", None],
         [10, 20, None, 99],
         ["A", "B", None, "Z"],
     ], names=["colA", "colB", "colVals", "colB_r", "colVals_r"])
+
+
+@pytest.mark.dataset
+def test_dataset_filter(tempdir):
+    t1 = pa.table({
+        "colA": [1, 2, 6],
+        "col2": ["a", "b", "f"]
+    })
+    ds.write_dataset(t1, tempdir / "t1", format="ipc")
+    ds1 = ds.dataset(tempdir / "t1", format="ipc")
+
+    result = ds1.scanner(filter=pc.field("colA") < 3)
+    assert result.to_table() == pa.table({
+        "colA": [1, 2],
+        "col2": ["a", "b"]
+    })
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_deprecations.py` & `pyarrow-9.0.0/pyarrow/substrait.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,10 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-# Check that various deprecation warnings are raised
-
-# flake8: noqa
-
-import pyarrow as pa
-import pytest
+from pyarrow._substrait import (  # noqa
+    run_query,
+)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_extension_type.py` & `pyarrow-9.0.0/pyarrow/tests/test_extension_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import pickle
 import weakref
+from uuid import uuid4, UUID
 
 import numpy as np
 import pyarrow as pa
 
 import pytest
 
 
@@ -29,22 +30,39 @@
     def __init__(self):
         pa.PyExtensionType.__init__(self, pa.int64())
 
     def __reduce__(self):
         return IntegerType, ()
 
 
+class UuidScalarType(pa.ExtensionScalar):
+    def as_py(self):
+        return None if self.value is None else UUID(bytes=self.value.as_py())
+
+
 class UuidType(pa.PyExtensionType):
 
     def __init__(self):
         pa.PyExtensionType.__init__(self, pa.binary(16))
 
     def __reduce__(self):
         return UuidType, ()
 
+    def __arrow_ext_scalar_class__(self):
+        return UuidScalarType
+
+
+class UuidType2(pa.PyExtensionType):
+
+    def __init__(self):
+        pa.PyExtensionType.__init__(self, pa.binary(16))
+
+    def __reduce__(self):
+        return UuidType, ()
+
 
 class ParamExtType(pa.PyExtensionType):
 
     def __init__(self, width):
         self._width = width
         pa.PyExtensionType.__init__(self, pa.binary(width))
 
@@ -131,14 +149,46 @@
     assert ty.storage_type == pa.binary(16)
     assert ty.__class__ is UuidType
     ty = ParamExtType(5)
     assert ty.storage_type == pa.binary(5)
     assert ty.__class__ is ParamExtType
 
 
+def test_ext_type_as_py():
+    ty = UuidType()
+    expected = uuid4()
+    scalar = pa.ExtensionScalar.from_storage(ty, expected.bytes)
+    assert scalar.as_py() == expected
+
+    # test array
+    uuids = [uuid4() for _ in range(3)]
+    storage = pa.array([uuid.bytes for uuid in uuids], type=pa.binary(16))
+    arr = pa.ExtensionArray.from_storage(ty, storage)
+
+    # Works for __get_item__
+    for i, expected in enumerate(uuids):
+        assert arr[i].as_py() == expected
+
+    # Works for __iter__
+    for result, expected in zip(arr, uuids):
+        assert result.as_py() == expected
+
+    # test chunked array
+    data = [
+        pa.ExtensionArray.from_storage(ty, storage),
+        pa.ExtensionArray.from_storage(ty, storage)
+    ]
+    carr = pa.chunked_array(data)
+    for i, expected in enumerate(uuids + uuids):
+        assert carr[i].as_py() == expected
+
+    for result, expected in zip(carr, uuids + uuids):
+        assert result.as_py() == expected
+
+
 def test_uuid_type_pickle():
     for proto in range(0, pickle.HIGHEST_PROTOCOL + 1):
         ty = UuidType()
         ser = pickle.dumps(ty, protocol=proto)
         del ty
         ty = pickle.loads(ser)
         wr = weakref.ref(ty)
@@ -244,39 +294,64 @@
 
 def test_ext_scalar_from_array():
     data = [b"0123456789abcdef", b"0123456789abcdef",
             b"zyxwvutsrqponmlk", None]
     storage = pa.array(data, type=pa.binary(16))
     ty1 = UuidType()
     ty2 = ParamExtType(16)
+    ty3 = UuidType2()
 
     a = pa.ExtensionArray.from_storage(ty1, storage)
     b = pa.ExtensionArray.from_storage(ty2, storage)
+    c = pa.ExtensionArray.from_storage(ty3, storage)
 
     scalars_a = list(a)
     assert len(scalars_a) == 4
 
+    assert ty1.__arrow_ext_scalar_class__() == UuidScalarType
+    assert type(a[0]) == UuidScalarType
+    assert type(scalars_a[0]) == UuidScalarType
+
     for s, val in zip(scalars_a, data):
         assert isinstance(s, pa.ExtensionScalar)
         assert s.is_valid == (val is not None)
         assert s.type == ty1
         if val is not None:
             assert s.value == pa.scalar(val, storage.type)
+            assert s.as_py() == UUID(bytes=val)
         else:
             assert s.value is None
-        assert s.as_py() == val
 
     scalars_b = list(b)
     assert len(scalars_b) == 4
 
     for sa, sb in zip(scalars_a, scalars_b):
+        assert isinstance(sb, pa.ExtensionScalar)
         assert sa.is_valid == sb.is_valid
-        assert sa.as_py() == sb.as_py()
+        if sa.as_py() is None:
+            assert sa.as_py() == sb.as_py()
+        else:
+            assert sa.as_py().bytes == sb.as_py()
         assert sa != sb
 
+    scalars_c = list(c)
+    assert len(scalars_c) == 4
+
+    for s, val in zip(scalars_c, data):
+        assert isinstance(s, pa.ExtensionScalar)
+        assert s.is_valid == (val is not None)
+        assert s.type == ty3
+        if val is not None:
+            assert s.value == pa.scalar(val, storage.type)
+            assert s.as_py() == val
+        else:
+            assert s.value is None
+
+    assert a.to_pylist() == [UUID(bytes=x) if x else None for x in data]
+
 
 def test_ext_scalar_from_storage():
     ty = UuidType()
 
     s = pa.ExtensionScalar.from_storage(ty, None)
     assert isinstance(s, pa.ExtensionScalar)
     assert s.type == ty
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_feather.py` & `pyarrow-9.0.0/pyarrow/tests/test_feather.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_filesystem.py` & `pyarrow-9.0.0/pyarrow/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_flight.py` & `pyarrow-9.0.0/pyarrow/tests/test_flight.py`

 * *Files 2% similar despite different names*

```diff
@@ -815,14 +815,17 @@
 
 class MultiHeaderClientMiddleware(ClientMiddleware):
     """Test sending/receiving multiple (binary-valued) headers."""
 
     EXPECTED = {
         "x-text": ["foo", "bar"],
         "x-binary-bin": [b"\x00", b"\x01"],
+        # ARROW-16606: ensure mixed-case headers are accepted
+        "x-MIXED-case": ["baz"],
+        b"x-other-MIXED-case": ["baz"],
     }
 
     def __init__(self, factory):
         self.factory = factory
 
     def sending_headers(self):
         return self.EXPECTED
@@ -1513,15 +1516,16 @@
 @pytest.mark.slow
 def test_cancel_do_get():
     """Test canceling a DoGet operation on the client side."""
     with ConstantFlightServer() as server, \
             FlightClient(('localhost', server.port)) as client:
         reader = client.do_get(flight.Ticket(b'ints'))
         reader.cancel()
-        with pytest.raises(flight.FlightCancelledError, match=".*Cancel.*"):
+        with pytest.raises(flight.FlightCancelledError,
+                           match="(?i).*cancel.*"):
             reader.read_chunk()
 
 
 @pytest.mark.slow
 def test_cancel_do_get_threaded():
     """Test canceling a DoGet operation from another thread."""
     with SlowFlightServer() as server, \
@@ -1905,14 +1909,17 @@
                 middleware=[headers]) as client:
             response = next(client.do_action(flight.Action(b"", b"")))
             # The server echoes the headers it got back to us.
             raw_headers = response.body.to_pybytes().decode("utf-8")
             client_headers = ast.literal_eval(raw_headers)
             # Don't directly compare; gRPC may add headers like User-Agent.
             for header, values in MultiHeaderClientMiddleware.EXPECTED.items():
+                header = header.lower()
+                if isinstance(header, bytes):
+                    header = header.decode("ascii")
                 assert client_headers.get(header) == values
                 assert headers.last_headers.get(header) == values
 
 
 @pytest.mark.requires_testing_data
 def test_generic_options():
     """Test setting generic client options."""
@@ -1989,14 +1996,19 @@
 
         reader = client.do_get(flight.Ticket(b""))
         test(reader.read_all)
 
         descriptor = flight.FlightDescriptor.for_command(b"echo")
         writer, reader = client.do_exchange(descriptor)
         test(reader.read_all)
+        try:
+            writer.close()
+        except (KeyboardInterrupt, flight.FlightCancelledError):
+            # Silence the Cancelled/Interrupt exception
+            pass
 
 
 def test_never_sends_data():
     # Regression test for ARROW-12779
     match = "application server implementation error"
     with NeverSendsDataFlightServer() as server, \
             flight.connect(('localhost', server.port)) as client:
@@ -2081,7 +2093,87 @@
     """
 
     with ActionNoneFlightServer() as server, \
             FlightClient(('localhost', server.port)) as client:
         client.do_action(flight.Action("append", b""))
         r = client.do_action(flight.Action("get_value", b""))
         assert json.loads(next(r).body.to_pybytes()) == [True]
+
+
+@pytest.mark.slow  # Takes a while for gRPC to "realize" writes fail
+def test_write_error_propagation():
+    """
+    Ensure that exceptions during writing preserve error context.
+
+    See https://issues.apache.org/jira/browse/ARROW-16592.
+    """
+    expected_message = "foo"
+    expected_info = b"bar"
+    exc = flight.FlightCancelledError(
+        expected_message, extra_info=expected_info)
+    descriptor = flight.FlightDescriptor.for_command(b"")
+    schema = pa.schema([("int64", pa.int64())])
+
+    class FailServer(flight.FlightServerBase):
+        def do_put(self, context, descriptor, reader, writer):
+            raise exc
+
+        def do_exchange(self, context, descriptor, reader, writer):
+            raise exc
+
+    with FailServer() as server, \
+            FlightClient(('localhost', server.port)) as client:
+        # DoPut
+        writer, reader = client.do_put(descriptor, schema)
+
+        # Set a concurrent reader - ensure this doesn't block the
+        # writer side from calling Close()
+        def _reader():
+            try:
+                while True:
+                    reader.read()
+            except flight.FlightError:
+                return
+
+        thread = threading.Thread(target=_reader, daemon=True)
+        thread.start()
+
+        with pytest.raises(flight.FlightCancelledError) as exc_info:
+            while True:
+                writer.write_batch(pa.record_batch([[1]], schema=schema))
+        assert exc_info.value.extra_info == expected_info
+
+        with pytest.raises(flight.FlightCancelledError) as exc_info:
+            writer.close()
+        assert exc_info.value.extra_info == expected_info
+        thread.join()
+
+        # DoExchange
+        writer, reader = client.do_exchange(descriptor)
+
+        def _reader():
+            try:
+                while True:
+                    reader.read_chunk()
+            except flight.FlightError:
+                return
+
+        thread = threading.Thread(target=_reader, daemon=True)
+        thread.start()
+        with pytest.raises(flight.FlightCancelledError) as exc_info:
+            while True:
+                writer.write_metadata(b" ")
+        assert exc_info.value.extra_info == expected_info
+
+        with pytest.raises(flight.FlightCancelledError) as exc_info:
+            writer.close()
+        assert exc_info.value.extra_info == expected_info
+        thread.join()
+
+
+def test_interpreter_shutdown():
+    """
+    Ensure that the gRPC server is stopped at interpreter shutdown.
+
+    See https://issues.apache.org/jira/browse/ARROW-16597.
+    """
+    util.invoke_script("arrow_16597.py")
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_fs.py` & `pyarrow-9.0.0/pyarrow/tests/test_fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,26 +197,56 @@
         pathfn=lambda p: p,
         allow_move_dir=True,
         allow_append_to_file=True,
     )
 
 
 @pytest.fixture
+def gcsfs(request, gcs_server):
+    request.config.pyarrow.requires('gcs')
+    from pyarrow.fs import GcsFileSystem
+
+    host, port = gcs_server['connection']
+    bucket = 'pyarrow-filesystem/'
+    # Make sure the server is alive.
+    assert gcs_server['process'].poll() is None
+
+    fs = GcsFileSystem(
+        endpoint_override=f'{host}:{port}',
+        scheme='http',
+        # Mock endpoint doesn't check credentials.
+        anonymous=True,
+        retry_time_limit=timedelta(seconds=45)
+    )
+    fs.create_dir(bucket)
+
+    yield dict(
+        fs=fs,
+        pathfn=bucket.__add__,
+        allow_move_dir=False,
+        allow_append_to_file=False,
+    )
+    fs.delete_dir(bucket)
+
+
+@pytest.fixture
 def s3fs(request, s3_server):
     request.config.pyarrow.requires('s3')
     from pyarrow.fs import S3FileSystem
 
     host, port, access_key, secret_key = s3_server['connection']
     bucket = 'pyarrow-filesystem/'
 
     fs = S3FileSystem(
         access_key=access_key,
         secret_key=secret_key,
         endpoint_override='{}:{}'.format(host, port),
-        scheme='http'
+        scheme='http',
+        allow_bucket_creation=True,
+        allow_bucket_deletion=True
     )
     fs.create_dir(bucket)
 
     yield dict(
         fs=fs,
         pathfn=bucket.__add__,
         allow_move_dir=False,
@@ -342,14 +372,19 @@
     ),
     pytest.param(
         pytest.lazy_fixture('s3fs'),
         id='S3FileSystem',
         marks=pytest.mark.s3
     ),
     pytest.param(
+        pytest.lazy_fixture('gcsfs'),
+        id='GcsFileSystem',
+        marks=pytest.mark.gcs
+    ),
+    pytest.param(
         pytest.lazy_fixture('hdfs'),
         id='HadoopFileSystem',
         marks=pytest.mark.hdfs
     ),
     pytest.param(
         pytest.lazy_fixture('mockfs'),
         id='_MockFileSystem()'
@@ -439,14 +474,20 @@
         access_key='limited',
         secret_key='limited123',
         endpoint_override='{}:{}'.format(host, port),
         scheme='http'
     )
     fs.create_dir('existing-bucket/test')
 
+    with pytest.raises(pa.ArrowIOError, match="Bucket 'new-bucket' not found"):
+        fs.create_dir('new-bucket')
+
+    with pytest.raises(pa.ArrowIOError, match="Would delete bucket"):
+        fs.delete_dir('existing-bucket')
+
 
 def test_file_info_constructor():
     dt = datetime.fromtimestamp(1568799826, timezone.utc)
 
     info = FileInfo("foo/bar")
     assert info.path == "foo/bar"
     assert info.base_name == "bar"
@@ -866,14 +907,18 @@
 
     data = b'some data' * 1024
     with fs.open_output_stream(p) as s:
         s.write(data)
 
     read_from = len(b'some data') * 512
     with fs.open_input_file(p) as f:
+        result = f.read()
+    assert result == data
+
+    with fs.open_input_file(p) as f:
         f.seek(read_from)
         result = f.read()
 
     assert result == data[read_from:]
 
 
 def test_open_input_stream_not_found(fs, pathfn):
@@ -947,15 +992,15 @@
     with fs.open_output_stream(p, metadata=metadata) as f:
         f.write(data)
 
     with fs.open_input_stream(p) as f:
         assert f.read() == data
         got_metadata = f.metadata()
 
-    if fs.type_name == 's3' or 'mock' in fs.type_name:
+    if fs.type_name in ['s3', 'gcs'] or 'mock' in fs.type_name:
         for k, v in metadata.items():
             assert got_metadata[k] == v.encode()
     else:
         assert got_metadata == {}
 
 
 def test_localfs_options():
@@ -1006,14 +1051,50 @@
 
     with fs.open_output_stream('foo'):
         pass
     [info] = fs.get_file_info(['foo'])
     assert info.mtime == dt
 
 
+@pytest.mark.gcs
+def test_gcs_options():
+    from pyarrow.fs import GcsFileSystem
+    dt = datetime.now()
+    fs = GcsFileSystem(access_token='abc',
+                       target_service_account='service_account@apache',
+                       credential_token_expiration=dt,
+                       default_bucket_location='us-west2',
+                       scheme='https', endpoint_override='localhost:8999')
+    assert isinstance(fs, GcsFileSystem)
+    assert fs.default_bucket_location == 'us-west2'
+    assert pickle.loads(pickle.dumps(fs)) == fs
+
+    fs = GcsFileSystem()
+    assert isinstance(fs, GcsFileSystem)
+    assert pickle.loads(pickle.dumps(fs)) == fs
+
+    fs = GcsFileSystem(anonymous=True)
+    assert isinstance(fs, GcsFileSystem)
+    assert pickle.loads(pickle.dumps(fs)) == fs
+
+    fs = GcsFileSystem(default_metadata={"ACL": "authenticated-read",
+                                         "Content-Type": "text/plain"})
+    assert isinstance(fs, GcsFileSystem)
+    assert pickle.loads(pickle.dumps(fs)) == fs
+
+    with pytest.raises(ValueError):
+        GcsFileSystem(access_token='access')
+    with pytest.raises(ValueError):
+        GcsFileSystem(anonymous=True, access_token='secret')
+    with pytest.raises(ValueError):
+        GcsFileSystem(anonymous=True, target_service_account='acct')
+    with pytest.raises(ValueError):
+        GcsFileSystem(credential_token_expiration=datetime.now())
+
+
 @pytest.mark.s3
 def test_s3_options():
     from pyarrow.fs import S3FileSystem
 
     fs = S3FileSystem(access_key='access', secret_key='secret',
                       session_token='token', region='us-east-2',
                       scheme='https', endpoint_override='localhost:8999')
@@ -1022,21 +1103,35 @@
     assert pickle.loads(pickle.dumps(fs)) == fs
 
     fs = S3FileSystem(role_arn='role', session_name='session',
                       external_id='id', load_frequency=100)
     assert isinstance(fs, S3FileSystem)
     assert pickle.loads(pickle.dumps(fs)) == fs
 
+    fs2 = S3FileSystem(role_arn='role')
+    assert isinstance(fs2, S3FileSystem)
+    assert pickle.loads(pickle.dumps(fs2)) == fs2
+    assert fs2 != fs
+
     fs = S3FileSystem(anonymous=True)
     assert isinstance(fs, S3FileSystem)
     assert pickle.loads(pickle.dumps(fs)) == fs
 
-    fs = S3FileSystem(background_writes=True,
-                      default_metadata={"ACL": "authenticated-read",
-                                        "Content-Type": "text/plain"})
+    fs = S3FileSystem(background_writes=True)
+    assert isinstance(fs, S3FileSystem)
+    assert pickle.loads(pickle.dumps(fs)) == fs
+
+    fs2 = S3FileSystem(background_writes=True,
+                       default_metadata={"ACL": "authenticated-read",
+                                         "Content-Type": "text/plain"})
+    assert isinstance(fs2, S3FileSystem)
+    assert pickle.loads(pickle.dumps(fs2)) == fs2
+    assert fs2 != fs
+
+    fs = S3FileSystem(allow_bucket_creation=True, allow_bucket_deletion=True)
     assert isinstance(fs, S3FileSystem)
     assert pickle.loads(pickle.dumps(fs)) == fs
 
     with pytest.raises(ValueError):
         S3FileSystem(access_key='access')
     with pytest.raises(ValueError):
         S3FileSystem(secret_key='secret')
@@ -1304,27 +1399,48 @@
 
 @pytest.mark.s3
 def test_filesystem_from_uri_s3(s3_server):
     from pyarrow.fs import S3FileSystem
 
     host, port, access_key, secret_key = s3_server['connection']
 
-    uri = "s3://{}:{}@mybucket/foo/bar?scheme=http&endpoint_override={}:{}" \
-        .format(access_key, secret_key, host, port)
+    uri = "s3://{}:{}@mybucket/foo/bar?scheme=http&endpoint_override={}:{}"\
+          "&allow_bucket_creation=True" \
+          .format(access_key, secret_key, host, port)
 
     fs, path = FileSystem.from_uri(uri)
     assert isinstance(fs, S3FileSystem)
     assert path == "mybucket/foo/bar"
 
     fs.create_dir(path)
     [info] = fs.get_file_info([path])
     assert info.path == path
     assert info.type == FileType.Directory
 
 
+@pytest.mark.gcs
+def test_filesystem_from_uri_gcs(gcs_server):
+    from pyarrow.fs import GcsFileSystem
+
+    host, port = gcs_server['connection']
+
+    uri = ("gs://anonymous@" +
+           f"mybucket/foo/bar?scheme=http&endpoint_override={host}:{port}&" +
+           "retry_limit_seconds=5")
+
+    fs, path = FileSystem.from_uri(uri)
+    assert isinstance(fs, GcsFileSystem)
+    assert path == "mybucket/foo/bar"
+
+    fs.create_dir(path)
+    [info] = fs.get_file_info([path])
+    assert info.path == path
+    assert info.type == FileType.Directory
+
+
 def test_py_filesystem():
     handler = DummyHandler()
     fs = PyFileSystem(handler)
     assert isinstance(fs, PyFileSystem)
     assert fs.type_name == "py::dummy"
     assert fs.handler is handler
 
@@ -1496,23 +1612,25 @@
     from pyarrow.fs import S3FileSystem
     default_region = (os.environ.get('PYARROW_TEST_S3_REGION') or
                       'us-east-1')
     fs = S3FileSystem(anonymous=True)
     assert fs.region == default_region
 
     fs = S3FileSystem(anonymous=True, region='us-east-2')
-    entries = fs.get_file_info(FileSelector('ursa-labs-taxi-data'))
+    entries = fs.get_file_info(FileSelector(
+        'voltrondata-labs-datasets/nyc-taxi'))
     assert len(entries) > 0
-    with fs.open_input_stream('ursa-labs-taxi-data/2019/06/data.parquet') as f:
+    key = 'voltrondata-labs-datasets/nyc-taxi/year=2019/month=6/part-0.parquet'
+    with fs.open_input_stream(key) as f:
         md = f.metadata()
         assert 'Content-Type' in md
-        assert md['Last-Modified'] == b'2020-01-17T16:26:28Z'
+        assert md['Last-Modified'] == b'2022-07-12T23:32:00Z'
         # For some reason, the header value is quoted
         # (both with AWS and Minio)
-        assert md['ETag'] == b'"f1efd5d76cb82861e1542117bfa52b90-8"'
+        assert md['ETag'] == b'"4c6a76826a695c6ac61592bc30cda3df-16"'
 
 
 @pytest.mark.s3
 def test_s3_real_aws_region_selection():
     # Taken from a registry of open S3-hosted datasets
     # at https://github.com/awslabs/open-data-registry
     fs, path = FileSystem.from_uri('s3://mf-nwp-models/README.txt')
@@ -1533,15 +1651,15 @@
         's3://x-arrow-non-existent-bucket?region=us-east-3')
     assert fs.region == 'us-east-3'
 
 
 @pytest.mark.s3
 def test_resolve_s3_region():
     from pyarrow.fs import resolve_s3_region
-    assert resolve_s3_region('ursa-labs-taxi-data') == 'us-east-2'
+    assert resolve_s3_region('voltrondata-labs-datasets') == 'us-east-2'
     assert resolve_s3_region('mf-nwp-models') == 'eu-west-1'
 
     with pytest.raises(ValueError, match="Not a valid bucket name"):
         resolve_s3_region('foo/bar')
     with pytest.raises(ValueError, match="Not a valid bucket name"):
         resolve_s3_region('s3:bucket')
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_gandiva.py` & `pyarrow-9.0.0/pyarrow/tests/test_gandiva.py`

 * *Files 4% similar despite different names*

```diff
@@ -385,7 +385,48 @@
     field_z = builder.make_field(pa.field('z', pa.bool_()))
     func_node = builder.make_function('not', [field_z], pa.bool_())
     assert str(func_node) == 'bool not((bool) z)'
 
     field_y = builder.make_field(pa.field('y', pa.bool_()))
     and_node = builder.make_and([func_node, field_y])
     assert str(and_node) == 'bool not((bool) z) && (bool) y'
+
+
+@pytest.mark.gandiva
+def test_rejects_none():
+    import pyarrow.gandiva as gandiva
+
+    builder = gandiva.TreeExprBuilder()
+
+    field_x = pa.field('x', pa.int32())
+    schema = pa.schema([field_x])
+    literal_true = builder.make_literal(True, pa.bool_())
+
+    with pytest.raises(TypeError):
+        builder.make_field(None)
+
+    with pytest.raises(TypeError):
+        builder.make_if(literal_true, None, None, None)
+
+    with pytest.raises(TypeError):
+        builder.make_and([literal_true, None])
+
+    with pytest.raises(TypeError):
+        builder.make_or([None, literal_true])
+
+    with pytest.raises(TypeError):
+        builder.make_in_expression(None, [1, 2, 3], pa.int32())
+
+    with pytest.raises(TypeError):
+        builder.make_expression(None, field_x)
+
+    with pytest.raises(TypeError):
+        builder.make_condition(None)
+
+    with pytest.raises(TypeError):
+        builder.make_function('less_than', [literal_true, None], pa.bool_())
+
+    with pytest.raises(TypeError):
+        gandiva.make_projector(schema, [None])
+
+    with pytest.raises(TypeError):
+        gandiva.make_filter(schema, None)
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_gdb.py` & `pyarrow-9.0.0/pyarrow/tests/test_gdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         'arrow::LargeStringScalar of size 6, value "héhé"')
 
     check_stack_repr(
         gdb_arrow, "fixed_size_binary_scalar",
         'arrow::FixedSizeBinaryScalar of size 3, value "abc"')
     check_stack_repr(
         gdb_arrow, "fixed_size_binary_scalar_null",
-        'arrow::FixedSizeBinaryScalar of size 3, null value')
+        'arrow::FixedSizeBinaryScalar of size 3, null with value "   "')
 
     check_stack_repr(
         gdb_arrow, "dict_scalar",
         re.compile(
             (r'^arrow::DictionaryScalar of index '
              r'arrow::Int8Scalar of value 42, '
              r'dictionary arrow::StringArray ')))
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_hdfs.py` & `pyarrow-9.0.0/pyarrow/tests/test_hdfs.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_io.py` & `pyarrow-9.0.0/pyarrow/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import bz2
 from contextlib import contextmanager
 from io import (BytesIO, StringIO, TextIOWrapper, BufferedIOBase, IOBase)
 import itertools
 import gc
 import gzip
+import math
 import os
 import pathlib
 import pickle
 import pytest
 import sys
 import tempfile
 import weakref
@@ -1197,14 +1198,73 @@
         fil.write(data)
 
     with TextIOWrapper(pa.OSFile(path2, mode='rb')) as fil:
         res = fil.read()
         assert res == data
 
 
+def test_native_file_TextIOWrapper_perf(tmpdir):
+    # ARROW-16272: TextIOWrapper.readline() shouldn't exhaust a large
+    # Arrow input stream.
+    data = b'foo\nquux\n'
+    path = str(tmpdir / 'largefile.txt')
+    with open(path, 'wb') as f:
+        f.write(data * 100_000)
+
+    binary_file = pa.OSFile(path, mode='rb')
+    with TextIOWrapper(binary_file) as f:
+        assert binary_file.tell() == 0
+        nbytes = 20_000
+        lines = f.readlines(nbytes)
+        assert len(lines) == math.ceil(2 * nbytes / len(data))
+        assert nbytes <= binary_file.tell() <= nbytes * 2
+
+
+def test_native_file_read1(tmpdir):
+    # ARROW-16272: read1() should not exhaust the input stream if there
+    # is a large amount of data remaining.
+    data = b'123\n' * 1_000_000
+    path = str(tmpdir / 'largefile.txt')
+    with open(path, 'wb') as f:
+        f.write(data)
+
+    chunks = []
+    with pa.OSFile(path, mode='rb') as f:
+        while True:
+            b = f.read1()
+            assert len(b) < len(data)
+            chunks.append(b)
+            b = f.read1(30_000)
+            assert len(b) <= 30_000
+            chunks.append(b)
+            if not b:
+                break
+
+    assert b"".join(chunks) == data
+
+
+@pytest.mark.pandas
+def test_native_file_pandas_text_reader(tmpdir):
+    # ARROW-16272: Pandas' read_csv() should not exhaust an Arrow
+    # input stream when a small nrows is passed.
+    import pandas as pd
+    import pandas.testing as tm
+    data = b'a,b\n' * 10_000_000
+    path = str(tmpdir / 'largefile.txt')
+    with open(path, 'wb') as f:
+        f.write(data)
+
+    with pa.OSFile(path, mode='rb') as f:
+        df = pd.read_csv(f, nrows=10)
+        expected = pd.DataFrame({'a': ['a'] * 10, 'b': ['b'] * 10})
+        tm.assert_frame_equal(df, expected)
+        # Some readahead occurred, but not up to the end of file
+        assert f.tell() <= 256 * 1024
+
+
 def test_native_file_open_error():
     with assert_file_not_found():
         pa.OSFile('non_existent_file', 'rb')
     with assert_file_not_found():
         pa.memory_map('non_existent_file', 'rb')
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_ipc.py` & `pyarrow-9.0.0/pyarrow/tests/test_ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,31 +1098,14 @@
 
     assert recons_schema.equals(schema)
     assert recons_schema.metadata == schema_metadata
     assert recons_schema[0].metadata is None
     assert recons_schema[1].metadata == field_metadata
 
 
-def test_deprecated_pyarrow_ns_apis():
-    table = pa.table([pa.array([1, 2, 3, 4])], names=['a'])
-    sink = pa.BufferOutputStream()
-    with pa.ipc.new_stream(sink, table.schema) as writer:
-        writer.write(table)
-
-    with pytest.warns(FutureWarning,
-                      match="please use pyarrow.ipc.open_stream"):
-        pa.open_stream(sink.getvalue())
-
-    sink = pa.BufferOutputStream()
-    with pa.ipc.new_file(sink, table.schema) as writer:
-        writer.write(table)
-    with pytest.warns(FutureWarning, match="please use pyarrow.ipc.open_file"):
-        pa.open_file(sink.getvalue())
-
-
 def write_file(batch, sink):
     with pa.ipc.new_file(sink, batch.schema) as writer:
         writer.write_batch(batch)
 
 
 def read_file(source):
     with pa.ipc.open_file(source) as reader:
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_json.py` & `pyarrow-9.0.0/pyarrow/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_jvm.py` & `pyarrow-9.0.0/pyarrow/tests/test_jvm.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_memory.py` & `pyarrow-9.0.0/pyarrow/tests/test_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,18 @@
     """
     Run a piece of code making an invalid memory write with the
     ARROW_DEBUG_MEMORY_POOL environment variable set to a specific value.
     """
     code = f"""if 1:
         import ctypes
         import pyarrow as pa
+        # ARROW-16873: some Python installs enable faulthandler by default,
+        # which could dump a spurious stack trace if the following crashes
+        import faulthandler
+        faulthandler.disable()
 
         pool = pa.{pool_factory}()
         buf = pa.allocate_buffer(64, memory_pool=pool)
 
         # Write memory out of bounds
         ptr = ctypes.cast(buf.address, ctypes.POINTER(ctypes.c_ubyte))
         ptr[64] = 0
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_misc.py` & `pyarrow-9.0.0/pyarrow/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_orc.py` & `pyarrow-9.0.0/pyarrow/tests/test_orc.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_pandas.py` & `pyarrow-9.0.0/pyarrow/tests/test_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,30 @@
     """
 
     def test_non_string_columns(self):
         df = pd.DataFrame({0: [1, 2, 3]})
         table = pa.Table.from_pandas(df)
         assert table.field(0).name == '0'
 
+    def test_non_string_columns_with_index(self):
+        df = pd.DataFrame({0: [1.0, 2.0, 3.0], 1: [4.0, 5.0, 6.0]})
+        df = df.set_index(0)
+
+        # assert that the from_pandas raises the warning
+        with pytest.warns(UserWarning):
+            table = pa.Table.from_pandas(df)
+            assert table.field(0).name == '1'
+
+        expected = df.copy()
+        # non-str index name will be converted to str
+        expected.index.name = str(expected.index.name)
+        with pytest.warns(UserWarning):
+            _check_pandas_roundtrip(df, expected=expected,
+                                    preserve_index=True)
+
     def test_from_pandas_with_columns(self):
         df = pd.DataFrame({0: [1, 2, 3], 1: [1, 3, 3], 2: [2, 4, 5]},
                           columns=[1, 0])
 
         table = pa.Table.from_pandas(df, columns=[0, 1])
         expected = pa.Table.from_pandas(df[[0, 1]])
         assert expected.equals(table)
@@ -222,15 +238,15 @@
         # ARROW-5606: pandas 0.25 deprecated private _start/stop/step
         # attributes -> can be removed if support < pd 0.25 is dropped
         df = pd.DataFrame(np.random.randn(4, 2), columns=['a', 'b'])
 
         with pytest.warns(None) as record:
             _check_pandas_roundtrip(df, preserve_index=True)
 
-        assert len(record) == 0
+        assert len(record) == 0, [r.message for r in record]
 
     def test_multiindex_columns(self):
         columns = pd.MultiIndex.from_arrays([
             ['one', 'two'], ['X', 'Y']
         ])
         df = pd.DataFrame([(1, 'a'), (2, 'b'), (3, 'c')], columns=columns)
         _check_pandas_roundtrip(df, preserve_index=True)
@@ -273,15 +289,15 @@
         # ARROW-3953: pandas 0.24 rename of MultiIndex labels to codes
         columns = pd.MultiIndex.from_arrays([['one', 'two'], ['X', 'Y']])
         df = pd.DataFrame([(1, 'a'), (2, 'b'), (3, 'c')], columns=columns)
 
         with pytest.warns(None) as record:
             _check_pandas_roundtrip(df, preserve_index=True)
 
-        assert len(record) == 0
+        assert len(record) == 0, [r.message for r in record]
 
     def test_integer_index_column(self):
         df = pd.DataFrame([(1, 'a'), (2, 'b'), (3, 'c')])
         _check_pandas_roundtrip(df, preserve_index=True)
 
     def test_index_metadata_field_name(self):
         # test None case, and strangely named non-index columns
@@ -4453,7 +4469,19 @@
             assert result[0].tzinfo is None
             expected = dt
         assert result[0] == expected
 
 
 def test_threaded_pandas_import():
     invoke_script("pandas_threaded_import.py")
+
+
+def test_does_not_mutate_timedelta_dtype():
+    expected = np.dtype('m8')
+
+    assert np.dtype(np.timedelta64) == expected
+
+    df = pd.DataFrame({"a": [np.timedelta64()]})
+    t = pa.Table.from_pandas(df)
+    t.to_pandas()
+
+    assert np.dtype(np.timedelta64) == expected
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_plasma.py` & `pyarrow-9.0.0/pyarrow/tests/test_plasma.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_plasma_tf_op.py` & `pyarrow-9.0.0/pyarrow/tests/test_plasma_tf_op.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_scalars.py` & `pyarrow-9.0.0/pyarrow/tests/test_scalars.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,71 +22,63 @@
 import weakref
 
 import numpy as np
 
 import pyarrow as pa
 
 
-@pytest.mark.parametrize(['value', 'ty', 'klass', 'deprecated'], [
-    (False, None, pa.BooleanScalar, pa.BooleanValue),
-    (True, None, pa.BooleanScalar, pa.BooleanValue),
-    (1, None, pa.Int64Scalar, pa.Int64Value),
-    (-1, None, pa.Int64Scalar, pa.Int64Value),
-    (1, pa.int8(), pa.Int8Scalar, pa.Int8Value),
-    (1, pa.uint8(), pa.UInt8Scalar, pa.UInt8Value),
-    (1, pa.int16(), pa.Int16Scalar, pa.Int16Value),
-    (1, pa.uint16(), pa.UInt16Scalar, pa.UInt16Value),
-    (1, pa.int32(), pa.Int32Scalar, pa.Int32Value),
-    (1, pa.uint32(), pa.UInt32Scalar, pa.UInt32Value),
-    (1, pa.int64(), pa.Int64Scalar, pa.Int64Value),
-    (1, pa.uint64(), pa.UInt64Scalar, pa.UInt64Value),
-    (1.0, None, pa.DoubleScalar, pa.DoubleValue),
-    (np.float16(1.0), pa.float16(), pa.HalfFloatScalar, pa.HalfFloatValue),
-    (1.0, pa.float32(), pa.FloatScalar, pa.FloatValue),
-    (decimal.Decimal("1.123"), None, pa.Decimal128Scalar, pa.Decimal128Value),
+@pytest.mark.parametrize(['value', 'ty', 'klass'], [
+    (False, None, pa.BooleanScalar),
+    (True, None, pa.BooleanScalar),
+    (1, None, pa.Int64Scalar),
+    (-1, None, pa.Int64Scalar),
+    (1, pa.int8(), pa.Int8Scalar),
+    (1, pa.uint8(), pa.UInt8Scalar),
+    (1, pa.int16(), pa.Int16Scalar),
+    (1, pa.uint16(), pa.UInt16Scalar),
+    (1, pa.int32(), pa.Int32Scalar),
+    (1, pa.uint32(), pa.UInt32Scalar),
+    (1, pa.int64(), pa.Int64Scalar),
+    (1, pa.uint64(), pa.UInt64Scalar),
+    (1.0, None, pa.DoubleScalar),
+    (np.float16(1.0), pa.float16(), pa.HalfFloatScalar),
+    (1.0, pa.float32(), pa.FloatScalar),
+    (decimal.Decimal("1.123"), None, pa.Decimal128Scalar),
     (decimal.Decimal("1.1234567890123456789012345678901234567890"),
-     None, pa.Decimal256Scalar, pa.Decimal256Value),
-    ("string", None, pa.StringScalar, pa.StringValue),
-    (b"bytes", None, pa.BinaryScalar, pa.BinaryValue),
-    ("largestring", pa.large_string(), pa.LargeStringScalar,
-     pa.LargeStringValue),
-    (b"largebytes", pa.large_binary(), pa.LargeBinaryScalar,
-     pa.LargeBinaryValue),
-    (b"abc", pa.binary(3), pa.FixedSizeBinaryScalar, pa.FixedSizeBinaryValue),
-    ([1, 2, 3], None, pa.ListScalar, pa.ListValue),
-    ([1, 2, 3, 4], pa.large_list(pa.int8()), pa.LargeListScalar,
-     pa.LargeListValue),
-    ([1, 2, 3, 4, 5], pa.list_(pa.int8(), 5), pa.FixedSizeListScalar,
-     pa.FixedSizeListValue),
-    (datetime.date.today(), None, pa.Date32Scalar, pa.Date32Value),
-    (datetime.date.today(), pa.date64(), pa.Date64Scalar, pa.Date64Value),
-    (datetime.datetime.now(), None, pa.TimestampScalar, pa.TimestampValue),
+     None, pa.Decimal256Scalar),
+    ("string", None, pa.StringScalar),
+    (b"bytes", None, pa.BinaryScalar),
+    ("largestring", pa.large_string(), pa.LargeStringScalar),
+    (b"largebytes", pa.large_binary(), pa.LargeBinaryScalar),
+    (b"abc", pa.binary(3), pa.FixedSizeBinaryScalar),
+    ([1, 2, 3], None, pa.ListScalar),
+    ([1, 2, 3, 4], pa.large_list(pa.int8()), pa.LargeListScalar),
+    ([1, 2, 3, 4, 5], pa.list_(pa.int8(), 5), pa.FixedSizeListScalar),
+    (datetime.date.today(), None, pa.Date32Scalar),
+    (datetime.date.today(), pa.date64(), pa.Date64Scalar),
+    (datetime.datetime.now(), None, pa.TimestampScalar),
     (datetime.datetime.now().time().replace(microsecond=0), pa.time32('s'),
-     pa.Time32Scalar, pa.Time32Value),
-    (datetime.datetime.now().time(), None, pa.Time64Scalar, pa.Time64Value),
-    (datetime.timedelta(days=1), None, pa.DurationScalar, pa.DurationValue),
+     pa.Time32Scalar),
+    (datetime.datetime.now().time(), None, pa.Time64Scalar),
+    (datetime.timedelta(days=1), None, pa.DurationScalar),
     (pa.MonthDayNano([1, -1, -10100]), None,
-     pa.MonthDayNanoIntervalScalar, None),
-    ({'a': 1, 'b': [1, 2]}, None, pa.StructScalar, pa.StructValue),
-    ([('a', 1), ('b', 2)], pa.map_(pa.string(), pa.int8()), pa.MapScalar,
-     pa.MapValue),
+     pa.MonthDayNanoIntervalScalar),
+    ({'a': 1, 'b': [1, 2]}, None, pa.StructScalar),
+    ([('a', 1), ('b', 2)], pa.map_(pa.string(), pa.int8()), pa.MapScalar),
 ])
-def test_basics(value, ty, klass, deprecated):
+def test_basics(value, ty, klass):
     s = pa.scalar(value, type=ty)
     assert isinstance(s, klass)
     assert s.as_py() == value
     assert s == pa.scalar(value, type=ty)
     assert s != value
     assert s != "else"
     assert hash(s) == hash(s)
     assert s.is_valid is True
     assert s != None  # noqa: E711
-    if deprecated is not None:
-        with pytest.warns(FutureWarning):
-            assert isinstance(s, deprecated)
 
     s = pa.scalar(None, type=s.type)
     assert s.is_valid is False
     assert s.as_py() is None
     assert s != pa.scalar(value, type=ty)
 
     # test pickle roundtrip
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_schema.py` & `pyarrow-9.0.0/pyarrow/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_serialization.py` & `pyarrow-9.0.0/pyarrow/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_serialization_deprecated.py` & `pyarrow-9.0.0/pyarrow/tests/test_serialization_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_sparse_tensor.py` & `pyarrow-9.0.0/pyarrow/tests/test_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_strategies.py` & `pyarrow-9.0.0/pyarrow/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_table.py` & `pyarrow-9.0.0/pyarrow/tests/test_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -2117,7 +2117,70 @@
     assert result.combine_chunks().sort_by("colA") == pa.table([
         [1, 2, 6, 99],
         [10, 20, 60, None],
         ["a", "b", "f", None],
         [10, 20, None, 99],
         ["A", "B", None, "Z"],
     ], names=["colA", "colB", "colVals", "colB", "colVals"])
+
+
+@pytest.mark.dataset
+def test_table_filter_expression():
+    t1 = pa.table({
+        "colA": [1, 2, 6],
+        "colB": [10, 20, 60],
+        "colVals": ["a", "b", "f"]
+    })
+
+    t2 = pa.table({
+        "colA": [99, 2, 1],
+        "colB": [99, 20, 10],
+        "colVals": ["Z", "B", "A"]
+    })
+
+    t3 = pa.concat_tables([t1, t2])
+
+    result = t3.filter(pc.field("colA") < 10)
+    assert result.combine_chunks() == pa.table({
+        "colA": [1, 2, 6, 2, 1],
+        "colB": [10, 20, 60, 20, 10],
+        "colVals": ["a", "b", "f", "B", "A"]
+    })
+
+
+@pytest.mark.dataset
+def test_table_join_many_columns():
+    t1 = pa.table({
+        "colA": [1, 2, 6],
+        "col2": ["a", "b", "f"]
+    })
+
+    t2 = pa.table({
+        "colB": [99, 2, 1],
+        "col3": ["Z", "B", "A"],
+        "col4": ["Z", "B", "A"],
+        "col5": ["Z", "B", "A"],
+        "col6": ["Z", "B", "A"],
+        "col7": ["Z", "B", "A"]
+    })
+
+    result = t1.join(t2, "colA", "colB")
+    assert result.combine_chunks() == pa.table({
+        "colA": [1, 2, 6],
+        "col2": ["a", "b", "f"],
+        "col3": ["A", "B", None],
+        "col4": ["A", "B", None],
+        "col5": ["A", "B", None],
+        "col6": ["A", "B", None],
+        "col7": ["A", "B", None]
+    })
+
+    result = t1.join(t2, "colA", "colB", join_type="full outer")
+    assert result.combine_chunks().sort_by("colA") == pa.table({
+        "colA": [1, 2, 6, 99],
+        "col2": ["a", "b", "f", None],
+        "col3": ["A", "B", None, "Z"],
+        "col4": ["A", "B", None, "Z"],
+        "col5": ["A", "B", None, "Z"],
+        "col6": ["A", "B", None, "Z"],
+        "col7": ["A", "B", None, "Z"],
+    })
```

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_tensor.py` & `pyarrow-9.0.0/pyarrow/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_types.py` & `pyarrow-9.0.0/pyarrow/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/test_util.py` & `pyarrow-9.0.0/pyarrow/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/tests/util.py` & `pyarrow-9.0.0/pyarrow/tests/util.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/types.pxi` & `pyarrow-9.0.0/pyarrow/types.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,31 @@
         """
         return self.list_type.list_size()
 
 
 cdef class StructType(DataType):
     """
     Concrete class for struct data types.
+
+    ``StructType`` supports direct indexing using ``[...]`` (implemented via
+    ``__getitem__``) to access its fields.
+    It will return the struct field with the given index or name.
+
+    Examples
+    --------
+    >>> import pyarrow as pa
+    >>> struct_type = pa.struct({'x': pa.int32(), 'y': pa.string()})
+    >>> struct_type[0]
+    pyarrow.Field<x: int32>
+    >>> struct_type['y']
+    pyarrow.Field<y: string>
+
+    >>> pa.schema(list(struct_type))
+    x: int32
+    y: string
     """
 
     cdef void init(self, const shared_ptr[CDataType]& type) except *:
         DataType.init(self, type)
         self.struct_type = <const CStructType*> type.get()
 
     cdef Field field_by_name(self, name):
@@ -898,14 +915,24 @@
 
         This method should return a subclass of the ExtensionArray class. By
         default, if not specialized in the extension implementation, an
         extension type array will be a built-in ExtensionArray instance.
         """
         return ExtensionArray
 
+    def __arrow_ext_scalar_class__(self):
+        """Return an extension scalar class for building scalars with this
+        extension type.
+
+        This method should return subclass of the ExtensionScalar class. By
+        default, if not specialized in the extension implementation, an
+        extension type scalar will be a built-in ExtensionScalar instance.
+        """
+        return ExtensionScalar
+
 
 cdef class PyExtensionType(ExtensionType):
     """
     Concrete base class for Python-defined extension types based on pickle
     for (de)serialization.
 
     Parameters
@@ -1141,15 +1168,15 @@
         for i in range(self.metadata.size()):
             key = self.metadata.key(i)
             if key not in result:
                 result[key] = self.metadata.value(i)
         return result
 
 
-cdef KeyValueMetadata ensure_metadata(object meta, c_bool allow_none=False):
+cpdef KeyValueMetadata ensure_metadata(object meta, c_bool allow_none=False):
     if allow_none and meta is None:
         return None
     elif isinstance(meta, KeyValueMetadata):
         return meta
     else:
         return KeyValueMetadata(meta)
```

### Comparing `pyarrow-8.0.0/pyarrow/types.py` & `pyarrow-9.0.0/pyarrow/types.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/util.py` & `pyarrow-9.0.0/pyarrow/util.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/vendored/__init__.py` & `pyarrow-9.0.0/pyarrow/vendored/__init__.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/vendored/docscrape.py` & `pyarrow-9.0.0/pyarrow/vendored/docscrape.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow/vendored/version.py` & `pyarrow-9.0.0/pyarrow/vendored/version.py`

 * *Files identical despite different names*

### Comparing `pyarrow-8.0.0/pyarrow.egg-info/PKG-INFO` & `pyarrow-9.0.0/pyarrow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarrow
-Version: 8.0.0
+Version: 9.0.0
 Summary: Python library for Apache Arrow
 Home-page: https://arrow.apache.org/
 Maintainer: Apache Arrow Developers
 Maintainer-email: dev@arrow.apache.org
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://arrow.apache.org/docs/python
 Project-URL: Source, https://github.com/apache/arrow
```

### Comparing `pyarrow-8.0.0/pyarrow.egg-info/SOURCES.txt` & `pyarrow-9.0.0/pyarrow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,38 +14,37 @@
 cmake_modules/FindArrowFlight.cmake
 cmake_modules/FindArrowFlightSql.cmake
 cmake_modules/FindArrowFlightTesting.cmake
 cmake_modules/FindArrowPython.cmake
 cmake_modules/FindArrowPythonFlight.cmake
 cmake_modules/FindArrowSubstrait.cmake
 cmake_modules/FindArrowTesting.cmake
-cmake_modules/FindBoostAlt.cmake
 cmake_modules/FindBrotli.cmake
 cmake_modules/FindClangTools.cmake
 cmake_modules/FindGLOG.cmake
 cmake_modules/FindGandiva.cmake
 cmake_modules/FindInferTools.cmake
 cmake_modules/FindLLVMAlt.cmake
-cmake_modules/FindLz4.cmake
 cmake_modules/FindNumPy.cmake
 cmake_modules/FindORC.cmake
 cmake_modules/FindOpenSSLAlt.cmake
 cmake_modules/FindParquet.cmake
 cmake_modules/FindPlasma.cmake
 cmake_modules/FindPython3Alt.cmake
 cmake_modules/FindPythonLibsNew.cmake
 cmake_modules/FindRapidJSONAlt.cmake
 cmake_modules/FindSQLite3Alt.cmake
-cmake_modules/FindSnappy.cmake
+cmake_modules/FindSnappyAlt.cmake
 cmake_modules/FindThrift.cmake
 cmake_modules/Findc-aresAlt.cmake
 cmake_modules/FindgRPCAlt.cmake
 cmake_modules/FindgflagsAlt.cmake
 cmake_modules/Findjemalloc.cmake
 cmake_modules/Findlibrados.cmake
+cmake_modules/Findlz4Alt.cmake
 cmake_modules/Findre2Alt.cmake
 cmake_modules/Findutf8proc.cmake
 cmake_modules/Findzstd.cmake
 cmake_modules/SetupCxxFlags.cmake
 cmake_modules/ThirdpartyToolchain.cmake
 cmake_modules/UseCython.cmake
 cmake_modules/Usevcpkg.cmake
@@ -64,35 +63,37 @@
 pyarrow/_dataset_orc.pyx
 pyarrow/_dataset_parquet.pyx
 pyarrow/_exec_plan.pyx
 pyarrow/_feather.pyx
 pyarrow/_flight.pyx
 pyarrow/_fs.pxd
 pyarrow/_fs.pyx
+pyarrow/_gcsfs.pyx
 pyarrow/_generated_version.py
 pyarrow/_hdfs.pyx
 pyarrow/_hdfsio.pyx
 pyarrow/_json.pyx
 pyarrow/_orc.pxd
 pyarrow/_orc.pyx
 pyarrow/_parquet.pxd
 pyarrow/_parquet.pyx
 pyarrow/_parquet_encryption.pxd
 pyarrow/_parquet_encryption.pyx
 pyarrow/_plasma.pyx
 pyarrow/_s3fs.pyx
+pyarrow/_substrait.pyx
 pyarrow/array.pxi
 pyarrow/benchmark.pxi
 pyarrow/benchmark.py
 pyarrow/builder.pxi
 pyarrow/cffi.py
 pyarrow/compat.pxi
-pyarrow/compat.py
 pyarrow/compute.py
 pyarrow/config.pxi
+pyarrow/conftest.py
 pyarrow/csv.py
 pyarrow/cuda.py
 pyarrow/dataset.py
 pyarrow/error.pxi
 pyarrow/feather.py
 pyarrow/filesystem.py
 pyarrow/flight.py
@@ -111,14 +112,15 @@
 pyarrow/pandas-shim.pxi
 pyarrow/pandas_compat.py
 pyarrow/plasma.py
 pyarrow/public-api.pxi
 pyarrow/scalar.pxi
 pyarrow/serialization.pxi
 pyarrow/serialization.py
+pyarrow/substrait.py
 pyarrow/table.pxi
 pyarrow/tensor.pxi
 pyarrow/types.pxi
 pyarrow/types.py
 pyarrow/util.py
 pyarrow.egg-info/PKG-INFO
 pyarrow.egg-info/SOURCES.txt
@@ -133,20 +135,22 @@
 pyarrow/includes/libarrow_cuda.pxd
 pyarrow/includes/libarrow_dataset.pxd
 pyarrow/includes/libarrow_dataset_parquet.pxd
 pyarrow/includes/libarrow_feather.pxd
 pyarrow/includes/libarrow_flight.pxd
 pyarrow/includes/libarrow_fs.pxd
 pyarrow/includes/libarrow_python.pxd
+pyarrow/includes/libarrow_substrait.pxd
 pyarrow/includes/libgandiva.pxd
 pyarrow/includes/libplasma.pxd
 pyarrow/parquet/__init__.py
 pyarrow/parquet/encryption.py
 pyarrow/tensorflow/plasma_op.cc
 pyarrow/tests/__init__.py
+pyarrow/tests/arrow_16597.py
 pyarrow/tests/arrow_7980.py
 pyarrow/tests/bound_function_visit_strings.pyx
 pyarrow/tests/conftest.py
 pyarrow/tests/deserialize_buffer.py
 pyarrow/tests/pandas_examples.py
 pyarrow/tests/pandas_threaded_import.py
 pyarrow/tests/pyarrow_cython_example.pyx
@@ -185,17 +189,19 @@
 pyarrow/tests/test_plasma_tf_op.py
 pyarrow/tests/test_scalars.py
 pyarrow/tests/test_schema.py
 pyarrow/tests/test_serialization.py
 pyarrow/tests/test_serialization_deprecated.py
 pyarrow/tests/test_sparse_tensor.py
 pyarrow/tests/test_strategies.py
+pyarrow/tests/test_substrait.py
 pyarrow/tests/test_table.py
 pyarrow/tests/test_tensor.py
 pyarrow/tests/test_types.py
+pyarrow/tests/test_udf.py
 pyarrow/tests/test_util.py
 pyarrow/tests/util.py
 pyarrow/tests/data/feather/v0.17.0.version.2-compression.lz4.feather
 pyarrow/tests/data/orc/README.md
 pyarrow/tests/data/orc/TestOrcFile.emptyFile.jsn.gz
 pyarrow/tests/data/orc/TestOrcFile.emptyFile.orc
 pyarrow/tests/data/orc/TestOrcFile.test1.jsn.gz
```

### Comparing `pyarrow-8.0.0/pyproject.toml` & `pyarrow-9.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 # under the License.
 
 [build-system]
 requires = [
     "cython >= 0.29.22",
     "oldest-supported-numpy>=0.14",
     "setuptools_scm",
-    "setuptools >= 38.6.0",
+    "setuptools >= 40.1.0",
     "wheel"
 ]
```

### Comparing `pyarrow-8.0.0/setup.py` & `pyarrow-9.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 if sys.version_info >= (3, 10):
     import sysconfig
 else:
     # Get correct EXT_SUFFIX on Windows (https://bugs.python.org/issue39825)
     from distutils import sysconfig
 
 import pkg_resources
-from setuptools import setup, Extension, Distribution
+from setuptools import setup, Extension, Distribution, find_namespace_packages
 
 from Cython.Distutils import build_ext as _build_ext
 import Cython
 
 # Check if we're running 64-bit Python
 is_64_bit = sys.maxsize > 2**32
 
@@ -104,18 +104,21 @@
                      ('extra-cmake-args=', None, 'extra arguments for CMake'),
                      ('build-type=', None,
                       'build type (debug or release), default release'),
                      ('boost-namespace=', None,
                       'namespace of boost (default: boost)'),
                      ('with-cuda', None, 'build the Cuda extension'),
                      ('with-flight', None, 'build the Flight extension'),
+                     ('with-substrait', None, 'build the Substrait extension'),
                      ('with-dataset', None, 'build the Dataset extension'),
                      ('with-parquet', None, 'build the Parquet extension'),
                      ('with-parquet-encryption', None,
                       'build the Parquet encryption extension'),
+                     ('with-gcs', None,
+                      'build the Google Cloud Storage (GCS) extension'),
                      ('with-s3', None, 'build the Amazon S3 extension'),
                      ('with-static-parquet', None, 'link parquet statically'),
                      ('with-static-boost', None, 'link boost statically'),
                      ('with-plasma', None, 'build the Plasma extension'),
                      ('with-tensorflow', None,
                       'build pyarrow with TensorFlow support'),
                      ('with-orc', None, 'build the ORC extension'),
@@ -150,20 +153,24 @@
 
         if sys.platform == 'win32':
             # Cannot do debug builds in Windows unless Python itself is a debug
             # build
             if not hasattr(sys, 'gettotalrefcount'):
                 self.build_type = 'release'
 
+        self.with_gcs = strtobool(
+            os.environ.get('PYARROW_WITH_GCS', '0'))
         self.with_s3 = strtobool(
             os.environ.get('PYARROW_WITH_S3', '0'))
         self.with_hdfs = strtobool(
             os.environ.get('PYARROW_WITH_HDFS', '0'))
         self.with_cuda = strtobool(
             os.environ.get('PYARROW_WITH_CUDA', '0'))
+        self.with_substrait = strtobool(
+            os.environ.get('PYARROW_WITH_SUBSTRAIT', '0'))
         self.with_flight = strtobool(
             os.environ.get('PYARROW_WITH_FLIGHT', '0'))
         self.with_dataset = strtobool(
             os.environ.get('PYARROW_WITH_DATASET', '0'))
         self.with_parquet = strtobool(
             os.environ.get('PYARROW_WITH_PARQUET', '0'))
         self.with_static_parquet = strtobool(
@@ -209,15 +216,17 @@
         '_dataset_parquet',
         '_exec_plan',
         '_feather',
         '_parquet',
         '_parquet_encryption',
         '_orc',
         '_plasma',
+        '_gcsfs',
         '_s3fs',
+        '_substrait',
         '_hdfs',
         '_hdfsio',
         'gandiva']
 
     def _run_cmake(self):
         # check if build_type is correctly passed / set
         if self.build_type.lower() not in ('release', 'debug'):
@@ -241,14 +250,19 @@
             # Detect if we built elsewhere
             if os.path.isfile('CMakeCache.txt'):
                 cachefile = open('CMakeCache.txt', 'r')
                 cachedir = re.search('CMAKE_CACHEFILE_DIR:INTERNAL=(.*)',
                                      cachefile.read()).group(1)
                 cachefile.close()
                 if (cachedir != build_temp):
+                    build_base = pjoin(saved_cwd, build_cmd.build_base)
+                    print(f"-- Skipping build. Temp build {build_temp} does "
+                          f"not match cached dir {cachedir}")
+                    print("---- For a clean build you might want to delete "
+                          f"{build_base}.")
                     return
 
             static_lib_option = ''
 
             cmake_options = [
                 '-DPYTHON_EXECUTABLE=%s' % sys.executable,
                 '-DPython3_EXECUTABLE=%s' % sys.executable,
@@ -259,22 +273,24 @@
                 cmake_options.append('-D{0}={1}'.format(
                     varname, 'on' if value else 'off'))
 
             if self.cmake_generator:
                 cmake_options += ['-G', self.cmake_generator]
 
             append_cmake_bool(self.with_cuda, 'PYARROW_BUILD_CUDA')
+            append_cmake_bool(self.with_substrait, 'PYARROW_BUILD_SUBSTRAIT')
             append_cmake_bool(self.with_flight, 'PYARROW_BUILD_FLIGHT')
             append_cmake_bool(self.with_gandiva, 'PYARROW_BUILD_GANDIVA')
             append_cmake_bool(self.with_dataset, 'PYARROW_BUILD_DATASET')
             append_cmake_bool(self.with_orc, 'PYARROW_BUILD_ORC')
             append_cmake_bool(self.with_parquet, 'PYARROW_BUILD_PARQUET')
             append_cmake_bool(self.with_parquet_encryption,
                               'PYARROW_BUILD_PARQUET_ENCRYPTION')
             append_cmake_bool(self.with_plasma, 'PYARROW_BUILD_PLASMA')
+            append_cmake_bool(self.with_gcs, 'PYARROW_BUILD_GCS')
             append_cmake_bool(self.with_s3, 'PYARROW_BUILD_S3')
             append_cmake_bool(self.with_hdfs, 'PYARROW_BUILD_HDFS')
             append_cmake_bool(self.with_tensorflow, 'PYARROW_USE_TENSORFLOW')
             append_cmake_bool(self.bundle_arrow_cpp,
                               'PYARROW_BUNDLE_ARROW_CPP')
             append_cmake_bool(self.bundle_boost,
                               'PYARROW_BUNDLE_BOOST')
@@ -384,14 +400,16 @@
 
     def _bundle_arrow_cpp(self, build_prefix, build_lib):
         print(pjoin(build_lib, 'pyarrow'))
         move_shared_libs(build_prefix, build_lib, "arrow")
         move_shared_libs(build_prefix, build_lib, "arrow_python")
         if self.with_cuda:
             move_shared_libs(build_prefix, build_lib, "arrow_cuda")
+        if self.with_substrait:
+            move_shared_libs(build_prefix, build_lib, "arrow_substrait")
         if self.with_flight:
             move_shared_libs(build_prefix, build_lib, "arrow_flight")
             move_shared_libs(build_prefix, build_lib,
                              "arrow_python_flight")
         if self.with_dataset:
             move_shared_libs(build_prefix, build_lib, "arrow_dataset")
         if self.with_plasma:
@@ -429,14 +447,18 @@
             return True
         if name == '_plasma' and not self.with_plasma:
             return True
         if name == '_orc' and not self.with_orc:
             return True
         if name == '_flight' and not self.with_flight:
             return True
+        if name == '_substrait' and not self.with_substrait:
+            return True
+        if name == '_gcsfs' and not self.with_gcs:
+            return True
         if name == '_s3fs' and not self.with_s3:
             return True
         if name == '_hdfs' and not self.with_hdfs:
             return True
         if name == '_dataset' and not self.with_dataset:
             return True
         if name == '_dataset_orc' and not (
@@ -541,15 +563,15 @@
     lib_filename = os.path.basename(libs[0])
     shutil.move(pjoin(build_prefix, lib_filename),
                 pjoin(build_lib, 'pyarrow', lib_filename))
 
 
 # If the event of not running from a git clone (e.g. from a git archive
 # or a Python sdist), see if we can set the version number ourselves
-default_version = '8.0.0'
+default_version = '9.0.0'
 if (not os.path.exists('../.git') and
         not os.environ.get('SETUPTOOLS_SCM_PRETEND_VERSION')):
     os.environ['SETUPTOOLS_SCM_PRETEND_VERSION'] = \
         default_version.replace('-SNAPSHOT', 'a0')
 
 
 # See https://github.com/pypa/setuptools_scm#configuration-parameters
@@ -595,17 +617,18 @@
 if {'pytest', 'test', 'ptr'}.intersection(sys.argv):
     setup_requires = ['pytest-runner']
 else:
     setup_requires = []
 
 
 if strtobool(os.environ.get('PYARROW_INSTALL_TESTS', '1')):
-    packages = ['pyarrow', 'pyarrow.tests']
+    packages = find_namespace_packages(include=['pyarrow*'])
 else:
-    packages = ['pyarrow']
+    packages = find_namespace_packages(include=['pyarrow*'],
+                                       exclude=["pyarrow.tests*"])
 
 
 setup(
     name='pyarrow',
     packages=packages,
     zip_safe=False,
     package_data={'pyarrow': ['*.pxd', '*.pyx', 'includes/*.pxd']},
```

