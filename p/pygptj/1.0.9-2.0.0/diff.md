# Comparing `tmp/pygptj-1.0.9.tar.gz` & `tmp/pygptj-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygptj-1.0.9.tar", last modified: Fri Apr 28 02:53:00 2023, max compression
+gzip compressed data, was "pygptj-2.0.0.tar", last modified: Tue May  2 18:35:09 2023, max compression
```

## Comparing `pygptj-1.0.9.tar` & `pygptj-2.0.0.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.547968 pygptj-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-28 02:52:48.000000 pygptj-1.0.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 02:52:48.000000 pygptj-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 02:52:48.000000 pygptj-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-28 02:53:00.547968 pygptj-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-28 02:52:48.000000 pygptj-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/gpt-2/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/gpt-2/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/gpt-j/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/gpt-j/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/mnist/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/stablelm/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/stablelm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/examples/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/examples/whisper/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/ggml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-28 02:52:51.000000 pygptj-1.0.9/ggml/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.535968 pygptj-1.0.9/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.543968 pygptj-1.0.9/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.547968 pygptj-1.0.9/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 02:52:48.000000 pygptj-1.0.9/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.539968 pygptj-1.0.9/pygptj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:52:48.000000 pygptj-1.0.9/pygptj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-28 02:52:48.000000 pygptj-1.0.9/pygptj/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 02:52:48.000000 pygptj-1.0.9/pygptj/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-28 02:52:48.000000 pygptj-1.0.9/pygptj/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.547968 pygptj-1.0.9/pygptj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-28 02:53:00.000000 pygptj-1.0.9/pygptj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-28 02:53:00.000000 pygptj-1.0.9/pygptj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:53:00.000000 pygptj-1.0.9/pygptj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:53:00.000000 pygptj-1.0.9/pygptj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 02:53:00.000000 pygptj-1.0.9/pygptj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-28 02:52:48.000000 pygptj-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:53:00.547968 pygptj-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-28 02:52:48.000000 pygptj-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:53:00.547968 pygptj-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/GGML_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26143 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/gptj.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/gptj.h
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-28 02:52:48.000000 pygptj-1.0.9/src/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-02 18:34:57.000000 pygptj-2.0.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 18:34:57.000000 pygptj-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 18:34:57.000000 pygptj-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-02 18:35:09.168091 pygptj-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 18:34:57.000000 pygptj-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/gpt-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/gpt-2/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/gpt-j/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/gpt-j/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/mnist/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/stablelm/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/stablelm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/examples/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/examples/whisper/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/ggml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-02 18:34:59.000000 pygptj-2.0.0/ggml/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.156091 pygptj-2.0.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.164091 pygptj-2.0.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 18:34:57.000000 pygptj-2.0.0/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.160091 pygptj-2.0.0/pygptj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-05-02 18:34:57.000000 pygptj-2.0.0/pygptj/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/pygptj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:35:08.000000 pygptj-2.0.0/pygptj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 18:35:09.000000 pygptj-2.0.0/pygptj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 18:34:57.000000 pygptj-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:35:09.168091 pygptj-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-02 18:34:57.000000 pygptj-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:35:09.168091 pygptj-2.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/GGML_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/gptj.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/gptj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-02 18:34:57.000000 pygptj-2.0.0/src/utils.h
```

### Comparing `pygptj-1.0.9/CMakeLists.txt` & `pygptj-2.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/LICENSE` & `pygptj-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/ggml/CMakeLists.txt` & `pygptj-2.0.0/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/ggml/cmake/BuildTypes.cmake` & `pygptj-2.0.0/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/ggml/cmake/GitVars.cmake` & `pygptj-2.0.0/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/ggml/src/CMakeLists.txt` & `pygptj-2.0.0/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/ggml/tests/CMakeLists.txt` & `pygptj-2.0.0/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/CMakeLists.txt` & `pygptj-2.0.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/LICENSE` & `pygptj-2.0.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/attr.h` & `pygptj-2.0.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/buffer_info.h` & `pygptj-2.0.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/cast.h` & `pygptj-2.0.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/chrono.h` & `pygptj-2.0.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/complex.h` & `pygptj-2.0.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/class.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/common.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/descr.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/init.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/internals.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/type_caster_base.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/detail/typeid.h` & `pygptj-2.0.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/eigen.h` & `pygptj-2.0.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/embed.h` & `pygptj-2.0.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/eval.h` & `pygptj-2.0.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/functional.h` & `pygptj-2.0.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/gil.h` & `pygptj-2.0.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/iostream.h` & `pygptj-2.0.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/numpy.h` & `pygptj-2.0.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/operators.h` & `pygptj-2.0.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/options.h` & `pygptj-2.0.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/pybind11.h` & `pygptj-2.0.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/pytypes.h` & `pygptj-2.0.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/stl/filesystem.h` & `pygptj-2.0.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/stl.h` & `pygptj-2.0.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/include/pybind11/stl_bind.h` & `pygptj-2.0.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tests/test_embed/CMakeLists.txt` & `pygptj-2.0.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/FindCatch.cmake` & `pygptj-2.0.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/FindEigen3.cmake` & `pygptj-2.0.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/FindPythonLibsNew.cmake` & `pygptj-2.0.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/check-style.sh` & `pygptj-2.0.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/cmake_uninstall.cmake.in` & `pygptj-2.0.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/libsize.py` & `pygptj-2.0.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/make_changelog.py` & `pygptj-2.0.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/pybind11Common.cmake` & `pygptj-2.0.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/pybind11Config.cmake.in` & `pygptj-2.0.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/pybind11NewTools.cmake` & `pygptj-2.0.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/pybind11Tools.cmake` & `pygptj-2.0.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/setup_global.py.in` & `pygptj-2.0.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pybind11/tools/setup_main.py.in` & `pygptj-2.0.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pygptj/_logger.py` & `pygptj-2.0.0/pygptj/_logger.py`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/pygptj.egg-info/SOURCES.txt` & `pygptj-2.0.0/pygptj.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 ./pygptj/__init__.py
 ./pygptj/_logger.py
+./pygptj/cli.py
 ./pygptj/constants.py
 ./pygptj/model.py
 ggml/CMakeLists.txt
 ggml/cmake/BuildTypes.cmake
 ggml/cmake/GitVars.cmake
 ggml/examples/CMakeLists.txt
 ggml/examples/gpt-2/CMakeLists.txt
@@ -70,14 +71,15 @@
 pybind11/tools/pybind11Tools.cmake
 pybind11/tools/pyproject.toml
 pybind11/tools/setup_global.py.in
 pybind11/tools/setup_main.py.in
 pygptj.egg-info/PKG-INFO
 pygptj.egg-info/SOURCES.txt
 pygptj.egg-info/dependency_links.txt
+pygptj.egg-info/entry_points.txt
 pygptj.egg-info/not-zip-safe
 pygptj.egg-info/top_level.txt
 src/GGML_LICENSE
 src/gptj.cpp
 src/gptj.h
 src/main.cpp
 src/main.h
```

### Comparing `pygptj-1.0.9/pyproject.toml` & `pygptj-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/setup.py` & `pygptj-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,32 +127,31 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pygptj",
-    version="1.0.9",
+    version="2.0.0",
     author="Abdeladim Sadiki",
     description="Python bindings for the GGML GPT-J Laguage model",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pygptj")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
     python_requires=">=3.8",
     packages=find_packages('.'),
     package_dir={'': '.'},
     long_description_content_type="text/markdown",
     license='MIT',
-    # entry_points={
-    #     'console_scripts': ['pyllamacpp-webui=pyllamacpp.webui:run',
-    #                         'pyllamacpp-convert-gpt4all=pyllamacpp.scripts.convert_gpt4all:main']
-    # },
-    # project_urls={
-    #     'Documentation': 'https://nomic-ai.github.io/pyllamacpp',
-    #     'Source': 'https://github.com/nomic-ai/pyllamacpp',
-    #     'Tracker': 'https://github.com/nomic-ai/pyllamacpp/issues',
-    # },
+    entry_points={
+        'console_scripts': ['pygptj=pygptj.cli:main']
+    },
+    project_urls={
+        'Documentation': 'https://abdeladim-s.github.io/pygptj',
+        'Source': 'https://github.com/abdeladim-s/pygptj',
+        'Tracker': 'https://github.com/abdeladim-s/pygptj/issues',
+    },
     # install_requires=[],
     # extras_require={"all": ["streamlit", "streamlit-ace", "sentencepiece", "torch"]},
 )
```

### Comparing `pygptj-1.0.9/src/GGML_LICENSE` & `pygptj-2.0.0/src/GGML_LICENSE`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/src/gptj.cpp` & `pygptj-2.0.0/src/gptj.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 #include <fstream>
 #include <map>
 #include <string>
 #include <vector>
 #include <iostream>
 
 #include <pybind11/pybind11.h>
+#include <pybind11/numpy.h>
+
 namespace py = pybind11;
 
 
+
 // load the model's weights from a file
 bool gptj_model_load(const std::string & fname, struct gptj_model & model, struct gpt_vocab & vocab) {
     printf("%s: loading model from '%s' - please wait ...\n", __func__, fname.c_str());
 
     auto fin = std::ifstream(fname, std::ios::binary);
     if (!fin) {
         fprintf(stderr, "%s: failed to open '%s'\n", __func__, fname.c_str());
@@ -338,25 +341,14 @@
     }
 
     fin.close();
 
     return true;
 }
 
-struct gptj_context gptj_load_model_ctx(const std::string & fname) {
-    struct gptj_context context;
-    auto model = context.model;
-    auto vocab = context.vocab;
-    if(gptj_model_load(fname, model, vocab)){
-        return context;
-    }
-    else{
-        fprintf(stderr, "%s: failed to load model from '%s'\n", __func__, fname.c_str());
-    }
-}
 
 void gptj_free(struct gptj_model * model){
     ggml_free(model->ctx);
 }
 
 // evaluate the transformer
 //
@@ -591,15 +583,15 @@
     //printf("used_mem = %zu\n", ggml_used_mem(ctx0));
 
     ggml_free(ctx0);
 
     return true;
 }
 
-int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab,  py::function new_text_callback) {
+int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab,  py::function new_text_callback, py::function logits_callback) {
 //    auto model = context->model;
 //    auto vocab = context->vocab;
 
     const int64_t t_main_start_us = ggml_time_us();
 
     params.model = "models/gpt-j-6B/ggml-model.bin";
 
@@ -652,15 +644,17 @@
         if (embd.size() > 0) {
             const int64_t t_start_us = ggml_time_us();
 
             if (!gptj_eval(model, params.n_threads, n_past, embd, logits, mem_per_token)) {
                 printf("Failed to predict\n");
                 return 1;
             }
-
+            // collect logits for each token
+            py::array_t<float> _logits = py::array_t<float>{model.hparams.n_vocab, logits.data(), py::none()};
+            logits_callback(_logits);
             t_predict_us += ggml_time_us() - t_start_us;
         }
 
         n_past += embd.size();
         embd.clear();
 
         if (i >= embd_inp.size()) {
```

### Comparing `pygptj-1.0.9/src/gptj.h` & `pygptj-2.0.0/src/gptj.h`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,19 @@
 struct gptj_context {
      struct gptj_model model;
      struct gpt_vocab vocab;
 };
 
 bool gptj_model_load(const std::string & fname,  struct gptj_model & model, struct gpt_vocab & vocab);
 
-struct gptj_context gptj_load_model_ctx(const std::string & fname);
 
 void gptj_free(struct gptj_model * model);
 
 bool gptj_eval(
         const gptj_model & model,
         const int n_threads,
         const int n_past,
         const std::vector<gpt_vocab::id> & embd_inp,
               std::vector<float>         & embd_w,
               size_t                     & mem_per_token);
 
-int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab, py::function new_text_callback);
+int gptj_generate(gpt_params params, struct gptj_model & model, struct gpt_vocab & vocab, py::function new_text_callback, py::function logits_callback);
```

### Comparing `pygptj-1.0.9/src/main.cpp` & `pygptj-2.0.0/src/main.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -11,27 +11,60 @@
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/functional.h>
 #include <pybind11/numpy.h>
 #include <map>
 
+//PYBIND11_MAKE_OPAQUE(std::vector<float>);
+
 #include "utils.h"
 #include "gptj.h"
 #include "main.h"
 
 
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 
 namespace py = pybind11;
 using namespace pybind11::literals; // to bring in the `_a` literal
 
+gpt_vocab::id gpt_sample_top_k_top_p_wrapper(
+        const gpt_vocab & vocab,
+        py::array_t<float> logits,
+        int    top_k,
+        double top_p,
+        double temp,
+        int seed){
+
+    py::buffer_info buf1 = logits.request();
+    auto *logits_ptr = static_cast<float *>(buf1.ptr);
+    std::mt19937 rng(seed);
+
+    return gpt_sample_top_k_top_p(vocab, logits_ptr, top_k, top_p, temp, rng);
+}
+
+py::tuple gptj_eval_wrapper(
+        const gptj_model & model,
+        const int n_threads,
+        const int n_past,
+        const std::vector<gpt_vocab::id> & embd_inp,
+        size_t mem_per_token){
+
+    std::vector<float> embd_w;
+    size_t mpt = mem_per_token;
+    auto res = gptj_eval(model, n_threads, n_past, embd_inp, embd_w, mpt);
+
+    py::tuple tup = py::make_tuple(embd_w, mpt);
+    return tup;
+}
+
+
 
 PYBIND11_MODULE(_pygptj, m) {
     m.doc() = R"pbdoc(
         PyGPT-J: Python binding to GPT-J
         -----------------------
 
         .. currentmodule:: _pygptj
@@ -52,33 +85,43 @@
         .def_readwrite("n_batch", &gpt_params::n_batch)
         .def_readwrite("model", &gpt_params::model)
         .def_readwrite("prompt", &gpt_params::prompt)
         ;
 
     py::class_<gptj_hparams>(m,"gptj_hparams" /*,py::dynamic_attr()*/)
         .def(py::init<>())
+        .def_readwrite("n_vocab", &gptj_hparams::n_vocab)
+        .def_readwrite("n_ctx", &gptj_hparams::n_ctx)
+        .def_readwrite("n_embd", &gptj_hparams::n_embd)
+        .def_readwrite("n_head", &gptj_hparams::n_head)
+        .def_readwrite("n_layer", &gptj_hparams::n_layer)
+        .def_readwrite("n_rot", &gptj_hparams::n_rot)
+        .def_readwrite("f16", &gptj_hparams::f16)
         ;
     py::class_<gptj_model>(m,"gptj_model" /*,py::dynamic_attr()*/)
         .def(py::init<>())
     ;
 
  py::class_<gpt_vocab>(m,"gpt_vocab" /*,py::dynamic_attr()*/)
         .def(py::init<>())
+        .def_readwrite("token_to_id", &gpt_vocab::token_to_id)
+        .def_readwrite("id_to_token", &gpt_vocab::id_to_token)
+
     ;
 
 py::class_<gptj_context>(m,"gptj_context" /*,py::dynamic_attr()*/)
 ;
 
     m.def("gptj_model_load", &gptj_model_load);
-    m.def("gptj_load_model_ctx", &gptj_load_model_ctx);
 
-    m.def("gptj_eval", &gptj_eval);
+    m.def("gptj_eval", &gptj_eval_wrapper);
     m.def("gptj_free", &gptj_free);
-    m.def("gpt_sample_top_k_top_p", &gpt_sample_top_k_top_p);
+    m.def("gpt_sample_top_k_top_p", &gpt_sample_top_k_top_p_wrapper);
     m.def("gpt_tokenize", &gpt_tokenize);
+    m.def("gpt_vocab_init", &gpt_vocab_init);
 
     m.def("gptj_generate", &gptj_generate);
 
 
 
 
 #ifdef VERSION_INFO
```

### Comparing `pygptj-1.0.9/src/utils.cpp` & `pygptj-2.0.0/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `pygptj-1.0.9/src/utils.h` & `pygptj-2.0.0/src/utils.h`

 * *Files identical despite different names*

