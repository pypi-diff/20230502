# Comparing `tmp/libsonata-0.1.8.tar.gz` & `tmp/libsonata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libsonata-0.1.8.tar", last modified: Wed Feb 10 17:14:12 2021, max compression
+gzip compressed data, was "dist/libsonata-0.1.9.tar", last modified: Thu Jul  1 12:58:57 2021, max compression
```

## Comparing `libsonata-0.1.8.tar` & `libsonata-0.1.9.tar`

### file list

```diff
@@ -1,227 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)     5586 2021-02-10 17:11:54.000000 libsonata-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2021-02-10 17:11:54.000000 libsonata-0.1.8/.github/workflows/coverage_test.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1980 2021-02-10 17:11:54.000000 libsonata-0.1.8/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)     3083 2021-02-10 17:11:54.000000 libsonata-0.1.8/.github/workflows/publish-sdist-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (116)      566 2021-02-10 17:11:54.000000 libsonata-0.1.8/.github/workflows/clang_format_check.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1156 2021-02-10 17:11:54.000000 libsonata-0.1.8/.github/workflows/docstring_check.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/CMake/
--rw-r--r--   0 runner    (1001) docker     (116)       57 2021-02-10 17:11:54.000000 libsonata-0.1.8/CMake/sonata-config.cmake
--rw-r--r--   0 runner    (1001) docker     (116)    11773 2021-02-10 17:11:54.000000 libsonata-0.1.8/CMake/CodeCoverage.cmake
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/ci/
--rwxr-xr-x   0 runner    (1001) docker     (116)      323 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/coverage_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)     1265 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/check_generated_docstrings.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      466 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/python_build_sdist.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      670 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/check_clang_format.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      484 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/python_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      779 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/cpp_test.sh
--rw-r--r--   0 runner    (1001) docker     (116)      592 2021-02-10 17:11:54.000000 libsonata-0.1.8/ci/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      648 2021-02-10 17:11:54.000000 libsonata-0.1.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (116)     1676 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (116)     2995 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (116)     9605 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (116)     2100 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (116)     8383 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/tools/FindPythonLibsNew.cmake
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (116)    19063 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (116)    14029 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (116)    58364 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/complex.h
--rw-r--r--   0 runner    (1001) docker     (116)     7849 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (116)    67677 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/numpy.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (116)    25323 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (116)    15964 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (116)    37850 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (116)     3566 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (116)    16322 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (116)     5655 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (116)     8749 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (116)     3865 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (116)     4823 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (116)    91933 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (116)     2031 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (116)    97860 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (116)      120 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (116)    29043 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (116)     3599 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (116)    23239 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (116)     7701 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (116)     6507 2021-02-10 17:12:01.000000 libsonata-0.1.8/python/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6513 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)    14239 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/libsonata/
--rw-r--r--   0 runner    (1001) docker     (116)      933 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/libsonata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      206 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20217 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (116)      465 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/python/generated/
--rw-r--r--   0 runner    (1001) docker     (116)    17016 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/generated/docstrings.h
--rw-r--r--   0 runner    (1001) docker     (116)       48 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/generated/.clang-format
--rw-r--r--   0 runner    (1001) docker     (116)    26738 2021-02-10 17:11:54.000000 libsonata-0.1.8/python/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-02-10 17:11:54.000000 libsonata-0.1.8/.gitreview
--rw-r--r--   0 runner    (1001) docker     (116)     1203 2021-02-10 17:11:54.000000 libsonata-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-10 17:14:12.000000 libsonata-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      243 2021-02-10 17:11:54.000000 libsonata-0.1.8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      638 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      111 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (116)   110733 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/docs/source/doxygen/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/doxygen/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/_templates/doxygen_page.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/docs/source/_images/
--rw-r--r--   0 runner    (1001) docker     (116)   296257 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/_images/libSonataLogo.jpg
--rw-r--r--   0 runner    (1001) docker     (116)      167 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/header.html
--rw-r--r--   0 runner    (1001) docker     (116)     7434 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/DoxygenLayout.xml
--rw-r--r--   0 runner    (1001) docker     (116)     6212 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      143 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/footer.html
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       63 2021-02-10 17:11:54.000000 libsonata-0.1.8/docs/source/cpp.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/include/bbp/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/include/bbp/sonata/
--rw-r--r--   0 runner    (1001) docker     (116)     2572 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/edges.h
--rw-r--r--   0 runner    (1001) docker     (116)     9437 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/population.h
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/nodes.h
--rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/node_sets.h
--rw-r--r--   0 runner    (1001) docker     (116)     5195 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/report_reader.h
--rw-r--r--   0 runner    (1001) docker     (116)     1177 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/common.h
--rw-r--r--   0 runner    (1001) docker     (116)    49307 2021-02-10 17:11:54.000000 libsonata-0.1.8/include/bbp/sonata/optional.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      384 2021-02-10 17:11:54.000000 libsonata-0.1.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (116)    10683 2021-02-10 17:11:54.000000 libsonata-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (116)      766 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/hdf5_mutex.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      153 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/version.cpp.in
--rw-r--r--   0 runner    (1001) docker     (116)    12770 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/population.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/edge_index.h
--rw-r--r--   0 runner    (1001) docker     (116)     5919 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/nodes.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      852 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     6684 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/edge_index.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      582 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/common.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      467 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (116)     7534 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/population.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    16081 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/report_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4069 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/edges.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      571 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/hdf5_mutex.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    11779 2021-02-10 17:11:54.000000 libsonata-0.1.8/src/node_sets.cpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/
--rw-r--r--   0 runner    (1001) docker     (116)      316 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)    68298 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/ChangeLog.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/support/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/support/cmake/
--rw-r--r--   0 runner    (1001) docker     (116)      299 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/support/cmake/FindSetEnv.cmake
--rw-r--r--   0 runner    (1001) docker     (116)     2799 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/support/cmake/cxx14.cmake
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/include/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/include/fmt/
--rw-r--r--   0 runner    (1001) docker     (116)    45897 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/core.h
--rw-r--r--   0 runner    (1001) docker     (116)   113256 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/format.h
--rw-r--r--   0 runner    (1001) docker     (116)    29669 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/format-inl.h
--rw-r--r--   0 runner    (1001) docker     (116)    21490 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/printf.h
--rw-r--r--   0 runner    (1001) docker     (116)     9069 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/ranges.h
--rw-r--r--   0 runner    (1001) docker     (116)     4867 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/ostream.h
--rw-r--r--   0 runner    (1001) docker     (116)     8820 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/posix.h
--rw-r--r--   0 runner    (1001) docker     (116)    14272 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/color.h
--rw-r--r--   0 runner    (1001) docker     (116)     4280 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/include/fmt/time.h
--rw-r--r--   0 runner    (1001) docker     (116)     1310 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (116)    19650 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/fmt/src/
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/src/format.cc
--rw-r--r--   0 runner    (1001) docker     (116)     6858 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/src/posix.cc
--rw-r--r--   0 runner    (1001) docker     (116)     9869 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/fmt/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/nlohmann/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/nlohmann/nlohmann/
--rw-r--r--   0 runner    (1001) docker     (116)   926233 2021-02-10 17:11:54.000000 libsonata-0.1.8/extlib/nlohmann/nlohmann/json.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      469 2021-02-10 17:11:54.000000 libsonata-0.1.8/extlib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/HighFive/
--rw-r--r--   0 runner    (1001) docker     (116)     1340 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/HighFive/include/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/
--rw-r--r--   0 runner    (1001) docker     (116)     9836 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataType.hpp
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/
--rw-r--r--   0 runner    (1001) docker     (116)     3717 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2921 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     6849 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     5088 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4555 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     5818 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2506 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2796 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Object.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      484 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5_definitions.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2786 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Annotate_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     6951 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Utils.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4498 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Slice_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1225 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Iterables_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     7055 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4242 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Exception_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4696 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Attribute_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    10772 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    12263 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5DataType_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     6776 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Node_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Reference_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     8758 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4620 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2737 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    14246 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Converter_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1130 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2130 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5DataSet_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     8437 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     3076 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Object_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Selection_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2750 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5File_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (116)    10476 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Easy.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2473 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Reference.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     4104 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5PropertyList.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2255 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5File.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     5377 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataSpace.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2839 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataSet.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     1630 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Selection.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      969 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Group.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     2339 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Attribute.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     3535 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Exception.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      839 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5Utility.hpp
--rw-r--r--   0 runner    (1001) docker     (116)      756 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/include/highfive/H5FileDriver.hpp
--rw-r--r--   0 runner    (1001) docker     (116)     3841 2021-02-10 17:11:58.000000 libsonata-0.1.8/extlib/HighFive/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     4469 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/test_selection.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     7163 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/test_node_sets.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     5721 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/test_report_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      166 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/main.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     4572 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/test_edges.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     9746 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/test_nodes.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      351 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 17:14:12.000000 libsonata-0.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)    22888 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/nodes1.h5
--rw-r--r--   0 runner    (1001) docker     (116)    17928 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/somas.h5
--rw-r--r--   0 runner    (1001) docker     (116)      297 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/node_sets.json
--rw-r--r--   0 runner    (1001) docker     (116)    21200 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/elements.h5
--rw-r--r--   0 runner    (1001) docker     (116)    15184 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/spikes.h5
--rw-r--r--   0 runner    (1001) docker     (116)    18856 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/edges-no-index.h5
--rw-r--r--   0 runner    (1001) docker     (116)    27712 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/edges1.h5
--rwxr-xr-x   0 runner    (1001) docker     (116)    10130 2021-02-10 17:11:54.000000 libsonata-0.1.8/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     5808 2021-02-10 17:11:54.000000 libsonata-0.1.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-02-10 17:11:54.000000 libsonata-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    14239 2021-02-10 17:14:12.000000 libsonata-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7653 2021-02-10 17:11:54.000000 libsonata-0.1.8/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (116)     2589 2021-02-10 17:11:54.000000 libsonata-0.1.8/.clang-format
--rw-r--r--   0 runner    (1001) docker     (116)    35150 2021-02-10 17:11:54.000000 libsonata-0.1.8/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35150 2021-07-01 12:56:46.000000 libsonata-0.1.9/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/edge_index.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7534 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/population.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13755 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/population.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    16634 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4069 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/edges.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/edge_index.h
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/hdf5_mutex.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6768 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/nodes.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/version.cpp.in
+-rw-r--r--   0 runner    (1001) docker     (121)    16081 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/report_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    16286 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/node_sets.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-07-01 12:56:46.000000 libsonata-0.1.9/src/hdf5_mutex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      779 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/cpp_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      484 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/python_test.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)      323 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/coverage_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      670 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/check_clang_format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      466 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/python_build_sdist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1265 2021-07-01 12:56:46.000000 libsonata-0.1.9/ci/check_generated_docstrings.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2021-07-01 12:56:46.000000 libsonata-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5908 2021-07-01 12:56:46.000000 libsonata-0.1.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-07-01 12:56:46.000000 libsonata-0.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-07-01 12:56:46.000000 libsonata-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7653 2021-07-01 12:56:46.000000 libsonata-0.1.9/COPYING.LESSER
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9918 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_node_sets.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    22888 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/nodes1.h5
+-rw-r--r--   0 runner    (1001) docker     (121)    27712 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/edges1.h5
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/node_sets.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/tests/data/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/config/circuit_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)    17928 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/somas.h5
+-rw-r--r--   0 runner    (1001) docker     (121)    15184 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/spikes.h5
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10130 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18856 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/edges-no-index.h5
+-rw-r--r--   0 runner    (1001) docker     (121)    21200 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/data/elements.h5
+-rw-r--r--   0 runner    (1001) docker     (121)     4572 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_edges.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10015 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_config.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4469 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_selection.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_report_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9981 2021-07-01 12:56:46.000000 libsonata-0.1.9/tests/test_nodes.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10913 2021-07-01 12:56:46.000000 libsonata-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2021-07-01 12:56:46.000000 libsonata-0.1.9/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-07-01 12:56:46.000000 libsonata-0.1.9/.github/workflows/coverage_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-07-01 12:56:46.000000 libsonata-0.1.9/.github/workflows/docstring_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2773 2021-07-01 12:56:46.000000 libsonata-0.1.9/.github/workflows/publish-sdist-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-07-01 12:56:46.000000 libsonata-0.1.9/.github/workflows/clang_format_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-07-01 12:56:46.000000 libsonata-0.1.9/.github/workflows/run-tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-07-01 12:56:46.000000 libsonata-0.1.9/extlib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/nlohmann/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/nlohmann/nlohmann/
+-rw-r--r--   0 runner    (1001) docker     (121)   926233 2021-07-01 12:56:46.000000 libsonata-0.1.9/extlib/nlohmann/nlohmann/json.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/filesystem/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)     3280 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/cmake/GhcHelper.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/cmake/config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/filesystem/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/fs_std.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/fs_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/fs_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/fs_std_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)   185321 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-07-01 12:56:50.000000 libsonata-0.1.9/extlib/filesystem/include/ghc/fs_std_fwd.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/HighFive/
+-rw-r--r--   0 runner    (1001) docker     (121)     3841 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/HighFive/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/
+-rw-r--r--   0 runner    (1001) docker     (121)     3535 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/
+-rw-r--r--   0 runner    (1001) docker     (121)     4498 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Slice_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Exception_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10772 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Iterables_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Annotate_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Selection_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Node_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    14246 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Converter_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5File_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5DataSet_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12263 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5DataType_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4696 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Attribute_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5_definitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Reference_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4242 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8758 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6951 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Object_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8437 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7055 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Selection.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5FileDriver.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2796 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Object.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5File.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Attribute.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4104 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5PropertyList.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataType.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Group.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5377 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataSpace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/
+-rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2921 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6849 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3717 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5818 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Utility.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Version.hpp.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10476 2021-07-01 12:56:49.000000 libsonata-0.1.9/extlib/HighFive/include/highfive/H5Easy.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     9800 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/src/os.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4089 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/src/format.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/support/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/support/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/support/cmake/FindSetEnv.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/support/cmake/cxx14.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/support/cmake/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    13051 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   143549 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/ChangeLog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    18528 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/extlib/fmt/include/fmt/
+-rw-r--r--   0 runner    (1001) docker     (121)     5905 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/ostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23649 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/color.h
+-rw-r--r--   0 runner    (1001) docker     (121)    24071 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/compile.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23257 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/printf.h
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/posix.h
+-rw-r--r--   0 runner    (1001) docker     (121)   132881 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/format.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/locale.h
+-rw-r--r--   0 runner    (1001) docker     (121)    35802 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)   109835 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/format-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12546 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/ranges.h
+-rw-r--r--   0 runner    (1001) docker     (121)    71298 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/core.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13680 2021-07-01 12:56:51.000000 libsonata-0.1.9/extlib/fmt/include/fmt/os.h
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-01 12:56:46.000000 libsonata-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-07-01 12:56:46.000000 libsonata-0.1.9/.gitreview
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/CMake/
+-rw-r--r--   0 runner    (1001) docker     (121)    11773 2021-07-01 12:56:46.000000 libsonata-0.1.9/CMake/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-07-01 12:56:46.000000 libsonata-0.1.9/CMake/sonata-config.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/docs/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (121)   296257 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/_images/libSonataLogo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/docs/source/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/doxygen/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/_templates/doxygen_page.rst_t
+-rw-r--r--   0 runner    (1001) docker     (121)   110733 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (121)     6219 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/header.html
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/cpp.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7434 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/source/DoxygenLayout.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-07-01 12:56:46.000000 libsonata-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-07-01 12:56:46.000000 libsonata-0.1.9/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/include/bbp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/include/bbp/sonata/
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/nodes.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5685 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/config.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/edges.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9583 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/population.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/node_sets.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)    49307 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5195 2021-07-01 12:56:46.000000 libsonata-0.1.9/include/bbp/sonata/report_reader.h
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-01 12:58:57.000000 libsonata-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    11309 2021-07-01 12:58:57.000000 libsonata-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22695 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/generated/
+-rw-r--r--   0 runner    (1001) docker     (121)    22239 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/generated/docstrings.h
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/generated/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/libsonata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7120 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11309 2021-07-01 12:58:56.000000 libsonata-0.1.9/python/libsonata.egg-info/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)     6507 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)     8383 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9605 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2995 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/tools/FindCatch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)     5655 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    91933 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/cast.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)     3566 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    15964 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (121)    37850 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)    25323 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16322 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7849 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3865 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19063 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    14029 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29043 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/complex.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    67677 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3599 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7701 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23239 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (121)    97860 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8749 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (121)    58364 2021-07-01 12:56:52.000000 libsonata-0.1.9/python/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (121)    28583 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 12:58:57.000000 libsonata-0.1.9/python/libsonata/
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-07-01 12:56:46.000000 libsonata-0.1.9/python/libsonata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2021-07-01 12:56:46.000000 libsonata-0.1.9/.clang-format
```

### Comparing `libsonata-0.1.8/setup.py` & `libsonata-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/.github/workflows/coverage_test.yaml` & `libsonata-0.1.9/.github/workflows/coverage_test.yaml`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/.github/workflows/run-tests.yml` & `libsonata-0.1.9/.github/workflows/run-tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         uses: actions/checkout@v2
         with:
           submodules: 'true'
 
       - name: Install packages on MacOS
         run: |
             brew update
-            brew unlink gcc@8 gcc@9  # work around for https://github.com/actions/virtual-environments/issues/2391
             brew install cmake || true  # macos image has cmake installed, but a new version may exist; ignore it if so
             brew install doxygen
             brew install hdf5
 
       - name: Build and run unittests
         run: |
             ./ci/cpp_test.sh
```

### Comparing `libsonata-0.1.8/.github/workflows/publish-sdist-wheels.yml` & `libsonata-0.1.9/.github/workflows/publish-sdist-wheels.yml`

 * *Files 12% similar despite different names*

```diff
@@ -45,18 +45,14 @@
       - name: Build wheels Mac OS
         if: runner.os == 'macOS'
         env:
           CIBW_BEFORE_BUILD: |
              brew update
              brew --version
              brew install cmake
-             # the HDF5 bottle uses gcc10; https://formulae.brew.sh/formula/hdf5
-             # so we are hit by this: https://github.com/Homebrew/homebrew-core/issues/68866
-             # sadly, it seems Homebrew/brew#10327 doesn't fix it, so we unlink old gcc's manually
-             brew unlink gcc@8 gcc@9
              brew install hdf5
         run: |
           python -m cibuildwheel --output-dir dist
       - name: Store wheel as artifact
         uses: actions/upload-artifact@v2
         with:
           name: dist
```

### Comparing `libsonata-0.1.8/.github/workflows/clang_format_check.yaml` & `libsonata-0.1.9/.github/workflows/clang_format_check.yaml`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/.github/workflows/docstring_check.yaml` & `libsonata-0.1.9/.github/workflows/docstring_check.yaml`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/CMake/CodeCoverage.cmake` & `libsonata-0.1.9/CMake/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/ci/check_generated_docstrings.sh` & `libsonata-0.1.9/ci/check_generated_docstrings.sh`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/ci/check_clang_format.sh` & `libsonata-0.1.9/ci/check_clang_format.sh`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/ci/cpp_test.sh` & `libsonata-0.1.9/ci/cpp_test.sh`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/ci/README.md` & `libsonata-0.1.9/ci/README.md`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/MANIFEST.in` & `libsonata-0.1.9/MANIFEST.in`

 * *Files 17% similar despite different names*

```diff
@@ -15,12 +15,18 @@
 include extlib/fmt/*.rst
 
 # highfive
 recursive-include extlib/HighFive/include *
 include extlib/HighFive/CMakeLists.txt
 include extlib/HighFive/LICENSE
 
+# filesystem
+recursive-include extlib/filesystem/cmake *
+recursive-include extlib/filesystem/include *
+include extlib/filesystem/CMakeLists.txt
+include extlib/filesystem/LICENSE
+
 # pybind11
 recursive-include python/pybind11/include *
 recursive-include python/pybind11/tools *.cmake
 include python/pybind11/CMakeLists.txt
 include python/pybind11/LICENSE
```

### Comparing `libsonata-0.1.8/python/pybind11/LICENSE` & `libsonata-0.1.9/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/tools/FindEigen3.cmake` & `libsonata-0.1.9/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/tools/pybind11Tools.cmake` & `libsonata-0.1.9/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/tools/FindCatch.cmake` & `libsonata-0.1.9/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/tools/FindPythonLibsNew.cmake` & `libsonata-0.1.9/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/attr.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/stl.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/pytypes.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/complex.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/embed.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/numpy.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/class.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/internals.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/typeid.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/common.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/descr.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/detail/init.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/iostream.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/operators.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/eval.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/buffer_info.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/cast.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/options.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/pybind11.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/eigen.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/functional.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/stl_bind.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/include/pybind11/chrono.h` & `libsonata-0.1.9/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/pybind11/CMakeLists.txt` & `libsonata-0.1.9/python/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/python/libsonata.egg-info/SOURCES.txt` & `libsonata-0.1.9/python/libsonata.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -81,34 +81,48 @@
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
 extlib/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+extlib/filesystem/CMakeLists.txt
+extlib/filesystem/LICENSE
+extlib/filesystem/cmake/GhcHelper.cmake
+extlib/filesystem/cmake/config.cmake.in
+extlib/filesystem/include/ghc/filesystem.hpp
+extlib/filesystem/include/ghc/fs_fwd.hpp
+extlib/filesystem/include/ghc/fs_impl.hpp
+extlib/filesystem/include/ghc/fs_std.hpp
+extlib/filesystem/include/ghc/fs_std_fwd.hpp
+extlib/filesystem/include/ghc/fs_std_impl.hpp
 extlib/fmt/CMakeLists.txt
-extlib/fmt/CONTRIBUTING.rst
 extlib/fmt/ChangeLog.rst
 extlib/fmt/LICENSE.rst
 extlib/fmt/README.rst
+extlib/fmt/include/fmt/chrono.h
 extlib/fmt/include/fmt/color.h
+extlib/fmt/include/fmt/compile.h
 extlib/fmt/include/fmt/core.h
 extlib/fmt/include/fmt/format-inl.h
 extlib/fmt/include/fmt/format.h
+extlib/fmt/include/fmt/locale.h
+extlib/fmt/include/fmt/os.h
 extlib/fmt/include/fmt/ostream.h
 extlib/fmt/include/fmt/posix.h
 extlib/fmt/include/fmt/printf.h
 extlib/fmt/include/fmt/ranges.h
-extlib/fmt/include/fmt/time.h
 extlib/fmt/src/format.cc
-extlib/fmt/src/posix.cc
+extlib/fmt/src/os.cc
 extlib/fmt/support/cmake/FindSetEnv.cmake
+extlib/fmt/support/cmake/JoinPaths.cmake
 extlib/fmt/support/cmake/cxx14.cmake
 extlib/nlohmann/nlohmann/json.hpp
 include/bbp/sonata/common.h
+include/bbp/sonata/config.h
 include/bbp/sonata/edges.h
 include/bbp/sonata/node_sets.h
 include/bbp/sonata/nodes.h
 include/bbp/sonata/optional.hpp
 include/bbp/sonata/population.h
 include/bbp/sonata/report_reader.h
 python/CMakeLists.txt
@@ -151,14 +165,15 @@
 python/pybind11/tools/FindCatch.cmake
 python/pybind11/tools/FindEigen3.cmake
 python/pybind11/tools/FindPythonLibsNew.cmake
 python/pybind11/tools/pybind11Tools.cmake
 python/tests/__init__.py
 python/tests/test.py
 src/common.cpp
+src/config.cpp
 src/edge_index.cpp
 src/edge_index.h
 src/edges.cpp
 src/hdf5_mutex.cpp
 src/hdf5_mutex.hpp
 src/node_sets.cpp
 src/nodes.cpp
@@ -166,20 +181,22 @@
 src/population.hpp
 src/report_reader.cpp
 src/utils.cpp
 src/utils.h
 src/version.cpp.in
 tests/CMakeLists.txt
 tests/main.cpp
+tests/test_config.cpp
 tests/test_edges.cpp
 tests/test_node_sets.cpp
 tests/test_nodes.cpp
 tests/test_report_reader.cpp
 tests/test_selection.cpp
 tests/data/edges-no-index.h5
 tests/data/edges1.h5
 tests/data/elements.h5
 tests/data/generate.py
 tests/data/node_sets.json
 tests/data/nodes1.h5
 tests/data/somas.h5
-tests/data/spikes.h5
+tests/data/spikes.h5
+tests/data/config/circuit_config.json
```

### Comparing `libsonata-0.1.8/python/libsonata.egg-info/PKG-INFO` & `libsonata-0.1.9/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,412 +1,401 @@
-Metadata-Version: 2.1
-Name: libsonata
-Version: 0.1.8
-Summary: SONATA files reader
-Home-page: https://github.com/BlueBrain/libsonata
-Author: Blue Brain Project, EPFL
-License: LGPLv3
-Description: |banner|
-        
-        |license| |coverage| |docs|
-        
-        libsonata
-        =========
-        
-        C++ / Python reader for SONATA circuit files:
-        `SONATA guide <https://github.com/AllenInstitute/sonata/blob/master/docs/SONATA_DEVELOPER_GUIDE.md>`__
-        
-        Installation
-        ------------
-        
-        Installing from PyPI
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           pip install libsonata
-        
-        Installing as a Python package, directly from GitHub
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           pip install git+https://github.com/BlueBrain/libsonata
-        
-        Building the C++ library
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           git clone git@github.com:BlueBrain/libsonata.git --recursive
-           cd libsonata
-           mkdir build && cd build
-           cmake  -DCMAKE_BUILD_TYPE=Release  -DEXTLIB_FROM_SUBMODULES=ON ..
-           make -j
-        
-        Usage (Python)
-        --------------
-        
-        Nodes
-        ~~~~~
-        
-        NodeStorage
-        +++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> import libsonata
-        
-           >>> nodes = libsonata.NodeStorage('path/to/H5/file')
-        
-           # list populations
-           >>> nodes.population_names
-        
-           # open population
-           >>> population = nodes.open_population(<name>)
-        
-        
-        NodePopulation
-        ++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # total number of nodes in the population
-           >>> population.size
-        
-           # attribute names
-           >>> population.attribute_names
-        
-           # get attribute value for single node, say 42
-           >>> population.get_attribute('mtype', 42)
-        
-           # ...or Selection of nodes (see below) => returns NumPy array with corresponding values
-           >>> selection = libsonata.Selection(values=[1, 5, 9, 42])  # nodes 1, 5, 9, 42
-           >>> mtypes = population.get_attribute('mtype', selection)
-           >>> list(zip(selection.flatten(), mtypes))
-           [(1, u'mtype_of_1'), (5, u'mtype_of_5'), (9, u'mtype_of_9'), (42, u'mtype_of_42')]
-        
-        
-        Selection
-        +++++++++
-        
-        List of element IDs (either `node_id`, or `edge_id`) where adjacent IDs are grouped for the sake of efficient HDF5 file access.
-        For instance, `{1, 2, 3, 5}` sequence becomes `{[1, 4), [5, 6)}`.
-        
-        `Selection` can be instantiated from:
-         - a sequence of scalar values (works for NumPy arrays as well)
-         - a sequence of pairs (interpreted as ranges above, works for N x 2 NumPy arrays as well)
-        
-        `EdgePopulation` connectivity queries (see below) return ``Selection``\ s as well.
-        
-        .. code-block:: pycon
-        
-           >>> selection = libsonata.Selection([1, 2, 3, 5])
-           >>> selection.ranges
-           [(1, 4), (5, 6)]
-        
-        
-        .. code-block:: pycon
-        
-           >>> selection = libsonata.Selection([(1, 4), (5, 6)])
-           >>> selection.flatten()
-           [1, 2, 3, 5]
-           >>> selection.flat_size
-           4
-           >>> bool(selection)
-           True
-        
-        
-        Edges
-        ~~~~~
-        
-        EdgeStorage
-        +++++++++++
-        
-        Population handling for `EdgeStorage` is analogous to `NodeStorage`:
-        
-        .. code-block:: pycon
-        
-           >>> edges = libsonata.EdgeStorage('path/to/H5/file')
-        
-           # list populations
-           >>> edges.population_names
-        
-           # open population
-           >>> population = edges.open_population(<name>)
-        
-        
-        EdgePopulation
-        ++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # total number of edges in the population
-           >>> population.size
-        
-           # attribute names
-           >>> population.attribute_names
-        
-           # get attribute value for single edge, say 123
-           >>> population.get_attribute('delay', 123)
-        
-           # ...or Selection of edges => returns NumPy array with corresponding values
-           >>> selection = libsonata.Selection([1, 5, 9])
-           >>> population.get_attribute('delay', selection) # returns delays for edges 1, 5, 9
-        
-        
-        ...with additional methods for querying connectivity, where the results are selections that can be applied like above
-        
-        .. code-block:: pycon
-        
-           # get source / target node ID for the 42nd edge:
-           >>> population.source_node(42)
-           >>> population.target_node(42)
-        
-           # query connectivity (result is Selection object)
-           >>> selection_to_1 = population.afferent_edges(1)  # all edges with target node_id 1
-           >>> population.target_nodes(selection_to_1)  # since selection only contains edges
-                                                        # targeting node_id 1 the result will be a
-                                                        # numpy array of all 1's
-           >>> selection_from_2 = population.efferent_edges(2)  # all edges sourced from node_id 2
-           >>> selection = population.connecting_edges(2, 1)  # this selection is all edges from
-                                                              # node_id 2 to node_id 1
-        
-           # ...or their vectorized analogues
-           >>> selection = population.afferent_edges([1, 2, 3])
-           >>> selection = population.efferent_edges([1, 2, 3])
-           >>> selection = population.connecting_edges([1, 2, 3], [4, 5, 6])
-        
-        
-        Reports
-        ~~~~~~~
-        
-        SpikeReader
-        +++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> import libsonata
-        
-           >>> spikes = libsonata.SpikeReader('path/to/H5/file')
-        
-           # list populations
-           >>> spikes.get_populations_names()
-        
-           # open population
-           >>> population = spikes['<name>']
-        
-        
-        SpikePopulation
-        +++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get all spikes [(node_id, timestep)]
-           >>> population.get()
-           [(5, 0.1), (2, 0.2), (3, 0.3), (2, 0.7), (3, 1.3)]
-        
-           # get all spikes betwen tstart and tstop
-           >>> population.get(tstart=0.2, tstop=1.0)
-           [(2, 0.2), (3, 0.3), (2, 0.7)]
-        
-           # get spikes attribute sorting (by_time, by_id, none)
-           >>> population.sorting
-           'by_time'
-        
-           Pandas can be used to create a dataframe and get a better representation of the data
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           data = population.get()
-           df = pandas.DataFrame(data=data, columns=['ids', 'times']).set_index('times')
-           print(df)
-                  ids
-           times
-           0.1      5
-           0.2      2
-           0.3      3
-           0.7      2
-           1.3      3
-        
-        
-        SomaReportReader
-        ++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> somas = libsonata.SomaReportReader('path/to/H5/file')
-        
-           # list populations
-           >>> somas.get_populations_names()
-        
-           # open population
-           >>> population_somas = somas['<name>']
-        
-        
-        SomaReportPopulation
-        ++++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get times (tstart, tstop, dt)
-           >>> population_somas.times
-           (0.0, 1.0, 0.1)
-        
-           # get unit attributes
-           >>> population_somas.time_units
-           'ms'
-           >>> population_somas.data_units
-           'mV'
-        
-           # node_ids sorted?
-           >>> population_somas.sorted
-           True
-        
-           # get a list of all node ids in the selected population
-           >>> population_somas.get_node_ids()
-           [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
-        
-           # get the DataFrame of the node_id values for the timesteps between tstart and tstop
-           >>> data_frame = population_somas.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
-        
-           # get the data values
-           >>> data_frame.data
-           [[13.8, 14.8], [13.9, 14.9]]
-        
-           # get the list of timesteps
-           >>> data_frame.times
-           [0.8, 0.9]
-        
-           # get the list of node ids
-           >>> data_frame.ids
-           [13, 14]
-        
-        
-        Once again, pandas can be used to create a dataframe using the data, ids and times lists
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           df = pandas.DataFrame(data_frame.data, columns=data_frame.ids, index=data_frame.times)
-           print(df)
-                  13    14
-           0.8  13.8  14.8
-           0.9  13.9  14.9
-        
-        
-        ElementReportReader
-        +++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> elements = libsonata.ElementReportReader('path/to/H5/file')
-        
-           # list populations
-           >>> elements.get_populations_names()
-        
-           # open population
-           >>> population_elements = elements['<name>']
-        
-        
-        ElementReportPopulation
-        +++++++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get times (tstart, tstop, dt)
-           >>> population_elements.times
-           (0.0, 4.0, 0.2)
-        
-           >>> population_elements.get_node_ids()
-           [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
-        
-           # get the DataFrame of the node_id values for the timesteps between tstart and tstop
-           >>> data_frame = population_elements.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
-        
-           # get the data values (list of list of floats with data[time_index][element_index])
-           >>> data_frame.data
-           [[46.0, 46.1, 46.2, 46.3, 46.4, 46.5, 46.6, 46.7, 46.8, 46.9], [56.0, 56.1, 56.2, 56.3, 56.4, 56.5, 56.6, 56.7, 56.8, 56.9]]
-        
-           # get the list of timesteps
-           >>> data_frame.times
-           [0.8, 1.0]
-        
-           # get the list of (node id, element_id)
-           >>> data_frame.ids
-           [(13, 30), (13, 30), (13, 31), (13, 31), (13, 32), (14, 32), (14, 33), (14, 33), (14, 34), (14, 34)]
-        
-        
-        The same way than with spikes and soma reports, pandas can be used to get a better representation of the data
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           df = pandas.DataFrame(data_frame.data, columns=pandas.MultiIndex.from_tuples(data_frame.ids), index=data_frame.times)
-           print(df)
-                  13                            14
-                  30    30    31    31    32    32    33    33    34    34
-           0.8  46.0  46.1  46.2  46.3  46.4  46.5  46.6  46.7  46.8  46.9
-           1.0  56.0  56.1  56.2  56.3  56.4  56.5  56.6  56.7  56.8  56.9
-        
-        For big datasets, using numpy arrays could greatly improve the performance
-        
-        .. code-block:: pycon
-        
-           >>> import numpy
-        
-           np_data = numpy.asarray(data_frame.data)
-           np_ids = numpy.asarray(data_frame.ids).T
-           np_times = numpy.asarray(data_frame.times)
-        
-           df = pandas.DataFrame(np_data, columns=pandas.MultiIndex.from_arrays(np_ids), index=np_times)
-        
-        
-        Acknowledgements
-        ----------------
-        
-        This project/research has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 785907 (Human Brain Project SGA2).
-        
-        
-        License
-        -------
-        
-        libsonata is distributed under the terms of the GNU Lesser General Public License version 3,
-        unless noted otherwise, for example, for external dependencies.
-        Refer to `COPYING.LESSER` and `COPYING` files for details.
-        
-        Copyright (C) 2018-2020, Blue Brain Project/EPFL and contributors.
-        
-        libsonata is free software: you can redistribute it and/or modify
-        it under the terms of the GNU Lesser General Public License version 3
-        as published by the Free Software Foundation.
-        
-        libsonata is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Lesser General Public License for more details.
-        
-        You should have received a copy of the GNU Lesser General Public License
-        along with libsonata.  If not, see <https://www.gnu.org/licenses/>.
-        
-        
-        .. |license| image:: https://img.shields.io/pypi/l/libsonata
-                        :target: https://github.com/BlueBrain/libsonata/blob/master/COPYING.LESSER
-        
-        .. |coverage| image:: https://coveralls.io/repos/github/BlueBrain/libsonata/badge.svg
-                         :target: https://coveralls.io/github/BlueBrain/libsonata
-        
-        .. |docs| image:: https://readthedocs.org/projects/libsonata/badge/?version=latest
-                     :target: https://libsonata.readthedocs.io/
-                     :alt: documentation status
-        
-        .. substitutions
-        .. |banner| image:: docs/source/_images/libSonataLogo.jpg
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
+|banner|
+
+|license| |coverage| |docs|
+
+libsonata
+=========
+
+C++ / Python reader for SONATA circuit files:
+`SONATA guide <https://github.com/AllenInstitute/sonata/blob/master/docs/SONATA_DEVELOPER_GUIDE.md>`__
+
+Installation
+------------
+
+Installing from PyPI
+~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   pip install libsonata
+
+Installing as a Python package, directly from GitHub
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   pip install git+https://github.com/BlueBrain/libsonata
+
+Building the C++ library
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   git clone git@github.com:BlueBrain/libsonata.git --recursive
+   cd libsonata
+   mkdir build && cd build
+   cmake  -DCMAKE_BUILD_TYPE=Release  -DEXTLIB_FROM_SUBMODULES=ON ..
+   make -j
+
+Usage (Python)
+--------------
+
+Nodes
+~~~~~
+
+NodeStorage
++++++++++++
+
+.. code-block:: pycon
+
+   >>> import libsonata
+
+   >>> nodes = libsonata.NodeStorage('path/to/H5/file')
+
+   # list populations
+   >>> nodes.population_names
+
+   # open population
+   >>> population = nodes.open_population(<name>)
+
+
+NodePopulation
+++++++++++++++
+
+.. code-block:: pycon
+
+   # total number of nodes in the population
+   >>> population.size
+
+   # attribute names
+   >>> population.attribute_names
+
+   # get attribute value for single node, say 42
+   >>> population.get_attribute('mtype', 42)
+
+   # ...or Selection of nodes (see below) => returns NumPy array with corresponding values
+   >>> selection = libsonata.Selection(values=[1, 5, 9, 42])  # nodes 1, 5, 9, 42
+   >>> mtypes = population.get_attribute('mtype', selection)
+   >>> list(zip(selection.flatten(), mtypes))
+   [(1, u'mtype_of_1'), (5, u'mtype_of_5'), (9, u'mtype_of_9'), (42, u'mtype_of_42')]
+
+
+Selection
++++++++++
+
+List of element IDs (either `node_id`, or `edge_id`) where adjacent IDs are grouped for the sake of efficient HDF5 file access.
+For instance, `{1, 2, 3, 5}` sequence becomes `{[1, 4), [5, 6)}`.
+
+`Selection` can be instantiated from:
+ - a sequence of scalar values (works for NumPy arrays as well)
+ - a sequence of pairs (interpreted as ranges above, works for N x 2 NumPy arrays as well)
+
+`EdgePopulation` connectivity queries (see below) return ``Selection``\ s as well.
+
+.. code-block:: pycon
+
+   >>> selection = libsonata.Selection([1, 2, 3, 5])
+   >>> selection.ranges
+   [(1, 4), (5, 6)]
+
+
+.. code-block:: pycon
+
+   >>> selection = libsonata.Selection([(1, 4), (5, 6)])
+   >>> selection.flatten()
+   [1, 2, 3, 5]
+   >>> selection.flat_size
+   4
+   >>> bool(selection)
+   True
+
+
+Edges
+~~~~~
+
+EdgeStorage
++++++++++++
+
+Population handling for `EdgeStorage` is analogous to `NodeStorage`:
+
+.. code-block:: pycon
+
+   >>> edges = libsonata.EdgeStorage('path/to/H5/file')
+
+   # list populations
+   >>> edges.population_names
+
+   # open population
+   >>> population = edges.open_population(<name>)
+
+
+EdgePopulation
+++++++++++++++
+
+.. code-block:: pycon
+
+   # total number of edges in the population
+   >>> population.size
+
+   # attribute names
+   >>> population.attribute_names
+
+   # get attribute value for single edge, say 123
+   >>> population.get_attribute('delay', 123)
+
+   # ...or Selection of edges => returns NumPy array with corresponding values
+   >>> selection = libsonata.Selection([1, 5, 9])
+   >>> population.get_attribute('delay', selection) # returns delays for edges 1, 5, 9
+
+
+...with additional methods for querying connectivity, where the results are selections that can be applied like above
+
+.. code-block:: pycon
+
+   # get source / target node ID for the 42nd edge:
+   >>> population.source_node(42)
+   >>> population.target_node(42)
+
+   # query connectivity (result is Selection object)
+   >>> selection_to_1 = population.afferent_edges(1)  # all edges with target node_id 1
+   >>> population.target_nodes(selection_to_1)  # since selection only contains edges
+                                                # targeting node_id 1 the result will be a
+                                                # numpy array of all 1's
+   >>> selection_from_2 = population.efferent_edges(2)  # all edges sourced from node_id 2
+   >>> selection = population.connecting_edges(2, 1)  # this selection is all edges from
+                                                      # node_id 2 to node_id 1
+
+   # ...or their vectorized analogues
+   >>> selection = population.afferent_edges([1, 2, 3])
+   >>> selection = population.efferent_edges([1, 2, 3])
+   >>> selection = population.connecting_edges([1, 2, 3], [4, 5, 6])
+
+
+Reports
+~~~~~~~
+
+SpikeReader
++++++++++++
+
+.. code-block:: pycon
+
+   >>> import libsonata
+
+   >>> spikes = libsonata.SpikeReader('path/to/H5/file')
+
+   # list populations
+   >>> spikes.get_populations_names()
+
+   # open population
+   >>> population = spikes['<name>']
+
+
+SpikePopulation
++++++++++++++++
+
+.. code-block:: pycon
+
+   # get all spikes [(node_id, timestep)]
+   >>> population.get()
+   [(5, 0.1), (2, 0.2), (3, 0.3), (2, 0.7), (3, 1.3)]
+
+   # get all spikes betwen tstart and tstop
+   >>> population.get(tstart=0.2, tstop=1.0)
+   [(2, 0.2), (3, 0.3), (2, 0.7)]
+
+   # get spikes attribute sorting (by_time, by_id, none)
+   >>> population.sorting
+   'by_time'
+
+   Pandas can be used to create a dataframe and get a better representation of the data
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   data = population.get()
+   df = pandas.DataFrame(data=data, columns=['ids', 'times']).set_index('times')
+   print(df)
+          ids
+   times
+   0.1      5
+   0.2      2
+   0.3      3
+   0.7      2
+   1.3      3
+
+
+SomaReportReader
+++++++++++++++++
+
+.. code-block:: pycon
+
+   >>> somas = libsonata.SomaReportReader('path/to/H5/file')
+
+   # list populations
+   >>> somas.get_populations_names()
+
+   # open population
+   >>> population_somas = somas['<name>']
+
+
+SomaReportPopulation
+++++++++++++++++++++
+
+.. code-block:: pycon
+
+   # get times (tstart, tstop, dt)
+   >>> population_somas.times
+   (0.0, 1.0, 0.1)
+
+   # get unit attributes
+   >>> population_somas.time_units
+   'ms'
+   >>> population_somas.data_units
+   'mV'
+
+   # node_ids sorted?
+   >>> population_somas.sorted
+   True
+
+   # get a list of all node ids in the selected population
+   >>> population_somas.get_node_ids()
+   [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
+
+   # get the DataFrame of the node_id values for the timesteps between tstart and tstop
+   >>> data_frame = population_somas.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
+
+   # get the data values
+   >>> data_frame.data
+   [[13.8, 14.8], [13.9, 14.9]]
+
+   # get the list of timesteps
+   >>> data_frame.times
+   [0.8, 0.9]
+
+   # get the list of node ids
+   >>> data_frame.ids
+   [13, 14]
+
+
+Once again, pandas can be used to create a dataframe using the data, ids and times lists
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   df = pandas.DataFrame(data_frame.data, columns=data_frame.ids, index=data_frame.times)
+   print(df)
+          13    14
+   0.8  13.8  14.8
+   0.9  13.9  14.9
+
+
+ElementReportReader
++++++++++++++++++++
+
+.. code-block:: pycon
+
+   >>> elements = libsonata.ElementReportReader('path/to/H5/file')
+
+   # list populations
+   >>> elements.get_populations_names()
+
+   # open population
+   >>> population_elements = elements['<name>']
+
+
+ElementReportPopulation
++++++++++++++++++++++++
+
+.. code-block:: pycon
+
+   # get times (tstart, tstop, dt)
+   >>> population_elements.times
+   (0.0, 4.0, 0.2)
+
+   >>> population_elements.get_node_ids()
+   [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
+
+   # get the DataFrame of the node_id values for the timesteps between tstart and tstop
+   >>> data_frame = population_elements.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
+
+   # get the data values (list of list of floats with data[time_index][element_index])
+   >>> data_frame.data
+   [[46.0, 46.1, 46.2, 46.3, 46.4, 46.5, 46.6, 46.7, 46.8, 46.9], [56.0, 56.1, 56.2, 56.3, 56.4, 56.5, 56.6, 56.7, 56.8, 56.9]]
+
+   # get the list of timesteps
+   >>> data_frame.times
+   [0.8, 1.0]
+
+   # get the list of (node id, element_id)
+   >>> data_frame.ids
+   [(13, 30), (13, 30), (13, 31), (13, 31), (13, 32), (14, 32), (14, 33), (14, 33), (14, 34), (14, 34)]
+
+
+The same way than with spikes and soma reports, pandas can be used to get a better representation of the data
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   df = pandas.DataFrame(data_frame.data, columns=pandas.MultiIndex.from_tuples(data_frame.ids), index=data_frame.times)
+   print(df)
+          13                            14
+          30    30    31    31    32    32    33    33    34    34
+   0.8  46.0  46.1  46.2  46.3  46.4  46.5  46.6  46.7  46.8  46.9
+   1.0  56.0  56.1  56.2  56.3  56.4  56.5  56.6  56.7  56.8  56.9
+
+For big datasets, using numpy arrays could greatly improve the performance
+
+.. code-block:: pycon
+
+   >>> import numpy
+
+   np_data = numpy.asarray(data_frame.data)
+   np_ids = numpy.asarray(data_frame.ids).T
+   np_times = numpy.asarray(data_frame.times)
+
+   df = pandas.DataFrame(np_data, columns=pandas.MultiIndex.from_arrays(np_ids), index=np_times)
+
+
+Acknowledgements
+----------------
+The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
+
+This project/research has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 785907 (Human Brain Project SGA2).
+
+
+License
+-------
+
+libsonata is distributed under the terms of the GNU Lesser General Public License version 3,
+unless noted otherwise, for example, for external dependencies.
+Refer to `COPYING.LESSER` and `COPYING` files for details.
+
+Copyright (c) 2018-2021 Blue Brain Project/EPFL
+
+libsonata is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License version 3
+as published by the Free Software Foundation.
+
+libsonata is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License
+along with libsonata.  If not, see <https://www.gnu.org/licenses/>.
+
+
+.. |license| image:: https://img.shields.io/pypi/l/libsonata
+                :target: https://github.com/BlueBrain/libsonata/blob/master/COPYING.LESSER
+
+.. |coverage| image:: https://coveralls.io/repos/github/BlueBrain/libsonata/badge.svg
+                 :target: https://coveralls.io/github/BlueBrain/libsonata
+
+.. |docs| image:: https://readthedocs.org/projects/libsonata/badge/?version=latest
+             :target: https://libsonata.readthedocs.io/
+             :alt: documentation status
+
+.. substitutions
+.. |banner| image:: docs/source/_images/libSonataLogo.jpg
```

### Comparing `libsonata-0.1.8/python/tests/test.py` & `libsonata-0.1.9/python/tests/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import json
 import os
 import pathlib
 import unittest
 
 import numpy as np
 
 from libsonata import (EdgeStorage, NodeStorage,
                        Selection, SonataError,
                        SpikeReader, SpikePopulation,
                        SomaReportReader, SomaReportPopulation,
                        ElementReportReader, ElementReportPopulation,
                        NodeSets,
+                       CircuitConfig
                        )
 
 
 PATH = os.path.dirname(os.path.realpath(__file__))
 PATH = os.path.join(PATH, '../../tests/data')
 
 
@@ -458,14 +460,23 @@
               "location": ["layer4", "layer5"]
           },
           "V1_point_prime": {
               "population": "biophysical",
               "model_type": "point",
               "node_id": [1, 2, 3, 5, 7, 9]
           },
+          "power_number_test": {
+              "numeric_attribute_gt": { "$gt": 3 },
+              "numeric_attribute_lt": { "$lt": 3 },
+              "numeric_attribute_gte": { "$gte": 3 },
+              "numeric_attribute_lte": { "$lte": 3 }
+          },
+          "power_regex_test": {
+              "string_attr": { "$regex": "^[s][o]me value$" }
+          },
           "combined": ["bio_layer45", "V1_point_prime"]
         }'''
         new = NodeSets(j).toJSON()
         ns1 = NodeSets(new)
         self.assertEqual(new, ns1.toJSON())
 
         ns = NodeSets.from_file(os.path.join(PATH, 'node_sets.json'))
@@ -477,11 +488,51 @@
     path = pathlib.Path(PATH)
 
     NodeStorage(path / 'nodes1.h5')
     EdgeStorage(path / 'edges1.h5')
     SpikeReader(path / 'spikes.h5')
     SomaReportReader(path / 'somas.h5')
     ElementReportReader(path / 'elements.h5')
+    NodeSets.from_file(path / 'node_sets.json')
+    CircuitConfig.from_file(path / 'config/circuit_config.json')
+
+
+class TestCircuitConfig(unittest.TestCase):
+    def setUp(self):
+        self.config = CircuitConfig.from_file(os.path.join(PATH, 'config/circuit_config.json'))
+
+    def test_basic(self):
+        self.assertEqual(self.config.node_sets_path,
+                         os.path.abspath(os.path.join(PATH, 'config/node_sets.json')))
 
+        self.assertEqual(self.config.node_populations,
+                         {'nodes-A', 'nodes-B'})
+        self.assertEqual(self.config.node_population('nodes-A').name, 'nodes-A')
+
+        self.assertEqual(self.config.edge_populations,
+                         {'edges-AB', 'edges-AC'})
+        self.assertEqual(self.config.edge_population('edges-AB').name, 'edges-AB')
+
+    def test_expanded_json(self):
+        config = json.loads(self.config.expanded_json)
+        self.assertEqual(config['components']['biophysical_neuron_models_dir'],
+                         'biophysical_neuron_models')
+        self.assertEqual(config['networks']['nodes'][0]['node_types_file'],
+                         None)
+        self.assertEqual(config['networks']['nodes'][0]['nodes_file'],
+                         '../nodes1.h5')
+
+    def test_get_population_properties(self):
+        node_prop = self.config.node_population_properties('nodes-A')
+        self.assertEqual(node_prop.type, 'biophysical')
+        self.assertTrue(node_prop.morphologies_dir.endswith('morphologies'))
+        self.assertTrue(node_prop.biophysical_neuron_models_dir.endswith('biophysical_neuron_models'))
+        self.assertEqual(node_prop.alternate_morphology_formats, {})
+
+        edge_prop = self.config.edge_population_properties('edges-AC')
+        self.assertEqual(edge_prop.type, 'chemical_synapse')
+        self.assertTrue(edge_prop.morphologies_dir.endswith('morphologies'))
+        self.assertTrue(edge_prop.biophysical_neuron_models_dir.endswith('biophysical_neuron_models'))
+        self.assertEqual(edge_prop.alternate_morphology_formats, {})
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `libsonata-0.1.8/python/generated/docstrings.h` & `libsonata-0.1.9/python/generated/docstrings.h`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,118 @@
 
 #if defined(__GNUG__)
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wunused-variable"
 #endif
 
 
+static const char *__doc_bbp_sonata_CircuitConfig = R"doc(Read access to a SONATA circuit config file.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_CircuitConfig =
+R"doc(Parses a SONATA JSON config file.
+
+Throws:
+    s SonataError on: - Ill-formed JSON - Missing mandatory entries
+    (in any depth) - Missing entries which become mandatory when
+    another entry is present - Multiple populations with the same name
+    in different edge/node networks)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_Components = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_Components_alternateMorphologiesDir = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_Components_biophysicalNeuronModelsDir = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_Components_morphologiesDir = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_Parser = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_PopulationResolver = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_SubnetworkFiles = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_SubnetworkFiles_elements = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_SubnetworkFiles_populations = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_SubnetworkFiles_types = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_components = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_edgePopulationProperties = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_expandedJSON = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_fromFile =
+R"doc(Loads a SONATA JSON config file from disk and returns a CircuitConfig
+object which parses it.
+
+Throws:
+    s SonataError on: - Non accesible file (does not exists / does not
+    have read access) - Ill-formed JSON - Missing mandatory entries
+    (in any depth) - Missing entries which become mandatory when
+    another entry is present - Multiple populations with the same name
+    in different edge/node networks)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getEdgePopulation =
+R"doc(Creates and returns an EdgePopulation object, initialized from the
+given population, and the edge network it belongs to.
+
+Throws:
+    s SonataError if the given population does not exist in any edge
+    network.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getEdgePopulationProperties =
+R"doc(Return a structure containing edge population specific properties,
+falling back to network properties if there are no population-specific
+ones.
+
+Throws:
+    s SonataError if the given population name does not correspond to
+    any existing edge population.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getExpandedJSON =
+R"doc(Returns the configuration file JSON whose variables have been expanded
+by the manifest entries.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getNodePopulation =
+R"doc(Creates and returns a NodePopulation object, initialized from the
+given population, and the node network it belongs to.
+
+Throws:
+    s SonataError if the given population does not exist in any node
+    network.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getNodePopulationProperties =
+R"doc(Return a structure containing node population specific properties,
+falling back to network properties if there are no population-specific
+ones.
+
+Throws:
+    s SonataError if the given population name does not correspond to
+    any existing node population.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_getNodeSetsPath = R"doc(Returns the path to the node sets file.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_listEdgePopulations =
+R"doc(Returns a set with all available population names across all the edge
+networks.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_listNodePopulations =
+R"doc(Returns a set with all available population names across all the node
+networks.)doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_networkEdges = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_networkNodes = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_nodePopulationProperties = R"doc()doc";
+
+static const char *__doc_bbp_sonata_CircuitConfig_nodeSetsFile = R"doc()doc";
+
 static const char *__doc_bbp_sonata_DataFrame = R"doc()doc";
 
 static const char *__doc_bbp_sonata_DataFrame_data = R"doc()doc";
 
 static const char *__doc_bbp_sonata_DataFrame_ids = R"doc()doc";
 
 static const char *__doc_bbp_sonata_DataFrame_times = R"doc()doc";
@@ -71,14 +175,18 @@
 Throws:
     if the attribute dtype is not comparable
 
 Note: This does not match dynamics_params datasets)doc";
 
 static const char *__doc_bbp_sonata_NodePopulation_matchAttributeValues_2 = R"doc(Like matchAttributeValues, but for vectors of values to match)doc";
 
+static const char *__doc_bbp_sonata_NodePopulation_regexMatch =
+R"doc(For named attribute, return a selection where the passed regular
+expression matches)doc";
+
 static const char *__doc_bbp_sonata_NodeSets = R"doc()doc";
 
 static const char *__doc_bbp_sonata_NodeSets_NodeSets =
 R"doc(Create nodeset from JSON
 
 See also: https://github.com/AllenInstitute/sonata/blob/master/docs/SO
 NATA_DEVELOPER_GUIDE.md#node-sets-file
@@ -112,14 +220,24 @@
 
 static const char *__doc_bbp_sonata_NodeSets_operator_assign = R"doc()doc";
 
 static const char *__doc_bbp_sonata_NodeSets_toJSON = R"doc(Return string version of node sets)doc";
 
 static const char *__doc_bbp_sonata_Population = R"doc()doc";
 
+static const char *__doc_bbp_sonata_PopulationProperties = R"doc(Stores population-specific network information.)doc";
+
+static const char *__doc_bbp_sonata_PopulationProperties_alternateMorphologyFormats = R"doc(Dictionary for alternate directory paths.)doc";
+
+static const char *__doc_bbp_sonata_PopulationProperties_biophysicalNeuronModelsDir = R"doc(Path to the template HOC files defining the E-Mode)doc";
+
+static const char *__doc_bbp_sonata_PopulationProperties_morphologiesDir = R"doc(Path to the directory containing the morphologies)doc";
+
+static const char *__doc_bbp_sonata_PopulationProperties_type = R"doc(Population type)doc";
+
 static const char *__doc_bbp_sonata_PopulationStorage = R"doc(Collection of {PopulationClass}s stored in a H5 file and optional CSV.)doc";
 
 static const char *__doc_bbp_sonata_PopulationStorage_Impl = R"doc()doc";
 
 static const char *__doc_bbp_sonata_PopulationStorage_PopulationStorage = R"doc()doc";
 
 static const char *__doc_bbp_sonata_PopulationStorage_PopulationStorage_2 = R"doc()doc";
@@ -178,14 +296,16 @@
 
 Parameter ``name``:
     is a string to allow attributes not defined in spec
 
 Throws:
     if there is no such attribute for the population)doc";
 
+static const char *__doc_bbp_sonata_Population_filterAttribute = R"doc()doc";
+
 static const char *__doc_bbp_sonata_Population_getAttribute =
 R"doc(Get attribute values for given {element} Selection
 
 If string values are requested and the attribute is a explicit
 enumeration, values will be resolved to strings.
 
 See also: https://github.com/AllenInstitute/sonata/blob/master/docs/SO
```

### Comparing `libsonata-0.1.8/python/bindings.cpp` & `libsonata-0.1.9/python/bindings.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 #include <bbp/sonata/common.h>
+#include <bbp/sonata/config.h>
 #include <bbp/sonata/edges.h>
 #include <bbp/sonata/node_sets.h>
 #include <bbp/sonata/nodes.h>
 #include <bbp/sonata/report_reader.h>
 
 #include "generated/docstrings.h"
 
@@ -469,19 +470,46 @@
             "value"_a,
             DOC_POP_NODE(matchAttributeValues));
 
     bindStorageClass<NodeStorage>(m, "NodeStorage", "NodePopulation");
 
     py::class_<NodeSets>(m, "NodeSets", "")
         .def(py::init<const std::string&>())
-        .def_static("from_file", &NodeSets::fromFile)
+        .def_static("from_file", [](py::object path) { return NodeSets::fromFile(py::str(path)); })
         .def_property_readonly("names", &NodeSets::names, DOC_NODESETS(names))
         .def("materialize", &NodeSets::materialize, DOC_NODESETS(materialize))
         .def("toJSON", &NodeSets::toJSON, DOC_NODESETS(toJSON));
 
+    py::class_<PopulationProperties>(m,
+                                     "PopulationProperties",
+                                     "Stores population-specific network information")
+        .def_readonly("type", &PopulationProperties::type, "Population type")
+        .def_readonly("biophysical_neuron_models_dir",
+                      &PopulationProperties::biophysicalNeuronModelsDir,
+                      "Path to the template HOC files defining the E-Mode")
+        .def_readonly("morphologies_dir",
+                      &PopulationProperties::morphologiesDir,
+                      "Path to the directory containing the morphologies")
+        .def_readonly("alternate_morphology_formats",
+                      &PopulationProperties::alternateMorphologyFormats,
+                      "Path to the directory containing the morphologies");
+
+    py::class_<CircuitConfig>(m, "CircuitConfig", "")
+        .def(py::init<const std::string&, const std::string&>())
+        .def_static("from_file",
+                    [](py::object path) { return CircuitConfig::fromFile(py::str(path)); })
+        .def_property_readonly("node_sets_path", &CircuitConfig::getNodeSetsPath)
+        .def_property_readonly("node_populations", &CircuitConfig::listNodePopulations)
+        .def("node_population", &CircuitConfig::getNodePopulation)
+        .def_property_readonly("edge_populations", &CircuitConfig::listEdgePopulations)
+        .def("edge_population", &CircuitConfig::getEdgePopulation)
+        .def("node_population_properties", &CircuitConfig::getNodePopulationProperties, "name"_a)
+        .def("edge_population_properties", &CircuitConfig::getEdgePopulationProperties, "name"_a)
+        .def_property_readonly("expanded_json", &CircuitConfig::getExpandedJSON);
+
 
     bindPopulationClass<EdgePopulation>(
         m, "EdgePopulation", "Collection of edges with attributes and connectivity index")
         .def_property_readonly("source", &EdgePopulation::source, DOC_POP_EDGE(source))
         .def_property_readonly("target", &EdgePopulation::target, DOC_POP_EDGE(target))
         .def(
             "source_node",
```

### Comparing `libsonata-0.1.8/CHANGELOG.md` & `libsonata-0.1.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## v0.1.9: Thu 01 Jul 2021
+
+### Added:
+    * circuit_config.json implementation (#142)
+    * allow for simple expressions (#147) in node_sets as proposed to the 
+      offical SONATA spec in https://github.com/AllenInstitute/sonata/pull/129
+
+### Fixed:
+    * upgrade Catch2 to 2.13.6; autodetect test names (#148)
+    * move to fmt 7.1.2 (#145)
+
 ## v0.1.8: Wed 10 Feb 2021
 
 ### Fixed:
  - moved extlib/nlohmann/json.hpp one level deaper so that building with
    non-versioned nlohmann json is easier
 
 ## v0.1.7: Thu Jan 21 2021
```

### Comparing `libsonata-0.1.8/docs/Makefile` & `libsonata-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/docs/source/Doxyfile` & `libsonata-0.1.9/docs/source/Doxyfile`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/docs/source/_images/libSonataLogo.jpg` & `libsonata-0.1.9/docs/source/_images/libSonataLogo.jpg`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/docs/source/header.html` & `libsonata-0.1.9/docs/source/header.html`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/docs/source/DoxygenLayout.xml` & `libsonata-0.1.9/docs/source/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/docs/source/conf.py` & `libsonata-0.1.9/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,17 +99,16 @@
 
         if NAMESPACE_SEP not in f.name or NAMESPACE_ROOT not in f.name:
             continue
 
         type_, name = f.name.split(NAMESPACE_ROOT, maxsplit=1)
         name = NAMESPACE_ROOT + name
 
-        name = "".join(
-            s.capitalize() for s in name.replace(NAMESPACE_SEP, "::").split("_")
-        ).rstrip(".html")
+        name = "".join(s.capitalize() for s in name.replace(NAMESPACE_SEP, "::").split("_"))
+        name = re.sub(r"\.html?$", "", name)
         name = name[0].lower() + name[1:]
         name = name.replace("bbp::sonata::", "")
 
         filename = "doxygen_" + name
         context = {"title": name, "file": f.name}
 
         output_file = output_path / (filename + ".rst")
```

### Comparing `libsonata-0.1.8/include/bbp/sonata/edges.h` & `libsonata-0.1.9/include/bbp/sonata/edges.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/include/bbp/sonata/population.h` & `libsonata-0.1.9/include/bbp/sonata/population.h`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  *************************************************************************/
 
 #pragma once
 
 #include "common.h"
 
 #include <cstdint>
+#include <functional>
 #include <memory>  // std::shared_ptr, std::unique_ptr
 #include <set>
 #include <string>
 #include <utility>  // std::move
 #include <vector>
 
 
@@ -228,14 +229,17 @@
 
      * \internal
      * It is a helper method for dynamic languages bindings;
      * and is not intended for use in the ordinary client C++ code.
      */
     std::string _dynamicsAttributeDataType(const std::string& name) const;
 
+    template <typename T>
+    Selection filterAttribute(const std::string& name, std::function<bool(const T)> pred) const;
+
   protected:
     Population(const std::string& h5FilePath,
                const std::string& csvFilePath,
                const std::string& name,
                const std::string& prefix);
 
     Population(const Population&) = delete;
```

### Comparing `libsonata-0.1.8/include/bbp/sonata/nodes.h` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,88 @@
-/*************************************************************************
- * Copyright (C) 2018-2020 Blue Brain Project
+/*
+ *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
- * This file is part of 'libsonata', distributed under the terms
- * of the GNU Lesser General Public License version 3.
+ *  Distributed under the Boost Software License, Version 1.0.
+ *    (See accompanying file LICENSE_1_0.txt or copy at
+ *          http://www.boost.org/LICENSE_1_0.txt)
  *
- * See top-level COPYING.LESSER and COPYING files for details.
- *************************************************************************/
-
-#pragma once
-
-#include "common.h"
-#include "population.h"
-
-#include <string>
-#include <vector>
-
-
-namespace bbp {
-namespace sonata {
-
-//--------------------------------------------------------------------------------------------------
-
-class SONATA_API NodePopulation: public Population
-{
-  public:
-    constexpr static const char* ELEMENT = "node";
-
-    NodePopulation(const std::string& h5FilePath,
-                   const std::string& csvFilePath,
-                   const std::string& name);
-
-    /**
-     * Return selection of where attribute values match value
-     *
-     * As per node_set predicates, <tt>value</tt> must be one of type:
-     *
-     * <li>number  H5T_IEEE_*LE, H5T_STD_*LE</li>
-     * <li>string  H5T_C_S1</li>
-     * <li>bool    H5T_STD_I8LE</li>
-     * <li>null    invalid</li>
-     *
-     * \throw if the attribute dtype is not comparable
-     *
-     * Note: This does not match dynamics_params datasets
-     */
-    template <typename T>
-    Selection matchAttributeValues(const std::string& attribute, const T value) const;
-
-    /**
-     * Like matchAttributeValues, but for vectors of values to match
-     */
-    template <typename T>
-    Selection matchAttributeValues(const std::string& attribute,
-                                   const std::vector<T>& values) const;
+ */
+#ifndef H5EASY_BITS_XTENSOR_HPP
+#define H5EASY_BITS_XTENSOR_HPP
+
+#include "../H5Easy.hpp"
+#include "H5Easy_misc.hpp"
+#include "H5Easy_scalar.hpp"
+
+#ifdef H5_USE_XTENSOR
+
+namespace H5Easy {
+
+namespace detail {
+
+template <class T>
+struct is_xtensor : std::false_type {};
+template <class T>
+struct is_xtensor<xt::xarray<T>> : std::true_type {};
+template <class T, size_t N>
+struct is_xtensor<xt::xtensor<T, N>> : std::true_type {};
+
+template <typename T>
+struct io_impl<T, typename std::enable_if<is_xtensor<T>::value>::type> {
+
+    inline static std::vector<size_t> shape(const T& data) {
+        return std::vector<size_t>(data.shape().cbegin(), data.shape().cend());
+    }
+
+    inline static DataSet dump(File& file,
+                               const std::string& path,
+                               const T& data,
+                               const DumpOptions& options) {
+        using value_type = typename std::decay_t<T>::value_type;
+        DataSet dataset = initDataset<value_type>(file, path, shape(data), options);
+        dataset.write_raw(data.data());
+        if (options.flush()) {
+            file.flush();
+        }
+        return dataset;
+    }
+
+    inline static T load(const File& file, const std::string& path) {
+        DataSet dataset = file.getDataSet(path);
+        std::vector<size_t> dims = dataset.getDimensions();
+        T data = T::from_shape(dims);
+        dataset.read(data.data());
+        return data;
+    }
+
+    inline static Attribute dumpAttribute(File& file,
+                                          const std::string& path,
+                                          const std::string& key,
+                                          const T& data,
+                                          const DumpOptions& options) {
+        using value_type = typename std::decay_t<T>::value_type;
+        Attribute attribute = initAttribute<value_type>(file, path, key, shape(data), options);
+        attribute.write_raw(data.data());
+        if (options.flush()) {
+            file.flush();
+        }
+        return attribute;
+    }
+
+    inline static T loadAttribute(const File& file,
+                                  const std::string& path,
+                                  const std::string& key) {
+        DataSet dataset = file.getDataSet(path);
+        Attribute attribute = dataset.getAttribute(key);
+        DataSpace dataspace = attribute.getSpace();
+        std::vector<size_t> dims = dataspace.getDimensions();
+        T data = T::from_shape(dims);
+        attribute.read(data.data());
+        return data;
+    }
 };
 
-//--------------------------------------------------------------------------------------------------
-
-using NodeStorage = PopulationStorage<NodePopulation>;
-
-//--------------------------------------------------------------------------------------------------
+}  // namespace detail
+}  // namespace H5Easy
 
-}  // namespace sonata
-}  // namespace bbp
+#endif  // H5_USE_XTENSOR
+#endif  // H5EASY_BITS_XTENSOR_HPP
```

### Comparing `libsonata-0.1.8/include/bbp/sonata/node_sets.h` & `libsonata-0.1.9/include/bbp/sonata/node_sets.h`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
      *
      * Note: floating point values aren't supported for comparison
      *
      * \param content is the JSON node_sets value
      * \throw if content cannot be parsed
      */
     NodeSets(const std::string& content);
-    NodeSets(NodeSets&&);
+    NodeSets(NodeSets&&) noexcept;
     NodeSets(const NodeSets& other) = delete;
-    NodeSets& operator=(NodeSets&&);
+    NodeSets& operator=(NodeSets&&) noexcept;
     ~NodeSets();
 
     /** Open a SONATA `node sets` file from a path */
     static NodeSets fromFile(const std::string& path);
 
     /**
      * Return a selection corresponding to the node_set name
```

### Comparing `libsonata-0.1.8/include/bbp/sonata/report_reader.h` & `libsonata-0.1.9/include/bbp/sonata/report_reader.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/include/bbp/sonata/common.h` & `libsonata-0.1.9/include/bbp/sonata/common.h`

 * *Files 12% similar despite different names*

```diff
@@ -41,9 +41,12 @@
 using ElementID = uint32_t;
 
 class SONATA_API SonataError: public std::runtime_error
 {
   public:
     explicit SonataError(const std::string& what);
 };
+
+#define THROW_IF_REACHED throw SonataError("Should never be reached");
+
 }  // namespace sonata
 }  // namespace bbp
```

### Comparing `libsonata-0.1.8/include/bbp/sonata/optional.hpp` & `libsonata-0.1.9/include/bbp/sonata/optional.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/README.rst` & `libsonata-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: libsonata
+Version: 0.1.9
+Summary: SONATA files reader
+Home-page: https://github.com/BlueBrain/libsonata
+Author: Blue Brain Project, EPFL
+License: LGPLv3
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+License-File: COPYING
+License-File: COPYING.LESSER
+
 |banner|
 
 |license| |coverage| |docs|
 
 libsonata
 =========
 
@@ -356,26 +370,27 @@
    np_times = numpy.asarray(data_frame.times)
 
    df = pandas.DataFrame(np_data, columns=pandas.MultiIndex.from_arrays(np_ids), index=np_times)
 
 
 Acknowledgements
 ----------------
+The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
 
 This project/research has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 785907 (Human Brain Project SGA2).
 
 
 License
 -------
 
 libsonata is distributed under the terms of the GNU Lesser General Public License version 3,
 unless noted otherwise, for example, for external dependencies.
 Refer to `COPYING.LESSER` and `COPYING` files for details.
 
-Copyright (C) 2018-2020, Blue Brain Project/EPFL and contributors.
+Copyright (c) 2018-2021 Blue Brain Project/EPFL
 
 libsonata is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License version 3
 as published by the Free Software Foundation.
 
 libsonata is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -394,7 +409,9 @@
 
 .. |docs| image:: https://readthedocs.org/projects/libsonata/badge/?version=latest
              :target: https://libsonata.readthedocs.io/
              :alt: documentation status
 
 .. substitutions
 .. |banner| image:: docs/source/_images/libSonataLogo.jpg
+
+
```

### Comparing `libsonata-0.1.8/src/hdf5_mutex.hpp` & `libsonata-0.1.9/src/hdf5_mutex.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/population.cpp` & `libsonata-0.1.9/src/population.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
  * See top-level COPYING.LESSER and COPYING files for details.
  *************************************************************************/
 
 #include <algorithm>  // std::copy, std::sort, std::max, std::min
 #include <utility>    // std::move
 
 #include "hdf5_mutex.hpp"
-#include "population.hpp"
+#include "utils.h"
 
 #include <fmt/format.h>
 #include <highfive/H5File.hpp>
 
+#include "population.hpp"
 
 namespace bbp {
 namespace sonata {
 
 namespace detail {
 using Range = Selection::Range;
 using Ranges = Selection::Ranges;
@@ -189,15 +190,15 @@
     } else if (dtype == HighFive::AtomicType<std::string>()) {
         return "string";
     } else {
         throw SonataError(fmt::format("Unexpected datatype for dataset '{}'", name));
     }
 }
 
-}  // unnamed namespace
+}  // anonymous namespace
 
 
 Population::Population(const std::string& h5FilePath,
                        const std::string& csvFilePath,
                        const std::string& name,
                        const std::string& prefix)
     : impl_([h5FilePath, csvFilePath, name, prefix] {
@@ -340,29 +341,51 @@
 
 
 std::string Population::_dynamicsAttributeDataType(const std::string& name) const {
     HDF5_LOCK_GUARD
     return _getDataType(impl_->getDynamicsAttributeDataSet(name), name);
 }
 
+template <>
+Selection Population::filterAttribute(const std::string& name,
+                                      std::function<bool(const std::string)> pred) const {
+    auto dtype = impl_->getAttributeDataSet(name).getDataType();
+    if (dtype != HighFive::AtomicType<std::string>()) {
+        throw SonataError("H5 dataset must be a string");
+    }
+
+    const auto& values = getAttribute<std::string>(name, selectAll());
+    return _getMatchingSelection(values, pred);
+}
+
+template <typename T>
+Selection Population::filterAttribute(const std::string& name,
+                                      std::function<bool(const T)> pred) const {
+    const auto& values = getAttribute<T>(name, selectAll());
+    return _getMatchingSelection(values, pred);
+}
+
+
 //--------------------------------------------------------------------------------------------------
 
 #define INSTANTIATE_TEMPLATE_METHODS(T)                                                         \
     template std::vector<T> Population::getAttribute<T>(const std::string&, const Selection&)   \
         const;                                                                                  \
     template std::vector<T> Population::getAttribute<T>(const std::string&,                     \
                                                         const Selection&,                       \
                                                         const T&) const;                        \
     template std::vector<T> Population::getEnumeration<T>(const std::string&, const Selection&) \
         const;                                                                                  \
     template std::vector<T> Population::getDynamicsAttribute<T>(const std::string&,             \
                                                                 const Selection&) const;        \
     template std::vector<T> Population::getDynamicsAttribute<T>(const std::string&,             \
                                                                 const Selection&,               \
-                                                                const T&) const;
+                                                                const T&) const;                \
+    template Selection Population::filterAttribute<T>(const std::string&,                       \
+                                                      std::function<bool(const T)> pred) const;
 
 
 INSTANTIATE_TEMPLATE_METHODS(float)
 INSTANTIATE_TEMPLATE_METHODS(double)
 
 INSTANTIATE_TEMPLATE_METHODS(int8_t)
 INSTANTIATE_TEMPLATE_METHODS(uint8_t)
```

### Comparing `libsonata-0.1.8/src/edge_index.h` & `libsonata-0.1.9/src/edge_index.h`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/nodes.cpp` & `libsonata-0.1.9/src/nodes.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -4,128 +4,148 @@
  * This file is part of 'libsonata', distributed under the terms
  * of the GNU Lesser General Public License version 3.
  *
  * See top-level COPYING.LESSER and COPYING files for details.
  *************************************************************************/
 
 #include "population.hpp"
+#include "utils.h"
 
-#include <algorithm>  // std::binary_search
+#include <algorithm>  // std::binary_search, std::max_element, std::any_of
+#include <regex>
 
 #include <fmt/format.h>
 
 #include <bbp/sonata/common.h>
 #include <bbp/sonata/nodes.h>
 
-
 namespace bbp {
 namespace sonata {
 
-//--------------------------------------------------------------------------------------------------
-
-NodePopulation::NodePopulation(const std::string& h5FilePath,
-                               const std::string& csvFilePath,
-                               const std::string& name)
-    : Population(h5FilePath, csvFilePath, name, ELEMENT) {}
-
-
 namespace {
 
 template <typename T>
-Selection _getMatchingSelection(const std::vector<T>& values, const std::vector<T>& wanted) {
-    Selection::Values idx;
-    Selection::Value id = 0;
-
-    if (wanted.size() == 1) {
-        for (const auto& v : values) {
-            if (v == wanted[0]) {
-                idx.push_back(id);
-            }
-            ++id;
-        }
+Selection _matchAttributeValues(const NodePopulation& population,
+                                const std::string& name,
+                                const std::vector<T>& wanted) {
+    if (wanted.empty()) {
+        return Selection({});
+    } else if (wanted.size() == 1) {
+        return population.filterAttribute<T>(name,
+                                             [&wanted](const T& v) { return wanted[0] == v; });
     } else {
         std::vector<T> wanted_sorted(wanted);
         std::sort(wanted_sorted.begin(), wanted_sorted.end());
-        for (const auto& v : values) {
-            if (std::binary_search(wanted_sorted.cbegin(), wanted_sorted.cend(), v)) {
-                idx.push_back(id);
+
+        const auto pred = [&wanted_sorted](const T& v) {
+            return std::binary_search(wanted_sorted.cbegin(), wanted_sorted.cend(), v);
+        };
+        return population.filterAttribute<T>(name, pred);
+    }
+}
+
+bool is_unsigned_int(const HighFive::DataType& dtype) {
+    return dtype == HighFive::AtomicType<uint8_t>() || dtype == HighFive::AtomicType<uint16_t>() ||
+           dtype == HighFive::AtomicType<uint32_t>() || dtype == HighFive::AtomicType<uint64_t>();
+}
+
+bool is_signed_int(const HighFive::DataType& dtype) {
+    return dtype == HighFive::AtomicType<int8_t>() || dtype == HighFive::AtomicType<int16_t>() ||
+           dtype == HighFive::AtomicType<int32_t>() || dtype == HighFive::AtomicType<int64_t>();
+}
+bool is_floating(const HighFive::DataType& dtype) {
+    return dtype == HighFive::AtomicType<float>() || dtype == HighFive::AtomicType<double>();
+}
+
+template <typename UnaryPredicate>
+Selection _filterStringAttribute(const NodePopulation& population,
+                                 std::string name,
+                                 UnaryPredicate pred) {
+    if (population.enumerationNames().count(name) > 0) {
+        const auto& enum_values = population.enumerationValues(name);
+        // it's assumed that the cardinality of a @library is low
+        // enough that a std::vector<bool> won't be too large
+        std::vector<bool> wanted_enum_mask(enum_values.size());
+
+        bool has_elements = false;
+        for (size_t i = 0; i < enum_values.size(); ++i) {
+            if (pred(enum_values[i])) {
+                wanted_enum_mask[i] = true;
+                has_elements = true;
             }
-            ++id;
         }
+
+        if (!has_elements) {
+            return Selection({});
+        }
+
+        const auto& values = population.getEnumeration<size_t>(name, population.selectAll());
+        return _getMatchingSelection(values, [&wanted_enum_mask](const size_t v) {
+            return wanted_enum_mask.at(v);
+        });
     }
-    return Selection::fromValues(idx);
-}
 
-template <typename T>
-Selection _matchAttributeValues(const NodePopulation& population,
-                                const std::string& name,
-                                const std::vector<T>& wanted) {
-    return _getMatchingSelection(population.getAttribute<T>(name, population.selectAll()), wanted);
+    // normal, non-enum, attribute
+    return population.filterAttribute<std::string>(name, pred);
 }
 }  // anonymous namespace
 
+NodePopulation::NodePopulation(const std::string& h5FilePath,
+                               const std::string& csvFilePath,
+                               const std::string& name)
+    : Population(h5FilePath, csvFilePath, name, ELEMENT) {}
+
+Selection NodePopulation::regexMatch(const std::string& name, const std::string& regex) const {
+    std::regex re(regex);
+    const auto pred = [re](const std::string& v) {
+        std::smatch match;
+        std::regex_search(v, match, re);
+        return !match.empty();
+    };
+    return _filterStringAttribute(*this, name, pred);
+}
+
 template <typename T>
-Selection NodePopulation::matchAttributeValues(const std::string& name,
-                                               const std::vector<T>& value) const {
-    auto dtype = impl_->getAttributeDataSet(name).getDataType();
-    if (dtype == HighFive::AtomicType<int8_t>() || dtype == HighFive::AtomicType<uint8_t>() ||
-        dtype == HighFive::AtomicType<int16_t>() || dtype == HighFive::AtomicType<uint16_t>() ||
-        dtype == HighFive::AtomicType<int32_t>() || dtype == HighFive::AtomicType<uint32_t>() ||
-        dtype == HighFive::AtomicType<int64_t>() || dtype == HighFive::AtomicType<uint64_t>()) {
-        return _matchAttributeValues<T>(*this, name, value);
-    } else if (dtype == HighFive::AtomicType<float>() || dtype == HighFive::AtomicType<double>()) {
+Selection NodePopulation::matchAttributeValues(const std::string& attribute,
+                                               const std::vector<T>& values) const {
+    auto dtype = impl_->getAttributeDataSet(attribute).getDataType();
+    if (is_unsigned_int(dtype) || is_signed_int(dtype)) {
+        return _matchAttributeValues<T>(*this, attribute, values);
+    } else if (is_floating(dtype)) {
         throw SonataError("Exact comparison for float/double explicitly not supported");
     } else {
         throw SonataError(
-            fmt::format("Unexpected datatype for dataset '{}'", _attributeDataType(name)));
+            fmt::format("Unexpected datatype for dataset '{}'", _attributeDataType(attribute)));
     }
 }
 
 template <typename T>
-Selection NodePopulation::matchAttributeValues(const std::string& name, const T value) const {
+Selection NodePopulation::matchAttributeValues(const std::string& attribute, const T value) const {
     std::vector<T> values{value};
-    return matchAttributeValues<T>(name, values);
+    return matchAttributeValues<T>(attribute, values);
 }
 
 template <>
 Selection NodePopulation::matchAttributeValues<std::string>(
-    const std::string& name, const std::vector<std::string>& values) const {
-    if (enumerationNames().count(name) > 0) {
-        const auto enum_values = enumerationValues(name);
-        std::vector<size_t> wanted_enum_value;
-        wanted_enum_value.reserve(values.size());
-        for (const auto& v : values) {
-            const auto wanted_index = std::find(enum_values.cbegin(), enum_values.cend(), v);
-            if (wanted_index != enum_values.cend()) {
-                wanted_enum_value.push_back(wanted_index - enum_values.cbegin());
-            }
-        }
-
-        if (wanted_enum_value.empty()) {
-            return Selection({});
-        }
+    const std::string& attribute, const std::vector<std::string>& values) const {
+    std::vector<std::string> values_sorted(values);
+    std::sort(values_sorted.begin(), values_sorted.end());
+
+    const auto pred = [&values_sorted](const std::string& v) {
+        return std::binary_search(values_sorted.cbegin(), values_sorted.cend(), v);
+    };
 
-        return _getMatchingSelection<size_t>(getEnumeration<size_t>(name, selectAll()),
-                                             wanted_enum_value);
-    }
-
-    auto dtype = impl_->getAttributeDataSet(name).getDataType();
-    if (dtype != HighFive::AtomicType<std::string>()) {
-        throw SonataError("H5 dataset must be a string");
-    }
-
-    // normal, non-enum, attribute
-    return _matchAttributeValues<std::string>(*this, name, values);
+    return _filterStringAttribute(*this, attribute, pred);
 }
 
 template <>
-Selection NodePopulation::matchAttributeValues<std::string>(const std::string& name,
+Selection NodePopulation::matchAttributeValues<std::string>(const std::string& attribute,
                                                             const std::string value) const {
     std::vector<std::string> values{value};
-    return matchAttributeValues<std::string>(name, values);
+    return matchAttributeValues<std::string>(attribute, values);
 }
 
 
 #define INSTANTIATE_TEMPLATE_METHODS(T)                                                            \
     template Selection NodePopulation::matchAttributeValues<T>(const std::string&, const T) const; \
     template Selection NodePopulation::matchAttributeValues<T>(const std::string&,                 \
                                                                const std::vector<T>&) const;
```

### Comparing `libsonata-0.1.8/src/utils.cpp` & `libsonata-0.1.9/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/edge_index.cpp` & `libsonata-0.1.9/src/edge_index.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/common.cpp` & `libsonata-0.1.9/src/common.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/population.hpp` & `libsonata-0.1.9/src/population.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/report_reader.cpp` & `libsonata-0.1.9/src/report_reader.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/edges.cpp` & `libsonata-0.1.9/src/edges.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/hdf5_mutex.cpp` & `libsonata-0.1.9/src/hdf5_mutex.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/src/node_sets.cpp` & `libsonata-0.1.9/src/node_sets.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 }
 
 class NodeSets;
 
 class NodeSetRule
 {
   public:
-    virtual ~NodeSetRule(){};
+    virtual ~NodeSetRule() = default;
 
     virtual Selection materialize(const NodeSets&, const NodePopulation&) const = 0;
     virtual std::string toJSON() const = 0;
 };
 
 using NodeSetRules = std::vector<std::unique_ptr<NodeSetRule>>;
 void parse_basic(const json& j, std::map<std::string, NodeSetRules>& node_sets);
 void parse_compound(const json& j, std::map<std::string, NodeSetRules>& node_sets);
 
 class NodeSets
 {
     std::map<std::string, NodeSetRules> node_sets_;
 
   public:
-    NodeSets(const std::string& content) {
+    explicit NodeSets(const std::string& content) {
         json j = json::parse(content);
         if (!j.is_object()) {
             throw SonataError("Top level node_set must be an object");
         }
 
         // Need to two pass parsing the json so that compound lookup can rely
         // on all the basic rules existing
@@ -172,21 +172,142 @@
         return toString("node_ids", values_);
     }
 
   private:
     Selection::Values values_;
 };
 
+class NodeSetBasicOperatorString: public NodeSetRule
+{
+  public:
+    explicit NodeSetBasicOperatorString(const std::string& attribute,
+                                        const std::string& op,
+                                        const std::string& value)
+        : op_(string2op(op))
+        , attribute_(attribute)
+        , value_(value) {}
+
+    Selection materialize(const detail::NodeSets& /* unused */,
+                          const NodePopulation& np) const final {
+        switch (op_) {
+        case Op::regex:
+            return np.regexMatch(attribute_, value_);
+        default:              // LCOV_EXCL_LINE
+            THROW_IF_REACHED  // LCOV_EXCL_LINE
+        }
+    }
+
+    std::string toJSON() const final {
+        return fmt::format(R"("{}": {{ "{}": "{}" }})", attribute_, op2string(op_), value_);
+    }
+
+    enum class Op {
+        regex = 1,
+    };
+
+    static Op string2op(const std::string& s) {
+        if (s == "$regex") {
+            return Op::regex;
+        }
+        throw SonataError(fmt::format("Operator '{}' not available for strings", s));
+    }
+
+    static std::string op2string(const Op op) {
+        switch (op) {
+        case Op::regex:
+            return "$regex";
+        default:              // LCOV_EXCL_LINE
+            THROW_IF_REACHED  // LCOV_EXCL_LINE
+        }
+    }
+
+  private:
+    Op op_;
+    std::string attribute_;
+    std::string value_;
+};
+
+class NodeSetBasicOperatorNumeric: public NodeSetRule
+{
+  public:
+    explicit NodeSetBasicOperatorNumeric(const std::string& name,
+                                         const std::string& op,
+                                         double value)
+        : name_(name)
+        , value_(value)
+        , op_(string2op(op)) {}
+
+    Selection materialize(const detail::NodeSets& /* unused */,
+                          const NodePopulation& np) const final {
+        switch (op_) {
+        case Op::gt:
+            return np.filterAttribute<double>(name_, [=](const double v) { return v > value_; });
+        case Op::lt:
+            return np.filterAttribute<double>(name_, [=](const double v) { return v < value_; });
+        case Op::gte:
+            return np.filterAttribute<double>(name_, [=](const double v) { return v >= value_; });
+        case Op::lte:
+            return np.filterAttribute<double>(name_, [=](const double v) { return v <= value_; });
+        default:              // LCOV_EXCL_LINE
+            THROW_IF_REACHED  // LCOV_EXCL_LINE
+        }
+    }
+
+    std::string toJSON() const final {
+        return fmt::format(R"("{}": {{ "{}": {} }})", name_, op2string(op_), value_);
+    }
+
+    enum class Op {
+        gt = 1,
+        lt = 2,
+        gte = 3,
+        lte = 4,
+    };
+
+    static Op string2op(const std::string& s) {
+        if (s == "$gt") {
+            return Op::gt;
+        } else if (s == "$lt") {
+            return Op::lt;
+        } else if (s == "$gte") {
+            return Op::gte;
+        } else if (s == "$lte") {
+            return Op::lte;
+        }
+        throw SonataError(fmt::format("Operator '{}' not available for numeric", s));
+    }
+
+    static std::string op2string(const Op op) {
+        switch (op) {
+        case Op::gt:
+            return "$gt";
+        case Op::lt:
+            return "$lt";
+        case Op::gte:
+            return "$gte";
+        case Op::lte:
+            return "$lte";
+        default:              // LCOV_EXCL_LINE
+            THROW_IF_REACHED  // LCOV_EXCL_LINE
+        }
+    }
+
+  private:
+    std::string name_;
+    double value_;
+    Op op_;
+};
+
 using CompoundTargets = std::vector<std::string>;
 class NodeSetCompoundRule: public NodeSetRule
 {
   public:
-    NodeSetCompoundRule(std::string name, const CompoundTargets& targets)
+    NodeSetCompoundRule(std::string name, CompoundTargets targets)
         : name_(std::move(name))
-        , targets_(targets) {}
+        , targets_(std::move(targets)) {}
 
     Selection materialize(const detail::NodeSets& ns, const NodePopulation& np) const final {
         Selection ret{{}};
         for (const auto& target : targets_) {
             ret = ret | ns.materialize(target, np);
         }
         return ret;
@@ -283,14 +404,34 @@
                 } else {
                     ret.emplace_back(
                         new NodeSetBasicRule<std::string>(attribute, std::move(values)));
                 }
             } else {
                 throw SonataError("Unknown array type");
             }
+        } else if (el.value().is_object()) {
+            const auto& definition = el.value();
+            if (definition.size() != 1) {
+                throw SonataError(
+                    fmt::format("Operator '{}' must have object with one key value pair",
+                                attribute));
+            }
+            const auto& key = definition.begin().key();
+            const auto& value = definition.begin().value();
+            if (value.is_number()) {
+                ret.emplace_back(
+                    new NodeSetBasicOperatorNumeric(attribute, key, value.get<double>()));
+            } else if (value.is_string()) {
+                ret.emplace_back(
+                    new NodeSetBasicOperatorString(attribute, key, value.get<std::string>()));
+            } else {
+                throw SonataError("Unknown operator");
+            }
+        } else {
+            THROW_IF_REACHED  // LCOV_EXCL_LINE
         }
     }
     return ret;
 }
 
 void parse_basic(const json& j, std::map<std::string, NodeSetRules>& node_sets) {
     for (const auto& el : j.items()) {
@@ -350,16 +491,16 @@
 }
 
 }  // namespace detail
 
 NodeSets::NodeSets(const std::string& content)
     : impl_(new detail::NodeSets(content)) {}
 
-NodeSets::NodeSets(NodeSets&&) = default;
-NodeSets& NodeSets::operator=(NodeSets&&) = default;
+NodeSets::NodeSets(NodeSets&&) noexcept = default;
+NodeSets& NodeSets::operator=(NodeSets&&) noexcept = default;
 NodeSets::~NodeSets() = default;
 
 NodeSets NodeSets::fromFile(const std::string& path) {
     const auto contents = readFile(path);
     return NodeSets(contents);
 }
```

### Comparing `libsonata-0.1.8/extlib/fmt/include/fmt/format.h` & `libsonata-0.1.9/extlib/fmt/include/fmt/format.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,492 +1,635 @@
 /*
  Formatting library for C++
 
  Copyright (c) 2012 - present, Victor Zverovich
- All rights reserved.
 
- Redistribution and use in source and binary forms, with or without
- modification, are permitted provided that the following conditions are met:
-
- 1. Redistributions of source code must retain the above copyright notice, this
-    list of conditions and the following disclaimer.
- 2. Redistributions in binary form must reproduce the above copyright notice,
-    this list of conditions and the following disclaimer in the documentation
-    and/or other materials provided with the distribution.
-
- THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
- ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
- WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
- DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
- ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
- (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
- LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
- ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
- (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
- SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ Permission is hereby granted, free of charge, to any person obtaining
+ a copy of this software and associated documentation files (the
+ "Software"), to deal in the Software without restriction, including
+ without limitation the rights to use, copy, modify, merge, publish,
+ distribute, sublicense, and/or sell copies of the Software, and to
+ permit persons to whom the Software is furnished to do so, subject to
+ the following conditions:
+
+ The above copyright notice and this permission notice shall be
+ included in all copies or substantial portions of the Software.
+
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+ EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+ MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+ NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+ LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+ OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+ WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+ --- Optional exception to the license ---
+
+ As an exception, if, as a result of your compiling your source code, portions
+ of this Software are embedded into a machine-executable object form of such
+ source code, you may redistribute such embedded portions in such object form
+ without including the above copyright and permission notices.
  */
 
 #ifndef FMT_FORMAT_H_
 #define FMT_FORMAT_H_
 
 #include <algorithm>
-#include <cassert>
+#include <cerrno>
 #include <cmath>
-#include <cstring>
+#include <cstdint>
 #include <limits>
 #include <memory>
 #include <stdexcept>
-#include <stdint.h>
 
-#ifdef __clang__
-# define FMT_CLANG_VERSION (__clang_major__ * 100 + __clang_minor__)
-#else
-# define FMT_CLANG_VERSION 0
-#endif
+#include "core.h"
 
 #ifdef __INTEL_COMPILER
-# define FMT_ICC_VERSION __INTEL_COMPILER
+#  define FMT_ICC_VERSION __INTEL_COMPILER
 #elif defined(__ICL)
-# define FMT_ICC_VERSION __ICL
+#  define FMT_ICC_VERSION __ICL
 #else
-# define FMT_ICC_VERSION 0
+#  define FMT_ICC_VERSION 0
 #endif
 
 #ifdef __NVCC__
-# define FMT_CUDA_VERSION (__CUDACC_VER_MAJOR__ * 100 + __CUDACC_VER_MINOR__)
+#  define FMT_CUDA_VERSION (__CUDACC_VER_MAJOR__ * 100 + __CUDACC_VER_MINOR__)
 #else
-# define FMT_CUDA_VERSION 0
-#endif
-
-#include "core.h"
-
-#if FMT_GCC_VERSION >= 406 || FMT_CLANG_VERSION
-# pragma GCC diagnostic push
-
-// Disable the warning about declaration shadowing because it affects too
-// many valid cases.
-# pragma GCC diagnostic ignored "-Wshadow"
-
-// Disable the warning about implicit conversions that may change the sign of
-// an integer; silencing it otherwise would require many explicit casts.
-# pragma GCC diagnostic ignored "-Wsign-conversion"
+#  define FMT_CUDA_VERSION 0
 #endif
 
-# if FMT_CLANG_VERSION
-#  pragma GCC diagnostic ignored "-Wgnu-string-literal-operator-template"
-# endif
-
-#ifdef _SECURE_SCL
-# define FMT_SECURE_SCL _SECURE_SCL
+#ifdef __has_builtin
+#  define FMT_HAS_BUILTIN(x) __has_builtin(x)
 #else
-# define FMT_SECURE_SCL 0
+#  define FMT_HAS_BUILTIN(x) 0
 #endif
 
-#if FMT_SECURE_SCL
-# include <iterator>
+#if FMT_GCC_VERSION || FMT_CLANG_VERSION
+#  define FMT_NOINLINE __attribute__((noinline))
+#else
+#  define FMT_NOINLINE
 #endif
 
-#ifdef __has_builtin
-# define FMT_HAS_BUILTIN(x) __has_builtin(x)
+#if __cplusplus == 201103L || __cplusplus == 201402L
+#  if defined(__INTEL_COMPILER) || defined(__PGI)
+#    define FMT_FALLTHROUGH
+#  elif defined(__clang__)
+#    define FMT_FALLTHROUGH [[clang::fallthrough]]
+#  elif FMT_GCC_VERSION >= 700 && \
+      (!defined(__EDG_VERSION__) || __EDG_VERSION__ >= 520)
+#    define FMT_FALLTHROUGH [[gnu::fallthrough]]
+#  else
+#    define FMT_FALLTHROUGH
+#  endif
+#elif FMT_HAS_CPP17_ATTRIBUTE(fallthrough) || \
+    (defined(_MSVC_LANG) && _MSVC_LANG >= 201703L)
+#  define FMT_FALLTHROUGH [[fallthrough]]
 #else
-# define FMT_HAS_BUILTIN(x) 0
+#  define FMT_FALLTHROUGH
 #endif
 
-#ifdef __GNUC_LIBSTD__
-# define FMT_GNUC_LIBSTD_VERSION (__GNUC_LIBSTD__ * 100 + __GNUC_LIBSTD_MINOR__)
+#ifndef FMT_MAYBE_UNUSED
+#  if FMT_HAS_CPP17_ATTRIBUTE(maybe_unused)
+#    define FMT_MAYBE_UNUSED [[maybe_unused]]
+#  else
+#    define FMT_MAYBE_UNUSED
+#  endif
 #endif
 
 #ifndef FMT_THROW
-# if FMT_EXCEPTIONS
-#  if FMT_MSC_VER
+#  if FMT_EXCEPTIONS
+#    if FMT_MSC_VER || FMT_NVCC
 FMT_BEGIN_NAMESPACE
-namespace internal {
-template <typename Exception>
-inline void do_throw(const Exception &x) {
-  // Silence unreachable code warnings in MSVC because these are nearly
-  // impossible to fix in a generic code.
+namespace detail {
+template <typename Exception> inline void do_throw(const Exception& x) {
+  // Silence unreachable code warnings in MSVC and NVCC because these
+  // are nearly impossible to fix in a generic code.
   volatile bool b = true;
-  if (b)
-    throw x;
-}
+  if (b) throw x;
 }
+}  // namespace detail
 FMT_END_NAMESPACE
-#   define FMT_THROW(x) fmt::internal::do_throw(x)
+#      define FMT_THROW(x) detail::do_throw(x)
+#    else
+#      define FMT_THROW(x) throw x
+#    endif
 #  else
-#   define FMT_THROW(x) throw x
+#    define FMT_THROW(x)              \
+      do {                            \
+        static_cast<void>(sizeof(x)); \
+        FMT_ASSERT(false, "");        \
+      } while (false)
 #  endif
-# else
-#  define FMT_THROW(x) do { static_cast<void>(sizeof(x)); assert(false); } while(false);
-# endif
 #endif
 
-#ifndef FMT_USE_USER_DEFINED_LITERALS
-// For Intel's compiler and NVIDIA's compiler both it and the system gcc/msc
-// must support UDLs.
-# if (FMT_HAS_FEATURE(cxx_user_literals) || \
-      FMT_GCC_VERSION >= 407 || FMT_MSC_VER >= 1900) && \
-      (!(FMT_ICC_VERSION || FMT_CUDA_VERSION) || \
-       FMT_ICC_VERSION >= 1500 || FMT_CUDA_VERSION >= 700)
-#  define FMT_USE_USER_DEFINED_LITERALS 1
-# else
-#  define FMT_USE_USER_DEFINED_LITERALS 0
-# endif
-#endif
-
-// EDG C++ Front End based compilers (icc, nvcc) do not currently support UDL
-// templates.
-#if FMT_USE_USER_DEFINED_LITERALS && \
-    FMT_ICC_VERSION == 0 && \
-    FMT_CUDA_VERSION == 0 && \
-    ((FMT_GCC_VERSION >= 600 && __cplusplus >= 201402L) || \
-    (defined(FMT_CLANG_VERSION) && FMT_CLANG_VERSION >= 304))
-# define FMT_UDL_TEMPLATE 1
+#if FMT_EXCEPTIONS
+#  define FMT_TRY try
+#  define FMT_CATCH(x) catch (x)
 #else
-# define FMT_UDL_TEMPLATE 0
+#  define FMT_TRY if (true)
+#  define FMT_CATCH(x) if (false)
 #endif
 
-#ifndef FMT_USE_EXTERN_TEMPLATES
-# ifndef FMT_HEADER_ONLY
-#  define FMT_USE_EXTERN_TEMPLATES \
-     ((FMT_CLANG_VERSION >= 209 && __cplusplus >= 201103L) || \
-      (FMT_GCC_VERSION >= 303 && FMT_HAS_GXX_CXX11))
-# else
-#  define FMT_USE_EXTERN_TEMPLATES 0
-# endif
-#endif
-
-#if FMT_HAS_GXX_CXX11 || FMT_HAS_FEATURE(cxx_trailing_return) || \
-    FMT_MSC_VER >= 1600
-# define FMT_USE_TRAILING_RETURN 1
-#else
-# define FMT_USE_TRAILING_RETURN 0
+#ifndef FMT_USE_USER_DEFINED_LITERALS
+// EDG based compilers (Intel, NVIDIA, Elbrus, etc), GCC and MSVC support UDLs.
+#  if (FMT_HAS_FEATURE(cxx_user_literals) || FMT_GCC_VERSION >= 407 || \
+       FMT_MSC_VER >= 1900) &&                                         \
+      (!defined(__EDG_VERSION__) || __EDG_VERSION__ >= /* UDL feature */ 480)
+#    define FMT_USE_USER_DEFINED_LITERALS 1
+#  else
+#    define FMT_USE_USER_DEFINED_LITERALS 0
+#  endif
+#endif
+
+#ifndef FMT_USE_UDL_TEMPLATE
+// EDG frontend based compilers (icc, nvcc, PGI, etc) and GCC < 6.4 do not
+// properly support UDL templates and GCC >= 9 warns about them.
+#  if FMT_USE_USER_DEFINED_LITERALS &&                         \
+      (!defined(__EDG_VERSION__) || __EDG_VERSION__ >= 501) && \
+      ((FMT_GCC_VERSION >= 604 && __cplusplus >= 201402L) ||   \
+       FMT_CLANG_VERSION >= 304) &&                            \
+      !defined(__PGI) && !defined(__NVCC__)
+#    define FMT_USE_UDL_TEMPLATE 1
+#  else
+#    define FMT_USE_UDL_TEMPLATE 0
+#  endif
+#endif
+
+#ifndef FMT_USE_FLOAT
+#  define FMT_USE_FLOAT 1
+#endif
+
+#ifndef FMT_USE_DOUBLE
+#  define FMT_USE_DOUBLE 1
 #endif
 
-#ifndef FMT_USE_GRISU
-# define FMT_USE_GRISU 0
+#ifndef FMT_USE_LONG_DOUBLE
+#  define FMT_USE_LONG_DOUBLE 1
+#endif
+
+// Defining FMT_REDUCE_INT_INSTANTIATIONS to 1, will reduce the number of
+// int_writer template instances to just one by only using the largest integer
+// type. This results in a reduction in binary size but will cause a decrease in
+// integer formatting performance.
+#if !defined(FMT_REDUCE_INT_INSTANTIATIONS)
+#  define FMT_REDUCE_INT_INSTANTIATIONS 0
 #endif
 
 // __builtin_clz is broken in clang with Microsoft CodeGen:
 // https://github.com/fmtlib/fmt/issues/519
-#ifndef _MSC_VER
-# if FMT_GCC_VERSION >= 400 || FMT_HAS_BUILTIN(__builtin_clz)
+#if (FMT_GCC_VERSION || FMT_HAS_BUILTIN(__builtin_clz)) && !FMT_MSC_VER
 #  define FMT_BUILTIN_CLZ(n) __builtin_clz(n)
-# endif
-
-# if FMT_GCC_VERSION >= 400 || FMT_HAS_BUILTIN(__builtin_clzll)
+#endif
+#if (FMT_GCC_VERSION || FMT_HAS_BUILTIN(__builtin_clzll)) && !FMT_MSC_VER
 #  define FMT_BUILTIN_CLZLL(n) __builtin_clzll(n)
-# endif
+#endif
+#if (FMT_GCC_VERSION || FMT_HAS_BUILTIN(__builtin_ctz))
+#  define FMT_BUILTIN_CTZ(n) __builtin_ctz(n)
+#endif
+#if (FMT_GCC_VERSION || FMT_HAS_BUILTIN(__builtin_ctzll))
+#  define FMT_BUILTIN_CTZLL(n) __builtin_ctzll(n)
 #endif
 
-// A workaround for gcc 4.4 that doesn't support union members with ctors.
-#if (FMT_GCC_VERSION && FMT_GCC_VERSION <= 404) || \
-    (FMT_MSC_VER && FMT_MSC_VER <= 1800)
-# define FMT_UNION struct
-#else
-# define FMT_UNION union
+#if FMT_MSC_VER
+#  include <intrin.h>  // _BitScanReverse[64], _BitScanForward[64], _umul128
 #endif
 
 // Some compilers masquerade as both MSVC and GCC-likes or otherwise support
 // __builtin_clz and __builtin_clzll, so only define FMT_BUILTIN_CLZ using the
 // MSVC intrinsics if the clz and clzll builtins are not available.
-#if FMT_MSC_VER && !defined(FMT_BUILTIN_CLZLL) && !defined(_MANAGED)
-# include <intrin.h>  // _BitScanReverse, _BitScanReverse64
-
+#if FMT_MSC_VER && !defined(FMT_BUILTIN_CLZLL) && \
+    !defined(FMT_BUILTIN_CTZLL) && !defined(_MANAGED)
 FMT_BEGIN_NAMESPACE
-namespace internal {
+namespace detail {
 // Avoid Clang with Microsoft CodeGen's -Wunknown-pragmas warning.
-# ifndef __clang__
-#  pragma intrinsic(_BitScanReverse)
-# endif
-inline uint32_t clz(uint32_t x) {
+#  ifndef __clang__
+#    pragma intrinsic(_BitScanForward)
+#    pragma intrinsic(_BitScanReverse)
+#  endif
+#  if defined(_WIN64) && !defined(__clang__)
+#    pragma intrinsic(_BitScanForward64)
+#    pragma intrinsic(_BitScanReverse64)
+#  endif
+
+inline int clz(uint32_t x) {
   unsigned long r = 0;
   _BitScanReverse(&r, x);
-
-  assert(x != 0);
+  FMT_ASSERT(x != 0, "");
   // Static analysis complains about using uninitialized data
   // "r", but the only way that can happen is if "x" is 0,
   // which the callers guarantee to not happen.
-# pragma warning(suppress: 6102)
-  return 31 - r;
+  FMT_SUPPRESS_MSC_WARNING(6102)
+  return 31 ^ static_cast<int>(r);
 }
-# define FMT_BUILTIN_CLZ(n) fmt::internal::clz(n)
+#  define FMT_BUILTIN_CLZ(n) detail::clz(n)
 
-# if defined(_WIN64) && !defined(__clang__)
-#  pragma intrinsic(_BitScanReverse64)
-# endif
-
-inline uint32_t clzll(uint64_t x) {
+inline int clzll(uint64_t x) {
   unsigned long r = 0;
-# ifdef _WIN64
+#  ifdef _WIN64
   _BitScanReverse64(&r, x);
-# else
+#  else
   // Scan the high 32 bits.
-  if (_BitScanReverse(&r, static_cast<uint32_t>(x >> 32)))
-    return 63 - (r + 32);
-
+  if (_BitScanReverse(&r, static_cast<uint32_t>(x >> 32))) return 63 ^ (r + 32);
   // Scan the low 32 bits.
   _BitScanReverse(&r, static_cast<uint32_t>(x));
-# endif
+#  endif
+  FMT_ASSERT(x != 0, "");
+  FMT_SUPPRESS_MSC_WARNING(6102)  // Suppress a bogus static analysis warning.
+  return 63 ^ static_cast<int>(r);
+}
+#  define FMT_BUILTIN_CLZLL(n) detail::clzll(n)
 
-  assert(x != 0);
-  // Static analysis complains about using uninitialized data
-  // "r", but the only way that can happen is if "x" is 0,
-  // which the callers guarantee to not happen.
-# pragma warning(suppress: 6102)
-  return 63 - r;
+inline int ctz(uint32_t x) {
+  unsigned long r = 0;
+  _BitScanForward(&r, x);
+  FMT_ASSERT(x != 0, "");
+  FMT_SUPPRESS_MSC_WARNING(6102)  // Suppress a bogus static analysis warning.
+  return static_cast<int>(r);
 }
-# define FMT_BUILTIN_CLZLL(n) fmt::internal::clzll(n)
+#  define FMT_BUILTIN_CTZ(n) detail::ctz(n)
+
+inline int ctzll(uint64_t x) {
+  unsigned long r = 0;
+  FMT_ASSERT(x != 0, "");
+  FMT_SUPPRESS_MSC_WARNING(6102)  // Suppress a bogus static analysis warning.
+#  ifdef _WIN64
+  _BitScanForward64(&r, x);
+#  else
+  // Scan the low 32 bits.
+  if (_BitScanForward(&r, static_cast<uint32_t>(x))) return static_cast<int>(r);
+  // Scan the high 32 bits.
+  _BitScanForward(&r, static_cast<uint32_t>(x >> 32));
+  r += 32;
+#  endif
+  return static_cast<int>(r);
 }
+#  define FMT_BUILTIN_CTZLL(n) detail::ctzll(n)
+}  // namespace detail
 FMT_END_NAMESPACE
 #endif
 
+// Enable the deprecated numeric alignment.
+#ifndef FMT_DEPRECATED_NUMERIC_ALIGN
+#  define FMT_DEPRECATED_NUMERIC_ALIGN 0
+#endif
+
 FMT_BEGIN_NAMESPACE
-namespace internal {
+namespace detail {
 
-// An equivalent of `*reinterpret_cast<Dest*>(&source)` that doesn't produce
+// An equivalent of `*reinterpret_cast<Dest*>(&source)` that doesn't have
 // undefined behavior (e.g. due to type aliasing).
 // Example: uint64_t d = bit_cast<uint64_t>(2.718);
 template <typename Dest, typename Source>
 inline Dest bit_cast(const Source& source) {
   static_assert(sizeof(Dest) == sizeof(Source), "size mismatch");
   Dest dest;
   std::memcpy(&dest, &source, sizeof(dest));
   return dest;
 }
 
-// An implementation of begin and end for pre-C++11 compilers such as gcc 4.
-template <typename C>
-FMT_CONSTEXPR auto begin(const C &c) -> decltype(c.begin()) {
-  return c.begin();
-}
-template <typename T, std::size_t N>
-FMT_CONSTEXPR T *begin(T (&array)[N]) FMT_NOEXCEPT { return array; }
-template <typename C>
-FMT_CONSTEXPR auto end(const C &c) -> decltype(c.end()) { return c.end(); }
-template <typename T, std::size_t N>
-FMT_CONSTEXPR T *end(T (&array)[N]) FMT_NOEXCEPT { return array + N; }
-
-// For std::result_of in gcc 4.4.
-template <typename Result>
-struct function {
-  template <typename T>
-  struct result { typedef Result type; };
-};
-
-struct dummy_int {
-  int data[2];
-  operator int() const { return 0; }
-};
-typedef std::numeric_limits<internal::dummy_int> fputil;
-
-// Dummy implementations of system functions such as signbit and ecvt called
-// if the latter are not available.
-inline dummy_int signbit(...) { return dummy_int(); }
-inline dummy_int _ecvt_s(...) { return dummy_int(); }
-inline dummy_int isinf(...) { return dummy_int(); }
-inline dummy_int _finite(...) { return dummy_int(); }
-inline dummy_int isnan(...) { return dummy_int(); }
-inline dummy_int _isnan(...) { return dummy_int(); }
-
-inline bool use_grisu() {
-  return FMT_USE_GRISU && std::numeric_limits<double>::is_iec559;
-}
-
-// Formats value using Grisu2 algorithm:
-// https://www.cs.tufts.edu/~nr/cs257/archive/florian-loitsch/printf.pdf
-template <typename Double>
-FMT_API typename std::enable_if<sizeof(Double) == sizeof(uint64_t)>::type
-  grisu2_format(Double value, char *buffer, size_t &size, char type,
-                int precision, bool write_decimal_point);
-template <typename Double>
-inline typename std::enable_if<sizeof(Double) != sizeof(uint64_t)>::type
-  grisu2_format(Double, char *, size_t &, char, int, bool) {}
-
-template <typename Allocator>
-typename Allocator::value_type *allocate(Allocator& alloc, std::size_t n) {
-#if __cplusplus >= 201103L || FMT_MSC_VER >= 1700
-  return std::allocator_traits<Allocator>::allocate(alloc, n);
+inline bool is_big_endian() {
+  const auto u = 1u;
+  struct bytes {
+    char data[sizeof(u)];
+  };
+  return bit_cast<bytes>(u).data[0] == 0;
+}
+
+// A fallback implementation of uintptr_t for systems that lack it.
+struct fallback_uintptr {
+  unsigned char value[sizeof(void*)];
+
+  fallback_uintptr() = default;
+  explicit fallback_uintptr(const void* p) {
+    *this = bit_cast<fallback_uintptr>(p);
+    if (is_big_endian()) {
+      for (size_t i = 0, j = sizeof(void*) - 1; i < j; ++i, --j)
+        std::swap(value[i], value[j]);
+    }
+  }
+};
+#ifdef UINTPTR_MAX
+using uintptr_t = ::uintptr_t;
+inline uintptr_t to_uintptr(const void* p) { return bit_cast<uintptr_t>(p); }
+#else
+using uintptr_t = fallback_uintptr;
+inline fallback_uintptr to_uintptr(const void* p) {
+  return fallback_uintptr(p);
+}
+#endif
+
+// Returns the largest possible value for type T. Same as
+// std::numeric_limits<T>::max() but shorter and not affected by the max macro.
+template <typename T> constexpr T max_value() {
+  return (std::numeric_limits<T>::max)();
+}
+template <typename T> constexpr int num_bits() {
+  return std::numeric_limits<T>::digits;
+}
+// std::numeric_limits<T>::digits may return 0 for 128-bit ints.
+template <> constexpr int num_bits<int128_t>() { return 128; }
+template <> constexpr int num_bits<uint128_t>() { return 128; }
+template <> constexpr int num_bits<fallback_uintptr>() {
+  return static_cast<int>(sizeof(void*) *
+                          std::numeric_limits<unsigned char>::digits);
+}
+
+FMT_INLINE void assume(bool condition) {
+  (void)condition;
+#if FMT_HAS_BUILTIN(__builtin_assume)
+  __builtin_assume(condition);
+#endif
+}
+
+// An approximation of iterator_t for pre-C++20 systems.
+template <typename T>
+using iterator_t = decltype(std::begin(std::declval<T&>()));
+template <typename T> using sentinel_t = decltype(std::end(std::declval<T&>()));
+
+// A workaround for std::string not having mutable data() until C++17.
+template <typename Char> inline Char* get_data(std::basic_string<Char>& s) {
+  return &s[0];
+}
+template <typename Container>
+inline typename Container::value_type* get_data(Container& c) {
+  return c.data();
+}
+
+#if defined(_SECURE_SCL) && _SECURE_SCL
+// Make a checked iterator to avoid MSVC warnings.
+template <typename T> using checked_ptr = stdext::checked_array_iterator<T*>;
+template <typename T> checked_ptr<T> make_checked(T* p, size_t size) {
+  return {p, size};
+}
 #else
-  return alloc.allocate(n);
+template <typename T> using checked_ptr = T*;
+template <typename T> inline T* make_checked(T* p, size_t) { return p; }
 #endif
+
+template <typename Container, FMT_ENABLE_IF(is_contiguous<Container>::value)>
+#if FMT_CLANG_VERSION
+__attribute__((no_sanitize("undefined")))
+#endif
+inline checked_ptr<typename Container::value_type>
+reserve(std::back_insert_iterator<Container> it, size_t n) {
+  Container& c = get_container(it);
+  size_t size = c.size();
+  c.resize(size + n);
+  return make_checked(get_data(c) + size, n);
 }
 
-// A helper function to suppress bogus "conditional expression is constant"
-// warnings.
 template <typename T>
-inline T const_check(T value) { return value; }
-}  // namespace internal
-FMT_END_NAMESPACE
+inline buffer_appender<T> reserve(buffer_appender<T> it, size_t n) {
+  buffer<T>& buf = get_container(it);
+  buf.try_reserve(buf.size() + n);
+  return it;
+}
+
+template <typename Iterator> inline Iterator& reserve(Iterator& it, size_t) {
+  return it;
+}
+
+template <typename T, typename OutputIt>
+constexpr T* to_pointer(OutputIt, size_t) {
+  return nullptr;
+}
+template <typename T> T* to_pointer(buffer_appender<T> it, size_t n) {
+  buffer<T>& buf = get_container(it);
+  auto size = buf.size();
+  if (buf.capacity() < size + n) return nullptr;
+  buf.try_resize(size + n);
+  return buf.data() + size;
+}
+
+template <typename Container, FMT_ENABLE_IF(is_contiguous<Container>::value)>
+inline std::back_insert_iterator<Container> base_iterator(
+    std::back_insert_iterator<Container>& it,
+    checked_ptr<typename Container::value_type>) {
+  return it;
+}
+
+template <typename Iterator>
+inline Iterator base_iterator(Iterator, Iterator it) {
+  return it;
+}
+
+// An output iterator that counts the number of objects written to it and
+// discards them.
+class counting_iterator {
+ private:
+  size_t count_;
 
-namespace std {
-// Standard permits specialization of std::numeric_limits. This specialization
-// is used to resolve ambiguity between isinf and std::isinf in glibc:
-// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=48891
-// and the same for isnan and signbit.
-template <>
-class numeric_limits<fmt::internal::dummy_int> :
-    public std::numeric_limits<int> {
  public:
-  // Portable version of isinf.
-  template <typename T>
-  static bool isinfinity(T x) {
-    using namespace fmt::internal;
-    // The resolution "priority" is:
-    // isinf macro > std::isinf > ::isinf > fmt::internal::isinf
-    if (const_check(sizeof(isinf(x)) != sizeof(dummy_int)))
-      return isinf(x) != 0;
-    return !_finite(static_cast<double>(x));
-  }
-
-  // Portable version of isnan.
-  template <typename T>
-  static bool isnotanumber(T x) {
-    using namespace fmt::internal;
-    if (const_check(sizeof(isnan(x)) != sizeof(fmt::internal::dummy_int)))
-      return isnan(x) != 0;
-    return _isnan(static_cast<double>(x)) != 0;
-  }
-
-  // Portable version of signbit.
-  static bool isnegative(double x) {
-    using namespace fmt::internal;
-    if (const_check(sizeof(signbit(x)) != sizeof(fmt::internal::dummy_int)))
-      return signbit(x) != 0;
-    if (x < 0) return true;
-    if (!isnotanumber(x)) return false;
-    int dec = 0, sign = 0;
-    char buffer[2];  // The buffer size must be >= 2 or _ecvt_s will fail.
-    _ecvt_s(buffer, sizeof(buffer), x, 0, &dec, &sign);
-    return sign != 0;
+  using iterator_category = std::output_iterator_tag;
+  using difference_type = std::ptrdiff_t;
+  using pointer = void;
+  using reference = void;
+  using _Unchecked_type = counting_iterator;  // Mark iterator as checked.
+
+  struct value_type {
+    template <typename T> void operator=(const T&) {}
+  };
+
+  counting_iterator() : count_(0) {}
+
+  size_t count() const { return count_; }
+
+  counting_iterator& operator++() {
+    ++count_;
+    return *this;
+  }
+  counting_iterator operator++(int) {
+    auto it = *this;
+    ++*this;
+    return it;
   }
-};
-}  // namespace std
 
-FMT_BEGIN_NAMESPACE
-template <typename Range>
-class basic_writer;
+  friend counting_iterator operator+(counting_iterator it, difference_type n) {
+    it.count_ += static_cast<size_t>(n);
+    return it;
+  }
 
-template <typename OutputIt, typename T = typename OutputIt::value_type>
-class output_range {
- private:
-  OutputIt it_;
+  value_type operator*() const { return {}; }
+};
 
-  // Unused yet.
-  typedef void sentinel;
-  sentinel end() const;
+template <typename OutputIt> class truncating_iterator_base {
+ protected:
+  OutputIt out_;
+  size_t limit_;
+  size_t count_;
+
+  truncating_iterator_base(OutputIt out, size_t limit)
+      : out_(out), limit_(limit), count_(0) {}
 
  public:
-  typedef OutputIt iterator;
-  typedef T value_type;
+  using iterator_category = std::output_iterator_tag;
+  using value_type = typename std::iterator_traits<OutputIt>::value_type;
+  using difference_type = void;
+  using pointer = void;
+  using reference = void;
+  using _Unchecked_type =
+      truncating_iterator_base;  // Mark iterator as checked.
 
-  explicit output_range(OutputIt it): it_(it) {}
-  OutputIt begin() const { return it_; }
+  OutputIt base() const { return out_; }
+  size_t count() const { return count_; }
 };
 
-// A range where begin() returns back_insert_iterator.
-template <typename Container>
-class back_insert_range:
-    public output_range<std::back_insert_iterator<Container>> {
-  typedef output_range<std::back_insert_iterator<Container>> base;
+// An output iterator that truncates the output and counts the number of objects
+// written to it.
+template <typename OutputIt,
+          typename Enable = typename std::is_void<
+              typename std::iterator_traits<OutputIt>::value_type>::type>
+class truncating_iterator;
+
+template <typename OutputIt>
+class truncating_iterator<OutputIt, std::false_type>
+    : public truncating_iterator_base<OutputIt> {
+  mutable typename truncating_iterator_base<OutputIt>::value_type blackhole_;
+
  public:
-  typedef typename Container::value_type value_type;
+  using value_type = typename truncating_iterator_base<OutputIt>::value_type;
 
-  back_insert_range(Container &c): base(std::back_inserter(c)) {}
-  back_insert_range(typename base::iterator it): base(it) {}
-};
+  truncating_iterator(OutputIt out, size_t limit)
+      : truncating_iterator_base<OutputIt>(out, limit) {}
 
-typedef basic_writer<back_insert_range<internal::buffer>> writer;
-typedef basic_writer<back_insert_range<internal::wbuffer>> wwriter;
+  truncating_iterator& operator++() {
+    if (this->count_++ < this->limit_) ++this->out_;
+    return *this;
+  }
 
-/** A formatting error such as invalid format string. */
-class format_error : public std::runtime_error {
+  truncating_iterator operator++(int) {
+    auto it = *this;
+    ++*this;
+    return it;
+  }
+
+  value_type& operator*() const {
+    return this->count_ < this->limit_ ? *this->out_ : blackhole_;
+  }
+};
+
+template <typename OutputIt>
+class truncating_iterator<OutputIt, std::true_type>
+    : public truncating_iterator_base<OutputIt> {
  public:
-  explicit format_error(const char *message)
-  : std::runtime_error(message) {}
+  truncating_iterator(OutputIt out, size_t limit)
+      : truncating_iterator_base<OutputIt>(out, limit) {}
 
-  explicit format_error(const std::string &message)
-  : std::runtime_error(message) {}
+  template <typename T> truncating_iterator& operator=(T val) {
+    if (this->count_++ < this->limit_) *this->out_++ = val;
+    return *this;
+  }
+
+  truncating_iterator& operator++() { return *this; }
+  truncating_iterator& operator++(int) { return *this; }
+  truncating_iterator& operator*() { return *this; }
 };
 
-namespace internal {
+template <typename Char>
+inline size_t count_code_points(basic_string_view<Char> s) {
+  return s.size();
+}
 
-#if FMT_SECURE_SCL
-template <typename T>
-struct checked { typedef stdext::checked_array_iterator<T*> type; };
+// Counts the number of code points in a UTF-8 string.
+inline size_t count_code_points(basic_string_view<char> s) {
+  const char* data = s.data();
+  size_t num_code_points = 0;
+  for (size_t i = 0, size = s.size(); i != size; ++i) {
+    if ((data[i] & 0xc0) != 0x80) ++num_code_points;
+  }
+  return num_code_points;
+}
 
-// Make a checked iterator to avoid warnings on MSVC.
-template <typename T>
-inline stdext::checked_array_iterator<T*> make_checked(T *p, std::size_t size) {
-  return {p, size};
+inline size_t count_code_points(basic_string_view<char8_type> s) {
+  return count_code_points(basic_string_view<char>(
+      reinterpret_cast<const char*>(s.data()), s.size()));
 }
-#else
-template <typename T>
-struct checked { typedef T *type; };
-template <typename T>
-inline T *make_checked(T *p, std::size_t) { return p; }
-#endif
 
-template <typename T>
-template <typename U>
-void basic_buffer<T>::append(const U *begin, const U *end) {
-  std::size_t new_size = size_ + internal::to_unsigned(end - begin);
-  reserve(new_size);
-  std::uninitialized_copy(begin, end,
-                          internal::make_checked(ptr_, capacity_) + size_);
-  size_ = new_size;
+template <typename Char>
+inline size_t code_point_index(basic_string_view<Char> s, size_t n) {
+  size_t size = s.size();
+  return n < size ? n : size;
 }
-}  // namespace internal
 
-// A UTF-8 code unit type.
-struct char8_t {
-  char value;
-  FMT_CONSTEXPR FMT_EXPLICIT operator bool() const FMT_NOEXCEPT {
-    return value != 0;
+// Calculates the index of the nth code point in a UTF-8 string.
+inline size_t code_point_index(basic_string_view<char8_type> s, size_t n) {
+  const char8_type* data = s.data();
+  size_t num_code_points = 0;
+  for (size_t i = 0, size = s.size(); i != size; ++i) {
+    if ((data[i] & 0xc0) != 0x80 && ++num_code_points > n) {
+      return i;
+    }
   }
-};
+  return s.size();
+}
 
-// A UTF-8 string view.
-class u8string_view : public basic_string_view<char8_t> {
- public:
-  typedef char8_t char_type;
+template <typename InputIt, typename OutChar>
+using needs_conversion = bool_constant<
+    std::is_same<typename std::iterator_traits<InputIt>::value_type,
+                 char>::value &&
+    std::is_same<OutChar, char8_type>::value>;
 
-  u8string_view(const char *s):
-    basic_string_view<char8_t>(reinterpret_cast<const char8_t*>(s)) {}
-  u8string_view(const char *s, size_t count) FMT_NOEXCEPT:
-    basic_string_view<char8_t>(reinterpret_cast<const char8_t*>(s), count) {}
-};
+template <typename OutChar, typename InputIt, typename OutputIt,
+          FMT_ENABLE_IF(!needs_conversion<InputIt, OutChar>::value)>
+OutputIt copy_str(InputIt begin, InputIt end, OutputIt it) {
+  return std::copy(begin, end, it);
+}
 
-#if FMT_USE_USER_DEFINED_LITERALS
-inline namespace literals {
-inline u8string_view operator"" _u(const char *s, std::size_t n) {
-  return {s, n};
+template <typename OutChar, typename InputIt, typename OutputIt,
+          FMT_ENABLE_IF(needs_conversion<InputIt, OutChar>::value)>
+OutputIt copy_str(InputIt begin, InputIt end, OutputIt it) {
+  return std::transform(begin, end, it,
+                        [](char c) { return static_cast<char8_type>(c); });
 }
+
+template <typename Char, typename InputIt>
+inline counting_iterator copy_str(InputIt begin, InputIt end,
+                                  counting_iterator it) {
+  return it + (end - begin);
 }
-#endif
 
-// A wrapper around std::locale used to reduce compile times since <locale>
-// is very heavy.
-class locale;
+template <typename T>
+using is_fast_float = bool_constant<std::numeric_limits<T>::is_iec559 &&
+                                    sizeof(T) <= sizeof(double)>;
 
-class locale_provider {
- public:
-  virtual ~locale_provider() {}
-  virtual fmt::locale locale();
-};
+#ifndef FMT_USE_FULL_CACHE_DRAGONBOX
+#  define FMT_USE_FULL_CACHE_DRAGONBOX 0
+#endif
+
+template <typename T>
+template <typename U>
+void buffer<T>::append(const U* begin, const U* end) {
+  do {
+    auto count = to_unsigned(end - begin);
+    try_reserve(size_ + count);
+    auto free_cap = capacity_ - size_;
+    if (free_cap < count) count = free_cap;
+    std::uninitialized_copy_n(begin, count, make_checked(ptr_ + size_, count));
+    size_ += count;
+    begin += count;
+  } while (begin != end);
+}
+
+template <typename OutputIt, typename T, typename Traits>
+void iterator_buffer<OutputIt, T, Traits>::flush() {
+  out_ = std::copy_n(data_, this->limit(this->size()), out_);
+  this->clear();
+}
+}  // namespace detail
 
 // The number of characters to store in the basic_memory_buffer object itself
 // to avoid dynamic memory allocation.
 enum { inline_buffer_size = 500 };
 
 /**
   \rst
   A dynamically growing memory buffer for trivially copyable/constructible types
   with the first ``SIZE`` elements stored in the object itself.
 
-  You can use one of the following typedefs for common character types:
+  You can use one of the following type aliases for common character types:
 
   +----------------+------------------------------+
   | Type           | Definition                   |
   +================+==============================+
   | memory_buffer  | basic_memory_buffer<char>    |
   +----------------+------------------------------+
   | wmemory_buffer | basic_memory_buffer<wchar_t> |
@@ -502,47 +645,52 @@
   .. code-block:: none
 
      The answer is 42.
 
   The output can be converted to an ``std::string`` with ``to_string(out)``.
   \endrst
  */
-template <typename T, std::size_t SIZE = inline_buffer_size,
-          typename Allocator = std::allocator<T> >
-class basic_memory_buffer: private Allocator, public internal::basic_buffer<T> {
+template <typename T, size_t SIZE = inline_buffer_size,
+          typename Allocator = std::allocator<T>>
+class basic_memory_buffer final : public detail::buffer<T> {
  private:
   T store_[SIZE];
 
+  // Don't inherit from Allocator avoid generating type_info for it.
+  Allocator alloc_;
+
   // Deallocate memory allocated by the buffer.
   void deallocate() {
     T* data = this->data();
-    if (data != store_) Allocator::deallocate(data, this->capacity());
+    if (data != store_) alloc_.deallocate(data, this->capacity());
   }
 
  protected:
-  void grow(std::size_t size) FMT_OVERRIDE;
+  void grow(size_t size) final FMT_OVERRIDE;
 
  public:
-  explicit basic_memory_buffer(const Allocator &alloc = Allocator())
-      : Allocator(alloc) {
+  using value_type = T;
+  using const_reference = const T&;
+
+  explicit basic_memory_buffer(const Allocator& alloc = Allocator())
+      : alloc_(alloc) {
     this->set(store_, SIZE);
   }
   ~basic_memory_buffer() { deallocate(); }
 
  private:
   // Move data from other to this buffer.
-  void move(basic_memory_buffer &other) {
-    Allocator &this_alloc = *this, &other_alloc = other;
-    this_alloc = std::move(other_alloc);
+  void move(basic_memory_buffer& other) {
+    alloc_ = std::move(other.alloc_);
     T* data = other.data();
-    std::size_t size = other.size(), capacity = other.capacity();
+    size_t size = other.size(), capacity = other.capacity();
     if (data == other.store_) {
       this->set(store_, capacity);
       std::uninitialized_copy(other.store_, other.store_ + size,
-                              internal::make_checked(store_, capacity));
+                              detail::make_checked(store_, capacity));
     } else {
       this->set(data, capacity);
       // Set pointer to the inline array so that delete is not called
       // when deallocating.
       other.set(other.store_, 0);
     }
     this->resize(size);
@@ -551,1816 +699,2591 @@
  public:
   /**
     \rst
     Constructs a :class:`fmt::basic_memory_buffer` object moving the content
     of the other object to it.
     \endrst
    */
-  basic_memory_buffer(basic_memory_buffer &&other) {
-    move(other);
-  }
+  basic_memory_buffer(basic_memory_buffer&& other) FMT_NOEXCEPT { move(other); }
 
   /**
     \rst
     Moves the content of the other ``basic_memory_buffer`` object to this one.
     \endrst
    */
-  basic_memory_buffer &operator=(basic_memory_buffer &&other) {
-    assert(this != &other);
+  basic_memory_buffer& operator=(basic_memory_buffer&& other) FMT_NOEXCEPT {
+    FMT_ASSERT(this != &other, "");
     deallocate();
     move(other);
     return *this;
   }
 
   // Returns a copy of the allocator associated with this buffer.
-  Allocator get_allocator() const { return *this; }
+  Allocator get_allocator() const { return alloc_; }
+
+  /**
+    Resizes the buffer to contain *count* elements. If T is a POD type new
+    elements may not be initialized.
+   */
+  void resize(size_t count) { this->try_resize(count); }
+
+  /** Increases the buffer capacity to *new_capacity*. */
+  void reserve(size_t new_capacity) { this->try_reserve(new_capacity); }
+
+  // Directly append data into the buffer
+  using detail::buffer<T>::append;
+  template <typename ContiguousRange>
+  void append(const ContiguousRange& range) {
+    append(range.data(), range.data() + range.size());
+  }
 };
 
-template <typename T, std::size_t SIZE, typename Allocator>
-void basic_memory_buffer<T, SIZE, Allocator>::grow(std::size_t size) {
-  std::size_t old_capacity = this->capacity();
-  std::size_t new_capacity = old_capacity + old_capacity / 2;
-  if (size > new_capacity)
-      new_capacity = size;
-  T *old_data = this->data();
-  T *new_data = internal::allocate<Allocator>(*this, new_capacity);
+template <typename T, size_t SIZE, typename Allocator>
+void basic_memory_buffer<T, SIZE, Allocator>::grow(size_t size) {
+#ifdef FMT_FUZZ
+  if (size > 5000) throw std::runtime_error("fuzz mode - won't grow that much");
+#endif
+  size_t old_capacity = this->capacity();
+  size_t new_capacity = old_capacity + old_capacity / 2;
+  if (size > new_capacity) new_capacity = size;
+  T* old_data = this->data();
+  T* new_data =
+      std::allocator_traits<Allocator>::allocate(alloc_, new_capacity);
   // The following code doesn't throw, so the raw pointer above doesn't leak.
   std::uninitialized_copy(old_data, old_data + this->size(),
-                          internal::make_checked(new_data, new_capacity));
+                          detail::make_checked(new_data, new_capacity));
   this->set(new_data, new_capacity);
   // deallocate must not throw according to the standard, but even if it does,
   // the buffer already uses the new storage and will deallocate it in
   // destructor.
-  if (old_data != store_)
-    Allocator::deallocate(old_data, old_capacity);
+  if (old_data != store_) alloc_.deallocate(old_data, old_capacity);
 }
 
-typedef basic_memory_buffer<char> memory_buffer;
-typedef basic_memory_buffer<wchar_t> wmemory_buffer;
+using memory_buffer = basic_memory_buffer<char>;
+using wmemory_buffer = basic_memory_buffer<wchar_t>;
 
-/**
-  \rst
-  A fixed-size memory buffer. For a dynamically growing buffer use
-  :class:`fmt::basic_memory_buffer`.
+template <typename T, size_t SIZE, typename Allocator>
+struct is_contiguous<basic_memory_buffer<T, SIZE, Allocator>> : std::true_type {
+};
 
-  Trying to increase the buffer size past the initial capacity will throw
-  ``std::runtime_error``.
-  \endrst
- */
-template <typename Char>
-class basic_fixed_buffer : public internal::basic_buffer<Char> {
+/** A formatting error such as invalid format string. */
+FMT_CLASS_API
+class FMT_API format_error : public std::runtime_error {
  public:
-  /**
-   \rst
-   Constructs a :class:`fmt::basic_fixed_buffer` object for *array* of the
-   given size.
-   \endrst
-   */
-  basic_fixed_buffer(Char *array, std::size_t size) {
-    this->set(array, size);
-  }
-
-  /**
-   \rst
-   Constructs a :class:`fmt::basic_fixed_buffer` object for *array* of the
-   size known at compile time.
-   \endrst
-   */
-  template <std::size_t SIZE>
-  explicit basic_fixed_buffer(Char (&array)[SIZE]) {
-    this->set(array, SIZE);
-  }
-
- protected:
-  FMT_API void grow(std::size_t size) FMT_OVERRIDE;
+  explicit format_error(const char* message) : std::runtime_error(message) {}
+  explicit format_error(const std::string& message)
+      : std::runtime_error(message) {}
+  format_error(const format_error&) = default;
+  format_error& operator=(const format_error&) = default;
+  format_error(format_error&&) = default;
+  format_error& operator=(format_error&&) = default;
+  ~format_error() FMT_NOEXCEPT FMT_OVERRIDE;
 };
 
-namespace internal {
-
-template <typename Char>
-struct char_traits;
-
-template <>
-struct char_traits<char> {
-  // Formats a floating-point number.
-  template <typename T>
-  FMT_API static int format_float(char *buffer, std::size_t size,
-      const char *format, int precision, T value);
-};
+namespace detail {
 
-template <>
-struct char_traits<wchar_t> {
-  template <typename T>
-  FMT_API static int format_float(wchar_t *buffer, std::size_t size,
-      const wchar_t *format, int precision, T value);
-};
-
-#if FMT_USE_EXTERN_TEMPLATES
-extern template int char_traits<char>::format_float<double>(
-    char *buffer, std::size_t size, const char* format, int precision,
-    double value);
-extern template int char_traits<char>::format_float<long double>(
-    char *buffer, std::size_t size, const char* format, int precision,
-    long double value);
-
-extern template int char_traits<wchar_t>::format_float<double>(
-    wchar_t *buffer, std::size_t size, const wchar_t* format, int precision,
-    double value);
-extern template int char_traits<wchar_t>::format_float<long double>(
-    wchar_t *buffer, std::size_t size, const wchar_t* format, int precision,
-    long double value);
-#endif
+template <typename T>
+using is_signed =
+    std::integral_constant<bool, std::numeric_limits<T>::is_signed ||
+                                     std::is_same<T, int128_t>::value>;
 
-template <typename Container>
-inline typename std::enable_if<
-  is_contiguous<Container>::value,
-  typename checked<typename Container::value_type>::type>::type
-    reserve(std::back_insert_iterator<Container> &it, std::size_t n) {
-  Container &c = internal::get_container(it);
-  std::size_t size = c.size();
-  c.resize(size + n);
-  return make_checked(&c[size], n);
+// Returns true if value is negative, false otherwise.
+// Same as `value < 0` but doesn't produce warnings if T is an unsigned type.
+template <typename T, FMT_ENABLE_IF(is_signed<T>::value)>
+FMT_CONSTEXPR bool is_negative(T value) {
+  return value < 0;
+}
+template <typename T, FMT_ENABLE_IF(!is_signed<T>::value)>
+FMT_CONSTEXPR bool is_negative(T) {
+  return false;
 }
 
-template <typename Iterator>
-inline Iterator &reserve(Iterator &it, std::size_t) { return it; }
-
-template <typename Char>
-class null_terminating_iterator;
-
-template <typename Char>
-FMT_CONSTEXPR_DECL const Char *pointer_from(null_terminating_iterator<Char> it);
-
-// An iterator that produces a null terminator on *end. This simplifies parsing
-// and allows comparing the performance of processing a null-terminated string
-// vs string_view.
-template <typename Char>
-class null_terminating_iterator {
- public:
-  typedef std::ptrdiff_t difference_type;
-  typedef Char value_type;
-  typedef const Char* pointer;
-  typedef const Char& reference;
-  typedef std::random_access_iterator_tag iterator_category;
-
-  null_terminating_iterator() : ptr_(0), end_(0) {}
-
-  FMT_CONSTEXPR null_terminating_iterator(const Char *ptr, const Char *end)
-    : ptr_(ptr), end_(end) {}
-
-  template <typename Range>
-  FMT_CONSTEXPR explicit null_terminating_iterator(const Range &r)
-    : ptr_(r.begin()), end_(r.end()) {}
-
-  FMT_CONSTEXPR null_terminating_iterator &operator=(const Char *ptr) {
-    assert(ptr <= end_);
-    ptr_ = ptr;
-    return *this;
-  }
-
-  FMT_CONSTEXPR Char operator*() const {
-    return ptr_ != end_ ? *ptr_ : 0;
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator++() {
-    ++ptr_;
-    return *this;
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator++(int) {
-    null_terminating_iterator result(*this);
-    ++ptr_;
-    return result;
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator--() {
-    --ptr_;
-    return *this;
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator+(difference_type n) {
-    return null_terminating_iterator(ptr_ + n, end_);
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator-(difference_type n) {
-    return null_terminating_iterator(ptr_ - n, end_);
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator+=(difference_type n) {
-    ptr_ += n;
-    return *this;
-  }
-
-  FMT_CONSTEXPR difference_type operator-(
-      null_terminating_iterator other) const {
-    return ptr_ - other.ptr_;
-  }
-
-  FMT_CONSTEXPR bool operator!=(null_terminating_iterator other) const {
-    return ptr_ != other.ptr_;
-  }
-
-  bool operator>=(null_terminating_iterator other) const {
-    return ptr_ >= other.ptr_;
-  }
-
-  // This should be a friend specialization pointer_from<Char> but the latter
-  // doesn't compile by gcc 5.1 due to a compiler bug.
-  template <typename CharT>
-  friend FMT_CONSTEXPR_DECL const CharT *pointer_from(
-      null_terminating_iterator<CharT> it);
-
- private:
-  const Char *ptr_;
-  const Char *end_;
-};
+template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_CONSTEXPR bool is_supported_floating_point(T) {
+  return (std::is_same<T, float>::value && FMT_USE_FLOAT) ||
+         (std::is_same<T, double>::value && FMT_USE_DOUBLE) ||
+         (std::is_same<T, long double>::value && FMT_USE_LONG_DOUBLE);
+}
 
+// Smallest of uint32_t, uint64_t, uint128_t that is large enough to
+// represent all values of an integral type T.
 template <typename T>
-FMT_CONSTEXPR const T *pointer_from(const T *p) { return p; }
+using uint32_or_64_or_128_t =
+    conditional_t<num_bits<T>() <= 32 && !FMT_REDUCE_INT_INSTANTIATIONS,
+                  uint32_t,
+                  conditional_t<num_bits<T>() <= 64, uint64_t, uint128_t>>;
 
-template <typename Char>
-FMT_CONSTEXPR const Char *pointer_from(null_terminating_iterator<Char> it) {
-  return it.ptr_;
-}
+// 128-bit integer type used internally
+struct FMT_EXTERN_TEMPLATE_API uint128_wrapper {
+  uint128_wrapper() = default;
 
-// An output iterator that counts the number of objects written to it and
-// discards them.
-template <typename T>
-class counting_iterator {
- private:
-  std::size_t count_;
-  mutable T blackhole_;
+#if FMT_USE_INT128
+  uint128_t internal_;
 
- public:
-  typedef std::output_iterator_tag iterator_category;
-  typedef T value_type;
-  typedef std::ptrdiff_t difference_type;
-  typedef T* pointer;
-  typedef T& reference;
-  typedef counting_iterator _Unchecked_type;  // Mark iterator as checked.
+  uint128_wrapper(uint64_t high, uint64_t low) FMT_NOEXCEPT
+      : internal_{static_cast<uint128_t>(low) |
+                  (static_cast<uint128_t>(high) << 64)} {}
 
-  counting_iterator(): count_(0) {}
+  uint128_wrapper(uint128_t u) : internal_{u} {}
 
-  std::size_t count() const { return count_; }
+  uint64_t high() const FMT_NOEXCEPT { return uint64_t(internal_ >> 64); }
+  uint64_t low() const FMT_NOEXCEPT { return uint64_t(internal_); }
 
-  counting_iterator& operator++() {
-    ++count_;
+  uint128_wrapper& operator+=(uint64_t n) FMT_NOEXCEPT {
+    internal_ += n;
     return *this;
   }
+#else
+  uint64_t high_;
+  uint64_t low_;
 
-  counting_iterator operator++(int) {
-    auto it = *this;
-    ++*this;
-    return it;
-  }
-
-  T &operator*() const { return blackhole_; }
-};
-
-// An output iterator that truncates the output and counts the number of objects
-// written to it.
-template <typename OutputIt>
-class truncating_iterator {
- private:
-  typedef std::iterator_traits<OutputIt> traits;
-
-  OutputIt out_;
-  std::size_t limit_;
-  std::size_t count_;
-  mutable typename traits::value_type blackhole_;
-
- public:
-  typedef std::output_iterator_tag iterator_category;
-  typedef typename traits::value_type value_type;
-  typedef typename traits::difference_type difference_type;
-  typedef typename traits::pointer pointer;
-  typedef typename traits::reference reference;
-  typedef truncating_iterator _Unchecked_type;  // Mark iterator as checked.
+  uint128_wrapper(uint64_t high, uint64_t low) FMT_NOEXCEPT : high_{high},
+                                                              low_{low} {}
 
-  truncating_iterator(OutputIt out, std::size_t limit)
-    : out_(out), limit_(limit), count_(0) {}
+  uint64_t high() const FMT_NOEXCEPT { return high_; }
+  uint64_t low() const FMT_NOEXCEPT { return low_; }
 
-  OutputIt base() const { return out_; }
-  std::size_t count() const { return count_; }
-
-  truncating_iterator& operator++() {
-    if (count_++ < limit_)
-      ++out_;
+  uint128_wrapper& operator+=(uint64_t n) FMT_NOEXCEPT {
+#  if defined(_MSC_VER) && defined(_M_X64)
+    unsigned char carry = _addcarry_u64(0, low_, n, &low_);
+    _addcarry_u64(carry, high_, 0, &high_);
     return *this;
+#  else
+    uint64_t sum = low_ + n;
+    high_ += (sum < low_ ? 1 : 0);
+    low_ = sum;
+    return *this;
+#  endif
   }
-
-  truncating_iterator operator++(int) {
-    auto it = *this;
-    ++*this;
-    return it;
-  }
-
-  reference operator*() const { return count_ < limit_ ? *out_ : blackhole_; }
+#endif
 };
 
-// Returns true if value is negative, false otherwise.
-// Same as (value < 0) but doesn't produce warnings if T is an unsigned type.
-template <typename T>
-FMT_CONSTEXPR typename std::enable_if<
-    std::numeric_limits<T>::is_signed, bool>::type is_negative(T value) {
-  return value < 0;
-}
-template <typename T>
-FMT_CONSTEXPR typename std::enable_if<
-    !std::numeric_limits<T>::is_signed, bool>::type is_negative(T) {
-  return false;
+// Table entry type for divisibility test used internally
+template <typename T> struct FMT_EXTERN_TEMPLATE_API divtest_table_entry {
+  T mod_inv;
+  T max_quotient;
+};
+
+// Static data is placed in this class template for the header-only config.
+template <typename T = void> struct FMT_EXTERN_TEMPLATE_API basic_data {
+  static const uint64_t powers_of_10_64[];
+  static const uint32_t zero_or_powers_of_10_32_new[];
+  static const uint64_t zero_or_powers_of_10_64_new[];
+  static const uint64_t grisu_pow10_significands[];
+  static const int16_t grisu_pow10_exponents[];
+  static const divtest_table_entry<uint32_t> divtest_table_for_pow5_32[];
+  static const divtest_table_entry<uint64_t> divtest_table_for_pow5_64[];
+  static const uint64_t dragonbox_pow10_significands_64[];
+  static const uint128_wrapper dragonbox_pow10_significands_128[];
+  // log10(2) = 0x0.4d104d427de7fbcc...
+  static const uint64_t log10_2_significand = 0x4d104d427de7fbcc;
+#if !FMT_USE_FULL_CACHE_DRAGONBOX
+  static const uint64_t powers_of_5_64[];
+  static const uint32_t dragonbox_pow10_recovery_errors[];
+#endif
+  // GCC generates slightly better code for pairs than chars.
+  using digit_pair = char[2];
+  static const digit_pair digits[];
+  static const char hex_digits[];
+  static const char foreground_color[];
+  static const char background_color[];
+  static const char reset_color[5];
+  static const wchar_t wreset_color[5];
+  static const char signs[];
+  static const char left_padding_shifts[5];
+  static const char right_padding_shifts[5];
+
+  // DEPRECATED! These are for ABI compatibility.
+  static const uint32_t zero_or_powers_of_10_32[];
+  static const uint64_t zero_or_powers_of_10_64[];
+};
+
+// Maps bsr(n) to ceil(log10(pow(2, bsr(n) + 1) - 1)).
+// This is a function instead of an array to workaround a bug in GCC10 (#1810).
+FMT_INLINE uint16_t bsr2log10(int bsr) {
+  static constexpr uint16_t data[] = {
+      1,  1,  1,  2,  2,  2,  3,  3,  3,  4,  4,  4,  4,  5,  5,  5,
+      6,  6,  6,  7,  7,  7,  7,  8,  8,  8,  9,  9,  9,  10, 10, 10,
+      10, 11, 11, 11, 12, 12, 12, 13, 13, 13, 13, 14, 14, 14, 15, 15,
+      15, 16, 16, 16, 16, 17, 17, 17, 18, 18, 18, 19, 19, 19, 19, 20};
+  return data[bsr];
 }
 
-template <typename T>
-struct int_traits {
-  // Smallest of uint32_t and uint64_t that is large enough to represent
-  // all values of T.
-  typedef typename std::conditional<
-    std::numeric_limits<T>::digits <= 32, uint32_t, uint64_t>::type main_type;
-};
-
-// Static data is placed in this class template to allow header-only
-// configuration.
-template <typename T = void>
-struct FMT_API basic_data {
-  static const uint32_t POWERS_OF_10_32[];
-  static const uint32_t ZERO_OR_POWERS_OF_10_32[];
-  static const uint64_t ZERO_OR_POWERS_OF_10_64[];
-  static const uint64_t POW10_SIGNIFICANDS[];
-  static const int16_t POW10_EXPONENTS[];
-  static const char DIGITS[];
-  static const char FOREGROUND_COLOR[];
-  static const char BACKGROUND_COLOR[];
-  static const char RESET_COLOR[];
-  static const wchar_t WRESET_COLOR[];
-};
-
-#if FMT_USE_EXTERN_TEMPLATES
-extern template struct basic_data<void>;
+#ifndef FMT_EXPORTED
+FMT_EXTERN template struct basic_data<void>;
 #endif
 
-typedef basic_data<> data;
+// This is a struct rather than an alias to avoid shadowing warnings in gcc.
+struct data : basic_data<> {};
 
 #ifdef FMT_BUILTIN_CLZLL
 // Returns the number of decimal digits in n. Leading zeros are not counted
 // except for n == 0 in which case count_digits returns 1.
-inline unsigned count_digits(uint64_t n) {
-  // Based on http://graphics.stanford.edu/~seander/bithacks.html#IntegerLog10
-  // and the benchmark https://github.com/localvoid/cxx-benchmark-count-digits.
-  int t = (64 - FMT_BUILTIN_CLZLL(n | 1)) * 1233 >> 12;
-  return to_unsigned(t) - (n < data::ZERO_OR_POWERS_OF_10_64[t]) + 1;
+inline int count_digits(uint64_t n) {
+  // https://github.com/fmtlib/format-benchmark/blob/master/digits10
+  auto t = bsr2log10(FMT_BUILTIN_CLZLL(n | 1) ^ 63);
+  return t - (n < data::zero_or_powers_of_10_64_new[t]);
 }
 #else
 // Fallback version of count_digits used when __builtin_clz is not available.
-inline unsigned count_digits(uint64_t n) {
-  unsigned count = 1;
+inline int count_digits(uint64_t n) {
+  int count = 1;
   for (;;) {
     // Integer division is slow so do it for a group of four digits instead
     // of for every digit. The idea comes from the talk by Alexandrescu
     // "Three Optimization Tips for C++". See speed-test for a comparison.
     if (n < 10) return count;
     if (n < 100) return count + 1;
     if (n < 1000) return count + 2;
     if (n < 10000) return count + 3;
     n /= 10000u;
     count += 4;
   }
 }
 #endif
 
-// Counts the number of code points in a UTF-8 string.
-FMT_API size_t count_code_points(u8string_view s);
-
-#if FMT_HAS_CPP_ATTRIBUTE(always_inline)
-# define FMT_ALWAYS_INLINE __attribute__((always_inline))
-#else
-# define FMT_ALWAYS_INLINE
+#if FMT_USE_INT128
+inline int count_digits(uint128_t n) {
+  int count = 1;
+  for (;;) {
+    // Integer division is slow so do it for a group of four digits instead
+    // of for every digit. The idea comes from the talk by Alexandrescu
+    // "Three Optimization Tips for C++". See speed-test for a comparison.
+    if (n < 10) return count;
+    if (n < 100) return count + 1;
+    if (n < 1000) return count + 2;
+    if (n < 10000) return count + 3;
+    n /= 10000U;
+    count += 4;
+  }
+}
 #endif
 
-template <typename Handler>
-inline char *lg(uint32_t n, Handler h) FMT_ALWAYS_INLINE;
-
-// Computes g = floor(log10(n)) and calls h.on<g>(n);
-template <typename Handler>
-inline char *lg(uint32_t n, Handler h) {
-  return n < 100 ? n < 10 ? h.template on<0>(n) : h.template on<1>(n)
-                 : n < 1000000
-                       ? n < 10000 ? n < 1000 ? h.template on<2>(n)
-                                              : h.template on<3>(n)
-                                   : n < 100000 ? h.template on<4>(n)
-                                                : h.template on<5>(n)
-                       : n < 100000000 ? n < 10000000 ? h.template on<6>(n)
-                                                      : h.template on<7>(n)
-                                       : n < 1000000000 ? h.template on<8>(n)
-                                                        : h.template on<9>(n);
+// Counts the number of digits in n. BITS = log2(radix).
+template <unsigned BITS, typename UInt> inline int count_digits(UInt n) {
+  int num_digits = 0;
+  do {
+    ++num_digits;
+  } while ((n >>= BITS) != 0);
+  return num_digits;
 }
 
-// An lg handler that formats a decimal number.
-// Usage: lg(n, decimal_formatter(buffer));
-class decimal_formatter {
- private:
-  char *buffer_;
-
-  void write_pair(unsigned N, uint32_t index) {
-    std::memcpy(buffer_ + N, data::DIGITS + index * 2, 2);
-  }
-
- public:
-  explicit decimal_formatter(char *buf) : buffer_(buf) {}
-
-  template <unsigned N> char *on(uint32_t u) {
-    if (N == 0) {
-      *buffer_ = static_cast<char>(u) + '0';
-    } else if (N == 1) {
-      write_pair(0, u);
-    } else {
-      // The idea of using 4.32 fixed-point numbers is based on
-      // https://github.com/jeaiii/itoa
-      unsigned n = N - 1;
-      unsigned a = n / 5 * n * 53 / 16;
-      uint64_t t = ((1ULL << (32 + a)) /
-                   data::ZERO_OR_POWERS_OF_10_32[n] + 1 - n / 9);
-      t = ((t * u) >> a) + n / 5 * 4;
-      write_pair(0, t >> 32);
-      for (unsigned i = 2; i < N; i += 2) {
-        t = 100ULL * static_cast<uint32_t>(t);
-        write_pair(i, t >> 32);
-      }
-      if (N % 2 == 0) {
-        buffer_[N] = static_cast<char>(
-          (10ULL * static_cast<uint32_t>(t)) >> 32) + '0';
-      }
-    }
-    return buffer_ += N + 1;
-  }
-};
+template <> int count_digits<4>(detail::fallback_uintptr n);
 
-// An lg handler that formats a decimal number with a terminating null.
-class decimal_formatter_null : public decimal_formatter {
- public:
-  explicit decimal_formatter_null(char *buf) : decimal_formatter(buf) {}
+#if FMT_GCC_VERSION || FMT_CLANG_VERSION
+#  define FMT_ALWAYS_INLINE inline __attribute__((always_inline))
+#elif FMT_MSC_VER
+#  define FMT_ALWAYS_INLINE __forceinline
+#else
+#  define FMT_ALWAYS_INLINE inline
+#endif
 
-  template <unsigned N> char *on(uint32_t u) {
-    char *buf = decimal_formatter::on<N>(u);
-    *buf = '\0';
-    return buf;
-  }
-};
+// To suppress unnecessary security cookie checks
+#if FMT_MSC_VER && !FMT_CLANG_VERSION
+#  define FMT_SAFEBUFFERS __declspec(safebuffers)
+#else
+#  define FMT_SAFEBUFFERS
+#endif
 
 #ifdef FMT_BUILTIN_CLZ
 // Optional version of count_digits for better performance on 32-bit platforms.
-inline unsigned count_digits(uint32_t n) {
-  int t = (32 - FMT_BUILTIN_CLZ(n | 1)) * 1233 >> 12;
-  return to_unsigned(t) - (n < data::ZERO_OR_POWERS_OF_10_32[t]) + 1;
+inline int count_digits(uint32_t n) {
+  auto t = bsr2log10(FMT_BUILTIN_CLZ(n | 1) ^ 31);
+  return t - (n < data::zero_or_powers_of_10_32_new[t]);
 }
 #endif
 
-// A functor that doesn't add a thousands separator.
-struct no_thousands_sep {
-  typedef char char_type;
+template <typename Int> constexpr int digits10() FMT_NOEXCEPT {
+  return std::numeric_limits<Int>::digits10;
+}
+template <> constexpr int digits10<int128_t>() FMT_NOEXCEPT { return 38; }
+template <> constexpr int digits10<uint128_t>() FMT_NOEXCEPT { return 38; }
 
-  template <typename Char>
-  void operator()(Char *) {}
-};
+template <typename Char> FMT_API std::string grouping_impl(locale_ref loc);
+template <typename Char> inline std::string grouping(locale_ref loc) {
+  return grouping_impl<char>(loc);
+}
+template <> inline std::string grouping<wchar_t>(locale_ref loc) {
+  return grouping_impl<wchar_t>(loc);
+}
 
-// A functor that adds a thousands separator.
-template <typename Char>
-class add_thousands_sep {
- private:
-  basic_string_view<Char> sep_;
+template <typename Char> FMT_API Char thousands_sep_impl(locale_ref loc);
+template <typename Char> inline Char thousands_sep(locale_ref loc) {
+  return Char(thousands_sep_impl<char>(loc));
+}
+template <> inline wchar_t thousands_sep(locale_ref loc) {
+  return thousands_sep_impl<wchar_t>(loc);
+}
 
-  // Index of a decimal digit with the least significant digit having index 0.
-  unsigned digit_index_;
+template <typename Char> FMT_API Char decimal_point_impl(locale_ref loc);
+template <typename Char> inline Char decimal_point(locale_ref loc) {
+  return Char(decimal_point_impl<char>(loc));
+}
+template <> inline wchar_t decimal_point(locale_ref loc) {
+  return decimal_point_impl<wchar_t>(loc);
+}
 
- public:
-  typedef Char char_type;
+// Compares two characters for equality.
+template <typename Char> bool equal2(const Char* lhs, const char* rhs) {
+  return lhs[0] == rhs[0] && lhs[1] == rhs[1];
+}
+inline bool equal2(const char* lhs, const char* rhs) {
+  return memcmp(lhs, rhs, 2) == 0;
+}
 
-  explicit add_thousands_sep(basic_string_view<Char> sep)
-    : sep_(sep), digit_index_(0) {}
+// Copies two characters from src to dst.
+template <typename Char> void copy2(Char* dst, const char* src) {
+  *dst++ = static_cast<Char>(*src++);
+  *dst = static_cast<Char>(*src);
+}
+FMT_INLINE void copy2(char* dst, const char* src) { memcpy(dst, src, 2); }
 
-  void operator()(Char *&buffer) {
-    if (++digit_index_ % 3 != 0)
-      return;
-    buffer -= sep_.size();
-    std::uninitialized_copy(sep_.data(), sep_.data() + sep_.size(),
-                            internal::make_checked(buffer, sep_.size()));
-  }
+template <typename Iterator> struct format_decimal_result {
+  Iterator begin;
+  Iterator end;
 };
 
-template <typename Char>
-FMT_API Char thousands_sep(locale_provider *lp);
-
-// Formats a decimal unsigned integer value writing into buffer.
-// thousands_sep is a functor that is called after writing each char to
-// add a thousands separator if necessary.
-template <typename UInt, typename Char, typename ThousandsSep>
-inline Char *format_decimal(Char *buffer, UInt value, unsigned num_digits,
-                            ThousandsSep thousands_sep) {
-  buffer += num_digits;
-  Char *end = buffer;
+// Formats a decimal unsigned integer value writing into out pointing to a
+// buffer of specified size. The caller must ensure that the buffer is large
+// enough.
+template <typename Char, typename UInt>
+inline format_decimal_result<Char*> format_decimal(Char* out, UInt value,
+                                                   int size) {
+  FMT_ASSERT(size >= count_digits(value), "invalid digit count");
+  out += size;
+  Char* end = out;
   while (value >= 100) {
     // Integer division is slow so do it for a group of two digits instead
     // of for every digit. The idea comes from the talk by Alexandrescu
     // "Three Optimization Tips for C++". See speed-test for a comparison.
-    unsigned index = static_cast<unsigned>((value % 100) * 2);
+    out -= 2;
+    copy2(out, data::digits[value % 100]);
     value /= 100;
-    *--buffer = data::DIGITS[index + 1];
-    thousands_sep(buffer);
-    *--buffer = data::DIGITS[index];
-    thousands_sep(buffer);
   }
   if (value < 10) {
-    *--buffer = static_cast<char>('0' + value);
-    return end;
+    *--out = static_cast<Char>('0' + value);
+    return {out, end};
   }
-  unsigned index = static_cast<unsigned>(value * 2);
-  *--buffer = data::DIGITS[index + 1];
-  thousands_sep(buffer);
-  *--buffer = data::DIGITS[index];
-  return end;
-}
-
-template <typename UInt, typename Iterator, typename ThousandsSep>
-inline Iterator format_decimal(
-    Iterator out, UInt value, unsigned num_digits, ThousandsSep sep) {
-  typedef typename ThousandsSep::char_type char_type;
-  // Buffer should be large enough to hold all digits (digits10 + 1) and null.
-  char_type buffer[std::numeric_limits<UInt>::digits10 + 2];
-  format_decimal(buffer, value, num_digits, sep);
-  return std::copy_n(buffer, num_digits, out);
-}
-
-template <typename It, typename UInt>
-inline It format_decimal(It out, UInt value, unsigned num_digits) {
-  return format_decimal(out, value, num_digits, no_thousands_sep());
+  out -= 2;
+  copy2(out, data::digits[value]);
+  return {out, end};
+}
+
+template <typename Char, typename UInt, typename Iterator,
+          FMT_ENABLE_IF(!std::is_pointer<remove_cvref_t<Iterator>>::value)>
+inline format_decimal_result<Iterator> format_decimal(Iterator out, UInt value,
+                                                      int size) {
+  // Buffer is large enough to hold all digits (digits10 + 1).
+  Char buffer[digits10<UInt>() + 1];
+  auto end = format_decimal(buffer, value, size).end;
+  return {out, detail::copy_str<Char>(buffer, end, out)};
 }
 
 template <unsigned BASE_BITS, typename Char, typename UInt>
-inline Char *format_uint(Char *buffer, UInt value, unsigned num_digits,
+inline Char* format_uint(Char* buffer, UInt value, int num_digits,
                          bool upper = false) {
   buffer += num_digits;
-  Char *end = buffer;
+  Char* end = buffer;
   do {
-    const char *digits = upper ? "0123456789ABCDEF" : "0123456789abcdef";
+    const char* digits = upper ? "0123456789ABCDEF" : data::hex_digits;
     unsigned digit = (value & ((1 << BASE_BITS) - 1));
-    *--buffer = BASE_BITS < 4 ? static_cast<char>('0' + digit) : digits[digit];
+    *--buffer = static_cast<Char>(BASE_BITS < 4 ? static_cast<char>('0' + digit)
+                                                : digits[digit]);
   } while ((value >>= BASE_BITS) != 0);
   return end;
 }
 
-template <unsigned BASE_BITS, typename It, typename UInt>
-inline It format_uint(It out, UInt value, unsigned num_digits,
-                      bool upper = false) {
-  // Buffer should be large enough to hold all digits (digits / BASE_BITS + 1)
-  // and null.
-  char buffer[std::numeric_limits<UInt>::digits / BASE_BITS + 2];
+template <unsigned BASE_BITS, typename Char>
+Char* format_uint(Char* buffer, detail::fallback_uintptr n, int num_digits,
+                  bool = false) {
+  auto char_digits = std::numeric_limits<unsigned char>::digits / 4;
+  int start = (num_digits + char_digits - 1) / char_digits - 1;
+  if (int start_digits = num_digits % char_digits) {
+    unsigned value = n.value[start--];
+    buffer = format_uint<BASE_BITS>(buffer, value, start_digits);
+  }
+  for (; start >= 0; --start) {
+    unsigned value = n.value[start];
+    buffer += char_digits;
+    auto p = buffer;
+    for (int i = 0; i < char_digits; ++i) {
+      unsigned digit = (value & ((1 << BASE_BITS) - 1));
+      *--p = static_cast<Char>(data::hex_digits[digit]);
+      value >>= BASE_BITS;
+    }
+  }
+  return buffer;
+}
+
+template <unsigned BASE_BITS, typename Char, typename It, typename UInt>
+inline It format_uint(It out, UInt value, int num_digits, bool upper = false) {
+  if (auto ptr = to_pointer<Char>(out, to_unsigned(num_digits))) {
+    format_uint<BASE_BITS>(ptr, value, num_digits, upper);
+    return out;
+  }
+  // Buffer should be large enough to hold all digits (digits / BASE_BITS + 1).
+  char buffer[num_bits<UInt>() / BASE_BITS + 1];
   format_uint<BASE_BITS>(buffer, value, num_digits, upper);
-  return std::copy_n(buffer, num_digits, out);
+  return detail::copy_str<Char>(buffer, buffer + num_digits, out);
 }
 
-#ifndef _WIN32
-# define FMT_USE_WINDOWS_H 0
-#elif !defined(FMT_USE_WINDOWS_H)
-# define FMT_USE_WINDOWS_H 1
-#endif
-
-// Define FMT_USE_WINDOWS_H to 0 to disable use of windows.h.
-// All the functionality that relies on it will be disabled too.
-#if FMT_USE_WINDOWS_H
 // A converter from UTF-8 to UTF-16.
-// It is only provided for Windows since other systems support UTF-8 natively.
 class utf8_to_utf16 {
  private:
   wmemory_buffer buffer_;
 
  public:
   FMT_API explicit utf8_to_utf16(string_view s);
-  operator wstring_view() const { return wstring_view(&buffer_[0], size()); }
+  operator wstring_view() const { return {&buffer_[0], size()}; }
   size_t size() const { return buffer_.size() - 1; }
-  const wchar_t *c_str() const { return &buffer_[0]; }
-  std::wstring str() const { return std::wstring(&buffer_[0], size()); }
-};
-
-// A converter from UTF-16 to UTF-8.
-// It is only provided for Windows since other systems support UTF-8 natively.
-class utf16_to_utf8 {
- private:
-  memory_buffer buffer_;
-
- public:
-  utf16_to_utf8() {}
-  FMT_API explicit utf16_to_utf8(wstring_view s);
-  operator string_view() const { return string_view(&buffer_[0], size()); }
-  size_t size() const { return buffer_.size() - 1; }
-  const char *c_str() const { return &buffer_[0]; }
-  std::string str() const { return std::string(&buffer_[0], size()); }
-
-  // Performs conversion returning a system error code instead of
-  // throwing exception on conversion error. This method may still throw
-  // in case of memory allocation error.
-  FMT_API int convert(wstring_view s);
-};
-
-FMT_API void format_windows_error(fmt::internal::buffer &out, int error_code,
-                                  fmt::string_view message) FMT_NOEXCEPT;
-#endif
-
-template <typename T = void>
-struct null {};
-}  // namespace internal
-
-enum alignment {
-  ALIGN_DEFAULT, ALIGN_LEFT, ALIGN_RIGHT, ALIGN_CENTER, ALIGN_NUMERIC
+  const wchar_t* c_str() const { return &buffer_[0]; }
+  std::wstring str() const { return {&buffer_[0], size()}; }
 };
 
-// Flags.
-enum {SIGN_FLAG = 1, PLUS_FLAG = 2, MINUS_FLAG = 4, HASH_FLAG = 8};
+template <typename T = void> struct null {};
 
-enum format_spec_tag {fill_tag, align_tag, width_tag, type_tag};
-
-// Format specifier.
-template <typename T, format_spec_tag>
-class format_spec {
+// Workaround an array initialization issue in gcc 4.8.
+template <typename Char> struct fill_t {
  private:
-  T value_;
-
- public:
-  typedef T value_type;
-
-  explicit format_spec(T value) : value_(value) {}
-
-  T value() const { return value_; }
-};
+  enum { max_size = 4 };
+  Char data_[max_size];
+  unsigned char size_;
 
-// template <typename Char>
-// typedef format_spec<Char, fill_tag> fill_spec;
-template <typename Char>
-class fill_spec : public format_spec<Char, fill_tag> {
  public:
-  explicit fill_spec(Char value) : format_spec<Char, fill_tag>(value) {}
-};
-
-typedef format_spec<unsigned, width_tag> width_spec;
-typedef format_spec<char, type_tag> type_spec;
-
-// An empty format specifier.
-struct empty_spec {};
-
-// An alignment specifier.
-struct align_spec : empty_spec {
-  unsigned width_;
-  // Fill is always wchar_t and cast to char if necessary to avoid having
-  // two specialization of AlignSpec and its subclasses.
-  wchar_t fill_;
-  alignment align_;
-
-  FMT_CONSTEXPR align_spec(
-      unsigned width, wchar_t fill, alignment align = ALIGN_DEFAULT)
-  : width_(width), fill_(fill), align_(align) {}
+  FMT_CONSTEXPR void operator=(basic_string_view<Char> s) {
+    auto size = s.size();
+    if (size > max_size) {
+      FMT_THROW(format_error("invalid fill"));
+      return;
+    }
+    for (size_t i = 0; i < size; ++i) data_[i] = s[i];
+    size_ = static_cast<unsigned char>(size);
+  }
 
-  FMT_CONSTEXPR unsigned width() const { return width_; }
-  FMT_CONSTEXPR wchar_t fill() const { return fill_; }
-  FMT_CONSTEXPR alignment align() const { return align_; }
+  size_t size() const { return size_; }
+  const Char* data() const { return data_; }
 
-  int precision() const { return -1; }
+  FMT_CONSTEXPR Char& operator[](size_t index) { return data_[index]; }
+  FMT_CONSTEXPR const Char& operator[](size_t index) const {
+    return data_[index];
+  }
+
+  static FMT_CONSTEXPR fill_t<Char> make() {
+    auto fill = fill_t<Char>();
+    fill[0] = Char(' ');
+    fill.size_ = 1;
+    return fill;
+  }
+};
+}  // namespace detail
+
+// We cannot use enum classes as bit fields because of a gcc bug
+// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=61414.
+namespace align {
+enum type { none, left, right, center, numeric };
+}
+using align_t = align::type;
+
+namespace sign {
+enum type { none, minus, plus, space };
+}
+using sign_t = sign::type;
+
+// Format specifiers for built-in and string types.
+template <typename Char> struct basic_format_specs {
+  int width;
+  int precision;
+  char type;
+  align_t align : 4;
+  sign_t sign : 3;
+  bool alt : 1;  // Alternate form ('#').
+  detail::fill_t<Char> fill;
+
+  constexpr basic_format_specs()
+      : width(0),
+        precision(-1),
+        type(0),
+        align(align::none),
+        sign(sign::none),
+        alt(false),
+        fill(detail::fill_t<Char>::make()) {}
+};
+
+using format_specs = basic_format_specs<char>;
+
+namespace detail {
+namespace dragonbox {
+
+// Type-specific information that Dragonbox uses.
+template <class T> struct float_info;
+
+template <> struct float_info<float> {
+  using carrier_uint = uint32_t;
+  static const int significand_bits = 23;
+  static const int exponent_bits = 8;
+  static const int min_exponent = -126;
+  static const int max_exponent = 127;
+  static const int exponent_bias = -127;
+  static const int decimal_digits = 9;
+  static const int kappa = 1;
+  static const int big_divisor = 100;
+  static const int small_divisor = 10;
+  static const int min_k = -31;
+  static const int max_k = 46;
+  static const int cache_bits = 64;
+  static const int divisibility_check_by_5_threshold = 39;
+  static const int case_fc_pm_half_lower_threshold = -1;
+  static const int case_fc_pm_half_upper_threshold = 6;
+  static const int case_fc_lower_threshold = -2;
+  static const int case_fc_upper_threshold = 6;
+  static const int case_shorter_interval_left_endpoint_lower_threshold = 2;
+  static const int case_shorter_interval_left_endpoint_upper_threshold = 3;
+  static const int shorter_interval_tie_lower_threshold = -35;
+  static const int shorter_interval_tie_upper_threshold = -35;
+  static const int max_trailing_zeros = 7;
+};
+
+template <> struct float_info<double> {
+  using carrier_uint = uint64_t;
+  static const int significand_bits = 52;
+  static const int exponent_bits = 11;
+  static const int min_exponent = -1022;
+  static const int max_exponent = 1023;
+  static const int exponent_bias = -1023;
+  static const int decimal_digits = 17;
+  static const int kappa = 2;
+  static const int big_divisor = 1000;
+  static const int small_divisor = 100;
+  static const int min_k = -292;
+  static const int max_k = 326;
+  static const int cache_bits = 128;
+  static const int divisibility_check_by_5_threshold = 86;
+  static const int case_fc_pm_half_lower_threshold = -2;
+  static const int case_fc_pm_half_upper_threshold = 9;
+  static const int case_fc_lower_threshold = -4;
+  static const int case_fc_upper_threshold = 9;
+  static const int case_shorter_interval_left_endpoint_lower_threshold = 2;
+  static const int case_shorter_interval_left_endpoint_upper_threshold = 3;
+  static const int shorter_interval_tie_lower_threshold = -77;
+  static const int shorter_interval_tie_upper_threshold = -77;
+  static const int max_trailing_zeros = 16;
+};
+
+template <typename T> struct decimal_fp {
+  using significand_type = typename float_info<T>::carrier_uint;
+  significand_type significand;
+  int exponent;
 };
 
-// Format specifiers.
-template <typename Char>
-class basic_format_specs : public align_spec {
- public:
-  unsigned flags_;
-  int precision_;
-  Char type_;
-
-  FMT_CONSTEXPR basic_format_specs(
-      unsigned width = 0, char type = 0, wchar_t fill = ' ')
-  : align_spec(width, fill), flags_(0), precision_(-1), type_(type) {}
+template <typename T> decimal_fp<T> to_decimal(T x) FMT_NOEXCEPT;
+}  // namespace dragonbox
 
-  FMT_CONSTEXPR bool flag(unsigned f) const { return (flags_ & f) != 0; }
-  FMT_CONSTEXPR int precision() const { return precision_; }
-  FMT_CONSTEXPR Char type() const { return type_; }
-};
+template <typename T>
+constexpr typename dragonbox::float_info<T>::carrier_uint exponent_mask() {
+  using uint = typename dragonbox::float_info<T>::carrier_uint;
+  return ((uint(1) << dragonbox::float_info<T>::exponent_bits) - 1)
+         << dragonbox::float_info<T>::significand_bits;
+}
+
+// A floating-point presentation format.
+enum class float_format : unsigned char {
+  general,  // General: exponent notation or fixed point based on magnitude.
+  exp,      // Exponent notation with the default precision of 6, e.g. 1.2e-3.
+  fixed,    // Fixed point with the default precision of 6, e.g. 0.0012.
+  hex
+};
+
+struct float_specs {
+  int precision;
+  float_format format : 8;
+  sign_t sign : 8;
+  bool upper : 1;
+  bool locale : 1;
+  bool binary32 : 1;
+  bool use_grisu : 1;
+  bool showpoint : 1;
+};
+
+// Writes the exponent exp in the form "[+-]d{2,3}" to buffer.
+template <typename Char, typename It> It write_exponent(int exp, It it) {
+  FMT_ASSERT(-10000 < exp && exp < 10000, "exponent out of range");
+  if (exp < 0) {
+    *it++ = static_cast<Char>('-');
+    exp = -exp;
+  } else {
+    *it++ = static_cast<Char>('+');
+  }
+  if (exp >= 100) {
+    const char* top = data::digits[exp / 100];
+    if (exp >= 1000) *it++ = static_cast<Char>(top[0]);
+    *it++ = static_cast<Char>(top[1]);
+    exp %= 100;
+  }
+  const char* d = data::digits[exp];
+  *it++ = static_cast<Char>(d[0]);
+  *it++ = static_cast<Char>(d[1]);
+  return it;
+}
 
-typedef basic_format_specs<char> format_specs;
+template <typename T>
+int format_float(T value, int precision, float_specs specs, buffer<char>& buf);
 
-template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR unsigned basic_parse_context<Char, ErrorHandler>::next_arg_id() {
-  if (next_arg_id_ >= 0)
-    return internal::to_unsigned(next_arg_id_++);
-  on_error("cannot switch from manual to automatic argument indexing");
-  return 0;
-}
+// Formats a floating-point number with snprintf.
+template <typename T>
+int snprintf_float(T value, int precision, float_specs specs,
+                   buffer<char>& buf);
 
-namespace internal {
-
-template <typename S>
-struct format_string_traits<
-  S, typename std::enable_if<std::is_base_of<compile_string, S>::value>::type>:
-    format_string_traits_base<char> {};
+template <typename T> T promote_float(T value) { return value; }
+inline double promote_float(float value) { return static_cast<double>(value); }
 
-template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_int_type_spec(Char spec, Handler &&handler) {
+template <typename Handler>
+FMT_CONSTEXPR void handle_int_type_spec(char spec, Handler&& handler) {
   switch (spec) {
-  case 0: case 'd':
+  case 0:
+  case 'd':
     handler.on_dec();
     break;
-  case 'x': case 'X':
+  case 'x':
+  case 'X':
     handler.on_hex();
     break;
-  case 'b': case 'B':
+  case 'b':
+  case 'B':
     handler.on_bin();
     break;
   case 'o':
     handler.on_oct();
     break;
+#ifdef FMT_DEPRECATED_N_SPECIFIER
   case 'n':
+#endif
+  case 'L':
     handler.on_num();
     break;
+  case 'c':
+    handler.on_chr();
+    break;
   default:
     handler.on_error();
   }
 }
 
-template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_float_type_spec(Char spec, Handler &&handler) {
-  switch (spec) {
-  case 0: case 'g': case 'G':
-    handler.on_general();
+template <typename ErrorHandler = error_handler, typename Char>
+FMT_CONSTEXPR float_specs parse_float_type_spec(
+    const basic_format_specs<Char>& specs, ErrorHandler&& eh = {}) {
+  auto result = float_specs();
+  result.showpoint = specs.alt;
+  switch (specs.type) {
+  case 0:
+    result.format = float_format::general;
+    result.showpoint |= specs.precision > 0;
     break;
-  case 'e': case 'E':
-    handler.on_exp();
+  case 'G':
+    result.upper = true;
+    FMT_FALLTHROUGH;
+  case 'g':
+    result.format = float_format::general;
     break;
-  case 'f': case 'F':
-    handler.on_fixed();
+  case 'E':
+    result.upper = true;
+    FMT_FALLTHROUGH;
+  case 'e':
+    result.format = float_format::exp;
+    result.showpoint |= specs.precision != 0;
     break;
-   case 'a': case 'A':
-    handler.on_hex();
+  case 'F':
+    result.upper = true;
+    FMT_FALLTHROUGH;
+  case 'f':
+    result.format = float_format::fixed;
+    result.showpoint |= specs.precision != 0;
+    break;
+  case 'A':
+    result.upper = true;
+    FMT_FALLTHROUGH;
+  case 'a':
+    result.format = float_format::hex;
+    break;
+#ifdef FMT_DEPRECATED_N_SPECIFIER
+  case 'n':
+#endif
+  case 'L':
+    result.locale = true;
     break;
   default:
-    handler.on_error();
+    eh.on_error("invalid type specifier");
     break;
   }
+  return result;
 }
 
 template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_char_specs(
-    const basic_format_specs<Char> *specs, Handler &&handler) {
+FMT_CONSTEXPR void handle_char_specs(const basic_format_specs<Char>* specs,
+                                     Handler&& handler) {
   if (!specs) return handler.on_char();
-  if (specs->type() && specs->type() != 'c') return handler.on_int();
-  if (specs->align() == ALIGN_NUMERIC || specs->flag(~0u) != 0)
+  if (specs->type && specs->type != 'c') return handler.on_int();
+  if (specs->align == align::numeric || specs->sign != sign::none || specs->alt)
     handler.on_error("invalid format specifier for char");
   handler.on_char();
 }
 
 template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_cstring_type_spec(Char spec, Handler &&handler) {
+FMT_CONSTEXPR void handle_cstring_type_spec(Char spec, Handler&& handler) {
   if (spec == 0 || spec == 's')
     handler.on_string();
   else if (spec == 'p')
     handler.on_pointer();
   else
     handler.on_error("invalid type specifier");
 }
 
 template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR void check_string_type_spec(Char spec, ErrorHandler &&eh) {
-  if (spec != 0 && spec != 's')
-    eh.on_error("invalid type specifier");
+FMT_CONSTEXPR void check_string_type_spec(Char spec, ErrorHandler&& eh) {
+  if (spec != 0 && spec != 's') eh.on_error("invalid type specifier");
 }
 
 template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR void check_pointer_type_spec(Char spec, ErrorHandler &&eh) {
-  if (spec != 0 && spec != 'p')
-    eh.on_error("invalid type specifier");
+FMT_CONSTEXPR void check_pointer_type_spec(Char spec, ErrorHandler&& eh) {
+  if (spec != 0 && spec != 'p') eh.on_error("invalid type specifier");
 }
 
-template <typename ErrorHandler>
-class int_type_checker : private ErrorHandler {
+template <typename ErrorHandler> class int_type_checker : private ErrorHandler {
  public:
   FMT_CONSTEXPR explicit int_type_checker(ErrorHandler eh) : ErrorHandler(eh) {}
 
   FMT_CONSTEXPR void on_dec() {}
   FMT_CONSTEXPR void on_hex() {}
   FMT_CONSTEXPR void on_bin() {}
   FMT_CONSTEXPR void on_oct() {}
   FMT_CONSTEXPR void on_num() {}
+  FMT_CONSTEXPR void on_chr() {}
 
   FMT_CONSTEXPR void on_error() {
     ErrorHandler::on_error("invalid type specifier");
   }
 };
 
 template <typename ErrorHandler>
-class float_type_checker : private ErrorHandler {
- public:
-  FMT_CONSTEXPR explicit float_type_checker(ErrorHandler eh)
-    : ErrorHandler(eh) {}
-
-  FMT_CONSTEXPR void on_general() {}
-  FMT_CONSTEXPR void on_exp() {}
-  FMT_CONSTEXPR void on_fixed() {}
-  FMT_CONSTEXPR void on_hex() {}
-
-  FMT_CONSTEXPR void on_error() {
-    ErrorHandler::on_error("invalid type specifier");
-  }
-};
-
-template <typename ErrorHandler, typename CharType>
 class char_specs_checker : public ErrorHandler {
  private:
-  CharType type_;
+  char type_;
 
  public:
-  FMT_CONSTEXPR char_specs_checker(CharType type, ErrorHandler eh)
-    : ErrorHandler(eh), type_(type) {}
+  FMT_CONSTEXPR char_specs_checker(char type, ErrorHandler eh)
+      : ErrorHandler(eh), type_(type) {}
 
   FMT_CONSTEXPR void on_int() {
     handle_int_type_spec(type_, int_type_checker<ErrorHandler>(*this));
   }
   FMT_CONSTEXPR void on_char() {}
 };
 
 template <typename ErrorHandler>
 class cstring_type_checker : public ErrorHandler {
  public:
   FMT_CONSTEXPR explicit cstring_type_checker(ErrorHandler eh)
-    : ErrorHandler(eh) {}
+      : ErrorHandler(eh) {}
 
   FMT_CONSTEXPR void on_string() {}
   FMT_CONSTEXPR void on_pointer() {}
 };
 
-template <typename Context>
-void arg_map<Context>::init(const basic_format_args<Context> &args) {
-  if (map_)
-    return;
-  map_ = new entry[args.max_size()];
-  bool use_values = args.type(max_packed_args - 1) == internal::none_type;
-  if (use_values) {
-    for (unsigned i = 0;/*nothing*/; ++i) {
-      internal::type arg_type = args.type(i);
-      switch (arg_type) {
-        case internal::none_type:
-          return;
-        case internal::named_arg_type:
-          push_back(args.values_[i]);
-          break;
-        default:
-          break; // Do nothing.
+template <typename OutputIt, typename Char>
+FMT_NOINLINE OutputIt fill(OutputIt it, size_t n, const fill_t<Char>& fill) {
+  auto fill_size = fill.size();
+  if (fill_size == 1) return std::fill_n(it, n, fill[0]);
+  for (size_t i = 0; i < n; ++i) it = std::copy_n(fill.data(), fill_size, it);
+  return it;
+}
+
+// Writes the output of f, padded according to format specifications in specs.
+// size: output size in code units.
+// width: output display width in (terminal) column positions.
+template <align::type align = align::left, typename OutputIt, typename Char,
+          typename F>
+inline OutputIt write_padded(OutputIt out,
+                             const basic_format_specs<Char>& specs, size_t size,
+                             size_t width, F&& f) {
+  static_assert(align == align::left || align == align::right, "");
+  unsigned spec_width = to_unsigned(specs.width);
+  size_t padding = spec_width > width ? spec_width - width : 0;
+  auto* shifts = align == align::left ? data::left_padding_shifts
+                                      : data::right_padding_shifts;
+  size_t left_padding = padding >> shifts[specs.align];
+  auto it = reserve(out, size + padding * specs.fill.size());
+  it = fill(it, left_padding, specs.fill);
+  it = f(it);
+  it = fill(it, padding - left_padding, specs.fill);
+  return base_iterator(out, it);
+}
+
+template <align::type align = align::left, typename OutputIt, typename Char,
+          typename F>
+inline OutputIt write_padded(OutputIt out,
+                             const basic_format_specs<Char>& specs, size_t size,
+                             F&& f) {
+  return write_padded<align>(out, specs, size, size, f);
+}
+
+template <typename Char, typename OutputIt>
+OutputIt write_bytes(OutputIt out, string_view bytes,
+                     const basic_format_specs<Char>& specs) {
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  return write_padded(out, specs, bytes.size(), [bytes](iterator it) {
+    const char* data = bytes.data();
+    return copy_str<Char>(data, data + bytes.size(), it);
+  });
+}
+
+// Data for write_int that doesn't depend on output iterator type. It is used to
+// avoid template code bloat.
+template <typename Char> struct write_int_data {
+  size_t size;
+  size_t padding;
+
+  write_int_data(int num_digits, string_view prefix,
+                 const basic_format_specs<Char>& specs)
+      : size(prefix.size() + to_unsigned(num_digits)), padding(0) {
+    if (specs.align == align::numeric) {
+      auto width = to_unsigned(specs.width);
+      if (width > size) {
+        padding = width - size;
+        size = width;
       }
+    } else if (specs.precision > num_digits) {
+      size = prefix.size() + to_unsigned(specs.precision);
+      padding = to_unsigned(specs.precision - num_digits);
+    }
+  }
+};
+
+// Writes an integer in the format
+//   <left-padding><prefix><numeric-padding><digits><right-padding>
+// where <digits> are written by f(it).
+template <typename OutputIt, typename Char, typename F>
+OutputIt write_int(OutputIt out, int num_digits, string_view prefix,
+                   const basic_format_specs<Char>& specs, F f) {
+  auto data = write_int_data<Char>(num_digits, prefix, specs);
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  return write_padded<align::right>(out, specs, data.size, [=](iterator it) {
+    if (prefix.size() != 0)
+      it = copy_str<Char>(prefix.begin(), prefix.end(), it);
+    it = std::fill_n(it, data.padding, static_cast<Char>('0'));
+    return f(it);
+  });
+}
+
+template <typename StrChar, typename Char, typename OutputIt>
+OutputIt write(OutputIt out, basic_string_view<StrChar> s,
+               const basic_format_specs<Char>& specs) {
+  auto data = s.data();
+  auto size = s.size();
+  if (specs.precision >= 0 && to_unsigned(specs.precision) < size)
+    size = code_point_index(s, to_unsigned(specs.precision));
+  auto width = specs.width != 0
+                   ? count_code_points(basic_string_view<StrChar>(data, size))
+                   : 0;
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  return write_padded(out, specs, size, width, [=](iterator it) {
+    return copy_str<Char>(data, data + size, it);
+  });
+}
+
+// The handle_int_type_spec handler that writes an integer.
+template <typename OutputIt, typename Char, typename UInt> struct int_writer {
+  OutputIt out;
+  locale_ref locale;
+  const basic_format_specs<Char>& specs;
+  UInt abs_value;
+  char prefix[4];
+  unsigned prefix_size;
+
+  using iterator =
+      remove_reference_t<decltype(reserve(std::declval<OutputIt&>(), 0))>;
+
+  string_view get_prefix() const { return string_view(prefix, prefix_size); }
+
+  template <typename Int>
+  int_writer(OutputIt output, locale_ref loc, Int value,
+             const basic_format_specs<Char>& s)
+      : out(output),
+        locale(loc),
+        specs(s),
+        abs_value(static_cast<UInt>(value)),
+        prefix_size(0) {
+    static_assert(std::is_same<uint32_or_64_or_128_t<Int>, UInt>::value, "");
+    if (is_negative(value)) {
+      prefix[0] = '-';
+      ++prefix_size;
+      abs_value = 0 - abs_value;
+    } else if (specs.sign != sign::none && specs.sign != sign::minus) {
+      prefix[0] = specs.sign == sign::plus ? '+' : ' ';
+      ++prefix_size;
     }
   }
-  for (unsigned i = 0; ; ++i) {
-    switch (args.args_[i].type_) {
-      case internal::none_type:
-        return;
-      case internal::named_arg_type:
-        push_back(args.args_[i].value_);
-        break;
-      default:
-        break; // Do nothing.
+
+  void on_dec() {
+    auto num_digits = count_digits(abs_value);
+    out = write_int(
+        out, num_digits, get_prefix(), specs, [this, num_digits](iterator it) {
+          return format_decimal<Char>(it, abs_value, num_digits).end;
+        });
+  }
+
+  void on_hex() {
+    if (specs.alt) {
+      prefix[prefix_size++] = '0';
+      prefix[prefix_size++] = specs.type;
+    }
+    int num_digits = count_digits<4>(abs_value);
+    out = write_int(out, num_digits, get_prefix(), specs,
+                    [this, num_digits](iterator it) {
+                      return format_uint<4, Char>(it, abs_value, num_digits,
+                                                  specs.type != 'x');
+                    });
+  }
+
+  void on_bin() {
+    if (specs.alt) {
+      prefix[prefix_size++] = '0';
+      prefix[prefix_size++] = static_cast<char>(specs.type);
+    }
+    int num_digits = count_digits<1>(abs_value);
+    out = write_int(out, num_digits, get_prefix(), specs,
+                    [this, num_digits](iterator it) {
+                      return format_uint<1, Char>(it, abs_value, num_digits);
+                    });
+  }
+
+  void on_oct() {
+    int num_digits = count_digits<3>(abs_value);
+    if (specs.alt && specs.precision <= num_digits && abs_value != 0) {
+      // Octal prefix '0' is counted as a digit, so only add it if precision
+      // is not greater than the number of digits.
+      prefix[prefix_size++] = '0';
+    }
+    out = write_int(out, num_digits, get_prefix(), specs,
+                    [this, num_digits](iterator it) {
+                      return format_uint<3, Char>(it, abs_value, num_digits);
+                    });
+  }
+
+  enum { sep_size = 1 };
+
+  void on_num() {
+    std::string groups = grouping<Char>(locale);
+    if (groups.empty()) return on_dec();
+    auto sep = thousands_sep<Char>(locale);
+    if (!sep) return on_dec();
+    int num_digits = count_digits(abs_value);
+    int size = num_digits, n = num_digits;
+    std::string::const_iterator group = groups.cbegin();
+    while (group != groups.cend() && n > *group && *group > 0 &&
+           *group != max_value<char>()) {
+      size += sep_size;
+      n -= *group;
+      ++group;
+    }
+    if (group == groups.cend()) size += sep_size * ((n - 1) / groups.back());
+    char digits[40];
+    format_decimal(digits, abs_value, num_digits);
+    basic_memory_buffer<Char> buffer;
+    size += static_cast<int>(prefix_size);
+    const auto usize = to_unsigned(size);
+    buffer.resize(usize);
+    basic_string_view<Char> s(&sep, sep_size);
+    // Index of a decimal digit with the least significant digit having index 0.
+    int digit_index = 0;
+    group = groups.cbegin();
+    auto p = buffer.data() + size - 1;
+    for (int i = num_digits - 1; i > 0; --i) {
+      *p-- = static_cast<Char>(digits[i]);
+      if (*group <= 0 || ++digit_index % *group != 0 ||
+          *group == max_value<char>())
+        continue;
+      if (group + 1 != groups.cend()) {
+        digit_index = 0;
+        ++group;
+      }
+      std::uninitialized_copy(s.data(), s.data() + s.size(),
+                              make_checked(p, s.size()));
+      p -= s.size();
     }
+    *p-- = static_cast<Char>(*digits);
+    if (prefix_size != 0) *p = static_cast<Char>('-');
+    auto data = buffer.data();
+    out = write_padded<align::right>(
+        out, specs, usize, usize,
+        [=](iterator it) { return copy_str<Char>(data, data + size, it); });
+  }
+
+  void on_chr() { *out++ = static_cast<Char>(abs_value); }
+
+  FMT_NORETURN void on_error() {
+    FMT_THROW(format_error("invalid type specifier"));
   }
+};
+
+template <typename Char, typename OutputIt>
+OutputIt write_nonfinite(OutputIt out, bool isinf,
+                         const basic_format_specs<Char>& specs,
+                         const float_specs& fspecs) {
+  auto str =
+      isinf ? (fspecs.upper ? "INF" : "inf") : (fspecs.upper ? "NAN" : "nan");
+  constexpr size_t str_size = 3;
+  auto sign = fspecs.sign;
+  auto size = str_size + (sign ? 1 : 0);
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  return write_padded(out, specs, size, [=](iterator it) {
+    if (sign) *it++ = static_cast<Char>(data::signs[sign]);
+    return copy_str<Char>(str, str + str_size, it);
+  });
+}
+
+// A decimal floating-point number significand * pow(10, exp).
+struct big_decimal_fp {
+  const char* significand;
+  int significand_size;
+  int exponent;
+};
+
+inline int get_significand_size(const big_decimal_fp& fp) {
+  return fp.significand_size;
+}
+template <typename T>
+inline int get_significand_size(const dragonbox::decimal_fp<T>& fp) {
+  return count_digits(fp.significand);
 }
 
-template <typename Range>
-class arg_formatter_base {
- public:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef basic_format_specs<char_type> format_specs;
+template <typename Char, typename OutputIt>
+inline OutputIt write_significand(OutputIt out, const char* significand,
+                                  int& significand_size) {
+  return copy_str<Char>(significand, significand + significand_size, out);
+}
+template <typename Char, typename OutputIt, typename UInt>
+inline OutputIt write_significand(OutputIt out, UInt significand,
+                                  int significand_size) {
+  return format_decimal<Char>(out, significand, significand_size).end;
+}
+
+template <typename Char, typename UInt,
+          FMT_ENABLE_IF(std::is_integral<UInt>::value)>
+inline Char* write_significand(Char* out, UInt significand,
+                               int significand_size, int integral_size,
+                               Char decimal_point) {
+  if (!decimal_point)
+    return format_decimal(out, significand, significand_size).end;
+  auto end = format_decimal(out + 1, significand, significand_size).end;
+  if (integral_size == 1)
+    out[0] = out[1];
+  else
+    std::copy_n(out + 1, integral_size, out);
+  out[integral_size] = decimal_point;
+  return end;
+}
 
- private:
-  typedef basic_writer<Range> writer_type;
-  writer_type writer_;
-  format_specs *specs_;
-
-  struct char_writer {
-    char_type value;
-    template <typename It>
-    void operator()(It &&it) const { *it++ = value; }
+template <typename OutputIt, typename UInt, typename Char,
+          FMT_ENABLE_IF(!std::is_pointer<remove_cvref_t<OutputIt>>::value)>
+inline OutputIt write_significand(OutputIt out, UInt significand,
+                                  int significand_size, int integral_size,
+                                  Char decimal_point) {
+  // Buffer is large enough to hold digits (digits10 + 1) and a decimal point.
+  Char buffer[digits10<UInt>() + 2];
+  auto end = write_significand(buffer, significand, significand_size,
+                               integral_size, decimal_point);
+  return detail::copy_str<Char>(buffer, end, out);
+}
+
+template <typename OutputIt, typename Char>
+inline OutputIt write_significand(OutputIt out, const char* significand,
+                                  int significand_size, int integral_size,
+                                  Char decimal_point) {
+  out = detail::copy_str<Char>(significand, significand + integral_size, out);
+  if (!decimal_point) return out;
+  *out++ = decimal_point;
+  return detail::copy_str<Char>(significand + integral_size,
+                                significand + significand_size, out);
+}
+
+template <typename OutputIt, typename DecimalFP, typename Char>
+OutputIt write_float(OutputIt out, const DecimalFP& fp,
+                     const basic_format_specs<Char>& specs, float_specs fspecs,
+                     Char decimal_point) {
+  auto significand = fp.significand;
+  int significand_size = get_significand_size(fp);
+  static const Char zero = static_cast<Char>('0');
+  auto sign = fspecs.sign;
+  size_t size = to_unsigned(significand_size) + (sign ? 1 : 0);
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+
+  int output_exp = fp.exponent + significand_size - 1;
+  auto use_exp_format = [=]() {
+    if (fspecs.format == float_format::exp) return true;
+    if (fspecs.format != float_format::general) return false;
+    // Use the fixed notation if the exponent is in [exp_lower, exp_upper),
+    // e.g. 0.0001 instead of 1e-04. Otherwise use the exponent notation.
+    const int exp_lower = -4, exp_upper = 16;
+    return output_exp < exp_lower ||
+           output_exp >= (fspecs.precision > 0 ? fspecs.precision : exp_upper);
   };
+  if (use_exp_format()) {
+    int num_zeros = 0;
+    if (fspecs.showpoint) {
+      num_zeros = (std::max)(fspecs.precision - significand_size, 0);
+      size += to_unsigned(num_zeros);
+    } else if (significand_size == 1) {
+      decimal_point = Char();
+    }
+    auto abs_output_exp = output_exp >= 0 ? output_exp : -output_exp;
+    int exp_digits = 2;
+    if (abs_output_exp >= 100) exp_digits = abs_output_exp >= 1000 ? 4 : 3;
+
+    size += to_unsigned((decimal_point ? 1 : 0) + 2 + exp_digits);
+    char exp_char = fspecs.upper ? 'E' : 'e';
+    auto write = [=](iterator it) {
+      if (sign) *it++ = static_cast<Char>(data::signs[sign]);
+      // Insert a decimal point after the first digit and add an exponent.
+      it = write_significand(it, significand, significand_size, 1,
+                             decimal_point);
+      if (num_zeros > 0) it = std::fill_n(it, num_zeros, zero);
+      *it++ = static_cast<Char>(exp_char);
+      return write_exponent<Char>(output_exp, it);
+    };
+    return specs.width > 0 ? write_padded<align::right>(out, specs, size, write)
+                           : base_iterator(out, write(reserve(out, size)));
+  }
 
-  void write_char(char_type value) {
-    if (specs_)
-      writer_.write_padded(1, *specs_, char_writer{value});
+  int exp = fp.exponent + significand_size;
+  if (fp.exponent >= 0) {
+    // 1234e5 -> 123400000[.0+]
+    size += to_unsigned(fp.exponent);
+    int num_zeros = fspecs.precision - exp;
+#ifdef FMT_FUZZ
+    if (num_zeros > 5000)
+      throw std::runtime_error("fuzz mode - avoiding excessive cpu use");
+#endif
+    if (fspecs.showpoint) {
+      if (num_zeros <= 0 && fspecs.format != float_format::fixed) num_zeros = 1;
+      if (num_zeros > 0) size += to_unsigned(num_zeros);
+    }
+    return write_padded<align::right>(out, specs, size, [&](iterator it) {
+      if (sign) *it++ = static_cast<Char>(data::signs[sign]);
+      it = write_significand<Char>(it, significand, significand_size);
+      it = std::fill_n(it, fp.exponent, zero);
+      if (!fspecs.showpoint) return it;
+      *it++ = decimal_point;
+      return num_zeros > 0 ? std::fill_n(it, num_zeros, zero) : it;
+    });
+  } else if (exp > 0) {
+    // 1234e-2 -> 12.34[0+]
+    int num_zeros = fspecs.showpoint ? fspecs.precision - significand_size : 0;
+    size += 1 + to_unsigned(num_zeros > 0 ? num_zeros : 0);
+    return write_padded<align::right>(out, specs, size, [&](iterator it) {
+      if (sign) *it++ = static_cast<Char>(data::signs[sign]);
+      it = write_significand(it, significand, significand_size, exp,
+                             decimal_point);
+      return num_zeros > 0 ? std::fill_n(it, num_zeros, zero) : it;
+    });
+  }
+  // 1234e-6 -> 0.001234
+  int num_zeros = -exp;
+  if (significand_size == 0 && fspecs.precision >= 0 &&
+      fspecs.precision < num_zeros) {
+    num_zeros = fspecs.precision;
+  }
+  size += 2 + to_unsigned(num_zeros);
+  return write_padded<align::right>(out, specs, size, [&](iterator it) {
+    if (sign) *it++ = static_cast<Char>(data::signs[sign]);
+    *it++ = zero;
+    if (num_zeros == 0 && significand_size == 0 && !fspecs.showpoint) return it;
+    *it++ = decimal_point;
+    it = std::fill_n(it, num_zeros, zero);
+    return write_significand<Char>(it, significand, significand_size);
+  });
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+OutputIt write(OutputIt out, T value, basic_format_specs<Char> specs,
+               locale_ref loc = {}) {
+  if (const_check(!is_supported_floating_point(value))) return out;
+  float_specs fspecs = parse_float_type_spec(specs);
+  fspecs.sign = specs.sign;
+  if (std::signbit(value)) {  // value < 0 is false for NaN so use signbit.
+    fspecs.sign = sign::minus;
+    value = -value;
+  } else if (fspecs.sign == sign::minus) {
+    fspecs.sign = sign::none;
+  }
+
+  if (!std::isfinite(value))
+    return write_nonfinite(out, std::isinf(value), specs, fspecs);
+
+  if (specs.align == align::numeric && fspecs.sign) {
+    auto it = reserve(out, 1);
+    *it++ = static_cast<Char>(data::signs[fspecs.sign]);
+    out = base_iterator(out, it);
+    fspecs.sign = sign::none;
+    if (specs.width != 0) --specs.width;
+  }
+
+  memory_buffer buffer;
+  if (fspecs.format == float_format::hex) {
+    if (fspecs.sign) buffer.push_back(data::signs[fspecs.sign]);
+    snprintf_float(promote_float(value), specs.precision, fspecs, buffer);
+    return write_bytes(out, {buffer.data(), buffer.size()}, specs);
+  }
+  int precision = specs.precision >= 0 || !specs.type ? specs.precision : 6;
+  if (fspecs.format == float_format::exp) {
+    if (precision == max_value<int>())
+      FMT_THROW(format_error("number is too big"));
     else
-      writer_.write(value);
+      ++precision;
+  }
+  if (const_check(std::is_same<T, float>())) fspecs.binary32 = true;
+  fspecs.use_grisu = is_fast_float<T>();
+  int exp = format_float(promote_float(value), precision, fspecs, buffer);
+  fspecs.precision = precision;
+  Char point =
+      fspecs.locale ? decimal_point<Char>(loc) : static_cast<Char>('.');
+  auto fp = big_decimal_fp{buffer.data(), static_cast<int>(buffer.size()), exp};
+  return write_float(out, fp, specs, fspecs, point);
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_fast_float<T>::value)>
+OutputIt write(OutputIt out, T value) {
+  if (const_check(!is_supported_floating_point(value))) return out;
+
+  using floaty = conditional_t<std::is_same<T, long double>::value, double, T>;
+  using uint = typename dragonbox::float_info<floaty>::carrier_uint;
+  auto bits = bit_cast<uint>(value);
+
+  auto fspecs = float_specs();
+  auto sign_bit = bits & (uint(1) << (num_bits<uint>() - 1));
+  if (sign_bit != 0) {
+    fspecs.sign = sign::minus;
+    value = -value;
+  }
+
+  static const auto specs = basic_format_specs<Char>();
+  uint mask = exponent_mask<floaty>();
+  if ((bits & mask) == mask)
+    return write_nonfinite(out, std::isinf(value), specs, fspecs);
+
+  auto dec = dragonbox::to_decimal(static_cast<floaty>(value));
+  return write_float(out, dec, specs, fspecs, static_cast<Char>('.'));
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_floating_point<T>::value &&
+                        !is_fast_float<T>::value)>
+inline OutputIt write(OutputIt out, T value) {
+  return write(out, value, basic_format_specs<Char>());
+}
+
+template <typename Char, typename OutputIt>
+OutputIt write_char(OutputIt out, Char value,
+                    const basic_format_specs<Char>& specs) {
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  return write_padded(out, specs, 1, [=](iterator it) {
+    *it++ = value;
+    return it;
+  });
+}
+
+template <typename Char, typename OutputIt, typename UIntPtr>
+OutputIt write_ptr(OutputIt out, UIntPtr value,
+                   const basic_format_specs<Char>* specs) {
+  int num_digits = count_digits<4>(value);
+  auto size = to_unsigned(num_digits) + size_t(2);
+  using iterator = remove_reference_t<decltype(reserve(out, 0))>;
+  auto write = [=](iterator it) {
+    *it++ = static_cast<Char>('0');
+    *it++ = static_cast<Char>('x');
+    return format_uint<4, Char>(it, value, num_digits);
+  };
+  return specs ? write_padded<align::right>(out, *specs, size, write)
+               : base_iterator(out, write(reserve(out, size)));
+}
+
+template <typename T> struct is_integral : std::is_integral<T> {};
+template <> struct is_integral<int128_t> : std::true_type {};
+template <> struct is_integral<uint128_t> : std::true_type {};
+
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, monostate) {
+  FMT_ASSERT(false, "");
+  return out;
+}
+
+template <typename Char, typename OutputIt,
+          FMT_ENABLE_IF(!std::is_same<Char, char>::value)>
+OutputIt write(OutputIt out, string_view value) {
+  auto it = reserve(out, value.size());
+  it = copy_str<Char>(value.begin(), value.end(), it);
+  return base_iterator(out, it);
+}
+
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, basic_string_view<Char> value) {
+  auto it = reserve(out, value.size());
+  it = std::copy(value.begin(), value.end(), it);
+  return base_iterator(out, it);
+}
+
+template <typename Char>
+buffer_appender<Char> write(buffer_appender<Char> out,
+                            basic_string_view<Char> value) {
+  get_container(out).append(value.begin(), value.end());
+  return out;
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_integral<T>::value &&
+                        !std::is_same<T, bool>::value &&
+                        !std::is_same<T, Char>::value)>
+OutputIt write(OutputIt out, T value) {
+  auto abs_value = static_cast<uint32_or_64_or_128_t<T>>(value);
+  bool negative = is_negative(value);
+  // Don't do -abs_value since it trips unsigned-integer-overflow sanitizer.
+  if (negative) abs_value = ~abs_value + 1;
+  int num_digits = count_digits(abs_value);
+  auto size = (negative ? 1 : 0) + static_cast<size_t>(num_digits);
+  auto it = reserve(out, size);
+  if (auto ptr = to_pointer<Char>(it, size)) {
+    if (negative) *ptr++ = static_cast<Char>('-');
+    format_decimal<Char>(ptr, abs_value, num_digits);
+    return out;
   }
+  if (negative) *it++ = static_cast<Char>('-');
+  it = format_decimal<Char>(it, abs_value, num_digits).end;
+  return base_iterator(out, it);
+}
+
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, bool value) {
+  return write<Char>(out, string_view(value ? "true" : "false"));
+}
+
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, Char value) {
+  auto it = reserve(out, 1);
+  *it++ = value;
+  return base_iterator(out, it);
+}
 
-  void write_pointer(const void *p) {
-    format_specs specs = specs_ ? *specs_ : format_specs();
-    specs.flags_ = HASH_FLAG;
-    specs.type_ = 'x';
-    writer_.write_int(reinterpret_cast<uintptr_t>(p), specs);
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, const Char* value) {
+  if (!value) {
+    FMT_THROW(format_error("string pointer is null"));
+  } else {
+    auto length = std::char_traits<Char>::length(value);
+    out = write(out, basic_string_view<Char>(value, length));
   }
+  return out;
+}
 
- protected:
-  writer_type &writer() { return writer_; }
-  format_specs *spec() { return specs_; }
-  iterator out() { return writer_.out(); }
+template <typename Char, typename OutputIt>
+OutputIt write(OutputIt out, const void* value) {
+  return write_ptr<Char>(out, to_uintptr(value), nullptr);
+}
+
+template <typename Char, typename OutputIt, typename T>
+auto write(OutputIt out, const T& value) -> typename std::enable_if<
+    mapped_type_constant<T, basic_format_context<OutputIt, Char>>::value ==
+        type::custom_type,
+    OutputIt>::type {
+  using context_type = basic_format_context<OutputIt, Char>;
+  using formatter_type =
+      conditional_t<has_formatter<T, context_type>::value,
+                    typename context_type::template formatter_type<T>,
+                    fallback_formatter<T, Char>>;
+  context_type ctx(out, {}, {});
+  return formatter_type().format(value, ctx);
+}
+
+// An argument visitor that formats the argument and writes it via the output
+// iterator. It's a class and not a generic lambda for compatibility with C++11.
+template <typename OutputIt, typename Char> struct default_arg_formatter {
+  using context = basic_format_context<OutputIt, Char>;
 
-  void write(bool value) {
-    string_view sv(value ? "true" : "false");
-    specs_ ? writer_.write_str(sv, *specs_) : writer_.write(sv);
+  OutputIt out;
+  basic_format_args<context> args;
+  locale_ref loc;
+
+  template <typename T> OutputIt operator()(T value) {
+    return write<Char>(out, value);
   }
 
-  void write(const char_type *value) {
-    if (!value)
-      FMT_THROW(format_error("string pointer is null"));
-    auto length = std::char_traits<char_type>::length(value);
-    basic_string_view<char_type> sv(value, length);
-    specs_ ? writer_.write_str(sv, *specs_) : writer_.write(sv);
+  OutputIt operator()(typename basic_format_arg<context>::handle handle) {
+    basic_format_parse_context<Char> parse_ctx({});
+    basic_format_context<OutputIt, Char> format_ctx(out, args, loc);
+    handle.format(parse_ctx, format_ctx);
+    return format_ctx.out();
   }
+};
 
+template <typename OutputIt, typename Char,
+          typename ErrorHandler = error_handler>
+class arg_formatter_base {
  public:
-  arg_formatter_base(Range r, format_specs *s): writer_(r), specs_(s) {}
+  using iterator = OutputIt;
+  using char_type = Char;
+  using format_specs = basic_format_specs<Char>;
 
-  iterator operator()(monostate) {
-    FMT_ASSERT(false, "invalid argument type");
-    return out();
+ private:
+  iterator out_;
+  locale_ref locale_;
+  format_specs* specs_;
+
+  // Attempts to reserve space for n extra characters in the output range.
+  // Returns a pointer to the reserved range or a reference to out_.
+  auto reserve(size_t n) -> decltype(detail::reserve(out_, n)) {
+    return detail::reserve(out_, n);
   }
 
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, iterator>::type
-      operator()(T value) {
-    // MSVC2013 fails to compile separate overloads for bool and char_type so
-    // use std::is_same instead.
-    if (std::is_same<T, bool>::value) {
-      if (specs_ && specs_->type_)
-        return (*this)(value ? 1 : 0);
-      write(value != 0);
-    } else if (std::is_same<T, char_type>::value) {
-      internal::handle_char_specs(
-        specs_, char_spec_handler(*this, static_cast<char_type>(value)));
-    } else {
-      specs_ ? writer_.write_int(value, *specs_) : writer_.write(value);
-    }
-    return out();
+  using reserve_iterator = remove_reference_t<decltype(
+      detail::reserve(std::declval<iterator&>(), 0))>;
+
+  template <typename T> void write_int(T value, const format_specs& spec) {
+    using uint_type = uint32_or_64_or_128_t<T>;
+    int_writer<iterator, Char, uint_type> w(out_, locale_, value, spec);
+    handle_int_type_spec(spec.type, w);
+    out_ = w.out;
   }
 
-  template <typename T>
-  typename std::enable_if<std::is_floating_point<T>::value, iterator>::type
-      operator()(T value) {
-    writer_.write_double(value, specs_ ? *specs_ : format_specs());
-    return out();
+  void write(char value) {
+    auto&& it = reserve(1);
+    *it++ = value;
+  }
+
+  template <typename Ch, FMT_ENABLE_IF(std::is_same<Ch, Char>::value)>
+  void write(Ch value) {
+    out_ = detail::write<Char>(out_, value);
+  }
+
+  void write(string_view value) {
+    auto&& it = reserve(value.size());
+    it = copy_str<Char>(value.begin(), value.end(), it);
+  }
+  void write(wstring_view value) {
+    static_assert(std::is_same<Char, wchar_t>::value, "");
+    auto&& it = reserve(value.size());
+    it = std::copy(value.begin(), value.end(), it);
   }
 
-  struct char_spec_handler : internal::error_handler {
-    arg_formatter_base &formatter;
-    char_type value;
+  template <typename Ch>
+  void write(const Ch* s, size_t size, const format_specs& specs) {
+    auto width = specs.width != 0
+                     ? count_code_points(basic_string_view<Ch>(s, size))
+                     : 0;
+    out_ = write_padded(out_, specs, size, width, [=](reserve_iterator it) {
+      return copy_str<Char>(s, s + size, it);
+    });
+  }
+
+  template <typename Ch>
+  void write(basic_string_view<Ch> s, const format_specs& specs = {}) {
+    out_ = detail::write(out_, s, specs);
+  }
+
+  void write_pointer(const void* p) {
+    out_ = write_ptr<char_type>(out_, to_uintptr(p), specs_);
+  }
 
-    char_spec_handler(arg_formatter_base& f, char_type val)
-      : formatter(f), value(val) {}
+  struct char_spec_handler : ErrorHandler {
+    arg_formatter_base& formatter;
+    Char value;
+
+    char_spec_handler(arg_formatter_base& f, Char val)
+        : formatter(f), value(val) {}
 
     void on_int() {
+      // char is only formatted as int if there are specs.
+      formatter.write_int(static_cast<int>(value), *formatter.specs_);
+    }
+    void on_char() {
       if (formatter.specs_)
-        formatter.writer_.write_int(value, *formatter.specs_);
+        formatter.out_ = write_char(formatter.out_, value, *formatter.specs_);
       else
-        formatter.writer_.write(value);
+        formatter.write(value);
     }
-    void on_char() { formatter.write_char(value); }
   };
 
-  struct cstring_spec_handler : internal::error_handler {
-    arg_formatter_base &formatter;
-    const char_type *value;
+  struct cstring_spec_handler : error_handler {
+    arg_formatter_base& formatter;
+    const Char* value;
 
-    cstring_spec_handler(arg_formatter_base &f, const char_type *val)
-      : formatter(f), value(val) {}
+    cstring_spec_handler(arg_formatter_base& f, const Char* val)
+        : formatter(f), value(val) {}
 
     void on_string() { formatter.write(value); }
     void on_pointer() { formatter.write_pointer(value); }
   };
 
-  iterator operator()(const char_type *value) {
-    if (!specs_) return write(value), out();
-    internal::handle_cstring_type_spec(
-          specs_->type_, cstring_spec_handler(*this, value));
-    return out();
+ protected:
+  iterator out() { return out_; }
+  format_specs* specs() { return specs_; }
+
+  void write(bool value) {
+    if (specs_)
+      write(string_view(value ? "true" : "false"), *specs_);
+    else
+      out_ = detail::write<Char>(out_, value);
   }
 
-  iterator operator()(basic_string_view<char_type> value) {
-    if (specs_) {
-      internal::check_string_type_spec(
-            specs_->type_, internal::error_handler());
-      writer_.write_str(value, *specs_);
+  void write(const Char* value) {
+    if (!value) {
+      FMT_THROW(format_error("string pointer is null"));
     } else {
-      writer_.write(value);
+      auto length = std::char_traits<char_type>::length(value);
+      basic_string_view<char_type> sv(value, length);
+      specs_ ? write(sv, *specs_) : write(sv);
     }
-    return out();
   }
 
-  iterator operator()(const void *value) {
+ public:
+  arg_formatter_base(OutputIt out, format_specs* s, locale_ref loc)
+      : out_(out), locale_(loc), specs_(s) {}
+
+  iterator operator()(monostate) {
+    FMT_ASSERT(false, "invalid argument type");
+    return out_;
+  }
+
+  template <typename T, FMT_ENABLE_IF(is_integral<T>::value)>
+  FMT_INLINE iterator operator()(T value) {
     if (specs_)
-      check_pointer_type_spec(specs_->type_, internal::error_handler());
+      write_int(value, *specs_);
+    else
+      out_ = detail::write<Char>(out_, value);
+    return out_;
+  }
+
+  iterator operator()(Char value) {
+    handle_char_specs(specs_,
+                      char_spec_handler(*this, static_cast<Char>(value)));
+    return out_;
+  }
+
+  iterator operator()(bool value) {
+    if (specs_ && specs_->type) return (*this)(value ? 1 : 0);
+    write(value != 0);
+    return out_;
+  }
+
+  template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+  iterator operator()(T value) {
+    auto specs = specs_ ? *specs_ : format_specs();
+    if (const_check(is_supported_floating_point(value)))
+      out_ = detail::write(out_, value, specs, locale_);
+    else
+      FMT_ASSERT(false, "unsupported float argument type");
+    return out_;
+  }
+
+  iterator operator()(const Char* value) {
+    if (!specs_) return write(value), out_;
+    handle_cstring_type_spec(specs_->type, cstring_spec_handler(*this, value));
+    return out_;
+  }
+
+  iterator operator()(basic_string_view<Char> value) {
+    if (specs_) {
+      check_string_type_spec(specs_->type, error_handler());
+      write(value, *specs_);
+    } else {
+      write(value);
+    }
+    return out_;
+  }
+
+  iterator operator()(const void* value) {
+    if (specs_) check_pointer_type_spec(specs_->type, error_handler());
     write_pointer(value);
-    return out();
+    return out_;
   }
 };
 
-template <typename Char>
-FMT_CONSTEXPR bool is_name_start(Char c) {
-  return ('a' <= c && c <= 'z') || ('A' <= c && c <= 'Z') || '_' == c;
-}
+/** The default argument formatter. */
+template <typename OutputIt, typename Char>
+class arg_formatter : public arg_formatter_base<OutputIt, Char> {
+ private:
+  using char_type = Char;
+  using base = arg_formatter_base<OutputIt, Char>;
+  using context_type = basic_format_context<OutputIt, Char>;
 
-// DEPRECATED: Parses the input as an unsigned integer. This function assumes
-// that the first character is a digit and presence of a non-digit character at
-// the end.
-// it: an iterator pointing to the beginning of the input range.
-template <typename Iterator, typename ErrorHandler>
-FMT_CONSTEXPR unsigned parse_nonnegative_int(Iterator &it, ErrorHandler &&eh) {
-  assert('0' <= *it && *it <= '9');
-  unsigned value = 0;
-  // Convert to unsigned to prevent a warning.
-  unsigned max_int = (std::numeric_limits<int>::max)();
-  unsigned big = max_int / 10;
-  do {
-    // Check for overflow.
-    if (value > big) {
-      value = max_int + 1;
-      break;
-    }
-    value = value * 10 + unsigned(*it - '0');
-    // Workaround for MSVC "setup_exception stack overflow" error:
-    auto next = it;
-    ++next;
-    it = next;
-  } while ('0' <= *it && *it <= '9');
-  if (value > max_int)
-    eh.on_error("number is too big");
-  return value;
+  context_type& ctx_;
+  basic_format_parse_context<char_type>* parse_ctx_;
+  const Char* ptr_;
+
+ public:
+  using iterator = typename base::iterator;
+  using format_specs = typename base::format_specs;
+
+  /**
+    \rst
+    Constructs an argument formatter object.
+    *ctx* is a reference to the formatting context,
+    *specs* contains format specifier information for standard argument types.
+    \endrst
+   */
+  explicit arg_formatter(
+      context_type& ctx,
+      basic_format_parse_context<char_type>* parse_ctx = nullptr,
+      format_specs* specs = nullptr, const Char* ptr = nullptr)
+      : base(ctx.out(), specs, ctx.locale()),
+        ctx_(ctx),
+        parse_ctx_(parse_ctx),
+        ptr_(ptr) {}
+
+  using base::operator();
+
+  /** Formats an argument of a user-defined type. */
+  iterator operator()(typename basic_format_arg<context_type>::handle handle) {
+    if (ptr_) advance_to(*parse_ctx_, ptr_);
+    handle.format(*parse_ctx_, ctx_);
+    return ctx_.out();
+  }
+};
+
+template <typename Char> FMT_CONSTEXPR bool is_name_start(Char c) {
+  return ('a' <= c && c <= 'z') || ('A' <= c && c <= 'Z') || '_' == c;
 }
 
 // Parses the range [begin, end) as an unsigned integer. This function assumes
 // that the range is non-empty and the first character is a digit.
 template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR unsigned parse_nonnegative_int(
-    const Char *&begin, const Char *end, ErrorHandler &&eh) {
-  assert(begin != end && '0' <= *begin && *begin <= '9');
+FMT_CONSTEXPR int parse_nonnegative_int(const Char*& begin, const Char* end,
+                                        ErrorHandler&& eh) {
+  FMT_ASSERT(begin != end && '0' <= *begin && *begin <= '9', "");
   unsigned value = 0;
   // Convert to unsigned to prevent a warning.
-  unsigned max_int = (std::numeric_limits<int>::max)();
+  constexpr unsigned max_int = max_value<int>();
   unsigned big = max_int / 10;
   do {
     // Check for overflow.
     if (value > big) {
       value = max_int + 1;
       break;
     }
-    value = value * 10 + unsigned(*begin++ - '0');
+    value = value * 10 + unsigned(*begin - '0');
+    ++begin;
   } while (begin != end && '0' <= *begin && *begin <= '9');
-  if (value > max_int)
-    eh.on_error("number is too big");
-  return value;
+  if (value > max_int) eh.on_error("number is too big");
+  return static_cast<int>(value);
 }
 
-template <typename Char, typename Context>
-class custom_formatter: public function<bool> {
+template <typename Context> class custom_formatter {
  private:
-  Context &ctx_;
+  using char_type = typename Context::char_type;
+
+  basic_format_parse_context<char_type>& parse_ctx_;
+  Context& ctx_;
 
  public:
-  explicit custom_formatter(Context &ctx): ctx_(ctx) {}
+  explicit custom_formatter(basic_format_parse_context<char_type>& parse_ctx,
+                            Context& ctx)
+      : parse_ctx_(parse_ctx), ctx_(ctx) {}
 
-  bool operator()(typename basic_format_arg<Context>::handle h) const {
-    h.format(ctx_);
-    return true;
+  void operator()(typename basic_format_arg<Context>::handle h) const {
+    h.format(parse_ctx_, ctx_);
   }
 
-  template <typename T>
-  bool operator()(T) const { return false; }
+  template <typename T> void operator()(T) const {}
 };
 
 template <typename T>
-struct is_integer {
-  enum {
-    value = std::is_integral<T>::value && !std::is_same<T, bool>::value &&
-            !std::is_same<T, char>::value && !std::is_same<T, wchar_t>::value
-  };
-};
-
-template <typename ErrorHandler>
-class width_checker: public function<unsigned long long> {
- public:
-  explicit FMT_CONSTEXPR width_checker(ErrorHandler &eh) : handler_(eh) {}
-
-  template <typename T>
-  FMT_CONSTEXPR
-  typename std::enable_if<
-      is_integer<T>::value, unsigned long long>::type operator()(T value) {
-    if (is_negative(value))
-      handler_.on_error("negative width");
+using is_integer =
+    bool_constant<is_integral<T>::value && !std::is_same<T, bool>::value &&
+                  !std::is_same<T, char>::value &&
+                  !std::is_same<T, wchar_t>::value>;
+
+template <typename ErrorHandler> class width_checker {
+ public:
+  explicit FMT_CONSTEXPR width_checker(ErrorHandler& eh) : handler_(eh) {}
+
+  template <typename T, FMT_ENABLE_IF(is_integer<T>::value)>
+  FMT_CONSTEXPR unsigned long long operator()(T value) {
+    if (is_negative(value)) handler_.on_error("negative width");
     return static_cast<unsigned long long>(value);
   }
 
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      !is_integer<T>::value, unsigned long long>::type operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!is_integer<T>::value)>
+  FMT_CONSTEXPR unsigned long long operator()(T) {
     handler_.on_error("width is not integer");
     return 0;
   }
 
  private:
-  ErrorHandler &handler_;
+  ErrorHandler& handler_;
 };
 
-template <typename ErrorHandler>
-class precision_checker: public function<unsigned long long> {
+template <typename ErrorHandler> class precision_checker {
  public:
-  explicit FMT_CONSTEXPR precision_checker(ErrorHandler &eh) : handler_(eh) {}
+  explicit FMT_CONSTEXPR precision_checker(ErrorHandler& eh) : handler_(eh) {}
 
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      is_integer<T>::value, unsigned long long>::type operator()(T value) {
-    if (is_negative(value))
-      handler_.on_error("negative precision");
+  template <typename T, FMT_ENABLE_IF(is_integer<T>::value)>
+  FMT_CONSTEXPR unsigned long long operator()(T value) {
+    if (is_negative(value)) handler_.on_error("negative precision");
     return static_cast<unsigned long long>(value);
   }
 
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      !is_integer<T>::value, unsigned long long>::type operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!is_integer<T>::value)>
+  FMT_CONSTEXPR unsigned long long operator()(T) {
     handler_.on_error("precision is not integer");
     return 0;
   }
 
  private:
-  ErrorHandler &handler_;
+  ErrorHandler& handler_;
 };
 
 // A format specifier handler that sets fields in basic_format_specs.
-template <typename Char>
-class specs_setter {
+template <typename Char> class specs_setter {
  public:
-  explicit FMT_CONSTEXPR specs_setter(basic_format_specs<Char> &specs):
-    specs_(specs) {}
+  explicit FMT_CONSTEXPR specs_setter(basic_format_specs<Char>& specs)
+      : specs_(specs) {}
 
-  FMT_CONSTEXPR specs_setter(const specs_setter &other) : specs_(other.specs_) {}
+  FMT_CONSTEXPR specs_setter(const specs_setter& other)
+      : specs_(other.specs_) {}
 
-  FMT_CONSTEXPR void on_align(alignment align) { specs_.align_ = align; }
-  FMT_CONSTEXPR void on_fill(Char fill) { specs_.fill_ = fill; }
-  FMT_CONSTEXPR void on_plus() { specs_.flags_ |= SIGN_FLAG | PLUS_FLAG; }
-  FMT_CONSTEXPR void on_minus() { specs_.flags_ |= MINUS_FLAG; }
-  FMT_CONSTEXPR void on_space() { specs_.flags_ |= SIGN_FLAG; }
-  FMT_CONSTEXPR void on_hash() { specs_.flags_ |= HASH_FLAG; }
+  FMT_CONSTEXPR void on_align(align_t align) { specs_.align = align; }
+  FMT_CONSTEXPR void on_fill(basic_string_view<Char> fill) {
+    specs_.fill = fill;
+  }
+  FMT_CONSTEXPR void on_plus() { specs_.sign = sign::plus; }
+  FMT_CONSTEXPR void on_minus() { specs_.sign = sign::minus; }
+  FMT_CONSTEXPR void on_space() { specs_.sign = sign::space; }
+  FMT_CONSTEXPR void on_hash() { specs_.alt = true; }
 
   FMT_CONSTEXPR void on_zero() {
-    specs_.align_ = ALIGN_NUMERIC;
-    specs_.fill_ = '0';
+    specs_.align = align::numeric;
+    specs_.fill[0] = Char('0');
   }
 
-  FMT_CONSTEXPR void on_width(unsigned width) { specs_.width_ = width; }
-  FMT_CONSTEXPR void on_precision(unsigned precision) {
-    specs_.precision_ = static_cast<int>(precision);
+  FMT_CONSTEXPR void on_width(int width) { specs_.width = width; }
+  FMT_CONSTEXPR void on_precision(int precision) {
+    specs_.precision = precision;
   }
   FMT_CONSTEXPR void end_precision() {}
 
-  FMT_CONSTEXPR void on_type(Char type) { specs_.type_ = type; }
+  FMT_CONSTEXPR void on_type(Char type) {
+    specs_.type = static_cast<char>(type);
+  }
 
  protected:
-  basic_format_specs<Char> &specs_;
+  basic_format_specs<Char>& specs_;
+};
+
+template <typename ErrorHandler> class numeric_specs_checker {
+ public:
+  FMT_CONSTEXPR numeric_specs_checker(ErrorHandler& eh, detail::type arg_type)
+      : error_handler_(eh), arg_type_(arg_type) {}
+
+  FMT_CONSTEXPR void require_numeric_argument() {
+    if (!is_arithmetic_type(arg_type_))
+      error_handler_.on_error("format specifier requires numeric argument");
+  }
+
+  FMT_CONSTEXPR void check_sign() {
+    require_numeric_argument();
+    if (is_integral_type(arg_type_) && arg_type_ != type::int_type &&
+        arg_type_ != type::long_long_type && arg_type_ != type::char_type) {
+      error_handler_.on_error("format specifier requires signed argument");
+    }
+  }
+
+  FMT_CONSTEXPR void check_precision() {
+    if (is_integral_type(arg_type_) || arg_type_ == type::pointer_type)
+      error_handler_.on_error("precision not allowed for this argument type");
+  }
+
+ private:
+  ErrorHandler& error_handler_;
+  detail::type arg_type_;
 };
 
 // A format specifier handler that checks if specifiers are consistent with the
 // argument type.
-template <typename Handler>
-class specs_checker : public Handler {
+template <typename Handler> class specs_checker : public Handler {
+ private:
+  numeric_specs_checker<Handler> checker_;
+
+  // Suppress an MSVC warning about using this in initializer list.
+  FMT_CONSTEXPR Handler& error_handler() { return *this; }
+
  public:
-  FMT_CONSTEXPR specs_checker(const Handler& handler, internal::type arg_type)
-    : Handler(handler), arg_type_(arg_type) {}
+  FMT_CONSTEXPR specs_checker(const Handler& handler, detail::type arg_type)
+      : Handler(handler), checker_(error_handler(), arg_type) {}
 
-  FMT_CONSTEXPR specs_checker(const specs_checker &other)
-    : Handler(other), arg_type_(other.arg_type_) {}
+  FMT_CONSTEXPR specs_checker(const specs_checker& other)
+      : Handler(other), checker_(error_handler(), other.arg_type_) {}
 
-  FMT_CONSTEXPR void on_align(alignment align) {
-    if (align == ALIGN_NUMERIC)
-      require_numeric_argument();
+  FMT_CONSTEXPR void on_align(align_t align) {
+    if (align == align::numeric) checker_.require_numeric_argument();
     Handler::on_align(align);
   }
 
   FMT_CONSTEXPR void on_plus() {
-    check_sign();
+    checker_.check_sign();
     Handler::on_plus();
   }
 
   FMT_CONSTEXPR void on_minus() {
-    check_sign();
+    checker_.check_sign();
     Handler::on_minus();
   }
 
   FMT_CONSTEXPR void on_space() {
-    check_sign();
+    checker_.check_sign();
     Handler::on_space();
   }
 
   FMT_CONSTEXPR void on_hash() {
-    require_numeric_argument();
+    checker_.require_numeric_argument();
     Handler::on_hash();
   }
 
   FMT_CONSTEXPR void on_zero() {
-    require_numeric_argument();
+    checker_.require_numeric_argument();
     Handler::on_zero();
   }
 
-  FMT_CONSTEXPR void end_precision() {
-    if (is_integral(arg_type_) || arg_type_ == pointer_type)
-      this->on_error("precision not allowed for this argument type");
-  }
-
- private:
-  FMT_CONSTEXPR void require_numeric_argument() {
-    if (!is_arithmetic(arg_type_))
-      this->on_error("format specifier requires numeric argument");
-  }
-
-  FMT_CONSTEXPR void check_sign() {
-    require_numeric_argument();
-    if (is_integral(arg_type_) && arg_type_ != int_type &&
-        arg_type_ != long_long_type && arg_type_ != internal::char_type) {
-      this->on_error("format specifier requires signed argument");
-    }
-  }
-
-  internal::type arg_type_;
+  FMT_CONSTEXPR void end_precision() { checker_.check_precision(); }
 };
 
-template <template <typename> class Handler, typename T,
-          typename Context, typename ErrorHandler>
-FMT_CONSTEXPR void set_dynamic_spec(
-    T &value, basic_format_arg<Context> arg, ErrorHandler eh) {
-  unsigned long long big_value = fmt::visit(Handler<ErrorHandler>(eh), arg);
-  if (big_value > (std::numeric_limits<int>::max)())
-    eh.on_error("number is too big");
-  value = static_cast<T>(big_value);
+template <template <typename> class Handler, typename FormatArg,
+          typename ErrorHandler>
+FMT_CONSTEXPR int get_dynamic_spec(FormatArg arg, ErrorHandler eh) {
+  unsigned long long value = visit_format_arg(Handler<ErrorHandler>(eh), arg);
+  if (value > to_unsigned(max_value<int>())) eh.on_error("number is too big");
+  return static_cast<int>(value);
 }
 
 struct auto_id {};
 
+template <typename Context, typename ID>
+FMT_CONSTEXPR typename Context::format_arg get_arg(Context& ctx, ID id) {
+  auto arg = ctx.arg(id);
+  if (!arg) ctx.on_error("argument not found");
+  return arg;
+}
+
 // The standard format specifier handler with checking.
-template <typename Context>
-class specs_handler: public specs_setter<typename Context::char_type> {
+template <typename ParseContext, typename Context>
+class specs_handler : public specs_setter<typename Context::char_type> {
  public:
-  typedef typename Context::char_type char_type;
+  using char_type = typename Context::char_type;
 
-  FMT_CONSTEXPR specs_handler(
-      basic_format_specs<char_type> &specs, Context &ctx)
-    : specs_setter<char_type>(specs), context_(ctx) {}
+  FMT_CONSTEXPR specs_handler(basic_format_specs<char_type>& specs,
+                              ParseContext& parse_ctx, Context& ctx)
+      : specs_setter<char_type>(specs),
+        parse_context_(parse_ctx),
+        context_(ctx) {}
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
-    set_dynamic_spec<width_checker>(
-          this->specs_.width_, get_arg(arg_id), context_.error_handler());
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
+    this->specs_.width = get_dynamic_spec<width_checker>(
+        get_arg(arg_id), context_.error_handler());
   }
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
-    set_dynamic_spec<precision_checker>(
-          this->specs_.precision_, get_arg(arg_id), context_.error_handler());
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
+    this->specs_.precision = get_dynamic_spec<precision_checker>(
+        get_arg(arg_id), context_.error_handler());
   }
 
-  void on_error(const char *message) {
-    context_.on_error(message);
-  }
+  void on_error(const char* message) { context_.on_error(message); }
 
  private:
-  FMT_CONSTEXPR basic_format_arg<Context> get_arg(auto_id) {
-    return context_.next_arg();
+  // This is only needed for compatibility with gcc 4.4.
+  using format_arg = typename Context::format_arg;
+
+  FMT_CONSTEXPR format_arg get_arg(auto_id) {
+    return detail::get_arg(context_, parse_context_.next_arg_id());
   }
 
-  template <typename Id>
-  FMT_CONSTEXPR basic_format_arg<Context> get_arg(Id arg_id) {
-    context_.parse_context().check_arg_id(arg_id);
-    return context_.get_arg(arg_id);
+  FMT_CONSTEXPR format_arg get_arg(int arg_id) {
+    parse_context_.check_arg_id(arg_id);
+    return detail::get_arg(context_, arg_id);
   }
 
-  Context &context_;
+  FMT_CONSTEXPR format_arg get_arg(basic_string_view<char_type> arg_id) {
+    parse_context_.check_arg_id(arg_id);
+    return detail::get_arg(context_, arg_id);
+  }
+
+  ParseContext& parse_context_;
+  Context& context_;
 };
 
+enum class arg_id_kind { none, index, name };
+
 // An argument reference.
-template <typename Char>
-struct arg_ref {
-  enum Kind { NONE, INDEX, NAME };
+template <typename Char> struct arg_ref {
+  FMT_CONSTEXPR arg_ref() : kind(arg_id_kind::none), val() {}
 
-  FMT_CONSTEXPR arg_ref() : kind(NONE), index(0) {}
-  FMT_CONSTEXPR explicit arg_ref(unsigned index) : kind(INDEX), index(index) {}
-  explicit arg_ref(basic_string_view<Char> name) : kind(NAME), name(name) {}
-
-  FMT_CONSTEXPR arg_ref &operator=(unsigned idx) {
-    kind = INDEX;
-    index = idx;
+  FMT_CONSTEXPR explicit arg_ref(int index)
+      : kind(arg_id_kind::index), val(index) {}
+  FMT_CONSTEXPR explicit arg_ref(basic_string_view<Char> name)
+      : kind(arg_id_kind::name), val(name) {}
+
+  FMT_CONSTEXPR arg_ref& operator=(int idx) {
+    kind = arg_id_kind::index;
+    val.index = idx;
     return *this;
   }
 
-  Kind kind;
-  FMT_UNION {
-    unsigned index;
+  arg_id_kind kind;
+  union value {
+    FMT_CONSTEXPR value(int id = 0) : index{id} {}
+    FMT_CONSTEXPR value(basic_string_view<Char> n) : name(n) {}
+
+    int index;
     basic_string_view<Char> name;
-  };
+  } val;
 };
 
 // Format specifiers with width and precision resolved at formatting rather
 // than parsing time to allow re-using the same parsed specifiers with
-// differents sets of arguments (precompilation of format strings).
+// different sets of arguments (precompilation of format strings).
 template <typename Char>
 struct dynamic_format_specs : basic_format_specs<Char> {
   arg_ref<Char> width_ref;
   arg_ref<Char> precision_ref;
 };
 
 // Format spec handler that saves references to arguments representing dynamic
 // width and precision to be resolved at formatting time.
 template <typename ParseContext>
-class dynamic_specs_handler :
-    public specs_setter<typename ParseContext::char_type> {
+class dynamic_specs_handler
+    : public specs_setter<typename ParseContext::char_type> {
  public:
-  typedef typename ParseContext::char_type char_type;
+  using char_type = typename ParseContext::char_type;
 
-  FMT_CONSTEXPR dynamic_specs_handler(
-      dynamic_format_specs<char_type> &specs, ParseContext &ctx)
-    : specs_setter<char_type>(specs), specs_(specs), context_(ctx) {}
+  FMT_CONSTEXPR dynamic_specs_handler(dynamic_format_specs<char_type>& specs,
+                                      ParseContext& ctx)
+      : specs_setter<char_type>(specs), specs_(specs), context_(ctx) {}
 
-  FMT_CONSTEXPR dynamic_specs_handler(const dynamic_specs_handler &other)
-    : specs_setter<char_type>(other),
-      specs_(other.specs_), context_(other.context_) {}
+  FMT_CONSTEXPR dynamic_specs_handler(const dynamic_specs_handler& other)
+      : specs_setter<char_type>(other),
+        specs_(other.specs_),
+        context_(other.context_) {}
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
     specs_.width_ref = make_arg_ref(arg_id);
   }
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
     specs_.precision_ref = make_arg_ref(arg_id);
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) {
+  FMT_CONSTEXPR void on_error(const char* message) {
     context_.on_error(message);
   }
 
  private:
-  typedef arg_ref<char_type> arg_ref_type;
+  using arg_ref_type = arg_ref<char_type>;
 
-  template <typename Id>
-  FMT_CONSTEXPR arg_ref_type make_arg_ref(Id arg_id) {
+  FMT_CONSTEXPR arg_ref_type make_arg_ref(int arg_id) {
     context_.check_arg_id(arg_id);
     return arg_ref_type(arg_id);
   }
 
   FMT_CONSTEXPR arg_ref_type make_arg_ref(auto_id) {
     return arg_ref_type(context_.next_arg_id());
   }
 
-  dynamic_format_specs<char_type> &specs_;
-  ParseContext &context_;
+  FMT_CONSTEXPR arg_ref_type make_arg_ref(basic_string_view<char_type> arg_id) {
+    context_.check_arg_id(arg_id);
+    basic_string_view<char_type> format_str(
+        context_.begin(), to_unsigned(context_.end() - context_.begin()));
+    return arg_ref_type(arg_id);
+  }
+
+  dynamic_format_specs<char_type>& specs_;
+  ParseContext& context_;
 };
 
-template <typename Iterator, typename IDHandler>
-FMT_CONSTEXPR Iterator parse_arg_id(Iterator it, IDHandler &&handler) {
-  typedef typename std::iterator_traits<Iterator>::value_type char_type;
-  char_type c = *it;
+template <typename Char, typename IDHandler>
+FMT_CONSTEXPR const Char* parse_arg_id(const Char* begin, const Char* end,
+                                       IDHandler&& handler) {
+  FMT_ASSERT(begin != end, "");
+  Char c = *begin;
   if (c == '}' || c == ':') {
     handler();
-    return it;
+    return begin;
   }
   if (c >= '0' && c <= '9') {
-    unsigned index = parse_nonnegative_int(it, handler);
-    if (*it != '}' && *it != ':') {
+    int index = 0;
+    if (c != '0')
+      index = parse_nonnegative_int(begin, end, handler);
+    else
+      ++begin;
+    if (begin == end || (*begin != '}' && *begin != ':'))
       handler.on_error("invalid format string");
-      return it;
-    }
-    handler(index);
-    return it;
+    else
+      handler(index);
+    return begin;
   }
   if (!is_name_start(c)) {
     handler.on_error("invalid format string");
-    return it;
-  }
-  auto start = it;
-  do {
-    c = *++it;
-  } while (is_name_start(c) || ('0' <= c && c <= '9'));
-  handler(basic_string_view<char_type>(
-            pointer_from(start), to_unsigned(it - start)));
-  return it;
-}
-
-template <typename Char, typename IDHandler>
-FMT_CONSTEXPR const Char *parse_arg_id(
-    const Char *begin, const Char *end, IDHandler &&handler) {
-  assert(begin != end);
-  Char c = *begin;
-  if (c == '}' || c == ':')
-    return handler(), begin;
-  if (c >= '0' && c <= '9') {
-    unsigned index = parse_nonnegative_int(begin, end, handler);
-    if (begin == end || (*begin != '}' && *begin != ':'))
-      return handler.on_error("invalid format string"), begin;
-    handler(index);
     return begin;
   }
-  if (!is_name_start(c))
-    return handler.on_error("invalid format string"), begin;
   auto it = begin;
   do {
-    c = *++it;
-  } while (it != end && (is_name_start(c) || ('0' <= c && c <= '9')));
+    ++it;
+  } while (it != end && (is_name_start(c = *it) || ('0' <= c && c <= '9')));
   handler(basic_string_view<Char>(begin, to_unsigned(it - begin)));
   return it;
 }
 
 // Adapts SpecHandler to IDHandler API for dynamic width.
-template <typename SpecHandler, typename Char>
-struct width_adapter {
-  explicit FMT_CONSTEXPR width_adapter(SpecHandler &h) : handler(h) {}
+template <typename SpecHandler, typename Char> struct width_adapter {
+  explicit FMT_CONSTEXPR width_adapter(SpecHandler& h) : handler(h) {}
 
   FMT_CONSTEXPR void operator()() { handler.on_dynamic_width(auto_id()); }
-  FMT_CONSTEXPR void operator()(unsigned id) { handler.on_dynamic_width(id); }
+  FMT_CONSTEXPR void operator()(int id) { handler.on_dynamic_width(id); }
   FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
     handler.on_dynamic_width(id);
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) {
+  FMT_CONSTEXPR void on_error(const char* message) {
     handler.on_error(message);
   }
 
-  SpecHandler &handler;
+  SpecHandler& handler;
 };
 
 // Adapts SpecHandler to IDHandler API for dynamic precision.
-template <typename SpecHandler, typename Char>
-struct precision_adapter {
-  explicit FMT_CONSTEXPR precision_adapter(SpecHandler &h) : handler(h) {}
+template <typename SpecHandler, typename Char> struct precision_adapter {
+  explicit FMT_CONSTEXPR precision_adapter(SpecHandler& h) : handler(h) {}
 
   FMT_CONSTEXPR void operator()() { handler.on_dynamic_precision(auto_id()); }
-  FMT_CONSTEXPR void operator()(unsigned id) {
-    handler.on_dynamic_precision(id);
-  }
+  FMT_CONSTEXPR void operator()(int id) { handler.on_dynamic_precision(id); }
   FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
     handler.on_dynamic_precision(id);
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) { handler.on_error(message); }
+  FMT_CONSTEXPR void on_error(const char* message) {
+    handler.on_error(message);
+  }
 
-  SpecHandler &handler;
+  SpecHandler& handler;
 };
 
-// Parses standard format specifiers and sends notifications about parsed
-// components to handler.
-// it: an iterator pointing to the beginning of a null-terminated range of
-//     characters, possibly emulated via null_terminating_iterator, representing
-//     format specifiers.
-template <typename Iterator, typename SpecHandler>
-FMT_CONSTEXPR Iterator parse_format_specs(Iterator it, SpecHandler &&handler) {
-  typedef typename std::iterator_traits<Iterator>::value_type char_type;
-  char_type c = *it;
-  if (c == '}' || !c)
-    return it;
+template <typename Char>
+FMT_CONSTEXPR int code_point_length(const Char* begin) {
+  if (const_check(sizeof(Char) != 1)) return 1;
+  constexpr char lengths[] = {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
+                              0, 0, 0, 0, 0, 0, 0, 0, 2, 2, 2, 2, 3, 3, 4, 0};
+  int len = lengths[static_cast<unsigned char>(*begin) >> 3];
 
-  // Parse fill and alignment.
-  alignment align = ALIGN_DEFAULT;
-  int i = 1;
-  do {
-    auto p = it + i;
-    switch (*p) {
-      case '<':
-        align = ALIGN_LEFT;
-        break;
-      case '>':
-        align = ALIGN_RIGHT;
-        break;
-      case '=':
-        align = ALIGN_NUMERIC;
-        break;
-      case '^':
-        align = ALIGN_CENTER;
-        break;
-    }
-    if (align != ALIGN_DEFAULT) {
-      if (p != it) {
-        if (c == '{') {
-          handler.on_error("invalid fill character '{'");
-          return it;
-        }
-        it += 2;
-        handler.on_fill(c);
-      } else ++it;
+  // Compute the pointer to the next character early so that the next
+  // iteration can start working on the next character. Neither Clang
+  // nor GCC figure out this reordering on their own.
+  return len + !len;
+}
+
+template <typename Char> constexpr bool is_ascii_letter(Char c) {
+  return (c >= 'a' && c <= 'z') || (c >= 'A' && c <= 'Z');
+}
+
+// Converts a character to ASCII. Returns a number > 127 on conversion failure.
+template <typename Char, FMT_ENABLE_IF(std::is_integral<Char>::value)>
+constexpr Char to_ascii(Char value) {
+  return value;
+}
+template <typename Char, FMT_ENABLE_IF(std::is_enum<Char>::value)>
+constexpr typename std::underlying_type<Char>::type to_ascii(Char value) {
+  return value;
+}
+
+// Parses fill and alignment.
+template <typename Char, typename Handler>
+FMT_CONSTEXPR const Char* parse_align(const Char* begin, const Char* end,
+                                      Handler&& handler) {
+  FMT_ASSERT(begin != end, "");
+  auto align = align::none;
+  auto p = begin + code_point_length(begin);
+  if (p >= end) p = begin;
+  for (;;) {
+    switch (to_ascii(*p)) {
+    case '<':
+      align = align::left;
+      break;
+    case '>':
+      align = align::right;
+      break;
+#if FMT_DEPRECATED_NUMERIC_ALIGN
+    case '=':
+      align = align::numeric;
+      break;
+#endif
+    case '^':
+      align = align::center;
+      break;
+    }
+    if (align != align::none) {
+      if (p != begin) {
+        auto c = *begin;
+        if (c == '{')
+          return handler.on_error("invalid fill character '{'"), begin;
+        handler.on_fill(basic_string_view<Char>(begin, to_unsigned(p - begin)));
+        begin = p + 1;
+      } else
+        ++begin;
       handler.on_align(align);
       break;
+    } else if (p == begin) {
+      break;
+    }
+    p = begin;
+  }
+  return begin;
+}
+
+template <typename Char, typename Handler>
+FMT_CONSTEXPR const Char* parse_width(const Char* begin, const Char* end,
+                                      Handler&& handler) {
+  FMT_ASSERT(begin != end, "");
+  if ('0' <= *begin && *begin <= '9') {
+    handler.on_width(parse_nonnegative_int(begin, end, handler));
+  } else if (*begin == '{') {
+    ++begin;
+    if (begin != end)
+      begin = parse_arg_id(begin, end, width_adapter<Handler, Char>(handler));
+    if (begin == end || *begin != '}')
+      return handler.on_error("invalid format string"), begin;
+    ++begin;
+  }
+  return begin;
+}
+
+template <typename Char, typename Handler>
+FMT_CONSTEXPR const Char* parse_precision(const Char* begin, const Char* end,
+                                          Handler&& handler) {
+  ++begin;
+  auto c = begin != end ? *begin : Char();
+  if ('0' <= c && c <= '9') {
+    handler.on_precision(parse_nonnegative_int(begin, end, handler));
+  } else if (c == '{') {
+    ++begin;
+    if (begin != end) {
+      begin =
+          parse_arg_id(begin, end, precision_adapter<Handler, Char>(handler));
     }
-  } while (--i >= 0);
+    if (begin == end || *begin++ != '}')
+      return handler.on_error("invalid format string"), begin;
+  } else {
+    return handler.on_error("missing precision specifier"), begin;
+  }
+  handler.end_precision();
+  return begin;
+}
+
+// Parses standard format specifiers and sends notifications about parsed
+// components to handler.
+template <typename Char, typename SpecHandler>
+FMT_CONSTEXPR const Char* parse_format_specs(const Char* begin, const Char* end,
+                                             SpecHandler&& handler) {
+  if (begin == end) return begin;
+
+  begin = parse_align(begin, end, handler);
+  if (begin == end) return begin;
 
   // Parse sign.
-  switch (*it) {
-    case '+':
-      handler.on_plus();
-      ++it;
-      break;
-    case '-':
-      handler.on_minus();
-      ++it;
-      break;
-    case ' ':
-      handler.on_space();
-      ++it;
-      break;
+  switch (to_ascii(*begin)) {
+  case '+':
+    handler.on_plus();
+    ++begin;
+    break;
+  case '-':
+    handler.on_minus();
+    ++begin;
+    break;
+  case ' ':
+    handler.on_space();
+    ++begin;
+    break;
   }
+  if (begin == end) return begin;
 
-  if (*it == '#') {
+  if (*begin == '#') {
     handler.on_hash();
-    ++it;
+    if (++begin == end) return begin;
   }
 
   // Parse zero flag.
-  if (*it == '0') {
+  if (*begin == '0') {
     handler.on_zero();
-    ++it;
+    if (++begin == end) return begin;
   }
 
-  // Parse width.
-  if ('0' <= *it && *it <= '9') {
-    handler.on_width(parse_nonnegative_int(it, handler));
-  } else if (*it == '{') {
-    it = parse_arg_id(it + 1, width_adapter<SpecHandler, char_type>(handler));
-    if (*it++ != '}') {
-      handler.on_error("invalid format string");
-      return it;
-    }
-  }
+  begin = parse_width(begin, end, handler);
+  if (begin == end) return begin;
 
   // Parse precision.
-  if (*it == '.') {
-    ++it;
-    if ('0' <= *it && *it <= '9') {
-      handler.on_precision(parse_nonnegative_int(it, handler));
-    } else if (*it == '{') {
-      it = parse_arg_id(
-            it + 1, precision_adapter<SpecHandler, char_type>(handler));
-      if (*it++ != '}') {
-        handler.on_error("invalid format string");
-        return it;
-      }
-    } else {
-      handler.on_error("missing precision specifier");
-      return it;
-    }
-    handler.end_precision();
+  if (*begin == '.') {
+    begin = parse_precision(begin, end, handler);
   }
 
   // Parse type.
-  if (*it != '}' && *it)
-    handler.on_type(*it++);
-  return it;
+  if (begin != end && *begin != '}') handler.on_type(*begin++);
+  return begin;
 }
 
 // Return the result via the out param to workaround gcc bug 77539.
 template <bool IS_CONSTEXPR, typename T, typename Ptr = const T*>
-FMT_CONSTEXPR bool find(Ptr first, Ptr last, T value, Ptr &out) {
+FMT_CONSTEXPR bool find(Ptr first, Ptr last, T value, Ptr& out) {
   for (out = first; out != last; ++out) {
-    if (*out == value)
-      return true;
+    if (*out == value) return true;
   }
   return false;
 }
 
 template <>
-inline bool find<false, char>(
-    const char *first, const char *last, char value, const char *&out) {
-  out = static_cast<const char*>(std::memchr(first, value, last - first));
-  return out != FMT_NULL;
+inline bool find<false, char>(const char* first, const char* last, char value,
+                              const char*& out) {
+  out = static_cast<const char*>(
+      std::memchr(first, value, detail::to_unsigned(last - first)));
+  return out != nullptr;
 }
 
-template <typename Handler, typename Char>
-struct id_adapter {
-  FMT_CONSTEXPR void operator()() { handler.on_arg_id(); }
-  FMT_CONSTEXPR void operator()(unsigned id) { handler.on_arg_id(id); }
+template <typename Handler, typename Char> struct id_adapter {
+  Handler& handler;
+  int arg_id;
+
+  FMT_CONSTEXPR void operator()() { arg_id = handler.on_arg_id(); }
+  FMT_CONSTEXPR void operator()(int id) { arg_id = handler.on_arg_id(id); }
   FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
-    handler.on_arg_id(id);
+    arg_id = handler.on_arg_id(id);
   }
-  FMT_CONSTEXPR void on_error(const char *message) {
+  FMT_CONSTEXPR void on_error(const char* message) {
     handler.on_error(message);
   }
-  Handler &handler;
 };
 
+template <typename Char, typename Handler>
+FMT_CONSTEXPR const Char* parse_replacement_field(const Char* begin,
+                                                  const Char* end,
+                                                  Handler&& handler) {
+  ++begin;
+  if (begin == end) return handler.on_error("invalid format string"), end;
+  if (*begin == '}') {
+    handler.on_replacement_field(handler.on_arg_id(), begin);
+  } else if (*begin == '{') {
+    handler.on_text(begin, begin + 1);
+  } else {
+    auto adapter = id_adapter<Handler, Char>{handler, 0};
+    begin = parse_arg_id(begin, end, adapter);
+    Char c = begin != end ? *begin : Char();
+    if (c == '}') {
+      handler.on_replacement_field(adapter.arg_id, begin);
+    } else if (c == ':') {
+      begin = handler.on_format_specs(adapter.arg_id, begin + 1, end);
+      if (begin == end || *begin != '}')
+        return handler.on_error("unknown format specifier"), end;
+    } else {
+      return handler.on_error("missing '}' in format string"), end;
+    }
+  }
+  return begin + 1;
+}
+
 template <bool IS_CONSTEXPR, typename Char, typename Handler>
-FMT_CONSTEXPR void parse_format_string(
-        basic_string_view<Char> format_str, Handler &&handler) {
+FMT_CONSTEXPR_DECL FMT_INLINE void parse_format_string(
+    basic_string_view<Char> format_str, Handler&& handler) {
+  auto begin = format_str.data();
+  auto end = begin + format_str.size();
+  if (end - begin < 32) {
+    // Use a simple loop instead of memchr for small strings.
+    const Char* p = begin;
+    while (p != end) {
+      auto c = *p++;
+      if (c == '{') {
+        handler.on_text(begin, p - 1);
+        begin = p = parse_replacement_field(p - 1, end, handler);
+      } else if (c == '}') {
+        if (p == end || *p != '}')
+          return handler.on_error("unmatched '}' in format string");
+        handler.on_text(begin, p);
+        begin = ++p;
+      }
+    }
+    handler.on_text(begin, end);
+    return;
+  }
   struct writer {
-    FMT_CONSTEXPR void operator()(const Char *begin, const Char *end) {
-      if (begin == end) return;
+    FMT_CONSTEXPR void operator()(const Char* pbegin, const Char* pend) {
+      if (pbegin == pend) return;
       for (;;) {
-        const Char *p = FMT_NULL;
-        if (!find<IS_CONSTEXPR>(begin, end, '}', p))
-          return handler_.on_text(begin, end);
+        const Char* p = nullptr;
+        if (!find<IS_CONSTEXPR>(pbegin, pend, '}', p))
+          return handler_.on_text(pbegin, pend);
         ++p;
-        if (p == end || *p != '}')
+        if (p == pend || *p != '}')
           return handler_.on_error("unmatched '}' in format string");
-        handler_.on_text(begin, p);
-        begin = p + 1;
+        handler_.on_text(pbegin, p);
+        pbegin = p + 1;
       }
     }
-    Handler &handler_;
+    Handler& handler_;
   } write{handler};
-  auto begin = format_str.data();
-  auto end = begin + format_str.size();
   while (begin != end) {
     // Doing two passes with memchr (one for '{' and another for '}') is up to
     // 2.5x faster than the naive one-pass implementation on big format strings.
-    const Char *p = begin;
-    if (*begin != '{' && !find<IS_CONSTEXPR>(begin, end, '{', p))
+    const Char* p = begin;
+    if (*begin != '{' && !find<IS_CONSTEXPR>(begin + 1, end, '{', p))
       return write(begin, end);
     write(begin, p);
-    ++p;
-    if (p == end)
-      return handler.on_error("invalid format string");
-    if (*p == '}') {
-      handler.on_arg_id();
-      handler.on_replacement_field(p);
-    } else if (*p == '{') {
-      handler.on_text(p, p + 1);
-    } else {
-      p = parse_arg_id(p, end, id_adapter<Handler, Char>{handler});
-      Char c = p != end ? *p : 0;
-      if (c == '}') {
-        handler.on_replacement_field(p);
-      } else if (c == ':') {
-        internal::null_terminating_iterator<Char> it(p + 1, end);
-        it = handler.on_format_specs(it);
-        if (*it != '}')
-          return handler.on_error("unknown format specifier");
-        p = pointer_from(it);
-      } else {
-        return handler.on_error("missing '}' in format string");
-      }
-    }
-    begin = p + 1;
+    begin = parse_replacement_field(p, end, handler);
   }
 }
 
 template <typename T, typename ParseContext>
-FMT_CONSTEXPR const typename ParseContext::char_type *
-    parse_format_specs(ParseContext &ctx) {
-  // GCC 7.2 requires initializer.
-  formatter<T, typename ParseContext::char_type> f{};
+FMT_CONSTEXPR const typename ParseContext::char_type* parse_format_specs(
+    ParseContext& ctx) {
+  using char_type = typename ParseContext::char_type;
+  using context = buffer_context<char_type>;
+  using mapped_type =
+      conditional_t<detail::mapped_type_constant<T, context>::value !=
+                        type::custom_type,
+                    decltype(arg_mapper<context>().map(std::declval<T>())), T>;
+  auto f = conditional_t<has_formatter<mapped_type, context>::value,
+                         formatter<mapped_type, char_type>,
+                         detail::fallback_formatter<T, char_type>>();
   return f.parse(ctx);
 }
 
+template <typename OutputIt, typename Char, typename Context>
+struct format_handler : detail::error_handler {
+  basic_format_parse_context<Char> parse_context;
+  Context context;
+
+  format_handler(OutputIt out, basic_string_view<Char> str,
+                 basic_format_args<Context> format_args, detail::locale_ref loc)
+      : parse_context(str), context(out, format_args, loc) {}
+
+  void on_text(const Char* begin, const Char* end) {
+    auto size = to_unsigned(end - begin);
+    auto out = context.out();
+    auto&& it = reserve(out, size);
+    it = std::copy_n(begin, size, it);
+    context.advance_to(out);
+  }
+
+  int on_arg_id() { return parse_context.next_arg_id(); }
+  int on_arg_id(int id) { return parse_context.check_arg_id(id), id; }
+  int on_arg_id(basic_string_view<Char> id) {
+    int arg_id = context.arg_id(id);
+    if (arg_id < 0) on_error("argument not found");
+    return arg_id;
+  }
+
+  FMT_INLINE void on_replacement_field(int id, const Char*) {
+    auto arg = get_arg(context, id);
+    context.advance_to(visit_format_arg(
+        default_arg_formatter<OutputIt, Char>{context.out(), context.args(),
+                                              context.locale()},
+        arg));
+  }
+
+  const Char* on_format_specs(int id, const Char* begin, const Char* end) {
+    auto arg = get_arg(context, id);
+    if (arg.type() == type::custom_type) {
+      advance_to(parse_context, begin);
+      visit_format_arg(custom_formatter<Context>(parse_context, context), arg);
+      return parse_context.begin();
+    }
+    auto specs = basic_format_specs<Char>();
+    if (begin + 1 < end && begin[1] == '}' && is_ascii_letter(*begin)) {
+      specs.type = static_cast<char>(*begin++);
+    } else {
+      using parse_context_t = basic_format_parse_context<Char>;
+      specs_checker<specs_handler<parse_context_t, Context>> handler(
+          specs_handler<parse_context_t, Context>(specs, parse_context,
+                                                  context),
+          arg.type());
+      begin = parse_format_specs(begin, end, handler);
+      if (begin == end || *begin != '}')
+        on_error("missing '}' in format string");
+    }
+    context.advance_to(visit_format_arg(
+        arg_formatter<OutputIt, Char>(context, &parse_context, &specs), arg));
+    return begin;
+  }
+};
+
+// A parse context with extra argument id checks. It is only used at compile
+// time because adding checks at runtime would introduce substantial overhead
+// and would be redundant since argument ids are checked when arguments are
+// retrieved anyway.
+template <typename Char, typename ErrorHandler = error_handler>
+class compile_parse_context
+    : public basic_format_parse_context<Char, ErrorHandler> {
+ private:
+  int num_args_;
+  using base = basic_format_parse_context<Char, ErrorHandler>;
+
+ public:
+  explicit FMT_CONSTEXPR compile_parse_context(
+      basic_string_view<Char> format_str, int num_args = max_value<int>(),
+      ErrorHandler eh = {})
+      : base(format_str, eh), num_args_(num_args) {}
+
+  FMT_CONSTEXPR int next_arg_id() {
+    int id = base::next_arg_id();
+    if (id >= num_args_) this->on_error("argument not found");
+    return id;
+  }
+
+  FMT_CONSTEXPR void check_arg_id(int id) {
+    base::check_arg_id(id);
+    if (id >= num_args_) this->on_error("argument not found");
+  }
+  using base::check_arg_id;
+};
+
 template <typename Char, typename ErrorHandler, typename... Args>
 class format_string_checker {
  public:
   explicit FMT_CONSTEXPR format_string_checker(
       basic_string_view<Char> format_str, ErrorHandler eh)
-    : arg_id_(-1), context_(format_str, eh),
-      parse_funcs_{&parse_format_specs<Args, parse_context_type>...} {}
+      : context_(format_str, num_args, eh),
+        parse_funcs_{&parse_format_specs<Args, parse_context_type>...} {}
 
-  typedef internal::null_terminating_iterator<Char> iterator;
+  FMT_CONSTEXPR void on_text(const Char*, const Char*) {}
 
-  FMT_CONSTEXPR void on_text(const Char *, const Char *) {}
-
-  FMT_CONSTEXPR void on_arg_id() {
-    arg_id_ = context_.next_arg_id();
-    check_arg_id();
-  }
-  FMT_CONSTEXPR void on_arg_id(unsigned id) {
-    arg_id_ = id;
-    context_.check_arg_id(id);
-    check_arg_id();
+  FMT_CONSTEXPR int on_arg_id() { return context_.next_arg_id(); }
+  FMT_CONSTEXPR int on_arg_id(int id) { return context_.check_arg_id(id), id; }
+  FMT_CONSTEXPR int on_arg_id(basic_string_view<Char>) {
+    on_error("compile-time checks don't support named arguments");
+    return 0;
   }
-  FMT_CONSTEXPR void on_arg_id(basic_string_view<Char>) {}
 
-  FMT_CONSTEXPR void on_replacement_field(const Char *) {}
+  FMT_CONSTEXPR void on_replacement_field(int, const Char*) {}
 
-  FMT_CONSTEXPR const Char *on_format_specs(iterator it) {
-    auto p = pointer_from(it);
-    context_.advance_to(p);
-    return to_unsigned(arg_id_) < NUM_ARGS ?
-          parse_funcs_[arg_id_](context_) : p;
+  FMT_CONSTEXPR const Char* on_format_specs(int id, const Char* begin,
+                                            const Char*) {
+    advance_to(context_, begin);
+    return id < num_args ? parse_funcs_[id](context_) : begin;
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) {
+  FMT_CONSTEXPR void on_error(const char* message) {
     context_.on_error(message);
   }
 
  private:
-  typedef basic_parse_context<Char, ErrorHandler> parse_context_type;
-  enum { NUM_ARGS = sizeof...(Args) };
-
-  FMT_CONSTEXPR void check_arg_id() {
-    if (internal::to_unsigned(arg_id_) >= NUM_ARGS)
-      context_.on_error("argument index out of range");
-  }
+  using parse_context_type = compile_parse_context<Char, ErrorHandler>;
+  enum { num_args = sizeof...(Args) };
 
   // Format specifier parsing function.
-  typedef const Char *(*parse_func)(parse_context_type &);
+  using parse_func = const Char* (*)(parse_context_type&);
 
-  int arg_id_;
   parse_context_type context_;
-  parse_func parse_funcs_[NUM_ARGS > 0 ? NUM_ARGS : 1];
+  parse_func parse_funcs_[num_args > 0 ? num_args : 1];
 };
 
-template <typename Char, typename ErrorHandler, typename... Args>
-FMT_CONSTEXPR bool check_format_string(
-    basic_string_view<Char> s, ErrorHandler eh = ErrorHandler()) {
-  format_string_checker<Char, ErrorHandler, Args...> checker(s, eh);
-  parse_format_string<true>(s, checker);
-  return true;
+// Converts string literals to basic_string_view.
+template <typename Char, size_t N>
+FMT_CONSTEXPR basic_string_view<Char> compile_string_to_view(
+    const Char (&s)[N]) {
+  // Remove trailing null character if needed. Won't be present if this is used
+  // with raw character array (i.e. not defined as a string).
+  return {s,
+          N - ((std::char_traits<Char>::to_int_type(s[N - 1]) == 0) ? 1 : 0)};
 }
 
-template <typename... Args, typename String>
-typename std::enable_if<is_compile_string<String>::value>::type
-    check_format_string(String format_str) {
+// Converts string_view to basic_string_view.
+template <typename Char>
+FMT_CONSTEXPR basic_string_view<Char> compile_string_to_view(
+    const std_string_view<Char>& s) {
+  return {s.data(), s.size()};
+}
+
+#define FMT_STRING_IMPL(s, base)                                  \
+  [] {                                                            \
+    /* Use a macro-like name to avoid shadowing warnings. */      \
+    struct FMT_COMPILE_STRING : base {                            \
+      using char_type = fmt::remove_cvref_t<decltype(s[0])>;      \
+      FMT_MAYBE_UNUSED FMT_CONSTEXPR                              \
+      operator fmt::basic_string_view<char_type>() const {        \
+        return fmt::detail::compile_string_to_view<char_type>(s); \
+      }                                                           \
+    };                                                            \
+    return FMT_COMPILE_STRING();                                  \
+  }()
+
+/**
+  \rst
+  Constructs a compile-time format string from a string literal *s*.
+
+  **Example**::
+
+    // A compile-time error because 'd' is an invalid specifier for strings.
+    std::string s = fmt::format(FMT_STRING("{:d}"), "foo");
+  \endrst
+ */
+#define FMT_STRING(s) FMT_STRING_IMPL(s, fmt::compile_string)
+
+template <typename... Args, typename S,
+          enable_if_t<(is_compile_string<S>::value), int>>
+void check_format_string(S format_str) {
+  FMT_CONSTEXPR_DECL auto s = to_string_view(format_str);
+  using checker = format_string_checker<typename S::char_type, error_handler,
+                                        remove_cvref_t<Args>...>;
   FMT_CONSTEXPR_DECL bool invalid_format =
-      internal::check_format_string<char, internal::error_handler, Args...>(
-        string_view(format_str.data(), format_str.size()));
+      (parse_format_string<true>(s, checker(s, {})), true);
   (void)invalid_format;
 }
 
-// Specifies whether to format T using the standard formatter.
-// It is not possible to use get_type in formatter specialization directly
-// because of a bug in MSVC.
-template <typename Context, typename T>
-struct format_type :
-  std::integral_constant<bool, get_type<Context, T>::value != custom_type> {};
-
-template <template <typename> class Handler, typename Spec, typename Context>
-void handle_dynamic_spec(
-    Spec &value, arg_ref<typename Context::char_type> ref, Context &ctx) {
-  typedef typename Context::char_type char_type;
+template <template <typename> class Handler, typename Context>
+void handle_dynamic_spec(int& value, arg_ref<typename Context::char_type> ref,
+                         Context& ctx) {
   switch (ref.kind) {
-  case arg_ref<char_type>::NONE:
+  case arg_id_kind::none:
     break;
-  case arg_ref<char_type>::INDEX:
-    internal::set_dynamic_spec<Handler>(
-          value, ctx.get_arg(ref.index), ctx.error_handler());
+  case arg_id_kind::index:
+    value = detail::get_dynamic_spec<Handler>(ctx.arg(ref.val.index),
+                                              ctx.error_handler());
     break;
-  case arg_ref<char_type>::NAME:
-    internal::set_dynamic_spec<Handler>(
-          value, ctx.get_arg(ref.name), ctx.error_handler());
+  case arg_id_kind::name:
+    value = detail::get_dynamic_spec<Handler>(ctx.arg(ref.val.name),
+                                              ctx.error_handler());
     break;
   }
 }
-}  // namespace internal
-
-/** The default argument formatter. */
-template <typename Range>
-class arg_formatter:
-  public internal::function<
-    typename internal::arg_formatter_base<Range>::iterator>,
-  public internal::arg_formatter_base<Range> {
- private:
-  typedef typename Range::value_type char_type;
-  typedef internal::arg_formatter_base<Range> base;
-  typedef basic_format_context<typename base::iterator, char_type> context_type;
-
-  context_type &ctx_;
-
- public:
-  typedef Range range;
-  typedef typename base::iterator iterator;
-  typedef typename base::format_specs format_specs;
-
-  /**
-    \rst
-    Constructs an argument formatter object.
-    *ctx* is a reference to the formatting context,
-    *spec* contains format specifier information for standard argument types.
-    \endrst
-   */
-  explicit arg_formatter(context_type &ctx, format_specs *spec = {})
-  : base(Range(ctx.out()), spec), ctx_(ctx) {}
 
-  // Deprecated.
-  arg_formatter(context_type &ctx, format_specs &spec)
-  : base(Range(ctx.out()), &spec), ctx_(ctx) {}
+using format_func = void (*)(detail::buffer<char>&, int, string_view);
 
-  using base::operator();
+FMT_API void format_error_code(buffer<char>& out, int error_code,
+                               string_view message) FMT_NOEXCEPT;
 
-  /** Formats an argument of a user-defined type. */
-  iterator operator()(typename basic_format_arg<context_type>::handle handle) {
-    handle.format(ctx_);
-    return this->out();
-  }
-};
+FMT_API void report_error(format_func func, int error_code,
+                          string_view message) FMT_NOEXCEPT;
+}  // namespace detail
+
+template <typename OutputIt, typename Char>
+using arg_formatter FMT_DEPRECATED_ALIAS =
+    detail::arg_formatter<OutputIt, Char>;
 
 /**
  An error returned by an operating system or a language runtime,
  for example a file opening error.
 */
-class system_error : public std::runtime_error {
+FMT_CLASS_API
+class FMT_API system_error : public std::runtime_error {
  private:
-  FMT_API void init(int err_code, string_view format_str, format_args args);
+  void init(int err_code, string_view format_str, format_args args);
 
  protected:
   int error_code_;
 
-  system_error() : std::runtime_error("") {}
+  system_error() : std::runtime_error(""), error_code_(0) {}
 
  public:
   /**
    \rst
    Constructs a :class:`fmt::system_error` object with a description
    formatted with `fmt::format_system_error`. *message* and additional
    arguments passed into the constructor are formatted similarly to
@@ -2374,18 +3297,23 @@
      const char *filename = "madeup";
      std::FILE *file = std::fopen(filename, "r");
      if (!file)
        throw fmt::system_error(errno, "cannot open file '{}'", filename);
    \endrst
   */
   template <typename... Args>
-  system_error(int error_code, string_view message, const Args &... args)
-    : std::runtime_error("") {
+  system_error(int error_code, string_view message, const Args&... args)
+      : std::runtime_error("") {
     init(error_code, message, make_format_args(args...));
   }
+  system_error(const system_error&) = default;
+  system_error& operator=(const system_error&) = default;
+  system_error(system_error&&) = default;
+  system_error& operator=(system_error&&) = default;
+  ~system_error() FMT_NOEXCEPT FMT_OVERRIDE;
 
   int error_code() const { return error_code_; }
 };
 
 /**
   \rst
   Formats an error returned by an operating system or a language runtime,
@@ -2398,1328 +3326,643 @@
   where *<message>* is the passed message and *<system-message>* is
   the system message corresponding to the error code.
   *error_code* is a system error code as given by ``errno``.
   If *error_code* is not a valid error code such as -1, the system message
   may look like "Unknown error -1" and is platform-dependent.
   \endrst
  */
-FMT_API void format_system_error(internal::buffer &out, int error_code,
-                                 fmt::string_view message) FMT_NOEXCEPT;
-
-/**
-  This template provides operations for formatting and writing data into a
-  character range.
- */
-template <typename Range>
-class basic_writer {
- public:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef basic_format_specs<char_type> format_specs;
-
- private:
-  iterator out_;  // Output iterator.
-  std::unique_ptr<locale_provider> locale_;
-
-  iterator out() const { return out_; }
-
-  // Attempts to reserve space for n extra characters in the output range.
-  // Returns a pointer to the reserved range or a reference to out_.
-  auto reserve(std::size_t n) -> decltype(internal::reserve(out_, n)) {
-    return internal::reserve(out_, n);
-  }
-
-  // Writes a value in the format
-  //   <left-padding><value><right-padding>
-  // where <value> is written by f(it).
-  template <typename F>
-  void write_padded(std::size_t size, const align_spec &spec, F &&f);
-
-  template <typename F>
-  struct padded_int_writer {
-    string_view prefix;
-    char_type fill;
-    std::size_t padding;
-    F f;
-
-    template <typename It>
-    void operator()(It &&it) const {
-      if (prefix.size() != 0)
-        it = std::copy_n(prefix.data(), prefix.size(), it);
-      it = std::fill_n(it, padding, fill);
-      f(it);
-    }
-  };
-
-  // Writes an integer in the format
-  //   <left-padding><prefix><numeric-padding><digits><right-padding>
-  // where <digits> are written by f(it).
-  template <typename Spec, typename F>
-  void write_int(unsigned num_digits, string_view prefix,
-                 const Spec &spec, F f) {
-    std::size_t size = prefix.size() + num_digits;
-    char_type fill = static_cast<char_type>(spec.fill());
-    std::size_t padding = 0;
-    if (spec.align() == ALIGN_NUMERIC) {
-      if (spec.width() > size) {
-        padding = spec.width() - size;
-        size = spec.width();
-      }
-    } else if (spec.precision() > static_cast<int>(num_digits)) {
-      size = prefix.size() + static_cast<std::size_t>(spec.precision());
-      padding = static_cast<std::size_t>(spec.precision()) - num_digits;
-      fill = '0';
-    }
-    align_spec as = spec;
-    if (spec.align() == ALIGN_DEFAULT)
-      as.align_ = ALIGN_RIGHT;
-    write_padded(size, as, padded_int_writer<F>{prefix, fill, padding, f});
-  }
-
-  // Writes a decimal integer.
-  template <typename Int>
-  void write_decimal(Int value) {
-    typedef typename internal::int_traits<Int>::main_type main_type;
-    main_type abs_value = static_cast<main_type>(value);
-    bool is_negative = internal::is_negative(value);
-    if (is_negative)
-      abs_value = 0 - abs_value;
-    unsigned num_digits = internal::count_digits(abs_value);
-    auto &&it = reserve((is_negative ? 1 : 0) + num_digits);
-    if (is_negative)
-      *it++ = '-';
-    it = internal::format_decimal(it, abs_value, num_digits);
-  }
-
-  // The handle_int_type_spec handler that writes an integer.
-  template <typename Int, typename Spec>
-  struct int_writer {
-    typedef typename internal::int_traits<Int>::main_type unsigned_type;
-
-    basic_writer<Range> &writer;
-    const Spec &spec;
-    unsigned_type abs_value;
-    char prefix[4];
-    unsigned prefix_size;
-
-    string_view get_prefix() const { return string_view(prefix, prefix_size); }
-
-    // Counts the number of digits in abs_value. BITS = log2(radix).
-    template <unsigned BITS>
-    unsigned count_digits() const {
-      unsigned_type n = abs_value;
-      unsigned num_digits = 0;
-      do {
-        ++num_digits;
-      } while ((n >>= BITS) != 0);
-      return num_digits;
-    }
-
-    int_writer(basic_writer<Range> &w, Int value, const Spec &s)
-      : writer(w), spec(s), abs_value(static_cast<unsigned_type>(value)),
-        prefix_size(0) {
-      if (internal::is_negative(value)) {
-        prefix[0] = '-';
-        ++prefix_size;
-        abs_value = 0 - abs_value;
-      } else if (spec.flag(SIGN_FLAG)) {
-        prefix[0] = spec.flag(PLUS_FLAG) ? '+' : ' ';
-        ++prefix_size;
-      }
-    }
-
-    struct dec_writer {
-      unsigned_type abs_value;
-      unsigned num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_decimal(it, abs_value, num_digits);
-      }
-    };
-
-    void on_dec() {
-      unsigned num_digits = internal::count_digits(abs_value);
-      writer.write_int(num_digits, get_prefix(), spec,
-                       dec_writer{abs_value, num_digits});
-    }
-
-    struct hex_writer {
-      int_writer &self;
-      unsigned num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_uint<4>(it, self.abs_value, num_digits,
-                                      self.spec.type() != 'x');
-      }
-    };
-
-    void on_hex() {
-      if (spec.flag(HASH_FLAG)) {
-        prefix[prefix_size++] = '0';
-        prefix[prefix_size++] = static_cast<char>(spec.type());
-      }
-      unsigned num_digits = count_digits<4>();
-      writer.write_int(num_digits, get_prefix(), spec,
-                       hex_writer{*this, num_digits});
-    }
-
-    template <int BITS>
-    struct bin_writer {
-      unsigned_type abs_value;
-      unsigned num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_uint<BITS>(it, abs_value, num_digits);
-      }
-    };
-
-    void on_bin() {
-      if (spec.flag(HASH_FLAG)) {
-        prefix[prefix_size++] = '0';
-        prefix[prefix_size++] = static_cast<char>(spec.type());
-      }
-      unsigned num_digits = count_digits<1>();
-      writer.write_int(num_digits, get_prefix(), spec,
-                       bin_writer<1>{abs_value, num_digits});
-    }
-
-    void on_oct() {
-      unsigned num_digits = count_digits<3>();
-      if (spec.flag(HASH_FLAG) &&
-          spec.precision() <= static_cast<int>(num_digits)) {
-        // Octal prefix '0' is counted as a digit, so only add it if precision
-        // is not greater than the number of digits.
-        prefix[prefix_size++] = '0';
-      }
-      writer.write_int(num_digits, get_prefix(), spec,
-                       bin_writer<3>{abs_value, num_digits});
-    }
-
-    enum { SEP_SIZE = 1 };
-
-    struct num_writer {
-      unsigned_type abs_value;
-      unsigned size;
-      char_type sep;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        basic_string_view<char_type> s(&sep, SEP_SIZE);
-        it = format_decimal(it, abs_value, size,
-                            internal::add_thousands_sep<char_type>(s));
-      }
-    };
-
-    void on_num() {
-      unsigned num_digits = internal::count_digits(abs_value);
-      char_type sep = internal::thousands_sep<char_type>(writer.locale_.get());
-      unsigned size = num_digits + SEP_SIZE * ((num_digits - 1) / 3);
-      writer.write_int(size, get_prefix(), spec,
-                       num_writer{abs_value, size, sep});
-    }
-
-    void on_error() {
-      FMT_THROW(format_error("invalid type specifier"));
-    }
-  };
-
-  // Writes a formatted integer.
-  template <typename T, typename Spec>
-  void write_int(T value, const Spec &spec) {
-    internal::handle_int_type_spec(spec.type(),
-                                   int_writer<T, Spec>(*this, value, spec));
-  }
-
-  enum {INF_SIZE = 3}; // This is an enum to workaround a bug in MSVC.
-
-  struct inf_or_nan_writer {
-    char sign;
-    const char *str;
-
-    template <typename It>
-    void operator()(It &&it) const {
-      if (sign)
-        *it++ = sign;
-      it = std::copy_n(str, static_cast<std::size_t>(INF_SIZE), it);
-    }
-  };
-
-  struct double_writer {
-    size_t n;
-    char sign;
-    basic_memory_buffer<char_type> &buffer;
-
-    template <typename It>
-    void operator()(It &&it) {
-      if (sign) {
-        *it++ = sign;
-        --n;
-      }
-      it = std::copy_n(buffer.begin(), n, it);
-    }
-  };
-
-  // Formats a floating-point number (double or long double).
-  template <typename T>
-  void write_double(T value, const format_specs &spec);
-  template <typename T>
-  void write_double_sprintf(T value, const format_specs &spec,
-                            internal::basic_buffer<char_type> &buffer);
-
-  template <typename Char>
-  struct str_writer {
-    const Char *s;
-    std::size_t size;
-
-    template <typename It>
-    void operator()(It &&it) const {
-      it = std::copy_n(s, size, it);
-    }
-  };
-
-  // Writes a formatted string.
-  template <typename Char>
-  void write_str(const Char *s, std::size_t size, const align_spec &spec) {
-    write_padded(size, spec, str_writer<Char>{s, size});
-  }
-
-  template <typename Char>
-  void write_str(basic_string_view<Char> str, const format_specs &spec);
-
-  // Appends floating-point length specifier to the format string.
-  // The second argument is only used for overload resolution.
-  void append_float_length(char_type *&format_ptr, long double) {
-    *format_ptr++ = 'L';
-  }
-
-  template<typename T>
-  void append_float_length(char_type *&, T) {}
-
-  template <typename Char>
-  friend class internal::arg_formatter_base;
-
- public:
-  /** Constructs a ``basic_writer`` object. */
-  explicit basic_writer(Range out): out_(out.begin()) {}
-
-  void write(int value) { write_decimal(value); }
-  void write(long value) { write_decimal(value); }
-  void write(long long value) { write_decimal(value); }
-
-  void write(unsigned value) { write_decimal(value); }
-  void write(unsigned long value) { write_decimal(value); }
-  void write(unsigned long long value) { write_decimal(value); }
-
-  /**
-    \rst
-    Formats *value* and writes it to the buffer.
-    \endrst
-   */
-  template <typename T, typename FormatSpec, typename... FormatSpecs>
-  typename std::enable_if<std::is_integral<T>::value, void>::type
-      write(T value, FormatSpec spec, FormatSpecs... specs) {
-    format_specs s(spec, specs...);
-    s.align_ = ALIGN_RIGHT;
-    write_int(value, s);
-  }
-
-  void write(double value) {
-    write_double(value, format_specs());
-  }
-
-  /**
-    \rst
-    Formats *value* using the general format for floating-point numbers
-    (``'g'``) and writes it to the buffer.
-    \endrst
-   */
-  void write(long double value) {
-    write_double(value, format_specs());
-  }
-
-  /** Writes a character to the buffer. */
-  void write(char value) {
-    *reserve(1) = value;
-  }
-  void write(wchar_t value) {
-    static_assert(std::is_same<char_type, wchar_t>::value, "");
-    *reserve(1) = value;
-  }
-
-  /**
-    \rst
-    Writes *value* to the buffer.
-    \endrst
-   */
-  void write(string_view value) {
-    auto &&it = reserve(value.size());
-    it = std::copy(value.begin(), value.end(), it);
-  }
-  void write(wstring_view value) {
-    static_assert(std::is_same<char_type, wchar_t>::value, "");
-    auto &&it = reserve(value.size());
-    it = std::copy(value.begin(), value.end(), it);
-  }
-
-  template <typename... FormatSpecs>
-  void write(basic_string_view<char_type> str, FormatSpecs... specs) {
-    write_str(str, format_specs(specs...));
-  }
-
-  template <typename T>
-  typename std::enable_if<std::is_same<T, void>::value>::type
-      write(const T *p) {
-    format_specs specs;
-    specs.flags_ = HASH_FLAG;
-    specs.type_ = 'x';
-    write_int(reinterpret_cast<uintptr_t>(p), specs);
-  }
-};
-
-template <typename Range>
-template <typename F>
-void basic_writer<Range>::write_padded(
-    std::size_t size, const align_spec &spec, F &&f) {
-  unsigned width = spec.width();
-  if (width <= size)
-    return f(reserve(size));
-  auto &&it = reserve(width);
-  char_type fill = static_cast<char_type>(spec.fill());
-  std::size_t padding = width - size;
-  if (spec.align() == ALIGN_RIGHT) {
-    it = std::fill_n(it, padding, fill);
-    f(it);
-  } else if (spec.align() == ALIGN_CENTER) {
-    std::size_t left_padding = padding / 2;
-    it = std::fill_n(it, left_padding, fill);
-    f(it);
-    it = std::fill_n(it, padding - left_padding, fill);
-  } else {
-    f(it);
-    it = std::fill_n(it, padding, fill);
-  }
-}
-
-template <typename Range>
-template <typename Char>
-void basic_writer<Range>::write_str(
-    basic_string_view<Char> s, const format_specs &spec) {
-  const Char *data = s.data();
-  std::size_t size = s.size();
-  std::size_t precision = static_cast<std::size_t>(spec.precision_);
-  if (spec.precision_ >= 0 && precision < size)
-    size = precision;
-  write_str(data, size, spec);
-}
-
-template <typename Char>
-struct float_spec_handler {
-  Char type;
-  bool upper;
-
-  explicit float_spec_handler(Char t) : type(t), upper(false) {}
-
-  void on_general() {
-    if (type == 'G')
-      upper = true;
-    else
-      type = 'g';
-  }
-
-  void on_exp() {
-    if (type == 'E')
-      upper = true;
-  }
-
-  void on_fixed() {
-    if (type == 'F') {
-      upper = true;
-#if FMT_MSC_VER
-      // MSVC's printf doesn't support 'F'.
-      type = 'f';
-#endif
-    }
-  }
-
-  void on_hex() {
-    if (type == 'A')
-      upper = true;
-  }
-
-  void on_error() {
-    FMT_THROW(format_error("invalid type specifier"));
-  }
-};
-
-template <typename Range>
-template <typename T>
-void basic_writer<Range>::write_double(T value, const format_specs &spec) {
-  // Check type.
-  float_spec_handler<char_type> handler(spec.type());
-  internal::handle_float_type_spec(spec.type(), handler);
-
-  char sign = 0;
-  // Use isnegative instead of value < 0 because the latter is always
-  // false for NaN.
-  if (internal::fputil::isnegative(static_cast<double>(value))) {
-    sign = '-';
-    value = -value;
-  } else if (spec.flag(SIGN_FLAG)) {
-    sign = spec.flag(PLUS_FLAG) ? '+' : ' ';
-  }
-
-  struct write_inf_or_nan_t {
-    basic_writer &writer;
-    format_specs spec;
-    char sign;
-    void operator()(const char *str) const {
-      writer.write_padded(INF_SIZE + (sign ? 1 : 0), spec,
-                          inf_or_nan_writer{sign, str});
-    }
-  } write_inf_or_nan = {*this, spec, sign};
-
-  // Format NaN and ininity ourselves because sprintf's output is not consistent
-  // across platforms.
-  if (internal::fputil::isnotanumber(value))
-    return write_inf_or_nan(handler.upper ? "NAN" : "nan");
-  if (internal::fputil::isinfinity(value))
-    return write_inf_or_nan(handler.upper ? "INF" : "inf");
-
-  basic_memory_buffer<char_type> buffer;
-  char type = static_cast<char>(spec.type());
-  if (internal::const_check(
-        internal::use_grisu() && sizeof(T) <= sizeof(double)) &&
-      type != 'a' && type != 'A') {
-    char buf[100]; // TODO: correct buffer size
-    size_t size = 0;
-    internal::grisu2_format(static_cast<double>(value), buf, size, type,
-                            spec.precision(), spec.flag(HASH_FLAG));
-    FMT_ASSERT(size <= 100, "buffer overflow");
-    buffer.append(buf, buf + size); // TODO: avoid extra copy
-  } else {
-    format_specs normalized_spec(spec);
-    normalized_spec.type_ = handler.type;
-    write_double_sprintf(value, normalized_spec, buffer);
-  }
-  size_t n = buffer.size();
-  align_spec as = spec;
-  if (spec.align() == ALIGN_NUMERIC) {
-    if (sign) {
-      auto &&it = reserve(1);
-      *it++ = sign;
-      sign = 0;
-      if (as.width_)
-        --as.width_;
-    }
-    as.align_ = ALIGN_RIGHT;
-  } else {
-    if (spec.align() == ALIGN_DEFAULT)
-      as.align_ = ALIGN_RIGHT;
-    if (sign)
-      ++n;
-  }
-  write_padded(n, as, double_writer{n, sign, buffer});
-}
-
-template <typename Range>
-template <typename T>
-void basic_writer<Range>::write_double_sprintf(
-    T value, const format_specs &spec,
-    internal::basic_buffer<char_type> &buffer) {
-  // Buffer capacity must be non-zero, otherwise MSVC's vsnprintf_s will fail.
-  FMT_ASSERT(buffer.capacity() != 0, "empty buffer");
-
-  // Build format string.
-  enum { MAX_FORMAT_SIZE = 10}; // longest format: %#-*.*Lg
-  char_type format[MAX_FORMAT_SIZE];
-  char_type *format_ptr = format;
-  *format_ptr++ = '%';
-  if (spec.flag(HASH_FLAG))
-    *format_ptr++ = '#';
-  if (spec.precision() >= 0) {
-    *format_ptr++ = '.';
-    *format_ptr++ = '*';
-  }
-
-  append_float_length(format_ptr, value);
-  *format_ptr++ = spec.type();
-  *format_ptr = '\0';
-
-  // Format using snprintf.
-  char_type *start = FMT_NULL;
-  for (;;) {
-    std::size_t buffer_size = buffer.capacity();
-    start = &buffer[0];
-    int result = internal::char_traits<char_type>::format_float(
-        start, buffer_size, format, spec.precision(), value);
-    if (result >= 0) {
-      unsigned n = internal::to_unsigned(result);
-      if (n < buffer.capacity()) {
-        buffer.resize(n);
-        break;  // The buffer is large enough - continue with formatting.
-      }
-      buffer.reserve(n + 1);
-    } else {
-      // If result is negative we ask to increase the capacity by at least 1,
-      // but as std::vector, the buffer grows exponentially.
-      buffer.reserve(buffer.capacity() + 1);
-    }
-  }
-}
+FMT_API void format_system_error(detail::buffer<char>& out, int error_code,
+                                 string_view message) FMT_NOEXCEPT;
 
 // Reports a system error without throwing an exception.
 // Can be used to report errors from destructors.
 FMT_API void report_system_error(int error_code,
                                  string_view message) FMT_NOEXCEPT;
 
-#if FMT_USE_WINDOWS_H
-
-/** A Windows error. */
-class windows_error : public system_error {
- private:
-  FMT_API void init(int error_code, string_view format_str, format_args args);
-
- public:
-  /**
-   \rst
-   Constructs a :class:`fmt::windows_error` object with the description
-   of the form
-
-   .. parsed-literal::
-     *<message>*: *<system-message>*
-
-   where *<message>* is the formatted message and *<system-message>* is the
-   system message corresponding to the error code.
-   *error_code* is a Windows error code as given by ``GetLastError``.
-   If *error_code* is not a valid error code such as -1, the system message
-   will look like "error -1".
-
-   **Example**::
-
-     // This throws a windows_error with the description
-     //   cannot open file 'madeup': The system cannot find the file specified.
-     // or similar (system message may vary).
-     const char *filename = "madeup";
-     LPOFSTRUCT of = LPOFSTRUCT();
-     HFILE file = OpenFile(filename, &of, OF_READ);
-     if (file == HFILE_ERROR) {
-       throw fmt::windows_error(GetLastError(),
-                                "cannot open file '{}'", filename);
-     }
-   \endrst
-  */
-  template <typename... Args>
-  windows_error(int error_code, string_view message, const Args &... args) {
-    init(error_code, message, make_format_args(args...));
-  }
-};
-
-// Reports a Windows error without throwing an exception.
-// Can be used to report errors from destructors.
-FMT_API void report_windows_error(int error_code,
-                                  string_view message) FMT_NOEXCEPT;
-
-#endif
-
 /** Fast integer formatter. */
 class format_int {
  private:
   // Buffer should be large enough to hold all digits (digits10 + 1),
   // a sign and a null character.
-  enum {BUFFER_SIZE = std::numeric_limits<unsigned long long>::digits10 + 3};
-  mutable char buffer_[BUFFER_SIZE];
-  char *str_;
-
-  // Formats value in reverse and returns a pointer to the beginning.
-  char *format_decimal(unsigned long long value) {
-    char *ptr = buffer_ + BUFFER_SIZE - 1;
-    while (value >= 100) {
-      // Integer division is slow so do it for a group of two digits instead
-      // of for every digit. The idea comes from the talk by Alexandrescu
-      // "Three Optimization Tips for C++". See speed-test for a comparison.
-      unsigned index = static_cast<unsigned>((value % 100) * 2);
-      value /= 100;
-      *--ptr = internal::data::DIGITS[index + 1];
-      *--ptr = internal::data::DIGITS[index];
-    }
-    if (value < 10) {
-      *--ptr = static_cast<char>('0' + value);
-      return ptr;
-    }
-    unsigned index = static_cast<unsigned>(value * 2);
-    *--ptr = internal::data::DIGITS[index + 1];
-    *--ptr = internal::data::DIGITS[index];
-    return ptr;
+  enum { buffer_size = std::numeric_limits<unsigned long long>::digits10 + 3 };
+  mutable char buffer_[buffer_size];
+  char* str_;
+
+  template <typename UInt> char* format_unsigned(UInt value) {
+    auto n = static_cast<detail::uint32_or_64_or_128_t<UInt>>(value);
+    return detail::format_decimal(buffer_, n, buffer_size - 1).begin;
   }
 
-  void format_signed(long long value) {
-    unsigned long long abs_value = static_cast<unsigned long long>(value);
+  template <typename Int> char* format_signed(Int value) {
+    auto abs_value = static_cast<detail::uint32_or_64_or_128_t<Int>>(value);
     bool negative = value < 0;
-    if (negative)
-      abs_value = 0 - abs_value;
-    str_ = format_decimal(abs_value);
-    if (negative)
-      *--str_ = '-';
+    if (negative) abs_value = 0 - abs_value;
+    auto begin = format_unsigned(abs_value);
+    if (negative) *--begin = '-';
+    return begin;
   }
 
  public:
-  explicit format_int(int value) { format_signed(value); }
-  explicit format_int(long value) { format_signed(value); }
-  explicit format_int(long long value) { format_signed(value); }
-  explicit format_int(unsigned value) : str_(format_decimal(value)) {}
-  explicit format_int(unsigned long value) : str_(format_decimal(value)) {}
-  explicit format_int(unsigned long long value) : str_(format_decimal(value)) {}
+  explicit format_int(int value) : str_(format_signed(value)) {}
+  explicit format_int(long value) : str_(format_signed(value)) {}
+  explicit format_int(long long value) : str_(format_signed(value)) {}
+  explicit format_int(unsigned value) : str_(format_unsigned(value)) {}
+  explicit format_int(unsigned long value) : str_(format_unsigned(value)) {}
+  explicit format_int(unsigned long long value)
+      : str_(format_unsigned(value)) {}
 
   /** Returns the number of characters written to the output buffer. */
-  std::size_t size() const {
-    return internal::to_unsigned(buffer_ - str_ + BUFFER_SIZE - 1);
+  size_t size() const {
+    return detail::to_unsigned(buffer_ - str_ + buffer_size - 1);
   }
 
   /**
     Returns a pointer to the output buffer content. No terminating null
     character is appended.
    */
-  const char *data() const { return str_; }
+  const char* data() const { return str_; }
 
   /**
     Returns a pointer to the output buffer content with terminating null
     character appended.
    */
-  const char *c_str() const {
-    buffer_[BUFFER_SIZE - 1] = '\0';
+  const char* c_str() const {
+    buffer_[buffer_size - 1] = '\0';
     return str_;
   }
 
   /**
     \rst
     Returns the content of the output buffer as an ``std::string``.
     \endrst
    */
   std::string str() const { return std::string(str_, size()); }
 };
 
-// Formats a decimal integer value writing into buffer and returns
-// a pointer to the end of the formatted string. This function doesn't
-// write a terminating null character.
-template <typename T>
-inline void format_decimal(char *&buffer, T value) {
-  typedef typename internal::int_traits<T>::main_type main_type;
-  main_type abs_value = static_cast<main_type>(value);
-  if (internal::is_negative(value)) {
-    *buffer++ = '-';
-    abs_value = 0 - abs_value;
-  }
-  if (abs_value < 100) {
-    if (abs_value < 10) {
-      *buffer++ = static_cast<char>('0' + abs_value);
-      return;
-    }
-    unsigned index = static_cast<unsigned>(abs_value * 2);
-    *buffer++ = internal::data::DIGITS[index];
-    *buffer++ = internal::data::DIGITS[index + 1];
-    return;
-  }
-  unsigned num_digits = internal::count_digits(abs_value);
-  internal::format_decimal(buffer, abs_value, num_digits);
-  buffer += num_digits;
-}
-
-// Formatter of objects of type T.
+// A formatter specialization for the core types corresponding to detail::type
+// constants.
 template <typename T, typename Char>
-struct formatter<
-    T, Char,
-    typename std::enable_if<internal::format_type<
-        typename buffer_context<Char>::type, T>::value>::type> {
+struct formatter<T, Char,
+                 enable_if_t<detail::type_constant<T, Char>::value !=
+                             detail::type::custom_type>> {
+  FMT_CONSTEXPR formatter() = default;
 
   // Parses format specifiers stopping either at the end of the range or at the
   // terminating '}'.
   template <typename ParseContext>
-  FMT_CONSTEXPR typename ParseContext::iterator parse(ParseContext &ctx) {
-    auto it = internal::null_terminating_iterator<Char>(ctx);
-    typedef internal::dynamic_specs_handler<ParseContext> handler_type;
-    auto type = internal::get_type<
-      typename buffer_context<Char>::type, T>::value;
-    internal::specs_checker<handler_type>
-        handler(handler_type(specs_, ctx), type);
-    it = parse_format_specs(it, handler);
-    auto type_spec = specs_.type();
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    using handler_type = detail::dynamic_specs_handler<ParseContext>;
+    auto type = detail::type_constant<T, Char>::value;
+    detail::specs_checker<handler_type> handler(handler_type(specs_, ctx),
+                                                type);
+    auto it = parse_format_specs(ctx.begin(), ctx.end(), handler);
     auto eh = ctx.error_handler();
     switch (type) {
-    case internal::none_type:
-    case internal::named_arg_type:
+    case detail::type::none_type:
       FMT_ASSERT(false, "invalid argument type");
       break;
-    case internal::int_type:
-    case internal::uint_type:
-    case internal::long_long_type:
-    case internal::ulong_long_type:
-    case internal::bool_type:
-      handle_int_type_spec(
-            type_spec, internal::int_type_checker<decltype(eh)>(eh));
+    case detail::type::int_type:
+    case detail::type::uint_type:
+    case detail::type::long_long_type:
+    case detail::type::ulong_long_type:
+    case detail::type::int128_type:
+    case detail::type::uint128_type:
+    case detail::type::bool_type:
+      handle_int_type_spec(specs_.type,
+                           detail::int_type_checker<decltype(eh)>(eh));
       break;
-    case internal::char_type:
+    case detail::type::char_type:
       handle_char_specs(
-          &specs_,
-          internal::char_specs_checker<decltype(eh), decltype(type_spec)>(
-              type_spec, eh));
-      break;
-    case internal::double_type:
-    case internal::long_double_type:
-      handle_float_type_spec(
-            type_spec, internal::float_type_checker<decltype(eh)>(eh));
-      break;
-    case internal::cstring_type:
-      internal::handle_cstring_type_spec(
-            type_spec, internal::cstring_type_checker<decltype(eh)>(eh));
+          &specs_, detail::char_specs_checker<decltype(eh)>(specs_.type, eh));
+      break;
+    case detail::type::float_type:
+      if (detail::const_check(FMT_USE_FLOAT))
+        detail::parse_float_type_spec(specs_, eh);
+      else
+        FMT_ASSERT(false, "float support disabled");
       break;
-    case internal::string_type:
-      internal::check_string_type_spec(type_spec, eh);
+    case detail::type::double_type:
+      if (detail::const_check(FMT_USE_DOUBLE))
+        detail::parse_float_type_spec(specs_, eh);
+      else
+        FMT_ASSERT(false, "double support disabled");
+      break;
+    case detail::type::long_double_type:
+      if (detail::const_check(FMT_USE_LONG_DOUBLE))
+        detail::parse_float_type_spec(specs_, eh);
+      else
+        FMT_ASSERT(false, "long double support disabled");
+      break;
+    case detail::type::cstring_type:
+      detail::handle_cstring_type_spec(
+          specs_.type, detail::cstring_type_checker<decltype(eh)>(eh));
+      break;
+    case detail::type::string_type:
+      detail::check_string_type_spec(specs_.type, eh);
       break;
-    case internal::pointer_type:
-      internal::check_pointer_type_spec(type_spec, eh);
+    case detail::type::pointer_type:
+      detail::check_pointer_type_spec(specs_.type, eh);
       break;
-    case internal::custom_type:
+    case detail::type::custom_type:
       // Custom format specifiers should be checked in parse functions of
       // formatter specializations.
       break;
     }
-    return pointer_from(it);
+    return it;
   }
 
   template <typename FormatContext>
-  auto format(const T &val, FormatContext &ctx) -> decltype(ctx.out()) {
-    internal::handle_dynamic_spec<internal::width_checker>(
-      specs_.width_, specs_.width_ref, ctx);
-    internal::handle_dynamic_spec<internal::precision_checker>(
-      specs_.precision_, specs_.precision_ref, ctx);
-    typedef output_range<typename FormatContext::iterator,
-                         typename FormatContext::char_type> range_type;
-    return fmt::visit(arg_formatter<range_type>(ctx, &specs_),
-                      internal::make_arg<FormatContext>(val));
+  auto format(const T& val, FormatContext& ctx) -> decltype(ctx.out()) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+    using af = detail::arg_formatter<typename FormatContext::iterator,
+                                     typename FormatContext::char_type>;
+    return visit_format_arg(af(ctx, nullptr, &specs_),
+                            detail::make_arg<FormatContext>(val));
   }
 
  private:
-  internal::dynamic_format_specs<Char> specs_;
+  detail::dynamic_format_specs<Char> specs_;
+};
+
+#define FMT_FORMAT_AS(Type, Base)                                             \
+  template <typename Char>                                                    \
+  struct formatter<Type, Char> : formatter<Base, Char> {                      \
+    template <typename FormatContext>                                         \
+    auto format(Type const& val, FormatContext& ctx) -> decltype(ctx.out()) { \
+      return formatter<Base, Char>::format(val, ctx);                         \
+    }                                                                         \
+  }
+
+FMT_FORMAT_AS(signed char, int);
+FMT_FORMAT_AS(unsigned char, unsigned);
+FMT_FORMAT_AS(short, int);
+FMT_FORMAT_AS(unsigned short, unsigned);
+FMT_FORMAT_AS(long, long long);
+FMT_FORMAT_AS(unsigned long, unsigned long long);
+FMT_FORMAT_AS(Char*, const Char*);
+FMT_FORMAT_AS(std::basic_string<Char>, basic_string_view<Char>);
+FMT_FORMAT_AS(std::nullptr_t, const void*);
+FMT_FORMAT_AS(detail::std_string_view<Char>, basic_string_view<Char>);
+
+template <typename Char>
+struct formatter<void*, Char> : formatter<const void*, Char> {
+  template <typename FormatContext>
+  auto format(void* val, FormatContext& ctx) -> decltype(ctx.out()) {
+    return formatter<const void*, Char>::format(val, ctx);
+  }
+};
+
+template <typename Char, size_t N>
+struct formatter<Char[N], Char> : formatter<basic_string_view<Char>, Char> {
+  template <typename FormatContext>
+  auto format(const Char* val, FormatContext& ctx) -> decltype(ctx.out()) {
+    return formatter<basic_string_view<Char>, Char>::format(val, ctx);
+  }
 };
 
 // A formatter for types known only at run time such as variant alternatives.
 //
 // Usage:
-//   typedef std::variant<int, std::string> variant;
+//   using variant = std::variant<int, std::string>;
 //   template <>
 //   struct formatter<variant>: dynamic_formatter<> {
-//     void format(buffer &buf, const variant &v, context &ctx) {
-//       visit([&](const auto &val) { format(buf, val, ctx); }, v);
+//     auto format(const variant& v, format_context& ctx) {
+//       return visit([&](const auto& val) {
+//           return dynamic_formatter<>::format(val, ctx);
+//       }, v);
 //     }
 //   };
-template <typename Char = char>
-class dynamic_formatter {
+template <typename Char = char> class dynamic_formatter {
  private:
-  struct null_handler: internal::error_handler {
-    void on_align(alignment) {}
+  struct null_handler : detail::error_handler {
+    void on_align(align_t) {}
     void on_plus() {}
     void on_minus() {}
     void on_space() {}
     void on_hash() {}
   };
 
  public:
   template <typename ParseContext>
-  auto parse(ParseContext &ctx) -> decltype(ctx.begin()) {
-    auto it = internal::null_terminating_iterator<Char>(ctx);
+  auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    format_str_ = ctx.begin();
     // Checks are deferred to formatting time when the argument type is known.
-    internal::dynamic_specs_handler<ParseContext> handler(specs_, ctx);
-    it = parse_format_specs(it, handler);
-    return pointer_from(it);
+    detail::dynamic_specs_handler<ParseContext> handler(specs_, ctx);
+    return parse_format_specs(ctx.begin(), ctx.end(), handler);
   }
 
   template <typename T, typename FormatContext>
-  auto format(const T &val, FormatContext &ctx) -> decltype(ctx.out()) {
+  auto format(const T& val, FormatContext& ctx) -> decltype(ctx.out()) {
     handle_specs(ctx);
-    internal::specs_checker<null_handler>
-        checker(null_handler(), internal::get_type<FormatContext, T>::value);
-    checker.on_align(specs_.align());
-    if (specs_.flags_ == 0) {
-      // Do nothing.
-    } else if (specs_.flag(SIGN_FLAG)) {
-      if (specs_.flag(PLUS_FLAG))
-        checker.on_plus();
-      else
-        checker.on_space();
-    } else if (specs_.flag(MINUS_FLAG)) {
+    detail::specs_checker<null_handler> checker(
+        null_handler(), detail::mapped_type_constant<T, FormatContext>::value);
+    checker.on_align(specs_.align);
+    switch (specs_.sign) {
+    case sign::none:
+      break;
+    case sign::plus:
+      checker.on_plus();
+      break;
+    case sign::minus:
       checker.on_minus();
-    } else if (specs_.flag(HASH_FLAG)) {
-      checker.on_hash();
+      break;
+    case sign::space:
+      checker.on_space();
+      break;
     }
-    if (specs_.precision_ != -1)
-      checker.end_precision();
-    typedef output_range<typename FormatContext::iterator,
-                         typename FormatContext::char_type> range;
-    fmt::visit(arg_formatter<range>(ctx, &specs_),
-               internal::make_arg<FormatContext>(val));
+    if (specs_.alt) checker.on_hash();
+    if (specs_.precision >= 0) checker.end_precision();
+    using af = detail::arg_formatter<typename FormatContext::iterator,
+                                     typename FormatContext::char_type>;
+    visit_format_arg(af(ctx, nullptr, &specs_),
+                     detail::make_arg<FormatContext>(val));
     return ctx.out();
   }
 
  private:
-  template <typename Context>
-  void handle_specs(Context &ctx) {
-    internal::handle_dynamic_spec<internal::width_checker>(
-      specs_.width_, specs_.width_ref, ctx);
-    internal::handle_dynamic_spec<internal::precision_checker>(
-      specs_.precision_, specs_.precision_ref, ctx);
-  }
-
-  internal::dynamic_format_specs<Char> specs_;
-};
-
-template <typename Range, typename Char>
-typename basic_format_context<Range, Char>::format_arg
-  basic_format_context<Range, Char>::get_arg(
-    basic_string_view<char_type> name) {
-  map_.init(this->args());
-  format_arg arg = map_.find(name);
-  if (arg.type() == internal::none_type)
-    this->on_error("argument not found");
-  return arg;
+  template <typename Context> void handle_specs(Context& ctx) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+  }
+
+  detail::dynamic_format_specs<Char> specs_;
+  const Char* format_str_;
+};
+
+template <typename Char, typename ErrorHandler>
+FMT_CONSTEXPR void advance_to(
+    basic_format_parse_context<Char, ErrorHandler>& ctx, const Char* p) {
+  ctx.advance_to(ctx.begin() + (p - &*ctx.begin()));
+}
+
+/**
+  \rst
+  Converts ``p`` to ``const void*`` for pointer formatting.
+
+  **Example**::
+
+    auto s = fmt::format("{}", fmt::ptr(p));
+  \endrst
+ */
+template <typename T> inline const void* ptr(const T* p) { return p; }
+template <typename T> inline const void* ptr(const std::unique_ptr<T>& p) {
+  return p.get();
 }
+template <typename T> inline const void* ptr(const std::shared_ptr<T>& p) {
+  return p.get();
+}
+
+class bytes {
+ private:
+  string_view data_;
+  friend struct formatter<bytes>;
 
-template <typename ArgFormatter, typename Char, typename Context>
-struct format_handler : internal::error_handler {
-  typedef internal::null_terminating_iterator<Char> iterator;
-  typedef typename ArgFormatter::range range;
-
-  format_handler(range r, basic_string_view<Char> str,
-                 basic_format_args<Context> format_args)
-    : context(r.begin(), str, format_args) {}
+ public:
+  explicit bytes(string_view data) : data_(data) {}
+};
 
-  void on_text(const Char *begin, const Char *end) {
-    auto size = internal::to_unsigned(end - begin);
-    auto out = context.out();
-    auto &&it = internal::reserve(out, size);
-    it = std::copy_n(begin, size, it);
-    context.advance_to(out);
-  }
+template <> struct formatter<bytes> {
+ private:
+  detail::dynamic_format_specs<char> specs_;
 
-  void on_arg_id() { arg = context.next_arg(); }
-  void on_arg_id(unsigned id) {
-    context.parse_context().check_arg_id(id);
-    arg = context.get_arg(id);
-  }
-  void on_arg_id(basic_string_view<Char> id) {
-    arg = context.get_arg(id);
-  }
-
-  void on_replacement_field(const Char *p) {
-    context.parse_context().advance_to(p);
-    if (!fmt::visit(internal::custom_formatter<Char, Context>(context), arg))
-      context.advance_to(fmt::visit(ArgFormatter(context), arg));
-  }
-
-  iterator on_format_specs(iterator it) {
-    auto &parse_ctx = context.parse_context();
-    parse_ctx.advance_to(pointer_from(it));
-    if (fmt::visit(internal::custom_formatter<Char, Context>(context), arg))
-      return iterator(parse_ctx);
-    basic_format_specs<Char> specs;
-    using internal::specs_handler;
-    internal::specs_checker<specs_handler<Context>>
-        handler(specs_handler<Context>(specs, context), arg.type());
-    it = parse_format_specs(it, handler);
-    if (*it != '}')
-      on_error("missing '}' in format string");
-    parse_ctx.advance_to(pointer_from(it));
-    context.advance_to(fmt::visit(ArgFormatter(context, &specs), arg));
+ public:
+  template <typename ParseContext>
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    using handler_type = detail::dynamic_specs_handler<ParseContext>;
+    detail::specs_checker<handler_type> handler(handler_type(specs_, ctx),
+                                                detail::type::string_type);
+    auto it = parse_format_specs(ctx.begin(), ctx.end(), handler);
+    detail::check_string_type_spec(specs_.type, ctx.error_handler());
     return it;
   }
 
-  Context context;
-  basic_format_arg<Context> arg;
+  template <typename FormatContext>
+  auto format(bytes b, FormatContext& ctx) -> decltype(ctx.out()) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+    return detail::write_bytes(ctx.out(), b.data_, specs_);
+  }
 };
 
-/** Formats arguments and writes the output to the range. */
-template <typename ArgFormatter, typename Char, typename Context>
-typename Context::iterator vformat_to(typename ArgFormatter::range out,
-                                      basic_string_view<Char> format_str,
-                                      basic_format_args<Context> args) {
-  format_handler<ArgFormatter, Char, Context> h(out, format_str, args);
-  internal::parse_format_string<false>(format_str, h);
-  return h.context.out();
-}
-
-// Casts ``p`` to ``const void*`` for pointer formatting.
-// Example:
-//   auto s = format("{}", ptr(p));
-template <typename T>
-inline const void *ptr(const T *p) { return p; }
-
-template <typename It, typename Char>
-struct arg_join {
+template <typename It, typename Sentinel, typename Char>
+struct arg_join : detail::view {
   It begin;
-  It end;
+  Sentinel end;
   basic_string_view<Char> sep;
 
-  arg_join(It begin, It end, basic_string_view<Char> sep)
-    : begin(begin), end(end), sep(sep) {}
+  arg_join(It b, Sentinel e, basic_string_view<Char> s)
+      : begin(b), end(e), sep(s) {}
 };
 
-template <typename It, typename Char>
-struct formatter<arg_join<It, Char>, Char>:
-    formatter<typename std::iterator_traits<It>::value_type, Char> {
+template <typename It, typename Sentinel, typename Char>
+struct formatter<arg_join<It, Sentinel, Char>, Char>
+    : formatter<typename std::iterator_traits<It>::value_type, Char> {
   template <typename FormatContext>
-  auto format(const arg_join<It, Char> &value, FormatContext &ctx)
+  auto format(const arg_join<It, Sentinel, Char>& value, FormatContext& ctx)
       -> decltype(ctx.out()) {
-    typedef formatter<typename std::iterator_traits<It>::value_type, Char> base;
+    using base = formatter<typename std::iterator_traits<It>::value_type, Char>;
     auto it = value.begin;
     auto out = ctx.out();
     if (it != value.end) {
       out = base::format(*it++, ctx);
       while (it != value.end) {
         out = std::copy(value.sep.begin(), value.sep.end(), out);
         ctx.advance_to(out);
         out = base::format(*it++, ctx);
       }
     }
     return out;
   }
 };
 
-template <typename It>
-arg_join<It, char> join(It begin, It end, string_view sep) {
-  return arg_join<It, char>(begin, end, sep);
+/**
+  Returns an object that formats the iterator range `[begin, end)` with elements
+  separated by `sep`.
+ */
+template <typename It, typename Sentinel>
+arg_join<It, Sentinel, char> join(It begin, Sentinel end, string_view sep) {
+  return {begin, end, sep};
 }
 
-template <typename It>
-arg_join<It, wchar_t> join(It begin, It end, wstring_view sep) {
-  return arg_join<It, wchar_t>(begin, end, sep);
+template <typename It, typename Sentinel>
+arg_join<It, Sentinel, wchar_t> join(It begin, Sentinel end, wstring_view sep) {
+  return {begin, end, sep};
 }
 
-// The following causes ICE in gcc 4.4.
-#if FMT_USE_TRAILING_RETURN && (!FMT_GCC_VERSION || FMT_GCC_VERSION >= 405)
+/**
+  \rst
+  Returns an object that formats `range` with elements separated by `sep`.
+
+  **Example**::
+
+    std::vector<int> v = {1, 2, 3};
+    fmt::print("{}", fmt::join(v, ", "));
+    // Output: "1, 2, 3"
+
+  ``fmt::join`` applies passed format specifiers to the range elements::
+
+    fmt::print("{:02}", fmt::join(v, ", "));
+    // Output: "01, 02, 03"
+  \endrst
+ */
 template <typename Range>
-auto join(const Range &range, string_view sep)
-    -> arg_join<decltype(internal::begin(range)), char> {
-  return join(internal::begin(range), internal::end(range), sep);
+arg_join<detail::iterator_t<Range>, detail::sentinel_t<Range>, char> join(
+    Range&& range, string_view sep) {
+  return join(std::begin(range), std::end(range), sep);
 }
 
 template <typename Range>
-auto join(const Range &range, wstring_view sep)
-    -> arg_join<decltype(internal::begin(range)), wchar_t> {
-  return join(internal::begin(range), internal::end(range), sep);
+arg_join<detail::iterator_t<Range>, detail::sentinel_t<Range>, wchar_t> join(
+    Range&& range, wstring_view sep) {
+  return join(std::begin(range), std::end(range), sep);
 }
-#endif
 
 /**
   \rst
   Converts *value* to ``std::string`` using the default format for type *T*.
-  It doesn't support user-defined types with custom formatters.
 
   **Example**::
 
     #include <fmt/format.h>
 
     std::string answer = fmt::to_string(42);
   \endrst
  */
-template <typename T>
-std::string to_string(const T &value) {
-  std::string str;
-  internal::container_buffer<std::string> buf(str);
-  writer(buf).write(value);
-  return str;
+template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+inline std::string to_string(const T& value) {
+  std::string result;
+  detail::write<char>(std::back_inserter(result), value);
+  return result;
+}
+
+template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+inline std::string to_string(T value) {
+  // The buffer should be large enough to store the number including the sign or
+  // "false" for bool.
+  constexpr int max_size = detail::digits10<T>() + 2;
+  char buffer[max_size > 5 ? static_cast<unsigned>(max_size) : 5];
+  char* begin = buffer;
+  return std::string(begin, detail::write<char>(begin, value));
 }
 
 /**
   Converts *value* to ``std::wstring`` using the default format for type *T*.
  */
-template <typename T>
-std::wstring to_wstring(const T &value) {
-  std::wstring str;
-  internal::container_buffer<std::wstring> buf(str);
-  wwriter(buf).write(value);
-  return str;
-}
-
-template <typename Char, std::size_t SIZE>
-std::basic_string<Char> to_string(const basic_memory_buffer<Char, SIZE> &buf) {
-  return std::basic_string<Char>(buf.data(), buf.size());
-}
-
-inline format_context::iterator vformat_to(
-    internal::buffer &buf, string_view format_str, format_args args) {
-  typedef back_insert_range<internal::buffer> range;
-  return vformat_to<arg_formatter<range>>(buf, format_str, args);
-}
-
-inline wformat_context::iterator vformat_to(
-    internal::wbuffer &buf, wstring_view format_str, wformat_args args) {
-  typedef back_insert_range<internal::wbuffer> range;
-  return vformat_to<arg_formatter<range>>(buf, format_str, args);
-}
-
-template <
-    typename String, typename... Args,
-    std::size_t SIZE = inline_buffer_size,
-    typename Char = typename internal::format_string_traits<String>::char_type>
-inline typename buffer_context<Char>::type::iterator format_to(
-    basic_memory_buffer<Char, SIZE> &buf, const String &format_str,
-    const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  return vformat_to(
-        buf, basic_string_view<Char>(format_str),
-        make_format_args<typename buffer_context<Char>::type>(args...));
+template <typename T> inline std::wstring to_wstring(const T& value) {
+  return format(L"{}", value);
 }
 
-template <typename OutputIt, typename Char = char>
-//using format_context_t = basic_format_context<OutputIt, Char>;
-struct format_context_t { typedef basic_format_context<OutputIt, Char> type; };
-
-template <typename OutputIt, typename Char = char>
-//using format_args_t = basic_format_args<format_context_t<OutputIt, Char>>;
-struct format_args_t {
-  typedef basic_format_args<
-    typename format_context_t<OutputIt, Char>::type> type;
-};
-
-template <typename OutputIt, typename... Args>
-inline OutputIt vformat_to(OutputIt out, string_view format_str,
-                           typename format_args_t<OutputIt>::type args) {
-  typedef output_range<OutputIt, char> range;
-  return vformat_to<arg_formatter<range>>(range(out), format_str, args);
-}
-template <typename OutputIt, typename... Args>
-inline OutputIt vformat_to(
-    OutputIt out, wstring_view format_str,
-    typename format_args_t<OutputIt, wchar_t>::type args) {
-  typedef output_range<OutputIt, wchar_t> range;
-  return vformat_to<arg_formatter<range>>(range(out), format_str, args);
+template <typename Char, size_t SIZE>
+std::basic_string<Char> to_string(const basic_memory_buffer<Char, SIZE>& buf) {
+  auto size = buf.size();
+  detail::assume(size < std::basic_string<Char>().max_size());
+  return std::basic_string<Char>(buf.data(), size);
 }
 
-/**
- \rst
- Formats arguments, writes the result to the output iterator ``out`` and returns
- the iterator past the end of the output range.
-
- **Example**::
-
-   std::vector<char> out;
-   fmt::format_to(std::back_inserter(out), "{}", 42);
- \endrst
- */
-template <typename OutputIt, typename String, typename... Args>
-inline typename std::enable_if<internal::is_format_string<String>::value, OutputIt>::type
-  format_to(OutputIt out, const String &format_str,
-                          const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef typename format_context_t<OutputIt, FMT_CHAR(String) >::type context_t;
-  format_arg_store<context_t, Args...> as{args...};
-  return vformat_to(out, basic_string_view< FMT_CHAR(String) >(format_str),
-                    basic_format_args<context_t>(as));
+template <typename Char>
+void detail::vformat_to(
+    detail::buffer<Char>& buf, basic_string_view<Char> format_str,
+    basic_format_args<buffer_context<type_identity_t<Char>>> args,
+    detail::locale_ref loc) {
+  using iterator = typename buffer_context<Char>::iterator;
+  auto out = buffer_appender<Char>(buf);
+  if (format_str.size() == 2 && equal2(format_str.data(), "{}")) {
+    auto arg = args.get(0);
+    if (!arg) error_handler().on_error("argument not found");
+    visit_format_arg(default_arg_formatter<iterator, Char>{out, args, loc},
+                     arg);
+    return;
+  }
+  format_handler<iterator, Char, buffer_context<Char>> h(out, format_str, args,
+                                                         loc);
+  parse_format_string<false>(format_str, h);
+}
+
+#ifndef FMT_HEADER_ONLY
+extern template void detail::vformat_to(detail::buffer<char>&, string_view,
+                                        basic_format_args<format_context>,
+                                        detail::locale_ref);
+namespace detail {
+
+extern template FMT_API std::string grouping_impl<char>(locale_ref loc);
+extern template FMT_API std::string grouping_impl<wchar_t>(locale_ref loc);
+extern template FMT_API char thousands_sep_impl<char>(locale_ref loc);
+extern template FMT_API wchar_t thousands_sep_impl<wchar_t>(locale_ref loc);
+extern template FMT_API char decimal_point_impl(locale_ref loc);
+extern template FMT_API wchar_t decimal_point_impl(locale_ref loc);
+extern template int format_float<double>(double value, int precision,
+                                         float_specs specs, buffer<char>& buf);
+extern template int format_float<long double>(long double value, int precision,
+                                              float_specs specs,
+                                              buffer<char>& buf);
+int snprintf_float(float value, int precision, float_specs specs,
+                   buffer<char>& buf) = delete;
+extern template int snprintf_float<double>(double value, int precision,
+                                           float_specs specs,
+                                           buffer<char>& buf);
+extern template int snprintf_float<long double>(long double value,
+                                                int precision,
+                                                float_specs specs,
+                                                buffer<char>& buf);
+}  // namespace detail
+#endif
+
+template <typename S, typename Char = char_t<S>,
+          FMT_ENABLE_IF(detail::is_string<S>::value)>
+inline void vformat_to(
+    detail::buffer<Char>& buf, const S& format_str,
+    basic_format_args<FMT_BUFFER_CONTEXT(type_identity_t<Char>)> args) {
+  return detail::vformat_to(buf, to_string_view(format_str), args);
+}
+
+template <typename S, typename... Args, size_t SIZE = inline_buffer_size,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+inline typename buffer_context<Char>::iterator format_to(
+    basic_memory_buffer<Char, SIZE>& buf, const S& format_str, Args&&... args) {
+  const auto& vargs = fmt::make_args_checked<Args...>(format_str, args...);
+  detail::vformat_to(buf, to_string_view(format_str), vargs);
+  return detail::buffer_appender<Char>(buf);
 }
 
-template <typename OutputIt>
-struct format_to_n_result {
-  /** Iterator past the end of the output range. */
-  OutputIt out;
-  /** Total (not truncated) output size. */
-  std::size_t size;
-};
-
-template <typename OutputIt>
-using format_to_n_context = typename fmt::format_context_t<
-  fmt::internal::truncating_iterator<OutputIt>>::type;
+template <typename OutputIt, typename Char = char>
+using format_context_t = basic_format_context<OutputIt, Char>;
 
-template <typename OutputIt>
-using format_to_n_args = fmt::basic_format_args<format_to_n_context<OutputIt>>;
+template <typename OutputIt, typename Char = char>
+using format_args_t = basic_format_args<format_context_t<OutputIt, Char>>;
 
-template <typename OutputIt, typename ...Args>
-inline format_arg_store<format_to_n_context<OutputIt>, Args...>
-    make_format_to_n_args(const Args &... args) {
-  return format_arg_store<format_to_n_context<OutputIt>, Args...>(args...);
-}
+template <typename OutputIt, typename Char = typename OutputIt::value_type>
+using format_to_n_context FMT_DEPRECATED_ALIAS = buffer_context<Char>;
 
-template <typename OutputIt, typename... Args>
-inline format_to_n_result<OutputIt> vformat_to_n(
-    OutputIt out, std::size_t n, string_view format_str,
-    format_to_n_args<OutputIt> args) {
-  typedef internal::truncating_iterator<OutputIt> It;
-  auto it = vformat_to(It(out, n), format_str, args);
-  return {it.base(), it.count()};
-}
+template <typename OutputIt, typename Char = typename OutputIt::value_type>
+using format_to_n_args FMT_DEPRECATED_ALIAS =
+    basic_format_args<buffer_context<Char>>;
 
-/**
- \rst
- Formats arguments, writes up to ``n`` characters of the result to the output
- iterator ``out`` and returns the total output size and the iterator past the
- end of the output range.
- \endrst
- */
-template <typename OutputIt, typename... Args>
-inline format_to_n_result<OutputIt> format_to_n(
-    OutputIt out, std::size_t n, string_view format_str, const Args &... args) {
-  return vformat_to_n<OutputIt>(
-    out, n, format_str, make_format_to_n_args<OutputIt>(args...));
-}
-template <typename OutputIt, typename... Args>
-inline format_to_n_result<OutputIt> format_to_n(
-    OutputIt out, std::size_t n, wstring_view format_str,
-    const Args &... args) {
-  typedef internal::truncating_iterator<OutputIt> It;
-  auto it = vformat_to(It(out, n), format_str,
-      make_format_args<typename format_context_t<It, wchar_t>::type>(args...));
-  return {it.base(), it.count()};
+template <typename OutputIt, typename Char, typename... Args>
+FMT_DEPRECATED format_arg_store<buffer_context<Char>, Args...>
+make_format_to_n_args(const Args&... args) {
+  return format_arg_store<buffer_context<Char>, Args...>(args...);
 }
 
-template <typename Char>
-inline std::basic_string<Char> internal::vformat(
+template <typename Char, enable_if_t<(!std::is_same<Char, char>::value), int>>
+std::basic_string<Char> detail::vformat(
     basic_string_view<Char> format_str,
-    basic_format_args<typename buffer_context<Char>::type> args) {
+    basic_format_args<buffer_context<type_identity_t<Char>>> args) {
   basic_memory_buffer<Char> buffer;
-  vformat_to(buffer, format_str, args);
-  return fmt::to_string(buffer);
-}
-
-template <typename String, typename... Args>
-inline typename std::enable_if<internal::is_compile_string<String>::value>::type
-    print(String format_str, const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  return vprint(format_str.data(), make_format_args(args...));
+  detail::vformat_to(buffer, format_str, args);
+  return to_string(buffer);
 }
 
-/**
-  Returns the number of characters in the output of
-  ``format(format_str, args...)``.
- */
-template <typename... Args>
-inline std::size_t formatted_size(string_view format_str,
-                                  const Args &... args) {
-  auto it = format_to(internal::counting_iterator<char>(), format_str, args...);
-  return it.count();
+template <typename Char, FMT_ENABLE_IF(std::is_same<Char, wchar_t>::value)>
+void vprint(std::FILE* f, basic_string_view<Char> format_str,
+            wformat_args args) {
+  wmemory_buffer buffer;
+  detail::vformat_to(buffer, format_str, args);
+  buffer.push_back(L'\0');
+  if (std::fputws(buffer.data(), f) == -1)
+    FMT_THROW(system_error(errno, "cannot write to file"));
+}
+
+template <typename Char, FMT_ENABLE_IF(std::is_same<Char, wchar_t>::value)>
+void vprint(basic_string_view<Char> format_str, wformat_args args) {
+  vprint(stdout, format_str, args);
 }
 
 #if FMT_USE_USER_DEFINED_LITERALS
-namespace internal {
+namespace detail {
 
-# if FMT_UDL_TEMPLATE
-template <typename Char, Char... CHARS>
-class udl_formatter {
+#  if FMT_USE_UDL_TEMPLATE
+template <typename Char, Char... CHARS> class udl_formatter {
  public:
   template <typename... Args>
-  std::basic_string<Char> operator()(const Args &... args) const {
-    FMT_CONSTEXPR_DECL Char s[] = {CHARS..., '\0'};
-    FMT_CONSTEXPR_DECL bool invalid_format =
-        check_format_string<Char, error_handler, Args...>(
-          basic_string_view<Char>(s, sizeof...(CHARS)));
-    (void)invalid_format;
-    return format(s, args...);
+  std::basic_string<Char> operator()(Args&&... args) const {
+    static FMT_CONSTEXPR_DECL Char s[] = {CHARS..., '\0'};
+    return format(FMT_STRING(s), std::forward<Args>(args)...);
   }
 };
-# else
-template <typename Char>
-struct udl_formatter {
-  const Char *str;
+#  else
+template <typename Char> struct udl_formatter {
+  basic_string_view<Char> str;
 
   template <typename... Args>
-  auto operator()(Args &&... args) const
-                  -> decltype(format(str, std::forward<Args>(args)...)) {
+  std::basic_string<Char> operator()(Args&&... args) const {
     return format(str, std::forward<Args>(args)...);
   }
 };
-# endif // FMT_UDL_TEMPLATE
+#  endif  // FMT_USE_UDL_TEMPLATE
 
-template <typename Char>
-struct udl_arg {
-  const Char *str;
+template <typename Char> struct udl_arg {
+  const Char* str;
 
-  template <typename T>
-  named_arg<T, Char> operator=(T &&value) const {
+  template <typename T> named_arg<Char, T> operator=(T&& value) const {
     return {str, std::forward<T>(value)};
   }
 };
-
-} // namespace internal
+}  // namespace detail
 
 inline namespace literals {
-
-# if FMT_UDL_TEMPLATE
+#  if FMT_USE_UDL_TEMPLATE
+#    pragma GCC diagnostic push
+#    pragma GCC diagnostic ignored "-Wpedantic"
+#    if FMT_CLANG_VERSION
+#      pragma GCC diagnostic ignored "-Wgnu-string-literal-operator-template"
+#    endif
 template <typename Char, Char... CHARS>
-FMT_CONSTEXPR internal::udl_formatter<Char, CHARS...> operator""_format() {
+FMT_CONSTEXPR detail::udl_formatter<Char, CHARS...> operator""_format() {
   return {};
 }
-# else
+#    pragma GCC diagnostic pop
+#  else
 /**
   \rst
   User-defined literal equivalent of :func:`fmt::format`.
 
   **Example**::
 
     using namespace fmt::literals;
     std::string message = "The answer is {}"_format(42);
   \endrst
  */
-inline internal::udl_formatter<char>
-operator"" _format(const char *s, std::size_t) { return {s}; }
-inline internal::udl_formatter<wchar_t>
-operator"" _format(const wchar_t *s, std::size_t) { return {s}; }
-# endif // FMT_UDL_TEMPLATE
+FMT_CONSTEXPR detail::udl_formatter<char> operator"" _format(const char* s,
+                                                             size_t n) {
+  return {{s, n}};
+}
+FMT_CONSTEXPR detail::udl_formatter<wchar_t> operator"" _format(
+    const wchar_t* s, size_t n) {
+  return {{s, n}};
+}
+#  endif  // FMT_USE_UDL_TEMPLATE
 
 /**
   \rst
   User-defined literal equivalent of :func:`fmt::arg`.
 
   **Example**::
 
     using namespace fmt::literals;
     fmt::print("Elapsed time: {s:.2f} seconds", "s"_a=1.23);
   \endrst
  */
-inline internal::udl_arg<char>
-operator"" _a(const char *s, std::size_t) { return {s}; }
-inline internal::udl_arg<wchar_t>
-operator"" _a(const wchar_t *s, std::size_t) { return {s}; }
-} // inline namespace literals
-#endif // FMT_USE_USER_DEFINED_LITERALS
+FMT_CONSTEXPR detail::udl_arg<char> operator"" _a(const char* s, size_t) {
+  return {s};
+}
+FMT_CONSTEXPR detail::udl_arg<wchar_t> operator"" _a(const wchar_t* s, size_t) {
+  return {s};
+}
+}  // namespace literals
+#endif  // FMT_USE_USER_DEFINED_LITERALS
 FMT_END_NAMESPACE
 
-#define FMT_STRING(s) [] { \
-    typedef typename std::decay<decltype(s)>::type pointer; \
-    struct S : fmt::compile_string { \
-      static FMT_CONSTEXPR pointer data() { return s; } \
-      static FMT_CONSTEXPR size_t size() { return sizeof(s); } \
-      explicit operator fmt::string_view() const { return s; } \
-    }; \
-    return S{}; \
-  }()
-
-#if defined(FMT_STRING_ALIAS) && FMT_STRING_ALIAS
-/**
-  \rst
-  Constructs a compile-time format string. This macro is disabled by default to
-  prevent potential name collisions. To enable it define ``FMT_STRING_ALIAS`` to
-  1 before including ``fmt/format.h``.
-
-  **Example**::
-
-    #define FMT_STRING_ALIAS 1
-    #include <fmt/format.h>
-    // A compile-time error because 'd' is an invalid specifier for strings.
-    std::string s = format(fmt("{:d}"), "foo");
-  \endrst
- */
-# define fmt(s) FMT_STRING(s)
-#endif
-
 #ifdef FMT_HEADER_ONLY
-# define FMT_FUNC inline
-# include "format-inl.h"
+#  define FMT_FUNC inline
+#  include "format-inl.h"
 #else
-# define FMT_FUNC
-#endif
-
-// Restore warnings.
-#if FMT_GCC_VERSION >= 406 || FMT_CLANG_VERSION
-# pragma GCC diagnostic pop
+#  define FMT_FUNC
 #endif
 
 #endif  // FMT_FORMAT_H_
```

### Comparing `libsonata-0.1.8/extlib/fmt/include/fmt/printf.h` & `libsonata-0.1.9/extlib/fmt/include/fmt/printf.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,726 +1,751 @@
-// Formatting library for C++
+// Formatting library for C++ - legacy printf implementation
 //
 // Copyright (c) 2012 - 2016, Victor Zverovich
 // All rights reserved.
 //
 // For the license information refer to format.h.
 
 #ifndef FMT_PRINTF_H_
 #define FMT_PRINTF_H_
 
-#include <algorithm>  // std::fill_n
+#include <algorithm>  // std::max
 #include <limits>     // std::numeric_limits
 
 #include "ostream.h"
 
 FMT_BEGIN_NAMESPACE
-namespace internal {
+namespace detail {
 
 // Checks if a value fits in int - used to avoid warnings about comparing
 // signed and unsigned integers.
-template <bool IsSigned>
-struct int_checker {
-  template <typename T>
-  static bool fits_in_int(T value) {
-    unsigned max = std::numeric_limits<int>::max();
+template <bool IsSigned> struct int_checker {
+  template <typename T> static bool fits_in_int(T value) {
+    unsigned max = max_value<int>();
     return value <= max;
   }
   static bool fits_in_int(bool) { return true; }
 };
 
-template <>
-struct int_checker<true> {
-  template <typename T>
-  static bool fits_in_int(T value) {
-    return value >= std::numeric_limits<int>::min() &&
-           value <= std::numeric_limits<int>::max();
+template <> struct int_checker<true> {
+  template <typename T> static bool fits_in_int(T value) {
+    return value >= (std::numeric_limits<int>::min)() &&
+           value <= max_value<int>();
   }
   static bool fits_in_int(int) { return true; }
 };
 
-class printf_precision_handler: public function<int> {
+class printf_precision_handler {
  public:
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, int>::type
-      operator()(T value) {
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  int operator()(T value) {
     if (!int_checker<std::numeric_limits<T>::is_signed>::fits_in_int(value))
       FMT_THROW(format_error("number is too big"));
-    return static_cast<int>(value);
+    return (std::max)(static_cast<int>(value), 0);
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, int>::type operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  int operator()(T) {
     FMT_THROW(format_error("precision is not integer"));
     return 0;
   }
 };
 
 // An argument visitor that returns true iff arg is a zero integer.
-class is_zero_int: public function<bool> {
+class is_zero_int {
  public:
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, bool>::type
-      operator()(T value) { return value == 0; }
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  bool operator()(T value) {
+    return value == 0;
+  }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, bool>::type
-      operator()(T) { return false; }
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  bool operator()(T) {
+    return false;
+  }
 };
 
-template <typename T>
-struct make_unsigned_or_bool : std::make_unsigned<T> {};
+template <typename T> struct make_unsigned_or_bool : std::make_unsigned<T> {};
 
-template <>
-struct make_unsigned_or_bool<bool> {
-  typedef bool type;
-};
+template <> struct make_unsigned_or_bool<bool> { using type = bool; };
 
-template <typename T, typename Context>
-class arg_converter: public function<void> {
+template <typename T, typename Context> class arg_converter {
  private:
-  typedef typename Context::char_type Char;
+  using char_type = typename Context::char_type;
 
-  basic_format_arg<Context> &arg_;
-  typename Context::char_type type_;
+  basic_format_arg<Context>& arg_;
+  char_type type_;
 
  public:
-  arg_converter(basic_format_arg<Context> &arg, Char type)
-    : arg_(arg), type_(type) {}
+  arg_converter(basic_format_arg<Context>& arg, char_type type)
+      : arg_(arg), type_(type) {}
 
   void operator()(bool value) {
-    if (type_ != 's')
-      operator()<bool>(value);
+    if (type_ != 's') operator()<bool>(value);
   }
 
-  template <typename U>
-  typename std::enable_if<std::is_integral<U>::value>::type
-      operator()(U value) {
+  template <typename U, FMT_ENABLE_IF(std::is_integral<U>::value)>
+  void operator()(U value) {
     bool is_signed = type_ == 'd' || type_ == 'i';
-    typedef typename std::conditional<
-        std::is_same<T, void>::value, U, T>::type TargetType;
-    if (const_check(sizeof(TargetType) <= sizeof(int))) {
+    using target_type = conditional_t<std::is_same<T, void>::value, U, T>;
+    if (const_check(sizeof(target_type) <= sizeof(int))) {
       // Extra casts are used to silence warnings.
       if (is_signed) {
-        arg_ = internal::make_arg<Context>(
-          static_cast<int>(static_cast<TargetType>(value)));
+        arg_ = detail::make_arg<Context>(
+            static_cast<int>(static_cast<target_type>(value)));
       } else {
-        typedef typename make_unsigned_or_bool<TargetType>::type Unsigned;
-        arg_ = internal::make_arg<Context>(
-          static_cast<unsigned>(static_cast<Unsigned>(value)));
+        using unsigned_type = typename make_unsigned_or_bool<target_type>::type;
+        arg_ = detail::make_arg<Context>(
+            static_cast<unsigned>(static_cast<unsigned_type>(value)));
       }
     } else {
       if (is_signed) {
         // glibc's printf doesn't sign extend arguments of smaller types:
         //   std::printf("%lld", -42);  // prints "4294967254"
         // but we don't have to do the same because it's a UB.
-        arg_ = internal::make_arg<Context>(static_cast<long long>(value));
+        arg_ = detail::make_arg<Context>(static_cast<long long>(value));
       } else {
-        arg_ = internal::make_arg<Context>(
-          static_cast<typename make_unsigned_or_bool<U>::type>(value));
+        arg_ = detail::make_arg<Context>(
+            static_cast<typename make_unsigned_or_bool<U>::type>(value));
       }
     }
   }
 
-  template <typename U>
-  typename std::enable_if<!std::is_integral<U>::value>::type operator()(U) {
-    // No coversion needed for non-integral types.
-  }
+  template <typename U, FMT_ENABLE_IF(!std::is_integral<U>::value)>
+  void operator()(U) {}  // No conversion needed for non-integral types.
 };
 
 // Converts an integer argument to T for printf, if T is an integral type.
 // If T is void, the argument is converted to corresponding signed or unsigned
 // type depending on the type specifier: 'd' and 'i' - signed, other -
 // unsigned).
 template <typename T, typename Context, typename Char>
-void convert_arg(basic_format_arg<Context> &arg, Char type) {
-  fmt::visit(arg_converter<T, Context>(arg, type), arg);
+void convert_arg(basic_format_arg<Context>& arg, Char type) {
+  visit_format_arg(arg_converter<T, Context>(arg, type), arg);
 }
 
 // Converts an integer argument to char for printf.
-template <typename Context>
-class char_converter: public function<void> {
+template <typename Context> class char_converter {
  private:
-  basic_format_arg<Context> &arg_;
+  basic_format_arg<Context>& arg_;
 
  public:
-  explicit char_converter(basic_format_arg<Context> &arg) : arg_(arg) {}
+  explicit char_converter(basic_format_arg<Context>& arg) : arg_(arg) {}
 
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value>::type
-      operator()(T value) {
-    typedef typename Context::char_type Char;
-    arg_ = internal::make_arg<Context>(static_cast<Char>(value));
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  void operator()(T value) {
+    arg_ = detail::make_arg<Context>(
+        static_cast<typename Context::char_type>(value));
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value>::type operator()(T) {
-    // No coversion needed for non-integral types.
-  }
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  void operator()(T) {}  // No conversion needed for non-integral types.
+};
+
+// An argument visitor that return a pointer to a C string if argument is a
+// string or null otherwise.
+template <typename Char> struct get_cstring {
+  template <typename T> const Char* operator()(T) { return nullptr; }
+  const Char* operator()(const Char* s) { return s; }
 };
 
 // Checks if an argument is a valid printf width specifier and sets
 // left alignment if it is negative.
-template <typename Char>
-class printf_width_handler: public function<unsigned> {
+template <typename Char> class printf_width_handler {
  private:
-  typedef basic_format_specs<Char> format_specs;
+  using format_specs = basic_format_specs<Char>;
 
-  format_specs &spec_;
+  format_specs& specs_;
 
  public:
-  explicit printf_width_handler(format_specs &spec) : spec_(spec) {}
+  explicit printf_width_handler(format_specs& specs) : specs_(specs) {}
 
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, unsigned>::type
-      operator()(T value) {
-    typedef typename internal::int_traits<T>::main_type UnsignedType;
-    UnsignedType width = static_cast<UnsignedType>(value);
-    if (internal::is_negative(value)) {
-      spec_.align_ = ALIGN_LEFT;
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  unsigned operator()(T value) {
+    auto width = static_cast<uint32_or_64_or_128_t<T>>(value);
+    if (detail::is_negative(value)) {
+      specs_.align = align::left;
       width = 0 - width;
     }
-    unsigned int_max = std::numeric_limits<int>::max();
-    if (width > int_max)
-      FMT_THROW(format_error("number is too big"));
+    unsigned int_max = max_value<int>();
+    if (width > int_max) FMT_THROW(format_error("number is too big"));
     return static_cast<unsigned>(width);
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, unsigned>::type
-      operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  unsigned operator()(T) {
     FMT_THROW(format_error("width is not integer"));
     return 0;
   }
 };
-}  // namespace internal
 
-template <typename Range>
-class printf_arg_formatter;
+template <typename Char, typename Context>
+void vprintf(buffer<Char>& buf, basic_string_view<Char> format,
+             basic_format_args<Context> args) {
+  Context(buffer_appender<Char>(buf), format, args).format();
+}
+}  // namespace detail
 
-template <
-    typename OutputIt, typename Char,
-    typename ArgFormatter =
-      printf_arg_formatter<back_insert_range<internal::basic_buffer<Char>>>>
-class basic_printf_context;
+// For printing into memory_buffer.
+template <typename Char, typename Context>
+FMT_DEPRECATED void printf(detail::buffer<Char>& buf,
+                           basic_string_view<Char> format,
+                           basic_format_args<Context> args) {
+  return detail::vprintf(buf, format, args);
+}
+using detail::vprintf;
+
+template <typename Char>
+class basic_printf_parse_context : public basic_format_parse_context<Char> {
+  using basic_format_parse_context<Char>::basic_format_parse_context;
+};
+template <typename OutputIt, typename Char> class basic_printf_context;
 
 /**
   \rst
   The ``printf`` argument formatter.
   \endrst
  */
-template <typename Range>
-class printf_arg_formatter:
-  public internal::function<
-    typename internal::arg_formatter_base<Range>::iterator>,
-  public internal::arg_formatter_base<Range> {
+template <typename OutputIt, typename Char>
+class printf_arg_formatter : public detail::arg_formatter_base<OutputIt, Char> {
+ public:
+  using iterator = OutputIt;
+
  private:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef internal::arg_formatter_base<Range> base;
-  typedef basic_printf_context<iterator, char_type> context_type;
+  using char_type = Char;
+  using base = detail::arg_formatter_base<OutputIt, Char>;
+  using context_type = basic_printf_context<OutputIt, Char>;
 
-  context_type &context_;
+  context_type& context_;
 
   void write_null_pointer(char) {
-    this->spec()->type_ = 0;
+    this->specs()->type = 0;
     this->write("(nil)");
   }
 
   void write_null_pointer(wchar_t) {
-    this->spec()->type_ = 0;
+    this->specs()->type = 0;
     this->write(L"(nil)");
   }
 
  public:
-  typedef typename base::format_specs format_specs;
+  using format_specs = typename base::format_specs;
 
   /**
     \rst
     Constructs an argument formatter object.
-    *buffer* is a reference to the output buffer and *spec* contains format
+    *buffer* is a reference to the output buffer and *specs* contains format
     specifier information for standard argument types.
     \endrst
    */
-  printf_arg_formatter(internal::basic_buffer<char_type> &buffer,
-                       format_specs &spec, context_type &ctx)
-    : base(back_insert_range<internal::basic_buffer<char_type>>(buffer), &spec),
-      context_(ctx) {}
-
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, iterator>::type
-      operator()(T value) {
+  printf_arg_formatter(iterator iter, format_specs& specs, context_type& ctx)
+      : base(iter, &specs, detail::locale_ref()), context_(ctx) {}
+
+  template <typename T, FMT_ENABLE_IF(fmt::detail::is_integral<T>::value)>
+  iterator operator()(T value) {
     // MSVC2013 fails to compile separate overloads for bool and char_type so
     // use std::is_same instead.
     if (std::is_same<T, bool>::value) {
-      format_specs &fmt_spec = *this->spec();
-      if (fmt_spec.type_ != 's')
-        return base::operator()(value ? 1 : 0);
-      fmt_spec.type_ = 0;
+      format_specs& fmt_specs = *this->specs();
+      if (fmt_specs.type != 's') return base::operator()(value ? 1 : 0);
+      fmt_specs.type = 0;
       this->write(value != 0);
     } else if (std::is_same<T, char_type>::value) {
-      format_specs &fmt_spec = *this->spec();
-      if (fmt_spec.type_ && fmt_spec.type_ != 'c')
+      format_specs& fmt_specs = *this->specs();
+      if (fmt_specs.type && fmt_specs.type != 'c')
         return (*this)(static_cast<int>(value));
-      fmt_spec.flags_ = 0;
-      fmt_spec.align_ = ALIGN_RIGHT;
+      fmt_specs.sign = sign::none;
+      fmt_specs.alt = false;
+      fmt_specs.fill[0] = ' ';  // Ignore '0' flag for char types.
+      // align::numeric needs to be overwritten here since the '0' flag is
+      // ignored for non-numeric types
+      if (fmt_specs.align == align::none || fmt_specs.align == align::numeric)
+        fmt_specs.align = align::right;
       return base::operator()(value);
     } else {
       return base::operator()(value);
     }
     return this->out();
   }
 
-  template <typename T>
-  typename std::enable_if<std::is_floating_point<T>::value, iterator>::type
-      operator()(T value) {
+  template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+  iterator operator()(T value) {
     return base::operator()(value);
   }
 
   /** Formats a null-terminated C string. */
-  iterator operator()(const char *value) {
+  iterator operator()(const char* value) {
     if (value)
       base::operator()(value);
-    else if (this->spec()->type_ == 'p')
+    else if (this->specs()->type == 'p')
       write_null_pointer(char_type());
     else
       this->write("(null)");
     return this->out();
   }
 
   /** Formats a null-terminated wide C string. */
-  iterator operator()(const wchar_t *value) {
+  iterator operator()(const wchar_t* value) {
     if (value)
       base::operator()(value);
-    else if (this->spec()->type_ == 'p')
+    else if (this->specs()->type == 'p')
       write_null_pointer(char_type());
     else
       this->write(L"(null)");
     return this->out();
   }
 
   iterator operator()(basic_string_view<char_type> value) {
     return base::operator()(value);
   }
 
-  iterator operator()(monostate value) {
-    return base::operator()(value);
-  }
+  iterator operator()(monostate value) { return base::operator()(value); }
 
   /** Formats a pointer. */
-  iterator operator()(const void *value) {
-    if (value)
-      return base::operator()(value);
-    this->spec()->type_ = 0;
+  iterator operator()(const void* value) {
+    if (value) return base::operator()(value);
+    this->specs()->type = 0;
     write_null_pointer(char_type());
     return this->out();
   }
 
   /** Formats an argument of a custom (user-defined) type. */
   iterator operator()(typename basic_format_arg<context_type>::handle handle) {
-    handle.format(context_);
+    handle.format(context_.parse_context(), context_);
     return this->out();
   }
 };
 
-template <typename T>
-struct printf_formatter {
+template <typename T> struct printf_formatter {
+  printf_formatter() = delete;
+
   template <typename ParseContext>
-  auto parse(ParseContext &ctx) -> decltype(ctx.begin()) { return ctx.begin(); }
+  auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    return ctx.begin();
+  }
 
   template <typename FormatContext>
-  auto format(const T &value, FormatContext &ctx) -> decltype(ctx.out()) {
-    internal::format_value(internal::get_container(ctx.out()), value);
+  auto format(const T& value, FormatContext& ctx) -> decltype(ctx.out()) {
+    detail::format_value(detail::get_container(ctx.out()), value);
     return ctx.out();
   }
 };
 
-/** This template formats data and writes the output to a writer. */
-template <typename OutputIt, typename Char, typename ArgFormatter>
-class basic_printf_context :
-  // Inherit publicly as a workaround for the icc bug
-  // https://software.intel.com/en-us/forums/intel-c-compiler/topic/783476.
-  public internal::context_base<
-    OutputIt, basic_printf_context<OutputIt, Char, ArgFormatter>, Char> {
+/**
+ This template formats data and writes the output through an output iterator.
+ */
+template <typename OutputIt, typename Char> class basic_printf_context {
  public:
   /** The character type for the output. */
-  typedef Char char_type;
-
-  template <typename T>
-  struct formatter_type { typedef printf_formatter<T> type; };
+  using char_type = Char;
+  using iterator = OutputIt;
+  using format_arg = basic_format_arg<basic_printf_context>;
+  using parse_context_type = basic_printf_parse_context<Char>;
+  template <typename T> using formatter_type = printf_formatter<T>;
 
  private:
-  typedef internal::context_base<OutputIt, basic_printf_context, Char> base;
-  typedef typename base::format_arg format_arg;
-  typedef basic_format_specs<char_type> format_specs;
-  typedef internal::null_terminating_iterator<char_type> iterator;
-
-  void parse_flags(format_specs &spec, iterator &it);
-
-  // Returns the argument with specified index or, if arg_index is equal
-  // to the maximum unsigned value, the next argument.
-  format_arg get_arg(
-      iterator it,
-      unsigned arg_index = (std::numeric_limits<unsigned>::max)());
+  using format_specs = basic_format_specs<char_type>;
+
+  OutputIt out_;
+  basic_format_args<basic_printf_context> args_;
+  parse_context_type parse_ctx_;
+
+  static void parse_flags(format_specs& specs, const Char*& it,
+                          const Char* end);
+
+  // Returns the argument with specified index or, if arg_index is -1, the next
+  // argument.
+  format_arg get_arg(int arg_index = -1);
 
   // Parses argument index, flags and width and returns the argument index.
-  unsigned parse_header(iterator &it, format_specs &spec);
+  int parse_header(const Char*& it, const Char* end, format_specs& specs);
 
  public:
   /**
    \rst
-   Constructs a ``printf_context`` object. References to the arguments and
-   the writer are stored in the context object so make sure they have
-   appropriate lifetimes.
+   Constructs a ``printf_context`` object. References to the arguments are
+   stored in the context object so make sure they have appropriate lifetimes.
    \endrst
    */
   basic_printf_context(OutputIt out, basic_string_view<char_type> format_str,
                        basic_format_args<basic_printf_context> args)
-    : base(out, format_str, args) {}
+      : out_(out), args_(args), parse_ctx_(format_str) {}
+
+  OutputIt out() { return out_; }
+  void advance_to(OutputIt it) { out_ = it; }
+
+  detail::locale_ref locale() { return {}; }
+
+  format_arg arg(int id) const { return args_.get(id); }
 
-  using base::parse_context;
-  using base::out;
-  using base::advance_to;
+  parse_context_type& parse_context() { return parse_ctx_; }
+
+  FMT_CONSTEXPR void on_error(const char* message) {
+    parse_ctx_.on_error(message);
+  }
 
   /** Formats stored arguments and writes the output to the range. */
-  void format();
+  template <typename ArgFormatter = printf_arg_formatter<OutputIt, Char>>
+  OutputIt format();
 };
 
-template <typename OutputIt, typename Char, typename AF>
-void basic_printf_context<OutputIt, Char, AF>::parse_flags(
-    format_specs &spec, iterator &it) {
-  for (;;) {
-    switch (*it++) {
-      case '-':
-        spec.align_ = ALIGN_LEFT;
-        break;
-      case '+':
-        spec.flags_ |= SIGN_FLAG | PLUS_FLAG;
-        break;
-      case '0':
-        spec.fill_ = '0';
-        break;
-      case ' ':
-        spec.flags_ |= SIGN_FLAG;
-        break;
-      case '#':
-        spec.flags_ |= HASH_FLAG;
-        break;
-      default:
-        --it;
-        return;
+template <typename OutputIt, typename Char>
+void basic_printf_context<OutputIt, Char>::parse_flags(format_specs& specs,
+                                                       const Char*& it,
+                                                       const Char* end) {
+  for (; it != end; ++it) {
+    switch (*it) {
+    case '-':
+      specs.align = align::left;
+      break;
+    case '+':
+      specs.sign = sign::plus;
+      break;
+    case '0':
+      specs.fill[0] = '0';
+      break;
+    case ' ':
+      if (specs.sign != sign::plus) {
+        specs.sign = sign::space;
+      }
+      break;
+    case '#':
+      specs.alt = true;
+      break;
+    default:
+      return;
     }
   }
 }
 
-template <typename OutputIt, typename Char, typename AF>
-typename basic_printf_context<OutputIt, Char, AF>::format_arg
-  basic_printf_context<OutputIt, Char, AF>::get_arg(
-    iterator it, unsigned arg_index) {
-  (void)it;
-  if (arg_index == std::numeric_limits<unsigned>::max())
-    return this->do_get_arg(this->parse_context().next_arg_id());
-  return base::get_arg(arg_index - 1);
+template <typename OutputIt, typename Char>
+typename basic_printf_context<OutputIt, Char>::format_arg
+basic_printf_context<OutputIt, Char>::get_arg(int arg_index) {
+  if (arg_index < 0)
+    arg_index = parse_ctx_.next_arg_id();
+  else
+    parse_ctx_.check_arg_id(--arg_index);
+  return detail::get_arg(*this, arg_index);
 }
 
-template <typename OutputIt, typename Char, typename AF>
-unsigned basic_printf_context<OutputIt, Char, AF>::parse_header(
-  iterator &it, format_specs &spec) {
-  unsigned arg_index = std::numeric_limits<unsigned>::max();
+template <typename OutputIt, typename Char>
+int basic_printf_context<OutputIt, Char>::parse_header(const Char*& it,
+                                                       const Char* end,
+                                                       format_specs& specs) {
+  int arg_index = -1;
   char_type c = *it;
   if (c >= '0' && c <= '9') {
     // Parse an argument index (if followed by '$') or a width possibly
     // preceded with '0' flag(s).
-    internal::error_handler eh;
-    unsigned value = parse_nonnegative_int(it, eh);
-    if (*it == '$') {  // value is an argument index
+    detail::error_handler eh;
+    int value = parse_nonnegative_int(it, end, eh);
+    if (it != end && *it == '$') {  // value is an argument index
       ++it;
       arg_index = value;
     } else {
-      if (c == '0')
-        spec.fill_ = '0';
+      if (c == '0') specs.fill[0] = '0';
       if (value != 0) {
         // Nonzero value means that we parsed width and don't need to
         // parse it or flags again, so return now.
-        spec.width_ = value;
+        specs.width = value;
         return arg_index;
       }
     }
   }
-  parse_flags(spec, it);
+  parse_flags(specs, it, end);
   // Parse width.
-  if (*it >= '0' && *it <= '9') {
-    internal::error_handler eh;
-    spec.width_ = parse_nonnegative_int(it, eh);
-  } else if (*it == '*') {
-    ++it;
-    spec.width_ =
-        fmt::visit(internal::printf_width_handler<char_type>(spec), get_arg(it));
+  if (it != end) {
+    if (*it >= '0' && *it <= '9') {
+      detail::error_handler eh;
+      specs.width = parse_nonnegative_int(it, end, eh);
+    } else if (*it == '*') {
+      ++it;
+      specs.width = static_cast<int>(visit_format_arg(
+          detail::printf_width_handler<char_type>(specs), get_arg()));
+    }
   }
   return arg_index;
 }
 
-template <typename OutputIt, typename Char, typename AF>
-void basic_printf_context<OutputIt, Char, AF>::format() {
-  auto &buffer = internal::get_container(this->out());
-  auto start = iterator(this->parse_context());
+template <typename OutputIt, typename Char>
+template <typename ArgFormatter>
+OutputIt basic_printf_context<OutputIt, Char>::format() {
+  auto out = this->out();
+  const Char* start = parse_ctx_.begin();
+  const Char* end = parse_ctx_.end();
   auto it = start;
-  using internal::pointer_from;
-  while (*it) {
+  while (it != end) {
     char_type c = *it++;
     if (c != '%') continue;
-    if (*it == c) {
-      buffer.append(pointer_from(start), pointer_from(it));
+    if (it != end && *it == c) {
+      out = std::copy(start, it, out);
       start = ++it;
       continue;
     }
-    buffer.append(pointer_from(start), pointer_from(it) - 1);
+    out = std::copy(start, it - 1, out);
 
-    format_specs spec;
-    spec.align_ = ALIGN_RIGHT;
+    format_specs specs;
+    specs.align = align::right;
 
     // Parse argument index, flags and width.
-    unsigned arg_index = parse_header(it, spec);
+    int arg_index = parse_header(it, end, specs);
+    if (arg_index == 0) on_error("argument not found");
 
     // Parse precision.
-    if (*it == '.') {
+    if (it != end && *it == '.') {
       ++it;
-      if ('0' <= *it && *it <= '9') {
-        internal::error_handler eh;
-        spec.precision_ = static_cast<int>(parse_nonnegative_int(it, eh));
-      } else if (*it == '*') {
+      c = it != end ? *it : 0;
+      if ('0' <= c && c <= '9') {
+        detail::error_handler eh;
+        specs.precision = parse_nonnegative_int(it, end, eh);
+      } else if (c == '*') {
         ++it;
-        spec.precision_ =
-            fmt::visit(internal::printf_precision_handler(), get_arg(it));
+        specs.precision = static_cast<int>(
+            visit_format_arg(detail::printf_precision_handler(), get_arg()));
       } else {
-        spec.precision_ = 0;
+        specs.precision = 0;
       }
     }
 
-    format_arg arg = get_arg(it, arg_index);
-    if (spec.flag(HASH_FLAG) && fmt::visit(internal::is_zero_int(), arg))
-      spec.flags_ &= ~internal::to_unsigned<int>(HASH_FLAG);
-    if (spec.fill_ == '0') {
-      if (arg.is_arithmetic())
-        spec.align_ = ALIGN_NUMERIC;
+    format_arg arg = get_arg(arg_index);
+    // For d, i, o, u, x, and X conversion specifiers, if a precision is
+    // specified, the '0' flag is ignored
+    if (specs.precision >= 0 && arg.is_integral())
+      specs.fill[0] =
+          ' ';  // Ignore '0' flag for non-numeric types or if '-' present.
+    if (specs.precision >= 0 && arg.type() == detail::type::cstring_type) {
+      auto str = visit_format_arg(detail::get_cstring<Char>(), arg);
+      auto str_end = str + specs.precision;
+      auto nul = std::find(str, str_end, Char());
+      arg = detail::make_arg<basic_printf_context>(basic_string_view<Char>(
+          str,
+          detail::to_unsigned(nul != str_end ? nul - str : specs.precision)));
+    }
+    if (specs.alt && visit_format_arg(detail::is_zero_int(), arg))
+      specs.alt = false;
+    if (specs.fill[0] == '0') {
+      if (arg.is_arithmetic() && specs.align != align::left)
+        specs.align = align::numeric;
       else
-        spec.fill_ = ' ';  // Ignore '0' flag for non-numeric types.
+        specs.fill[0] = ' ';  // Ignore '0' flag for non-numeric types or if '-'
+                              // flag is also present.
     }
 
     // Parse length and convert the argument to the required type.
-    using internal::convert_arg;
-    switch (*it++) {
+    c = it != end ? *it++ : 0;
+    char_type t = it != end ? *it : 0;
+    using detail::convert_arg;
+    switch (c) {
     case 'h':
-      if (*it == 'h')
-        convert_arg<signed char>(arg, *++it);
-      else
-        convert_arg<short>(arg, *it);
+      if (t == 'h') {
+        ++it;
+        t = it != end ? *it : 0;
+        convert_arg<signed char>(arg, t);
+      } else {
+        convert_arg<short>(arg, t);
+      }
       break;
     case 'l':
-      if (*it == 'l')
-        convert_arg<long long>(arg, *++it);
-      else
-        convert_arg<long>(arg, *it);
+      if (t == 'l') {
+        ++it;
+        t = it != end ? *it : 0;
+        convert_arg<long long>(arg, t);
+      } else {
+        convert_arg<long>(arg, t);
+      }
       break;
     case 'j':
-      convert_arg<intmax_t>(arg, *it);
+      convert_arg<intmax_t>(arg, t);
       break;
     case 'z':
-      convert_arg<std::size_t>(arg, *it);
+      convert_arg<size_t>(arg, t);
       break;
     case 't':
-      convert_arg<std::ptrdiff_t>(arg, *it);
+      convert_arg<std::ptrdiff_t>(arg, t);
       break;
     case 'L':
       // printf produces garbage when 'L' is omitted for long double, no
       // need to do the same.
       break;
     default:
       --it;
-      convert_arg<void>(arg, *it);
+      convert_arg<void>(arg, c);
     }
 
     // Parse type.
-    if (!*it)
-      FMT_THROW(format_error("invalid format string"));
-    spec.type_ = static_cast<char>(*it++);
+    if (it == end) FMT_THROW(format_error("invalid format string"));
+    specs.type = static_cast<char>(*it++);
     if (arg.is_integral()) {
       // Normalize type.
-      switch (spec.type_) {
-      case 'i': case 'u':
-        spec.type_ = 'd';
+      switch (specs.type) {
+      case 'i':
+      case 'u':
+        specs.type = 'd';
         break;
       case 'c':
-        // TODO: handle wchar_t better?
-        fmt::visit(internal::char_converter<basic_printf_context>(arg), arg);
+        visit_format_arg(detail::char_converter<basic_printf_context>(arg),
+                         arg);
         break;
       }
     }
 
     start = it;
 
     // Format argument.
-    fmt::visit(AF(buffer, spec, *this), arg);
+    out = visit_format_arg(ArgFormatter(out, specs, *this), arg);
   }
-  buffer.append(pointer_from(start), pointer_from(it));
+  return std::copy(start, it, out);
 }
 
-template <typename Char, typename Context>
-void printf(internal::basic_buffer<Char> &buf, basic_string_view<Char> format,
-            basic_format_args<Context> args) {
-  Context(std::back_inserter(buf), format, args).format();
-}
+template <typename Char>
+using basic_printf_context_t =
+    basic_printf_context<detail::buffer_appender<Char>, Char>;
 
-template <typename Buffer>
-struct printf_context {
-  typedef basic_printf_context<
-    std::back_insert_iterator<Buffer>, typename Buffer::value_type> type;
-};
+using printf_context = basic_printf_context_t<char>;
+using wprintf_context = basic_printf_context_t<wchar_t>;
+
+using printf_args = basic_format_args<printf_context>;
+using wprintf_args = basic_format_args<wprintf_context>;
 
-template <typename ...Args>
-inline format_arg_store<printf_context<internal::buffer>::type, Args...>
-    make_printf_args(const Args & ... args) {
-  return format_arg_store<printf_context<internal::buffer>::type, Args...>(
-      args...);
+/**
+  \rst
+  Constructs an `~fmt::format_arg_store` object that contains references to
+  arguments and can be implicitly converted to `~fmt::printf_args`.
+  \endrst
+ */
+template <typename... Args>
+inline format_arg_store<printf_context, Args...> make_printf_args(
+    const Args&... args) {
+  return {args...};
+}
+
+/**
+  \rst
+  Constructs an `~fmt::format_arg_store` object that contains references to
+  arguments and can be implicitly converted to `~fmt::wprintf_args`.
+  \endrst
+ */
+template <typename... Args>
+inline format_arg_store<wprintf_context, Args...> make_wprintf_args(
+    const Args&... args) {
+  return {args...};
 }
-typedef basic_format_args<printf_context<internal::buffer>::type> printf_args;
-typedef basic_format_args<printf_context<internal::wbuffer>::type> wprintf_args;
 
-inline std::string vsprintf(string_view format, printf_args args) {
-  memory_buffer buffer;
-  printf(buffer, format, args);
+template <typename S, typename Char = char_t<S>>
+inline std::basic_string<Char> vsprintf(
+    const S& format,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args) {
+  basic_memory_buffer<Char> buffer;
+  vprintf(buffer, to_string_view(format), args);
   return to_string(buffer);
 }
 
 /**
   \rst
   Formats arguments and returns the result as a string.
 
   **Example**::
 
     std::string message = fmt::sprintf("The answer is %d", 42);
   \endrst
 */
-template <typename... Args>
-inline std::string sprintf(string_view format_str, const Args & ... args) {
-  return vsprintf(format_str,
-    make_format_args<typename printf_context<internal::buffer>::type>(args...));
-}
-
-inline std::wstring vsprintf(wstring_view format, wprintf_args args) {
-  wmemory_buffer buffer;
-  printf(buffer, format, args);
-  return to_string(buffer);
-}
-
-template <typename... Args>
-inline std::wstring sprintf(wstring_view format_str, const Args & ... args) {
-  return vsprintf(format_str,
-    make_format_args<typename printf_context<internal::wbuffer>::type>(args...));
+template <typename S, typename... Args,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+inline std::basic_string<Char> sprintf(const S& format, const Args&... args) {
+  using context = basic_printf_context_t<Char>;
+  return vsprintf(to_string_view(format), make_format_args<context>(args...));
 }
 
-template <typename Char>
-inline int vfprintf(std::FILE *f, basic_string_view<Char> format,
-                    basic_format_args<typename printf_context<
-                      internal::basic_buffer<Char>>::type> args) {
+template <typename S, typename Char = char_t<S>>
+inline int vfprintf(
+    std::FILE* f, const S& format,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args) {
   basic_memory_buffer<Char> buffer;
-  printf(buffer, format, args);
-  std::size_t size = buffer.size();
-  return std::fwrite(
-    buffer.data(), sizeof(Char), size, f) < size ? -1 : static_cast<int>(size);
+  vprintf(buffer, to_string_view(format), args);
+  size_t size = buffer.size();
+  return std::fwrite(buffer.data(), sizeof(Char), size, f) < size
+             ? -1
+             : static_cast<int>(size);
 }
 
 /**
   \rst
   Prints formatted data to the file *f*.
 
   **Example**::
 
     fmt::fprintf(stderr, "Don't %s!", "panic");
   \endrst
  */
-template <typename... Args>
-inline int fprintf(std::FILE *f, string_view format_str, const Args & ... args) {
-  auto vargs = make_format_args<
-    typename printf_context<internal::buffer>::type>(args...);
-  return vfprintf<char>(f, format_str, vargs);
-}
-
-template <typename... Args>
-inline int fprintf(std::FILE *f, wstring_view format_str,
-                   const Args & ... args) {
-  return vfprintf(f, format_str,
-    make_format_args<typename printf_context<internal::wbuffer>::type>(args...));
+template <typename S, typename... Args,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+inline int fprintf(std::FILE* f, const S& format, const Args&... args) {
+  using context = basic_printf_context_t<Char>;
+  return vfprintf(f, to_string_view(format),
+                  make_format_args<context>(args...));
 }
 
-inline int vprintf(string_view format, printf_args args) {
-  return vfprintf(stdout, format, args);
-}
-
-inline int vprintf(wstring_view format, wprintf_args args) {
-  return vfprintf(stdout, format, args);
+template <typename S, typename Char = char_t<S>>
+inline int vprintf(
+    const S& format,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args) {
+  return vfprintf(stdout, to_string_view(format), args);
 }
 
 /**
   \rst
   Prints formatted data to ``stdout``.
 
   **Example**::
 
     fmt::printf("Elapsed time: %.2f seconds", 1.23);
   \endrst
  */
-template <typename... Args>
-inline int printf(string_view format_str, const Args & ... args) {
-  return vprintf(format_str,
-    make_format_args<typename printf_context<internal::buffer>::type>(args...));
-}
-
-template <typename... Args>
-inline int printf(wstring_view format_str, const Args & ... args) {
-  return vprintf(format_str,
-    make_format_args<typename printf_context<internal::wbuffer>::type>(args...));
+template <typename S, typename... Args,
+          FMT_ENABLE_IF(detail::is_string<S>::value)>
+inline int printf(const S& format_str, const Args&... args) {
+  using context = basic_printf_context_t<char_t<S>>;
+  return vprintf(to_string_view(format_str),
+                 make_format_args<context>(args...));
 }
 
-inline int vfprintf(std::ostream &os, string_view format_str,
-                    printf_args args) {
-  memory_buffer buffer;
-  printf(buffer, format_str, args);
-  internal::write(os, buffer);
+template <typename S, typename Char = char_t<S>>
+inline int vfprintf(
+    std::basic_ostream<Char>& os, const S& format,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args) {
+  basic_memory_buffer<Char> buffer;
+  vprintf(buffer, to_string_view(format), args);
+  detail::write_buffer(os, buffer);
   return static_cast<int>(buffer.size());
 }
 
-inline int vfprintf(std::wostream &os, wstring_view format_str,
-                    wprintf_args args) {
-  wmemory_buffer buffer;
-  printf(buffer, format_str, args);
-  internal::write(os, buffer);
-  return static_cast<int>(buffer.size());
+/** Formats arguments and writes the output to the range. */
+template <typename ArgFormatter, typename Char,
+          typename Context =
+              basic_printf_context<typename ArgFormatter::iterator, Char>>
+typename ArgFormatter::iterator vprintf(
+    detail::buffer<Char>& out, basic_string_view<Char> format_str,
+    basic_format_args<type_identity_t<Context>> args) {
+  typename ArgFormatter::iterator iter(out);
+  Context(iter, format_str, args).template format<ArgFormatter>();
+  return iter;
 }
 
 /**
   \rst
   Prints formatted data to the stream *os*.
 
   **Example**::
 
     fmt::fprintf(cerr, "Don't %s!", "panic");
   \endrst
  */
-template <typename... Args>
-inline int fprintf(std::ostream &os, string_view format_str,
-                   const Args & ... args) {
-  auto vargs = make_format_args<
-    typename printf_context<internal::buffer>::type>(args...);
-  return vfprintf(os, format_str, vargs);
-}
-
-template <typename... Args>
-inline int fprintf(std::wostream &os, wstring_view format_str,
-                   const Args & ... args) {
-  auto vargs = make_format_args<
-    typename printf_context<internal::buffer>::type>(args...);
-  return vfprintf(os, format_str, vargs);
+template <typename S, typename... Args, typename Char = char_t<S>>
+inline int fprintf(std::basic_ostream<Char>& os, const S& format_str,
+                   const Args&... args) {
+  using context = basic_printf_context_t<Char>;
+  return vfprintf(os, to_string_view(format_str),
+                  make_format_args<context>(args...));
 }
 FMT_END_NAMESPACE
 
 #endif  // FMT_PRINTF_H_
```

### Comparing `libsonata-0.1.8/extlib/fmt/include/fmt/ranges.h` & `libsonata-0.1.9/extlib/fmt/include/fmt/ranges.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-// Formatting library for C++ - the core API
+// Formatting library for C++ - experimental range support
 //
 // Copyright (c) 2012 - present, Victor Zverovich
 // All rights reserved.
 //
 // For the license information refer to format.h.
 //
 // Copyright (c) 2018 - present, Remotion (Igor Schulz)
 // All Rights Reserved
 // {fmt} support for ranges, containers and types tuple interface.
 
 #ifndef FMT_RANGES_H_
 #define FMT_RANGES_H_
 
-#include "format.h"
+#include <initializer_list>
 #include <type_traits>
 
+#include "format.h"
+
 // output only up to N items from the range.
 #ifndef FMT_RANGE_OUTPUT_LENGTH_LIMIT
-# define FMT_RANGE_OUTPUT_LENGTH_LIMIT 256
+#  define FMT_RANGE_OUTPUT_LENGTH_LIMIT 256
 #endif
 
 FMT_BEGIN_NAMESPACE
 
-template <typename Char>
-struct formatting_base {
+template <typename Char> struct formatting_base {
   template <typename ParseContext>
-  FMT_CONSTEXPR auto parse(ParseContext &ctx) -> decltype(ctx.begin()) {
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
     return ctx.begin();
   }
 };
 
 template <typename Char, typename Enable = void>
 struct formatting_range : formatting_base<Char> {
-  static FMT_CONSTEXPR_DECL const std::size_t range_length_limit =
-      FMT_RANGE_OUTPUT_LENGTH_LIMIT; // output only up to N items from the range.
+  static FMT_CONSTEXPR_DECL const size_t range_length_limit =
+      FMT_RANGE_OUTPUT_LENGTH_LIMIT;  // output only up to N items from the
+                                      // range.
   Char prefix;
   Char delimiter;
   Char postfix;
   formatting_range() : prefix('{'), delimiter(','), postfix('}') {}
   static FMT_CONSTEXPR_DECL const bool add_delimiter_spaces = true;
   static FMT_CONSTEXPR_DECL const bool add_prepostfix_space = false;
 };
@@ -48,261 +50,344 @@
   Char delimiter;
   Char postfix;
   formatting_tuple() : prefix('('), delimiter(','), postfix(')') {}
   static FMT_CONSTEXPR_DECL const bool add_delimiter_spaces = true;
   static FMT_CONSTEXPR_DECL const bool add_prepostfix_space = false;
 };
 
-namespace internal {
+namespace detail {
 
 template <typename RangeT, typename OutputIterator>
-void copy(const RangeT &range, OutputIterator out) {
+OutputIterator copy(const RangeT& range, OutputIterator out) {
   for (auto it = range.begin(), end = range.end(); it != end; ++it)
     *out++ = *it;
+  return out;
 }
 
 template <typename OutputIterator>
-void copy(const char *str, OutputIterator out) {
-  const char *p_curr = str;
-  while (*p_curr) {
-    *out++ = *p_curr++;
-  }
+OutputIterator copy(const char* str, OutputIterator out) {
+  while (*str) *out++ = *str++;
+  return out;
 }
 
 template <typename OutputIterator>
-void copy(char ch, OutputIterator out) {
+OutputIterator copy(char ch, OutputIterator out) {
   *out++ = ch;
+  return out;
 }
 
 /// Return true value if T has std::string interface, like std::string_view.
-template <typename T>
-class is_like_std_string {
+template <typename T> class is_like_std_string {
   template <typename U>
-  static auto check(U *p) ->
-    decltype(p->find('a'), p->length(), p->data(), int());
-  template <typename>
-  static void check(...);
+  static auto check(U* p)
+      -> decltype((void)p->find('a'), p->length(), (void)p->data(), int());
+  template <typename> static void check(...);
 
  public:
   static FMT_CONSTEXPR_DECL const bool value =
-    !std::is_void<decltype(check<T>(FMT_NULL))>::value;
+      is_string<T>::value || !std::is_void<decltype(check<T>(nullptr))>::value;
 };
 
 template <typename Char>
 struct is_like_std_string<fmt::basic_string_view<Char>> : std::true_type {};
 
-template <typename... Ts>
-struct conditional_helper {};
+template <typename... Ts> struct conditional_helper {};
 
-template <typename T, typename _ = void>
-struct is_range_ : std::false_type {};
+template <typename T, typename _ = void> struct is_range_ : std::false_type {};
 
 #if !FMT_MSC_VER || FMT_MSC_VER > 1800
 template <typename T>
-struct is_range_<T, typename std::conditional<
-                    false,
-                    conditional_helper<decltype(internal::declval<T>().begin()),
-                                       decltype(internal::declval<T>().end())>,
-                    void>::type> : std::true_type {};
+struct is_range_<
+    T, conditional_t<false,
+                     conditional_helper<decltype(std::declval<T>().begin()),
+                                        decltype(std::declval<T>().end())>,
+                     void>> : std::true_type {};
 #endif
 
 /// tuple_size and tuple_element check.
-template <typename T>
-class is_tuple_like_ {
+template <typename T> class is_tuple_like_ {
   template <typename U>
-  static auto check(U *p) ->
-    decltype(std::tuple_size<U>::value,
-      internal::declval<typename std::tuple_element<0, U>::type>(), int());
-  template <typename>
-  static void check(...);
+  static auto check(U* p) -> decltype(std::tuple_size<U>::value, int());
+  template <typename> static void check(...);
 
  public:
   static FMT_CONSTEXPR_DECL const bool value =
-    !std::is_void<decltype(check<T>(FMT_NULL))>::value;
+      !std::is_void<decltype(check<T>(nullptr))>::value;
 };
 
 // Check for integer_sequence
 #if defined(__cpp_lib_integer_sequence) || FMT_MSC_VER >= 1900
 template <typename T, T... N>
 using integer_sequence = std::integer_sequence<T, N...>;
-template <std::size_t... N>
-using index_sequence = std::index_sequence<N...>;
-template <std::size_t N>
-using make_index_sequence = std::make_index_sequence<N>;
+template <size_t... N> using index_sequence = std::index_sequence<N...>;
+template <size_t N> using make_index_sequence = std::make_index_sequence<N>;
 #else
-template <typename T, T... N>
-struct integer_sequence {
-  typedef T value_type;
+template <typename T, T... N> struct integer_sequence {
+  using value_type = T;
 
-  static FMT_CONSTEXPR std::size_t size() {
-    return sizeof...(N);
-  }
+  static FMT_CONSTEXPR size_t size() { return sizeof...(N); }
 };
 
-template <std::size_t... N>
-using index_sequence = integer_sequence<std::size_t, N...>;
+template <size_t... N> using index_sequence = integer_sequence<size_t, N...>;
 
-template <typename T, std::size_t N, T... Ns>
+template <typename T, size_t N, T... Ns>
 struct make_integer_sequence : make_integer_sequence<T, N - 1, N - 1, Ns...> {};
 template <typename T, T... Ns>
 struct make_integer_sequence<T, 0, Ns...> : integer_sequence<T, Ns...> {};
 
-template <std::size_t N>
-using make_index_sequence = make_integer_sequence<std::size_t, N>;
+template <size_t N>
+using make_index_sequence = make_integer_sequence<size_t, N>;
 #endif
 
 template <class Tuple, class F, size_t... Is>
-void for_each(index_sequence<Is...>, Tuple &&tup, F &&f) FMT_NOEXCEPT {
+void for_each(index_sequence<Is...>, Tuple&& tup, F&& f) FMT_NOEXCEPT {
   using std::get;
   // using free function get<I>(T) now.
   const int _[] = {0, ((void)f(get<Is>(tup)), 0)...};
   (void)_;  // blocks warnings
 }
 
 template <class T>
-FMT_CONSTEXPR make_index_sequence<std::tuple_size<T>::value> 
-get_indexes(T const &) { return {}; }
+FMT_CONSTEXPR make_index_sequence<std::tuple_size<T>::value> get_indexes(
+    T const&) {
+  return {};
+}
 
-template <class Tuple, class F>
-void for_each(Tuple &&tup, F &&f) {
+template <class Tuple, class F> void for_each(Tuple&& tup, F&& f) {
   const auto indexes = get_indexes(tup);
   for_each(indexes, std::forward<Tuple>(tup), std::forward<F>(f));
 }
 
-template<typename Arg>
-FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const Arg&, 
-  typename std::enable_if<
-    !is_like_std_string<typename std::decay<Arg>::type>::value>::type* = nullptr) {
+template <typename Range>
+using value_type = remove_cvref_t<decltype(*std::declval<Range>().begin())>;
+
+template <typename Arg, FMT_ENABLE_IF(!is_like_std_string<
+                                      typename std::decay<Arg>::type>::value)>
+FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const Arg&) {
   return add_space ? " {}" : "{}";
 }
 
-template<typename Arg>
-FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const Arg&, 
-  typename std::enable_if<
-    is_like_std_string<typename std::decay<Arg>::type>::value>::type* = nullptr) {
+template <typename Arg, FMT_ENABLE_IF(is_like_std_string<
+                                      typename std::decay<Arg>::type>::value)>
+FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const Arg&) {
   return add_space ? " \"{}\"" : "\"{}\"";
 }
 
 FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const char*) {
   return add_space ? " \"{}\"" : "\"{}\"";
 }
 FMT_CONSTEXPR const wchar_t* format_str_quoted(bool add_space, const wchar_t*) {
-    return add_space ? L" \"{}\"" : L"\"{}\"";
+  return add_space ? L" \"{}\"" : L"\"{}\"";
 }
 
 FMT_CONSTEXPR const char* format_str_quoted(bool add_space, const char) {
-    return add_space ? " '{}'" : "'{}'";
+  return add_space ? " '{}'" : "'{}'";
 }
 FMT_CONSTEXPR const wchar_t* format_str_quoted(bool add_space, const wchar_t) {
-    return add_space ? L" '{}'" : L"'{}'";
+  return add_space ? L" '{}'" : L"'{}'";
 }
+}  // namespace detail
 
-}  // namespace internal
-
-template <typename T>
-struct is_tuple_like {
+template <typename T> struct is_tuple_like {
   static FMT_CONSTEXPR_DECL const bool value =
-    internal::is_tuple_like_<T>::value && !internal::is_range_<T>::value;
+      detail::is_tuple_like_<T>::value && !detail::is_range_<T>::value;
 };
 
 template <typename TupleT, typename Char>
-struct formatter<TupleT, Char, 
-    typename std::enable_if<fmt::is_tuple_like<TupleT>::value>::type> {
-private:
+struct formatter<TupleT, Char, enable_if_t<fmt::is_tuple_like<TupleT>::value>> {
+ private:
   // C++11 generic lambda for format()
-  template <typename FormatContext>
-  struct format_each {
-    template <typename T>
-    void operator()(const T& v) {
+  template <typename FormatContext> struct format_each {
+    template <typename T> void operator()(const T& v) {
       if (i > 0) {
         if (formatting.add_prepostfix_space) {
           *out++ = ' ';
         }
-        internal::copy(formatting.delimiter, out);
+        out = detail::copy(formatting.delimiter, out);
       }
-      format_to(out,
-                internal::format_str_quoted(
-                    (formatting.add_delimiter_spaces && i > 0), v),
-                v);
+      out = format_to(out,
+                      detail::format_str_quoted(
+                          (formatting.add_delimiter_spaces && i > 0), v),
+                      v);
       ++i;
     }
 
     formatting_tuple<Char>& formatting;
-    std::size_t& i;
-    typename std::add_lvalue_reference<decltype(std::declval<FormatContext>().out())>::type out;
+    size_t& i;
+    typename std::add_lvalue_reference<decltype(
+        std::declval<FormatContext>().out())>::type out;
   };
 
-public:
+ public:
   formatting_tuple<Char> formatting;
 
   template <typename ParseContext>
-  FMT_CONSTEXPR auto parse(ParseContext &ctx) -> decltype(ctx.begin()) {
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
     return formatting.parse(ctx);
   }
 
   template <typename FormatContext = format_context>
-  auto format(const TupleT &values, FormatContext &ctx) -> decltype(ctx.out()) {
+  auto format(const TupleT& values, FormatContext& ctx) -> decltype(ctx.out()) {
     auto out = ctx.out();
-    std::size_t i = 0;
-    internal::copy(formatting.prefix, out);
+    size_t i = 0;
+    detail::copy(formatting.prefix, out);
 
-    internal::for_each(values, format_each<FormatContext>{formatting, i, out});
+    detail::for_each(values, format_each<FormatContext>{formatting, i, out});
     if (formatting.add_prepostfix_space) {
       *out++ = ' ';
     }
-    internal::copy(formatting.postfix, out);
+    detail::copy(formatting.postfix, out);
 
     return ctx.out();
   }
 };
 
-template <typename T>
-struct is_range {
+template <typename T, typename Char> struct is_range {
   static FMT_CONSTEXPR_DECL const bool value =
-    internal::is_range_<T>::value && !internal::is_like_std_string<T>::value;
+      detail::is_range_<T>::value && !detail::is_like_std_string<T>::value &&
+      !std::is_convertible<T, std::basic_string<Char>>::value &&
+      !std::is_constructible<detail::std_string_view<Char>, T>::value;
 };
 
-template <typename RangeT, typename Char>
-struct formatter<RangeT, Char,
-    typename std::enable_if<fmt::is_range<RangeT>::value>::type> {
-
+template <typename T, typename Char>
+struct formatter<
+    T, Char,
+    enable_if_t<fmt::is_range<T, Char>::value
+// Workaround a bug in MSVC 2017 and earlier.
+#if !FMT_MSC_VER || FMT_MSC_VER >= 1927
+                && has_formatter<detail::value_type<T>, format_context>::value
+#endif
+                >> {
   formatting_range<Char> formatting;
 
   template <typename ParseContext>
-  FMT_CONSTEXPR auto parse(ParseContext &ctx) -> decltype(ctx.begin()) {
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
     return formatting.parse(ctx);
   }
 
   template <typename FormatContext>
-  typename FormatContext::iterator format(
-      const RangeT &values, FormatContext &ctx) {
-    auto out = ctx.out();
-    internal::copy(formatting.prefix, out);
-    std::size_t i = 0;
-    for (auto it = values.begin(), end = values.end(); it != end; ++it) {
+  typename FormatContext::iterator format(const T& values, FormatContext& ctx) {
+    auto out = detail::copy(formatting.prefix, ctx.out());
+    size_t i = 0;
+    auto it = values.begin();
+    auto end = values.end();
+    for (; it != end; ++it) {
       if (i > 0) {
-        if (formatting.add_prepostfix_space) {
-          *out++ = ' ';
-        }
-        internal::copy(formatting.delimiter, out);
+        if (formatting.add_prepostfix_space) *out++ = ' ';
+        out = detail::copy(formatting.delimiter, out);
       }
-      format_to(out,
-                internal::format_str_quoted(
-                    (formatting.add_delimiter_spaces && i > 0), *it),
-                *it);
+      out = format_to(out,
+                      detail::format_str_quoted(
+                          (formatting.add_delimiter_spaces && i > 0), *it),
+                      *it);
       if (++i > formatting.range_length_limit) {
-        format_to(out, " ... <other elements>");
+        out = format_to(out, " ... <other elements>");
         break;
       }
     }
-    if (formatting.add_prepostfix_space) {
-      *out++ = ' ';
-    }
-    internal::copy(formatting.postfix, out);
+    if (formatting.add_prepostfix_space) *out++ = ' ';
+    return detail::copy(formatting.postfix, out);
+  }
+};
+
+template <typename Char, typename... T> struct tuple_arg_join : detail::view {
+  const std::tuple<T...>& tuple;
+  basic_string_view<Char> sep;
+
+  tuple_arg_join(const std::tuple<T...>& t, basic_string_view<Char> s)
+      : tuple{t}, sep{s} {}
+};
+
+template <typename Char, typename... T>
+struct formatter<tuple_arg_join<Char, T...>, Char> {
+  template <typename ParseContext>
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    return ctx.begin();
+  }
+
+  template <typename FormatContext>
+  typename FormatContext::iterator format(
+      const tuple_arg_join<Char, T...>& value, FormatContext& ctx) {
+    return format(value, ctx, detail::make_index_sequence<sizeof...(T)>{});
+  }
+
+ private:
+  template <typename FormatContext, size_t... N>
+  typename FormatContext::iterator format(
+      const tuple_arg_join<Char, T...>& value, FormatContext& ctx,
+      detail::index_sequence<N...>) {
+    return format_args(value, ctx, std::get<N>(value.tuple)...);
+  }
+
+  template <typename FormatContext>
+  typename FormatContext::iterator format_args(
+      const tuple_arg_join<Char, T...>&, FormatContext& ctx) {
+    // NOTE: for compilers that support C++17, this empty function instantiation
+    // can be replaced with a constexpr branch in the variadic overload.
     return ctx.out();
   }
+
+  template <typename FormatContext, typename Arg, typename... Args>
+  typename FormatContext::iterator format_args(
+      const tuple_arg_join<Char, T...>& value, FormatContext& ctx,
+      const Arg& arg, const Args&... args) {
+    using base = formatter<typename std::decay<Arg>::type, Char>;
+    auto out = ctx.out();
+    out = base{}.format(arg, ctx);
+    if (sizeof...(Args) > 0) {
+      out = std::copy(value.sep.begin(), value.sep.end(), out);
+      ctx.advance_to(out);
+      return format_args(value, ctx, args...);
+    }
+    return out;
+  }
 };
 
-FMT_END_NAMESPACE
+/**
+  \rst
+  Returns an object that formats `tuple` with elements separated by `sep`.
+
+  **Example**::
+
+    std::tuple<int, char> t = {1, 'a'};
+    fmt::print("{}", fmt::join(t, ", "));
+    // Output: "1, a"
+  \endrst
+ */
+template <typename... T>
+FMT_CONSTEXPR tuple_arg_join<char, T...> join(const std::tuple<T...>& tuple,
+                                              string_view sep) {
+  return {tuple, sep};
+}
+
+template <typename... T>
+FMT_CONSTEXPR tuple_arg_join<wchar_t, T...> join(const std::tuple<T...>& tuple,
+                                                 wstring_view sep) {
+  return {tuple, sep};
+}
+
+/**
+  \rst
+  Returns an object that formats `initializer_list` with elements separated by
+  `sep`.
+
+  **Example**::
+
+    fmt::print("{}", fmt::join({1, 2, 3}, ", "));
+    // Output: "1, 2, 3"
+  \endrst
+ */
+template <typename T>
+arg_join<const T*, const T*, char> join(std::initializer_list<T> list,
+                                        string_view sep) {
+  return join(std::begin(list), std::end(list), sep);
+}
+
+template <typename T>
+arg_join<const T*, const T*, wchar_t> join(std::initializer_list<T> list,
+                                           wstring_view sep) {
+  return join(std::begin(list), std::end(list), sep);
+}
 
-#endif // FMT_RANGES_H_
+FMT_END_NAMESPACE
 
+#endif  // FMT_RANGES_H_
```

### Comparing `libsonata-0.1.8/extlib/fmt/include/fmt/ostream.h` & `libsonata-0.1.9/extlib/fmt/include/fmt/ostream.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 // Formatting library for C++ - std::ostream support
 //
-// Copyright (c) 2012 - 2016, Victor Zverovich
+// Copyright (c) 2012 - present, Victor Zverovich
 // All rights reserved.
 //
 // For the license information refer to format.h.
 
 #ifndef FMT_OSTREAM_H_
 #define FMT_OSTREAM_H_
 
-#include "format.h"
 #include <ostream>
 
+#include "format.h"
+
 FMT_BEGIN_NAMESPACE
-namespace internal {
 
-template <class Char>
-class formatbuf : public std::basic_streambuf<Char> {
+template <typename Char> class basic_printf_parse_context;
+template <typename OutputIt, typename Char> class basic_printf_context;
+
+namespace detail {
+
+template <class Char> class formatbuf : public std::basic_streambuf<Char> {
  private:
-  typedef typename std::basic_streambuf<Char>::int_type int_type;
-  typedef typename std::basic_streambuf<Char>::traits_type traits_type;
+  using int_type = typename std::basic_streambuf<Char>::int_type;
+  using traits_type = typename std::basic_streambuf<Char>::traits_type;
 
-  basic_buffer<Char> &buffer_;
+  buffer<Char>& buffer_;
 
  public:
-  formatbuf(basic_buffer<Char> &buffer) : buffer_(buffer) {}
+  formatbuf(buffer<Char>& buf) : buffer_(buf) {}
 
  protected:
   // The put-area is actually always empty. This makes the implementation
   // simpler and has the advantage that the streambuf and the buffer are always
   // in sync and sputc never writes into uninitialized memory. The obvious
   // disadvantage is that each call to sputc always results in a (virtual) call
   // to overflow. There is no disadvantage here for sputn since this always
@@ -35,123 +39,139 @@
 
   int_type overflow(int_type ch = traits_type::eof()) FMT_OVERRIDE {
     if (!traits_type::eq_int_type(ch, traits_type::eof()))
       buffer_.push_back(static_cast<Char>(ch));
     return ch;
   }
 
-  std::streamsize xsputn(const Char *s, std::streamsize count) FMT_OVERRIDE {
+  std::streamsize xsputn(const Char* s, std::streamsize count) FMT_OVERRIDE {
     buffer_.append(s, s + count);
     return count;
   }
 };
 
-template <typename Char>
-struct test_stream : std::basic_ostream<Char> {
+struct converter {
+  template <typename T, FMT_ENABLE_IF(is_integral<T>::value)> converter(T);
+};
+
+template <typename Char> struct test_stream : std::basic_ostream<Char> {
  private:
-  struct null;
-  // Hide all operator<< from std::basic_ostream<Char>.
-  void operator<<(null);
+  void_t<> operator<<(converter);
 };
 
-// Checks if T has a user-defined operator<< (e.g. not a member of std::ostream).
-template <typename T, typename Char>
-class is_streamable {
+// Hide insertion operators for built-in types.
+template <typename Char, typename Traits>
+void_t<> operator<<(std::basic_ostream<Char, Traits>&, Char);
+template <typename Char, typename Traits>
+void_t<> operator<<(std::basic_ostream<Char, Traits>&, char);
+template <typename Traits>
+void_t<> operator<<(std::basic_ostream<char, Traits>&, char);
+template <typename Traits>
+void_t<> operator<<(std::basic_ostream<char, Traits>&, signed char);
+template <typename Traits>
+void_t<> operator<<(std::basic_ostream<char, Traits>&, unsigned char);
+
+// Checks if T has a user-defined operator<< (e.g. not a member of
+// std::ostream).
+template <typename T, typename Char> class is_streamable {
  private:
   template <typename U>
-  static decltype(
-    internal::declval<test_stream<Char>&>()
-      << internal::declval<U>(), std::true_type()) test(int);
+  static bool_constant<!std::is_same<decltype(std::declval<test_stream<Char>&>()
+                                              << std::declval<U>()),
+                                     void_t<>>::value>
+  test(int);
 
-  template <typename>
-  static std::false_type test(...);
+  template <typename> static std::false_type test(...);
 
-  typedef decltype(test<T>(0)) result;
+  using result = decltype(test<T>(0));
 
  public:
   static const bool value = result::value;
 };
 
 // Write the content of buf to os.
 template <typename Char>
-void write(std::basic_ostream<Char> &os, basic_buffer<Char> &buf) {
-  const Char *data = buf.data();
-  typedef std::make_unsigned<std::streamsize>::type UnsignedStreamSize;
-  UnsignedStreamSize size = buf.size();
-  UnsignedStreamSize max_size =
-      internal::to_unsigned((std::numeric_limits<std::streamsize>::max)());
+void write_buffer(std::basic_ostream<Char>& os, buffer<Char>& buf) {
+  const Char* buf_data = buf.data();
+  using unsigned_streamsize = std::make_unsigned<std::streamsize>::type;
+  unsigned_streamsize size = buf.size();
+  unsigned_streamsize max_size = to_unsigned(max_value<std::streamsize>());
   do {
-    UnsignedStreamSize n = size <= max_size ? size : max_size;
-    os.write(data, static_cast<std::streamsize>(n));
-    data += n;
+    unsigned_streamsize n = size <= max_size ? size : max_size;
+    os.write(buf_data, static_cast<std::streamsize>(n));
+    buf_data += n;
     size -= n;
   } while (size != 0);
 }
 
 template <typename Char, typename T>
-void format_value(basic_buffer<Char> &buffer, const T &value) {
-  internal::formatbuf<Char> format_buf(buffer);
+void format_value(buffer<Char>& buf, const T& value,
+                  locale_ref loc = locale_ref()) {
+  formatbuf<Char> format_buf(buf);
   std::basic_ostream<Char> output(&format_buf);
-  output.exceptions(std::ios_base::failbit | std::ios_base::badbit);
+#if !defined(FMT_STATIC_THOUSANDS_SEPARATOR)
+  if (loc) output.imbue(loc.get<std::locale>());
+#endif
   output << value;
-  buffer.resize(buffer.size());
+  output.exceptions(std::ios_base::failbit | std::ios_base::badbit);
+  buf.try_resize(buf.size());
 }
-}  // namespace internal
-
-// Disable conversion to int if T has an overloaded operator<< which is a free
-// function (not a member of std::ostream).
-template <typename T, typename Char>
-struct convert_to_int<T, Char, void> {
-  static const bool value =
-    convert_to_int<T, Char, int>::value &&
-    !internal::is_streamable<T, Char>::value;
-};
 
 // Formats an object of type T that has an overloaded ostream operator<<.
 template <typename T, typename Char>
-struct formatter<T, Char,
-    typename std::enable_if<
-      internal::is_streamable<T, Char>::value &&
-      !internal::format_type<
-        typename buffer_context<Char>::type, T>::value>::type>
-    : formatter<basic_string_view<Char>, Char> {
+struct fallback_formatter<T, Char, enable_if_t<is_streamable<T, Char>::value>>
+    : private formatter<basic_string_view<Char>, Char> {
+  FMT_CONSTEXPR auto parse(basic_format_parse_context<Char>& ctx)
+      -> decltype(ctx.begin()) {
+    return formatter<basic_string_view<Char>, Char>::parse(ctx);
+  }
+  template <typename ParseCtx,
+            FMT_ENABLE_IF(std::is_same<
+                          ParseCtx, basic_printf_parse_context<Char>>::value)>
+  auto parse(ParseCtx& ctx) -> decltype(ctx.begin()) {
+    return ctx.begin();
+  }
 
-  template <typename Context>
-  auto format(const T &value, Context &ctx) -> decltype(ctx.out()) {
+  template <typename OutputIt>
+  auto format(const T& value, basic_format_context<OutputIt, Char>& ctx)
+      -> OutputIt {
     basic_memory_buffer<Char> buffer;
-    internal::format_value(buffer, value);
+    format_value(buffer, value, ctx.locale());
     basic_string_view<Char> str(buffer.data(), buffer.size());
     return formatter<basic_string_view<Char>, Char>::format(str, ctx);
   }
+  template <typename OutputIt>
+  auto format(const T& value, basic_printf_context<OutputIt, Char>& ctx)
+      -> OutputIt {
+    basic_memory_buffer<Char> buffer;
+    format_value(buffer, value, ctx.locale());
+    return std::copy(buffer.begin(), buffer.end(), ctx.out());
+  }
 };
+}  // namespace detail
 
 template <typename Char>
-inline void vprint(std::basic_ostream<Char> &os,
-                   basic_string_view<Char> format_str,
-                   basic_format_args<typename buffer_context<Char>::type> args) {
+void vprint(std::basic_ostream<Char>& os, basic_string_view<Char> format_str,
+            basic_format_args<buffer_context<type_identity_t<Char>>> args) {
   basic_memory_buffer<Char> buffer;
-  vformat_to(buffer, format_str, args);
-  internal::write(os, buffer);
+  detail::vformat_to(buffer, format_str, args);
+  detail::write_buffer(os, buffer);
 }
+
 /**
   \rst
   Prints formatted data to the stream *os*.
 
   **Example**::
 
     fmt::print(cerr, "Don't {}!", "panic");
   \endrst
  */
-template <typename... Args>
-inline void print(std::ostream &os, string_view format_str,
-                  const Args & ... args) {
-  vprint<char>(os, format_str, make_format_args<format_context>(args...));
-}
-
-template <typename... Args>
-inline void print(std::wostream &os, wstring_view format_str,
-                  const Args & ... args) {
-  vprint<wchar_t>(os, format_str, make_format_args<wformat_context>(args...));
+template <typename S, typename... Args,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+void print(std::basic_ostream<Char>& os, const S& format_str, Args&&... args) {
+  vprint(os, to_string_view(format_str),
+         fmt::make_args_checked<Args...>(format_str, args...));
 }
 FMT_END_NAMESPACE
 
 #endif  // FMT_OSTREAM_H_
```

### Comparing `libsonata-0.1.8/extlib/fmt/README.rst` & `libsonata-0.1.9/extlib/fmt/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,365 +2,217 @@
 =====
 
 .. image:: https://travis-ci.org/fmtlib/fmt.png?branch=master
    :target: https://travis-ci.org/fmtlib/fmt
 
 .. image:: https://ci.appveyor.com/api/projects/status/ehjkiefde6gucy1v
    :target: https://ci.appveyor.com/project/vitaut/fmt
-   
-.. image:: https://badges.gitter.im/Join%20Chat.svg
-   :alt: Join the chat at https://gitter.im/fmtlib/fmt
-   :target: https://gitter.im/fmtlib/fmt
-
-**{fmt}** is an open-source formatting library for C++.
-It can be used as a safe and fast alternative to (s)printf and IOStreams.
-
-`Documentation <http://fmtlib.net/latest/>`__
-
-This is a development branch that implements the C++ standards proposal `P0645
-Text Formatting <http://fmtlib.net/Text%20Formatting.html>`__.
-Released versions are available from the `Releases page
-<https://github.com/fmtlib/fmt/releases>`__.
+
+.. image:: https://oss-fuzz-build-logs.storage.googleapis.com/badges/fmt.svg
+   :alt: fmt is continuously fuzzed at oss-fuzz
+   :target: https://bugs.chromium.org/p/oss-fuzz/issues/list?\
+            colspec=ID%20Type%20Component%20Status%20Proj%20Reported%20Owner%20\
+            Summary&q=proj%3Dfmt&can=1
+
+.. image:: https://img.shields.io/badge/stackoverflow-fmt-blue.svg
+   :alt: Ask questions at StackOverflow with the tag fmt
+   :target: https://stackoverflow.com/questions/tagged/fmt
+
+**{fmt}** is an open-source formatting library providing a fast and safe
+alternative to C stdio and C++ iostreams.
+
+If you like this project, please consider donating to BYSOL,
+an initiative to help victims of political repressions in Belarus:
+https://www.facebook.com/donate/759400044849707/108388587646909/.
+
+`Documentation <https://fmt.dev>`__
+
+Q&A: ask questions on `StackOverflow with the tag fmt
+<https://stackoverflow.com/questions/tagged/fmt>`_.
+
+Try {fmt} in `Compiler Explorer <https://godbolt.org/z/Eq5763>`_.
 
 Features
 --------
 
-* Replacement-based `format API <http://fmtlib.net/dev/api.html>`_ with
-  positional arguments for localization.
-* `Format string syntax <http://fmtlib.net/dev/syntax.html>`_ similar to the one
-  of `str.format <https://docs.python.org/2/library/stdtypes.html#str.format>`_
-  in Python.
+* Simple `format API <https://fmt.dev/latest/api.html>`_ with positional arguments
+  for localization
+* Implementation of `C++20 std::format
+  <https://en.cppreference.com/w/cpp/utility/format>`__
+* `Format string syntax <https://fmt.dev/latest/syntax.html>`_ similar to Python's
+  `format <https://docs.python.org/3/library/stdtypes.html#str.format>`_
+* Fast IEEE 754 floating-point formatter with correct rounding, shortness and
+  round-trip guarantees
 * Safe `printf implementation
-  <http://fmtlib.net/latest/api.html#printf-formatting-functions>`_ including
-  the POSIX extension for positional arguments.
-* Support for user-defined types.
-* High speed: performance of the format API is close to that of glibc's `printf
-  <http://en.cppreference.com/w/cpp/io/c/fprintf>`_ and better than the
-  performance of IOStreams. See `Speed tests`_ and
-  `Fast integer to string conversion in C++
-  <http://zverovich.net/2013/09/07/integer-to-string-conversion-in-cplusplus.html>`_.
-* Small code size both in terms of source code (the minimum configuration
-  consists of just three header files, ``core.h``, ``format.h`` and
-  ``format-inl.h``) and compiled code. See `Compile time and code bloat`_.
-* Reliability: the library has an extensive set of `unit tests
-  <https://github.com/fmtlib/fmt/tree/master/test>`_.
+  <https://fmt.dev/latest/api.html#printf-formatting>`_ including the POSIX
+  extension for positional arguments
+* Extensibility: `support for user-defined types
+  <https://fmt.dev/latest/api.html#formatting-user-defined-types>`_
+* High performance: faster than common standard library implementations of
+  ``(s)printf``, iostreams, ``to_string`` and ``to_chars``, see `Speed tests`_
+  and `Converting a hundred million integers to strings per second
+  <http://www.zverovich.net/2020/06/13/fast-int-to-string-revisited.html>`_
+* Small code size both in terms of source code with the minimum configuration
+  consisting of just three files, ``core.h``, ``format.h`` and ``format-inl.h``,
+  and compiled code; see `Compile time and code bloat`_
+* Reliability: the library has an extensive set of `tests
+  <https://github.com/fmtlib/fmt/tree/master/test>`_ and is `continuously fuzzed
+  <https://bugs.chromium.org/p/oss-fuzz/issues/list?colspec=ID%20Type%20
+  Component%20Status%20Proj%20Reported%20Owner%20Summary&q=proj%3Dfmt&can=1>`_
 * Safety: the library is fully type safe, errors in format strings can be
   reported at compile time, automatic memory management prevents buffer overflow
-  errors.
+  errors
 * Ease of use: small self-contained code base, no external dependencies,
-  permissive BSD `license
+  permissive MIT `license
   <https://github.com/fmtlib/fmt/blob/master/LICENSE.rst>`_
-* `Portability <http://fmtlib.net/latest/index.html#portability>`_ with
-  consistent output across platforms and support for older compilers.
-* Clean warning-free codebase even on high warning levels
-  (``-Wall -Wextra -pedantic``).
-* Support for wide strings.
-* Optional header-only configuration enabled with the ``FMT_HEADER_ONLY`` macro.
+* `Portability <https://fmt.dev/latest/index.html#portability>`_ with
+  consistent output across platforms and support for older compilers
+* Clean warning-free codebase even on high warning levels such as
+  ``-Wall -Wextra -pedantic``
+* Locale-independence by default
+* Optional header-only configuration enabled with the ``FMT_HEADER_ONLY`` macro
 
-See the `documentation <http://fmtlib.net/latest/>`_ for more details.
+See the `documentation <https://fmt.dev>`_ for more details.
 
 Examples
 --------
 
-This prints ``Hello, world!`` to stdout:
+**Print to stdout** (`run <https://godbolt.org/z/Tevcjh>`_)
 
 .. code:: c++
 
-    fmt::print("Hello, {}!", "world");  // uses Python-like format string syntax
-    fmt::printf("Hello, %s!", "world"); // uses printf format string syntax
-
-Arguments can be accessed by position and arguments' indices can be repeated:
-
-.. code:: c++
-
-    std::string s = fmt::format("{0}{1}{0}", "abra", "cad");
-    // s == "abracadabra"
+    #include <fmt/core.h>
+    
+    int main() {
+      fmt::print("Hello, world!\n");
+    }
 
-Format strings can be checked at compile time:
+**Format a string** (`run <https://godbolt.org/z/oK8h33>`_)
 
 .. code:: c++
 
-    // test.cc
-    #define FMT_STRING_ALIAS 1
-    #include <fmt/format.h>
-    std::string s = format(fmt("{2}"), 42);
-
-.. code::
-
-    $ c++ -Iinclude -std=c++14 test.cc
-    ...
-    test.cc:4:17: note: in instantiation of function template specialization 'fmt::v5::format<S, int>' requested here
-    std::string s = format(fmt("{2}"), 42);
-                    ^
-    include/fmt/core.h:778:19: note: non-constexpr function 'on_error' cannot be used in a constant expression
-        ErrorHandler::on_error(message);
-                      ^
-    include/fmt/format.h:2226:16: note: in call to '&checker.context_->on_error(&"argument index out of range"[0])'
-          context_.on_error("argument index out of range");
-                   ^
+    std::string s = fmt::format("The answer is {}.", 42);
+    // s == "The answer is 42."
 
-{fmt} can be used as a safe portable replacement for ``itoa``
-(`godbolt <https://godbolt.org/g/NXmpU4>`_):
+**Format a string using positional arguments** (`run <https://godbolt.org/z/Yn7Txe>`_)
 
 .. code:: c++
 
-    fmt::memory_buffer buf;
-    format_to(buf, "{}", 42);    // replaces itoa(42, buffer, 10)
-    format_to(buf, "{:x}", 42);  // replaces itoa(42, buffer, 16)
-    // access the string using to_string(buf) or buf.data()
+    std::string s = fmt::format("I'd rather be {1} than {0}.", "right", "happy");
+    // s == "I'd rather be happy than right."
 
-Formatting of user-defined types is supported via a simple
-`extension API <http://fmtlib.net/latest/api.html#formatting-user-defined-types>`_:
+**Print chrono durations** (`run <https://godbolt.org/z/K8s4Mc>`_)
 
 .. code:: c++
 
-    #include "fmt/format.h"
-
-    struct date {
-      int year, month, day;
-    };
-
-    template <>
-    struct fmt::formatter<date> {
-      template <typename ParseContext>
-      constexpr auto parse(ParseContext &ctx) { return ctx.begin(); }
-
-      template <typename FormatContext>
-      auto format(const date &d, FormatContext &ctx) {
-        return format_to(ctx.begin(), "{}-{}-{}", d.year, d.month, d.day);
-      }
-    };
-
-    std::string s = fmt::format("The date is {}", date{2012, 12, 9});
-    // s == "The date is 2012-12-9"
-
-You can create your own functions similar to `format
-<http://fmtlib.net/latest/api.html#format>`_ and
-`print <http://fmtlib.net/latest/api.html#print>`_
-which take arbitrary arguments (`godbolt <https://godbolt.org/g/MHjHVf>`_):
+    #include <fmt/chrono.h>
 
-.. code:: c++
-
-    // Prints formatted error message.
-    void vreport_error(const char *format, fmt::format_args args) {
-      fmt::print("Error: ");
-      fmt::vprint(format, args);
-    }
-    template <typename... Args>
-    void report_error(const char *format, const Args & ... args) {
-      vreport_error(format, fmt::make_format_args(args...));
+    int main() {
+      using namespace std::literals::chrono_literals;
+      fmt::print("Default format: {} {}\n", 42s, 100ms);
+      fmt::print("strftime-like format: {:%H:%M:%S}\n", 3h + 15min + 30s);
     }
 
-    report_error("file not found: {}", path);
-
-Note that ``vreport_error`` is not parameterized on argument types which can
-improve compile times and reduce code size compared to fully parameterized version.
-
-Projects using this library
----------------------------
-
-* `0 A.D. <http://play0ad.com/>`_: A free, open-source, cross-platform real-time strategy game
-
-* `AMPL/MP <https://github.com/ampl/mp>`_:
-  An open-source library for mathematical programming
-  
-* `AvioBook <https://www.aviobook.aero/en>`_: A comprehensive aircraft operations suite
-
-* `CUAUV <http://cuauv.org/>`_: Cornell University's autonomous underwater vehicle
-
-* `HarpyWar/pvpgn <https://github.com/pvpgn/pvpgn-server>`_:
-  Player vs Player Gaming Network with tweaks
-
-* `KBEngine <http://kbengine.org/>`_: An open-source MMOG server engine
-
-* `Keypirinha <http://keypirinha.com/>`_: A semantic launcher for Windows
-
-* `Kodi <https://kodi.tv/>`_ (formerly xbmc): Home theater software
-
-* `Lifeline <https://github.com/peter-clark/lifeline>`_: A 2D game
-
-* `Drake <http://drake.mit.edu/>`_: A planning, control, and analysis toolbox
-  for nonlinear dynamical systems (MIT)
-
-* `Envoy <https://lyft.github.io/envoy/>`_: C++ L7 proxy and communication bus
-  (Lyft)
-
-* `FiveM <https://fivem.net/>`_: a modification framework for GTA V
-
-* `MongoDB Smasher <https://github.com/duckie/mongo_smasher>`_: A small tool to
-  generate randomized datasets
-
-* `OpenSpace <http://openspaceproject.com/>`_: An open-source astrovisualization
-  framework
-
-* `PenUltima Online (POL) <http://www.polserver.com/>`_:
-  An MMO server, compatible with most Ultima Online clients
-
-* `quasardb <https://www.quasardb.net/>`_: A distributed, high-performance,
-  associative database
-
-* `readpe <https://bitbucket.org/sys_dev/readpe>`_: Read Portable Executable
-
-* `redis-cerberus <https://github.com/HunanTV/redis-cerberus>`_: A Redis cluster proxy
-
-* `Saddy <https://github.com/mamontov-cpp/saddy-graphics-engine-2d>`_:
-  Small crossplatform 2D graphic engine
-
-* `Salesforce Analytics Cloud <http://www.salesforce.com/analytics-cloud/overview/>`_:
-  Business intelligence software
-
-* `Scylla <http://www.scylladb.com/>`_: A Cassandra-compatible NoSQL data store that can handle
-  1 million transactions per second on a single server
+Output::
 
-* `Seastar <http://www.seastar-project.org/>`_: An advanced, open-source C++ framework for
-  high-performance server applications on modern hardware
+    Default format: 42s 100ms
+    strftime-like format: 03:15:30
 
-* `spdlog <https://github.com/gabime/spdlog>`_: Super fast C++ logging library
+**Print a container** (`run <https://godbolt.org/z/MjsY7c>`_)
 
-* `Stellar <https://www.stellar.org/>`_: Financial platform
-
-* `Touch Surgery <https://www.touchsurgery.com/>`_: Surgery simulator
-
-* `TrinityCore <https://github.com/TrinityCore/TrinityCore>`_: Open-source MMORPG framework
-
-`More... <https://github.com/search?q=cppformat&type=Code>`_
-
-If you are aware of other projects using this library, please let me know
-by `email <mailto:victor.zverovich@gmail.com>`_ or by submitting an
-`issue <https://github.com/fmtlib/fmt/issues>`_.
-
-Motivation
-----------
-
-So why yet another formatting library?
-
-There are plenty of methods for doing this task, from standard ones like
-the printf family of function and IOStreams to Boost Format library and
-FastFormat. The reason for creating a new library is that every existing
-solution that I found either had serious issues or didn't provide
-all the features I needed.
-
-Printf
-~~~~~~
-
-The good thing about printf is that it is pretty fast and readily available
-being a part of the C standard library. The main drawback is that it
-doesn't support user-defined types. Printf also has safety issues although
-they are mostly solved with `__attribute__ ((format (printf, ...))
-<http://gcc.gnu.org/onlinedocs/gcc/Function-Attributes.html>`_ in GCC.
-There is a POSIX extension that adds positional arguments required for
-`i18n <https://en.wikipedia.org/wiki/Internationalization_and_localization>`_
-to printf but it is not a part of C99 and may not be available on some
-platforms.
+.. code:: c++
 
-IOStreams
-~~~~~~~~~
+    #include <vector>
+    #include <fmt/ranges.h>
 
-The main issue with IOStreams is best illustrated with an example:
+    int main() {
+      std::vector<int> v = {1, 2, 3};
+      fmt::print("{}\n", v);
+    }
 
-.. code:: c++
+Output::
 
-    std::cout << std::setprecision(2) << std::fixed << 1.23456 << "\n";
+    {1, 2, 3}
 
-which is a lot of typing compared to printf:
+**Check a format string at compile time**
 
 .. code:: c++
 
-    printf("%.2f\n", 1.23456);
+    std::string s = fmt::format(FMT_STRING("{:d}"), "don't panic");
 
-Matthew Wilson, the author of FastFormat, referred to this situation with
-IOStreams as "chevron hell". IOStreams doesn't support positional arguments
-by design.
-
-The good part is that IOStreams supports user-defined types and is safe
-although error reporting is awkward.
-
-Boost Format library
-~~~~~~~~~~~~~~~~~~~~
-
-This is a very powerful library which supports both printf-like format
-strings and positional arguments. Its main drawback is performance.
-According to various benchmarks it is much slower than other methods
-considered here. Boost Format also has excessive build times and severe
-code bloat issues (see `Benchmarks`_).
+This gives a compile-time error because ``d`` is an invalid format specifier for
+a string.
 
-FastFormat
-~~~~~~~~~~
+**Write a file from a single thread**
 
-This is an interesting library which is fast, safe and has positional
-arguments. However it has significant limitations, citing its author:
+.. code:: c++
 
-    Three features that have no hope of being accommodated within the
-    current design are:
+    #include <fmt/os.h>
 
-    * Leading zeros (or any other non-space padding)
-    * Octal/hexadecimal encoding
-    * Runtime width/alignment specification
+    int main() {
+      auto out = fmt::output_file("guide.txt");
+      out.print("Don't {}", "Panic");
+    }
 
-It is also quite big and has a heavy dependency, STLSoft, which might be
-too restrictive for using it in some projects.
+This can be `5 to 9 times faster than fprintf
+<http://www.zverovich.net/2020/08/04/optimal-file-buffer-size.html>`_.
 
-Loki SafeFormat
-~~~~~~~~~~~~~~~
+**Print with colors and text styles**
 
-SafeFormat is a formatting library which uses printf-like format strings
-and is type safe. It doesn't support user-defined types or positional
-arguments. It makes unconventional use of ``operator()`` for passing
-format arguments.
+.. code:: c++
 
-Tinyformat
-~~~~~~~~~~
+    #include <fmt/color.h>
 
-This library supports printf-like format strings and is very small and
-fast. Unfortunately it doesn't support positional arguments and wrapping
-it in C++98 is somewhat difficult. Also its performance and code compactness
-are limited by IOStreams.
+    int main() {
+      fmt::print(fg(fmt::color::crimson) | fmt::emphasis::bold,
+                 "Hello, {}!\n", "world");
+      fmt::print(fg(fmt::color::floral_white) | bg(fmt::color::slate_gray) |
+                 fmt::emphasis::underline, "Hello, {}!\n", "мир");
+      fmt::print(fg(fmt::color::steel_blue) | fmt::emphasis::italic,
+                 "Hello, {}!\n", "世界");
+    }
 
-Boost Spirit.Karma
-~~~~~~~~~~~~~~~~~~
+Output on a modern terminal:
 
-This is not really a formatting library but I decided to include it here
-for completeness. As IOStreams it suffers from the problem of mixing
-verbatim text with arguments. The library is pretty fast, but slower
-on integer formatting than ``fmt::Writer`` on Karma's own benchmark,
-see `Fast integer to string conversion in C++
-<http://zverovich.net/2013/09/07/integer-to-string-conversion-in-cplusplus.html>`_.
+.. image:: https://user-images.githubusercontent.com/
+           576385/88485597-d312f600-cf2b-11ea-9cbe-61f535a86e28.png
 
 Benchmarks
 ----------
 
 Speed tests
 ~~~~~~~~~~~
 
-The following speed tests results were generated by building
-``tinyformat_test.cpp`` on Ubuntu GNU/Linux 14.04.1 with
-``g++-4.8.2 -O3 -DSPEED_TEST -DHAVE_FORMAT``, and taking the best of three
-runs.  In the test, the format string ``"%0.10f:%04d:%+g:%s:%p:%c:%%\n"`` or
-equivalent is filled 2000000 times with output sent to ``/dev/null``; for
-further details see the `source
-<https://github.com/fmtlib/format-benchmark/blob/master/tinyformat_test.cpp>`_.
-
 ================= ============= ===========
 Library           Method        Run Time, s
 ================= ============= ===========
-libc              printf          1.35
-libc++            std::ostream    3.42
-fmt 534bff7       fmt::print      1.56
-tinyformat 2.0.1  tfm::printf     3.73
-Boost Format 1.54 boost::format   8.44
-Folly Format      folly::format   2.54
+libc              printf          1.04
+libc++            std::ostream    3.05
+{fmt} 6.1.1       fmt::print      0.75
+Boost Format 1.67 boost::format   7.24
+Folly Format      folly::format   2.23
 ================= ============= ===========
 
-As you can see ``boost::format`` is much slower than the alternative methods; this
-is confirmed by `other tests <http://accu.org/index.php/journals/1539>`_.
-Tinyformat is quite good coming close to IOStreams.  Unfortunately tinyformat
-cannot be faster than the IOStreams because it uses them internally.
-Performance of fmt is close to that of printf, being `faster than printf on integer
-formatting <http://zverovich.net/2013/09/07/integer-to-string-conversion-in-cplusplus.html>`_,
-but slower on floating-point formatting which dominates this benchmark.
+{fmt} is the fastest of the benchmarked methods, ~35% faster than ``printf``.
+
+The above results were generated by building ``tinyformat_test.cpp`` on macOS
+10.14.6 with ``clang++ -O3 -DNDEBUG -DSPEED_TEST -DHAVE_FORMAT``, and taking the
+best of three runs. In the test, the format string ``"%0.10f:%04d:%+g:%s:%p:%c:%%\n"``
+or equivalent is filled 2,000,000 times with output sent to ``/dev/null``; for
+further details refer to the `source
+<https://github.com/fmtlib/format-benchmark/blob/master/tinyformat_test.cpp>`_.
+
+{fmt} is up to 20-30x faster than ``std::ostringstream`` and ``sprintf`` on
+floating-point formatting (`dtoa-benchmark <https://github.com/fmtlib/dtoa-benchmark>`_)
+and faster than `double-conversion <https://github.com/google/double-conversion>`_ and
+`ryu <https://github.com/ulfjack/ryu>`_:
+
+.. image:: https://user-images.githubusercontent.com/576385/
+           95684665-11719600-0ba8-11eb-8e5b-972ff4e49428.png
+   :target: https://fmt.dev/unknown_mac64_clang12.0.html
 
 Compile time and code bloat
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The script `bloat-test.py
 <https://github.com/fmtlib/format-benchmark/blob/master/bloat-test.py>`_
 from `format-benchmark <https://github.com/fmtlib/format-benchmark>`_
@@ -373,54 +225,51 @@
 **Optimized build (-O3)**
 
 ============= =============== ==================== ==================
 Method        Compile Time, s Executable size, KiB Stripped size, KiB
 ============= =============== ==================== ==================
 printf                    2.6                   29                 26
 printf+string            16.4                   29                 26
-IOStreams                31.1                   59                 55
-fmt                      19.0                   37                 34
-tinyformat               44.0                  103                 97
+iostreams                31.1                   59                 55
+{fmt}                    19.0                   37                 34
 Boost Format             91.9                  226                203
 Folly Format            115.7                  101                 88
 ============= =============== ==================== ==================
 
-As you can see, fmt has 60% less overhead in terms of resulting binary code
-size compared to IOStreams and comes pretty close to ``printf``. Boost Format
+As you can see, {fmt} has 60% less overhead in terms of resulting binary code
+size compared to iostreams and comes pretty close to ``printf``. Boost Format
 and Folly Format have the largest overheads.
 
 ``printf+string`` is the same as ``printf`` but with extra ``<string>``
 include to measure the overhead of the latter.
 
 **Non-optimized build**
 
 ============= =============== ==================== ==================
 Method        Compile Time, s Executable size, KiB Stripped size, KiB
 ============= =============== ==================== ==================
 printf                    2.2                   33                 30
 printf+string            16.0                   33                 30
-IOStreams                28.3                   56                 52
-fmt                      18.2                   59                 50
-tinyformat               32.6                   88                 82
+iostreams                28.3                   56                 52
+{fmt}                    18.2                   59                 50
 Boost Format             54.1                  365                303
 Folly Format             79.9                  445                430
 ============= =============== ==================== ==================
 
-``libc``, ``lib(std)c++`` and ``libfmt`` are all linked as shared
-libraries to compare formatting function overhead only. Boost Format
-and tinyformat are header-only libraries so they don't provide any
-linkage options.
+``libc``, ``lib(std)c++`` and ``libfmt`` are all linked as shared libraries to
+compare formatting function overhead only. Boost Format is a
+header-only library so it doesn't provide any linkage options.
 
 Running the tests
 ~~~~~~~~~~~~~~~~~
 
 Please refer to `Building the library`__ for the instructions on how to build
 the library and run the unit tests.
 
-__ http://fmtlib.net/latest/usage.html#building-the-library
+__ https://fmt.dev/latest/usage.html#building-the-library
 
 Benchmarks reside in a separate repository,
 `format-benchmarks <https://github.com/fmtlib/format-benchmark>`_,
 so to run the benchmarks you first need to clone this repository and
 generate Makefiles with CMake::
 
     $ git clone --recursive https://github.com/fmtlib/format-benchmark.git
@@ -431,76 +280,227 @@
 
     $ make speed-test
 
 or the bloat test::
 
     $ make bloat-test
 
-FAQ
----
+Projects using this library
+---------------------------
+
+* `0 A.D. <https://play0ad.com/>`_: a free, open-source, cross-platform
+  real-time strategy game
+
+* `AMPL/MP <https://github.com/ampl/mp>`_:
+  an open-source library for mathematical programming
+
+* `Aseprite <https://github.com/aseprite/aseprite>`_:
+  animated sprite editor & pixel art tool 
+
+* `AvioBook <https://www.aviobook.aero/en>`_: a comprehensive aircraft
+  operations suite
+  
+* `Blizzard Battle.net <https://battle.net/>`_: an online gaming platform
+  
+* `Celestia <https://celestia.space/>`_: real-time 3D visualization of space
+
+* `Ceph <https://ceph.com/>`_: a scalable distributed storage system
+
+* `ccache <https://ccache.dev/>`_: a compiler cache
+
+* `ClickHouse <https://github.com/ClickHouse/ClickHouse>`_: analytical database
+  management system
+
+* `CUAUV <http://cuauv.org/>`_: Cornell University's autonomous underwater
+  vehicle
+
+* `Drake <https://drake.mit.edu/>`_: a planning, control, and analysis toolbox
+  for nonlinear dynamical systems (MIT)
+
+* `Envoy <https://lyft.github.io/envoy/>`_: C++ L7 proxy and communication bus
+  (Lyft)
+
+* `FiveM <https://fivem.net/>`_: a modification framework for GTA V
+
+* `Folly <https://github.com/facebook/folly>`_: Facebook open-source library
+
+* `HarpyWar/pvpgn <https://github.com/pvpgn/pvpgn-server>`_:
+  Player vs Player Gaming Network with tweaks
+
+* `KBEngine <https://github.com/kbengine/kbengine>`_: an open-source MMOG server
+  engine
+
+* `Keypirinha <https://keypirinha.com/>`_: a semantic launcher for Windows
+
+* `Kodi <https://kodi.tv/>`_ (formerly xbmc): home theater software
+
+* `Knuth <https://kth.cash/>`_: high-performance Bitcoin full-node
+
+* `Microsoft Verona <https://github.com/microsoft/verona>`_:
+  research programming language for concurrent ownership
+
+* `MongoDB <https://mongodb.com/>`_: distributed document database
+
+* `MongoDB Smasher <https://github.com/duckie/mongo_smasher>`_: a small tool to
+  generate randomized datasets
+
+* `OpenSpace <https://openspaceproject.com/>`_: an open-source
+  astrovisualization framework
+
+* `PenUltima Online (POL) <https://www.polserver.com/>`_:
+  an MMO server, compatible with most Ultima Online clients
+
+* `PyTorch <https://github.com/pytorch/pytorch>`_: an open-source machine
+  learning library
+
+* `quasardb <https://www.quasardb.net/>`_: a distributed, high-performance,
+  associative database
+  
+* `Quill <https://github.com/odygrd/quill>`_: asynchronous low-latency logging library
+
+* `QKW <https://github.com/ravijanjam/qkw>`_: generalizing aliasing to simplify
+  navigation, and executing complex multi-line terminal command sequences
+
+* `redis-cerberus <https://github.com/HunanTV/redis-cerberus>`_: a Redis cluster
+  proxy
+
+* `redpanda <https://vectorized.io/redpanda>`_: a 10x faster Kafka® replacement
+  for mission critical systems written in C++
+
+* `rpclib <http://rpclib.net/>`_: a modern C++ msgpack-RPC server and client
+  library
+
+* `Salesforce Analytics Cloud
+  <https://www.salesforce.com/analytics-cloud/overview/>`_:
+  business intelligence software
+
+* `Scylla <https://www.scylladb.com/>`_: a Cassandra-compatible NoSQL data store
+  that can handle 1 million transactions per second on a single server
+
+* `Seastar <http://www.seastar-project.org/>`_: an advanced, open-source C++
+  framework for high-performance server applications on modern hardware
+
+* `spdlog <https://github.com/gabime/spdlog>`_: super fast C++ logging library
+
+* `Stellar <https://www.stellar.org/>`_: financial platform
+
+* `Touch Surgery <https://www.touchsurgery.com/>`_: surgery simulator
+
+* `TrinityCore <https://github.com/TrinityCore/TrinityCore>`_: open-source
+  MMORPG framework
+
+* `Windows Terminal <https://github.com/microsoft/terminal>`_: the new Windows
+  terminal
+
+`More... <https://github.com/search?q=fmtlib&type=Code>`_
 
-Q: how can I capture formatting arguments and format them later?
+If you are aware of other projects using this library, please let me know
+by `email <mailto:victor.zverovich@gmail.com>`_ or by submitting an
+`issue <https://github.com/fmtlib/fmt/issues>`_.
+
+Motivation
+----------
+
+So why yet another formatting library?
+
+There are plenty of methods for doing this task, from standard ones like
+the printf family of function and iostreams to Boost Format and FastFormat
+libraries. The reason for creating a new library is that every existing
+solution that I found either had serious issues or didn't provide
+all the features I needed.
+
+printf
+~~~~~~
+
+The good thing about ``printf`` is that it is pretty fast and readily available
+being a part of the C standard library. The main drawback is that it
+doesn't support user-defined types. ``printf`` also has safety issues although
+they are somewhat mitigated with `__attribute__ ((format (printf, ...))
+<https://gcc.gnu.org/onlinedocs/gcc/Function-Attributes.html>`_ in GCC.
+There is a POSIX extension that adds positional arguments required for
+`i18n <https://en.wikipedia.org/wiki/Internationalization_and_localization>`_
+to ``printf`` but it is not a part of C99 and may not be available on some
+platforms.
+
+iostreams
+~~~~~~~~~
+
+The main issue with iostreams is best illustrated with an example:
+
+.. code:: c++
+
+    std::cout << std::setprecision(2) << std::fixed << 1.23456 << "\n";
 
-A: use ``std::tuple``:
+which is a lot of typing compared to printf:
 
 .. code:: c++
 
-   template <typename... Args>
-   auto capture(const Args&... args) {
-     return std::make_tuple(args...);
-   }
-
-   auto print_message = [](const auto&... args) {
-     fmt::print(args...);
-   };
-
-   // Capture and store arguments:
-   auto args = capture("{} {}", 42, "foo");
-   // Do formatting:
-   std::apply(print_message, args);
+    printf("%.2f\n", 1.23456);
+
+Matthew Wilson, the author of FastFormat, called this "chevron hell". iostreams
+don't support positional arguments by design.
+
+The good part is that iostreams support user-defined types and are safe although
+error handling is awkward.
+
+Boost Format
+~~~~~~~~~~~~
+
+This is a very powerful library which supports both ``printf``-like format
+strings and positional arguments. Its main drawback is performance. According to
+various, benchmarks it is much slower than other methods considered here. Boost
+Format also has excessive build times and severe code bloat issues (see
+`Benchmarks`_).
+
+FastFormat
+~~~~~~~~~~
+
+This is an interesting library which is fast, safe and has positional arguments.
+However, it has significant limitations, citing its author:
+
+    Three features that have no hope of being accommodated within the
+    current design are:
+
+    * Leading zeros (or any other non-space padding)
+    * Octal/hexadecimal encoding
+    * Runtime width/alignment specification
+
+It is also quite big and has a heavy dependency, STLSoft, which might be too
+restrictive for using it in some projects.
+
+Boost Spirit.Karma
+~~~~~~~~~~~~~~~~~~
+
+This is not really a formatting library but I decided to include it here for
+completeness. As iostreams, it suffers from the problem of mixing verbatim text
+with arguments. The library is pretty fast, but slower on integer formatting
+than ``fmt::format_to`` with format string compilation on Karma's own benchmark,
+see `Converting a hundred million integers to strings per second
+<http://www.zverovich.net/2020/06/13/fast-int-to-string-revisited.html>`_.
 
 License
 -------
 
-fmt is distributed under the BSD `license
+{fmt} is distributed under the MIT `license
 <https://github.com/fmtlib/fmt/blob/master/LICENSE.rst>`_.
 
-The `Format String Syntax
-<http://fmtlib.net/latest/syntax.html>`_
+Documentation License
+---------------------
+
+The `Format String Syntax <https://fmt.dev/latest/syntax.html>`_
 section in the documentation is based on the one from Python `string module
-documentation <https://docs.python.org/3/library/string.html#module-string>`_
-adapted for the current library. For this reason the documentation is
-distributed under the Python Software Foundation license available in
-`doc/python-license.txt
+documentation <https://docs.python.org/3/library/string.html#module-string>`_.
+For this reason the documentation is distributed under the Python Software
+Foundation license available in `doc/python-license.txt
 <https://raw.github.com/fmtlib/fmt/master/doc/python-license.txt>`_.
-It only applies if you distribute the documentation of fmt.
+It only applies if you distribute the documentation of {fmt}.
 
-Acknowledgments
----------------
+Maintainers
+-----------
 
-The fmt library is maintained by Victor Zverovich (`vitaut
+The {fmt} library is maintained by Victor Zverovich (`vitaut
 <https://github.com/vitaut>`_) and Jonathan Müller (`foonathan
 <https://github.com/foonathan>`_) with contributions from many other people.
 See `Contributors <https://github.com/fmtlib/fmt/graphs/contributors>`_ and
 `Releases <https://github.com/fmtlib/fmt/releases>`_ for some of the names.
 Let us know if your contribution is not listed or mentioned incorrectly and
 we'll make it right.
-
-The benchmark section of this readme file and the performance tests are taken
-from the excellent `tinyformat <https://github.com/c42f/tinyformat>`_ library
-written by Chris Foster.  Boost Format library is acknowledged transitively
-since it had some influence on tinyformat.
-Some ideas used in the implementation are borrowed from `Loki
-<http://loki-lib.sourceforge.net/>`_ SafeFormat and `Diagnostic API
-<http://clang.llvm.org/doxygen/classclang_1_1Diagnostic.html>`_ in
-`Clang <http://clang.llvm.org/>`_.
-Format string syntax and the documentation are based on Python's `str.format
-<http://docs.python.org/2/library/stdtypes.html#str.format>`_.
-Thanks `Doug Turnbull <https://github.com/softwaredoug>`_ for his valuable
-comments and contribution to the design of the type-safe API and
-`Gregory Czajkowski <https://github.com/gcflymoto>`_ for implementing binary
-formatting. Thanks `Ruslan Baratov <https://github.com/ruslo>`_ for comprehensive
-`comparison of integer formatting algorithms <https://github.com/ruslo/int-dec-format-tests>`_
-and useful comments regarding performance, `Boris Kaul <https://github.com/localvoid>`_ for
-`C++ counting digits benchmark <https://github.com/localvoid/cxx-benchmark-count-digits>`_.
-Thanks to `CarterLi <https://github.com/CarterLi>`_ for contributing various
-improvements to the code.
```

### Comparing `libsonata-0.1.8/extlib/nlohmann/nlohmann/json.hpp` & `libsonata-0.1.9/extlib/nlohmann/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/LICENSE` & `libsonata-0.1.9/extlib/HighFive/LICENSE`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataType.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataType.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -2,87 +2,79 @@
  *  Copyright (c), 2017, Adrien Devresse <adrien.devresse@epfl.ch>
  *
  *  Distributed under the Boost Software License, Version 1.0.
  *    (See accompanying file LICENSE_1_0.txt or copy at
  *          http://www.boost.org/LICENSE_1_0.txt)
  *
  */
-#ifndef H5EASY_BITS_XTENSOR_HPP
-#define H5EASY_BITS_XTENSOR_HPP
+#ifndef H5EASY_BITS_VECTOR_HPP
+#define H5EASY_BITS_VECTOR_HPP
 
 #include "../H5Easy.hpp"
 #include "H5Easy_misc.hpp"
 #include "H5Easy_scalar.hpp"
 
-#ifdef H5_USE_XTENSOR
-
 namespace H5Easy {
 
 namespace detail {
 
 template <class T>
-struct is_xtensor : std::false_type {};
+struct is_vector : std::false_type {};
 template <class T>
-struct is_xtensor<xt::xarray<T>> : std::true_type {};
-template <class T, size_t N>
-struct is_xtensor<xt::xtensor<T, N>> : std::true_type {};
+struct is_vector<std::vector<T>> : std::true_type {};
 
-template <typename T>
-struct io_impl<T, typename std::enable_if<is_xtensor<T>::value>::type> {
+using HighFive::details::get_dim_vector;
+using HighFive::details::type_of_array;
 
-    inline static std::vector<size_t> shape(const T& data) {
-        return std::vector<size_t>(data.shape().cbegin(), data.shape().cend());
-    }
+template <typename T>
+struct io_impl<T, typename std::enable_if<is_vector<T>::value>::type> {
 
     inline static DataSet dump(File& file,
                                const std::string& path,
                                const T& data,
                                const DumpOptions& options) {
-        using value_type = typename std::decay_t<T>::value_type;
-        DataSet dataset = initDataset<value_type>(file, path, shape(data), options);
-        dataset.write_raw(data.data());
+        using value_type = typename type_of_array<T>::type;
+        DataSet dataset = initDataset<value_type>(file, path, get_dim_vector(data), options);
+        dataset.write(data);
         if (options.flush()) {
             file.flush();
         }
         return dataset;
     }
 
     inline static T load(const File& file, const std::string& path) {
         DataSet dataset = file.getDataSet(path);
-        std::vector<size_t> dims = dataset.getDimensions();
-        T data = T::from_shape(dims);
-        dataset.read(data.data());
+        T data;
+        dataset.read(data);
         return data;
     }
 
-    inline static Attribute dumpAttribute(File& file,
-                                          const std::string& path,
-                                          const std::string& key,
-                                          const T& data,
-                                          const DumpOptions& options) {
-        using value_type = typename std::decay_t<T>::value_type;
-        Attribute attribute = initAttribute<value_type>(file, path, key, shape(data), options);
-        attribute.write_raw(data.data());
+   inline static Attribute dumpAttribute(File& file,
+                                         const std::string& path,
+                                         const std::string& key,
+                                         const T& data,
+                                         const DumpOptions& options) {
+        using value_type = typename type_of_array<T>::type;
+        std::vector<size_t> shape = get_dim_vector(data);
+        Attribute attribute = initAttribute<value_type>(file, path, key, shape, options);
+        attribute.write(data);
         if (options.flush()) {
             file.flush();
         }
         return attribute;
     }
 
     inline static T loadAttribute(const File& file,
                                   const std::string& path,
                                   const std::string& key) {
         DataSet dataset = file.getDataSet(path);
         Attribute attribute = dataset.getAttribute(key);
-        DataSpace dataspace = attribute.getSpace();
-        std::vector<size_t> dims = dataspace.getDimensions();
-        T data = T::from_shape(dims);
-        attribute.read(data.data());
+        T data;
+        attribute.read(data);
         return data;
     }
 };
 
 }  // namespace detail
 }  // namespace H5Easy
 
-#endif  // H5_USE_XTENSOR
-#endif  // H5EASY_BITS_XTENSOR_HPP
+#endif  // H5EASY_BITS_VECTOR_HPP
```

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Object.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Object.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5_definitions.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5_definitions.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Annotate_traits.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Annotate_traits.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Utils.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Utils.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Slice_traits.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Slice_traits.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Iterables_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Iterables_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5ConverterEigen_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Exception_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Exception_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Attribute_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Attribute_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Node_traits_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Node_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5DataType_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5DataType_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Node_traits.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Node_traits.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Reference_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Reference_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5PropertyList_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5PropertyList_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Converter_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Converter_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5FileDriver_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5FileDriver_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5DataSet_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5DataSet_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Dataspace_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Dataspace_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Object_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Object_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5Selection_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5Selection_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/bits/H5File_misc.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/bits/H5File_misc.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Easy.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Easy.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Reference.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Reference.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5PropertyList.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5PropertyList.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5File.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5File.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataSpace.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataSpace.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5DataSet.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5DataSet.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Selection.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Selection.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Group.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Group.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Attribute.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Attribute.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Exception.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Exception.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5Utility.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5Utility.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/include/highfive/H5FileDriver.hpp` & `libsonata-0.1.9/extlib/HighFive/include/highfive/H5FileDriver.hpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/extlib/HighFive/CMakeLists.txt` & `libsonata-0.1.9/extlib/HighFive/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/test_selection.cpp` & `libsonata-0.1.9/tests/test_selection.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/test_node_sets.cpp` & `libsonata-0.1.9/tests/test_node_sets.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -52,14 +52,26 @@
 
     SECTION("MissingNameInMaterialize") {
         const NodePopulation population("./data/nodes1.h5", "", "nodes-A");
         auto node_sets = R"({ "NodeSet0": { "attr-Y": 21 } })";
         NodeSets ns(node_sets);
         CHECK_THROWS_AS(ns.materialize("NONEXISTANT", population), SonataError);
     }
+
+    SECTION("OperatorMultipleClauses")
+    {
+        auto node_sets = R""({ "NodeSet0": {"attr-Y": {"has to ops": 3, "2nd": 3}} })"";
+        CHECK_THROWS_AS(NodeSets(node_sets), SonataError);
+    }
+
+    SECTION("OperatorObject")
+    {
+        auto node_sets = R""({ "NodeSet0": {"attr-Y": {"has to ops": {}}} })"";
+        CHECK_THROWS_AS(NodeSets(node_sets), SonataError);
+    }
 }
 
 TEST_CASE("NodeSetBasic") {
     const NodePopulation population("./data/nodes1.h5", "", "nodes-A");
     SECTION("BasicScalarInt") {
         auto node_sets = R"({ "NodeSet0": { "attr-Y": 21 } })";
         NodeSets ns(node_sets);
@@ -79,14 +91,65 @@
     SECTION("BasicScalarEnum") {
         auto node_sets = R"({ "NodeSet0": { "E-mapping-good": "C" } })";
         NodeSets ns(node_sets);
         Selection sel = ns.materialize("NodeSet0", population);
         CHECK(sel == Selection({{0, 1}, {2, 3}, {4, 6}}));
     }
 
+    SECTION("BasicScalarOperatorStringRegex") {
+        {
+            auto node_sets = R"({ "NodeSet0": {"E-mapping-good": {"$regex": "^[AC].*"}} })";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{0, 1}, {2, 6}}));
+        }
+
+        {
+            auto node_sets = R""({ "NodeSet0": {"attr-Z": {"$regex": "^(aa|bb|ff)"}} })"";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{0, 2}, {5,6}}));
+        }
+        {
+            auto node_sets = R""({ "NodeSet0": {"attr-Z": {"$op-does-not-exist": "dne"}} })"";
+            CHECK_THROWS_AS(NodeSets(node_sets), SonataError);
+        }
+    }
+
+    SECTION("BasicScalarOperatorNumeric") {
+        {
+            auto node_sets = R"({ "NodeSet0": {"attr-Y": {"$gt": 23}} })";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{3, 6}}));
+        }
+        {
+            auto node_sets = R"({ "NodeSet0": {"attr-Y": {"$lt": 23}} })";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{0, 2}}));
+        }
+        {
+            auto node_sets = R"({ "NodeSet0": {"attr-Y": {"$gte": 23}} })";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{2, 6}}));
+        }
+        {
+            auto node_sets = R"({ "NodeSet0": {"attr-Y": {"$lte": 23}} })";
+            NodeSets ns(node_sets);
+            Selection sel = ns.materialize("NodeSet0", population);
+            CHECK(sel == Selection({{0, 3}}));
+        }
+        {
+            auto node_sets = R""({ "NodeSet0": {"attr-Y": {"$op-does-not-exist": 3}} })"";
+            CHECK_THROWS_AS(NodeSets(node_sets), SonataError);
+        }
+    }
+
     SECTION("BasicScalarAnded") {
         auto node_sets = R"({"NodeSet0": {"E-mapping-good": "C",
                                           "attr-Y": [21, 22]
                                           }
                             })";
         NodeSets ns(node_sets);
         Selection sel = ns.materialize("NodeSet0", population);
@@ -172,14 +235,23 @@
             "location": ["layer4", "layer5"]
         },
         "V1_point_prime": {
             "population": "biophysical",
             "model_type": "point",
             "node_id": [1, 2, 3, 5, 7, 9]
         },
+        "power_number_test": {
+            "numeric_attribute_gt": { "$gt": 3 },
+            "numeric_attribute_lt": { "$lt": 3 },
+            "numeric_attribute_gte": { "$gte": 3 },
+            "numeric_attribute_lte": { "$lte": 3 }
+        },
+        "power_regex_test": {
+            "string_attr": { "$regex": "^[s][o]me value$" }
+        },
         "combined": ["bio_layer45", "V1_point_prime"]
     })";
 
     SECTION("toJSON") {
         NodeSets ns0(node_sets);
         std::string j = ns0.toJSON();
         NodeSets ns1(j);
@@ -187,11 +259,11 @@
 
         auto ns = NodeSets::fromFile("./data/node_sets.json");
         CHECK(ns.toJSON() == ns1.toJSON());
     }
 
     SECTION("names") {
         NodeSets ns(node_sets);
-        std::set<std::string> expected = {"bio_layer45", "V1_point_prime", "combined"};
+        std::set<std::string> expected = {"bio_layer45", "V1_point_prime", "combined", "power_number_test", "power_regex_test"};
         CHECK(ns.names() == expected);
     }
 }
```

### Comparing `libsonata-0.1.8/tests/test_report_reader.cpp` & `libsonata-0.1.9/tests/test_report_reader.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/test_edges.cpp` & `libsonata-0.1.9/tests/test_edges.cpp`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/test_nodes.cpp` & `libsonata-0.1.9/tests/test_nodes.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -173,14 +173,19 @@
         auto sel0 = population.matchAttributeValues("E-mapping-good", std::string("C"));
         CHECK(sel0.flatSize() == 4);
         CHECK(Selection::fromValues({0, 2, 4, 5}) == sel0);
 
         auto sel1 = population.matchAttributeValues("E-mapping-good",
                                                     std::string("does-not-exist"));
         CHECK(Selection({}) == sel1);
+
+        std::vector<std::string> strings {"C", "C", "C", "A", "B", "A"};
+        auto sel2 = population.matchAttributeValues("E-mapping-good", strings);
+        CHECK(sel2.flatSize() == 6);
+        CHECK(Selection({{0, 6}}) == sel2);
     }
 
     SECTION("Float attribute") {
         CHECK_THROWS_AS(population.matchAttributeValues("attr-X", 2), SonataError);
     }
 }
```

### Comparing `libsonata-0.1.8/tests/data/nodes1.h5` & `libsonata-0.1.9/tests/data/nodes1.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/somas.h5` & `libsonata-0.1.9/tests/data/somas.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/elements.h5` & `libsonata-0.1.9/tests/data/elements.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/spikes.h5` & `libsonata-0.1.9/tests/data/spikes.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/edges-no-index.h5` & `libsonata-0.1.9/tests/data/edges-no-index.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/edges1.h5` & `libsonata-0.1.9/tests/data/edges1.h5`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/tests/data/generate.py` & `libsonata-0.1.9/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/CMakeLists.txt` & `libsonata-0.1.9/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
 # =============================================================================
 # Targets
 # =============================================================================
 
 set(SONATA_SRC
     src/common.cpp
+    src/config.cpp
     src/edge_index.cpp
     src/edges.cpp
     src/hdf5_mutex.cpp
     src/node_sets.cpp
     src/nodes.cpp
     src/population.cpp
     src/report_reader.cpp
@@ -103,21 +104,23 @@
     set_target_properties(${TARGET}
         PROPERTIES
             POSITION_INDEPENDENT_CODE ON
             CXX_VISIBILITY_PRESET hidden
             OUTPUT_NAME "sonata"
     )
     target_include_directories(${TARGET}
+        PRIVATE $<TARGET_PROPERTY:ghc_filesystem,INTERFACE_INCLUDE_DIRECTORIES>
         PUBLIC
             $<BUILD_INTERFACE:${SONATA_INCLUDE_DIR}>
             $<INSTALL_INTERFACE:include>
     )
     target_compile_options(${TARGET}
         PRIVATE ${SONATA_COMPILE_OPTIONS}
     )
+
     if (ENABLE_COVERAGE)
         target_compile_options(${TARGET}
             PRIVATE -g -O0 --coverage -fprofile-arcs -ftest-coverage
         )
         target_link_libraries(${TARGET}
             PRIVATE gcov
         )
@@ -130,16 +133,16 @@
         SOVERSION ${SONATA_VERSION_ABI}
 )
 target_compile_definitions(sonata_shared
     PUBLIC SONATA_DLL
     PRIVATE SONATA_DLL_EXPORTS
 )
 target_link_libraries(sonata_shared
-    PRIVATE fmt::fmt-header-only
     PRIVATE HighFive
+    PRIVATE fmt::fmt-header-only
     PRIVATE nlohmann_json::nlohmann_json
 )
 
 target_compile_definitions(sonata_static
     PRIVATE FMT_HEADER_ONLY=1
 )
 target_include_directories(sonata_static
```

### Comparing `libsonata-0.1.8/PKG-INFO` & `libsonata-0.1.9/python/libsonata.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,412 +1,417 @@
 Metadata-Version: 2.1
 Name: libsonata
-Version: 0.1.8
+Version: 0.1.9
 Summary: SONATA files reader
 Home-page: https://github.com/BlueBrain/libsonata
 Author: Blue Brain Project, EPFL
 License: LGPLv3
-Description: |banner|
-        
-        |license| |coverage| |docs|
-        
-        libsonata
-        =========
-        
-        C++ / Python reader for SONATA circuit files:
-        `SONATA guide <https://github.com/AllenInstitute/sonata/blob/master/docs/SONATA_DEVELOPER_GUIDE.md>`__
-        
-        Installation
-        ------------
-        
-        Installing from PyPI
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           pip install libsonata
-        
-        Installing as a Python package, directly from GitHub
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           pip install git+https://github.com/BlueBrain/libsonata
-        
-        Building the C++ library
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: shell
-        
-           git clone git@github.com:BlueBrain/libsonata.git --recursive
-           cd libsonata
-           mkdir build && cd build
-           cmake  -DCMAKE_BUILD_TYPE=Release  -DEXTLIB_FROM_SUBMODULES=ON ..
-           make -j
-        
-        Usage (Python)
-        --------------
-        
-        Nodes
-        ~~~~~
-        
-        NodeStorage
-        +++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> import libsonata
-        
-           >>> nodes = libsonata.NodeStorage('path/to/H5/file')
-        
-           # list populations
-           >>> nodes.population_names
-        
-           # open population
-           >>> population = nodes.open_population(<name>)
-        
-        
-        NodePopulation
-        ++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # total number of nodes in the population
-           >>> population.size
-        
-           # attribute names
-           >>> population.attribute_names
-        
-           # get attribute value for single node, say 42
-           >>> population.get_attribute('mtype', 42)
-        
-           # ...or Selection of nodes (see below) => returns NumPy array with corresponding values
-           >>> selection = libsonata.Selection(values=[1, 5, 9, 42])  # nodes 1, 5, 9, 42
-           >>> mtypes = population.get_attribute('mtype', selection)
-           >>> list(zip(selection.flatten(), mtypes))
-           [(1, u'mtype_of_1'), (5, u'mtype_of_5'), (9, u'mtype_of_9'), (42, u'mtype_of_42')]
-        
-        
-        Selection
-        +++++++++
-        
-        List of element IDs (either `node_id`, or `edge_id`) where adjacent IDs are grouped for the sake of efficient HDF5 file access.
-        For instance, `{1, 2, 3, 5}` sequence becomes `{[1, 4), [5, 6)}`.
-        
-        `Selection` can be instantiated from:
-         - a sequence of scalar values (works for NumPy arrays as well)
-         - a sequence of pairs (interpreted as ranges above, works for N x 2 NumPy arrays as well)
-        
-        `EdgePopulation` connectivity queries (see below) return ``Selection``\ s as well.
-        
-        .. code-block:: pycon
-        
-           >>> selection = libsonata.Selection([1, 2, 3, 5])
-           >>> selection.ranges
-           [(1, 4), (5, 6)]
-        
-        
-        .. code-block:: pycon
-        
-           >>> selection = libsonata.Selection([(1, 4), (5, 6)])
-           >>> selection.flatten()
-           [1, 2, 3, 5]
-           >>> selection.flat_size
-           4
-           >>> bool(selection)
-           True
-        
-        
-        Edges
-        ~~~~~
-        
-        EdgeStorage
-        +++++++++++
-        
-        Population handling for `EdgeStorage` is analogous to `NodeStorage`:
-        
-        .. code-block:: pycon
-        
-           >>> edges = libsonata.EdgeStorage('path/to/H5/file')
-        
-           # list populations
-           >>> edges.population_names
-        
-           # open population
-           >>> population = edges.open_population(<name>)
-        
-        
-        EdgePopulation
-        ++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # total number of edges in the population
-           >>> population.size
-        
-           # attribute names
-           >>> population.attribute_names
-        
-           # get attribute value for single edge, say 123
-           >>> population.get_attribute('delay', 123)
-        
-           # ...or Selection of edges => returns NumPy array with corresponding values
-           >>> selection = libsonata.Selection([1, 5, 9])
-           >>> population.get_attribute('delay', selection) # returns delays for edges 1, 5, 9
-        
-        
-        ...with additional methods for querying connectivity, where the results are selections that can be applied like above
-        
-        .. code-block:: pycon
-        
-           # get source / target node ID for the 42nd edge:
-           >>> population.source_node(42)
-           >>> population.target_node(42)
-        
-           # query connectivity (result is Selection object)
-           >>> selection_to_1 = population.afferent_edges(1)  # all edges with target node_id 1
-           >>> population.target_nodes(selection_to_1)  # since selection only contains edges
-                                                        # targeting node_id 1 the result will be a
-                                                        # numpy array of all 1's
-           >>> selection_from_2 = population.efferent_edges(2)  # all edges sourced from node_id 2
-           >>> selection = population.connecting_edges(2, 1)  # this selection is all edges from
-                                                              # node_id 2 to node_id 1
-        
-           # ...or their vectorized analogues
-           >>> selection = population.afferent_edges([1, 2, 3])
-           >>> selection = population.efferent_edges([1, 2, 3])
-           >>> selection = population.connecting_edges([1, 2, 3], [4, 5, 6])
-        
-        
-        Reports
-        ~~~~~~~
-        
-        SpikeReader
-        +++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> import libsonata
-        
-           >>> spikes = libsonata.SpikeReader('path/to/H5/file')
-        
-           # list populations
-           >>> spikes.get_populations_names()
-        
-           # open population
-           >>> population = spikes['<name>']
-        
-        
-        SpikePopulation
-        +++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get all spikes [(node_id, timestep)]
-           >>> population.get()
-           [(5, 0.1), (2, 0.2), (3, 0.3), (2, 0.7), (3, 1.3)]
-        
-           # get all spikes betwen tstart and tstop
-           >>> population.get(tstart=0.2, tstop=1.0)
-           [(2, 0.2), (3, 0.3), (2, 0.7)]
-        
-           # get spikes attribute sorting (by_time, by_id, none)
-           >>> population.sorting
-           'by_time'
-        
-           Pandas can be used to create a dataframe and get a better representation of the data
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           data = population.get()
-           df = pandas.DataFrame(data=data, columns=['ids', 'times']).set_index('times')
-           print(df)
-                  ids
-           times
-           0.1      5
-           0.2      2
-           0.3      3
-           0.7      2
-           1.3      3
-        
-        
-        SomaReportReader
-        ++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> somas = libsonata.SomaReportReader('path/to/H5/file')
-        
-           # list populations
-           >>> somas.get_populations_names()
-        
-           # open population
-           >>> population_somas = somas['<name>']
-        
-        
-        SomaReportPopulation
-        ++++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get times (tstart, tstop, dt)
-           >>> population_somas.times
-           (0.0, 1.0, 0.1)
-        
-           # get unit attributes
-           >>> population_somas.time_units
-           'ms'
-           >>> population_somas.data_units
-           'mV'
-        
-           # node_ids sorted?
-           >>> population_somas.sorted
-           True
-        
-           # get a list of all node ids in the selected population
-           >>> population_somas.get_node_ids()
-           [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
-        
-           # get the DataFrame of the node_id values for the timesteps between tstart and tstop
-           >>> data_frame = population_somas.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
-        
-           # get the data values
-           >>> data_frame.data
-           [[13.8, 14.8], [13.9, 14.9]]
-        
-           # get the list of timesteps
-           >>> data_frame.times
-           [0.8, 0.9]
-        
-           # get the list of node ids
-           >>> data_frame.ids
-           [13, 14]
-        
-        
-        Once again, pandas can be used to create a dataframe using the data, ids and times lists
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           df = pandas.DataFrame(data_frame.data, columns=data_frame.ids, index=data_frame.times)
-           print(df)
-                  13    14
-           0.8  13.8  14.8
-           0.9  13.9  14.9
-        
-        
-        ElementReportReader
-        +++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           >>> elements = libsonata.ElementReportReader('path/to/H5/file')
-        
-           # list populations
-           >>> elements.get_populations_names()
-        
-           # open population
-           >>> population_elements = elements['<name>']
-        
-        
-        ElementReportPopulation
-        +++++++++++++++++++++++
-        
-        .. code-block:: pycon
-        
-           # get times (tstart, tstop, dt)
-           >>> population_elements.times
-           (0.0, 4.0, 0.2)
-        
-           >>> population_elements.get_node_ids()
-           [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
-        
-           # get the DataFrame of the node_id values for the timesteps between tstart and tstop
-           >>> data_frame = population_elements.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
-        
-           # get the data values (list of list of floats with data[time_index][element_index])
-           >>> data_frame.data
-           [[46.0, 46.1, 46.2, 46.3, 46.4, 46.5, 46.6, 46.7, 46.8, 46.9], [56.0, 56.1, 56.2, 56.3, 56.4, 56.5, 56.6, 56.7, 56.8, 56.9]]
-        
-           # get the list of timesteps
-           >>> data_frame.times
-           [0.8, 1.0]
-        
-           # get the list of (node id, element_id)
-           >>> data_frame.ids
-           [(13, 30), (13, 30), (13, 31), (13, 31), (13, 32), (14, 32), (14, 33), (14, 33), (14, 34), (14, 34)]
-        
-        
-        The same way than with spikes and soma reports, pandas can be used to get a better representation of the data
-        
-        .. code-block:: pycon
-        
-           >>> import pandas
-        
-           df = pandas.DataFrame(data_frame.data, columns=pandas.MultiIndex.from_tuples(data_frame.ids), index=data_frame.times)
-           print(df)
-                  13                            14
-                  30    30    31    31    32    32    33    33    34    34
-           0.8  46.0  46.1  46.2  46.3  46.4  46.5  46.6  46.7  46.8  46.9
-           1.0  56.0  56.1  56.2  56.3  56.4  56.5  56.6  56.7  56.8  56.9
-        
-        For big datasets, using numpy arrays could greatly improve the performance
-        
-        .. code-block:: pycon
-        
-           >>> import numpy
-        
-           np_data = numpy.asarray(data_frame.data)
-           np_ids = numpy.asarray(data_frame.ids).T
-           np_times = numpy.asarray(data_frame.times)
-        
-           df = pandas.DataFrame(np_data, columns=pandas.MultiIndex.from_arrays(np_ids), index=np_times)
-        
-        
-        Acknowledgements
-        ----------------
-        
-        This project/research has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 785907 (Human Brain Project SGA2).
-        
-        
-        License
-        -------
-        
-        libsonata is distributed under the terms of the GNU Lesser General Public License version 3,
-        unless noted otherwise, for example, for external dependencies.
-        Refer to `COPYING.LESSER` and `COPYING` files for details.
-        
-        Copyright (C) 2018-2020, Blue Brain Project/EPFL and contributors.
-        
-        libsonata is free software: you can redistribute it and/or modify
-        it under the terms of the GNU Lesser General Public License version 3
-        as published by the Free Software Foundation.
-        
-        libsonata is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Lesser General Public License for more details.
-        
-        You should have received a copy of the GNU Lesser General Public License
-        along with libsonata.  If not, see <https://www.gnu.org/licenses/>.
-        
-        
-        .. |license| image:: https://img.shields.io/pypi/l/libsonata
-                        :target: https://github.com/BlueBrain/libsonata/blob/master/COPYING.LESSER
-        
-        .. |coverage| image:: https://coveralls.io/repos/github/BlueBrain/libsonata/badge.svg
-                         :target: https://coveralls.io/github/BlueBrain/libsonata
-        
-        .. |docs| image:: https://readthedocs.org/projects/libsonata/badge/?version=latest
-                     :target: https://libsonata.readthedocs.io/
-                     :alt: documentation status
-        
-        .. substitutions
-        .. |banner| image:: docs/source/_images/libSonataLogo.jpg
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
+License-File: COPYING
+License-File: COPYING.LESSER
+
+|banner|
+
+|license| |coverage| |docs|
+
+libsonata
+=========
+
+C++ / Python reader for SONATA circuit files:
+`SONATA guide <https://github.com/AllenInstitute/sonata/blob/master/docs/SONATA_DEVELOPER_GUIDE.md>`__
+
+Installation
+------------
+
+Installing from PyPI
+~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   pip install libsonata
+
+Installing as a Python package, directly from GitHub
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   pip install git+https://github.com/BlueBrain/libsonata
+
+Building the C++ library
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: shell
+
+   git clone git@github.com:BlueBrain/libsonata.git --recursive
+   cd libsonata
+   mkdir build && cd build
+   cmake  -DCMAKE_BUILD_TYPE=Release  -DEXTLIB_FROM_SUBMODULES=ON ..
+   make -j
+
+Usage (Python)
+--------------
+
+Nodes
+~~~~~
+
+NodeStorage
++++++++++++
+
+.. code-block:: pycon
+
+   >>> import libsonata
+
+   >>> nodes = libsonata.NodeStorage('path/to/H5/file')
+
+   # list populations
+   >>> nodes.population_names
+
+   # open population
+   >>> population = nodes.open_population(<name>)
+
+
+NodePopulation
+++++++++++++++
+
+.. code-block:: pycon
+
+   # total number of nodes in the population
+   >>> population.size
+
+   # attribute names
+   >>> population.attribute_names
+
+   # get attribute value for single node, say 42
+   >>> population.get_attribute('mtype', 42)
+
+   # ...or Selection of nodes (see below) => returns NumPy array with corresponding values
+   >>> selection = libsonata.Selection(values=[1, 5, 9, 42])  # nodes 1, 5, 9, 42
+   >>> mtypes = population.get_attribute('mtype', selection)
+   >>> list(zip(selection.flatten(), mtypes))
+   [(1, u'mtype_of_1'), (5, u'mtype_of_5'), (9, u'mtype_of_9'), (42, u'mtype_of_42')]
+
+
+Selection
++++++++++
+
+List of element IDs (either `node_id`, or `edge_id`) where adjacent IDs are grouped for the sake of efficient HDF5 file access.
+For instance, `{1, 2, 3, 5}` sequence becomes `{[1, 4), [5, 6)}`.
+
+`Selection` can be instantiated from:
+ - a sequence of scalar values (works for NumPy arrays as well)
+ - a sequence of pairs (interpreted as ranges above, works for N x 2 NumPy arrays as well)
+
+`EdgePopulation` connectivity queries (see below) return ``Selection``\ s as well.
+
+.. code-block:: pycon
+
+   >>> selection = libsonata.Selection([1, 2, 3, 5])
+   >>> selection.ranges
+   [(1, 4), (5, 6)]
+
+
+.. code-block:: pycon
+
+   >>> selection = libsonata.Selection([(1, 4), (5, 6)])
+   >>> selection.flatten()
+   [1, 2, 3, 5]
+   >>> selection.flat_size
+   4
+   >>> bool(selection)
+   True
+
+
+Edges
+~~~~~
+
+EdgeStorage
++++++++++++
+
+Population handling for `EdgeStorage` is analogous to `NodeStorage`:
+
+.. code-block:: pycon
+
+   >>> edges = libsonata.EdgeStorage('path/to/H5/file')
+
+   # list populations
+   >>> edges.population_names
+
+   # open population
+   >>> population = edges.open_population(<name>)
+
+
+EdgePopulation
+++++++++++++++
+
+.. code-block:: pycon
+
+   # total number of edges in the population
+   >>> population.size
+
+   # attribute names
+   >>> population.attribute_names
+
+   # get attribute value for single edge, say 123
+   >>> population.get_attribute('delay', 123)
+
+   # ...or Selection of edges => returns NumPy array with corresponding values
+   >>> selection = libsonata.Selection([1, 5, 9])
+   >>> population.get_attribute('delay', selection) # returns delays for edges 1, 5, 9
+
+
+...with additional methods for querying connectivity, where the results are selections that can be applied like above
+
+.. code-block:: pycon
+
+   # get source / target node ID for the 42nd edge:
+   >>> population.source_node(42)
+   >>> population.target_node(42)
+
+   # query connectivity (result is Selection object)
+   >>> selection_to_1 = population.afferent_edges(1)  # all edges with target node_id 1
+   >>> population.target_nodes(selection_to_1)  # since selection only contains edges
+                                                # targeting node_id 1 the result will be a
+                                                # numpy array of all 1's
+   >>> selection_from_2 = population.efferent_edges(2)  # all edges sourced from node_id 2
+   >>> selection = population.connecting_edges(2, 1)  # this selection is all edges from
+                                                      # node_id 2 to node_id 1
+
+   # ...or their vectorized analogues
+   >>> selection = population.afferent_edges([1, 2, 3])
+   >>> selection = population.efferent_edges([1, 2, 3])
+   >>> selection = population.connecting_edges([1, 2, 3], [4, 5, 6])
+
+
+Reports
+~~~~~~~
+
+SpikeReader
++++++++++++
+
+.. code-block:: pycon
+
+   >>> import libsonata
+
+   >>> spikes = libsonata.SpikeReader('path/to/H5/file')
+
+   # list populations
+   >>> spikes.get_populations_names()
+
+   # open population
+   >>> population = spikes['<name>']
+
+
+SpikePopulation
++++++++++++++++
+
+.. code-block:: pycon
+
+   # get all spikes [(node_id, timestep)]
+   >>> population.get()
+   [(5, 0.1), (2, 0.2), (3, 0.3), (2, 0.7), (3, 1.3)]
+
+   # get all spikes betwen tstart and tstop
+   >>> population.get(tstart=0.2, tstop=1.0)
+   [(2, 0.2), (3, 0.3), (2, 0.7)]
+
+   # get spikes attribute sorting (by_time, by_id, none)
+   >>> population.sorting
+   'by_time'
+
+   Pandas can be used to create a dataframe and get a better representation of the data
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   data = population.get()
+   df = pandas.DataFrame(data=data, columns=['ids', 'times']).set_index('times')
+   print(df)
+          ids
+   times
+   0.1      5
+   0.2      2
+   0.3      3
+   0.7      2
+   1.3      3
+
+
+SomaReportReader
+++++++++++++++++
+
+.. code-block:: pycon
+
+   >>> somas = libsonata.SomaReportReader('path/to/H5/file')
+
+   # list populations
+   >>> somas.get_populations_names()
+
+   # open population
+   >>> population_somas = somas['<name>']
+
+
+SomaReportPopulation
+++++++++++++++++++++
+
+.. code-block:: pycon
+
+   # get times (tstart, tstop, dt)
+   >>> population_somas.times
+   (0.0, 1.0, 0.1)
+
+   # get unit attributes
+   >>> population_somas.time_units
+   'ms'
+   >>> population_somas.data_units
+   'mV'
+
+   # node_ids sorted?
+   >>> population_somas.sorted
+   True
+
+   # get a list of all node ids in the selected population
+   >>> population_somas.get_node_ids()
+   [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
+
+   # get the DataFrame of the node_id values for the timesteps between tstart and tstop
+   >>> data_frame = population_somas.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
+
+   # get the data values
+   >>> data_frame.data
+   [[13.8, 14.8], [13.9, 14.9]]
+
+   # get the list of timesteps
+   >>> data_frame.times
+   [0.8, 0.9]
+
+   # get the list of node ids
+   >>> data_frame.ids
+   [13, 14]
+
+
+Once again, pandas can be used to create a dataframe using the data, ids and times lists
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   df = pandas.DataFrame(data_frame.data, columns=data_frame.ids, index=data_frame.times)
+   print(df)
+          13    14
+   0.8  13.8  14.8
+   0.9  13.9  14.9
+
+
+ElementReportReader
++++++++++++++++++++
+
+.. code-block:: pycon
+
+   >>> elements = libsonata.ElementReportReader('path/to/H5/file')
+
+   # list populations
+   >>> elements.get_populations_names()
+
+   # open population
+   >>> population_elements = elements['<name>']
+
+
+ElementReportPopulation
++++++++++++++++++++++++
+
+.. code-block:: pycon
+
+   # get times (tstart, tstop, dt)
+   >>> population_elements.times
+   (0.0, 4.0, 0.2)
+
+   >>> population_elements.get_node_ids()
+   [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
+
+   # get the DataFrame of the node_id values for the timesteps between tstart and tstop
+   >>> data_frame = population_elements.get(node_ids=[13, 14], tstart=0.8, tstop=1.0)
+
+   # get the data values (list of list of floats with data[time_index][element_index])
+   >>> data_frame.data
+   [[46.0, 46.1, 46.2, 46.3, 46.4, 46.5, 46.6, 46.7, 46.8, 46.9], [56.0, 56.1, 56.2, 56.3, 56.4, 56.5, 56.6, 56.7, 56.8, 56.9]]
+
+   # get the list of timesteps
+   >>> data_frame.times
+   [0.8, 1.0]
+
+   # get the list of (node id, element_id)
+   >>> data_frame.ids
+   [(13, 30), (13, 30), (13, 31), (13, 31), (13, 32), (14, 32), (14, 33), (14, 33), (14, 34), (14, 34)]
+
+
+The same way than with spikes and soma reports, pandas can be used to get a better representation of the data
+
+.. code-block:: pycon
+
+   >>> import pandas
+
+   df = pandas.DataFrame(data_frame.data, columns=pandas.MultiIndex.from_tuples(data_frame.ids), index=data_frame.times)
+   print(df)
+          13                            14
+          30    30    31    31    32    32    33    33    34    34
+   0.8  46.0  46.1  46.2  46.3  46.4  46.5  46.6  46.7  46.8  46.9
+   1.0  56.0  56.1  56.2  56.3  56.4  56.5  56.6  56.7  56.8  56.9
+
+For big datasets, using numpy arrays could greatly improve the performance
+
+.. code-block:: pycon
+
+   >>> import numpy
+
+   np_data = numpy.asarray(data_frame.data)
+   np_ids = numpy.asarray(data_frame.ids).T
+   np_times = numpy.asarray(data_frame.times)
+
+   df = pandas.DataFrame(np_data, columns=pandas.MultiIndex.from_arrays(np_ids), index=np_times)
+
+
+Acknowledgements
+----------------
+The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
+
+This project/research has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 785907 (Human Brain Project SGA2).
+
+
+License
+-------
+
+libsonata is distributed under the terms of the GNU Lesser General Public License version 3,
+unless noted otherwise, for example, for external dependencies.
+Refer to `COPYING.LESSER` and `COPYING` files for details.
+
+Copyright (c) 2018-2021 Blue Brain Project/EPFL
+
+libsonata is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License version 3
+as published by the Free Software Foundation.
+
+libsonata is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License
+along with libsonata.  If not, see <https://www.gnu.org/licenses/>.
+
+
+.. |license| image:: https://img.shields.io/pypi/l/libsonata
+                :target: https://github.com/BlueBrain/libsonata/blob/master/COPYING.LESSER
+
+.. |coverage| image:: https://coveralls.io/repos/github/BlueBrain/libsonata/badge.svg
+                 :target: https://coveralls.io/github/BlueBrain/libsonata
+
+.. |docs| image:: https://readthedocs.org/projects/libsonata/badge/?version=latest
+             :target: https://libsonata.readthedocs.io/
+             :alt: documentation status
+
+.. substitutions
+.. |banner| image:: docs/source/_images/libSonataLogo.jpg
+
+
```

### Comparing `libsonata-0.1.8/COPYING.LESSER` & `libsonata-0.1.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/.clang-format` & `libsonata-0.1.9/.clang-format`

 * *Files identical despite different names*

### Comparing `libsonata-0.1.8/COPYING` & `libsonata-0.1.9/COPYING`

 * *Files identical despite different names*

