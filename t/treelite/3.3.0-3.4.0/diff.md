# Comparing `tmp/treelite-3.3.0.tar.gz` & `tmp/treelite-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treelite-3.3.0.tar", last modified: Fri Apr 28 00:37:19 2023, max compression
+gzip compressed data, was "treelite-3.4.0.tar", last modified: Tue May  2 03:53:10 2023, max compression
```

## Comparing `treelite-3.3.0.tar` & `treelite-3.4.0.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 00:36:18.000000 treelite-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 00:37:19.619170 treelite-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:37:19.619170 treelite-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-28 00:36:18.000000 treelite-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Doxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/ExternalLibs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/FetchContentMakeAvailable.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Python_version.in
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Version.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/version.h.in
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/gcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/msvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    45355 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gallery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gallery/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gallery/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gtil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gtil/gtil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.603170 treelite-3.3.0/treelite/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/include/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/annotator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/base.h
--rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_error.h
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/compiler_param.h
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/data.h
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/frontend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/frontend_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/gtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/math.h
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/omp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/omp_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/optional.h
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/predictor.h
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/thread_local.h
--rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/tree_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/typeinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/libpath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/serialize/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/annotator.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/src/c_api/
--rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_common.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_error.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_runtime.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/ast/
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/ast.h
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/build.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/dump.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/fold_code.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/is_categorical_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/load_data_counts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/quantize.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/split.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast_native.cc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast_native.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/categorical_bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/code_folding_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/format_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/compiler.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/elf/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/failsafe.cc
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/failsafe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/native/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/code_folder_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/header_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/main_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/qnode_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/typeinfo_ctypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/filesystem.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/json_importer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/lightgbm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/sklearn.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/frontend/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost/xgboost.h
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost/xgboost_json.h
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost.cc
--rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/config.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/json_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/model_concat.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/predictor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/treelite/src/predictor/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/thread_pool/spsc_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/thread_pool/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/serializer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/treelite/src/threading_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/threading_utils/parallel_for.h
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/typeinfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-02 03:52:46.000000 treelite-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 03:53:10.835741 treelite-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:53:10.835741 treelite-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-02 03:52:46.000000 treelite-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/ExternalLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/FetchContentMakeAvailable.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Python_version.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/version.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/gcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/msvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gallery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gallery/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gallery/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gtil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gtil/gtil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.819741 treelite-3.4.0/treelite/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/include/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/annotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/compiler_param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/frontend_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/gtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/omp_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/optional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/predictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/thread_local.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/tree_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/typeinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/libpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/serialize/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/annotator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/c_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_error.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_runtime.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/build.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/dump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/fold_code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/is_categorical_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/load_data_counts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/quantize.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/split.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast_native.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast_native.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/categorical_bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/code_folding_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/format_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/compiler.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/failsafe.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/failsafe.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/compiler/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/code_folder_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/header_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/main_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/qnode_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/typeinfo_ctypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/filesystem.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/json_importer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/lightgbm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/sklearn.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/frontend/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost/xgboost.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost/xgboost_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/config.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/json_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/model_concat.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/predictor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/predictor/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/thread_pool/spsc_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/thread_pool/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/serializer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/threading_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/threading_utils/parallel_for.h
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/typeinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/top_level.txt
```

### Comparing `treelite-3.3.0/PKG-INFO` & `treelite-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.3.0
+Version: 3.4.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.3.0/setup.py` & `treelite-3.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # coding: utf-8
 """Setup Treelite package."""
 import os
 import shutil
 import subprocess
 import collections
 import logging
+import sys
 from platform import system
 from setuptools import setup, find_packages, Extension
 from setuptools.command import build_ext, sdist, install_lib, install
 
 CURRENT_DIR = os.path.abspath(os.path.dirname(__file__))
 
 UserOption = collections.namedtuple('UserOption', 'description is_boolean value')
 
 USER_OPTIONS = {
     'cmake-build-dir': UserOption(description='Build directory used for CMake build',
-                                  value='build', is_boolean=False)
+                                  value='build', is_boolean=False),
+    'use-system-libtreelite': UserOption(description='Use libtreelite.so from system path',
+                                         value=False, is_boolean=True)
 }
 
 NEED_CLEAN_TREE = set()
 NEED_CLEAN_FILE = set()
 BUILD_TEMP_DIR = None
 
 
@@ -113,14 +116,17 @@
             subprocess.check_call(build_cmd, cwd=build_dir)
         else:
             subprocess.check_call(['cmake', '--build', '.', '--config', 'Release',
                                    '--target', 'treelite'], cwd=build_dir)
 
     def build_cmake_extension(self):
         """Configure and build using CMake"""
+        if USER_OPTIONS['use-system-libtreelite'].value:
+            self.logger.info('Using system libtreelite.')
+            return
         src_dir = 'treelite'
         try:
             copy_tree(os.path.join(CURRENT_DIR, os.path.pardir),
                       os.path.join(self.build_temp, src_dir))
         except Exception:  # pylint: disable=broad-except
             copy_tree(src_dir, os.path.join(self.build_temp, src_dir))
         build_dir = self.build_temp
@@ -174,17 +180,24 @@
 
 
 class InstallLib(install_lib.install_lib):
     """Install native library into Python package"""
     logger = logging.getLogger('Treelite install_lib')
 
     def install(self):
-
         outfiles = super().install()
 
+        if USER_OPTIONS['use-system-libtreelite'].value:
+            self.logger.info('Using system libtreelite.')
+            lib_path = os.path.join(sys.prefix, 'lib')
+            msg = 'use-system-libtreelite is specified, but ' + lib_name() + \
+                  ' is not found in: ' + lib_path
+            assert os.path.exists(os.path.join(lib_path, lib_name())), msg
+            return []
+
         # Copy shared library
         libtreelite_name = lib_name()
         dst_dir = os.path.join(self.install_dir, 'treelite', 'lib')
         if not os.path.exists(dst_dir):
             os.mkdir(dst_dir)
         dst = os.path.join(dst_dir, libtreelite_name)
         # CMake build dir is specified relative to the project root directory
@@ -251,15 +264,15 @@
     # - python setup.py bdist_wheel && pip install <wheel-name>
     with open(os.path.join(CURRENT_DIR, 'treelite/VERSION'), 'r', encoding='UTF-8') as f:
         version = f.read().strip()
     logging.basicConfig(level=logging.INFO)
     setup(name='treelite',
           version=version,
           description='Treelite: model compiler for decision trees',
-          install_requires=['numpy', 'scipy'],
+          install_requires=['numpy', 'scipy', 'packaging'],
           ext_modules=[CMakeExtension('libtreelite')],
           cmdclass={
               'build_ext': BuildExt,
               'sdist': SDist,
               'install_lib': InstallLib,
               'install': Install
           },
```

### Comparing `treelite-3.3.0/treelite/CMakeLists.txt` & `treelite-3.4.0/treelite/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,48 @@
-set (CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
-cmake_minimum_required (VERSION 3.13)
-project(treelite LANGUAGES CXX C VERSION 3.3.0)
+cmake_policy(SET CMP0091 NEW)
+set(CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
+cmake_minimum_required (VERSION 3.16)
+project(treelite LANGUAGES CXX C VERSION 3.4.0)
 
 # check MSVC version
 if(MSVC)
-  if(MSVC_VERSION LESS 1910)
-    message(FATAL_ERROR "Need Visual Studio 2017 or newer to compile Treelite")
+  if(MSVC_VERSION LESS 1920)
+    message(FATAL_ERROR "Need Visual Studio 2019 or newer to compile Treelite")
   endif()
 endif()
 
+# Options useful for downstream projects
+option(Treelite_BUILD_STATIC_LIBS "Build static libs, in addition to dynamic libs" OFF)
+option(Treelite_USE_DYNAMIC_MSVC_RUNTIME
+    "Whether to dynamically link MSVC runtime. ON: Use dynamic link (-MD), OFF: Use static link (-MT)"
+    OFF)
+
+# Developer options
 option(TEST_COVERAGE "C++ test coverage" OFF)
 option(USE_OPENMP "Use OpenMP" ON)
 option(BUILD_DOXYGEN "Build documentation for C/C++ functions using Doxygen." OFF)
 option(BUILD_CPP_TEST "Build C++ tests" OFF)
-option(BUILD_STATIC_LIBS "Build static libs, in addition to dynamic libs" OFF)
 option(DETECT_CONDA_ENV "Enable detection of conda environment for dependencies" ON)
+option(HIDE_CXX_SYMBOLS "Hide all C++ symbols. Useful when building Pip package" OFF)
 option(BUILD_JVM_RUNTIME "Build Treelite runtime for JVM" OFF)
 option(ENABLE_ALL_WARNINGS "Enable all compiler warnings. Only effective for GCC/Clang" OFF)
 option(USE_SANITIZER "Use sanitizer flags" OFF)
 SET(ENABLED_SANITIZERS "address" "leak" "undefined" CACHE STRING
         "Semicolon separated list of sanitizer names. E.g 'address;leak'.")
 
+if(MSVC)
+  if(Treelite_USE_DYNAMIC_MSVC_RUNTIME)
+    message(STATUS "Using dynamically linked MSVC runtime...")
+    set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>DLL")
+  else()
+    message(STATUS "Using statically linked MSVC runtime...")
+    set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
+  endif()
+endif()
+
 if(USE_SANITIZER)
   include(cmake/Sanitizer.cmake)
   enable_sanitizers("${ENABLED_SANITIZERS}")
 endif()
 
 if(ENABLE_ALL_WARNINGS)
   if((NOT CMAKE_CXX_COMPILER_ID MATCHES "Clang") AND (NOT CMAKE_CXX_COMPILER_ID STREQUAL "GNU"))
@@ -66,15 +84,15 @@
 add_library(treelite SHARED)
 add_library(treelite_runtime SHARED)
 target_link_libraries(treelite PRIVATE objtreelite objtreelite_common)
 target_link_libraries(treelite_runtime PRIVATE objtreelite_runtime objtreelite_common)
 
 set(TREELITE_TARGETS treelite treelite_runtime)
 
-if(BUILD_STATIC_LIBS)
+if(Treelite_BUILD_STATIC_LIBS)
   add_library(treelite_static STATIC)
   add_library(treelite_runtime_static STATIC)
   target_link_libraries(treelite_static PRIVATE objtreelite objtreelite_common)
   target_link_libraries(treelite_runtime_static PRIVATE objtreelite_runtime objtreelite_common)
   list(APPEND TREELITE_TARGETS treelite_static treelite_runtime_static)
 endif()
 
@@ -114,8 +132,7 @@
     ${PROJECT_BINARY_DIR}/cmake/TreeliteConfig.cmake
     ${PROJECT_BINARY_DIR}/cmake/TreeliteConfigVersion.cmake
     DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/treelite)
 
 write_version()
 
 set_default_configuration_release()
-msvc_use_static_runtime()
```

### Comparing `treelite-3.3.0/treelite/LICENSE` & `treelite-3.4.0/treelite/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/__init__.py` & `treelite-3.4.0/treelite/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/annotator.py` & `treelite-3.4.0/treelite/annotator.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/cmake/ExternalLibs.cmake` & `treelite-3.4.0/treelite/cmake/ExternalLibs.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/cmake/Sanitizer.cmake` & `treelite-3.4.0/treelite/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/cmake/Utils.cmake` & `treelite-3.4.0/treelite/cmake/Utils.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -9,32 +9,14 @@
       string(REPLACE "/" "\\\\" GROUP "${GROUP}")
       string(REGEX REPLACE "^\\\\" "" GROUP "${GROUP}")
 
       source_group("${GROUP}" FILES "${FILE}")
   endforeach()
 endfunction(auto_source_group)
 
-# Force static runtime for MSVC
-function(msvc_use_static_runtime)
-  if(MSVC)
-    set(variables
-        CMAKE_CXX_FLAGS_DEBUG
-        CMAKE_CXX_FLAGS_MINSIZEREL
-        CMAKE_CXX_FLAGS_RELEASE
-        CMAKE_CXX_FLAGS_RELWITHDEBINFO
-    )
-    foreach(variable ${variables})
-      if(${variable} MATCHES "/MD")
-        string(REGEX REPLACE "/MD" "/MT" ${variable} "${${variable}}")
-        set(${variable} "${${variable}}"  PARENT_SCOPE)
-      endif()
-    endforeach()
-  endif()
-endfunction(msvc_use_static_runtime)
-
 # Set output directory of target, ignoring debug or release
 function(set_output_directory target dir)
   set_target_properties(${target} PROPERTIES
     RUNTIME_OUTPUT_DIRECTORY ${dir}              # for executable
     RUNTIME_OUTPUT_DIRECTORY_DEBUG ${dir}
     RUNTIME_OUTPUT_DIRECTORY_RELEASE ${dir}
     LIBRARY_OUTPUT_DIRECTORY ${dir}              # for shared library
```

### Comparing `treelite-3.3.0/treelite/cmake/Version.cmake` & `treelite-3.4.0/treelite/cmake/Version.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/contrib/__init__.py` & `treelite-3.4.0/treelite/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/contrib/gcc.py` & `treelite-3.4.0/treelite/contrib/gcc.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/contrib/msvc.py` & `treelite-3.4.0/treelite/contrib/msvc.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Tools to interact with Microsoft Visual C++ (MSVC) toolchain
 """
 
 from __future__ import absolute_import as _abs
 import os
 import glob
 import re
-from pkg_resources import parse_version
+from packaging.version import parse as parse_version
 from .util import _create_shared_base, _libext
 
 LIBEXT = _libext()
 
 
 def _is_64bit_windows():
     return 'PROGRAMFILES(X86)' in os.environ
```

### Comparing `treelite-3.3.0/treelite/contrib/util.py` & `treelite-3.4.0/treelite/contrib/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/core.py` & `treelite-3.4.0/treelite/core.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/frontend.py` & `treelite-3.4.0/treelite/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import collections
 import shutil
 import os
 import json
 from tempfile import TemporaryDirectory
 from typing import Union, List, Optional
 
-from pkg_resources import parse_version
+from packaging.version import parse as parse_version
 
 import numpy as np
 
 from .util import c_str, py_str, TreeliteError, type_info_to_ctypes_type, type_info_to_numpy_type
 from .core import _LIB, c_array, _check_call
 from .contrib import create_shared, generate_makefile, generate_cmakelists, _toolchain_exist_check
 
@@ -535,16 +535,17 @@
             import lightgbm
         except ImportError as e:
             raise TreeliteError('lightgbm module must be installed to read from ' +
                                 '`lightgbm.Booster` object') from e
         if not isinstance(booster, lightgbm.Booster):
             raise ValueError('booster must be of type `lightgbm.Booster`')
         model_str = booster.model_to_string()
-        _check_call(_LIB.TreeliteLoadLightGBMModelFromString(
+        _check_call(_LIB.TreeliteLoadLightGBMModelFromStringEx(
             c_str(model_str),
+            c_str("{}"),
             ctypes.byref(handle)))
         return Model(handle)
 
     @classmethod
     def load(
         cls,
         filename: str,
```

### Comparing `treelite-3.3.0/treelite/gtil/gtil.py` & `treelite-3.4.0/treelite/gtil/gtil.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/annotator.h` & `treelite-3.4.0/treelite/include/treelite/annotator.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/base.h` & `treelite-3.4.0/treelite/include/treelite/base.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/c_api.h` & `treelite-3.4.0/treelite/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/c_api_common.h` & `treelite-3.4.0/treelite/include/treelite/c_api_common.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/c_api_error.h` & `treelite-3.4.0/treelite/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/c_api_runtime.h` & `treelite-3.4.0/treelite/include/treelite/c_api_runtime.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/compiler.h` & `treelite-3.4.0/treelite/include/treelite/compiler.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/compiler_param.h` & `treelite-3.4.0/treelite/include/treelite/compiler_param.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/data.h` & `treelite-3.4.0/treelite/include/treelite/data.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/filesystem.h` & `treelite-3.4.0/treelite/include/treelite/filesystem.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/frontend.h` & `treelite-3.4.0/treelite/include/treelite/frontend.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/frontend_impl.h` & `treelite-3.4.0/treelite/include/treelite/frontend_impl.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/gtil.h` & `treelite-3.4.0/treelite/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/logging.h` & `treelite-3.4.0/treelite/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/math.h` & `treelite-3.4.0/treelite/include/treelite/math.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/omp.h` & `treelite-3.4.0/treelite/include/treelite/omp.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/omp_exception.h` & `treelite-3.4.0/treelite/include/treelite/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/optional.h` & `treelite-3.4.0/treelite/include/treelite/optional.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/predictor.h` & `treelite-3.4.0/treelite/include/treelite/predictor.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/thread_local.h` & `treelite-3.4.0/treelite/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/tree.h` & `treelite-3.4.0/treelite/include/treelite/tree.h`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,21 @@
 namespace treelite {
 
 class GTILBridge;
 
 template <typename ThresholdType, typename LeafOutputType>
 class ModelImpl;
 
+// Used for returning version triple from a Model object
+struct Version {
+  std::int32_t major_ver;
+  std::int32_t minor_ver;
+  std::int32_t patch_ver;
+};
+
 // Represent a frame in the Python buffer protocol (PEP 3118). We use a simplified representation
 // to hold only 1-D arrays with stride 1.
 struct PyBufferFrame {
   void* buf;
   char* format;
   std::size_t itemsize;
   std::size_t nitem;
@@ -805,14 +812,18 @@
   TREELITE_DLL_EXPORT std::vector<PyBufferFrame> GetPyBuffer();
   TREELITE_DLL_EXPORT static std::unique_ptr<Model>
     CreateFromPyBuffer(std::vector<PyBufferFrame> frames);
 
   /* Serialization to a file stream */
   void SerializeToStream(std::ostream& os);
   static std::unique_ptr<Model> DeserializeFromStream(std::istream& is);
+  /*! \brief Return the Treelite version that produced this Model object. */
+  inline Version GetVersion() const {
+    return {major_ver_, minor_ver_, patch_ver_};
+  }
 
   /*!
    * \brief number of features used for the model.
    * It is assumed that all feature indices are between 0 and [num_feature]-1.
    */
   int32_t num_feature{0};
   /*! \brief Task type */
```

### Comparing `treelite-3.3.0/treelite/include/treelite/tree_impl.h` & `treelite-3.4.0/treelite/include/treelite/tree_impl.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/include/treelite/typeinfo.h` & `treelite-3.4.0/treelite/include/treelite/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/libpath.py` & `treelite-3.4.0/treelite/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/serialize/__main__.py` & `treelite-3.4.0/treelite/serialize/__main__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/__init__.py` & `treelite-3.4.0/treelite/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/common.py` & `treelite-3.4.0/treelite/sklearn/common.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/gbm_classifier.py` & `treelite-3.4.0/treelite/sklearn/gbm_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/gbm_multi_classifier.py` & `treelite-3.4.0/treelite/sklearn/gbm_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/gbm_regressor.py` & `treelite-3.4.0/treelite/sklearn/gbm_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/importer.py` & `treelite-3.4.0/treelite/sklearn/importer.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/rf_classifier.py` & `treelite-3.4.0/treelite/sklearn/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/rf_multi_classifier.py` & `treelite-3.4.0/treelite/sklearn/rf_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/sklearn/rf_regressor.py` & `treelite-3.4.0/treelite/sklearn/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/CMakeLists.txt` & `treelite-3.4.0/treelite/src/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,21 @@
 
 set_target_properties(objtreelite objtreelite_runtime objtreelite_common
   PROPERTIES
   POSITION_INDEPENDENT_CODE ON
   CXX_STANDARD 17
   CXX_STANDARD_REQUIRED ON)
 
+if(HIDE_CXX_SYMBOLS)
+  set_target_properties(objtreelite objtreelite_runtime objtreelite_common
+    PROPERTIES
+    C_VISIBILITY_PRESET hidden
+    CXX_VISIBILITY_PRESET hidden)
+endif(HIDE_CXX_SYMBOLS)
+
 target_sources(objtreelite
     PRIVATE
     c_api/c_api.cc
     compiler/ast/ast.h
     compiler/ast/build.cc
     compiler/ast/builder.h
     compiler/ast/dump.cc
@@ -162,12 +169,10 @@
     ${PROJECT_SOURCE_DIR}/include/treelite/logging.h
     ${PROJECT_SOURCE_DIR}/include/treelite/math.h
     ${PROJECT_SOURCE_DIR}/include/treelite/omp_exception.h
     ${PROJECT_SOURCE_DIR}/include/treelite/typeinfo.h
     ${PROJECT_SOURCE_DIR}/include/treelite/data.h
 )
 
-msvc_use_static_runtime()
-
 # In MSVC solution, group sources according to directories
 file(GLOB_RECURSE ALL_SOURCES *.cc *.h)
 auto_source_group("${ALL_SOURCES}")
```

### Comparing `treelite-3.3.0/treelite/src/annotator.cc` & `treelite-3.4.0/treelite/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/c_api/c_api.cc` & `treelite-3.4.0/treelite/src/c_api/c_api.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/c_api/c_api_common.cc` & `treelite-3.4.0/treelite/src/c_api/c_api_common.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/c_api/c_api_error.cc` & `treelite-3.4.0/treelite/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/c_api/c_api_runtime.cc` & `treelite-3.4.0/treelite/src/c_api/c_api_runtime.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/ast.h` & `treelite-3.4.0/treelite/src/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/build.cc` & `treelite-3.4.0/treelite/src/compiler/ast/build.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/builder.h` & `treelite-3.4.0/treelite/src/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/dump.cc` & `treelite-3.4.0/treelite/src/compiler/ast/dump.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/fold_code.cc` & `treelite-3.4.0/treelite/src/compiler/ast/fold_code.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/is_categorical_array.cc` & `treelite-3.4.0/treelite/src/compiler/ast/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/load_data_counts.cc` & `treelite-3.4.0/treelite/src/compiler/ast/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/quantize.cc` & `treelite-3.4.0/treelite/src/compiler/ast/quantize.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast/split.cc` & `treelite-3.4.0/treelite/src/compiler/ast/split.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast_native.cc` & `treelite-3.4.0/treelite/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/ast_native.h` & `treelite-3.4.0/treelite/src/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/common/categorical_bitmap.h` & `treelite-3.4.0/treelite/src/compiler/common/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/common/code_folding_util.h` & `treelite-3.4.0/treelite/src/compiler/common/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/common/format_util.h` & `treelite-3.4.0/treelite/src/compiler/common/format_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/compiler.cc` & `treelite-3.4.0/treelite/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.cc` & `treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.h` & `treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/failsafe.cc` & `treelite-3.4.0/treelite/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/failsafe.h` & `treelite-3.4.0/treelite/src/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/code_folder_template.h` & `treelite-3.4.0/treelite/src/compiler/native/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/header_template.h` & `treelite-3.4.0/treelite/src/compiler/native/header_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/main_template.h` & `treelite-3.4.0/treelite/src/compiler/native/main_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/pred_transform.h` & `treelite-3.4.0/treelite/src/compiler/native/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/qnode_template.h` & `treelite-3.4.0/treelite/src/compiler/native/qnode_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/native/typeinfo_ctypes.h` & `treelite-3.4.0/treelite/src/compiler/native/typeinfo_ctypes.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/pred_transform.cc` & `treelite-3.4.0/treelite/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/compiler/pred_transform.h` & `treelite-3.4.0/treelite/src/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/data.cc` & `treelite-3.4.0/treelite/src/data.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/filesystem.cc` & `treelite-3.4.0/treelite/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/builder.cc` & `treelite-3.4.0/treelite/src/frontend/builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/json_importer.cc` & `treelite-3.4.0/treelite/src/frontend/json_importer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/lightgbm.cc` & `treelite-3.4.0/treelite/src/frontend/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/sklearn.cc` & `treelite-3.4.0/treelite/src/frontend/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/xgboost/xgboost.h` & `treelite-3.4.0/treelite/src/frontend/xgboost/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/xgboost/xgboost_json.h` & `treelite-3.4.0/treelite/src/frontend/xgboost/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/xgboost.cc` & `treelite-3.4.0/treelite/src/frontend/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/xgboost_json.cc` & `treelite-3.4.0/treelite/src/frontend/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/frontend/xgboost_util.cc` & `treelite-3.4.0/treelite/src/frontend/xgboost_util.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/gtil/config.cc` & `treelite-3.4.0/treelite/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/gtil/pred_transform.cc` & `treelite-3.4.0/treelite/src/gtil/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/gtil/pred_transform.h` & `treelite-3.4.0/treelite/src/gtil/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/gtil/predict.cc` & `treelite-3.4.0/treelite/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/json_serializer.cc` & `treelite-3.4.0/treelite/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/logging.cc` & `treelite-3.4.0/treelite/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/model_concat.cc` & `treelite-3.4.0/treelite/src/model_concat.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/predictor/predictor.cc` & `treelite-3.4.0/treelite/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/predictor/thread_pool/spsc_queue.h` & `treelite-3.4.0/treelite/src/predictor/thread_pool/spsc_queue.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/predictor/thread_pool/thread_pool.h` & `treelite-3.4.0/treelite/src/predictor/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/serializer.cc` & `treelite-3.4.0/treelite/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/threading_utils/parallel_for.h` & `treelite-3.4.0/treelite/src/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/src/typeinfo.cc` & `treelite-3.4.0/treelite/src/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite/util.py` & `treelite-3.4.0/treelite/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.3.0/treelite.egg-info/PKG-INFO` & `treelite-3.4.0/treelite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.3.0
+Version: 3.4.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.3.0/treelite.egg-info/SOURCES.txt` & `treelite-3.4.0/treelite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 treelite/VERSION
 treelite/__init__.py
 treelite/annotator.py
 treelite/compat.py
 treelite/core.py
 treelite/frontend.py
 treelite/libpath.py
+treelite/py.typed
 treelite/util.py
 treelite.egg-info/PKG-INFO
 treelite.egg-info/SOURCES.txt
 treelite.egg-info/dependency_links.txt
 treelite.egg-info/not-zip-safe
 treelite.egg-info/requires.txt
 treelite.egg-info/top_level.txt
```

