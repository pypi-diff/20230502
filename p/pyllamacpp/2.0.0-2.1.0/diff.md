# Comparing `tmp/pyllamacpp-2.0.0.tar.gz` & `tmp/pyllamacpp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.0.0.tar", last modified: Thu Apr 27 03:41:35 2023, max compression
+gzip compressed data, was "pyllamacpp-2.1.0.tar", last modified: Tue May  2 00:53:34 2023, max compression
```

## Comparing `pyllamacpp-2.0.0.tar` & `pyllamacpp-2.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 03:41:23.000000 pyllamacpp-2.0.0/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.957341 pyllamacpp-2.0.0/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.965341 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.961341 pyllamacpp-2.0.0/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 03:41:35.000000 pyllamacpp-2.0.0/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:41:35.969342 pyllamacpp-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-27 03:41:22.000000 pyllamacpp-2.0.0/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 00:53:23.000000 pyllamacpp-2.1.0/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.323646 pyllamacpp-2.1.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.331646 pyllamacpp-2.1.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.327646 pyllamacpp-2.1.0/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 00:53:34.000000 pyllamacpp-2.1.0/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:53:34.335646 pyllamacpp-2.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26926 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-02 00:53:22.000000 pyllamacpp-2.1.0/src/main.h
```

### Comparing `pyllamacpp-2.0.0/CMakeLists.txt` & `pyllamacpp-2.1.0/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 cmake_minimum_required(VERSION 3.4...3.18)
+set(CMAKE_CXX_STANDARD 11)
+set(CMAKE_CXX_STANDARD_REQUIRED true)
+set(CMAKE_C_STANDARD 11)
+set(CMAKE_C_STANDARD_REQUIRED true)
+set(THREADS_PREFER_PTHREAD_FLAG ON)
+
 project(pyllamacpp)
 
 # fix  "undefined reference to `pthread_join'" in github action
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
 
 add_subdirectory(pybind11)
 add_subdirectory(llama.cpp)
@@ -79,19 +85,14 @@
 option(LLAMA_BUILD_TESTS            "llama: build tests"    ${LLAMA_STANDALONE})
 option(LLAMA_BUILD_EXAMPLES         "llama: build examples" ${LLAMA_STANDALONE})
 
 #
 # Compile flags
 #
 
-set(CMAKE_CXX_STANDARD 11)
-set(CMAKE_CXX_STANDARD_REQUIRED true)
-set(CMAKE_C_STANDARD 11)
-set(CMAKE_C_STANDARD_REQUIRED true)
-set(THREADS_PREFER_PTHREAD_FLAG ON)
 find_package(Threads REQUIRED)
 
 if (NOT MSVC)
     if (LLAMA_SANITIZE_THREAD)
         add_compile_options(-fsanitize=thread)
         link_libraries(-fsanitize=thread)
     endif()
```

### Comparing `pyllamacpp-2.0.0/LICENSE` & `pyllamacpp-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/PKG-INFO` & `pyllamacpp-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
-[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+
+<p align="center">
+  <img src="./docs/demo.gif">
+</p>
 
 
 For those who don't know, `llama.cpp` is a port of Facebook's LLaMA model in pure C/C++:
 
 <blockquote>
 
 - Without dependencies
@@ -35,15 +39,16 @@
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [CLI](#cli)
 * [Tutorial](#tutorial)
     * [Quick start](#quick-start)
     * [Interactive Dialogue](#interactive-dialogue)
-    * [Different persona](#different-persona)
+    * [Attribute a persona to the language model](#attribute-a-persona-to-the-language-model)
+* [API reference](#api-reference)
 * [Supported models](#supported-models)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to install the prebuilt wheels
@@ -51,35 +56,36 @@
 pip install pyllamacpp
 ```
 
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
-git clone --recursive https://github.com/nomic-ai/pyllamacpp && cd pyllamacpp
-pip install .
+pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
 # CLI 
 
-You can run the flowering simple command line interface to test the package once it is installed:
+You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
 
 ```shell
 pyllamacpp -h
 
 usage: pyllamacpp [-h] [--n_ctx N_CTX] [--n_parts N_PARTS] [--seed SEED] [--f16_kv F16_KV] [--logits_all LOGITS_ALL]
                   [--vocab_only VOCAB_ONLY] [--use_mlock USE_MLOCK] [--embedding EMBEDDING] [--n_predict N_PREDICT] [--n_threads N_THREADS]
                   [--repeat_last_n REPEAT_LAST_N] [--top_k TOP_K] [--top_p TOP_P] [--temp TEMP] [--repeat_penalty REPEAT_PENALTY]
                   [--n_batch N_BATCH]
                   model
 
+This is like a chatbot, You can start the conversation with `Hi, can you help me ?` Pay attention though that it may hallucinate!
+
 positional arguments:
   model                 The path of the model file
 
 options:
   -h, --help            show this help message and exit
   --n_ctx N_CTX         text context
   --n_parts N_PARTS
@@ -101,16 +107,16 @@
                         Last n tokens to penalize
   --top_k TOP_K         top_k
   --top_p TOP_P         top_p
   --temp TEMP           temp
   --repeat_penalty REPEAT_PENALTY
                         repeat_penalty
   --n_batch N_BATCH     batch size for prompt processing
-
 ```
+
 # Tutorial
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
@@ -122,61 +128,83 @@
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='/path/to/ggml/model')
 while True:
     try:
         prompt = input("You: ", flush=True)
         if prompt == '':
             continue
         print(f"AI:", end='')
         for tok in model.generate(prompt):
             print(f"{tok}", end='', flush=True)
         print()
     except KeyboardInterrupt:
         break
 ```
-### Different persona
-You can customize the `prompt_context` to _"give the language model a different persona"_ as follows:
+### Attribute a persona to the language model
+
+The following is an example showing how to _"attribute a persona to the language model"_ :
 
 ```python
 from pyllamacpp.model import Model
 
-prompt_context = """ Act as Bob. Bob is helpful, kind, honest, good at writing, and never fails to answer the User's requests immediately and with precision. To do this, Bob uses a database of information collected from many different sources, including books, journals, online articles, and more.
+prompt_context = """Act as Bob. Bob is helpful, kind, honest,
+and never fails to answer the User's requests immediately and with precision. 
 
 User: Nice to meet you Bob!
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
-prompt_prefix = "\n User:"
-prompt_suffix = "\n Bob:"
+prompt_prefix = "\nUser:"
+prompt_suffix = "\nBob:"
 
-model = Model(ggml_model=model, n_ctx=512, prompt_context=prompt_context, prompt_prefix=prompt_prefix,
+model = Model(model_path='/path/to/ggml/model', 
+              prompt_context=prompt_context, 
+              prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
+sequence = ''
+stop_word = prompt_prefix.strip()
+
 while True:
     try:
         prompt = input("You: ")
         if prompt == '':
             continue
-        print(f"Bob:", end='')
-        for tok in model.generate(prompt):
-            print(f"{tok}", end='', flush=True)
+        print(f"AI: ", end='')
+        for token in model.generate(prompt):
+            if token == '\n':
+                sequence += token
+                continue
+            if len(sequence) != 0:
+                if stop_word.startswith(sequence.strip()):
+                    sequence += token
+                    if sequence.strip() == stop_word:
+                        sequence = ''
+                        break
+                    else:
+                        continue
+                else:
+                    print(f"{sequence}", end='', flush=True)
+                    sequence = ''
+            print(f"{token}", end='', flush=True)
+
         print()
     except KeyboardInterrupt:
         break
-
 ```
 
 
-You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
```

### Comparing `pyllamacpp-2.0.0/README.md` & `pyllamacpp-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # PyLLaMACpp
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
-[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+
+<p align="center">
+  <img src="./docs/demo.gif">
+</p>
 
 
 For those who don't know, `llama.cpp` is a port of Facebook's LLaMA model in pure C/C++:
 
 <blockquote>
 
 - Without dependencies
@@ -22,15 +26,16 @@
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [CLI](#cli)
 * [Tutorial](#tutorial)
     * [Quick start](#quick-start)
     * [Interactive Dialogue](#interactive-dialogue)
-    * [Different persona](#different-persona)
+    * [Attribute a persona to the language model](#attribute-a-persona-to-the-language-model)
+* [API reference](#api-reference)
 * [Supported models](#supported-models)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to install the prebuilt wheels
@@ -38,35 +43,36 @@
 pip install pyllamacpp
 ```
 
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
-git clone --recursive https://github.com/nomic-ai/pyllamacpp && cd pyllamacpp
-pip install .
+pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
 # CLI 
 
-You can run the flowering simple command line interface to test the package once it is installed:
+You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
 
 ```shell
 pyllamacpp -h
 
 usage: pyllamacpp [-h] [--n_ctx N_CTX] [--n_parts N_PARTS] [--seed SEED] [--f16_kv F16_KV] [--logits_all LOGITS_ALL]
                   [--vocab_only VOCAB_ONLY] [--use_mlock USE_MLOCK] [--embedding EMBEDDING] [--n_predict N_PREDICT] [--n_threads N_THREADS]
                   [--repeat_last_n REPEAT_LAST_N] [--top_k TOP_K] [--top_p TOP_P] [--temp TEMP] [--repeat_penalty REPEAT_PENALTY]
                   [--n_batch N_BATCH]
                   model
 
+This is like a chatbot, You can start the conversation with `Hi, can you help me ?` Pay attention though that it may hallucinate!
+
 positional arguments:
   model                 The path of the model file
 
 options:
   -h, --help            show this help message and exit
   --n_ctx N_CTX         text context
   --n_parts N_PARTS
@@ -88,16 +94,16 @@
                         Last n tokens to penalize
   --top_k TOP_K         top_k
   --top_p TOP_P         top_p
   --temp TEMP           temp
   --repeat_penalty REPEAT_PENALTY
                         repeat_penalty
   --n_batch N_BATCH     batch size for prompt processing
-
 ```
+
 # Tutorial
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
@@ -109,61 +115,83 @@
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='/path/to/ggml/model')
 while True:
     try:
         prompt = input("You: ", flush=True)
         if prompt == '':
             continue
         print(f"AI:", end='')
         for tok in model.generate(prompt):
             print(f"{tok}", end='', flush=True)
         print()
     except KeyboardInterrupt:
         break
 ```
-### Different persona
-You can customize the `prompt_context` to _"give the language model a different persona"_ as follows:
+### Attribute a persona to the language model
+
+The following is an example showing how to _"attribute a persona to the language model"_ :
 
 ```python
 from pyllamacpp.model import Model
 
-prompt_context = """ Act as Bob. Bob is helpful, kind, honest, good at writing, and never fails to answer the User's requests immediately and with precision. To do this, Bob uses a database of information collected from many different sources, including books, journals, online articles, and more.
+prompt_context = """Act as Bob. Bob is helpful, kind, honest,
+and never fails to answer the User's requests immediately and with precision. 
 
 User: Nice to meet you Bob!
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
-prompt_prefix = "\n User:"
-prompt_suffix = "\n Bob:"
+prompt_prefix = "\nUser:"
+prompt_suffix = "\nBob:"
 
-model = Model(ggml_model=model, n_ctx=512, prompt_context=prompt_context, prompt_prefix=prompt_prefix,
+model = Model(model_path='/path/to/ggml/model', 
+              prompt_context=prompt_context, 
+              prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
+sequence = ''
+stop_word = prompt_prefix.strip()
+
 while True:
     try:
         prompt = input("You: ")
         if prompt == '':
             continue
-        print(f"Bob:", end='')
-        for tok in model.generate(prompt):
-            print(f"{tok}", end='', flush=True)
+        print(f"AI: ", end='')
+        for token in model.generate(prompt):
+            if token == '\n':
+                sequence += token
+                continue
+            if len(sequence) != 0:
+                if stop_word.startswith(sequence.strip()):
+                    sequence += token
+                    if sequence.strip() == stop_word:
+                        sequence = ''
+                        break
+                    else:
+                        continue
+                else:
+                    print(f"{sequence}", end='', flush=True)
+                    sequence = ''
+            print(f"{token}", end='', flush=True)
+
         print()
     except KeyboardInterrupt:
         break
-
 ```
 
 
-You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
```

### Comparing `pyllamacpp-2.0.0/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.1.0/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.1.0/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/LICENSE` & `pyllamacpp-2.1.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/options.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.1.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.1.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.1.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.1.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.1.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/check-style.sh` & `pyllamacpp-2.1.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.1.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/libsize.py` & `pyllamacpp-2.1.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/make_changelog.py` & `pyllamacpp-2.1.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.1.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.1.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.1.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.1.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.1.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.1.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pyllamacpp/_logger.py` & `pyllamacpp-2.1.0/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pyllamacpp/model.py` & `pyllamacpp-2.1.0/pyllamacpp/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,146 +3,144 @@
 
 """
 This module contains a simple Python API around [llama.cpp](https://github.com/ggerganov/llama.cpp)
 """
 
 import logging
 from pathlib import Path
-from typing import Callable, Tuple, Union
+from typing import Callable, Tuple, Union, List, Generator
 import pyllamacpp.constants as constants
 from pyllamacpp._logger import set_log_level
 
 __author__ = "abdeladim-s"
 __github__ = "https://github.com/abdeladim-s/pyllamacpp"
 __copyright__ = "Copyright 2023, "
 __license__ = "MIT"
 
 import logging
-import sys
 import _pyllamacpp as pp
 
 
 class Model:
     """
     A simple Python class on top of llama.cpp
 
     Example usage
     ```python
     from pyllamacpp.model import Model
-    import sys
 
     model = Model(ggml_model='./models/ggml-model-f16-q4_0.bin')
     for token in model.generate("Tell me a joke ?"):
         print(token, end='', flush=True)
     ```
     """
     _new_text_callback = None
 
     def __init__(self,
-                 ggml_model: str,
-                 prompt_context=constants.PROMPT_CONTEXT,
-                 prompt_prefix=constants.PROMPT_PREFIX,
-                 prompt_suffix=constants.PROMPT_SUFFIX,
-                 anti_prompts=[],
+                 model_path: str,
+                 prompt_context='',
+                 prompt_prefix='',
+                 prompt_suffix='',
                  log_level: int = logging.ERROR,
-                 **llama_params):
-        """
-        :param ggml_model: the path to the ggml model
-        :param prompt_context: the global context of the interaction, default to [PROMPT_CONTEXT](/pyllamacpp/#pyllamacpp.constants.PROMPT_CONTEXT)
-        :param prompt_prefix: the prompt prefix, default to [PROMPT_PREFIX](/pyllamacpp/#pyllamacpp.constants.PROMPT_PREFIX)
-        :param prompt_suffix: the prompt suffix, default to [PROMPT_SUFFIX](/pyllamacpp/#pyllamacpp.constants.PROMPT_SUFFIX)
-        :param anti_prompts: The inference will stop if an anti_prompt is detected, it will always contain the `prompt_prefix`
+                 n_ctx: int = 512,
+                 seed: int = 0,
+                 n_parts: int = -1,
+                 f16_kv: bool = False,
+                 logits_all: bool = False,
+                 vocab_only: bool = False,
+                 use_mlock: bool = False,
+                 embedding: bool = False):
+        """
+        :param model_path: the path to the ggml model
+        :param prompt_context: the global context of the interaction
+        :param prompt_prefix: the prompt prefix
+        :param prompt_suffix: the prompt suffix
         :param log_level: logging level, set to INFO by default
-        :param llama_params: keyword arguments for different whisper.cpp parameters,
-                        see [PARAMS_SCHEMA](/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA)
+        :param n_ctx: LLaMA context
+        :param seed: random seed
+        :param n_parts: LLaMA n_parts
+        :param f16_kv: use fp16 for KV cache
+        :param logits_all: the llama_eval() call computes all logits, not just the last one
+        :param vocab_only: only load the vocabulary, no weights
+        :param use_mlock: force system to keep model in RAM
+        :param embedding: embedding mode only
         """
+
         # set logging level
         set_log_level(log_level)
         self._ctx = None
 
-        if not Path(ggml_model).is_file():
-            raise Exception(f"File {ggml_model} not found!")
+        if not Path(model_path).is_file():
+            raise Exception(f"File {model_path} not found!")
 
         self.llama_params = pp.llama_context_default_params()
         # update llama_params
-        self._set_params(self.llama_params, llama_params)
+        self.llama_params.n_ctx = n_ctx
+        self.llama_params.seed = seed
+        self.llama_params.n_parts = n_parts
+        self.llama_params.f16_kv = f16_kv
+        self.llama_params.logits_all = logits_all
+        self.llama_params.vocab_only = vocab_only
+        self.llama_params.use_mlock = use_mlock
+        self.llama_params.embedding = embedding
 
-        self._ctx = pp.llama_init_from_file(ggml_model, self.llama_params)
+        self._ctx = pp.llama_init_from_file(model_path, self.llama_params)
 
         # gpt params
         self.gpt_params = pp.gpt_params()
 
         self.res = ""
 
         self._n_ctx = pp.llama_n_ctx(self._ctx)
         self._last_n_tokens = [0] * self._n_ctx  # n_ctx elements
         self._n_past = 0
         self.prompt_cntext = prompt_context
         self.prompt_prefix = prompt_prefix
         self.prompt_suffix = prompt_suffix
-        self.anti_prompts = anti_prompts
 
         self._prompt_context_tokens = []
         self._prompt_prefix_tokens = []
+        self._prompt_suffix_tokens = []
 
         self.reset()
 
     def reset(self):
         self._prompt_context_tokens = pp.llama_tokenize(self._ctx, self.prompt_cntext, True)
         self._prompt_prefix_tokens = pp.llama_tokenize(self._ctx, self.prompt_prefix, True)
-        self.anti_prompts.append(self.prompt_prefix)
+        self._prompt_suffix_tokens = pp.llama_tokenize(self._ctx, self.prompt_suffix, True)
         self._last_n_tokens = [0] * self._n_ctx  # n_ctx elements
         self._n_past = 0
 
-    def _is_anti_prompt(self, predicted_word: str) -> Tuple[bool, Union[None, str]]:
-        """
-        Returns True if an anti_prompt is detected
-        :param predicted_word: the predicted word
-        :return: Tuple[bool, Union[str, None]]
-        """
-        if predicted_word == '':
-            return False, None
-        for word in self.anti_prompts:
-            if word.startswith(predicted_word):
-                if word == predicted_word:
-                    return True, None
-                else:
-                    return True, predicted_word
-
-        return False, word
-
     def generate(self,
                  prompt: str,
                  n_predict: Union[None, int] = None,
                  infinite_generation: bool = False,
                  n_threads: int = 4,
-                 repeat_last_n: int = 128,
+                 repeat_last_n: int = 64,
                  top_k: int = 40,
                  top_p: float = 0.95,
                  temp: float = 0.8,
-                 repeat_penalty: float = 1.10,
-                 verbose: bool = True):
+                 repeat_penalty: float = 1.10) -> Generator:
         """
         Runs llama.cpp inference and yields new predicted tokens from the prompt provided as input
 
         :param prompt: The prompt :)
         :param n_predict: if n_predict is not None, the inference will stop if it reaches `n_predict` tokens, otherwise
                           it will continue until `EOS`
         :param infinite_generation: set it to `True` to make the generation go infinitely
         :param n_threads: The number of CPU threads
         :param repeat_last_n: last n tokens to penalize
         :param top_k: top K sampling parameter
         :param top_p: top P sampling parameter
         :param temp: temperature
         :param repeat_penalty: repeat penalty sampling parameter
-        :param verbose: if `True`, `llama.cpp` stuff will be printed
         :return: Tokens generator
         """
-        prompt = f' {self.prompt_prefix}{prompt}{self.prompt_suffix}'
-        input_tokens = pp.llama_tokenize(self._ctx, prompt, True)
+        input_tokens = self._prompt_prefix_tokens + pp.llama_tokenize(self._ctx, prompt,
+                                                                      True) + self._prompt_suffix_tokens
         if len(input_tokens) > self._n_ctx - 4:
             raise Exception('Prompt too long!')
         predicted_tokens = []
         predicted_token = 0
 
         # add global context for the first time
         if self._n_past == 0:
@@ -153,19 +151,16 @@
 
         # consume input tokens
         for tok in input_tokens:
             predicted_tokens.append(tok)
             self._last_n_tokens.pop(0)
             self._last_n_tokens.append(tok)
 
-        predicted_word = ""
         n_remain = 0
 
-        tokens_queue = []
-
         while infinite_generation or predicted_token != pp.llama_token_eos():
             if len(predicted_tokens) > 0:
                 if (pp.llama_eval(self._ctx,
                                   predicted_tokens,
                                   len(predicted_tokens),
                                   self._n_past,
                                   n_threads)):
@@ -179,38 +174,23 @@
                                                           top_k,
                                                           top_p,
                                                           temp,
                                                           repeat_penalty)
 
             predicted_tokens.append(predicted_token)
             token_str = pp.llama_token_to_str(self._ctx, predicted_token)
-            predicted_word = predicted_word + token_str
-            anti_prompt_flag, previous_word = self._is_anti_prompt(predicted_word)
-            if anti_prompt_flag and previous_word is None:
-                logging.info(f'Anti prompt {predicted_word} detected'.strip())
-                break
-            elif anti_prompt_flag and previous_word is not None:
-                predicted_word = previous_word
-                tokens_queue.append(token_str)
-                continue
-            else:
-                self._last_n_tokens.pop(0)
-                self._last_n_tokens.append(predicted_token)
-                predicted_word = token_str
-                # consume tokens_queue first
-                while len(tokens_queue) != 0:
-                    yield tokens_queue.pop(0)
-
-                yield token_str
-
+            self._last_n_tokens.pop(0)
+            self._last_n_tokens.append(predicted_token)
+            yield token_str
             if n_predict is not None:
                 if n_remain == n_predict:
                     break
                 else:
                     n_remain += 1
+
     @staticmethod
     def _set_params(params, kwargs: dict) -> None:
         """
         Private method to set the kwargs params to the `Params` class
         :param kwargs: dict like object for the different params
         :return: None
         """
@@ -223,40 +203,75 @@
         :return: None
         """
         if Model._new_text_callback is not None:
             Model._new_text_callback(text)
         # save res
         self.res += text
 
-    def _generate(self, prompt: str,
-                 n_predict: int = 128,
-                 new_text_callback: Callable[[str], None] = None,
-                 verbose: bool = False,
-                 **gpt_params) -> str:
+    def cpp_generate(self, prompt: str,
+                     n_predict: int = 128,
+                     new_text_callback: Callable[[str], None] = None,
+                     n_threads: int = 4,
+                     repeat_last_n: int = 64,
+                     top_k: int = 40,
+                     top_p: float = 0.95,
+                     temp: float = 0.8,
+                     repeat_penalty: float = 1.10,
+                     n_batch: int = 8,
+                     n_keep: int = 0,
+                     interactive: bool = False,
+                     antiprompt: List = [],
+                     ignore_eos: bool = False,
+                     instruct: bool = False,
+                     verbose_prompt: bool = False,
+                     ) -> str:
         """
-        Runs llama.cpp inference to generate new text content from the prompt provided as input
+        The generate function from `llama.cpp`
 
         :param prompt: the prompt
         :param n_predict: number of tokens to generate
         :param new_text_callback: a callback function called when new text is generated, default `None`
-        :param verbose: print some info about the inference
-        :param gpt_params: any other llama.cpp params see [PARAMS_SCHEMA](/pyllamacpp/#pyllamacpp.constants.GPT_PARAMS_SCHEMA)
+        :param n_threads: The number of CPU threads
+        :param repeat_last_n: last n tokens to penalize
+        :param top_k: top K sampling parameter
+        :param top_p: top P sampling parameter
+        :param temp: temperature
+        :param repeat_penalty: repeat penalty sampling parameter
+        :param n_batch: GPT params n_batch
+        :param n_keep: GPT params n_keep
+        :param interactive: interactive communication
+        :param antiprompt: list of anti prompts
+        :param ignore_eos: Ignore LLaMA EOS
+        :param instruct: Activate instruct mode
+        :param verbose_prompt: verbose prompt
         :return: the new generated text
         """
         self.gpt_params.prompt = prompt
         self.gpt_params.n_predict = n_predict
         # update other params if any
-        self._set_params(self.gpt_params, gpt_params)
+        self.gpt_params.n_threads = n_threads
+        self.gpt_params.repeat_last_n = repeat_last_n
+        self.gpt_params.top_k = top_k
+        self.gpt_params.top_p = top_p
+        self.gpt_params.temp = temp
+        self.gpt_params.repeat_penalty = repeat_penalty
+        self.gpt_params.n_batch = n_batch
+        self.gpt_params.n_keep = n_keep
+        self.gpt_params.interactive = interactive
+        self.gpt_params.antiprompt = antiprompt
+        self.gpt_params.ignore_eos = ignore_eos
+        self.gpt_params.instruct = instruct
+        self.gpt_params.verbose_prompt = verbose_prompt
 
         # assign new_text_callback
         self.res = ""
         Model._new_text_callback = new_text_callback
 
         # run the prediction
-        pp.llama_generate(self._ctx, self.gpt_params, self._call_new_text_callback, verbose)
+        pp.llama_generate(self._ctx, self.gpt_params, self._call_new_text_callback)
         return self.res
 
     @staticmethod
     def get_params(params) -> dict:
         """
         Returns a `dict` representation of the params
         :return: params dict
@@ -264,48 +279,17 @@
         res = {}
         for param in dir(params):
             if param.startswith('__'):
                 continue
             res[param] = getattr(params, param)
         return res
 
-    @staticmethod
-    def get_params_schema() -> dict:
-        """
-        A simple link to [PARAMS_SCHEMA](/pyllamacpp/#pyllamacpp.constants.PARAMS_SCHEMA)
-        :return: dict of params schema
-        """
-        return constants.GPT_PARAMS_SCHEMA
-
     def llama_print_timings(self):
         pp.llama_print_timings(self._ctx)
 
     @staticmethod
     def llama_print_system_info():
         pp.llama_print_system_info()
 
     def __del__(self):
         if self._ctx:
             pp.llama_free(self._ctx)
-
-
-if __name__ == '__main__':
-    model = '/home/su/Downloads/gpt4all/gpt4all-lora-quantized-converted.bin'
-    # model = "/opt/gpt4all-chat 0.1.0/bin/ggml-model-q4_0.bin"
-    prompt = """
-Below is an instruction that describes a task. Write a response that appropriately completes the request.
-
-## Instruction:
-what time is it ?
-## Response:
-it is 9:30 AM.
-
-
-##Instruction:
-what time is it ?
-##Response:
-it is 9:30 AM.
-    """
-    model = Model(ggml_model=model, log_level=logging.INFO, anti_prompts=['##Instruction'])
-    for token in model.generate(prompt, infinite_generation=True):
-        print(token, end='')
-        sys.stdout.flush()
```

### Comparing `pyllamacpp-2.0.0/pyllamacpp/utils.py` & `pyllamacpp-2.1.0/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pyllamacpp/webui.py` & `pyllamacpp-2.1.0/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.1.0/pyllamacpp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
-[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
+
+<p align="center">
+  <img src="./docs/demo.gif">
+</p>
 
 
 For those who don't know, `llama.cpp` is a port of Facebook's LLaMA model in pure C/C++:
 
 <blockquote>
 
 - Without dependencies
@@ -35,15 +39,16 @@
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [CLI](#cli)
 * [Tutorial](#tutorial)
     * [Quick start](#quick-start)
     * [Interactive Dialogue](#interactive-dialogue)
-    * [Different persona](#different-persona)
+    * [Attribute a persona to the language model](#attribute-a-persona-to-the-language-model)
+* [API reference](#api-reference)
 * [Supported models](#supported-models)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to install the prebuilt wheels
@@ -51,35 +56,36 @@
 pip install pyllamacpp
 ```
 
 However, the compilation process of `llama.cpp` is taking into account the architecture of the target `CPU`, 
 so you might need to build it from source:
 
 ```shell
-git clone --recursive https://github.com/nomic-ai/pyllamacpp && cd pyllamacpp
-pip install .
+pip install git+https://github.com/abdeladim-s/pyllamacpp.git
 ```
 
 # CLI 
 
-You can run the flowering simple command line interface to test the package once it is installed:
+You can run the following simple command line interface to test the package once it is installed:
 
 ```shell
 pyllamacpp path/to/ggml/model
 ```
 
 ```shell
 pyllamacpp -h
 
 usage: pyllamacpp [-h] [--n_ctx N_CTX] [--n_parts N_PARTS] [--seed SEED] [--f16_kv F16_KV] [--logits_all LOGITS_ALL]
                   [--vocab_only VOCAB_ONLY] [--use_mlock USE_MLOCK] [--embedding EMBEDDING] [--n_predict N_PREDICT] [--n_threads N_THREADS]
                   [--repeat_last_n REPEAT_LAST_N] [--top_k TOP_K] [--top_p TOP_P] [--temp TEMP] [--repeat_penalty REPEAT_PENALTY]
                   [--n_batch N_BATCH]
                   model
 
+This is like a chatbot, You can start the conversation with `Hi, can you help me ?` Pay attention though that it may hallucinate!
+
 positional arguments:
   model                 The path of the model file
 
 options:
   -h, --help            show this help message and exit
   --n_ctx N_CTX         text context
   --n_parts N_PARTS
@@ -101,16 +107,16 @@
                         Last n tokens to penalize
   --top_k TOP_K         top_k
   --top_p TOP_P         top_p
   --temp TEMP           temp
   --repeat_penalty REPEAT_PENALTY
                         repeat_penalty
   --n_batch N_BATCH     batch size for prompt processing
-
 ```
+
 # Tutorial
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
@@ -122,61 +128,83 @@
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='/path/to/ggml/model')
 while True:
     try:
         prompt = input("You: ", flush=True)
         if prompt == '':
             continue
         print(f"AI:", end='')
         for tok in model.generate(prompt):
             print(f"{tok}", end='', flush=True)
         print()
     except KeyboardInterrupt:
         break
 ```
-### Different persona
-You can customize the `prompt_context` to _"give the language model a different persona"_ as follows:
+### Attribute a persona to the language model
+
+The following is an example showing how to _"attribute a persona to the language model"_ :
 
 ```python
 from pyllamacpp.model import Model
 
-prompt_context = """ Act as Bob. Bob is helpful, kind, honest, good at writing, and never fails to answer the User's requests immediately and with precision. To do this, Bob uses a database of information collected from many different sources, including books, journals, online articles, and more.
+prompt_context = """Act as Bob. Bob is helpful, kind, honest,
+and never fails to answer the User's requests immediately and with precision. 
 
 User: Nice to meet you Bob!
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
-prompt_prefix = "\n User:"
-prompt_suffix = "\n Bob:"
+prompt_prefix = "\nUser:"
+prompt_suffix = "\nBob:"
 
-model = Model(ggml_model=model, n_ctx=512, prompt_context=prompt_context, prompt_prefix=prompt_prefix,
+model = Model(model_path='/path/to/ggml/model', 
+              prompt_context=prompt_context, 
+              prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
+sequence = ''
+stop_word = prompt_prefix.strip()
+
 while True:
     try:
         prompt = input("You: ")
         if prompt == '':
             continue
-        print(f"Bob:", end='')
-        for tok in model.generate(prompt):
-            print(f"{tok}", end='', flush=True)
+        print(f"AI: ", end='')
+        for token in model.generate(prompt):
+            if token == '\n':
+                sequence += token
+                continue
+            if len(sequence) != 0:
+                if stop_word.startswith(sequence.strip()):
+                    sequence += token
+                    if sequence.strip() == stop_word:
+                        sequence = ''
+                        break
+                    else:
+                        continue
+                else:
+                    print(f"{sequence}", end='', flush=True)
+                    sequence = ''
+            print(f"{token}", end='', flush=True)
+
         print()
     except KeyboardInterrupt:
         break
-
 ```
 
 
-You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
```

### Comparing `pyllamacpp-2.0.0/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.1.0/pyllamacpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/pyproject.toml` & `pyllamacpp-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/setup.py` & `pyllamacpp-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.0.0",
+    version="2.1.0",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
@@ -148,10 +148,8 @@
         'console_scripts': ['pyllamacpp=pyllamacpp.cli:main']
     },
     project_urls={
         'Documentation': 'https://abdeladim-s.github.io/pyllamacpp',
         'Source': 'https://github.com/abdeladim-s/pyllamacpp',
         'Tracker': 'https://github.com/abdeladim-s/pyllamacpp/issues',
     },
-    # install_requires=[],
-    # extras_require={},
 )
```

### Comparing `pyllamacpp-2.0.0/src/llama.cpp_LICENSE` & `pyllamacpp-2.1.0/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.0.0/src/main.cpp` & `pyllamacpp-2.1.0/src/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -194,21 +194,22 @@
     }
 
     return "The";
 }
 
 // quick and dirty implementation! just copied from main.cpp with some minor changes
 // Needs lots of improvements
-int llama_generate(struct llama_context_wrapper * ctx_w, gpt_params params, py::function new_text_callback, bool verbose){
+int llama_generate(struct llama_context_wrapper * ctx_w, gpt_params params, py::function new_text_callback){
 
     if (params.perplexity) {
         printf("\n************\n");
         printf("%s: please use the 'perplexity' tool for perplexity calculations\n", __func__);
         printf("************\n\n");
 
+
         return 0;
     }
 
     if (params.embedding) {
         printf("\n************\n");
         printf("%s: please use the 'embedding' tool for embedding calculations\n", __func__);
         printf("************\n\n");
```

### Comparing `pyllamacpp-2.0.0/src/main.h` & `pyllamacpp-2.1.0/src/main.h`

 * *Files identical despite different names*

