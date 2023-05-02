# Comparing `tmp/libmav-0.0.1.tar.gz` & `tmp/libmav-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmav-0.0.1.tar", last modified: Tue Apr 11 17:43:05 2023, max compression
+gzip compressed data, was "libmav-0.0.2.tar", last modified: Tue May  2 09:42:04 2023, max compression
```

## Comparing `libmav-0.0.1.tar` & `libmav-0.0.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.030577 libmav-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-11 17:42:53.000000 libmav-0.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-11 17:42:53.000000 libmav-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 17:42:53.000000 libmav-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 17:43:05.030577 libmav-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-11 17:42:53.000000 libmav-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 17:42:54.000000 libmav-0.0.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.018577 libmav-0.0.1/libmav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 17:43:04.000000 libmav-0.0.1/libmav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-11 17:43:05.000000 libmav-0.0.1/libmav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:43:04.000000 libmav-0.0.1/libmav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:43:04.000000 libmav-0.0.1/libmav.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 17:43:04.000000 libmav-0.0.1/libmav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 17:43:04.000000 libmav-0.0.1/libmav.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.018577 libmav-0.0.1/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.014577 libmav-0.0.1/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.022577 libmav-0.0.1/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-11 17:42:53.000000 libmav-0.0.1/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-11 17:42:53.000000 libmav-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:43:05.030577 libmav-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-11 17:42:53.000000 libmav-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_Connection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_Message.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_MessageDefinition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_MessageSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_NetworkRuntime.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_PhysicalNetwork.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-11 17:42:53.000000 libmav-0.0.1/src/bind_utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/libmav/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.014577 libmav-0.0.1/src/libmav/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/libmav/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/libmav/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/cmake/mavConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/gcovr.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.014577 libmav-0.0.1/src/libmav/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/libmav/include/mav/
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/BuiltInMessages.h
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/Connection.h
--rw-r--r--   0 runner    (1001) docker     (123)    22611 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/Message.h
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/MessageDefinition.h
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/MessageFieldIterator.h
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/MessageSet.h
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/Network.h
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/Serial.h
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/TCPClient.h
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/TCPServer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/UDPClient.h
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/UDPServer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.026577 libmav-0.0.1/src/libmav/include/mav/rapidxml/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/rapidxml/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)   120937 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_print.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/include/mav/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:43:05.030577 libmav-0.0.1/src/libmav/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/Message.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/MessageDefinition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/MessageFieldIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/MessageSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/Network.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/TCP.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/UDP.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   318437 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/doctest.h
--rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/minimal.h
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 17:42:54.000000 libmav-0.0.1/src/libmav/tests/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.218502 libmav-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 09:41:50.000000 libmav-0.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-02 09:41:50.000000 libmav-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 09:41:50.000000 libmav-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-02 09:42:04.218502 libmav-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-02 09:41:50.000000 libmav-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 09:41:51.000000 libmav-0.0.2/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.194502 libmav-0.0.2/libmav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-02 09:42:04.000000 libmav-0.0.2/libmav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 09:42:04.000000 libmav-0.0.2/libmav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:42:04.000000 libmav-0.0.2/libmav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:42:03.000000 libmav-0.0.2/libmav.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 09:42:04.000000 libmav-0.0.2/libmav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 09:42:04.000000 libmav-0.0.2/libmav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.194502 libmav-0.0.2/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.190502 libmav-0.0.2/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.202502 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.206502 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.206502 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.206502 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.206502 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.206502 libmav-0.0.2/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.210502 libmav-0.0.2/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 09:41:50.000000 libmav-0.0.2/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 09:41:50.000000 libmav-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:42:04.218502 libmav-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 09:41:50.000000 libmav-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.210502 libmav-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_Connection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_Message.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_MessageDefinition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_MessageSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_NetworkRuntime.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_PhysicalNetwork.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-02 09:41:50.000000 libmav-0.0.2/src/bind_utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.210502 libmav-0.0.2/src/libmav/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.190502 libmav-0.0.2/src/libmav/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.210502 libmav-0.0.2/src/libmav/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.210502 libmav-0.0.2/src/libmav/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/cmake/mavConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/gcovr.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.190502 libmav-0.0.2/src/libmav/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.214502 libmav-0.0.2/src/libmav/include/mav/
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/BuiltInMessages.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/Connection.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22611 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/Message.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/MessageDefinition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/MessageFieldIterator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/MessageSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/Network.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/Serial.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/TCPClient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/TCPServer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/UDPClient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/UDPServer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.218502 libmav-0.0.2/src/libmav/include/mav/rapidxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/rapidxml/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   120937 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_print.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/include/mav/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:42:04.218502 libmav-0.0.2/src/libmav/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/Message.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/MessageDefinition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/MessageFieldIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/MessageSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/Network.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/TCP.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/UDP.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   318437 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/doctest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/minimal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 09:41:51.000000 libmav-0.0.2/src/libmav/tests/test_main.cpp
```

### Comparing `libmav-0.0.1/CMakeLists.txt` & `libmav-0.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/LICENSE` & `libmav-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/PKG-INFO` & `libmav-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-Metadata-Version: 2.1
-Name: libmav
-Version: 0.0.1
-Summary: A library for the MAVLink protocol
-Author: Auterion
-Author-email: success@auterion.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # Libmav Python
 
 Native python bindings for the [libmav](https://github.com/ThomasDebrunner/libmav) library.
+libmav-python is a runtime defined low-level MAVLink library. 
+
+In comparison to other python MAVLink libaries, it has certain advantages:
+
+- **Runtime defined message set.** No need to recompile on message set change or custom messages
+- **Implemented in C++.** Much faster than pure python
+- **Simple, pythonic API.** No need to learn a new API or asyncio, just use python
+
 
 ## Installation
 
 ```
 pip install libmav
 ```
 
@@ -33,15 +30,15 @@
         <message>
             ...
         </message>
     </messages>
 </mavlink>''')
 
 # Create a message from the message set
-message = self.message_set.create('MY_PROTOCOL_MESSAGE')
+message = message_set.create('MY_PROTOCOL_MESSAGE')
 
 # Set fields of the message individually
 message['my_numeric_field'] = 1
 message['my_char_array_field'] = 'Hello world'
 message['my_float_array_field'] = [1.0, 2.0, 3.0]
 message['my_int_array_field'] = [4, 5, 6]
 
@@ -91,15 +88,15 @@
 # This avoids the race condition between us sending and then waiting for reception
 expectation = connection.receive("PARAM_VALUE")
 connection.send(our_param_request_message)
 received_message = connection.receive(expectation, 1000)
 
 
 # Connect to a Serial port
-conn_physical = libmav.TCPClient('/dev/ttyUSB0', 14550)
+conn_physical = libmav.Serial('/dev/ttyUSB0')
 conn_runtime = libmav.NetworkRuntime(self.message_set, heartbeat, client_physical)
 
 ```
 
 ## Install from source
 
 ### Prerequisites
@@ -113,8 +110,8 @@
 
 ```bash
 git clone --recursive https://github.com/Auterion/libmav-python.git
 pip install ./libmav-python
 ```
 
 With the `setup.py` file included in this project, the `pip install` command will
-invoke CMake and build the pybind11 module as specified in `CMakeLists.txt`.
+invoke CMake and build the pybind11 module as specified in `CMakeLists.txt`.
```

### Comparing `libmav-0.0.1/README.md` & `libmav-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+Metadata-Version: 2.1
+Name: libmav
+Version: 0.0.2
+Summary: A library for the MAVLink protocol
+Author: Auterion
+Author-email: success@auterion.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # Libmav Python
 
 Native python bindings for the [libmav](https://github.com/ThomasDebrunner/libmav) library.
+libmav-python is a runtime defined low-level MAVLink library. 
+
+In comparison to other python MAVLink libaries, it has certain advantages:
+
+- **Runtime defined message set.** No need to recompile on message set change or custom messages
+- **Implemented in C++.** Much faster than pure python
+- **Simple, pythonic API.** No need to learn a new API or asyncio, just use python
+
 
 ## Installation
 
 ```
 pip install libmav
 ```
 
@@ -22,15 +41,15 @@
         <message>
             ...
         </message>
     </messages>
 </mavlink>''')
 
 # Create a message from the message set
-message = self.message_set.create('MY_PROTOCOL_MESSAGE')
+message = message_set.create('MY_PROTOCOL_MESSAGE')
 
 # Set fields of the message individually
 message['my_numeric_field'] = 1
 message['my_char_array_field'] = 'Hello world'
 message['my_float_array_field'] = [1.0, 2.0, 3.0]
 message['my_int_array_field'] = [4, 5, 6]
 
@@ -80,15 +99,15 @@
 # This avoids the race condition between us sending and then waiting for reception
 expectation = connection.receive("PARAM_VALUE")
 connection.send(our_param_request_message)
 received_message = connection.receive(expectation, 1000)
 
 
 # Connect to a Serial port
-conn_physical = libmav.TCPClient('/dev/ttyUSB0', 14550)
+conn_physical = libmav.Serial('/dev/ttyUSB0')
 conn_runtime = libmav.NetworkRuntime(self.message_set, heartbeat, client_physical)
 
 ```
 
 ## Install from source
 
 ### Prerequisites
@@ -102,8 +121,8 @@
 
 ```bash
 git clone --recursive https://github.com/Auterion/libmav-python.git
 pip install ./libmav-python
 ```
 
 With the `setup.py` file included in this project, the `pip install` command will
-invoke CMake and build the pybind11 module as specified in `CMakeLists.txt`.
+invoke CMake and build the pybind11 module as specified in `CMakeLists.txt`.
```

### Comparing `libmav-0.0.1/libmav.egg-info/PKG-INFO` & `libmav-0.0.2/libmav.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: libmav
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for the MAVLink protocol
 Author: Auterion
 Author-email: success@auterion.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Libmav Python
 
 Native python bindings for the [libmav](https://github.com/ThomasDebrunner/libmav) library.
+libmav-python is a runtime defined low-level MAVLink library. 
+
+In comparison to other python MAVLink libaries, it has certain advantages:
+
+- **Runtime defined message set.** No need to recompile on message set change or custom messages
+- **Implemented in C++.** Much faster than pure python
+- **Simple, pythonic API.** No need to learn a new API or asyncio, just use python
+
 
 ## Installation
 
 ```
 pip install libmav
 ```
 
@@ -33,15 +41,15 @@
         <message>
             ...
         </message>
     </messages>
 </mavlink>''')
 
 # Create a message from the message set
-message = self.message_set.create('MY_PROTOCOL_MESSAGE')
+message = message_set.create('MY_PROTOCOL_MESSAGE')
 
 # Set fields of the message individually
 message['my_numeric_field'] = 1
 message['my_char_array_field'] = 'Hello world'
 message['my_float_array_field'] = [1.0, 2.0, 3.0]
 message['my_int_array_field'] = [4, 5, 6]
 
@@ -91,15 +99,15 @@
 # This avoids the race condition between us sending and then waiting for reception
 expectation = connection.receive("PARAM_VALUE")
 connection.send(our_param_request_message)
 received_message = connection.receive(expectation, 1000)
 
 
 # Connect to a Serial port
-conn_physical = libmav.TCPClient('/dev/ttyUSB0', 14550)
+conn_physical = libmav.Serial('/dev/ttyUSB0')
 conn_runtime = libmav.NetworkRuntime(self.message_set, heartbeat, client_physical)
 
 ```
 
 ## Install from source
 
 ### Prerequisites
```

### Comparing `libmav-0.0.1/libmav.egg-info/SOURCES.txt` & `libmav-0.0.2/libmav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/CMakeLists.txt` & `libmav-0.0.2/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/LICENSE` & `libmav-0.0.2/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/attr.h` & `libmav-0.0.2/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/buffer_info.h` & `libmav-0.0.2/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/cast.h` & `libmav-0.0.2/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/chrono.h` & `libmav-0.0.2/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/complex.h` & `libmav-0.0.2/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/class.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/common.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/descr.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/init.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/internals.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/type_caster_base.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/detail/typeid.h` & `libmav-0.0.2/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/eigen.h` & `libmav-0.0.2/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/embed.h` & `libmav-0.0.2/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/eval.h` & `libmav-0.0.2/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/functional.h` & `libmav-0.0.2/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/gil.h` & `libmav-0.0.2/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/iostream.h` & `libmav-0.0.2/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/numpy.h` & `libmav-0.0.2/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/operators.h` & `libmav-0.0.2/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/options.h` & `libmav-0.0.2/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/pybind11.h` & `libmav-0.0.2/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/pytypes.h` & `libmav-0.0.2/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/stl/filesystem.h` & `libmav-0.0.2/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/stl.h` & `libmav-0.0.2/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/include/pybind11/stl_bind.h` & `libmav-0.0.2/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tests/test_embed/CMakeLists.txt` & `libmav-0.0.2/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/FindCatch.cmake` & `libmav-0.0.2/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/FindEigen3.cmake` & `libmav-0.0.2/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/FindPythonLibsNew.cmake` & `libmav-0.0.2/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/check-style.sh` & `libmav-0.0.2/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/cmake_uninstall.cmake.in` & `libmav-0.0.2/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/libsize.py` & `libmav-0.0.2/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/make_changelog.py` & `libmav-0.0.2/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/pybind11Common.cmake` & `libmav-0.0.2/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/pybind11Config.cmake.in` & `libmav-0.0.2/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/pybind11NewTools.cmake` & `libmav-0.0.2/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/pybind11Tools.cmake` & `libmav-0.0.2/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/setup_global.py.in` & `libmav-0.0.2/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pybind11/tools/setup_main.py.in` & `libmav-0.0.2/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/pyproject.toml` & `libmav-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/setup.py` & `libmav-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_Connection.cpp` & `libmav-0.0.2/src/bind_Connection.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                     py::arg("component_id") = mav::ANY_ID)
             .def("receive",
                  [](Connection& self, const _ExpectationWrapper& expectation, int timeout_ms) {
                      return self.receive(expectation.expectation, timeout_ms);
                  }, py::arg("expectation"), py::arg("timeout_ms") = -1)
             .def("receive",
                  py::overload_cast<const std::string&, int, int, int>(&Connection::receive),
-                    py::arg("message_name"), py::arg("source_id") = mav::ANY_ID,
-                    py::arg("component_id") = mav::ANY_ID, py::arg("timeout_ms") = -1)
+                    py::arg("message_name"), py::arg("source_id"),
+                    py::arg("component_id"), py::arg("timeout_ms") = -1)
             .def("receive", py::overload_cast<const std::string&, int>(&Connection::receive),
                     py::arg("message_name"), py::arg("timeout_ms") = -1)
             .def("receive", py::overload_cast<int, int, int, int>(&Connection::receive),
                     py::arg("message_id"), py::arg("source_id") = mav::ANY_ID,
                     py::arg("component_id") = mav::ANY_ID, py::arg("timeout_ms") = -1)
             .def("receive", py::overload_cast<int, int>(&Connection::receive),
                     py::arg("message_id"), py::arg("timeout_ms") = -1);
```

### Comparing `libmav-0.0.1/src/bind_Message.cpp` & `libmav-0.0.2/src/bind_Message.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_MessageDefinition.cpp` & `libmav-0.0.2/src/bind_MessageDefinition.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_MessageSet.cpp` & `libmav-0.0.2/src/bind_MessageSet.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_NetworkRuntime.cpp` & `libmav-0.0.2/src/bind_NetworkRuntime.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_PhysicalNetwork.cpp` & `libmav-0.0.2/src/bind_PhysicalNetwork.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_main.cpp` & `libmav-0.0.2/src/bind_main.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/bind_utils.cpp` & `libmav-0.0.2/src/bind_utils.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/CMakeLists.txt` & `libmav-0.0.2/src/libmav/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 cmake_minimum_required(VERSION 3.20)
 project(mav VERSION 0.1.0 DESCRIPTION "mavlink library with a runtime defined message set")
 
 include(GNUInstallDirs)
+
+set(THREADS_PREFER_PTHREAD_FLAG ON)
 find_package(Threads REQUIRED)
 
 set(CMAKE_CXX_STANDARD 17)
 
 add_library(mav INTERFACE)
 
 target_include_directories(
@@ -42,9 +44,12 @@
         DESTINATION ${CMAKE_INSTALL_DATAROOTDIR}/${PROJECT_NAME}/cmake)
 
 install(DIRECTORY ${PROJECT_SOURCE_DIR}/include/mav DESTINATION include)
 
 set(CPACK_RESOURCE_FILE_LICENSE "${PROJECT_SOURCE_DIR}/LICENSE")
 
 include(CPack)
+include(CTest)
 
-add_subdirectory(tests)
+if(BUILD_TESTING)
+    add_subdirectory(tests)
+endif()
```

### Comparing `libmav-0.0.1/src/libmav/LICENSE` & `libmav-0.0.2/src/libmav/LICENSE`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/README.md` & `libmav-0.0.2/src/libmav/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 networks and several of the mavlink internal protocols.
 
 ### What's the advantage?
 
 There are many mavlink libraries out there. The main advantages of this library over others are:
 
 - **Runtime defined message set**. No need to recompile on message set change
-- **Native python bindings** for C++ code. Faster than pure python. *Coming soon*
+- [**Native python bindings**](https://github.com/Auterion/libmav-python) for C++ code. Faster than pure python.
 - **Header-only, no dependencies**, C++ 17, >90% test coverage
 
 ## How to install
 
 There are several ways to get it:
 
 Install globally on your system
 ```bash
-cmake .
-sudo make install
+cmake -Bbuild -S.
+sudo cmake --build build --target install
 ```
 Since the library is header only, you only need the library on the build system.
 
 You can also include the library as a submodule in your project.
 
 ## Getting started
 
@@ -80,20 +80,20 @@
 
 
 ### Connecting to a Network
 
 Libmav has classes for the following protocols:
 - Serial
 - TCP Client
-- TCP Server *Coming soon*
+- TCP Server
 - UDP Client
 - UDP Server
 
 Libmav does not do any threading, except for the `NetworkRuntime` class.
-The `NetworkRuntime` class spawns a two threads. One two drive the receive
+The `NetworkRuntime` class spawns two threads. One to drive the receive
 loop and one to drive the HEARTBEAT transmission and timeout handling.
 
 ```C++
 // Create interface for physical network
 auto physical = libmav::TCPClient("<ip>", 14550);
 
 auto heartbeat_message = message_set.create("HEARTBEAT");
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/BuiltInMessages.h` & `libmav-0.0.2/src/libmav/include/mav/BuiltInMessages.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/Connection.h` & `libmav-0.0.2/src/libmav/include/mav/Connection.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/Message.h` & `libmav-0.0.2/src/libmav/include/mav/Message.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/MessageDefinition.h` & `libmav-0.0.2/src/libmav/include/mav/MessageDefinition.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/MessageFieldIterator.h` & `libmav-0.0.2/src/libmav/include/mav/MessageFieldIterator.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/MessageSet.h` & `libmav-0.0.2/src/libmav/include/mav/MessageSet.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/Network.h` & `libmav-0.0.2/src/libmav/include/mav/Network.h`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
  * POSSIBILITY OF SUCH DAMAGE.
  * 
  ****************************************************************************/
 
 #ifndef MAV_NETWORK_H
 #define MAV_NETWORK_H
 
+#include <cstring>
 #include <list>
 #include <thread>
 #include <array>
 #include <thread>
 #include <atomic>
 #include <iostream>
 #include <memory>
@@ -48,16 +49,24 @@
 #include "utils.h"
 
 namespace mav {
 
 
     class NetworkError : public std::runtime_error {
     public:
-        explicit NetworkError(const char* message) : std::runtime_error(message) {}
+        explicit NetworkError(const char* message, int errno_num = 0)
+                : std::runtime_error(
+                std::string(message) + (errno_num != 0 ? (std::string(" (") + strerror(errno_num) + ")") : "")),
+                  _errno_num(errno_num)
+        {}
         explicit NetworkError(const std::string& message) : std::runtime_error(message) {}
+
+        [[nodiscard]] int errnoNum() const { return _errno_num; }
+    private:
+        int _errno_num{-1};
     };
 
     class NetworkClosed : public NetworkError {
     public:
         explicit NetworkClosed(const char* message) : NetworkError(message) {}
         explicit NetworkClosed(const std::string& message) : NetworkError(message) {}
     };
@@ -193,15 +202,22 @@
                         // we do not have a connection for this message, create one
                         auto connection = _addConnection(message.source());
                         connection->consumeMessageFromNetwork(message);
                     } else {
                         connection_entry->second->consumeMessageFromNetwork(message);
                     }
                 } catch (NetworkError &e) {
-                    _should_terminate.store(true);
+                    // A connection might be refused initially if the other side is not up yet (e.g. UDP client). Continue
+                    // and let the upper layers handle any timeouts. If it happens later on we still forward the error.
+                    if (e.errnoNum() == ECONNREFUSED) {
+                        // Wait a bit to ensure there's no busy loop
+                        std::this_thread::sleep_for(std::chrono::milliseconds(100));
+                    } else {
+                        _should_terminate.store(true);
+                    }
                     // Spread the network error to all connections
                     std::lock_guard<std::mutex> lock(_connections_mutex);
                     for (auto& connection : _connections) {
                         connection.second->consumeNetworkExceptionFromNetwork(std::make_exception_ptr(e));
                     }
                 } catch (NetworkInterfaceInterrupt &e) {
                     _should_terminate.store(true);
@@ -314,20 +330,20 @@
                     throw TimeoutException("Timeout while waiting for first connection");
                 }
             }
             return fut.get();
         }
 
         void setHeartbeatMessage(const Message &message) {
-            std::unique_lock<std::mutex> lock(_send_mutex);
+            std::lock_guard heartbeat_message_lock(_heartbeat_message_mutex);
             _heartbeat_message = message;
         }
 
         void clearHeartbeat() {
-            std::unique_lock<std::mutex> lock(_send_mutex);
+            std::lock_guard heartbeat_message_lock(_heartbeat_message_mutex);
             _heartbeat_message = std::nullopt;
         }
 
         void stop() {
             _interface.close();
             _should_terminate.store(true);
             if (_receive_thread.joinable()) {
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/Serial.h` & `libmav-0.0.2/src/libmav/include/mav/Serial.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/TCPClient.h` & `libmav-0.0.2/src/libmav/include/mav/TCPClient.h`

 * *Files 3% similar despite different names*

```diff
@@ -53,26 +53,26 @@
         ConnectionPartner _partner;
 
     public:
 
         TCPClient(const std::string& address, int port) {
             _socket = socket(AF_INET, SOCK_STREAM, 0);
             if (_socket < 0) {
-                throw NetworkError("Could not create socket");
+                throw NetworkError("Could not create socket", errno);
             }
             struct sockaddr_in server_address{};
             server_address.sin_family = AF_INET;
             server_address.sin_port = htons(port);
             server_address.sin_addr.s_addr = inet_addr(address.c_str());
 
             _partner = {server_address.sin_addr.s_addr, server_address.sin_port, false};
 
             if (connect(_socket, (struct sockaddr *) &server_address, sizeof(server_address)) < 0) {
                 ::close(_socket);
-                throw NetworkError("Could not connect to server");
+                throw NetworkError("Could not connect to server", errno);
             }
         }
 
         void stop() {
             _should_terminate.store(true);
             if (_socket >= 0) {
                 ::shutdown(_socket, SHUT_RDWR);
@@ -87,15 +87,15 @@
 
         ConnectionPartner receive(uint8_t *destination, uint32_t size) override {
             uint32_t received = 0;
             while (received < size && !_should_terminate.load()) {
                 auto ret = read(_socket, destination, size - received);
                 if (ret < 0) {
                     ::close(_socket);
-                    throw NetworkError("Could not read from socket");
+                    throw NetworkError("Could not read from socket", errno);
                 }
                 received += ret;
             }
             if (_should_terminate.load()) {
                 ::close(_socket);
                 throw NetworkInterfaceInterrupt();
             }
@@ -104,15 +104,15 @@
 
         void send(const uint8_t *data, uint32_t size, ConnectionPartner) override {
             uint32_t sent = 0;
             while (sent < size && !_should_terminate.load()) {
                 auto ret = write(_socket, data, size - sent);
                 if (ret < 0) {
                     ::close(_socket);
-                    throw NetworkError("Could not write to socket");
+                    throw NetworkError("Could not write to socket", errno);
                 }
                 sent += ret;
             }
             if (_should_terminate.load()) {
                 ::close(_socket);
                 throw NetworkInterfaceInterrupt();
             }
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/TCPServer.h` & `libmav-0.0.2/src/libmav/include/mav/TCPServer.h`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         void _handleNewConnection() {
             struct sockaddr_in client_address{};
             socklen_t client_address_length = sizeof(client_address);
             auto client_socket = accept(_master_socket, (struct sockaddr *) &client_address,
                                         &client_address_length);
             if (client_socket < 0) {
                 ::close(_master_socket);
-                throw NetworkError("Could not accept connection");
+                throw NetworkError("Could not accept connection", errno);
             }
             struct sockaddr_in address{};
             int addrlen = sizeof(address);
             getpeername(client_socket , (struct sockaddr*)&address, (socklen_t*)&addrlen);
             ConnectionPartner partner = {address.sin_addr.s_addr, address.sin_port, false};
             _fd_to_partner.insert({client_socket, partner});
             _partner_to_fd.insert({partner, client_socket});
@@ -110,35 +110,35 @@
             if (_master_socket < 0) {
                 throw NetworkError("Could not create socket: " + std::to_string(_master_socket));
             }
 
             // Mark socket as non-blocking
             if (fcntl(_master_socket, F_SETFL, O_NONBLOCK) < 0) {
                 ::close(_master_socket);
-                throw NetworkError("Could not set socket to non-blocking");
+                throw NetworkError("Could not set socket to non-blocking", errno);
             }
 
             const int enable = 1;
             if (setsockopt(_master_socket, SOL_SOCKET, SO_REUSEADDR, &enable, sizeof(int)) < 0) {
                 ::close(_master_socket);
-                throw NetworkError("Could not set socket options");
+                throw NetworkError("Could not set socket options", errno);
             }
             struct sockaddr_in server_address{};
             server_address.sin_family = AF_INET;
             server_address.sin_port = htons(port);
             server_address.sin_addr.s_addr = htonl(INADDR_ANY);
 
             if (bind(_master_socket, (struct sockaddr *) &server_address, sizeof(server_address)) < 0) {
                 ::close(_master_socket);
-                throw NetworkError("Could not bind socket");
+                throw NetworkError("Could not bind socket", errno);
             }
 
             if (listen(_master_socket, 32) < 0) {
                 ::close(_master_socket);
-                throw NetworkError("Could not listen on socket");
+                throw NetworkError("Could not listen on socket", errno);
             }
 
             _addFd(_master_socket, POLLIN);
         }
 
         void stop() {
             _should_terminate.store(true);
@@ -175,15 +175,15 @@
                 // check for activity on one of the sockets
                 auto poll_ret = poll(_poll_fds.data(), _poll_fds.size(), 1000);
                 if (poll_ret < 0) {
                     if (errno == EINTR) {
                         continue;
                     } else {
                         stop();
-                        throw NetworkError("poll error");
+                        throw NetworkError("poll error", errno);
                     }
                 } else if (poll_ret == 0) {
                     continue;
                 } else {
                     int socket_to_read_from = -1;
                     ConnectionPartner partner_to_read_from;
 
@@ -234,15 +234,15 @@
         }
 
         void _sendToSingleTarget(const uint8_t *data, uint32_t size, int partner_socket) {
             uint32_t sent = 0;
             while (sent < size && !_should_terminate.load()) {
                 auto ret = write(partner_socket, data, size - sent);
                 if (ret < 0) {
-                    throw NetworkError("Could not write to socket");
+                    throw NetworkError("Could not write to socket", errno);
                 }
                 sent += ret;
             }
             if (_should_terminate.load()) {
                 stop();
                 throw NetworkInterfaceInterrupt();
             }
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/UDPClient.h` & `libmav-0.0.2/src/libmav/include/mav/UDPClient.h`

 * *Files 2% similar despite different names*

```diff
@@ -60,38 +60,39 @@
         int _bytes_available = 0;
         ConnectionPartner _partner;
 
     public:
         UDPClient(const std::string &remote_address, int remote_port) {
             _socket = socket(AF_INET, SOCK_DGRAM, IPPROTO_UDP);
             if (_socket < 0) {
-                throw NetworkError("Could not create socket");
+                throw NetworkError("Could not create socket", errno);
             }
 
             _server_address.sin_family = AF_INET;
             _server_address.sin_port = htons(remote_port);
             _server_address.sin_addr.s_addr = inet_addr(remote_address.c_str());
 
             // connect to server
             if(connect(_socket, (struct sockaddr *)&_server_address, sizeof(_server_address)) < 0) {
-                throw NetworkError("UDP connect call failed");
+                throw NetworkError("UDP connect call failed", errno);
             }
 
             _partner = {
                     _server_address.sin_addr.s_addr,
                     _server_address.sin_port,
                     false
             };
         }
 
         void stop() {
             _should_terminate.store(true);
             if (_socket >= 0) {
                 ::shutdown(_socket, SHUT_RDWR);
                 ::close(_socket);
+                _socket = -1;
             }
         }
 
         void close() override {
             stop();
         }
 
@@ -99,15 +100,15 @@
             // Receive as many messages as needed to have enough bytes available (none if already enough bytes)
             while (_bytes_available < size && !_should_terminate.load()) {
                 // If there are residual bytes from last packet, but not enough for parsing new packet, clear out
                 _bytes_available = 0;
                 ssize_t ret = ::recvfrom(_socket, _rx_buffer.data(), RX_BUFFER_SIZE, 0,
                                          (struct sockaddr *) nullptr, nullptr);
                 if (ret < 0) {
-                    throw NetworkError("Could not receive from socket");
+                    throw NetworkError("Could not receive from socket", errno);
                 }
                 _bytes_available += static_cast<int>(ret);
             }
 
             if (_should_terminate.load()) {
                 throw NetworkInterfaceInterrupt();
             }
@@ -118,15 +119,16 @@
             return _partner;
         }
 
         void send(const uint8_t *data, uint32_t size, ConnectionPartner target) override {
             // no need to specify target here, as we called the udp connect function in constructor
             if (sendto(_socket, data, size, 0, (struct sockaddr *) nullptr, 0) < 0) {
                 ::close(_socket);
-                throw NetworkError("Could not send to socket");
+                _socket = -1;
+                throw NetworkError("Could not send to socket", errno);
             }
         }
 
         void markSyncing() override {
             // we're out of sync. The beginning of a packet was not the magic number we expected,
             // therefore, we can discard the rest of the packet and just receive another datagram.
             _bytes_available = 0;
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/UDPServer.h` & `libmav-0.0.2/src/libmav/include/mav/UDPServer.h`

 * *Files 3% similar despite different names*

```diff
@@ -59,24 +59,24 @@
         int _bytes_available = 0;
         ConnectionPartner _current_partner;
 
     public:
         UDPServer(int local_port, const std::string& local_address="0.0.0.0") {
             _socket = socket(AF_INET, SOCK_DGRAM, 0);
             if (_socket < 0) {
-                throw NetworkError("Could not create socket");
+                throw NetworkError("Could not create socket", errno);
             }
             struct sockaddr_in server_address{};
             server_address.sin_family = AF_INET;
             server_address.sin_port = htons(local_port);
             server_address.sin_addr.s_addr = inet_addr(local_address.c_str());
 
             if (bind(_socket, (struct sockaddr *) &server_address, sizeof(server_address)) < 0) {
                 ::close(_socket);
-                throw NetworkError("Could not bind to socket. (Address already in use?)");
+                throw NetworkError("Could not bind to socket", errno);
             }
         }
 
         void stop() const {
             _should_terminate.store(true);
             if (_socket >= 0) {
                 ::shutdown(_socket, SHUT_RDWR);
@@ -94,15 +94,15 @@
                 // If there are residual bytes from last packet, but not enough for parsing new packet, clear out
                 _bytes_available = 0;
                 struct sockaddr_in source_address{};
                 socklen_t source_address_length = sizeof(source_address);
                 ssize_t ret = ::recvfrom(_socket, _rx_buffer.data(), RX_BUFFER_SIZE, 0,
                                      (struct sockaddr*)&source_address, &source_address_length);
                 if (ret < 0) {
-                    throw NetworkError("Could not receive from socket");
+                    throw NetworkError("Could not receive from socket", errno);
                 }
                 _bytes_available += static_cast<int>(ret);
 
                 // make sure this remote is in the set of known remotes
                 _current_partner = {
                     source_address.sin_addr.s_addr,
                     source_address.sin_port,
@@ -128,15 +128,15 @@
             struct sockaddr_in server_address{};
             server_address.sin_family = AF_INET;
             server_address.sin_port = target.port();
             server_address.sin_addr.s_addr = target.address();
 
             if (sendto(_socket, data, size, 0, (struct sockaddr *) &server_address, sizeof(server_address)) < 0) {
                 ::close(_socket);
-                throw NetworkError("Could not send to socket");
+                throw NetworkError("Could not send to socket", errno);
             }
         }
 
         void markSyncing() override {
             // we're out of sync. The beginning of a packet was not the magic number we expected,
             // therefore, we can discard the rest of the packet and just receive another datagram.
             _bytes_available = 0;
```

### Comparing `libmav-0.0.1/src/libmav/include/mav/rapidxml/license.txt` & `libmav-0.0.2/src/libmav/include/mav/rapidxml/license.txt`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml.hpp` & `libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml.hpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_iterators.hpp` & `libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_iterators.hpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_print.hpp` & `libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_print.hpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/rapidxml/rapidxml_utils.hpp` & `libmav-0.0.2/src/libmav/include/mav/rapidxml/rapidxml_utils.hpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/include/mav/utils.h` & `libmav-0.0.2/src/libmav/include/mav/utils.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/Message.cpp` & `libmav-0.0.2/src/libmav/tests/Message.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/MessageDefinition.cpp` & `libmav-0.0.2/src/libmav/tests/MessageDefinition.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/MessageFieldIterator.cpp` & `libmav-0.0.2/src/libmav/tests/MessageFieldIterator.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/MessageSet.cpp` & `libmav-0.0.2/src/libmav/tests/MessageSet.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/Network.cpp` & `libmav-0.0.2/src/libmav/tests/Network.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/TCP.cpp` & `libmav-0.0.2/src/libmav/tests/TCP.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/UDP.cpp` & `libmav-0.0.2/src/libmav/tests/UDP.cpp`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/doctest.h` & `libmav-0.0.2/src/libmav/tests/doctest.h`

 * *Files identical despite different names*

### Comparing `libmav-0.0.1/src/libmav/tests/minimal.h` & `libmav-0.0.2/src/libmav/tests/minimal.h`

 * *Files identical despite different names*

