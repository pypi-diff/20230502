# Comparing `tmp/pygptj-2.0.0.tar.gz` & `tmp/pygptj-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygptj-2.0.0.tar", last modified: Tue May  2 18:35:09 2023, max compression
+gzip compressed data, was "pygptj-2.0.1.tar", last modified: Tue May  2 21:29:59 2023, max compression
```

## Comparing `pygptj-2.0.0.tar` & `pygptj-2.0.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-02 18:34:57.000000 pygptj-2.0.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 18:34:57.000000 pygptj-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 18:34:57.000000 pygptj-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-02 18:35:09.168091 pygptj-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 18:34:57.000000 pygptj-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/gpt-2/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/gpt-2/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/gpt-j/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/gpt-j/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/mnist/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/stablelm/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/stablelm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/whisper/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.156091 pygptj-2.0.0/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/pygptj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/pygptj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:08.000000 pygptj-2.0.0/pygptj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 18:34:57.000000 pygptj-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:35:09.168091 pygptj-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-02 18:34:57.000000 pygptj-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/GGML_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/gptj.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/gptj.h
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.934395 pygptj-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-02 21:29:45.000000 pygptj-2.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 21:29:45.000000 pygptj-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 21:29:45.000000 pygptj-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-02 21:29:59.934395 pygptj-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-02 21:29:45.000000 pygptj-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.918395 pygptj-2.0.1/ggml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/gpt-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/gpt-2/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/gpt-j/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/gpt-j/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/mnist/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/stablelm/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/stablelm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/examples/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/examples/whisper/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/ggml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-02 21:29:47.000000 pygptj-2.0.1/ggml/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.922395 pygptj-2.0.1/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.918395 pygptj-2.0.1/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.926396 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 21:29:45.000000 pygptj-2.0.1/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.918395 pygptj-2.0.1/pygptj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:45.000000 pygptj-2.0.1/pygptj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 21:29:45.000000 pygptj-2.0.1/pygptj/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-02 21:29:45.000000 pygptj-2.0.1/pygptj/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 21:29:45.000000 pygptj-2.0.1/pygptj/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-02 21:29:45.000000 pygptj-2.0.1/pygptj/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.930395 pygptj-2.0.1/pygptj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 21:29:59.000000 pygptj-2.0.1/pygptj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 21:29:45.000000 pygptj-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:29:59.934395 pygptj-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-02 21:29:45.000000 pygptj-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:59.934395 pygptj-2.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/GGML_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26051 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/gptj.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/gptj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-02 21:29:45.000000 pygptj-2.0.1/src/utils.h
```

### Comparing `pygptj-2.0.0/CMakeLists.txt` & `pygptj-2.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/LICENSE` & `pygptj-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/PKG-INFO` & `pygptj-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygptj
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python bindings for the GGML GPT-J Laguage model
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pygptj
 Project-URL: Source, https://github.com/abdeladim-s/pygptj
 Project-URL: Tracker, https://github.com/abdeladim-s/pygptj/issues
 Requires-Python: >=3.8
@@ -112,15 +112,15 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-[//]: # (* You can always refer to the [short documentation]&#40;https://nomic-ai.github.io/pyllamacpp/&#41; for more details.)
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pygptj/) for more details.
 
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pygptj/) for more details.
 
 # License
```

### Comparing `pygptj-2.0.0/README.md` & `pygptj-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-[//]: # (* You can always refer to the [short documentation]&#40;https://nomic-ai.github.io/pyllamacpp/&#41; for more details.)
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pygptj/) for more details.
 
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pygptj/) for more details.
 
 # License
```

### Comparing `pygptj-2.0.0/ggml/CMakeLists.txt` & `pygptj-2.0.1/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/ggml/cmake/BuildTypes.cmake` & `pygptj-2.0.1/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/ggml/cmake/GitVars.cmake` & `pygptj-2.0.1/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/ggml/src/CMakeLists.txt` & `pygptj-2.0.1/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/ggml/tests/CMakeLists.txt` & `pygptj-2.0.1/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/CMakeLists.txt` & `pygptj-2.0.1/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/LICENSE` & `pygptj-2.0.1/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/attr.h` & `pygptj-2.0.1/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/buffer_info.h` & `pygptj-2.0.1/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/cast.h` & `pygptj-2.0.1/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/chrono.h` & `pygptj-2.0.1/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/complex.h` & `pygptj-2.0.1/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/class.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/common.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/descr.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/init.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/internals.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/detail/typeid.h` & `pygptj-2.0.1/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/eigen.h` & `pygptj-2.0.1/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/embed.h` & `pygptj-2.0.1/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/eval.h` & `pygptj-2.0.1/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/functional.h` & `pygptj-2.0.1/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/gil.h` & `pygptj-2.0.1/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/iostream.h` & `pygptj-2.0.1/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/numpy.h` & `pygptj-2.0.1/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/operators.h` & `pygptj-2.0.1/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/options.h` & `pygptj-2.0.1/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/pybind11.h` & `pygptj-2.0.1/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/pytypes.h` & `pygptj-2.0.1/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/stl/filesystem.h` & `pygptj-2.0.1/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/stl.h` & `pygptj-2.0.1/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/include/pybind11/stl_bind.h` & `pygptj-2.0.1/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tests/test_embed/CMakeLists.txt` & `pygptj-2.0.1/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/FindCatch.cmake` & `pygptj-2.0.1/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/FindEigen3.cmake` & `pygptj-2.0.1/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/FindPythonLibsNew.cmake` & `pygptj-2.0.1/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/check-style.sh` & `pygptj-2.0.1/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/cmake_uninstall.cmake.in` & `pygptj-2.0.1/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/libsize.py` & `pygptj-2.0.1/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/make_changelog.py` & `pygptj-2.0.1/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/pybind11Common.cmake` & `pygptj-2.0.1/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/pybind11Config.cmake.in` & `pygptj-2.0.1/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/pybind11NewTools.cmake` & `pygptj-2.0.1/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/pybind11Tools.cmake` & `pygptj-2.0.1/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/setup_global.py.in` & `pygptj-2.0.1/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pybind11/tools/setup_main.py.in` & `pygptj-2.0.1/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pygptj/_logger.py` & `pygptj-2.0.1/pygptj/_logger.py`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pygptj/cli.py` & `pygptj-2.0.1/pygptj/cli.py`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pygptj/model.py` & `pygptj-2.0.1/pygptj/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,21 +41,21 @@
     _logits_callback = None
 
     def __init__(self,
                  model_path: str,
                  prompt_context: str = '',
                  prompt_prefix: str = '',
                  prompt_suffix: str = '',
-                 log_level: int = logging.INFO):
+                 log_level: int = logging.ERROR):
         """
         :param model_path: The path to a gpt-j `ggml` model
         :param prompt_context: the global context of the interaction
         :param prompt_prefix: the prompt prefix
         :param prompt_suffix: the prompt suffix
-        :param log_level: logging level, set to INFO by default
+        :param log_level: logging level
         """
         # set logging level
         set_log_level(log_level)
         self._ctx = None
 
         if not Path(model_path).is_file():
             raise Exception(f"File {model_path} not found!")
```

### Comparing `pygptj-2.0.0/pygptj.egg-info/PKG-INFO` & `pygptj-2.0.1/pygptj.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygptj
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python bindings for the GGML GPT-J Laguage model
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pygptj
 Project-URL: Source, https://github.com/abdeladim-s/pygptj
 Project-URL: Tracker, https://github.com/abdeladim-s/pygptj/issues
 Requires-Python: >=3.8
@@ -112,15 +112,15 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-[//]: # (* You can always refer to the [short documentation]&#40;https://nomic-ai.github.io/pyllamacpp/&#41; for more details.)
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pygptj/) for more details.
 
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pygptj/) for more details.
 
 # License
```

### Comparing `pygptj-2.0.0/pygptj.egg-info/SOURCES.txt` & `pygptj-2.0.1/pygptj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/pyproject.toml` & `pygptj-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/setup.py` & `pygptj-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pygptj",
-    version="2.0.0",
+    version="2.0.1",
     author="Abdeladim Sadiki",
     description="Python bindings for the GGML GPT-J Laguage model",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pygptj")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pygptj-2.0.0/src/GGML_LICENSE` & `pygptj-2.0.1/src/GGML_LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-2.0.0/src/gptj.cpp` & `pygptj-2.0.1/src/gptj.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
     //printf("used_mem = %zu\n", ggml_used_mem(ctx0));
 
     ggml_free(ctx0);
 
     return true;
 }
 
-int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab,  py::function new_text_callback, py::function logits_callback) {
+int gptj_generate(gptj_gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab,  py::function new_text_callback, py::function logits_callback) {
 //    auto model = context->model;
 //    auto vocab = context->vocab;
 
     const int64_t t_main_start_us = ggml_time_us();
 
     params.model = "models/gpt-j-6B/ggml-model.bin";
```

### Comparing `pygptj-2.0.0/src/gptj.h` & `pygptj-2.0.1/src/gptj.h`

 * *Files 4% similar despite different names*

```diff
@@ -80,8 +80,8 @@
         const gptj_model & model,
         const int n_threads,
         const int n_past,
         const std::vector<gpt_vocab::id> & embd_inp,
               std::vector<float>         & embd_w,
               size_t                     & mem_per_token);
 
-int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab, py::function new_text_callback, py::function logits_callback);
+int gptj_generate(gptj_gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab, py::function new_text_callback, py::function logits_callback);
```

### Comparing `pygptj-2.0.0/src/main.cpp` & `pygptj-2.0.1/src/main.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -70,25 +70,25 @@
         .. currentmodule:: _pygptj
 
         .. autosummary::
            :toctree: _generate
 
     )pbdoc";
 
-    py::class_<gpt_params>(m,"gptj_gpt_params" /*,py::dynamic_attr()*/)
+    py::class_<gptj_gpt_params>(m,"gptj_gpt_params" /*,py::dynamic_attr()*/)
         .def(py::init<>())
-        .def_readwrite("seed", &gpt_params::seed)
-        .def_readwrite("n_threads", &gpt_params::n_threads)
-        .def_readwrite("n_predict", &gpt_params::n_predict)
-        .def_readwrite("top_k", &gpt_params::top_k)
-        .def_readwrite("top_p", &gpt_params::top_p)
-        .def_readwrite("temp", &gpt_params::temp)
-        .def_readwrite("n_batch", &gpt_params::n_batch)
-        .def_readwrite("model", &gpt_params::model)
-        .def_readwrite("prompt", &gpt_params::prompt)
+        .def_readwrite("seed", &gptj_gpt_params::seed)
+        .def_readwrite("n_threads", &gptj_gpt_params::n_threads)
+        .def_readwrite("n_predict", &gptj_gpt_params::n_predict)
+        .def_readwrite("top_k", &gptj_gpt_params::top_k)
+        .def_readwrite("top_p", &gptj_gpt_params::top_p)
+        .def_readwrite("temp", &gptj_gpt_params::temp)
+        .def_readwrite("n_batch", &gptj_gpt_params::n_batch)
+        .def_readwrite("model", &gptj_gpt_params::model)
+        .def_readwrite("prompt", &gptj_gpt_params::prompt)
         ;
 
     py::class_<gptj_hparams>(m,"gptj_hparams" /*,py::dynamic_attr()*/)
         .def(py::init<>())
         .def_readwrite("n_vocab", &gptj_hparams::n_vocab)
         .def_readwrite("n_ctx", &gptj_hparams::n_ctx)
         .def_readwrite("n_embd", &gptj_hparams::n_embd)
```

### Comparing `pygptj-2.0.0/src/utils.cpp` & `pygptj-2.0.1/src/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  */
 
 #include "utils.h"
 
 #include <fstream>
 #include <regex>
 
-bool gpt_params_parse(int argc, char ** argv, gpt_params & params) {
+bool gpt_params_parse(int argc, char ** argv, gptj_gpt_params & params) {
     for (int i = 1; i < argc; i++) {
         std::string arg = argv[i];
 
         if (arg == "-s" || arg == "--seed") {
             params.seed = std::stoi(argv[++i]);
         } else if (arg == "-t" || arg == "--threads") {
             params.n_threads = std::stoi(argv[++i]);
@@ -43,15 +43,15 @@
             exit(0);
         }
     }
 
     return true;
 }
 
-void gpt_print_usage(int argc, char ** argv, const gpt_params & params) {
+void gpt_print_usage(int argc, char ** argv, const gptj_gpt_params & params) {
     fprintf(stderr, "usage: %s [options]\n", argv[0]);
     fprintf(stderr, "\n");
     fprintf(stderr, "options:\n");
     fprintf(stderr, "  -h, --help            show this help message and exit\n");
     fprintf(stderr, "  -s SEED, --seed SEED  RNG seed (default: -1)\n");
     fprintf(stderr, "  -t N, --threads N     number of threads to use during computation (default: %d)\n", params.n_threads);
     fprintf(stderr, "  -p PROMPT, --prompt PROMPT\n");
```

### Comparing `pygptj-2.0.0/src/utils.h` & `pygptj-2.0.1/src/utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #include <random>
 #include <thread>
 
 //
 // CLI argument parsing
 //
 
-struct gpt_params {
+struct gptj_gpt_params {
     int32_t seed      = -1; // RNG seed
     int32_t n_threads = std::min(4, (int32_t) std::thread::hardware_concurrency());
     int32_t n_predict = 200; // new tokens to predict
 
     // sampling parameters
     int32_t top_k = 40;
     float   top_p = 0.9f;
@@ -34,17 +34,17 @@
 
     int32_t n_batch = 8; // batch size for prompt processing
 
     std::string model = "models/gpt-2-117M/ggml-model.bin"; // model path
     std::string prompt;
 };
 
-bool gpt_params_parse(int argc, char ** argv, gpt_params & params);
+bool gpt_params_parse(int argc, char ** argv, gptj_gpt_params & params);
 
-void gpt_print_usage(int argc, char ** argv, const gpt_params & params);
+void gpt_print_usage(int argc, char ** argv, const gptj_gpt_params & params);
 
 std::string gpt_random_prompt(std::mt19937 & rng);
 
 //
 // Vocab utils
 //
```

