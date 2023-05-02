# Comparing `tmp/treelite_runtime-3.3.0.tar.gz` & `tmp/treelite_runtime-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treelite_runtime-3.3.0.tar", last modified: Fri Apr 28 00:37:20 2023, max compression
+gzip compressed data, was "treelite_runtime-3.4.0.tar", last modified: Tue May  2 03:53:11 2023, max compression
```

## Comparing `treelite_runtime-3.3.0.tar` & `treelite_runtime-3.4.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.995171 treelite_runtime-3.3.0/treelite_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.995171 treelite_runtime-3.3.0/treelite_runtime/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/Doxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/ExternalLibs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/FetchContentMakeAvailable.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/Python_version.in
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/Sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/Version.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/cmake/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.991171 treelite_runtime-3.3.0/treelite_runtime/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.999171 treelite_runtime-3.3.0/treelite_runtime/include/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/annotator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/base.h
--rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_error.h
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/compiler_param.h
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/data.h
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/frontend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/frontend_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/gtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/math.h
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/omp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/omp_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/optional.h
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/predictor.h
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/thread_local.h
--rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/tree_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/include/treelite/typeinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/libpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.999171 treelite_runtime-3.3.0/treelite_runtime/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/annotator.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.999171 treelite_runtime-3.3.0/treelite_runtime/src/c_api/
--rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_common.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_error.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_runtime.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/ast.h
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/build.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/dump.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/fold_code.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/load_data_counts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/quantize.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/split.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast_native.cc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast_native.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/categorical_bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/code_folding_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/format_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/compiler.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/compiler/elf/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/elf/elf_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/elf/elf_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/failsafe.cc
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/failsafe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/code_folder_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/header_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/main_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/qnode_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/compiler/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/filesystem.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/json_importer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/lightgbm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/sklearn.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.003171 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost/xgboost.h
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost.cc
--rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/treelite_runtime/src/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/gtil/config.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/gtil/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/gtil/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/gtil/predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/json_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/model_concat.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/treelite_runtime/src/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/predictor/predictor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/treelite_runtime/src/predictor/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/serializer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:20.007171 treelite_runtime-3.3.0/treelite_runtime/src/threading_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/threading_utils/parallel_for.h
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/src/typeinfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 00:36:18.000000 treelite_runtime-3.3.0/treelite_runtime/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.995171 treelite_runtime-3.3.0/treelite_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 00:37:19.000000 treelite_runtime-3.3.0/treelite_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/ExternalLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/FetchContentMakeAvailable.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Python_version.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.211741 treelite_runtime-3.4.0/treelite_runtime/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/include/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/annotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler_param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/gtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/optional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/predictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/thread_local.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/typeinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/libpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/annotator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/c_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_error.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_runtime.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/build.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/dump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/fold_code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/load_data_counts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/quantize.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/split.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/categorical_bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/code_folding_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/format_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/compiler.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/code_folder_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/header_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/main_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/qnode_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/filesystem.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/json_importer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/lightgbm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/sklearn.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/config.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/json_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/model_concat.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/predictor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/serializer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/parallel_for.h
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/typeinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/top_level.txt
```

### Comparing `treelite_runtime-3.3.0/PKG-INFO` & `treelite_runtime-3.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite_runtime
-Version: 3.3.0
+Version: 3.4.0
 Summary: Treelite runtime
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite_runtime-3.3.0/setup.py` & `treelite_runtime-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/CMakeLists.txt` & `treelite_runtime-3.4.0/treelite_runtime/CMakeLists.txt`

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

### Comparing `treelite_runtime-3.3.0/treelite_runtime/LICENSE` & `treelite_runtime-3.4.0/treelite_runtime/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/cmake/ExternalLibs.cmake` & `treelite_runtime-3.4.0/treelite_runtime/cmake/ExternalLibs.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/cmake/Sanitizer.cmake` & `treelite_runtime-3.4.0/treelite_runtime/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/cmake/Utils.cmake` & `treelite_runtime-3.4.0/treelite_runtime/cmake/Utils.cmake`

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

### Comparing `treelite_runtime-3.3.0/treelite_runtime/cmake/Version.cmake` & `treelite_runtime-3.4.0/treelite_runtime/cmake/Version.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/annotator.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/annotator.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/base.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/base.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_common.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_common.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_error.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/c_api_runtime.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_runtime.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/compiler.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/compiler_param.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler_param.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/data.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/data.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/filesystem.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/filesystem.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/frontend.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/frontend_impl.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend_impl.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/gtil.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/logging.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/math.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/math.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/omp.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/omp_exception.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/optional.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/optional.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/predictor.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/predictor.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/thread_local.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/tree.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree.h`

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

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/tree_impl.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree_impl.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/include/treelite/typeinfo.h` & `treelite_runtime-3.4.0/treelite_runtime/include/treelite/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/libpath.py` & `treelite_runtime-3.4.0/treelite_runtime/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/predictor.py` & `treelite_runtime-3.4.0/treelite_runtime/predictor.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/CMakeLists.txt` & `treelite_runtime-3.4.0/treelite_runtime/src/CMakeLists.txt`

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

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/annotator.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_common.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_common.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_error.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/c_api/c_api_runtime.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_runtime.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/ast.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/build.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/build.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/builder.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/dump.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/dump.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/fold_code.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/fold_code.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/load_data_counts.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/quantize.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/quantize.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast/split.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/split.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast_native.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/ast_native.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/categorical_bitmap.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/code_folding_util.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/common/format_util.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/format_util.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/compiler.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/elf/elf_formatter.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/elf/elf_formatter.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/failsafe.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/failsafe.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/code_folder_template.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/header_template.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/header_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/main_template.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/main_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/pred_transform.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/qnode_template.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/qnode_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/pred_transform.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/compiler/pred_transform.h` & `treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/data.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/data.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/filesystem.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/builder.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/builder.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/json_importer.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/json_importer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/lightgbm.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/sklearn.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost/xgboost.h` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost_json.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/frontend/xgboost_util.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_util.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/gtil/config.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/gtil/pred_transform.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/gtil/pred_transform.h` & `treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/gtil/predict.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/json_serializer.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/logging.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/model_concat.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/model_concat.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/predictor/predictor.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h` & `treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h` & `treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/serializer.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/threading_utils/parallel_for.h` & `treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/src/typeinfo.cc` & `treelite_runtime-3.4.0/treelite_runtime/src/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime/util.py` & `treelite_runtime-3.4.0/treelite_runtime/util.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.3.0/treelite_runtime.egg-info/PKG-INFO` & `treelite_runtime-3.4.0/treelite_runtime.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite-runtime
-Version: 3.3.0
+Version: 3.4.0
 Summary: Treelite runtime
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite_runtime-3.3.0/treelite_runtime.egg-info/SOURCES.txt` & `treelite_runtime-3.4.0/treelite_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

